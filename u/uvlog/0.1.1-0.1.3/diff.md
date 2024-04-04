# Comparing `tmp/uvlog-0.1.1-py3-none-any.whl.zip` & `tmp/uvlog-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 13851 bytes, number of entries: 7
--rw-r--r--  2.0 unx      363 b- defN 24-Apr-01 20:38 uvlog/__init__.py
--rw-r--r--  2.0 unx    34859 b- defN 24-Apr-01 20:37 uvlog/uvlog.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7840 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      520 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/RECORD
-7 files, 44749 bytes uncompressed, 12937 bytes compressed:  71.1%
+Zip file size: 16302 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1119 b- defN 24-Apr-04 17:05 uvlog/__init__.py
+-rw-r--r--  2.0 unx     5448 b- defN 24-Apr-04 17:05 uvlog/formatters.py
+-rw-r--r--  2.0 unx     9844 b- defN 24-Apr-04 17:05 uvlog/handlers.py
+-rw-r--r--  2.0 unx    20197 b- defN 24-Apr-04 17:05 uvlog/uvlog.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9820 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      671 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/RECORD
+9 files, 48266 bytes uncompressed, 15164 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: uvlog/__init__.py
 Comment: 
 
+Filename: uvlog/formatters.py
+Comment: 
+
+Filename: uvlog/handlers.py
+Comment: 
+
 Filename: uvlog/uvlog.py
 Comment: 
 
-Filename: uvlog-0.1.1.dist-info/LICENSE
+Filename: uvlog-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: uvlog-0.1.1.dist-info/METADATA
+Filename: uvlog-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: uvlog-0.1.1.dist-info/WHEEL
+Filename: uvlog-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: uvlog-0.1.1.dist-info/top_level.txt
+Filename: uvlog-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: uvlog-0.1.1.dist-info/RECORD
+Filename: uvlog-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uvlog/__init__.py

```diff
@@ -1,17 +1,47 @@
 """Python logging utilities."""
 
 import atexit
+import logging
+from typing import Union, cast
 
+from uvlog.formatters import *
+from uvlog.handlers import *
 from uvlog.uvlog import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.1"
+__version__ = "0.1.3"
 
 add_formatter_type(TextFormatter)
 add_formatter_type(JSONFormatter)
 add_handler_type(StreamHandler)
-add_handler_type(QueueHandler)
+add_handler_type(QueueStreamHandler)
+
 configure(BASIC_CONFIG)
 atexit.register(clear)
+
+# compatibility with the standard library
+
+_root_logger = get_logger()
+debug = _root_logger.debug
+info = _root_logger.info
+warning = _root_logger.warning
+error = _root_logger.error
+critical = _root_logger.critical
+never = _root_logger.never
+getLogger = get_logger
+
+_level_to_name = {
+    logging.CRITICAL: "CRITICAL",
+    logging.ERROR: "ERROR",
+    logging.WARNING: "WARNING",
+    logging.INFO: "INFO",
+    logging.DEBUG: "DEBUG",
+}
+
+
+def basicConfig(level: Union[int, LevelName, None] = None):
+    if level is not None and isinstance(level, int):
+        level = cast(LevelName, _level_to_name[level])
+        _root_logger.set_level(level)
```

## uvlog/uvlog.py

```diff
@@ -1,158 +1,144 @@
 """Python logging utilities."""
 
-import io
 import logging
 import os
-import queue
 import sys
-import traceback
 from abc import abstractmethod
 from collections import ChainMap
 from contextvars import ContextVar  # noqa: pycharm bug?
 from dataclasses import dataclass, field
 from datetime import datetime
-from enum import Enum
-from json import dumps
 from random import random
-from pathlib import Path
-from threading import Thread
 from typing import (
     Any,
-    BinaryIO,
-    Callable,
-    ClassVar,
-    Collection,
+    Dict,
+    List,
     Literal,
     Mapping,
     Optional,
     Protocol,
+    Type,
     TypedDict,
     cast,
-    no_type_check,
-    Type,
-    Dict,
-    List,
 )
-from urllib.parse import urlparse
 from weakref import WeakValueDictionary
 
 __all__ = [
     "LOG_CONTEXT",
     "BASIC_CONFIG",
     "LogRecord",
     "Logger",
     "Handler",
     "Formatter",
-    "TextFormatter",
-    "JSONFormatter",
-    "StreamHandler",
-    "QueueHandler",
     "add_formatter_type",
     "add_handler_type",
     "set_logger_type",
     "add_handler",
     "add_formatter",
     "remove_handler",
     "get_logger",
     "configure",
     "clear",
-    "DEBUG",
-    "INFO",
-    "WARNING",
-    "ERROR",
-    "CRITICAL",
+    "LevelName",
+    "name_to_level",
 ]
 
 LOG_CONTEXT: ContextVar[Optional[Dict[str, Any]]] = ContextVar(
     "LOG_CONTEXT", default=None
 )  #: default log context
 
 
-class Stream(Enum):
-    """List of default log streams."""
-
-    stdout = sys.stdout.buffer
-    stderr = sys.stderr.buffer
-
-
-DEBUG = "DEBUG"
-INFO = "INFO"
-WARNING = "WARNING"
-ERROR = "ERROR"
-CRITICAL = "CRITICAL"
-
 _root_logger_name = ""
-_default_timespec = "seconds"
-_default_format = "{asctime} | {level} | {name} | {message} | {extra} | {ctx}"
 _formatter_types: Dict[str, Type["Formatter"]] = {}
 
 
 class _DictConfig(TypedDict, total=False):
     loggers: Dict[str, dict]
     handlers: Dict[str, dict]
     formatters: Dict[str, dict]
 
 
 BASIC_CONFIG: _DictConfig = {
     "loggers": {_root_logger_name: {}},
     "handlers": {
-        Stream.stderr.name: {},
-        Stream.stdout.name: {},
+        "stderr": {},
+        "stdout": {},
     },
     "formatters": {
         "text": {"class": "TextFormatter"},
         "json": {"class": "JSONFormatter"},
     },
 }  #: default log configuration
 
-_LevelName = Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+LevelName = Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL", "NEVER"]
 _handler_types: Dict[str, Type["Handler"]] = {}
 _handlers: Dict[str, "Handler"] = {}
 _formatters: Dict[str, "Formatter"] = {}
 _loggers_persistent: Dict[str, "Logger"] = {}
 _loggers_temp: WeakValueDictionary = WeakValueDictionary()
 _loggers: ChainMap = ChainMap(_loggers_persistent, _loggers_temp)
-_name_to_level: Dict[_LevelName, int] = {
+name_to_level: Dict[LevelName, int] = {
     "NOTSET": logging.NOTSET,
     "DEBUG": logging.DEBUG,
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
+    "NEVER": logging.CRITICAL + 100,
 }
 
 
 @dataclass
 class LogRecord:
     """Log record object.
 
     A log record object is created when a log method of a logger is called.
     """
 
-    __slots__ = ('name', 'level', 'levelno', 'asctime', 'filename', 'lineno', 'func', 'message', 'exc_info', 'extra', 'ctx')
+    __slots__ = (
+        "name",
+        "level",
+        "levelno",
+        "asctime",
+        "filename",
+        "lineno",
+        "func",
+        "message",
+        "exc_info",
+        "args",
+        "extra",
+        "ctx",
+    )
 
     name: str
     """Logger name"""
 
-    level: _LevelName
+    level: LevelName
     """Log record level name"""
 
     levelno: int
     """Log record level number"""
 
     asctime: datetime
     """Timestamp of record creation"""
 
     message: str
     """Log message"""
 
     exc_info: Optional[Exception]
     """Exception (if any)"""
 
+    args: Optional[tuple]
+    """Log extra information provided as positional arguments.
+    
+    This attribute is left only for compatibility reasons. It's better to use keyword arguments and `extra`
+    attribute instead.
+    """
+
     extra: Optional[Mapping[str, Any]]
     """Log extra information provided in kwargs"""
 
     ctx: Optional[Mapping[str, Any]]
     """Log contextual information"""
 
     filename: Optional[str]
@@ -184,15 +170,15 @@
     It's a protocol class, i.e. one doesn't need to inherit from it to create a valid handler.
     """
 
     @abstractmethod
     def handle(self, record: LogRecord, /) -> None: ...
 
     @abstractmethod
-    def set_level(self, level: _LevelName, /) -> None: ...
+    def set_level(self, level: LevelName, /) -> None: ...
 
     @abstractmethod
     def set_formatter(self, fmt: Formatter, /) -> None: ...
 
     @abstractmethod
     def set_destination(self, dest: str, /) -> None:
         """Set a handler destination.
@@ -233,19 +219,15 @@
 
 def add_formatter(name: str, formatter: Formatter, /) -> None:
     _formatters[name] = formatter
 
 
 def add_handler(destination: str, handler: Handler, /) -> None:
     if destination in _handlers:
-        raise ValueError(
-            f"handler already exists for this destination: {destination}\n\n"
-            f"Fix: ensure you don't have two handlers with the same destination, or use "
-            f"`uvlog.remove_handler(<dest>)` method to remove a conflicting handler"
-        )
+        remove_handler(destination)
     _handlers[destination] = handler
 
 
 def remove_handler(destination: str, /) -> None:
     handler = _handlers.pop(destination, None)
     if handler is not None:
         handler.close()
@@ -267,15 +249,15 @@
         logger.error('error happened', exc_info=Exception())
 
     """
 
     name: str
     """Logger name"""
 
-    level: _LevelName = "INFO"
+    level: LevelName = "INFO"
     """Logging level"""
 
     handlers: List[Handler] = field(default_factory=list)
     """List of attached log handlers"""
 
     sample_rate: float = 1.0
     """Log records sample rate which determines a probability at which a record should be sampled.
@@ -298,21 +280,27 @@
     capture_trace: bool = False
     """Capture traceback for each call such as line numbers, file names etc. — may affect performance"""
 
     _levelno: int = field(init=False, default=0)
     _parent: Optional["Logger"] = field(init=False, default=None)
 
     def __post_init__(self) -> None:
-        self._levelno = _name_to_level[self.level]
-        self.sample_rate = min(max(0.0, self.sample_rate), 1.0)
+        self._levelno = name_to_level[self.level]
 
-    def set_level(self, level: _LevelName, /) -> None:
-        self._levelno = _name_to_level[level]
+    def set_level(self, level: LevelName, /) -> None:
+        self._levelno = name_to_level[level]
         self.level = level
 
+    def getChild(self, name: str, /) -> "Logger":
+        """Get or create a child logger.
+
+        This is a compatibility wrapper around :py:meth:`~uvlog.uvlog.Logger.get_child`. Use that method instead.
+        """
+        return self.get_child(name)
+
     def get_child(self, name: str, /, *, persistent: bool = False) -> "Logger":
         """Get or create a child logger inheriting all the logger settings.
 
         .. attention::
 
             Note that by default a new logger is not *persistent*, i.e. it will be eventually garbage collected if
             there are no live references to it.
@@ -336,192 +324,166 @@
         child_logger._parent = self
         if persistent:
             _loggers_persistent[name] = child_logger
         else:
             _loggers_temp[name] = child_logger
         return child_logger
 
-    def critical(
+    def never(
         self,
         msg: str,
         /,
+        *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
-        if self._levelno > logging.CRITICAL:
-            return
         ctx = self.context.get()
-        if ctx and self.sample_rate < 1:
+        if ctx:
             ctx["_sample"] = True
-        fn, lno, func, _ = (
-            _find_caller(stack_info, stacklevel)
-            if self.capture_trace
-            else (None, None, None, None)
-        )
-        record = LogRecord(
-            self.name,
-            "CRITICAL",
-            logging.CRITICAL,
-            datetime.now(),
-            msg.format_map(kws),
+        self._log(
+            "NEVER",
+            name_to_level["NEVER"],
+            msg,
             exc_info,
-            kws if kws else None,
+            stack_info,
+            stacklevel,
             ctx,
-            fn,
-            func,
-            lno,
+            args,
+            kws,
         )
-        for handler in self.handlers:
-            handler.handle(record)
 
-    def error(
+    def critical(
         self,
         msg: str,
         /,
+        *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
-        if self._levelno > logging.ERROR:
+        levelno = name_to_level["CRITICAL"]
+        if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx and self.sample_rate < 1:
+        if ctx:
             ctx["_sample"] = True
-        fn, lno, func, _ = (
-            _find_caller(stack_info, stacklevel)
-            if self.capture_trace
-            else (None, None, None, None)
+        self._log(
+            "CRITICAL", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
-        record = LogRecord(
-            self.name,
-            "ERROR",
-            logging.ERROR,
-            datetime.now(),
-            msg.format_map(kws),
-            exc_info,
-            kws if kws else None,
-            ctx,
-            fn,
-            func,
-            lno,
+
+    def error(
+        self,
+        msg: str,
+        /,
+        *args,
+        exc_info: Optional[Exception] = None,
+        stack_info=None,
+        stacklevel=1,
+        **kws,
+    ) -> None:
+        levelno = name_to_level["ERROR"]
+        if self._levelno > levelno:
+            return
+        ctx = self.context.get()
+        if ctx:
+            ctx["_sample"] = True
+        self._log(
+            "ERROR", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
-        for handler in self.handlers:
-            handler.handle(record)
 
     def warning(
         self,
         msg: str,
         /,
+        *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
-        if self._levelno > logging.WARNING:
+        levelno = name_to_level["WARNING"]
+        if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx and self.sample_rate < 1:
+        if ctx:
             ctx["_sample"] = True
-        fn, lno, func, _ = (
-            _find_caller(stack_info, stacklevel)
-            if self.capture_trace
-            else (None, None, None, None)
+        self._log(
+            "WARNING", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
-        record = LogRecord(
-            self.name,
-            "WARNING",
-            logging.WARNING,
-            datetime.now(),
-            msg.format_map(kws),
-            exc_info,
-            kws if kws else None,
-            ctx,
-            fn,
-            func,
-            lno,
-        )
-        for handler in self.handlers:
-            handler.handle(record)
 
     def info(
         self,
         msg: str,
         /,
+        *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
-        if self._levelno > logging.INFO:
+        levelno = name_to_level["INFO"]
+        if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx and self.sample_rate < 1:
-            _sample = ctx.get("_sample")
-            if _sample is None:
-                _sample = random() < self.sample_rate
-                if self.sample_propagate:
-                    ctx["_sample"] = _sample
-            if not _sample:
+        if ctx and self.sample_rate < 1.0:
+            if not self._sample(ctx):
                 return
-        fn, lno, func, _ = (
-            _find_caller(stack_info, stacklevel)
-            if self.capture_trace
-            else (None, None, None, None)
-        )
-        record = LogRecord(
-            self.name,
-            "INFO",
-            logging.INFO,
-            datetime.now(),
-            msg.format_map(kws),
-            exc_info,
-            kws if kws else None,
-            ctx,
-            fn,
-            func,
-            lno,
+        self._log(
+            "INFO", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
-        for handler in self.handlers:
-            handler.handle(record)
 
     def debug(
         self,
         msg: str,
         /,
+        *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
-        if self._levelno > logging.DEBUG:
+        levelno = name_to_level["DEBUG"]
+        if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx and self.sample_rate < 1:
-            _sample = ctx.get("_sample")
-            if _sample is None:
-                _sample = random() < self.sample_rate
-                if self.sample_propagate:
-                    ctx["_sample"] = _sample
-            if not _sample:
+        if ctx and self.sample_rate < 1.0:
+            if not self._sample(ctx):
                 return
+        self._log(
+            "DEBUG", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
+        )
+
+    def _sample(self, ctx: dict, /) -> bool:
+        if not self.sample_propagate:
+            return random() < self.sample_rate
+        _sample = cast(bool, ctx.get("_sample"))
+        if _sample is None:
+            _sample = random() < self.sample_rate
+            ctx["_sample"] = _sample
+        return _sample
+
+    def _log(
+        self, level, levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws, /
+    ) -> None:
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
-            "DEBUG",
-            logging.DEBUG,
+            level,
+            levelno,
             datetime.now(),
-            msg.format_map(kws),
+            msg.format_map(kws) if kws else msg,
             exc_info,
+            args if args else None,
             kws if kws else None,
             ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
@@ -560,29 +522,17 @@
     parent = _loggers[_root_logger_name]
     for parent_name in split_name[:-1]:
         parent = parent.get_child(parent_name, persistent=persistent)
     logger = parent.get_child(split_name[-1], persistent=persistent)
     return logger
 
 
-def _dumps_default(obj: Any) -> str:
-    if isinstance(obj, datetime):
-        return obj.isoformat()
-    return str(obj)
-
-
-def _dumps_bytes(obj) -> bytes:
-    # patched standard json dumps method to dump bytestring
-    # in reality you'd rather want to use a faster json library like `orjson` etc.
-    return dumps(obj, default=_dumps_default).encode("utf-8")
-
-
 # python traceback extraction methods - a ripoff of the standard logging library method
 
-_srcfile = os.path.normcase(_dumps_bytes.__code__.co_filename)
+_srcfile = os.path.normcase(get_logger.__code__.co_filename)
 
 
 def _find_caller(stack_info=None, stacklevel: int = 1):
     """Find the stack frame of the caller so that we can note the source file name, line number, function name."""
     f = sys._getframe(1)  # noqa
     if f is None:
         return "(unknown file)", 0, "(unknown function)", None
@@ -597,427 +547,52 @@
         )
         if not is_internal_frame:
             stacklevel -= 1
     co = f.f_code
     return co.co_filename, f.f_lineno, co.co_name, None
 
 
-@dataclass
-class TextFormatter:
-    """Text log formatter.
-
-    Creates human-readable log output.
-
-    Formatter settings can be set directly.
-
-    .. code-block:: python
-
-        _formatter = TextFormatter()
-        _formatter.timestamp_separator = ' '
-
-    """
-
-    timespec: str = field(init=False, default=_default_timespec)
-    """Precision for ISO timestamps,
-    see `datetime.isoformat() <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_"""
-
-    timestamp_separator: str = field(init=False, default="T")
-    """Timestamp separator for ISO timestamps,
-    see `datetime.isoformat() <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_"""
-
-    format: str = field(init=False, default=_default_format)
-    """Log record format, a python f-string,
-    the available keys can be seen in :py:class:`~uvlog.LogRecord` type
-    """
-
-    def format_record(self, record: LogRecord, /) -> bytes:
-        message = self.format.format_map(
-            {
-                "asctime": record.asctime.isoformat(
-                    timespec=self.timespec, sep=self.timestamp_separator
-                ),
-                "level": record.level,
-                "name": record.name,
-                "message": record.message,
-                "filename": record.filename,
-                "func": record.func,
-                "lineno": record.lineno,
-                "extra": record.extra,
-                "ctx": record.ctx,
-            }
-        )
-        if record.exc_info is not None:
-            exc_info = record.exc_info
-            message += "\n" + self._format_exc(
-                type(exc_info), exc_info, exc_info.__traceback__
-            )
-        return message.encode("utf-8")
-
-    @staticmethod
-    def _format_exc(error_cls, exc, stack, /) -> str:
-        sio = io.StringIO()
-        traceback.print_exception(error_cls, exc, stack, None, sio)
-        s = sio.getvalue()
-        sio.close()
-        if s[-1:] == "\n":
-            s = s[:-1]
-        return s
-
-    def __str__(self):
-        return f"<{self.__class__.__name__}>"
-
-
-@dataclass
-class JSONFormatter:
-    """JSON log formatter.
-
-    To change the default `dumps` function assign it to the class attribute:
-
-    .. code-block:: python
-
-        import orjson
-
-        JSONFormatter.serializer = orjson.dumps
-
-    Formatter settings can be set directly.
-
-    .. code-block:: python
-
-        _formatter = JSONFormatter()
-        _formatter.exc_pass_locals = True
-
-    """
-
-    serializer: ClassVar[Callable[[Any], bytes]] = field(
-        init=False, default=_dumps_bytes
-    )
-    """Serializer function - a class attribute"""
-
-    keys: Collection[str] = field(
-        init=False,
-        default=(
-            "name",
-            "level",
-            "asctime",
-            "message",
-            "exc_info",
-            "extra",
-            "ctx",
-            "filename",
-            "lineno",
-            "func",
-        ),
-    )
-    """List of serialized log record keys,
-    the available keys can be seen in :py:class:`~uvlog.LogRecord` type"""
-
-    exc_pass_locals: bool = field(init=False, default=False)
-    """Pass locals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
-
-    exc_pass_globals: bool = field(init=False, default=False)
-    """Pass globals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
-
-    def __post_init__(self):
-        self.keys = set(self.keys)
-
-    def format_record(self, record: LogRecord, /) -> bytes:
-        data = {
-            k: getattr(record, k) for k in self.keys if getattr(record, k) is not None
-        }
-        exc_info = cast(Exception, data.pop("exc_info", None))
-        if exc_info and "exc_info" in self.keys:
-            error_cls, exc, _ = type(exc_info), exc_info, exc_info.__traceback__
-            if hasattr(exc, "serialize"):
-                data["exc_info"] = exc.serialize()
-            else:
-                data["exc_info"] = {
-                    "message": str(exc),
-                    "type": error_cls.__name__,
-                    "data": exc.__dict__,
-                }
-                if exc.__traceback__:
-                    frame = exc.__traceback__.tb_frame
-                    data["exc_info"]["traceback"] = tb = {
-                        "lineno": frame.f_lineno,
-                        "func": frame.f_code.co_name,
-                    }
-                    if self.exc_pass_locals:
-                        tb["locals"] = frame.f_locals
-                    if self.exc_pass_globals:
-                        tb["globals"] = frame.f_globals
-
-        return self.__class__.serializer(data)
-
-    def __str__(self):
-        return f"<{self.__class__.__name__}>"
-
-
-@dataclass
-class StreamHandler:
-    """Logging handler.
-
-    A simple stream handler which immediately writes a log record to the write buffer. It provides the best performance.
-    However, in server applications you may want to use `uvlog.QueueStreamLogger`
-    to ensure your code is not blocking due to intensive logging.
-    """
-
-    terminator: ClassVar[bytes] = b"\n"
-    """Delimiter between log records"""
-
-    _level: _LevelName = field(init=False, default="DEBUG")
-    _dest: str = field(init=False, default=Stream.stderr.name)
-    _formatter: Formatter = field(default_factory=TextFormatter)
-    _levelno: int = field(init=False, default=0)
-    _stream: Optional[BinaryIO] = field(init=False, default=None)
-
-    def __post_init__(self):
-        self._levelno = _name_to_level[self._level]
-        self._stream = None
-
-    def handle(self, record: LogRecord, /) -> None:
-        """Immediately write a log record to the write buffer."""
-        if record.levelno < self._levelno:
-            return
-        if self._stream is None:
-            self._stream = self._open_stream()
-        record_bytes = self._formatter.format_record(record)
-        try:
-            self._stream.write(record_bytes + self.terminator)
-        except Exception:  # noqa: acceptable
-            self._handle_error(record_bytes)
-
-    def set_level(self, level: _LevelName, /) -> None:
-        self._level = level
-        self._levelno = _name_to_level[level]
-
-    def set_formatter(self, formatter: Formatter, /) -> None:
-        self._formatter = formatter
-
-    def set_destination(self, dest: str, /) -> None:
-        """Set log destination (file stream).
-
-        Pre-configured destinations are: 'stdout' and 'stderr'.
-
-        Both plain and URL file formats are acceptable and normalized into a path string:
-
-        - logs.txt - relative path
-        - /logs.txt - absolute path
-        - file:///logs.txt - absolute path in file URL format
-        """
-        if dest not in (Stream.stdout.name, Stream.stderr.name):
-            _path = Path(urlparse(dest).path)
-            _path.parent.mkdir(parents=True, exist_ok=True)
-            _path.touch(exist_ok=True)
-        remove_handler(dest)
-        add_handler(dest, self)
-        self._dest = dest
-        self._stream = None
-
-    def close(self) -> None:
-        """Close the handler including all connections to its destination.
-
-        This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
-        """
-        if self._stream and not self._stream.closed:
-            self._stream.flush()
-            if self._stream not in (sys.stderr.buffer, sys.stdout.buffer):
-                self._stream.close()
-        self._stream = None
-
-    def _open_stream(self) -> BinaryIO:
-        """Open a file stream."""
-        if self._dest == Stream.stderr.name:
-            return Stream.stderr.value
-        elif self._dest == Stream.stdout.name:
-            return Stream.stdout.value
-        else:
-            return open(self._dest, "ab")
-
-    @staticmethod
-    @no_type_check
-    def _handle_error(message: bytes, /) -> None:
-        """Handle an error which occurs during an emit() call.
-
-        This method is a loose ripoff of the standard python logging error handling mechanism.
-        """
-        _, exc, tb = sys.exc_info()
-        try:
-            sys.stderr.write("--- Logging error ---\n")
-            traceback.print_exception(
-                exc, limit=None, file=sys.stderr, value=exc, tb=tb
-            )
-            sys.stderr.write("Call stack:\n")
-            frame = exc.__traceback__.tb_frame
-            while frame:
-                frame = frame.f_back
-            if frame:
-                traceback.print_stack(frame, file=sys.stderr)
-            try:
-                sys.stderr.write(f"Message: {message}\n")
-            except RecursionError:
-                raise
-            except Exception:  # noqa: acceptable
-                sys.stderr.write(
-                    "Unable to print the message and arguments"
-                    " - possible formatting error.\nUse the"
-                    " traceback above to help find the error.\n"
-                )
-        except OSError:
-            pass
-        finally:
-            del exc
-
-    def __str__(self) -> str:
-        return f"<{self.__class__.__name__}: {self._dest} / {self._formatter}>"
-
-
-@dataclass
-class QueueHandler(StreamHandler):
-    """Logging handler with an internal queue.
-
-    This handler uses a queue and a separate thread providing at least some concurrency during intensive logging
-    workload. It has a worse overall performance than :py:class:`~uvlog.StreamHandler` but may be beneficial if you have
-    concurrent code such as a server application.
-
-    You may want to set :py:attr:`~uvlog.QueueHandler.queue_size`
-    to some reasonable value considering your application workload.
-
-    The handler uses a separate thread to write logs to the buffer via the :py:meth:`~uvlog.QueueHandler.write_loop`
-    method. Note that this handler doesn't use any internal locks,
-    because it's expected by design that each handler has its own destination.
-    """
-
-    _sentinel = None
-
-    queue_size: int = -1
-    """Log queue size, infinite by default"""
-
-    batch_size: int = 50
-    """Maximum number of log records to concatenate and write at once,
-    consider setting it so an average batch would be ~ tens of KBs"""
-
-    _write_queue: queue.Queue = field(default_factory=queue.Queue)
-    _thread: Optional[Thread] = field(default=None)
-
-    def __post_init__(self):
-        self._levelno = _name_to_level[self._level]
-        self._write_queue.maxsize = self.queue_size
-        self._stream = None
-        self._thread = None
-
-    def handle(self, record: LogRecord, /) -> None:
-        """Put a log record to the write queue."""
-        if record.levelno < self._levelno:
-            return
-        if self._thread is None:
-            self._thread = self._open_thread()
-        self._write_queue.put(record)
-
-    def _open_thread(self) -> Thread:
-        self._write_queue.maxsize = self.queue_size
-        thread = Thread(
-            target=self.write_loop, name=f"{self} _write", args=(), daemon=True
-        )
-        thread.start()
-        return thread
-
-    def close(self) -> None:
-        """Close the handler including all connections to its destination.
-
-        This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
-        """
-        self._write_queue.put(self._sentinel)
-        if self._thread is not None:
-            self._thread.join()
-            self._thread = None
-        # just in case the stream is not closed, however it should be closed when existing the `_write` method
-        StreamHandler.close(self)
-
-    def write_loop(self) -> None:
-        """Write logs from the queue to the stream.
-
-        This method is executed in a separate thread.
-        """
-        _queue = self._write_queue
-        _queue.maxsize = self.queue_size
-        _sentinel = self._sentinel
-        _formatter = self._formatter
-        _batch_size = self.batch_size
-        self._stream = _stream = self._open_stream()
-        formatted_records: List[bytes] = []
-        while 1:
-            if _queue.qsize():
-                records = [_queue.get(block=True)]
-            else:
-                records = [
-                    _queue.get_nowait() for _ in range(min(_batch_size, _queue.qsize()))
-                ]
-            for record in records:
-                if record is _sentinel:
-                    self.write(_stream, _queue, formatted_records)
-                    StreamHandler.close(self)
-                    return
-
-                formatted_records.append(_formatter.format_record(record))
-
-            self.write(_stream, _queue, formatted_records)
-            formatted_records.clear()
-
-    def write(
-        self, _stream: BinaryIO, _queue: queue.Queue, formatted_records: List[bytes], /
-    ) -> None:
-        if not formatted_records:
-            return
-        try:
-            formatted_records.append(b"")
-            _stream.write(self.terminator.join(formatted_records))
-        except Exception:  # noqa: acdceptable
-            self._handle_error(formatted_records[0])
-        finally:
-            for _ in range(len(formatted_records) - 1):
-                _queue.task_done()
-
-
 def _merge_dicts(from_dict: dict, to_dict: dict) -> dict:
     _new_dict = {**from_dict}
     for key, value in to_dict.items():
-        if key in _new_dict and type(value) is dict:
+        if key in _new_dict and isinstance(value, dict):
             _new_dict[key] = _merge_dicts(_new_dict[key], value)
         else:
             _new_dict[key] = value
     return _new_dict
 
 
 def _configure_formatter(name: str, params: dict, /) -> None:
-    cls = _formatter_types[params.pop("class", TextFormatter.__name__)]
+    cls = _formatter_types[params.pop("class", "TextFormatter")]
     _formatter = cls()
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_formatter, key, value)
     _formatters[name] = _formatter
 
 
 def _configure_handler(dest: str, params: dict, /) -> None:
-    cls_name = params.pop("class", StreamHandler.__name__)
+    cls_name = params.pop("class", "StreamHandler")
     _handler = _handler_types[cls_name]()
     _handler.set_destination(dest)
     formatter_name = params.pop("formatter", "text")
     _handler.set_formatter(_formatters[formatter_name])
-    level: _LevelName = cast(_LevelName, params.pop("level", "DEBUG"))
+    level: LevelName = cast(LevelName, params.pop("level", "DEBUG"))
     _handler.set_level(level)
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_handler, key, value)
+    _handlers[dest] = _handler
 
 
 def _configure_logger(name: str, params: dict, context_var: ContextVar, /) -> None:
     _logger = get_logger(name, persistent=True)
-    handler_names = params.pop("handlers", [Stream.stderr.name])
+    handler_names = params.pop("handlers", ["stderr"])
     _logger.handlers = [_handlers[handler_name] for handler_name in handler_names]
-    level: _LevelName = cast(_LevelName, params.pop("level", "INFO"))
+    level: LevelName = cast(LevelName, params.pop("level", "INFO"))
     _logger.set_level(level)
     _logger.context = context_var
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_logger, key, value)
```

## Comparing `uvlog-0.1.1.dist-info/LICENSE` & `uvlog-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uvlog-0.1.1.dist-info/METADATA` & `uvlog-0.1.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: uvlog
-Version: 0.1.1
+Version: 0.1.3
 Summary: Pythonic logger with better performance and contextvars + JSON support out of the box
-Home-page: 
+Home-page: https://github.com/violet-black/uvlog
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: logging,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
@@ -28,14 +28,16 @@
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: bump2version ; extra == 'dev'
+Requires-Dist: bandit ; extra == 'dev'
+Requires-Dist: xenon ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest ==8.1.1 ; extra == 'test'
 Requires-Dist: orjson ==3.9.15 ; extra == 'test'
 
@@ -49,37 +51,36 @@
 [![3.10](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml)
 [![3.11](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml)
 [![3.12](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml)
 
 **uvlog** is yet another logging library built with an idea of a simple logger what 'just works' without
 need for extension and customization. 
 
-- Single file, no external dependencies
+- Single package, no other dependencies
 - JSON and [contextvars](https://docs.python.org/3/library/contextvars.html) out of the box
 - Less abstraction, better [performance](#Performance)
 - Pythonic method names and classes
 
-# Use cases
+# Use
 
 Our main scenario is logging our containerized server applications, i.e. writing all the logs to the stderr
 of the container, where they are gathered and sent to the log storage by another service. However, you
 can use this library for any application as long as it does not require very complicated things like
 complex filters, adapters etc.
 
-# Usage
-
 The easiest way to access a logger is similar to the standard module. Note that you can pass
 extra variables as keyword arguments while logging.
 
 ```python
 from uvlog import get_logger
 
 logger = get_logger('app')
 logger.set_level('DEBUG')
-logger.debug('Hello, world!', name='John', surname='Dowe')
+
+logger.info('Hello, {name} {surname}!', name='John', surname='Dowe')
 ```
 
 To write an exception use `exc_info` param.
 
 ```python
 try:
     ...
@@ -87,130 +88,169 @@
     logger.error('Something bad happened', exc_info=exc)
 ```
 
 Configuration is possible in a way similar to `dictConfig`. The configuration dict itself is JSON compatible.
 The `configure()` function returns the root logger instance. Note that one destination can be assigned to
 only one handler, but each logger can have any number of handlers.
 
+Here's an extensive example of such config.
+
 ```python
 from uvlog import configure
 
 logger = configure({
     'loggers': {
-        '': {
+        '': {  # the root logger
             'level': 'DEBUG',
             'handlers': ['stderr', '/etc/log.txt']
         }
     },
     'handlers': {
-        'stderr': {
+        'stderr': {  # 'stderr' and 'stdout' are reserved for these special destinations
             'class': 'StreamHandler',
             'formatter': 'json'
         },
         '/etc/log.txt': {
-            'class': 'QueueHandler',
+            'class': 'QueueStreamHandler',
             'formatter': 'text'
         }
     },
     'formatters': {
         'text': {
             'class': 'TextFormatter',
-            'format': '{asctime} : {name} : {message}',
-            'timestamp_separator': ' '
+            'format': '{asctime} : {name} : {message}',  # see `LogRecord` for the list of fields
+            'timestamp_separator': ' '                   # by default it's 'T'
         },
         'json': {
             'class': 'JSONFormatter',
-            'keys': ['asctime', 'name', 'message']
+            'keys': ['asctime', 'name', 'message']       # see `LogRecord` for the list of fields
         }
     }
 })
 
 app_logger = logger.get_child('app', persistent=True)
 ```
 
-You can use context variables to maintain log context between log records. This can be useful in the server
-environment where you can assign a unique *Request-Id* to each request and easily aggregate the logs for it
-afterward.
+You can use context variables to maintain log context between log records. This can be useful for log aggregation.
+See the [documentation on contextvars](https://uvlog.readthedocs.io/guide.html#context-variables) for more info.
 
 ```python
 from uvlog import LOG_CONTEXT, get_logger
 
 app_logger = get_logger('app')
 
 async def handler_request(request):
     LOG_CONTEXT.set({'request_id': request.headers['Request-Id']})
     await call_system_api()
 
 async def call_system_api():
-    # this log record will have 'request_id' in its context
+    # this record will have 'request_id' in its context
     app_logger.info('Making a system call')
 ```
 
 When using the `JSONFormatter` you should consider providing a better json serializer for
 better performance (such as [orjson](https://github.com/ijl/orjson)).
 
 ```python
 import orjson
 from uvlog import JSONFormatter
 
 JSONFormatter.serializer = orjson.dumps
 ```
 
+# Never say never
+
+The library adds support for additional log level - `NEVER`. The idea behind this is to use such logs in places of code
+which should never be executed in production and monitor such cases. 'NEVER' logs have the maximum priority.
+They cannot be suppressed by any logger and are always handled.
+
+The use of `NEVER` is straightforward.
+
+```python
+def handle_authorization(username, password) -> bool:
+    if DEBUG and username == debug_login:
+        logger.never('skip authorization for {username}', username=username)
+        return True
+    return check_password_is_valid(username, password)
+```
+
+Why not just use a `DEBUG` or `WARNING` level here? The reason is low priority of such records, which allows them
+to be mixed with less significant logs or even be skipped by loggers.
+
 # Loggers are weak
 
 Unlike the standard logging module, loggers are weak referenced unless they are described explicitly
 in the configuration dict or created with `persistent=True` argument.
 
 It means that a logger is eventually garbage collected once it has no active references.
 This allows creation of a logger per task, not being concerned about running out of memory eventually.
 However, this also means that all logger settings for a weak logger will be forgotten once it's collected.
 
 In general this is not a problem since you shouldn't fiddle with logger settings outside the initialization
 phase.
 
-# Customization
+# Sampling
 
-You can create custom formatters and handlers with ease. Note that inheritance is not required.
-Just be sure to implement `Handler` / `Formatter` protocol.
+The library implements internal log sampling. In shorts, it allows you to specify the `sample_rate`,
+a probability at which a logger will pass a record to the handlers. It allows to release some load due
+to extensive logging.
 
 ```python
-from uvlog import add_formatter_type, add_handler_type
-
-class IdioticFormatter:
-    
-    def format(self, record, /) -> bytes:
-        return b'Bang!'
+from uvlog import get_logger
 
-add_formatter_type(IdioticFormatter)
+logger = get_logger()
+logger.sample_rate = 0.25
 ```
 
-Custom logger class can be set using `set_logger_type`
+... or via a config dict
 
 ```python
-from uvlog import set_logger_type, Logger
-
-class MyLogger(Logger):
-    ...
+from uvlog import configure
 
-set_logger_type(MyLogger)
+configure({
+    'loggers': {
+        '': {
+            'sample_rate': 0.25
+        }
+    }
+})
 ```
 
+See the [documentation on sampling](https://uvlog.readthedocs.io/guide.html#sampling>) for more info.
+
+# Customization
+
+You can create custom formatters and handlers with ease. Note that inheritance is not required.
+Just be sure to implement `Handler` / `Formatter` protocol.
+
+See the extension guide for more info. There's an example of
+[HTTP queue logger](https://uvlog.readthedocs.io/extension.html#example-http-logger) using
+[requests](https://docs.python-requests.org/en/latest/index.html) library there.
+
 # Performance
 
 Benchmark results are provided for the M1 Pro Mac (16GB). The results are for the `StreamHandler`
-writing same log records into a file. The `QueueHandler` provides similar performance, but has been excluded
+writing same log records into a file. The `QueueStreamHandler` provides similar performance, but has been excluded
 from the test since Python threading model prevents results from being consistent between runs. However,
-I'd still recommend using the `QueueHandler` for server applications.
+I'd still recommend using the `QueueStreamHandler` for server applications.
 
 | name          | total (s) | logs/s | %   |
 |---------------|-----------|--------|-----|
 | python logger | 0.085     | 117357 | 100 |
 | uvlog text    | 0.022     | 455333 | 388 |
 | uvlog json    | 0.015     | 665942 | 567 |
 
+# Compatibility
+
+There's a certain compatibility between this logger and the standard logger. However, it's impossible to preserve
+full compatibility because of certain design decisions.
+
+See the [compatibility guide](https://uvlog.readthedocs.io/compatibility.html) if you want to migrate from the standard
+python logger to this one.
+
 # Ideas / goals
 
 - Rotating file handlers
 - Asynchronous queue logging to HTTP / TCP / UDP
 - Better customization for `Logger` / `LogRecord` objects
 - Better coverage
 - Cython?
```


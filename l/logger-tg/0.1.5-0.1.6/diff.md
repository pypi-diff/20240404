# Comparing `tmp/logger-tg-0.1.5.tar.gz` & `tmp/logger-tg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-tg-0.1.5.tar", last modified: Sun Feb 25 18:54:40 2024, max compression
+gzip compressed data, was "logger-tg-0.1.6.tar", last modified: Thu Apr  4 15:15:54 2024, max compression
```

## Comparing `logger-tg-0.1.5.tar` & `logger-tg-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 18:54:40.705329 logger-tg-0.1.5/
--rw-rw-rw-   0        0        0     1095 2024-02-25 01:30:39.000000 logger-tg-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     6035 2024-02-25 18:54:40.705329 logger-tg-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4897 2024-02-25 17:50:21.000000 logger-tg-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 18:54:40.693810 logger-tg-0.1.5/logger_tg.egg-info/
--rw-rw-rw-   0        0        0     6035 2024-02-25 18:54:40.000000 logger-tg-0.1.5/logger_tg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-02-25 18:54:40.000000 logger-tg-0.1.5/logger_tg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 18:54:40.000000 logger-tg-0.1.5/logger_tg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-02-25 18:54:40.000000 logger-tg-0.1.5/logger_tg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-25 18:54:40.000000 logger-tg-0.1.5/logger_tg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-25 18:54:40.706331 logger-tg-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3729 2024-02-25 02:12:45.000000 logger-tg-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-25 18:54:40.698809 logger-tg-0.1.5/tg_logger/
--rw-rw-rw-   0        0        0       40 2024-02-25 18:18:51.000000 logger-tg-0.1.5/tg_logger/__init__.py
--rw-rw-rw-   0        0        0       66 2024-02-25 18:54:26.000000 logger-tg-0.1.5/tg_logger/__version__.py
-drwxrwxrwx   0        0        0        0 2024-02-25 18:54:40.703329 logger-tg-0.1.5/tg_logger/logger/
--rw-rw-rw-   0        0        0        0 2024-02-24 23:38:14.000000 logger-tg-0.1.5/tg_logger/logger/__init__.py
--rw-rw-rw-   0        0        0     3583 2024-02-25 17:28:02.000000 logger-tg-0.1.5/tg_logger/logger/logger_warner.py
--rw-rw-rw-   0        0        0     9076 2024-02-25 18:54:26.000000 logger-tg-0.1.5/tg_logger/logger/loggers.py
--rw-rw-rw-   0        0        0     1186 2024-02-25 00:07:47.000000 logger-tg-0.1.5/tg_logger/settings.py
--rw-rw-rw-   0        0        0      131 2024-02-24 22:52:51.000000 logger-tg-0.1.5/tg_logger/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:54.469396 logger-tg-0.1.6/
+-rw-rw-rw-   0        0        0     1095 2024-02-25 01:30:39.000000 logger-tg-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6065 2024-04-04 15:15:54.468370 logger-tg-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4896 2024-04-04 15:15:06.000000 logger-tg-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:54.463075 logger-tg-0.1.6/logger_tg.egg-info/
+-rw-rw-rw-   0        0        0     6065 2024-04-04 15:15:54.000000 logger-tg-0.1.6/logger_tg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-04 15:15:54.000000 logger-tg-0.1.6/logger_tg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:15:54.000000 logger-tg-0.1.6/logger_tg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 15:15:54.000000 logger-tg-0.1.6/logger_tg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 15:15:54.000000 logger-tg-0.1.6/logger_tg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:15:54.469396 logger-tg-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     3729 2024-02-25 02:12:45.000000 logger-tg-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:54.465244 logger-tg-0.1.6/tg_logger/
+-rw-rw-rw-   0        0        0       78 2024-04-04 15:15:40.000000 logger-tg-0.1.6/tg_logger/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-04 15:15:53.000000 logger-tg-0.1.6/tg_logger/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:54.467342 logger-tg-0.1.6/tg_logger/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-24 23:38:14.000000 logger-tg-0.1.6/tg_logger/logger/__init__.py
+-rw-rw-rw-   0        0        0     3583 2024-02-25 17:28:02.000000 logger-tg-0.1.6/tg_logger/logger/logger_warner.py
+-rw-rw-rw-   0        0        0     8080 2024-04-04 15:09:02.000000 logger-tg-0.1.6/tg_logger/logger/loggers.py
+-rw-rw-rw-   0        0        0     1075 2024-04-04 15:15:06.000000 logger-tg-0.1.6/tg_logger/logger/utils.py
+-rw-rw-rw-   0        0        0     1186 2024-02-25 00:07:47.000000 logger-tg-0.1.6/tg_logger/settings.py
+-rw-rw-rw-   0        0        0      131 2024-02-24 22:52:51.000000 logger-tg-0.1.6/tg_logger/utils.py
```

### Comparing `logger-tg-0.1.5/LICENSE` & `logger-tg-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.5/PKG-INFO` & `logger-tg-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-tg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous Telegram logging for Python applications
 Home-page: https://github.com/Nezhinskiy/logger-tg
 Author: Mikhail Nezhinsky
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Keywords: logger logging telegram async asyncio telegram_logger tg_logger python
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.0
 
 
 # logger-tg
 [![PyPI version](https://badge.fury.io/py/logger-tg.svg)](https://badge.fury.io/py/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg)](https://pepy.tech/project/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg/month)](https://pepy.tech/project/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg/week)](https://pepy.tech/project/logger-tg)
@@ -71,25 +72,25 @@
 
 ## Configuration
 Custom Log Handlers
 `logger-tg` allows for custom log handlers, enabling you to log to files, console, and Telegram simultaneously.
 
 ```python
 from logging.handlers import TimedRotatingFileHandler
-from logger_tg import BaseLogger, TgLoggerSettings
+from logger_tg import BaseLogger, TgLoggerSettings, get_logger
 
 # File handler for logging to a file
 file_handler = TimedRotatingFileHandler('app.log', when='midnight', interval=1)
 file_handler.suffix = '%Y-%m-%d'
 
 # Console handler for logging to stderr
 console_handler = logging.StreamHandler()
 
 # Initialize the logger with custom handlers
-logger = BaseLogger().get_logger(
+logger = get_logger(
     'MyAppLogger',
     console_log_handler=console_handler,
     file_log_handler=file_handler
 )
 
 logger.info('Logging to console and file.')
 ```
```

### Comparing `logger-tg-0.1.5/README.md` & `logger-tg-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 
 ## Configuration
 Custom Log Handlers
 `logger-tg` allows for custom log handlers, enabling you to log to files, console, and Telegram simultaneously.
 
 ```python
 from logging.handlers import TimedRotatingFileHandler
-from logger_tg import BaseLogger, TgLoggerSettings
+from logger_tg import BaseLogger, TgLoggerSettings, get_logger
 
 # File handler for logging to a file
 file_handler = TimedRotatingFileHandler('app.log', when='midnight', interval=1)
 file_handler.suffix = '%Y-%m-%d'
 
 # Console handler for logging to stderr
 console_handler = logging.StreamHandler()
 
 # Initialize the logger with custom handlers
-logger = BaseLogger().get_logger(
+logger = get_logger(
     'MyAppLogger',
     console_log_handler=console_handler,
     file_log_handler=file_handler
 )
 
 logger.info('Logging to console and file.')
 ```
```

### Comparing `logger-tg-0.1.5/logger_tg.egg-info/PKG-INFO` & `logger-tg-0.1.6/logger_tg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-tg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous Telegram logging for Python applications
 Home-page: https://github.com/Nezhinskiy/logger-tg
 Author: Mikhail Nezhinsky
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Keywords: logger logging telegram async asyncio telegram_logger tg_logger python
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.0
 
 
 # logger-tg
 [![PyPI version](https://badge.fury.io/py/logger-tg.svg)](https://badge.fury.io/py/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg)](https://pepy.tech/project/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg/month)](https://pepy.tech/project/logger-tg)
 [![Downloads](https://pepy.tech/badge/logger-tg/week)](https://pepy.tech/project/logger-tg)
@@ -71,25 +72,25 @@
 
 ## Configuration
 Custom Log Handlers
 `logger-tg` allows for custom log handlers, enabling you to log to files, console, and Telegram simultaneously.
 
 ```python
 from logging.handlers import TimedRotatingFileHandler
-from logger_tg import BaseLogger, TgLoggerSettings
+from logger_tg import BaseLogger, TgLoggerSettings, get_logger
 
 # File handler for logging to a file
 file_handler = TimedRotatingFileHandler('app.log', when='midnight', interval=1)
 file_handler.suffix = '%Y-%m-%d'
 
 # Console handler for logging to stderr
 console_handler = logging.StreamHandler()
 
 # Initialize the logger with custom handlers
-logger = BaseLogger().get_logger(
+logger = get_logger(
     'MyAppLogger',
     console_log_handler=console_handler,
     file_log_handler=file_handler
 )
 
 logger.info('Logging to console and file.')
 ```
```

### Comparing `logger-tg-0.1.5/setup.py` & `logger-tg-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.5/tg_logger/logger/logger_warner.py` & `logger-tg-0.1.6/tg_logger/logger/logger_warner.py`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.5/tg_logger/logger/loggers.py` & `logger-tg-0.1.6/tg_logger/logger/loggers.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,24 +26,28 @@
     )
 
     def __init__(
             self,
             name: str = 'app',
             bot_token: str = None,
             recipient_id: str | int = None,
+            logger: logging.Logger = None
     ) -> None:
         """
         Initializes the BaseLogger with optional Telegram logging.
 
         Parameters:
         - name (str, optional): The name of the logger.
         - bot_token (str, optional): The Telegram bot token.
         - recipient_id (str, int, optional): The Telegram recipient ID.
         """
-        self.logger = logging.getLogger(name)
+        if logger is None:
+            self.logger = logging.getLogger(name)
+        else:
+            self.logger = logger
         self.start_time = datetime.now(timezone.utc)
         self.tg_logger = self.configure_tg_logger(bot_token, recipient_id)
 
     def __getattr__(self, name: str) -> callable:
         """
         Allows dynamic access to logging methods based on attribute name.
 
@@ -135,45 +139,14 @@
                 'You must configure the logger using "configure_logger" or '
                 'provide "bot_token" and "recipient_id" during initialization.'
             ) from AttributeError
         else:
             settings = TgLoggerSettings(bot_token, recipient_id)
             return ClientLogger(settings, self.logger)
 
-    def get_logger(
-            self,
-            name: str = None,
-            level: int = None,
-            console_log_handler: logging.StreamHandler = None,
-            file_log_handler: TimedRotatingFileHandler = None
-    ) -> 'BaseLogger':
-        """
-        Configures a logger with optional console and file handlers.
-
-        Parameters:
-        - name (str, optional): The name of the logger.
-        - level (int, optional): The log level.
-        - console_log_handler (logging.StreamHandler, optional): A console log
-            handler.
-        - file_log_handler (TimedRotatingFileHandler, optional): A file log
-            handler.
-
-        Returns:
-        - BaseLogger: The configured logger.
-        """
-        logger = logging.getLogger(name)
-        if console_log_handler is not None:
-            logger.addHandler(console_log_handler)
-        if file_log_handler is not None:
-            logger.addHandler(file_log_handler)
-        if level is not None:
-            logger.setLevel(level)
-        self.logger = self.tg_logger.logger = logger
-        return self
-
     def critical(self, message: str) -> None:
         """
         Logs a critical message and sends it to the configured Telegram chat.
 
         Parameters:
         - message (str): The critical message.
         """
```

### Comparing `logger-tg-0.1.5/tg_logger/settings.py` & `logger-tg-0.1.6/tg_logger/settings.py`

 * *Files identical despite different names*


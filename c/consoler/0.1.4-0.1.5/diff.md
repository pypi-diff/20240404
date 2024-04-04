# Comparing `tmp/consoler-0.1.4.tar.gz` & `tmp/consoler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoler-0.1.4.tar", max compression
+gzip compressed data, was "consoler-0.1.5.tar", max compression
```

## Comparing `consoler-0.1.4.tar` & `consoler-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1063 2022-09-15 10:53:01.490675 consoler-0.1.4/LICENSE
--rw-r--r--   0        0        0     1282 2022-09-15 10:53:01.490815 consoler-0.1.4/README.md
--rw-r--r--   0        0        0       88 2022-09-15 10:53:01.490985 consoler-0.1.4/consoler/__init__.py
--rw-r--r--   0        0        0     2419 2022-09-15 10:53:01.491097 consoler-0.1.4/consoler/colours.py
--rw-r--r--   0        0        0     7556 2022-09-15 10:53:01.491246 consoler-0.1.4/consoler/console.py
--rw-r--r--   0        0        0      507 2022-09-15 10:53:01.491355 consoler-0.1.4/consoler/settings.py
--rw-r--r--   0        0        0      704 2022-09-15 11:41:38.035777 consoler-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1965 2022-09-15 11:46:08.032744 consoler-0.1.4/setup.py
--rw-r--r--   0        0        0     2203 2022-09-15 11:46:08.032953 consoler-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-04 08:32:45.868780 consoler-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1282 2024-04-04 08:32:45.868930 consoler-0.1.5/README.md
+-rw-r--r--   0        0        0       88 2024-04-04 08:32:45.869096 consoler-0.1.5/consoler/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-04 11:22:39.483403 consoler-0.1.5/consoler/colours.py
+-rw-r--r--   0        0        0     7425 2024-04-04 14:58:52.364919 consoler-0.1.5/consoler/console.py
+-rw-r--r--   0        0        0      507 2024-04-04 08:32:45.869519 consoler-0.1.5/consoler/settings.py
+-rw-r--r--   0        0        0     1136 2024-04-04 14:59:17.756482 consoler-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 consoler-0.1.5/PKG-INFO
```

### Comparing `consoler-0.1.4/LICENSE` & `consoler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `consoler-0.1.4/README.md` & `consoler-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `consoler-0.1.4/consoler/colours.py` & `consoler-0.1.5/consoler/colours.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'WHITE': '\033[37m',
     'DARKGREY': '\033[90m',
     'LIGHTRED': '\033[91m',
     'LIGHTGREEN': '\033[92m',
     'YELLOW': '\033[93m',
     'LIGHTBLUE': '\033[94m',
     'PINK': '\033[95m',
-    'LIGHTCYAN': '\033[96m'
+    'LIGHTCYAN': '\033[96m',
 }
 
 
 def bg_black(msg):
     return '{}{}{}'.format(BG['BLACK'], msg, RESET)
```

### Comparing `consoler-0.1.4/consoler/console.py` & `consoler-0.1.5/consoler/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 
 """
     helpers.console
     ~~~~~~~~~~~~~~~
     Console level logging that doesn't barf on unicode.
 """
 
-from __future__ import absolute_import, unicode_literals
-
-import os
 import sys
 import math
 import inspect
 from typing import Any
+from pathlib import Path
 
 import arrow
-from loguru import logger as guru
+
+try:
+    from loguru import logger as guru
+except ImportError:
+    USE_GURU = False
+else:
+    USE_GURU = True
 
 from .settings import settings
 from .colours import blue, cyan, green, magenta, orange, red, bg_blue  # NOQA
 
 
 LOG_LEVELS = {
     'LOG': 0,
     'INFO': 1,
     'SUCCESS': 2,
     'TEMPLATE': 3,
     'WARN': 4,
-    'ERROR': 5
+    'ERROR': 5,
 }
 
 CLEAR = '\033[K'
 HIDE_CURSOR = '\033[?25l'
 SHOW_CURSOR = '\033[?25h'
 
 
@@ -66,129 +70,118 @@
             level_str = settings.CONSOLE_LOG_LEVEL
         except Exception:
             level_str = 'WARN'
         level = LOG_LEVELS[level_str]
         called = LOG_LEVELS[called_level]
         if called >= level:
             return True
-        else:
-            return False
+        return False
 
     def _get_code_position(self, curframe):
         frame = inspect.getouterframes(curframe, 0)
-        base = os.getcwd()
+        base = Path.cwd()
         try:
             pos = '{}{}:{}'.format(
                 self.path_prefix,
                 frame[1].filename.replace(base, ''),
-                frame[1].lineno
+                frame[1].lineno,
             )
         except IndexError:  # We couldn't get the stack info for some reason
             return '¯\\_(ツ)_/¯'
         else:
             return pos
 
     def _output(self, prefix: str, msg: str, extra: Any) -> None:
         print('{}\n> {} {}'.format(prefix, decode(msg), extra if extra else ''))
 
     def _ts(self) -> str:
         return magenta(str(arrow.now().format('H:mm:ss')))
 
     def log(self, msg=None, extra=None) -> None:
         if not self._check_log_level('LOG'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), cyan('LOG'), pos)
         self._output(prefix, msg, extra)
 
     def info(self, msg: str, extra=None) -> None:
         """Output a message in the INFO style
 
         Args:
             msg (str): The message you want to output
             extra (None, optional): Anything else you want added to the message
         """
         if not self._check_log_level('INFO'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), blue('INFO'), pos)
-        if settings.DEBUG:
-            self._output(prefix, msg, extra)
-        else:
+        if USE_GURU and settings.DEBUG is False:
             guru.info(f'{prefix} - {msg} - {extra}')
 
     def warn(self, msg: str, extra=None) -> None:
         """Output a message in the WARN style
 
         Args:
             msg (str): The message you want to output
             extra (None, optional): Anything else you want added to the message
         """
         if not self._check_log_level('WARN'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), orange('WARN'), pos)
         self._output(prefix, msg, extra)
-        if settings.DEBUG:
-            self._output(prefix, msg, extra)
-        else:
+        if USE_GURU and settings.DEBUG is False:
             guru.warning(f'{prefix} - {msg} - {extra}')
 
     def error(self, msg: str, extra=None) -> None:
         """Output a message in the ERROR style
 
         Args:
             msg (str): The message you want to output
             extra (None, optional): Anything else you want added to the message
         """
         if not self._check_log_level('ERROR'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), red('ERROR'), pos)
-        if settings.DEBUG:
-            self._output(prefix, msg, extra)
-        else:
+        if USE_GURU and settings.DEBUG is False:
             guru.error(f'{prefix} - {msg} - {extra}')
 
     def success(self, msg: str, extra=None) -> None:
         """Output a message in the SUCCESS style
 
         Args:
             msg (str): The message you want to output
             extra (None, optional): Anything else you want added to the message
         """
         if not self._check_log_level('SUCCESS'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), green('SUCCESS'), pos)
-        if settings.DEBUG:
-            self._output(prefix, msg, extra)
-        else:
+        if USE_GURU and settings.DEBUG is False:
             guru.success(f'{prefix} - {msg} - {extra}')
 
     def template(self, msg: str, extra=None) -> None:
         """Output a message in the TEMPLATE style
 
         Args:
             msg (str): The message you want to output
             extra (None, optional): Anything else you want added to the message
         """
         if not self._check_log_level('TEMPLATE'):
-            return None
+            return
         curframe = inspect.currentframe()
         pos = self._get_code_position(curframe)
         prefix = '{} - {} - {}'.format(self._ts(), magenta('TEMPLATE'), pos)
-        if settings.DEBUG:
-            self._output(prefix, msg, extra)
-        else:
+        if USE_GURU and settings.DEBUG is False:
             guru.success(f'{prefix} - {msg} - {extra}')
 
     def progress(self, msg: str = '', perc=0):
         spinner_frames = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
         if self.spindex == len(spinner_frames) - 1:
             self.spindex = 0
         else:
@@ -198,28 +191,28 @@
         self.terminal.flush()
         blocks = math.floor(perc / 5)
         spaces = math.ceil((100 - perc) / 5)
         human = f'{perc:.4f}'
         self.terminal.write(
             ' [{}{}] {} {}% {}\r'.format(
                 bg_blue(' ') * blocks,
-                ' ' * spaces, magenta(spinner_frames[self.spindex]), human, message
-            )
+                ' ' * spaces, magenta(spinner_frames[self.spindex]), human, message,
+            ),
         )
         self.terminal.flush()
         self.writing_progress = True
 
     def _parse(self, msg):
         if isinstance(msg, str):
             return msg
-        else:
-            try:
-                return str(msg)
-            except Exception:
-                raise
+
+        try:
+            return str(msg)
+        except Exception:
+            raise
 
 
 def decode(val):
     """Try to decode a string, and don't stop code execution if it fails.
 
     Args:
         val (str): Should be a string.
@@ -238,10 +231,11 @@
     except Exception:
         try:
             return val.decode('latin-1')
         except Exception:
             try:
                 return val.decode('ascii')
             except Exception:
-                pass
+                if USE_GURU and settings.DEBUG is False:
+                    guru.error(f'Failed to decode {val}')
 
     return val
```

### Comparing `consoler-0.1.4/PKG-INFO` & `consoler-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: consoler
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/hactar-is/consoler
 License: MIT
 Keywords: console,terminal,logging
 Author: Hactar
 Author-email: systems@hactar.is
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Project-URL: Repository, https://github.com/hactar-is/consoler
 Description-Content-Type: text/markdown
 
 ## Consoler
 
 A terminal printer that's totally tailored to how I like terminal printouts. If this happens to also be how you like terminal printouts, this package may well be for you too.
```


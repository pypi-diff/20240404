# Comparing `tmp/botl-105.tar.gz` & `tmp/botl-106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botl-105.tar", last modified: Tue Apr  2 03:06:51 2024, max compression
+gzip compressed data, was "botl-106.tar", last modified: Thu Apr  4 12:25:42 2024, max compression
```

## Comparing `botl-105.tar` & `botl-106.tar`

### file list

```diff
@@ -1,40 +1,49 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.256918 botl-105/
--rw-r--r--   0 bart      (1000) bart      (1000)     3964 2024-04-02 03:06:51.252917 botl-105/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3445 2024-04-02 02:53:55.000000 botl-105/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl/
--rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-04-01 19:52:46.000000 botl-105/botl/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3930 2024-04-02 02:56:38.000000 botl-105/botl/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-04-01 19:52:46.000000 botl-105/botl/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-04-01 19:52:46.000000 botl-105/botl/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-04-01 19:52:46.000000 botl-105/botl/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-04-01 20:34:46.000000 botl-105/botl/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-04-01 19:52:51.000000 botl-105/botl/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-04-01 19:52:51.000000 botl-105/botl/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-04-01 19:52:51.000000 botl-105/botl/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      741 2024-04-01 19:52:51.000000 botl-105/botl/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17673 2024-04-01 19:52:51.000000 botl-105/botl/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-04-01 19:52:51.000000 botl-105/botl/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3485 2024-04-01 19:52:51.000000 botl-105/botl/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16976 2024-04-01 19:55:33.000000 botl-105/botl/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-04-01 19:52:51.000000 botl-105/botl/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2398 2024-04-01 19:52:51.000000 botl-105/botl/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-04-01 19:52:51.000000 botl-105/botl/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2737 2024-04-01 19:52:51.000000 botl-105/botl/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1118 2024-04-01 19:52:51.000000 botl-105/botl/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-04-01 19:52:51.000000 botl-105/botl/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5020 2024-04-01 19:52:51.000000 botl-105/botl/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2913 2024-04-01 19:52:51.000000 botl-105/botl/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-04-01 19:52:46.000000 botl-105/botl/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-04-01 19:52:46.000000 botl-105/botl/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-04-01 19:52:46.000000 botl-105/botl/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3964 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      671 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       47 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      836 2024-04-02 02:59:24.000000 botl-105/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-02 03:06:51.256918 botl-105/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-01 19:43:21.000000 botl-105/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3963 2024-04-04 12:25:42.689670 botl-106/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3440 2024-04-04 12:15:24.000000 botl-106/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.685670 botl-106/botl/
+-rw-r--r--   0 bart      (1000) bart      (1000)       80 2024-04-04 11:34:13.000000 botl-106/botl/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4026 2024-04-04 12:07:39.000000 botl-106/botl/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      904 2024-04-04 11:48:34.000000 botl-106/botl/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1582 2024-04-04 12:05:43.000000 botl-106/botl/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      321 2024-04-04 11:47:18.000000 botl-106/botl/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1733 2024-04-04 11:47:57.000000 botl-106/botl/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      865 2024-04-04 11:46:43.000000 botl-106/botl/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1608 2024-04-04 12:10:33.000000 botl-106/botl/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/botl/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      436 2024-04-04 11:31:06.000000 botl-106/botl/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      220 2024-04-04 11:38:19.000000 botl-106/botl/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      229 2024-04-04 12:11:53.000000 botl-106/botl/modules/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      534 2024-04-04 11:31:06.000000 botl-106/botl/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      405 2024-04-04 11:38:51.000000 botl-106/botl/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      800 2024-04-04 11:40:01.000000 botl-106/botl/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    18973 2024-04-04 11:40:19.000000 botl-106/botl/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      825 2024-04-04 11:40:51.000000 botl-106/botl/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2469 2024-04-04 11:41:08.000000 botl-106/botl/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16437 2024-04-04 11:41:23.000000 botl-106/botl/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      245 2024-04-04 11:41:42.000000 botl-106/botl/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2409 2024-04-04 11:42:03.000000 botl-106/botl/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    10919 2024-04-04 11:42:15.000000 botl-106/botl/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3195 2024-04-04 11:42:35.000000 botl-106/botl/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1181 2024-04-04 11:42:49.000000 botl-106/botl/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1061 2024-04-04 11:43:07.000000 botl-106/botl/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5240 2024-04-04 11:43:22.000000 botl-106/botl/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3137 2024-04-04 11:43:38.000000 botl-106/botl/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6154 2024-04-04 11:48:18.000000 botl-106/botl/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-04 11:48:07.000000 botl-106/botl/parser.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3435 2024-04-04 11:46:19.000000 botl-106/botl/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-04 11:47:29.000000 botl-106/botl/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2029 2024-04-04 12:10:16.000000 botl-106/botl/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1151 2024-04-04 11:46:52.000000 botl-106/botl/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-04 11:47:07.000000 botl-106/botl/utils.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      779 2024-04-04 12:09:42.000000 botl-106/botl/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-04 12:25:42.689670 botl-106/botl.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3963 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      812 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       47 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-04 12:25:42.000000 botl-106/botl.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      840 2024-04-04 12:16:12.000000 botl-106/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-04 12:25:42.689670 botl-106/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-04 11:31:06.000000 botl-106/setup.py
```

### Comparing `botl-105/PKG-INFO` & `botl-106/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 105
-Summary: cli bot
+Version: 106
+Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
@@ -22,15 +22,15 @@
 
 
 SYNOPSIS
 
 ::
 
     botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v] [-w]
+    botl [-a] [-c] [-d] [-h] [-v]
 
     options are:
 
     -a     load all modules
     -c     start console
     -d     start daemon
     -h     display help
```

### Comparing `botl-105/README.rst` & `botl-106/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 SYNOPSIS
 
 ::
 
     botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v] [-w]
+    botl [-a] [-c] [-d] [-h] [-v]
 
     options are:
 
     -a     load all modules
     -c     start console
     -d     start daemon
     -h     display help
```

### Comparing `botl-105/botl/__main__.py` & `botl-106/botl/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,85 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
+# pylint: disable=C,R,W0105,W0212
 # ruff: noqa: E402
 
 
 "main"
 
 
 import getpass
 import os
 import pwd
-import readline # pylint: disable=W0611
 import sys
 import termios
 import time
 
 
-from .broker  import Broker
-from .errors  import debug
-from .handler import Client, Event, cmnd, parse_cmd
-from .object  import Default, cdir, spl
-from .errors  import Errors
-from .persist import Workdir
-
-
-Cfg         = Default()
-Cfg.mod     = "cmd,mod"
-Cfg.name    = "botl"
-Cfg.version = "105"
-Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.wd = Cfg.wd
+from .client  import Client, cmnd
+from .default import Default
+from .errors  import Errors,debug
+from .event   import Event
+from .object  import cdir
+from .parser  import parse_cmd
+from .utils   import spl
+from .workdir import Workdir
 
 
 from . import modules
 
 
-if os.path.exists("mods"):
-    import mods
-else:
-    mods = None
+Cfg          = Default()
+Cfg.mod      = "cmd,mod"
+Cfg.name     = "botl"
+Cfg.version  = "106"
+Cfg.dir      = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile  = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Workdir.workdir = Cfg.dir
 
 
 dte = time.ctime(time.time()).replace("  ", " ")
+ext = os._exit 
 
 
 class Console(Client):
 
-    def __init__(self):
-        Client.__init__(self)
-        Broker.add(self)
+    "Console"
 
     def announce(self, txt):
-        pass
+        "blind announce"
 
     def callback(self, evt):
+        "run and wait for callback to finish."
         Client.callback(self, evt)
-        evt.wait()
+        evt.wait(5.0)
 
     def poll(self):
+        "reconstruct event from input."
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, channel, txt):
+    def say(self, _channel, txt):
+        "say text in channel."
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
+    "fork into the background."
     pid = os.fork()
     if pid != 0:
-        os._exit(0)
+        ext(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
-        os._exit(0)
+        ext(0)
     if not verbose:
         with open('/dev/null', 'r', encoding="utf-8") as sis:
             os.dup2(sis.fileno(), sys.stdin.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as sos:
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
@@ -91,34 +89,37 @@
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
 def init(pkg, modstr, disable=""):
+    "start inits in modules."
     mds = []
     for modname in spl(modstr):
         if modname in spl(disable):
             continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
             module.init()
             mds.append(module)
     return mds
 
 
 def privileges(username):
+    "lower privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def wrap(func):
+    "restore terminal"
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
@@ -126,51 +127,55 @@
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
 def ver(event):
+    "show version."
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
+"runtime"
+
+
 def main():
+    "main code"
     Workdir.skel()
     Errors.enable(print)
-    Client.add(ver)
+    #Client.add(ver)
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
+    result = None
     if 'a' in Cfg.opts:
-        Cfg.mod = ",".join(mods.__dir__())
-        Cfg.mod += "," + ",".join(modules.__dir__())
+        Cfg.mod = "," + ",".join(modules.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
-        return
+        return result
     if "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
         Cfg.user = getpass.getuser()
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
-        return
-    if "c" in Cfg.opts:
+    elif "c" in Cfg.opts:
         init(modules, Cfg.mod)
-        init(mods, Cfg.mod)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
-        return
-    if Cfg.otxt:
-        return cmnd(Cfg.otxt, print)
+    elif Cfg.otxt:
+        cmnd(Cfg.otxt, print)
+    return result
 
 
 def wrapped():
+    "wrapped code"
     wrap(main)
     Errors.show()
 
 
 if __name__ == "__main__":
     wrapped()
```

### Comparing `botl-105/botl/broker.py` & `botl-106/botl/broker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402,E1102
+# pylint: disable=C,R,W0105
 
 
-"""object broker
-
-This Broker class stores objects on their repr name and can thus be
-retrieved by a client presenting a repr of an object.
-
-Client can carry a string (the repr) around instead of a memory
-reference to the object.
-
-Adding an object takes the repr and stores it in a dict, the rest are
-methods to retrieve an object from the broker.
-
-Broker is operating at an class level where the class level attributes
-are manipulated instead of an object inherited from that class.
-
-"""
+"broker"
 
 
 from .object import Object, keys, values
 
 
 rpr = object.__repr__
 
 
 class Broker:
 
+    "Broker"
+
     objs = Object()
 
     @staticmethod
     def add(obj):
         "add an object to the broker."
         setattr(Broker.objs, rpr(obj), obj)
 
@@ -53,15 +41,15 @@
 
     @staticmethod
     def remove(obj):
         "remove object from broker"
         delattr(Broker.objs, rpr(obj))
 
 
-"interfacce"
+"interface"
 
 
 def __dir__():
     return (
         'Broker',
     )
```

### Comparing `botl-105/botl/modules/err.py` & `botl-106/botl/modules/err.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0622,E0402,W0105
+#
 
 
 "status of bots"
 
 
 from ..broker  import Broker
-from ..handler import Client
+from ..client  import Client
 from ..errors  import Errors
 
 
 def err(event):
+    "show errors."
     nmr = 0
     for bot in Broker.all():
         if 'state' in dir(bot):
             event.reply(str(bot.state))
             nmr += 1
     event.reply(f"status: {nmr} errors: {len(Errors.errors)}")
     for exc in Errors.errors:
```

### Comparing `botl-105/botl/modules/fnd.py` & `botl-106/botl/modules/fnd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,E0402
+# pylint: disable=C,R
 
 
-"locate"
+"find"
 
 
+from ..client  import Client
 from ..object  import fmt
 from ..persist import Persist, Workdir, find
 
 
 def fnd(event):
+    "find objects."
     Workdir.skel()
     if not event.rest:
         res = sorted([x.split('.')[-1].lower() for x in Workdir.types()])
         if res:
             event.reply(",".join(res))
         return
     otype = event.args[0]
@@ -26,7 +28,10 @@
                 clz = fnm
     nmr = 0
     for fnm, obj in find(clz, event.gets):
         event.reply(f"{nmr} {fmt(obj)}")
         nmr += 1
     if not nmr:
         event.reply("no result")
+
+
+Client.add(fnd)
```

### Comparing `botl-105/botl/modules/irc.py` & `botl-106/botl/modules/irc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0612,W0718,E0402,W0201,W0603
+# pylint: disable=C,R,W0718
 # ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
@@ -15,53 +15,55 @@
 import textwrap
 import threading
 import time
 import _thread
 
 
 from ..broker  import Broker
-from ..handler import Client, Event
+from ..client  import Client
+from ..default import Default
+from ..event   import Event
 from ..errors  import Errors, debug
-from ..object  import Default, Object, edit, fmt, keys
+from ..object  import Object, edit, fmt, keys
 from ..persist import Persist, last, sync
 from ..thread  import launch
 
 
 NAME    = __file__.split(os.sep)[-3]
 get     = Broker.get
 saylock = _thread.allocate_lock()
 
 
 Errors.filter = ["PING", "PONG", "PRIVMSG"]
 
 
-myirc = None
-
-
 def init():
-    global myirc
+    "initialize a irc bot."
     irc = IRC()
-    myirc = object.__repr__(irc)
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
 def shutdown():
-    debug(f"IRC stopping {myirc}")
-    irc = Broker.get(myirc)
-    if irc:
-        irc.state.pongcheck = True
-        irc.state.keeprunning = False
-        irc.events.connected.clear()
-        irc.stop()
+    "shutdown irc bot."
+    for bot in Broker.all():
+        if "irc" not in type(bot):
+            continue
+        debug(f"IRC stopping {repr(bot)}")
+        bot.state.pongcheck = True
+        bot.state.keeprunning = False
+        bot.events.connected.clear()
+        bot.stop()
 
 
 class Config(Default):
 
+    "Config"
+
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
     realname = NAME
@@ -85,14 +87,16 @@
 
 
 Persist.add(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
+    "TextWrap"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -100,47 +104,54 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
+    "Output"
+
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
+        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
+        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
+        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
+        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -155,21 +166,24 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
+        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
+    "IRC"
+
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
         self.channels = []
         self.events = Default()
@@ -195,18 +209,20 @@
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
         Broker.add(self)
 
     def announce(self, txt):
+        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
+        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -215,14 +231,15 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
             debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
@@ -241,31 +258,34 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
+        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as ex:
+               ) as _ex:
             pass
         except Exception as ex:
             Errors.add(ex)
 
     def doconnect(self, server, nck, port=6667):
+        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
@@ -274,14 +294,15 @@
                 self.state.error = str(ex)
                 debug(str(ex))
             debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
+        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -300,18 +321,20 @@
         elif cmd == '433':
             self.state.error = txt
             nck = self.cfg.nick + '_'
             self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
+        "join all channels."
         for channel in self.channels:
             self.docommand('JOIN', channel)
 
     def keep(self):
+        "keep alive."
         while not self.stopped.is_set():
             if self.state.stopkeep:
                 self.state.stopkeep = False
                 break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
@@ -324,21 +347,23 @@
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
+        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
+        "parse text into an event."
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -392,14 +417,15 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
+        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -419,14 +445,15 @@
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
+        "send raw text."
         txt = txt.rstrip()
         debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
@@ -441,47 +468,52 @@
                 Errors.add(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
+        "reconnect to server."
         debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
+        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
+        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
+        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
         launch(Client.start, self)
@@ -491,85 +523,96 @@
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
+        "stop bot."
         self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
+        "wait for ready."
         self.events.ready.wait()
 
 
 def cb_auth(evt):
+    "auth callback."
     bot = get(evt.orig)
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(evt):
+    "capabilities callback."
     bot = get(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_error(evt):
+    "error callback."
     bot = get(evt.orig)
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
     debug(evt.txt)
 
 
 def cb_h903(evt):
+    "auth succeded callback."
     bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(evt):
+    "auth succeded callback."
     bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(evt):
-    pass
+    "got killed callback."
 
 
 def cb_log(evt):
-    pass
+    "log callback."
 
 
 def cb_ready(evt):
+    "bot is ready callback."
     bot = get(evt.orig)
     if bot:
         bot.events.ready.set()
 
 
 def cb_001(evt):
+    "first line received callback."
     bot = get(evt.orig)
     bot.logon()
 
 
 def cb_notice(evt):
+    "notice callback."
     bot = get(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(evt):
+    "privmsg callback."
     bot = get(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
@@ -579,21 +622,23 @@
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
         bot.command(evt)
 
 
 def cb_quit(evt):
+    "quit callback."
     bot = get(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
 def cfg(event):
+    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
@@ -606,14 +651,15 @@
         event.reply('ok')
 
 
 Client.add(cfg)
 
 
 def mre(event):
+    "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = Broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
@@ -628,14 +674,15 @@
     event.reply(f'{size} more in cache')
 
 
 Client.add(mre)
 
 
 def pwd(event):
+    "create a base64 password."
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
```

### Comparing `botl-105/botl/modules/log.py` & `botl-106/botl/modules/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C,E0402
+# pylint: disable=C,R
 
 
 "log text"
 
 
 import time
 
 
-from ..handler import Client
+from ..client  import Client
 from ..object  import Object
-from ..persist import Persist, find, fntime, laps, sync
+from ..persist import Persist, find, fntime, sync
+from ..utils   import laps
 
 
 class Log(Object):
 
+    "Log"
+
     def __init__(self):
-        super().__init__()
+        Object.__init__()
         self.txt = ''
 
+    def __yo__(self):
+        pass
+
+    def __yoyo__(self):
+        pass
+
 
 Persist.add(Log)
 
 
 def log(event):
+    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
```

### Comparing `botl-105/botl/modules/mdl.py` & `botl-106/botl/modules/mdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0613,E0402
+# pylint: disable=C,R
 
 
 "genocide model of the netherlands"
 
 
 import datetime
 import time
 
 
-from botl.broker  import Broker
-from botl.handler import Event
-from botl.object  import Object, construct, keys
-from botl.persist import laps
-from botl.thread  import Repeater, launch
+from ..broker   import Broker
+from ..client   import Client
+from ..event    import Event
+from ..object   import Object, construct, keys
+from ..repeater import Repeater
+from ..thread   import launch
+from ..utils    import laps
 
 
 def __dir__():
     return (
             'init',
             'now'
-           ) 
+           )
 
 
 def init():
+    "start genocide model."
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
-    
+
 
 DAY = 24*60*60
 YEAR = 365*DAY
 SOURCE = "https://github.com/bthate/genocide"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
@@ -277,121 +280,123 @@
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
 def getalias(txt):
+    "teturn matching alias."
+    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            return value
+            result = value
+            break
+    return result
 
 
 def getday():
+    "return timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
+    "return number of deaths by name."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
+    "calculate sedconds"
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
+    "see whether an item is wanted."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
+    "run a callback daily."
     while 1:
         time.sleep(24*60*60)
-        evt = Event()
-        cbnow(evt)
+        cbnow(Event())
 
 
 def hourly():
+    "run a callback hourly."
     while 1:
         time.sleep(60*60)
-        evt = Event()
-        cbnow(evt)
+        cbnow(Event())
 
 
 def cbnow(evt):
+    "check status now callback."
+    if not evt:
+        evt = Event()
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += "%s: %s " % (getalias(name), nrtimes)
+        txt += f"{getalias(name)}: {nrtimes}"
     txt += " http://genocide.rtfd.io"
     for bot in Broker.all():
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
+    "callback showing stats."
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
-        nrtimes = int(delta/needed)
-        nryear = int(YEAR/needed)
-        nrday = int(DAY/needed)
+        nrt = int(delta/needed)
+        nry = int(YEAR/needed)
+        nrd = int(DAY/needed)
         delta2 = time.time() - getday()
-        thisday = int(delta2/needed)
-        txt = "patient #%s died from %s (%s/%s) every %s (%s/year)" % (
-                                                               nrtimes,
-                                                               getalias(name),
-                                                               thisday,
-                                                               nrday,
-                                                               laps(needed),
-                                                               nryear,
-                                                              )
+        this = int(delta2/needed)
+        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)} ({nry}/year)"
         for bot in Broker.all():
             bot.announce(txt)
 
 
 def now(event):
+    "showing number of psychiatric patients victims."
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
-        nrtimes = int(delta/needed)
-        nryear = int(YEAR/needed)
-        nrday = int(DAY/needed)
-        thisday = int(DAY % needed)
-        txt += "patient #%s died from %s (%s/%s/%s) every %s" % (
-                                                                 nrtimes,
-                                                                 getalias(name),
-                                                                 thisday,
-                                                                 nrday,
-                                                                 nryear,
-                                                                 laps(needed)
-                                                                )
+        nrt = int(delta/needed)
+        nrd = int(DAY/needed)
+        this = int(DAY % needed)
+        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)}"
         event.reply(txt)
     else:
         event.reply("not needed")
 
 
+Client.add(now)
+
+
 def boot():
+    "format model data."
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
```

### Comparing `botl-105/botl/modules/req.py` & `botl-106/botl/modules/req.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0115,C0116
+# pylint: disable=C.R
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
@@ -75,15 +75,16 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-from ..handler import Client
+from ..client import Client
 
 
 def req(event):
+    "show request."
     event.reply(__doc__)
 
 
 Client.add(req)
```

### Comparing `botl-105/botl/modules/rss.py` & `botl-106/botl/modules/rss.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0201,W0612,E0402
+# pylint: disable=C,R
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,67 +14,79 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..broker  import Broker
-from ..handler import Client
-from ..object  import Default, Object, fmt, spl, update
-from ..persist import Persist, find, fntime, laps, last, sync
-from ..thread  import Repeater, launch
+from ..broker   import Broker
+from ..client   import Client
+from ..default  import Default
+from ..object   import Object, fmt, update
+from ..persist  import Persist, find, fntime, last, sync
+from ..repeater import Repeater
+from ..thread   import launch
+from ..utils    import laps, spl
 
 
 def init():
+    "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 DEBUG = False
 
 
 fetchlock = _thread.allocate_lock()
 
 
 class Feed(Default):
 
-    pass
+    "Feed"
 
 
 class Rss(Default):
 
+    "Rss"
+
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
+        self.rss          = ''
 
 
 Persist.add(Rss)
 
 
 class Seen(Default):
 
+    "Seen"
+
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
 
 Persist.add(Seen)
 
 
 class Fetcher(Object):
 
+    "Fetcher"
+
     def __init__(self):
         self.dosave = False
         self.seen = Seen()
         self.seenfn = None
 
     @staticmethod
     def display(obj):
+        "display object."
         result = ''
         displaylist = []
         try:
             displaylist = obj.display_list or 'title,link'
         except AttributeError:
             displaylist = 'title,link,author'
         for key in displaylist.split(","):
@@ -87,14 +99,15 @@
             data = striphtml(data.rstrip())
             data = unescape(data)
             result += data.rstrip()
             result += ' - '
         return result[:-2].rstrip()
 
     def fetch(self, feed):
+        "fetch feed."
         with fetchlock:
             counter = 0
             result = []
             for obj in reversed(getfeed(feed.rss, feed.display_list)):
                 fed = Feed()
                 update(fed, obj)
                 update(fed, feed)
@@ -120,62 +133,69 @@
             txt2 = txt + self.display(obj)
             for bot in Broker.all():
                 if "announce" in dir(bot):
                     bot.announce(txt2.rstrip())
         return counter
 
     def run(self):
+        "fetch all feeds."
         thrs = []
-        for fnm, feed in find('rss'):
+        for _fn, feed in find('rss'):
             thrs.append(launch(self.fetch, feed, name=f"{feed.rss}"))
         return thrs
 
     def start(self, repeat=True):
+        "start fetcher."
         self.seenfn = last(self.seen)
         if repeat:
             repeater = Repeater(300.0, self.run)
             repeater.start()
 
 
 class Parser:
 
+    "Parser"
+
     @staticmethod
     def getvalue(line, attr):
+        "retrieve attribute value."
         lne = ''
-        index1 = line.find(f' {attr}="')
+        index1 = line.find(f'{attr}="')
         if index1 == -1:
             return lne
-        index1 += len(attr) + 3
+        index1 += len(attr) + 2
         index2 = line.find('"', index1)
         if index2 == -1:
             index2 = line.find('"/>', index1)
         if index2 == -1:
             return lne
         lne = line[index1:index2]
         if 'CDATA' in lne:
             lne = lne.replace('![CDATA[', '')
             lne = lne.replace(']]', '')
             #lne = lne[1:-1]
         return lne
 
     @staticmethod
     def getattrs(line, token):
+        "split for attributes."
         result = ""
         index1 = line.find(f'<{token} ')
         if index1 == -1:
             return result
         index1 += len(token) + 2
         index2 = line.find('/>', index1)
         if index2 == -1:
             return result
         result = line[index1:index2]
         return result.strip()
-    
+
     @staticmethod
     def getitem(line, item):
+        "match items."
         lne = ''
         index1 = line.find(f'<{item}>')
         if index1 == -1:
             return lne
         index1 += len(item) + 2
         index2 = line.find(f'</{item}>', index1)
         if index2 == -1:
@@ -185,73 +205,79 @@
             lne = lne.replace('![CDATA[', '')
             lne = lne.replace(']]', '')
             lne = lne[1:-1]
         return lne.strip()
 
     @staticmethod
     def getitems(text, token):
+        "loop for items."
         index = 0
         result = []
         stop = False
         while not stop:
-            index1 = text.find(f'<{token}>', index)
+            index1 = text.find(f'<{token}', index)
             if index1 == -1:
                 break
             index1 += len(token) + 2
             index2 = text.find(f'</{token}>', index1)
             if index2 == -1:
                 break
             lne = text[index1:index2]
             result.append(lne)
-            index = index2             
+            index = index2
         return result
 
     @staticmethod
     def parse(txt, toke="item", items='title,link'):
+        "parse a text for tokens."
         result = []
         for line in Parser.getitems(txt, toke):
             line = line.strip()
             obj = Default()
             for itm in spl(items):
                 val = Parser.getitem(line, itm)
                 if val:
                     val = unescape(val.strip())
                     val = val.replace("\n", "")
                     val = striphtml(val)
                     setattr(obj, itm, val)
                 else:
-                    att = Parser.getattrs(line, itm)
-                    if att:
-                        if itm == "link":
-                            itm = "href"
-                        val = Parser.getvalue(att, itm)
-                        if val:
-                            if itm == "href":
-                                itm = "link"
-                            setattr(obj, itm, val.strip())
+                    att = Parser.getattrs(line, toke)
+                    if not att:
+                        continue
+                    if itm == "link":
+                        itm = "href"
+                    val = Parser.getvalue(att, itm)
+                    if not val:
+                        continue
+                    if itm == "href":
+                        itm = "link"
+                    setattr(obj, itm, val.strip())
             result.append(obj)
         return result
 
 
 def getfeed(url, items):
+    "fetch a feed."
+    result = [Object(), Object()]
     if DEBUG:
-        return [Object(), Object()]
+        return result
     try:
-        result = geturl(url)
+        rest = geturl(url)
     except (ValueError, HTTPError, URLError):
-        return [Object(), Object()]
-    if not result:
-        return [Object(), Object()]
-    if url.endswith('atom'):
-        return Parser.parse(str(result.data, 'utf-8'), 'entry', items) or []
-    else:
-        return Parser.parse(str(result.data, 'utf-8'), 'item', items) or []
-    
+        return result
+    if rest:
+        if url.endswith('atom'):
+            result = Parser.parse(str(rest.data, 'utf-8'), 'entry', items) or []
+        else:
+            result = Parser.parse(str(rest.data, 'utf-8'), 'item', items) or []
+    return result
 
 def gettinyurl(url):
+    "fetch a tinyurl."
     postarray = [
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
     req = urllib.request.Request('http://tinyurl.com/create.php',
                   data=bytes(postdata, 'UTF-8'))
@@ -262,69 +288,93 @@
             i = re.search('data-clipboard-text="(.*?)"', line, re.M)
             if i:
                 return i.groups()
     return []
 
 
 def geturl(url):
+    "fetch a url."
     if not url.startswith("http://") and not url.startswith("https://"):
         return ""
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
     req.add_header('User-agent', useragent("rss fetcher"))
     with urllib.request.urlopen(req) as response: # nosec
         response.data = response.read()
         return response
 
 
 def striphtml(text):
+    "strip html."
     clean = re.compile('<.*?>')
     return re.sub(clean, '', text)
 
 
 def unescape(text):
+    "unescape text."
     txt = re.sub(r'\s+', ' ', text)
     return html.unescape(txt)
 
 
 def useragent(txt):
+    "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
 def dpl(event):
+    "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
-    for fnm, feed in find('rss', {'rss': event.args[0]}):
+    for _fn, feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             sync(feed)
     event.reply('ok')
 
 
 Client.add(dpl)
 
 
+def exp(event):
+    "export to opml."
+    event.reply(TEMPLATE)
+    nrs = 0
+    for _fn, obj in find("rss"):
+        nrs += 1
+        name = obj.name or f"url{nrs}"
+        txt = f'<outline name={name} display_list={obj.display_list} xmlUrl="{obj.rss}"/>'
+        event.reply(" "*12 + txt)
+    event.reply(" "*8 + "</outline>")
+    event.reply("    <body>")
+    event.reply("</opml>")
+
+
+Client.add(exp)
+
+
 def nme(event):
+    "set name of feed."
     if len(event.args) != 2:
         event.reply('nme <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
-    for fnm, feed in find('rss', selector):
+    for _fn, feed in find('rss', selector):
         if feed:
             feed.name = event.args[1]
             sync(feed)
     event.reply('ok')
 
 
 Client.add(nme)
 
 
 def rem(event):
+    "remove a feed."
     if len(event.args) != 1:
         event.reply('rem <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector):
         if feed:
             feed.__deleted__ = True
@@ -332,14 +382,15 @@
     event.reply('ok')
 
 
 Client.add(rem)
 
 
 def res(event):
+    "restore a feed."
     if len(event.args) != 1:
         event.reply('res <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector, deleted=True):
         if feed:
             feed.__deleted__ = False
@@ -347,14 +398,15 @@
     event.reply('ok')
 
 
 Client.add(res)
 
 
 def rss(event):
+    "add a feed."
     if not event.rest:
         nrs = 0
         for fnm, feed in find('rss'):
             nrs += 1
             elp = laps(time.time()-fntime(fnm))
             txt = fmt(feed)
             event.reply(f'{nrs} {txt} {elp}')
@@ -372,7 +424,15 @@
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
 
 
 Client.add(rss)
+
+
+TEMPLATE = """<opml version="1.0">
+    <head>
+        <title>rssbot opml</title>
+    </head>
+    <body>
+        <outline title="rssbot opml" text="24/7 feed fetcher">"""
```

### Comparing `botl-105/botl/modules/rst.py` & `botl-106/botl/modules/rst.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,116 +1,138 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0612,W0613
+# pylint: disable=C,R
 
 
 "rest"
 
 
 import os
 import sys
 import time
 
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
+from ..default import Default
 from ..errors  import Errors, debug
-from ..object  import Default, Object
+from ..object  import Object
 from ..persist import Persist, Workdir
 from ..thread  import launch
 
 
 def init():
+    "start object server."
+    result = None
     try:
-        rest = REST((Config.hostname, int(Config.port)), RESTHandler)
+        result = REST((Config.hostname, int(Config.port)), RESTHandler)
     except OSError:
-        return
-    launch(rest.start)
-    return rest
+        pass
+    if result:
+        launch(result.start)
+    return result
 
 
 def html(txt):
-    return """<!doctype html>
-<html>
-   %s
-</html>
-""" % txt
+    "html template."
+    return f"<!doctype html><html>{txt}</html>"
 
 
 class Config(Default):
 
+    "Config"
+
     hostname = "localhost"
     port     = 10102
 
+    def __bla__(self):
+        pass
+
+    def __blabla__(self):
+        pass
+
 
 class REST(HTTPServer, Object):
 
+    "REST"
+
     allow_reuse_address = True
     daemon_thread = True
 
     def __init__(self, *args, **kwargs):
         HTTPServer.__init__(self, *args, **kwargs)
         Object.__init__(self)
         self.host = args[0]
         self._last = time.time()
         self._starttime = time.time()
         self._status = "start"
 
     def exit(self):
+        "shutdown server."
         self._status = ""
         time.sleep(0.2)
         self.shutdown()
 
-    def start(self): 
+    def start(self):
+        "start server/"
         self._status = "ok"
         self.serve_forever()
 
     def request(self):
+        "handler request."
         self._last = time.time()
 
     def error(self, request, addr):
-        exctype, excvalue, tb = sys.exc_info()
+        "handle error."
+        exctype, excvalue, _tb = sys.exc_info()
         exc = exctype(excvalue)
         Errors.add(exc)
-        debug('%s %s' % (addr, excvalue))
+        if request:
+            debug(f'{addr} {excvalue}')
 
 
 class RESTHandler(BaseHTTPRequestHandler):
 
+    "RESTHandler"
+
     def setup(self):
+        "setup request."
         BaseHTTPRequestHandler.setup(self)
         self._ip = self.client_address[0]
         self._size = 0
 
     def send(self, txt):
+        "send text."
         self.wfile.write(bytes(txt, "utf-8"))
         self.wfile.flush()
 
     def write_header(self, htype='text/plain'):
+        "write a header."
         self.send_response(200)
-        self.send_header('Content-type', '%s; charset=%s ' % (htype, "utf-8"))
+        self.send_header('Content-type', f'{htype}; charset="utf-8"')
         self.send_header('Server', "1")
         self.end_headers()
 
-    def do_GET(self):
+    def do_GET(self): # pylint: disable=C0103
+        "handle GET."
         if self.path == "/":
             self.write_header("text/html")
             txt = ""
             for fnm in Persist.fns():
                 txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a>\n'
             self.send(html(txt.strip()))
             return
-        fnm = Workdir.wd + os.sep + "store" + os.sep + self.path
+        fnm = Workdir.workdir + os.sep + "store" + os.sep + self.path
         try:
-            f = open(fnm, "r", encoding="utf-8")
-            txt = f.read()
-            f.close()
-            self.write_header("txt/plain")
-            self.send(html(txt))
+            with open(fnm, "r", encoding="utf-8") as file:
+                txt = file.read()
+                self.write_header("txt/plain")
+                self.send(html(txt))
         except (TypeError, FileNotFoundError, IsADirectoryError) as ex:
             self.send_response(404)
             Errors.add(ex)
             self.end_headers()
 
     def log(self, code):
-        debug('%s code %s path %s' % (self.address_string(), code, self.path))
+        "log access."
+        debug(f"{self.address_string()} code {code} path {self.path}")
```

### Comparing `botl-105/botl/modules/tdo.py` & `botl-106/botl/modules/tdo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,E0402
+# pylint: disable=C,R
 
 
 "todo list"
 
 
 import time
 
 
-from ..handler import Client
+from dataclasses import dataclass
+
+
+from ..client  import Client
 from ..object  import Object
-from ..persist import Persist, fntime, find, laps, sync
+from ..persist import Persist, fntime, find, sync
+from ..utils   import laps
 
 
 class NoDate(Exception):
 
-    pass
+    "NoDate"
 
 
+@dataclass
 class Todo(Object):
 
-    def __init__(self):
-        Object.__init__(self)
-        self.txt = ''
+    "Todo"
+
+    txt: str = ''
 
 
 Persist.add(Todo)
 
 
 def dne(event):
+    "mark todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
     for fnm, obj in find('todo', selector):
         nmr += 1
@@ -45,14 +51,15 @@
         event.reply("nothing todo")
 
 
 Client.add(dne)
 
 
 def tdo(event):
+    "add a todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
```

### Comparing `botl-105/botl/modules/thr.py` & `botl-106/botl/modules/thr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0116,W0105,E0402,E0401,E0611
+# pylint: disable=C,R
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
+from ..client  import Client
 from ..object  import Object, update
-from ..handler import Client
-from ..persist import laps
+from ..utils   import laps
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
+    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
```

### Comparing `botl-105/botl/modules/tmr.py` & `botl-106/botl/modules/tmr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0612,W0105,W0702,E0402
+# pylint: disable=C,R
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
-from ..broker import Broker
-from ..handler import Client, Event
-from ..object import update
-from ..persist import Persist, find, laps, sync
-from ..thread import Timer, launch
+from ..broker  import Broker
+from ..client  import Client
+from ..event   import Event
+from ..object  import update
+from ..persist import Persist, find, sync
+from ..thread  import launch
+from ..timer   import Timer
+from ..utils   import laps
 
 
 def init():
-    for fnm, obj in find("timer"):
+    "start timers."
+    for _fn, obj in find("timer"):
         if "time" not in obj:
             continue
         diff = float(obj.time) - ttime.time()
         if diff > 0:
             bot = Broker.first()
             evt = Event()
             update(evt, obj)
@@ -55,31 +59,34 @@
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    pass
+    "NoDate"
 
 
 Persist.add(Timer)
 
 
 def extract_date(daystr):
+    "extract date from string."
+    res = None
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
+            break
         except ValueError:
             res = None
-        if res:
-            return res
+    return res
 
 
 def get_day(daystr):
+    "return day from string."
     day = None
     month = None
     yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
         if ymdre:
             (day, month, yea) = ymdre.groups()
@@ -91,20 +98,21 @@
                 yea = ttime.strftime("%Y", ttime.localtime())
         except Exception as ex:
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
-        date = "%s %s %s" % (day, MONTHS[month], yea)
+        date = f"{day} {MONTHS[month]} {yea}"
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
     raise NoDate(daystr)
 
 
 def get_hour(daystr):
+    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -118,25 +126,27 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
+    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
 def parse_time(txt):
+    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -151,78 +161,77 @@
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
 def to_day(daystr):
+    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
+    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
+            break
         except ValueError:
             res = None
-        if res:
-            return res
         line = ""
+    return res
 
 
 def today():
+    "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
-"commands"
-
-
 def tmr(event):
+    "add a timer."
+    result = ""
     if not event.rest:
         nmr = 0
-        for fnm, obj in find('timer'):
-            if "time" not in obj:
-                continue
+        for _fn, obj in find('timer'):
             lap = float(obj.time) - ttime.time()
             if lap > 0:
                 event.reply(f'{nmr} {obj.txt} {laps(lap)}')
                 nmr += 1
-        if not nmr:
-            event.reply("no timers")
-        return
+        return result
     seconds = 0
     line = ""
     for word in event.args:
         if word.startswith("+"):
             try:
                 seconds = int(word[1:])
             except (ValueError, IndexError):
-                event.reply("%s is not an integer" % seconds)
-                return
+                event.reply(f"{seconds} is not an integer")
+                return result
         else:
             line += word + " "
     if seconds:
         target = ttime.time() + seconds
     else:
         try:
             target = get_day(event.rest)
         except NoDate:
             target = to_day(today())
         hour =  get_hour(event.rest)
         if hour:
             target += hour
     if not target or ttime.time() > target:
         event.reply("already passed given time.")
-        return
+        return result
     event.time = target
     diff = target - ttime.time()
     event.reply("ok " +  laps(diff))
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
+    return result
 
 
 Client.add(tmr)
```

### Comparing `botl-105/botl/modules/udp.py` & `botl-106/botl/modules/udp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0115,C0116,W0105,E0402,R0903
+# pylint: disable=C,R
 
 
 "udp to irc relay"
 
 
 import select
 import socket
 import sys
 import threading
 import time
 
 
+from dataclasses import dataclass
+
+
 from ..broker import Broker
-from ..handler import Client
+from ..client import Client
 from ..object import Object
 from ..thread import launch
 
 
 def init():
+    "start udp to irc relay."
     udpd = UDP()
     udpd.start()
     return udpd
 
 
+@dataclass
 class Cfg(Object):
 
+    "Cfg"
+
     addr = ""
     host = "localhost"
     port = 5500
 
 
 class UDP(Object):
 
+    "UDP"
+
     def __init__(self):
         Object.__init__(self)
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.ready = threading.Event()
 
     def output(self, txt, addr=None):
+        "output to fleet."
         if addr:
             Cfg.addr = addr
         for bot in Broker.all():
             bot.announce(txt.replace("\00", ""))
 
     def loop(self):
+        "udp input loop."
         try:
             self._sock.bind((Cfg.host, Cfg.port))
         except socket.gaierror:
             return
         self.ready.set()
         while not self.stopped:
             (txt, addr) = self._sock.recvfrom(64000)
@@ -62,31 +73,35 @@
                 break
             data = str(txt.rstrip(), "utf-8")
             if not data:
                 break
             self.output(data, addr)
 
     def exit(self):
+        "stop relay."
         self.stopped = True
         self._sock.settimeout(0.01)
         self._sock.sendto(
                           bytes("exit", "utf-8"),
                           (Cfg.host, Cfg.port)
                          )
 
     def start(self):
+        "start relay."
         launch(self.loop)
 
 
 def toudp(host, port, txt):
+    "send udp packet to bot."
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
 def udp(event):
+    "send udp command."
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
         event.reply(f"{len(event.rest)} characters sent")
         return
     if not select.select(
                          [sys.stdin, ],
                          [],
```

### Comparing `botl-105/botl/object.py` & `botl-106/botl/object.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0613,E0101
+# pylint: disable=C,R,W0105
 
 
-"""a clean namespace
-
-This module allows for easy json save//load to/from disk of objects. It
-provides an "clean namespace" Object class that only has dunder
-methods, so the namespace is not cluttered with method names. This makes
-storing and reading to/from json possible.
-
-"""
+"object"
 
 
 import json
 import os
 import pathlib
 import _thread
 
 
 disklock = _thread.allocate_lock()
 
 
 class Object:
 
-    "Base class."
+    "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
@@ -163,18 +156,18 @@
         cdir(os.path.dirname(pth))
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
-    "Object decoded"
+    "ObjectDecoder"
 
     def __init__(self, *args, **kwargs):
-        return json.JSONDecoder.__init__(self, *args)
+        json.JSONDecoder.__init__(self, *args, **kwargs)
 
     def decode(self, s, _w=None):
         "decoding string to object."
         val = json.JSONDecoder.decode(self, s)
         if not val:
             val = {}
         return hook(val)
@@ -206,18 +199,18 @@
     kw["cls"] = ObjectDecoder
     kw["object_hook"] = hook
     return json.loads(string, *args, **kw)
 
 
 class ObjectEncoder(json.JSONEncoder):
 
-    "Object encoder."
+    "ObjectEncoder"
 
     def __init__(self, *args, **kwargs):
-        return json.JSONEncoder.__init__(self, *args, **kwargs)
+        json.JSONEncoder.__init__(self, *args, **kwargs)
 
     def default(self, o):
         "return stringable value."
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
             return vars(o)
@@ -247,51 +240,27 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
-class Default(Object):
-
-    "Object that return a default value if key does not exist."
-
-    __slots__ = ("__default__",)
-
-    def __init__(self):
-        Object.__init__(self)
-        self.__default__ = ""
-
-    def __getattr__(self, key):
-        return self.__dict__.get(key, self.__default__)
-
-
 def cdir(pth):
     "create directory."
     if os.path.exists(pth):
         return
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
-def spl(txt):
-    "split comma separated string into a list."
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
-
-
 "interface"
 
 
 def __dir__():
     return (
-        'Default',
         'Object',
         'construct',
         'dump',
         'dumps',
         'edit',
         'fmt',
         'fqn',
```

### Comparing `botl-105/botl/persist.py` & `botl-106/botl/persist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,28 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,E0402
+# pylint: disable=C,R,W0105
 
 
-"""persistence
-
-Object persistence.
-
-"""
+"persist"
 
 
 import datetime
 import os
 import time
 
 
-from .object import Default, Object, cdir, fqn, read, search, update, write
-
-
-class Workdir(Object):
-
-    "directory to store objects."
-
-    wd = ""
-
-    @staticmethod
-    def skel():
-        "create directory,"
-        cdir(os.path.join(Workdir.wd, "store", ""))
-
-    @staticmethod
-    def store(pth=""):
-        "return objects directory."
-        return os.path.join(Workdir.wd, "store", pth)
-
-    @staticmethod
-    def strip(pth, nmr=3):
-        "reduce to path with directory."
-        return os.sep.join(pth.split(os.sep)[-nmr:])
-
-    @staticmethod
-    def types():
-        "return types stored."
-        return os.listdir(Workdir.store())
+from .default import Default
+from .object  import Object, fqn, read, search, update, write
+from .workdir import Workdir
 
 
 class Persist(Object):
 
-    "whitelist of types saveable to disk."
+    "Persist"
 
     classes = Object()
 
     @staticmethod
     def add(clz):
         "add class to whitelist."
         name = str(clz).split()[1][1:-2]
@@ -84,54 +55,14 @@
             for fnm in Workdir.types():
                 claz = fnm.split(".")[-1]
                 if fnm == claz.lower():
                     res = fnm
         return res
 
 
-def laps(seconds, short=True):
-    "show elapsed time."
-    txt = ""
-    nsec = float(seconds)
-    if nsec < 1:
-        return f"{nsec:.2f}s"
-    yea = 365*24*60*60
-    week = 7*24*60*60
-    nday = 24*60*60
-    hour = 60*60
-    minute = 60
-    yeas = int(nsec/yea)
-    nsec -= yeas*yea
-    weeks = int(nsec/week)
-    nsec -= weeks*week
-    nrdays = int(nsec/nday)
-    nsec -= nrdays*nday
-    hours = int(nsec/hour)
-    nsec -= hours*hour
-    minutes = int(nsec/minute)
-    nsec -= int(minute*minutes)
-    sec = int(nsec)
-    if yeas:
-        txt += f"{yeas}y"
-    if weeks:
-        nrdays += weeks * 7
-    if nrdays:
-        txt += f"{nrdays}d"
-    if short and txt:
-        return txt.strip()
-    if hours:
-        txt += f"{hours}h"
-    if minutes:
-        txt += f"{minutes}m"
-    if sec:
-        txt += f"{sec}s"
-    txt = txt.strip()
-    return txt
-
-
 def fntime(daystr):
     "convert file name to it's saved time."
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
         datestr, rest = datestr.rsplit('.', 1)
     else:
@@ -141,24 +72,24 @@
         timed += float('.' + rest)
     return timed
 
 
 def find(mtc, selector=None, index=None, deleted=False):
     "find object matching the selector dict."
     clz = Persist.long(mtc)
-    nr = -1
+    nrs = -1
     for fnm in sorted(Persist.fns(clz), key=fntime):
         obj = Default()
         fetch(obj, fnm)
         if not deleted and '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
-        nr += 1 
-        if index is not None and nr != int(index):
+        nrs += 1
+        if index is not None and nrs != int(index):
             continue
         yield (fnm, obj)
 
 
 def fetch(obj, pth):
     "read object from disk."
     pth2 = Workdir.store(pth)
@@ -169,27 +100,29 @@
 def ident(obj):
     "return an id for an object."
     return os.path.join(
                         fqn(obj),
                         os.path.join(*str(datetime.datetime.now()).split())
                        )
 
+
 def last(obj, selector=None):
     "return last object saved."
     if selector is None:
         selector = {}
     result = sorted(
                     find(fqn(obj), selector),
                     key=lambda x: fntime(x[0])
                    )
+    res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
-        return inp[0]
-
+        res = inp[0]
+    return res
 
 def sync(obj, pth=None):
     "sync object to disk."
     if pth is None:
         pth = ident(obj)
     pth2 = Workdir.store(pth)
     write(obj, pth2)
@@ -198,21 +131,17 @@
 
 "interface"
 
 
 def __dir__():
     return (
         'Persist',
-        'Workdir',
         'fetch',
         'fntime',
         'find',
-        'laps',
         'last',
         'ident',
-        'read',
         'sync',
-        'write'
     )
 
 
 __all__ = __dir__()
```

### Comparing `botl-105/botl.egg-info/PKG-INFO` & `botl-106/botl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 105
-Summary: cli bot
+Version: 106
+Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
@@ -22,15 +22,15 @@
 
 
 SYNOPSIS
 
 ::
 
     botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v] [-w]
+    botl [-a] [-c] [-d] [-h] [-v]
 
     options are:
 
     -a     load all modules
     -c     start console
     -d     start daemon
     -h     display help
```

### Comparing `botl-105/botl.egg-info/SOURCES.txt` & `botl-106/botl.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 README.rst
 pyproject.toml
 setup.py
 botl/__init__.py
 botl/__main__.py
 botl/broker.py
+botl/client.py
+botl/default.py
 botl/errors.py
+botl/event.py
 botl/handler.py
 botl/object.py
+botl/parser.py
 botl/persist.py
+botl/repeater.py
 botl/thread.py
+botl/timer.py
+botl/utils.py
+botl/workdir.py
 botl.egg-info/PKG-INFO
 botl.egg-info/SOURCES.txt
 botl.egg-info/dependency_links.txt
 botl.egg-info/entry_points.txt
 botl.egg-info/top_level.txt
 botl.egg-info/zip-safe
 botl/modules/__init__.py
 botl/modules/cmd.py
+botl/modules/dbg.py
 botl/modules/err.py
 botl/modules/flt.py
 botl/modules/fnd.py
 botl/modules/irc.py
 botl/modules/log.py
 botl/modules/mbx.py
 botl/modules/mdl.py
```

### Comparing `botl-105/pyproject.toml` & `botl-106/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "botl"
-description = "cli bot"
-version = "105"
+description = "bot library"
+version = "106"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```


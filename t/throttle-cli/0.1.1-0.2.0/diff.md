# Comparing `tmp/throttle_cli-0.1.1.tar.gz` & `tmp/throttle_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_cli-0.1.1.tar", max compression
+gzip compressed data, was "throttle_cli-0.2.0.tar", max compression
```

## Comparing `throttle_cli-0.1.1.tar` & `throttle_cli-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    13827 2024-03-04 13:14:43.080562 throttle_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     8403 2024-03-22 15:22:58.119825 throttle_cli-0.1.1/README.md
--rw-r--r--   0        0        0      756 2024-03-22 15:40:39.683718 throttle_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-17 19:54:08.955808 throttle_cli-0.1.1/throttle_cli/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-17 12:39:35.583256 throttle_cli-0.1.1/throttle_cli/cli.py
--rw-r--r--   0        0        0     1018 2024-03-17 15:36:30.340119 throttle_cli-0.1.1/throttle_cli/client.py
--rw-r--r--   0        0        0     8949 2024-03-11 14:10:27.798587 throttle_cli-0.1.1/throttle_cli/commandworker.py
--rw-r--r--   0        0        0     1439 2024-02-29 20:24:41.296737 throttle_cli-0.1.1/throttle_cli/loglib.py
--rw-r--r--   0        0        0     1490 2024-03-12 22:07:09.496788 throttle_cli-0.1.1/throttle_cli/server.py
--rw-r--r--   0        0        0     1030 2024-03-10 20:42:54.382440 throttle_cli-0.1.1/throttle_cli/structures.py
--rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 throttle_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-03-04 13:14:43.080562 throttle_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9213 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      756 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-17 19:54:08.955808 throttle_cli-0.2.0/throttle_cli/__init__.py
+-rw-r--r--   0        0        0     1197 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/arglib.py
+-rw-r--r--   0        0        0     1777 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/cli.py
+-rw-r--r--   0        0        0     1287 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/client.py
+-rw-r--r--   0        0        0     9009 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/commandworker.py
+-rw-r--r--   0        0        0     1439 2024-02-29 20:24:41.296737 throttle_cli-0.2.0/throttle_cli/loglib.py
+-rw-r--r--   0        0        0     1490 2024-03-12 22:07:09.496788 throttle_cli-0.2.0/throttle_cli/server.py
+-rw-r--r--   0        0        0     1155 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/structures.py
+-rw-r--r--   0        0        0     9940 1970-01-01 00:00:00.000000 throttle_cli-0.2.0/PKG-INFO
```

### Comparing `throttle_cli-0.1.1/LICENSE` & `throttle_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.1.1/README.md` & `throttle_cli-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,25 +75,28 @@
 a couple of hundred times before the first one finishes, `throttle` will queue
 up a single other instance of `mbsync inbox` after the first one finished.
 
 
 ## Usage
 
 ```
-usage: throttle [-h] [-s | -j JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+usage: throttle [-h] [-s | -j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
 
 options:
   -h, --help            show this help message and exit
   -s, --server          Start server.
   -j JOB, --job JOB     Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.
+  -J SILENT_JOB, --silent-job SILENT_JOB
+                        Same as --job, but no notifications will be sent on failure.
   -k, --kill            Kill a previously started job.
   -o ORIGIN, --origin ORIGIN
                         Set the origin of the message, which might be useful in tracking logs.
   --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
                         Set loglevel.
+
 ```
 
 First start a server with `throttle --server`. It will log to
 `$XDG_STATE/throttle/throttle.log`, which should default to
 `~/.local/state/throttle/throttle.log`.
 
 To start a job run `throttle my command` which will run `my command`. You can
@@ -122,14 +125,31 @@
 
 Practical usage of a multiple commands would be something like:
 
 ```
 throttle --job "mbsync personal-inbox" --job "notmuch new"
 ```
 
+The silent jobs can be used to check for prerequisite of commands. E.g. after moving a message locally one might run:
+
+```
+throttle \
+  --job "notmuch new" \
+  --silent-job "testinternetconnection" \
+  --job "mbsync personal-inbox" \
+  --job "notmuch new"
+```
+
+This first syncs the notmuch database locally, then checks for internet
+connectivity (see
+[this](https://github.com/ferdinandyb/dotfiles/blob/master/bin/testinternetconnection)
+for an example), which will silently continue to be checked until internet is
+back, then after internet is back, sync the local folder with the server and
+finally run notmuch again to include the changes pulled from the server.
+
 ## Configuration
 
 Configuration happens in `$XDG_CONFIG/throttle/config.toml`.
 
 Example config:
 
 ```
```

### Comparing `throttle_cli-0.1.1/pyproject.toml` & `throttle_cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "throttle-cli"
-version = "0.1.1"
+version = "0.2.0"
 description = "Throttle commands triggered from multiple async sources."
 authors = ["Bence Ferdinandy <bence@ferdinandy.com>"]
 readme = "README.md"
 license = "EUPL-1.2"
 homepage = "https://sr.ht/~ferdinandyb/throttle/"
 
 [tool.poetry.dependencies]
```

### Comparing `throttle_cli-0.1.1/throttle_cli/cli.py` & `throttle_cli-0.2.0/throttle_cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import logging
 from pathlib import Path
 
 from xdg import BaseDirectory
 
 from .client import send_message
 from .server import start_server
+from .arglib import storeJob, storeSilentJob
 
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser()
     group = parser.add_mutually_exclusive_group()
     group.add_argument("-s", "--server", action="store_true", help="Start server.")
     group.add_argument(
         "-j",
         "--job",
-        action="append",
+        action=storeJob,
         help="Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.",
     )
     parser.add_argument(
+        "-J",
+        "--silent-job",
+        action=storeSilentJob,
+        help="Same as --job, but no notifications will be sent on failure.",
+    )
+    parser.add_argument(
         "-k", "--kill", action="store_true", help="Kill a previously started job."
     )
     parser.add_argument(
         "-o",
         "--origin",
         type=str,
         help="Set the origin of the message, which might be useful in tracking logs.",
@@ -37,13 +44,18 @@
     socketpath = Path(BaseDirectory.get_runtime_dir()) / "throttle.sock"
     loglevel = logging.INFO
     if args.LOGLEVEL:
         loglevel = getattr(logging, args.LOGLEVEL)
     if args.server:
         start_server(socketpath, loglevel)
         return
-
-    send_message(socketpath, args.kill, args.job, args.origin, unknownargs)
+    if hasattr(args, "notifications"):
+        notifications = args.notifications
+    else:
+        notifications = []
+    send_message(
+        socketpath, args.kill, args.job, notifications, args.origin, unknownargs
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `throttle_cli-0.1.1/throttle_cli/client.py` & `throttle_cli-0.2.0/throttle_cli/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,47 @@
 
 from jsonrpclib import ServerProxy
 
 from .structures import ActionType
 
 
 def send_message(
-    socketpath: Path, kill: bool, jobs: List[str], origin: str, unknownargs: List[str]
+    socketpath: Path,
+    kill: bool,
+    jobs: List[str],
+    notifications: List[int],
+    origin: str,
+    unknownargs: List[str],
 ) -> None:
     if not socketpath.exists():
         print("socket doesn't exist, is throttle running?")
         import sys
 
         sys.exit(1)
     action = ActionType.KILL if kill else ActionType.RUN
     mergedjobs: List[str] = []
+    if notifications is None:
+        notifications = []
     if jobs is not None:
         mergedjobs += jobs
     if len(unknownargs) > 0:
         mergedjobs += [" ".join(unknownargs)]
+        notifications.append(1)
     if len(mergedjobs) == 0:
         return
     try:
         client = ServerProxy(f"unix+http://{socketpath}")
-        client.handle({"action": action, "jobs": mergedjobs, "origin": origin})
+        client.handle(
+            {
+                "action": action,
+                "jobs": mergedjobs,
+                "notifications": notifications,
+                "origin": origin,
+            }
+        )
         client("close")()
     except ConnectionRefusedError:
         import sys
 
         print(
             "Connection refused: did you start the server with `throttle --server`?",
             file=sys.stderr,
```

### Comparing `throttle_cli-0.1.1/throttle_cli/commandworker.py` & `throttle_cli-0.2.0/throttle_cli/commandworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,27 +190,27 @@
                     )
                     if proc.returncode != 0:
                         success = False
                         error_counter += 1
                         logger.error(
                             f"{proc.returncode=}, {proc.stdout=}, {proc.stderr=}, {error_counter=}"
                         )
-                        if error_counter >= self.notify_on_counter:
+                        if error_counter >= self.notify_on_counter and msg.notification:
                             self.sendNotification(
                                 job=msg.job,
                                 origin=msg.origin,
                                 msg=f"c:{error_counter}|{proc.stderr.decode('utf-8')} - {proc.stdout.decode('utf-8')}",
                                 errcode=proc.returncode,
                             )
                             error_counter = 0
                 except Exception as error:
                     success = False
                     error_counter += 1
                     logger.error(f"{msg.job}'s subprocess failed with {error}")
-                    if error_counter >= self.notify_on_counter:
+                    if error_counter >= self.notify_on_counter and msg.notification:
                         self.sendNotification(
                             job=msg.job,
                             origin=msg.origin,
                             msg=f"subprocess failed with {error}",
                         )
                         error_counter = 0
 
@@ -240,10 +240,10 @@
                     else:
                         logger.info("handling CONT")
                     if msg.next():
                         self.q.put(msg)
                 except queue.Empty:
                     logger.info("closing process")
                     break
-            self.q.put(Msg(jobs=[], action=ActionType.CLEAN))
+            self.q.put(Msg(jobs=[], notifications=[], action=ActionType.CLEAN))
 
         return worker
```

### Comparing `throttle_cli-0.1.1/throttle_cli/loglib.py` & `throttle_cli-0.2.0/throttle_cli/loglib.py`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.1.1/throttle_cli/server.py` & `throttle_cli-0.2.0/throttle_cli/server.py`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.1.1/throttle_cli/structures.py` & `throttle_cli-0.2.0/throttle_cli/structures.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,26 +9,31 @@
     KILL = auto()  # kill job
     CLEAN = auto()  # clear up dangling jobs
 
 
 @dataclass
 class Msg:
     jobs: List[str]
+    notifications: List[int]
     action: ActionType
     index: int = 0
     origin: str = ""
 
     @property
     def job(self) -> str:
         return self.jobs[self.index]
 
     @job.setter
     def job(self, j) -> None:
         self.jobs[self.index] = j
 
+    @property
+    def notification(self) -> int:
+        return self.notifications[self.index]
+
     def next(self):
         """
         Set the next job as executable.
         """
 
         if self.index < len(self.jobs) - 1:
             self.action = ActionType.RUN
```

### Comparing `throttle_cli-0.1.1/PKG-INFO` & `throttle_cli-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Throttle commands triggered from multiple async sources.
 Home-page: https://sr.ht/~ferdinandyb/throttle/
 License: EUPL-1.2
 Author: Bence Ferdinandy
 Author-email: bence@ferdinandy.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -94,25 +94,28 @@
 a couple of hundred times before the first one finishes, `throttle` will queue
 up a single other instance of `mbsync inbox` after the first one finished.
 
 
 ## Usage
 
 ```
-usage: throttle [-h] [-s | -j JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+usage: throttle [-h] [-s | -j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
 
 options:
   -h, --help            show this help message and exit
   -s, --server          Start server.
   -j JOB, --job JOB     Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.
+  -J SILENT_JOB, --silent-job SILENT_JOB
+                        Same as --job, but no notifications will be sent on failure.
   -k, --kill            Kill a previously started job.
   -o ORIGIN, --origin ORIGIN
                         Set the origin of the message, which might be useful in tracking logs.
   --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
                         Set loglevel.
+
 ```
 
 First start a server with `throttle --server`. It will log to
 `$XDG_STATE/throttle/throttle.log`, which should default to
 `~/.local/state/throttle/throttle.log`.
 
 To start a job run `throttle my command` which will run `my command`. You can
@@ -141,14 +144,31 @@
 
 Practical usage of a multiple commands would be something like:
 
 ```
 throttle --job "mbsync personal-inbox" --job "notmuch new"
 ```
 
+The silent jobs can be used to check for prerequisite of commands. E.g. after moving a message locally one might run:
+
+```
+throttle \
+  --job "notmuch new" \
+  --silent-job "testinternetconnection" \
+  --job "mbsync personal-inbox" \
+  --job "notmuch new"
+```
+
+This first syncs the notmuch database locally, then checks for internet
+connectivity (see
+[this](https://github.com/ferdinandyb/dotfiles/blob/master/bin/testinternetconnection)
+for an example), which will silently continue to be checked until internet is
+back, then after internet is back, sync the local folder with the server and
+finally run notmuch again to include the changes pulled from the server.
+
 ## Configuration
 
 Configuration happens in `$XDG_CONFIG/throttle/config.toml`.
 
 Example config:
 
 ```
```


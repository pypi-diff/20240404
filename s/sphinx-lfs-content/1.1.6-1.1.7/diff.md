# Comparing `tmp/sphinx_lfs_content-1.1.6.tar.gz` & `tmp/sphinx_lfs_content-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_lfs_content-1.1.6.tar", last modified: Mon Jan 22 09:29:12 2024, max compression
+gzip compressed data, was "sphinx_lfs_content-1.1.7.tar", last modified: Thu Apr  4 14:04:16 2024, max compression
```

## Comparing `sphinx_lfs_content-1.1.6.tar` & `sphinx_lfs_content-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:29:12.094513 sphinx_lfs_content-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-22 09:29:12.094513 sphinx_lfs_content-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-22 09:29:11.000000 sphinx_lfs_content-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 09:29:12.094513 sphinx_lfs_content-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-22 09:29:11.000000 sphinx_lfs_content-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:29:12.094513 sphinx_lfs_content-1.1.6/sphinx_lfs_content/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-01-22 09:29:11.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:29:12.094513 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-22 09:29:12.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-22 09:29:12.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 09:29:12.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-22 09:29:12.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-22 09:29:12.000000 sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:04:16.074915 sphinx_lfs_content-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-04 14:04:16.070915 sphinx_lfs_content-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-04 14:04:15.000000 sphinx_lfs_content-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:04:16.074915 sphinx_lfs_content-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 14:04:15.000000 sphinx_lfs_content-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:04:16.070915 sphinx_lfs_content-1.1.7/sphinx_lfs_content/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-04 14:04:15.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:04:16.070915 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-04 14:04:16.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 14:04:16.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:04:16.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:04:16.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 14:04:16.000000 sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/top_level.txt
```

### Comparing `sphinx_lfs_content-1.1.6/PKG-INFO` & `sphinx_lfs_content-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_lfs_content
-Version: 1.1.6
+Version: 1.1.7
 Summary: Ensure existence of LFS content in your LFS builds
 Home-page: UNKNOWN
 Author: Dominic Kempf
 Author-email: dominic.kempf@iwr.uni-heidelberg.de
 License: UNKNOWN
 Description: # sphinx_lfs_content
```

### Comparing `sphinx_lfs_content-1.1.6/README.md` & `sphinx_lfs_content-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_lfs_content-1.1.6/setup.py` & `sphinx_lfs_content-1.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="sphinx_lfs_content",
-    version="1.1.6",
+    version="1.1.7",
     author="Dominic Kempf",
     author_email="dominic.kempf@iwr.uni-heidelberg.de",
     description="Ensure existence of LFS content in your LFS builds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

### Comparing `sphinx_lfs_content-1.1.6/sphinx_lfs_content/__init__.py` & `sphinx_lfs_content-1.1.7/sphinx_lfs_content/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import shutil
 import sphinx
 import subprocess
 import tarfile
 import tempfile
 
 
-GIT_LFS_FILE = "https://github.com/git-lfs/git-lfs/releases/download/v3.4.1/git-lfs-linux-amd64-v3.4.1.tar.gz"
-GIT_LFS_CHECKSUM = "1772dc260961db27958088740b7e9ecebf945abad8c2d504d412448f53faf147"
+GIT_LFS_FILE = "https://github.com/git-lfs/git-lfs/releases/download/v3.5.1/git-lfs-linux-amd64-v3.5.1.tar.gz"
+GIT_LFS_CHECKSUM = "6f28eb19faa7a968882dca190d92adc82493378b933958d67ceaeb9ebe4d731e"
 
 
 def lfs_setup(_, config):
     # If we already have git-lfs, we do not need to set it up
     if shutil.which("git-lfs") is None:
         # Download the latest git-lfs tarball and check its checksum
         git_lfs_content = requests.get(GIT_LFS_FILE).content
@@ -31,15 +31,15 @@
             with tarfile.open(os.path.join(tmp_dir, "git-lfs.tar.gz"), "r:gz") as tar:
                 tar.extractall(path=tmp_dir)
 
             # Setup a modified environment that has the temporary directory in PATH
             # This works around a bug in git-lfs where git-lfs is called recursively,
             # but the inner calls rely on git-lfs being in PATH.
             env = os.environ
-            env["PATH"] = os.environ["PATH"] + os.path.pathsep + os.path.join(tmp_dir, "git-lfs-3.4.1")
+            env["PATH"] = os.environ["PATH"] + os.path.pathsep + os.path.join(tmp_dir, "git-lfs-3.5.1")
 
             # Fetch the LFS content of the repository
             subprocess.check_call("git-lfs install".split(), env=env)
             subprocess.check_call("git-lfs fetch".split(), env=env)
             subprocess.check_call("git-lfs checkout".split(), env=env)
 
     # Execute all of the given post commands
@@ -47,8 +47,8 @@
         subprocess.check_call(cmd, shell=True)
 
 
 def setup(app):
     app.add_config_value("lfs_content_post_commands", [], rebuild="")
     app.connect("config-inited", lfs_setup)
 
-    return {"version": "1.1.6", "parallel_read_safe": True}
+    return {"version": "1.1.7", "parallel_read_safe": True}
```

### Comparing `sphinx_lfs_content-1.1.6/sphinx_lfs_content.egg-info/PKG-INFO` & `sphinx_lfs_content-1.1.7/sphinx_lfs_content.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-lfs-content
-Version: 1.1.6
+Version: 1.1.7
 Summary: Ensure existence of LFS content in your LFS builds
 Home-page: UNKNOWN
 Author: Dominic Kempf
 Author-email: dominic.kempf@iwr.uni-heidelberg.de
 License: UNKNOWN
 Description: # sphinx_lfs_content
```


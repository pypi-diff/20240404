# Comparing `tmp/aic_tools_alpaca-0.0.2.tar.gz` & `tmp/aic_tools_alpaca-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aic_tools_alpaca-0.0.2.tar", last modified: Tue Apr  2 01:11:55 2024, max compression
+gzip compressed data, was "aic_tools_alpaca-0.0.3.tar", last modified: Thu Apr  4 04:09:58 2024, max compression
```

## Comparing `aic_tools_alpaca-0.0.2.tar` & `aic_tools_alpaca-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-02 01:11:55.471109 aic_tools_alpaca-0.0.2/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-02 01:11:55.470984 aic_tools_alpaca-0.0.2/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      584 2024-04-02 01:02:37.000000 aic_tools_alpaca-0.0.2/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-02 01:11:55.470815 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-02 01:11:55.000000 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      217 2024-04-02 01:11:55.000000 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-02 01:11:55.000000 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       18 2024-04-02 01:11:55.000000 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-02 01:11:55.000000 aic_tools_alpaca-0.0.2/aic_tools_alpaca.egg-info/top_level.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-02 01:11:55.471164 aic_tools_alpaca-0.0.2/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      734 2024-04-02 01:11:53.000000 aic_tools_alpaca-0.0.2/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.505378 aic_tools_alpaca-0.0.3/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-04 04:09:58.505253 aic_tools_alpaca-0.0.3/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      584 2024-04-02 01:02:37.000000 aic_tools_alpaca-0.0.3/README.md
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.504459 aic_tools_alpaca-0.0.3/aic_tools_alpaca/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:50.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      716 2024-04-04 04:09:41.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca/account_info.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.505083 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      279 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       18 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       17 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/top_level.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-04 04:09:58.505421 aic_tools_alpaca-0.0.3/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      734 2024-04-04 04:09:55.000000 aic_tools_alpaca-0.0.3/setup.py
```

### Comparing `aic_tools_alpaca-0.0.2/README.md` & `aic_tools_alpaca-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aic_tools_alpaca-0.0.2/setup.py` & `aic_tools_alpaca-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='aic_tools_alpaca',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     description='Alpaca tools for AI Characters',
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
     install_requires=install_requires
```


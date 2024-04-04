# Comparing `tmp/sentralify-1.2.3.tar.gz` & `tmp/sentralify-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentralify-1.2.3.tar", last modified: Wed Apr  3 04:46:45 2024, max compression
+gzip compressed data, was "sentralify-1.2.4.tar", last modified: Thu Apr  4 09:11:43 2024, max compression
```

## Comparing `sentralify-1.2.3.tar` & `sentralify-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 04:46:45.954499 sentralify-1.2.3/
--rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.3/LICENSE
--rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-03 04:46:45.954499 sentralify-1.2.3/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)    16147 2024-04-03 04:46:44.000000 sentralify-1.2.3/README.md
--rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-03 04:46:33.000000 sentralify-1.2.3/pyproject.toml
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-03 04:46:45.954499 sentralify-1.2.3/setup.cfg
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.3/setup.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 04:46:45.951166 sentralify-1.2.3/src/
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 04:46:45.954499 sentralify-1.2.3/src/sentralify/
--rw-r--r--   0 James     (1000) James     (1000)     4032 2024-04-03 04:46:44.000000 sentralify-1.2.3/src/sentralify/__init__.py
--rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-03 04:46:44.000000 sentralify-1.2.3/src/sentralify/generators.py
--rw-r--r--   0 James     (1000) James     (1000)    12503 2024-04-03 04:46:44.000000 sentralify-1.2.3/src/sentralify/scrapers.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 04:46:45.954499 sentralify-1.2.3/src/sentralify.egg-info/
--rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-03 04:46:45.000000 sentralify-1.2.3/src/sentralify.egg-info/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-03 04:46:45.000000 sentralify-1.2.3/src/sentralify.egg-info/SOURCES.txt
--rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-03 04:46:45.000000 sentralify-1.2.3/src/sentralify.egg-info/dependency_links.txt
--rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-03 04:46:45.000000 sentralify-1.2.3/src/sentralify.egg-info/requires.txt
--rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-03 04:46:45.000000 sentralify-1.2.3/src/sentralify.egg-info/top_level.txt
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/
+-rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.4/LICENSE
+-rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-04 09:11:43.590543 sentralify-1.2.4/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)    16147 2024-04-04 09:11:42.000000 sentralify-1.2.4/README.md
+-rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-04 09:11:04.000000 sentralify-1.2.4/pyproject.toml
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-04 09:11:43.590543 sentralify-1.2.4/setup.cfg
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.4/setup.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.587210 sentralify-1.2.4/src/
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/src/sentralify/
+-rw-r--r--   0 James     (1000) James     (1000)     4032 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/__init__.py
+-rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/generators.py
+-rw-r--r--   0 James     (1000) James     (1000)    12504 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/scrapers.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/src/sentralify.egg-info/
+-rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/SOURCES.txt
+-rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/dependency_links.txt
+-rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/requires.txt
+-rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/top_level.txt
```

### Comparing `sentralify-1.2.3/LICENSE` & `sentralify-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.3/PKG-INFO` & `sentralify-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.3
+Version: 1.2.4
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sentralify-1.2.3/README.md` & `sentralify-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.3/pyproject.toml` & `sentralify-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentralify"
-version = "1.2.3"
+version = "1.2.4"
 description = "Scrape Sentral data and use it!"
 readme = "README.md"
 authors = [{ name = "mario872", email = "jamesaglynn10@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sentralify-1.2.3/src/sentralify/__init__.py` & `sentralify-1.2.4/src/sentralify/__init__.py`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.3/src/sentralify/generators.py` & `sentralify-1.2.4/src/sentralify/generators.py`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.3/src/sentralify/scrapers.py` & `sentralify-1.2.4/src/sentralify/scrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             # Logging in using Microsoft account
             if not found_email_address:
                 page.get_by_placeholder(re.compile("Use your email address")).fill(f'{self.config["username"]}@education.{self.config["state"]}.gov.au')
                 page.get_by_role("button", name="Next").click()
                 
             page.get_by_placeholder("Enter your password").fill(self.config['password'])
             page.get_by_role("button", name="Sign in").click()
-            page.get_by_role("button", name="No").click()
+            page.get_by_role("button", name="Yes").click()
             
             try: # We expect that we will be logged into Sentral by now
                 expect(page).to_have_title(re.compile(f"Portal - {self.config['username'].split('.')[0].capitalize()}", re.IGNORECASE), timeout=3000)
             except AssertionError: # But sometimes, Sentral decides that EVEN A MICROSOFT ACCOUNT isn't enough veriication, and we have to log in again!
                 try:
                     expect(page).to_have_title(re.compile('Portal - Login'))
                     page.get_by_label("Email or Username*").fill(self.config['username'])
```

### Comparing `sentralify-1.2.3/src/sentralify.egg-info/PKG-INFO` & `sentralify-1.2.4/src/sentralify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.3
+Version: 1.2.4
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```


# Comparing `tmp/automation_tools-1.0.5.tar.gz` & `tmp/automation_tools-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/automation_tools-1.0.5.tar", last modified: Thu Apr  4 05:32:42 2024, max compression
+gzip compressed data, was "dist/automation_tools-1.0.6.tar", last modified: Thu Apr  4 05:40:22 2024, max compression
```

## Comparing `automation_tools-1.0.5.tar` & `automation_tools-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:32:42.035895 automation_tools-1.0.5/
--rw-r--r--   0 sporty     (501) staff       (20)        0 2024-02-29 20:50:12.000000 automation_tools-1.0.5/LICENSE
--rw-r--r--   0 sporty     (501) staff       (20)     2575 2024-04-04 05:32:42.035674 automation_tools-1.0.5/PKG-INFO
--rw-r--r--   0 sporty     (501) staff       (20)     2224 2024-04-04 05:31:16.000000 automation_tools-1.0.5/README.md
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:32:42.034642 automation_tools-1.0.5/automation_tools/
--rw-r--r--   0 sporty     (501) staff       (20)       14 2024-02-29 20:27:09.000000 automation_tools-1.0.5/automation_tools/__init__.py
--rw-r--r--   0 sporty     (501) staff       (20)     4757 2024-02-29 20:12:22.000000 automation_tools-1.0.5/automation_tools/excel_to_csv_converter.py
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:32:42.035418 automation_tools-1.0.5/automation_tools.egg-info/
--rw-r--r--   0 sporty     (501) staff       (20)     2575 2024-04-04 05:32:42.000000 automation_tools-1.0.5/automation_tools.egg-info/PKG-INFO
--rw-r--r--   0 sporty     (501) staff       (20)      297 2024-04-04 05:32:42.000000 automation_tools-1.0.5/automation_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sporty     (501) staff       (20)        1 2024-04-04 05:32:42.000000 automation_tools-1.0.5/automation_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sporty     (501) staff       (20)        9 2024-04-04 05:32:42.000000 automation_tools-1.0.5/automation_tools.egg-info/requires.txt
--rw-r--r--   0 sporty     (501) staff       (20)       17 2024-04-04 05:32:42.000000 automation_tools-1.0.5/automation_tools.egg-info/top_level.txt
--rw-r--r--   0 sporty     (501) staff       (20)       38 2024-04-04 05:32:42.035941 automation_tools-1.0.5/setup.cfg
--rw-r--r--   0 sporty     (501) staff       (20)      528 2024-04-04 05:32:37.000000 automation_tools-1.0.5/setup.py
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:40:22.310080 automation_tools-1.0.6/
+-rw-r--r--   0 sporty     (501) staff       (20)        0 2024-02-29 20:50:12.000000 automation_tools-1.0.6/LICENSE
+-rw-r--r--   0 sporty     (501) staff       (20)     2575 2024-04-04 05:40:22.309853 automation_tools-1.0.6/PKG-INFO
+-rw-r--r--   0 sporty     (501) staff       (20)     2224 2024-04-04 05:39:15.000000 automation_tools-1.0.6/README.md
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:40:22.308879 automation_tools-1.0.6/automation_tools/
+-rw-r--r--   0 sporty     (501) staff       (20)       14 2024-02-29 20:27:09.000000 automation_tools-1.0.6/automation_tools/__init__.py
+-rw-r--r--   0 sporty     (501) staff       (20)     4757 2024-02-29 20:12:22.000000 automation_tools-1.0.6/automation_tools/excel_to_csv_converter.py
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:40:22.309647 automation_tools-1.0.6/automation_tools.egg-info/
+-rw-r--r--   0 sporty     (501) staff       (20)     2575 2024-04-04 05:40:22.000000 automation_tools-1.0.6/automation_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sporty     (501) staff       (20)      297 2024-04-04 05:40:22.000000 automation_tools-1.0.6/automation_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sporty     (501) staff       (20)        1 2024-04-04 05:40:22.000000 automation_tools-1.0.6/automation_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sporty     (501) staff       (20)        9 2024-04-04 05:40:22.000000 automation_tools-1.0.6/automation_tools.egg-info/requires.txt
+-rw-r--r--   0 sporty     (501) staff       (20)       17 2024-04-04 05:40:22.000000 automation_tools-1.0.6/automation_tools.egg-info/top_level.txt
+-rw-r--r--   0 sporty     (501) staff       (20)       38 2024-04-04 05:40:22.310124 automation_tools-1.0.6/setup.cfg
+-rw-r--r--   0 sporty     (501) staff       (20)      528 2024-04-04 05:40:11.000000 automation_tools-1.0.6/setup.py
```

### Comparing `automation_tools-1.0.5/PKG-INFO` & `automation_tools-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: A suite of automation tools for various tasks.
 Home-page: https://github.com/sportyomar/automation_tools
 Author: Omar Lydale Morrison
 Author-email: omar.morrison@sportyventures.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,15 +56,15 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 The code produces the following graphical user interface for converting Excel files to csv files.
 
-![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QFMA6D6KLP7B5SVSGCZQOHNGA)
+![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QEJKVUMTGGDMVDEMMUZQOHUQQ)
 
 ### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
```

### Comparing `automation_tools-1.0.5/README.md` & `automation_tools-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 The code produces the following graphical user interface for converting Excel files to csv files.
 
-![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QFMA6D6KLP7B5SVSGCZQOHNGA)
+![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QEJKVUMTGGDMVDEMMUZQOHUQQ)
 
 ### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
```

### Comparing `automation_tools-1.0.5/automation_tools/excel_to_csv_converter.py` & `automation_tools-1.0.6/automation_tools/excel_to_csv_converter.py`

 * *Files identical despite different names*

### Comparing `automation_tools-1.0.5/automation_tools.egg-info/PKG-INFO` & `automation_tools-1.0.6/automation_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: A suite of automation tools for various tasks.
 Home-page: https://github.com/sportyomar/automation_tools
 Author: Omar Lydale Morrison
 Author-email: omar.morrison@sportyventures.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,15 +56,15 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 The code produces the following graphical user interface for converting Excel files to csv files.
 
-![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QFMA6D6KLP7B5SVSGCZQOHNGA)
+![Alt text](https://raw.githubusercontent.com/sportyomar/automation_tools/main/image.png?token=GHSAT0AAAAAACQQW5QEJKVUMTGGDMVDEMMUZQOHUQQ)
 
 ### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
```

### Comparing `automation_tools-1.0.5/setup.py` & `automation_tools-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='automation_tools',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     install_requires=[
         'openpyxl',
     ],
     author='Omar Lydale Morrison',
     author_email='omar.morrison@sportyventures.com',
     description='A suite of automation tools for various tasks.',
```

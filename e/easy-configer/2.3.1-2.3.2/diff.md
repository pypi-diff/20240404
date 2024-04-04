# Comparing `tmp/easy_configer-2.3.1.tar.gz` & `tmp/easy_configer-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_configer-2.3.1.tar", last modified: Thu Apr  4 09:32:29 2024, max compression
+gzip compressed data, was "dist/easy_configer-2.3.2.tar", last modified: Thu Apr  4 14:37:13 2024, max compression
```

## Comparing `easy_configer-2.3.1.tar` & `easy_configer-2.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:32:30.539892 easy_configer-2.3.1/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21648 2024-04-04 09:32:30.537908 easy_configer-2.3.1/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21059 2024-04-04 09:31:51.000000 easy_configer-2.3.1/README.md
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:32:30.450523 easy_configer-2.3.1/easy_configer/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    14856 2024-04-04 09:04:41.000000 easy_configer-2.3.1/easy_configer/Configer.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     5021 2024-04-04 09:04:41.000000 easy_configer-2.3.1/easy_configer/IO_Converter.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:32:30.529911 easy_configer-2.3.1/easy_configer/utils/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     2059 2024-04-04 09:04:41.000000 easy_configer-2.3.1/easy_configer/utils/Container.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4801 2024-04-04 09:04:41.000000 easy_configer-2.3.1/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 09:32:30.495526 easy_configer-2.3.1/easy_configer.egg-info/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21648 2024-04-04 09:32:30.000000 easy_configer-2.3.1/easy_configer.egg-info/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)      293 2024-04-04 09:32:30.000000 easy_configer-2.3.1/easy_configer.egg-info/SOURCES.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2024-04-04 09:32:30.000000 easy_configer-2.3.1/easy_configer.egg-info/dependency_links.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2024-04-04 09:32:30.000000 easy_configer-2.3.1/easy_configer.egg-info/top_level.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2024-04-04 09:32:30.539892 easy_configer-2.3.1/setup.cfg
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2024-04-04 09:32:28.000000 easy_configer-2.3.1/setup.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.922305 easy_configer-2.3.2/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21683 2024-04-04 14:37:14.921301 easy_configer-2.3.2/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21094 2024-04-04 14:34:44.000000 easy_configer-2.3.2/README.md
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.847288 easy_configer-2.3.2/easy_configer/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    14856 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/Configer.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     5021 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/IO_Converter.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.909292 easy_configer-2.3.2/easy_configer/utils/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     2059 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/utils/Container.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4801 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.887290 easy_configer-2.3.2/easy_configer.egg-info/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21683 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)      293 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/top_level.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2024-04-04 14:37:14.923291 easy_configer-2.3.2/setup.cfg
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2024-04-04 14:37:07.000000 easy_configer-2.3.2/setup.py
```

### Comparing `easy_configer-2.3.1/PKG-INFO` & `easy_configer-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easy_configer
-Version: 2.3.1
+Version: 2.3.2
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Keywords: configuration,commendline argument,argument
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Project description
-#### easy_configer version : 2.3.0
+#### easy_configer version : 2.3.2
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -484,16 +484,16 @@
 
     @dataclass
     class ModelConfig:
         data_source: Optional[TableConfig] = None
 
     @dataclass
     class ServerConfig:
-        db: DatabaseConfig
-        model: ModelConfig
+        db: DatabaseConfig = DatabaseConfig()
+        model: ModelConfig = ModelConfig()
 
     if __name__ == '__main__':
         from easy_configer.IO_Converter import IO_Converter
 
         # first import the IO_converter
         from easy_config.IO_Converter import IO_Converter
         cnvt = IO_Converter()
```

### Comparing `easy_configer-2.3.1/README.md` & `easy_configer-2.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Project description
-#### easy_configer version : 2.3.0
+#### easy_configer version : 2.3.2
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -468,16 +468,16 @@
 
     @dataclass
     class ModelConfig:
         data_source: Optional[TableConfig] = None
 
     @dataclass
     class ServerConfig:
-        db: DatabaseConfig
-        model: ModelConfig
+        db: DatabaseConfig = DatabaseConfig()
+        model: ModelConfig = ModelConfig()
 
     if __name__ == '__main__':
         from easy_configer.IO_Converter import IO_Converter
 
         # first import the IO_converter
         from easy_config.IO_Converter import IO_Converter
         cnvt = IO_Converter()
```

### Comparing `easy_configer-2.3.1/easy_configer/Configer.py` & `easy_configer-2.3.2/easy_configer/Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.1/easy_configer/IO_Converter.py` & `easy_configer-2.3.2/easy_configer/IO_Converter.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.1/easy_configer/utils/Container.py` & `easy_configer-2.3.2/easy_configer/utils/Container.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.1/easy_configer/utils/Type_Convertor.py` & `easy_configer-2.3.2/easy_configer/utils/Type_Convertor.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.1/easy_configer.egg-info/PKG-INFO` & `easy_configer-2.3.2/easy_configer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easy-configer
-Version: 2.3.1
+Version: 2.3.2
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Keywords: configuration,commendline argument,argument
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Project description
-#### easy_configer version : 2.3.0
+#### easy_configer version : 2.3.2
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -484,16 +484,16 @@
 
     @dataclass
     class ModelConfig:
         data_source: Optional[TableConfig] = None
 
     @dataclass
     class ServerConfig:
-        db: DatabaseConfig
-        model: ModelConfig
+        db: DatabaseConfig = DatabaseConfig()
+        model: ModelConfig = ModelConfig()
 
     if __name__ == '__main__':
         from easy_configer.IO_Converter import IO_Converter
 
         # first import the IO_converter
         from easy_config.IO_Converter import IO_Converter
         cnvt = IO_Converter()
```

### Comparing `easy_configer-2.3.1/setup.py` & `easy_configer-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='2.3.1',
+    version='2.3.2',
     description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
```


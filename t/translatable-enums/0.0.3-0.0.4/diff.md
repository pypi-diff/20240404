# Comparing `tmp/translatable_enums-0.0.3.tar.gz` & `tmp/translatable_enums-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translatable_enums-0.0.3.tar", max compression
+gzip compressed data, was "translatable_enums-0.0.4.tar", max compression
```

## Comparing `translatable_enums-0.0.3.tar` & `translatable_enums-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      539 2024-02-11 14:43:02.567345 translatable_enums-0.0.3/i18n/__init__.py
--rw-r--r--   0        0        0     2022 2024-02-11 15:20:36.424772 translatable_enums-0.0.3/i18n/__main__.py
--rw-r--r--   0        0        0      484 2024-02-11 18:24:31.975786 translatable_enums-0.0.3/i18n/enums.py
--rw-r--r--   0        0        0      218 2024-02-12 11:26:03.772662 translatable_enums-0.0.3/i18n/settings.py
--rw-r--r--   0        0        0      338 2024-02-11 12:08:21.511566 translatable_enums-0.0.3/i18n/tools.py
--rw-r--r--   0        0        0      145 2024-02-11 17:49:43.987989 translatable_enums-0.0.3/i18n/types.py
--rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.3/i18n/utils/__init__.py
--rw-r--r--   0        0        0       94 2024-02-11 10:25:57.928146 translatable_enums-0.0.3/i18n/utils/clsutils/__init__.py
--rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.3/i18n/utils/clsutils/generators.py
--rw-r--r--   0        0        0      222 2024-02-11 14:13:35.378888 translatable_enums-0.0.3/i18n/utils/gettext/__init__.py
--rw-r--r--   0        0        0      292 2024-02-11 14:13:35.390105 translatable_enums-0.0.3/i18n/utils/gettext/contexts.py
--rw-r--r--   0        0        0      412 2024-02-11 14:27:35.815709 translatable_enums-0.0.3/i18n/utils/gettext/shortcuts.py
--rw-r--r--   0        0        0       73 2024-02-11 15:08:51.918492 translatable_enums-0.0.3/i18n/utils/imputils/__init__.py
--rw-r--r--   0        0        0      798 2024-02-11 15:23:07.240044 translatable_enums-0.0.3/i18n/utils/imputils/utils.py
--rw-r--r--   0        0        0      115 2024-02-11 11:46:47.265559 translatable_enums-0.0.3/i18n/utils/potfile/__init__.py
--rw-r--r--   0        0        0      353 2024-02-11 11:33:58.286670 translatable_enums-0.0.3/i18n/utils/potfile/constants.py
--rw-r--r--   0        0        0     1571 2024-02-11 15:24:27.998602 translatable_enums-0.0.3/i18n/utils/potfile/potfile.py
--rw-r--r--   0        0        0      103 2024-02-12 11:26:03.765660 translatable_enums-0.0.3/i18n/utils/potfile/types.py
--rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.3/LICENSE
--rw-r--r--   0        0        0      781 2024-02-12 11:26:36.906661 translatable_enums-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2411 2024-02-12 11:40:38.252256 translatable_enums-0.0.3/README.md
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 translatable_enums-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      539 2024-02-11 14:43:02.567345 translatable_enums-0.0.4/i18n/__init__.py
+-rw-r--r--   0        0        0     2022 2024-02-11 15:20:36.424772 translatable_enums-0.0.4/i18n/__main__.py
+-rw-r--r--   0        0        0      484 2024-02-11 18:24:31.975786 translatable_enums-0.0.4/i18n/enums.py
+-rw-r--r--   0        0        0      218 2024-02-12 11:26:03.772662 translatable_enums-0.0.4/i18n/settings.py
+-rw-r--r--   0        0        0      338 2024-02-11 12:08:21.511566 translatable_enums-0.0.4/i18n/tools.py
+-rw-r--r--   0        0        0      169 2024-02-12 13:48:08.322619 translatable_enums-0.0.4/i18n/types.py
+-rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.4/i18n/utils/__init__.py
+-rw-r--r--   0        0        0       94 2024-02-11 10:25:57.928146 translatable_enums-0.0.4/i18n/utils/clsutils/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.4/i18n/utils/clsutils/generators.py
+-rw-r--r--   0        0        0      222 2024-02-11 14:13:35.378888 translatable_enums-0.0.4/i18n/utils/gettext/__init__.py
+-rw-r--r--   0        0        0      292 2024-02-11 14:13:35.390105 translatable_enums-0.0.4/i18n/utils/gettext/contexts.py
+-rw-r--r--   0        0        0      421 2024-04-04 18:32:32.879535 translatable_enums-0.0.4/i18n/utils/gettext/shortcuts.py
+-rw-r--r--   0        0        0       73 2024-02-11 15:08:51.918492 translatable_enums-0.0.4/i18n/utils/imputils/__init__.py
+-rw-r--r--   0        0        0      842 2024-03-28 11:02:20.867491 translatable_enums-0.0.4/i18n/utils/imputils/utils.py
+-rw-r--r--   0        0        0      115 2024-02-11 11:46:47.265559 translatable_enums-0.0.4/i18n/utils/potfile/__init__.py
+-rw-r--r--   0        0        0      353 2024-02-11 11:33:58.286670 translatable_enums-0.0.4/i18n/utils/potfile/constants.py
+-rw-r--r--   0        0        0     2030 2024-02-12 13:39:33.781025 translatable_enums-0.0.4/i18n/utils/potfile/potfile.py
+-rw-r--r--   0        0        0      103 2024-02-12 11:26:03.765660 translatable_enums-0.0.4/i18n/utils/potfile/types.py
+-rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.4/LICENSE
+-rw-r--r--   0        0        0      781 2024-04-04 18:36:39.836085 translatable_enums-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2591 2024-02-12 14:07:25.708666 translatable_enums-0.0.4/README.md
+-rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 translatable_enums-0.0.4/PKG-INFO
```

### Comparing `translatable_enums-0.0.3/i18n/__init__.py` & `translatable_enums-0.0.4/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.3/i18n/__main__.py` & `translatable_enums-0.0.4/i18n/__main__.py`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.3/i18n/utils/imputils/utils.py` & `translatable_enums-0.0.4/i18n/utils/imputils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if os.path.isdir(path):
         path = os.path.join(path, '__main__.py')
 
     directory = os.path.dirname(path)
     sys.path.append(directory)
     try:
         if not os.path.exists(path):
-            raise
+            raise ImportError(f'Module not found at: {path}')
         *_, filename = os.path.split(path)
         spec = importlib.util.spec_from_file_location(filename.replace('.py', ''), path)
         imported_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(imported_module)
         return imported_module
     except Exception:
         raise ImportError(f'Failed to import module: {path}')
```

### Comparing `translatable_enums-0.0.3/LICENSE` & `translatable_enums-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.3/pyproject.toml` & `translatable_enums-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "translatable-enums"
-version = "0.0.3"
+version = "0.0.4"
 description = "Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "i18n" },
 ]
```

### Comparing `translatable_enums-0.0.3/README.md` & `translatable_enums-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 <a href="https://github.com/CrazyProger1/Translatable-Enums/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Translatable-Enums"></a>
 <a href="https://pypi.org/project/translatable-enums/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/translatable-enums"></a>
 <img src="https://img.shields.io/badge/coverage-99%25-brightgreen" alt="Coverage"/>
 </p>
 
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient way to store translation keys.
 
+## Key-Features
+
+- No dependencies except the Python's standard library. Based on built-in enums & gettext
+- Powerful utility for extracting translation-keys
+- Easy-to-Use
+
 ## Installation
 
 You can use PIP:
 
 ```shell
 pip install translatable-enums
 ```
@@ -89,8 +95,9 @@
 
 ## Status
 
 ``0.0.3`` - RELEASED
 
 ## Licence
 
-Translatable-Enums is released under the MIT License. See the bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
+Translatable-Enums is released under the MIT License. See the
+bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
 # Translatable-Enums
                                   [Lib logo]
      _[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_][Coverage]
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient
-way to store translation keys. ## Installation You can use PIP: ```shell pip
-install translatable-enums ``` Or Poetry: ```shell poetry add translatable-
-enums ``` ## Getting-Started ```python from i18n import ( TranslatableEnum,
-set_domain, set_language ) class Messages(TranslatableEnum): HELLO = 'Hello,'
-WORLD = 'World!' set_domain('app', './resources/languages') set_language
-('en_US') print(Messages.HELLO, Messages.WORLD) # Hello, World! set_language
-('uk_UA') print(Messages.HELLO, Messages.WORLD) # ÐÑÐ¸Ð²ÑÑ, Ð¡Ð²ÑÑ!
-set_language('fr_FR') print(Messages.HELLO, Messages.WORLD) # Bonjour le monde!
-print(Messages.HELLO.language('uk'), Messages.WORLD.language('en')) #
-ÐÑÐ¸Ð²ÑÑ, World! ``` ### Extraction-Tools To extract the translation-keys
-from application: ```shell python -m i18n main.py application.pot ``` You will
+way to store translation keys. ## Key-Features - No dependencies except the
+Python's standard library. Based on built-in enums & gettext - Powerful utility
+for extracting translation-keys - Easy-to-Use ## Installation You can use PIP:
+```shell pip install translatable-enums ``` Or Poetry: ```shell poetry add
+translatable-enums ``` ## Getting-Started ```python from i18n import
+( TranslatableEnum, set_domain, set_language ) class Messages
+(TranslatableEnum): HELLO = 'Hello,' WORLD = 'World!' set_domain('app', './
+resources/languages') set_language('en_US') print(Messages.HELLO,
+Messages.WORLD) # Hello, World! set_language('uk_UA') print(Messages.HELLO,
+Messages.WORLD) # ÐÑÐ¸Ð²ÑÑ, Ð¡Ð²ÑÑ! set_language('fr_FR') print
+(Messages.HELLO, Messages.WORLD) # Bonjour le monde! print
+(Messages.HELLO.language('uk'), Messages.WORLD.language('en')) # ÐÑÐ¸Ð²ÑÑ,
+World! ``` ### Extraction-Tools To extract the translation-keys from
+application: ```shell python -m i18n main.py application.pot ``` You will
 obtain a [.pot](https://pofile.net/) file like this: ```potfile msgid "" msgstr
 "" "Project-Id-Version: \n" "POT-Creation-Date: \n" "Last-Translator: \n"
 "Language-Team: \n" "Language: \n" "MIME-Version: \n" "Content-Type: text/
 plain; charset=utf-8\n" "Content-Transfer-Encoding: 8bit\n" msgid "Hello,"
 msgstr "" msgid "World!" msgstr "" ``` ## Status ``0.0.3`` - RELEASED ##
 Licence Translatable-Enums is released under the MIT License. See the bundled
 [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/
```

### Comparing `translatable_enums-0.0.3/PKG-INFO` & `translatable_enums-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translatable-enums
-Version: 0.0.3
+Version: 0.0.4
 Summary: Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys.
 Home-page: https://github.com/CrazyProger1/Translatable-Enums
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,14 +27,20 @@
 <a href="https://github.com/CrazyProger1/Translatable-Enums/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Translatable-Enums"></a>
 <a href="https://pypi.org/project/translatable-enums/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/translatable-enums"></a>
 <img src="https://img.shields.io/badge/coverage-99%25-brightgreen" alt="Coverage"/>
 </p>
 
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient way to store translation keys.
 
+## Key-Features
+
+- No dependencies except the Python's standard library. Based on built-in enums & gettext
+- Powerful utility for extracting translation-keys
+- Easy-to-Use
+
 ## Installation
 
 You can use PIP:
 
 ```shell
 pip install translatable-enums
 ```
@@ -107,8 +113,9 @@
 
 ## Status
 
 ``0.0.3`` - RELEASED
 
 ## Licence
 
-Translatable-Enums is released under the MIT License. See the bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
+Translatable-Enums is released under the MIT License. See the
+bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```


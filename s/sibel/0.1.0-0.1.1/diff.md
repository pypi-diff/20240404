# Comparing `tmp/sibel-0.1.0.tar.gz` & `tmp/sibel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibel-0.1.0.tar", last modified: Mon Jan 29 12:52:42 2024, max compression
+gzip compressed data, was "sibel-0.1.1.tar", last modified: Thu Apr  4 15:41:05 2024, max compression
```

## Comparing `sibel-0.1.0.tar` & `sibel-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-01-29 12:52:42.503072 sibel-0.1.0/
--rw-r--r--   0 ellis     (1000) ellis     (1000)     7651 2024-01-20 12:48:45.000000 sibel-0.1.0/LICENSE.txt
--rw-r--r--   0 ellis     (1000) ellis     (1000)        9 2023-11-08 00:33:13.000000 sibel-0.1.0/MANIFEST.in
--rw-r--r--   0 ellis     (1000) ellis     (1000)     2353 2024-01-29 12:52:42.503072 sibel-0.1.0/PKG-INFO
--rw-r--r--   0 ellis     (1000) ellis     (1000)     1884 2024-01-29 12:52:04.000000 sibel-0.1.0/README.md
--rw-r--r--   0 ellis     (1000) ellis     (1000)      541 2024-01-27 16:16:51.000000 sibel-0.1.0/pyproject.toml
--rw-r--r--   0 ellis     (1000) ellis     (1000)       38 2024-01-29 12:52:42.503072 sibel-0.1.0/setup.cfg
--rw-r--r--   0 ellis     (1000) ellis     (1000)     1148 2024-01-29 12:40:29.000000 sibel-0.1.0/setup.py
-drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-01-29 12:52:42.503072 sibel-0.1.0/sibel/
--rw-r--r--   0 ellis     (1000) ellis     (1000)      367 2024-01-29 12:49:32.000000 sibel-0.1.0/sibel/__init__.pyi
--rw-r--r--   0 ellis     (1000) ellis     (1000)        0 2024-01-28 12:53:34.000000 sibel-0.1.0/sibel/py.typed
--rw-r--r--   0 ellis     (1000) ellis     (1000)      421 2024-01-29 12:51:40.000000 sibel-0.1.0/sibel/sibel.pyi
-drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-01-29 12:52:42.503072 sibel-0.1.0/sibel.egg-info/
--rw-r--r--   0 ellis     (1000) ellis     (1000)     2353 2024-01-29 12:52:42.000000 sibel-0.1.0/sibel.egg-info/PKG-INFO
--rw-r--r--   0 ellis     (1000) ellis     (1000)      297 2024-01-29 12:52:42.000000 sibel-0.1.0/sibel.egg-info/SOURCES.txt
--rw-r--r--   0 ellis     (1000) ellis     (1000)        1 2024-01-29 12:52:42.000000 sibel-0.1.0/sibel.egg-info/dependency_links.txt
--rw-r--r--   0 ellis     (1000) ellis     (1000)        6 2024-01-29 12:52:42.000000 sibel-0.1.0/sibel.egg-info/top_level.txt
-drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-01-29 12:52:42.503072 sibel-0.1.0/src/
--rw-r--r--   0 ellis     (1000) ellis     (1000)     1080 2024-01-28 03:17:54.000000 sibel-0.1.0/src/sibel.h
--rw-r--r--   0 ellis     (1000) ellis     (1000)     8090 2024-01-28 11:45:29.000000 sibel-0.1.0/src/sibelmodule.cc
--rw-r--r--   0 ellis     (1000) ellis     (1000)     1877 2024-01-28 10:04:51.000000 sibel-0.1.0/src/simplification.cc
--rw-r--r--   0 ellis     (1000) ellis     (1000)    12887 2024-01-29 07:22:08.000000 sibel-0.1.0/src/substitutions.cc
+drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-04-04 15:41:05.063329 sibel-0.1.1/
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     7651 2024-01-20 12:48:45.000000 sibel-0.1.1/LICENSE.txt
+-rw-r--r--   0 ellis     (1000) ellis     (1000)        9 2023-11-08 00:33:13.000000 sibel-0.1.1/MANIFEST.in
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     2353 2024-04-04 15:41:05.059329 sibel-0.1.1/PKG-INFO
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     1884 2024-01-29 12:52:04.000000 sibel-0.1.1/README.md
+-rw-r--r--   0 ellis     (1000) ellis     (1000)      541 2024-04-04 15:10:20.000000 sibel-0.1.1/pyproject.toml
+-rw-r--r--   0 ellis     (1000) ellis     (1000)       38 2024-04-04 15:41:05.063329 sibel-0.1.1/setup.cfg
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     1148 2024-04-04 15:15:59.000000 sibel-0.1.1/setup.py
+drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-04-04 15:41:05.059329 sibel-0.1.1/sibel/
+-rw-r--r--   0 ellis     (1000) ellis     (1000)      367 2024-01-29 12:49:32.000000 sibel-0.1.1/sibel/__init__.pyi
+-rw-r--r--   0 ellis     (1000) ellis     (1000)        0 2024-01-28 12:53:34.000000 sibel-0.1.1/sibel/py.typed
+-rw-r--r--   0 ellis     (1000) ellis     (1000)      421 2024-01-29 12:51:40.000000 sibel-0.1.1/sibel/sibel.pyi
+drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-04-04 15:41:05.059329 sibel-0.1.1/sibel.egg-info/
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     2353 2024-04-04 15:41:05.000000 sibel-0.1.1/sibel.egg-info/PKG-INFO
+-rw-r--r--   0 ellis     (1000) ellis     (1000)      306 2024-04-04 15:41:05.000000 sibel-0.1.1/sibel.egg-info/SOURCES.txt
+-rw-r--r--   0 ellis     (1000) ellis     (1000)        1 2024-04-04 15:41:05.000000 sibel-0.1.1/sibel.egg-info/dependency_links.txt
+-rw-r--r--   0 ellis     (1000) ellis     (1000)        6 2024-04-04 15:41:05.000000 sibel-0.1.1/sibel.egg-info/top_level.txt
+drwxr-xr-x   0 ellis     (1000) ellis     (1000)        0 2024-04-04 15:41:05.059329 sibel-0.1.1/src/
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     1142 2024-04-04 15:05:57.000000 sibel-0.1.1/src/sibel.h
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     8152 2024-04-04 15:08:14.000000 sibel-0.1.1/src/sibelmodule.cc
+-rw-r--r--   0 ellis     (1000) ellis     (1000)     1877 2024-02-07 00:40:33.000000 sibel-0.1.1/src/simplification.cc
+-rw-r--r--   0 ellis     (1000) ellis     (1000)    13875 2024-04-04 15:34:02.000000 sibel-0.1.1/src/substitutions.cc
+-rwxr-xr-x   0 ellis     (1000) ellis     (1000)    33848 2024-02-07 00:39:39.000000 sibel-0.1.1/src/test
```

### Comparing `sibel-0.1.0/LICENSE.txt` & `sibel-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sibel-0.1.0/PKG-INFO` & `sibel-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python spellchecker with Hunspell as back-end
 Author-email: Yi Xing <blandilyte@gmail.com>
 Project-URL: Homepage, https://github.com/Crissium/sibel
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `sibel-0.1.0/README.md` & `sibel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sibel-0.1.0/pyproject.toml` & `sibel-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sibel"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Yi Xing", email="blandilyte@gmail.com" },
 ]
 description = "Python spellchecker with Hunspell as back-end"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sibel-0.1.0/setup.py` & `sibel-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sibel-0.1.0/sibel.egg-info/PKG-INFO` & `sibel-0.1.1/sibel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python spellchecker with Hunspell as back-end
 Author-email: Yi Xing <blandilyte@gmail.com>
 Project-URL: Homepage, https://github.com/Crissium/sibel
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `sibel-0.1.0/src/sibelmodule.cc` & `sibel-0.1.1/src/sibelmodule.cc`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
 	Py_BEGIN_ALLOW_THREADS
 	std::vector<std::thread> threads;
 	std::mutex mtx;
 
 	if (substitution_table::is_substitutable(word))
 	{
-		if (self->sub_table)
+		if (self->sub_table && word.size() <= substitution_table::SUBSTITUTION_MAX_LENGTH)
 		{
 			for (const std::string & possible_form : self->sub_table->substitute(word))
 			{
 				threads.push_back(std::thread([&](const std::string & form)
 				{
 					if (self->hunspell->spell(form))
 					{
```

### Comparing `sibel-0.1.0/src/simplification.cc` & `sibel-0.1.1/src/simplification.cc`

 * *Files identical despite different names*

### Comparing `sibel-0.1.0/src/substitutions.cc` & `sibel-0.1.1/src/substitutions.cc`

 * *Files 26% similar despite different names*

```diff
@@ -420,14 +420,32 @@
 	return std::all_of(s.cbegin(), s.cend(), [](unsigned char c)
 					   { return std::isprint(c); }) &&
 	// Strings with spaces can't be checked anyway
 		   std::none_of(s.cbegin(), s.cend(), [](unsigned char c)
 						{ return std::isspace(c); });
 }
 
+/**
+ * The value is determined thus:
+ * Let's say on average a letter has two possible substitutions.
+ * Then the number of possible substitutions for a string of length n is 2^n.
+ * If n is too large, then the time spent in checking all the substitutions might exceed
+ * the time obtaining the suggestions from Hunspell.
+ * Also if there are too many threads, then we might get an exception
+ * (std::system_error Resource temporarily unavailable).
+ * 
+ * Then I run some simple empirical tests and decided that 8 would guarantee performance
+ * in most cases while also not causing exceptions. (On my system an exception is thrown
+ * when the number of threads exceeds ~1000. If the user loads three dictionaries with
+ * substitution tables, then the number of threads would be 3 * 2^8 = 768. On the other
+ * hand, if only one is loaded, we are wasting resources... but it's better to be safe
+ * than sorry, right?)
+ */
+const std::size_t substitution_table::SUBSTITUTION_MAX_LENGTH = 8;
+
 void substitution_table::generate_substitutions(const std::unordered_map<std::string, std::vector<std::string>> &map, const std::string &input, std::vector<std::string> &result, std::string::size_type index, std::string current, std::string::size_type len_of_key)
 {
 	if (index == input.size())
 	{
 		result.push_back(current);
 	}
 	else
```


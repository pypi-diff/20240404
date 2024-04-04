# Comparing `tmp/costsensitive-0.1.2.8.tar.gz` & `tmp/costsensitive-0.1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/costsensitive-0.1.2.8.tar", last modified: Tue Apr 23 18:48:43 2019, max compression
+gzip compressed data, was "dist/costsensitive-0.1.2.9.tar", last modified: Sun Jul 28 09:09:00 2019, max compression
```

## Comparing `costsensitive-0.1.2.8.tar` & `costsensitive-0.1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/
--rw-r--r--   0 david     (1000) david     (1000)       78 2019-04-23 18:44:24.000000 costsensitive-0.1.2.8/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      434 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     7754 2019-03-07 06:39:34.000000 costsensitive-0.1.2.8/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive/
--rw-r--r--   0 david     (1000) david     (1000)    38430 2019-03-07 11:53:50.000000 costsensitive-0.1.2.8/costsensitive/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      363 2019-02-10 14:06:36.000000 costsensitive-0.1.2.8/costsensitive/vwrapper.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      434 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      304 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       32 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       14 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/costsensitive.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       94 2019-04-23 18:47:34.000000 costsensitive-0.1.2.8/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     1446 2019-04-23 18:47:47.000000 costsensitive-0.1.2.8/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-04-23 18:48:43.000000 costsensitive-0.1.2.8/src/
--rw-r--r--   0 david     (1000) david     (1000)     4380 2019-03-07 17:39:30.000000 costsensitive-0.1.2.8/src/calcv.c
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/
+-rw-r--r--   0 david     (1000) david     (1000)       78 2019-04-23 18:44:24.000000 costsensitive-0.1.2.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      434 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     7754 2019-03-07 06:39:34.000000 costsensitive-0.1.2.9/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive/
+-rw-r--r--   0 david     (1000) david     (1000)    38430 2019-03-07 11:53:50.000000 costsensitive-0.1.2.9/costsensitive/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      363 2019-02-10 14:06:36.000000 costsensitive-0.1.2.9/costsensitive/vwrapper.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      434 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      304 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       32 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       14 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/costsensitive.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       94 2019-04-23 18:47:34.000000 costsensitive-0.1.2.9/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       79 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     2543 2019-07-28 09:07:20.000000 costsensitive-0.1.2.9/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2019-07-28 09:09:00.000000 costsensitive-0.1.2.9/src/
+-rw-r--r--   0 david     (1000) david     (1000)     4380 2019-03-07 17:39:30.000000 costsensitive-0.1.2.9/src/calcv.c
```

### Comparing `costsensitive-0.1.2.8/README.md` & `costsensitive-0.1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `costsensitive-0.1.2.8/costsensitive/__init__.py` & `costsensitive-0.1.2.9/costsensitive/__init__.py`

 * *Files identical despite different names*

### Comparing `costsensitive-0.1.2.8/setup.py` & `costsensitive-0.1.2.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 try:
 	from setuptools import setup
+	from setuptools import Extension
 except:
 	from distutils.core import setup
+	from distutils.extension import Extension
 import numpy as np
-from distutils.extension import Extension
-import os
-
+import os, warnings
+from sys import platform
 
 
 from Cython.Distutils import build_ext
 ## https://stackoverflow.com/questions/724664/python-distutils-how-to-get-a-compiler-that-is-going-to-be-used
 class build_ext_subclass( build_ext ):
 	def build_extensions(self):
 		c = self.compiler.compiler_type
 		if c == 'msvc': # visual studio
 			for e in self.extensions:
 				e.extra_compile_args = ['/O2']
 		else: # gcc and clang
 			for e in self.extensions:
-				e.extra_compile_args = ['-fopenmp', '-O2', '-march=native', '-std=c99']
-				e.extra_link_args = ['-fopenmp']
+				# e.extra_compile_args = ['-fopenmp', '-O2', '-march=native', '-std=c99']
+				# e.extra_link_args = ['-fopenmp']
+				e.extra_compile_args = ['-O2', '-march=native', '-std=c99']
+
+			## Note: apple will by default alias 'gcc' to 'clang', and will ship its own "special"
+			## 'clang' which has no OMP support and nowadays will purposefully fail to compile when passed
+			## '-fopenmp' flags. If you are using mac, and have an OMP-capable compiler,
+			## comment out the code below, and un-comment the lines above.
+			if platform[:3] == "dar":
+				apple_msg  = "\n\n\nMacOS detected. Package will be built without multi-threading capabilities, "
+				apple_msg += "due to Apple's lack of OpenMP support in default Xcode installs. In order to enable it, "
+				apple_msg += "install the package directly from GitHub: https://www.github.com/david-cortes/costsensitive\n"
+				apple_msg += "And modify the setup.py file where this message is shown. "
+				apple_msg += "You'll also need an OpenMP-capable compiler.\n\n\n"
+				warnings.warn(apple_msg)
+			else:
+				for e in self.extensions:
+					e.extra_compile_args.append('-fopenmp')
+					e.extra_link_args.append('-fopenmp')
 		build_ext.build_extensions(self)
 
 setup(
 	name = 'costsensitive',
 	packages = ['costsensitive'],
 	install_requires=[
 	 'numpy',
 	 'scipy',
 	 'joblib>=0.13',
 	 'cython'
 	],
 	python_requires = ">=3",
-	version = '0.1.2.8',
+	version = '0.1.2.9',
 	description = 'Reductions for Cost-Sensitive Multi-Class Classification',
 	author = 'David Cortes',
 	author_email = 'david.cortes.rivera@gmail.com',
 	url = 'https://github.com/david-cortes/costsensitive',
 	keywords = ['cost sensitive multi class', 'cost-sensitive multi-class classification', 'weighted all pairs', 'filter tree'],
 	classifiers = [],
 
 	cmdclass = {'build_ext': build_ext_subclass},
-	ext_modules = [Extension("costsensitive._vwrapper", sources=["costsensitive/vwrapper.pyx"], include_dirs=[np.get_include()], extra_link_args=["-fopenmp"])]
+	ext_modules = [Extension("costsensitive._vwrapper", sources=["costsensitive/vwrapper.pyx"], include_dirs=[np.get_include()])]
 )
```

### Comparing `costsensitive-0.1.2.8/src/calcv.c` & `costsensitive-0.1.2.9/src/calcv.c`

 * *Files identical despite different names*


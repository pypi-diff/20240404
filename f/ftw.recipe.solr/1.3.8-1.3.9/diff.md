# Comparing `tmp/ftw.recipe.solr-1.3.8.tar.gz` & `tmp/ftw.recipe.solr-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ftw.recipe.solr-1.3.8.tar", last modified: Thu Oct 12 09:20:34 2023, max compression
+gzip compressed data, was "ftw.recipe.solr-1.3.9.tar", last modified: Thu Apr  4 11:33:49 2024, max compression
```

## Comparing `ftw.recipe.solr-1.3.8.tar` & `ftw.recipe.solr-1.3.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     6075 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/PKG-INFO
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/
--rw-r--r--   0 lukasgraf   (501) staff       (20)       56 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/__init__.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/testdata/
--rw-r--r--   0 lukasgraf   (501) staff       (20)      218 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/testdata/solr-7.2.1.tgz
--rw-r--r--   0 lukasgraf   (501) staff       (20)     7494 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      220 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/utils.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1040 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/solr.xml.tmpl
--rw-r--r--   0 lukasgraf   (501) staff       (20)      975 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/zoo.cfg.tmpl
--rw-r--r--   0 lukasgraf   (501) staff       (20)       15 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/core.properties.tmpl
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2345 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/startup.tmpl
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2878 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/log4j2.xml.tmpl
--rw-r--r--   0 lukasgraf   (501) staff       (20)      264 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/defaults.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)    13523 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/README.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2170 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/tests.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/
--rw-r--r--   0 lukasgraf   (501) staff       (20)    15800 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/managed-schema
--rw-r--r--   0 lukasgraf   (501) staff       (20)    78514 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/mapping-FoldToASCII.txt
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/lang/
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/lang/de.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1122 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/synonyms.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)    50831 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/solrconfig.xml
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/stopwords.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)       56 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw/__init__.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     6075 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/PKG-INFO
--rw-r--r--   0 lukasgraf   (501) staff       (20)        1 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/not-zip-safe
--rw-r--r--   0 lukasgraf   (501) staff       (20)       15 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/namespace_packages.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1003 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/SOURCES.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)       48 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/entry_points.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)       73 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/requires.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)        4 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/top_level.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)        1 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/dependency_links.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)       59 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/MANIFEST.in
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1270 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/setup.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)       38 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/setup.cfg
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1890 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/HISTORY.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2143 2023-10-12 09:20:34.000000 ftw.recipe.solr-1.3.8/README.rst
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.955397 ftw.recipe.solr-1.3.9/
+-rw-r--r--   0 tbu       (1001) users      (100)     1991 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/HISTORY.txt
+-rw-r--r--   0 tbu       (1001) users      (100)       59 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/MANIFEST.in
+-rw-r--r--   0 tbu       (1001) users      (100)     4839 2024-04-04 11:33:49.954397 ftw.recipe.solr-1.3.9/PKG-INFO
+-rw-r--r--   0 tbu       (1001) users      (100)     2143 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/README.rst
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.952397 ftw.recipe.solr-1.3.9/ftw/
+-rw-r--r--   0 tbu       (1001) users      (100)       56 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.952397 ftw.recipe.solr-1.3.9/ftw/recipe/
+-rw-r--r--   0 tbu       (1001) users      (100)       56 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.953397 ftw.recipe.solr-1.3.9/ftw/recipe/solr/
+-rw-r--r--   0 tbu       (1001) users      (100)    13563 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/README.txt
+-rw-r--r--   0 tbu       (1001) users      (100)     7571 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.953397 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.953397 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/lang/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/lang/de.txt
+-rw-r--r--   0 tbu       (1001) users      (100)    15800 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/managed-schema
+-rw-r--r--   0 tbu       (1001) users      (100)    78514 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/mapping-FoldToASCII.txt
+-rw-r--r--   0 tbu       (1001) users      (100)    50831 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/solrconfig.xml
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/stopwords.txt
+-rw-r--r--   0 tbu       (1001) users      (100)     1122 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/synonyms.txt
+-rw-r--r--   0 tbu       (1001) users      (100)      303 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/defaults.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.954397 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/
+-rw-r--r--   0 tbu       (1001) users      (100)       15 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/core.properties.tmpl
+-rw-r--r--   0 tbu       (1001) users      (100)     2878 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/log4j2.xml.tmpl
+-rw-r--r--   0 tbu       (1001) users      (100)     1040 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/solr.xml.tmpl
+-rw-r--r--   0 tbu       (1001) users      (100)     2406 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/startup.tmpl
+-rw-r--r--   0 tbu       (1001) users      (100)      975 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/zoo.cfg.tmpl
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.954397 ftw.recipe.solr-1.3.9/ftw/recipe/solr/testdata/
+-rw-r--r--   0 tbu       (1001) users      (100)      218 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/testdata/solr-7.2.1.tgz
+-rw-r--r--   0 tbu       (1001) users      (100)     2170 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/tests.py
+-rw-r--r--   0 tbu       (1001) users      (100)      220 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw/recipe/solr/utils.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:33:49.954397 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/
+-rw-r--r--   0 tbu       (1001) users      (100)     4839 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/PKG-INFO
+-rw-r--r--   0 tbu       (1001) users      (100)     1003 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/SOURCES.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        1 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/dependency_links.txt
+-rw-r--r--   0 tbu       (1001) users      (100)       47 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/entry_points.txt
+-rw-r--r--   0 tbu       (1001) users      (100)       15 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/namespace_packages.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        1 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/not-zip-safe
+-rw-r--r--   0 tbu       (1001) users      (100)       73 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/requires.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        4 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/top_level.txt
+-rw-r--r--   0 tbu       (1001) users      (100)       38 2024-04-04 11:33:49.955397 ftw.recipe.solr-1.3.9/setup.cfg
+-rw-r--r--   0 tbu       (1001) users      (100)     1270 2024-04-04 11:33:49.000000 ftw.recipe.solr-1.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/__init__.py` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
             pid_file=self.options['pid-file'],
             jvm_opts=self.options['jvm-opts'],
             extra_opts=self.options['extra-opts'],
             solr_port=self.options['port'],
             solr_host=self.options['host'],
             solr_home=home_dir,
             solr_install_dir=destination,
+            enable_remote_streaming=self.options['enable-remote-streaming'],
             log_dir=log_dir,
             log4j2_xml=log4j2_xml,
         ))
 
         # Create configoverlay.json
         configoverlay = self.options.get('configoverlay')
         if configoverlay:
```

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/solr.xml.tmpl` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/solr.xml.tmpl`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/zoo.cfg.tmpl` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/zoo.cfg.tmpl`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/startup.tmpl` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/startup.tmpl`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 "${JVM_OPTS[@]}" \
 -Djetty.host={{ solr_host }}
 -Djetty.port=$SOLR_PORT \
 -Djetty.home=$SOLR_SERVER_DIR \
 -Dsolr.solr.home=$SOLR_HOME \
 -Dsolr.install.dir=$SOLR_INSTALL_DIR \
 -Dsolr.log.dir={{ log_dir }} \
+-Dsolr.enableRemoteStreaming={{ enable_remote_streaming }} \
 -Dlog4j2.formatMsgNoLookups=true \
 -Dlog4j2.configurationFile=file:{{ log4j2_xml }} \
 "${EXTRA_OPTS[@]}")
 
 start() {
     cd "$SOLR_SERVER_DIR"
     nohup "$JAVACMD" "${SOLR_START_OPT[@]}" -Dsolr.log.muteconsole -jar start.jar --module=http >/dev/null 2>&1 &
```

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/templates/log4j2.xml.tmpl` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/templates/log4j2.xml.tmpl`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/README.txt` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/README.txt`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     "${JVM_OPTS[@]}" \
     -Djetty.host=localhost
     -Djetty.port=$SOLR_PORT \
     -Djetty.home=$SOLR_SERVER_DIR \
     -Dsolr.solr.home=$SOLR_HOME \
     -Dsolr.install.dir=$SOLR_INSTALL_DIR \
     -Dsolr.log.dir=/sample-buildout/var/log \
+    -Dsolr.enableRemoteStreaming=true \
     -Dlog4j2.formatMsgNoLookups=true \
     -Dlog4j2.configurationFile=/sample-buildout/parts/solr/log4j2.xml \
     "${EXTRA_OPTS[@]}")
     <BLANKLINE>
     start() {
         cd "$SOLR_SERVER_DIR"
         nohup "$JAVACMD" "${SOLR_START_OPT[@]}" -Dsolr.log.muteconsole -jar start.jar --module=http >/dev/null 2>&1 &
```

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/tests.py` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/tests.py`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/managed-schema` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/managed-schema`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/mapping-FoldToASCII.txt` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/mapping-FoldToASCII.txt`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/synonyms.txt` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/synonyms.txt`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw/recipe/solr/conf/solrconfig.xml` & `ftw.recipe.solr-1.3.9/ftw/recipe/solr/conf/solrconfig.xml`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/ftw.recipe.solr.egg-info/SOURCES.txt` & `ftw.recipe.solr-1.3.9/ftw.recipe.solr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftw.recipe.solr-1.3.8/setup.py` & `ftw.recipe.solr-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-version = '1.3.8'
+version = '1.3.9'
 tests_require = ['zope.testing', 'manuel']
 
 setup(
     name='ftw.recipe.solr',
     version=version,
     description="A zc.buildout recipe to install a Solr server",
     long_description=open("README.rst").read()
```

### Comparing `ftw.recipe.solr-1.3.8/HISTORY.txt` & `ftw.recipe.solr-1.3.9/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.3.9 (2024-04-02)
+------------------
+
+- Use system property to enable remote streaming.
+  [buchi]
+
+
 1.3.8 (2023-10-12)
 ------------------
 
 - Add support for `extra-opts` (additional options for Solr cmdline).
   [lgraf]
```

### Comparing `ftw.recipe.solr-1.3.8/README.rst` & `ftw.recipe.solr-1.3.9/README.rst`

 * *Files identical despite different names*


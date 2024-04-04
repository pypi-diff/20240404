# Comparing `tmp/html_text-0.5.1.tar.gz` & `tmp/html_text-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/html_text-0.5.1.tar", last modified: Tue May 28 18:47:44 2019, max compression
+gzip compressed data, was "dist/html_text-0.5.2.tar", last modified: Wed Jul 22 19:12:24 2020, max compression
```

## Comparing `html_text-0.5.1.tar` & `html_text-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2019-05-28 18:47:44.000000 html_text-0.5.1/
--rw-r--r--   0 kmike      (501) staff       (20)     9099 2019-05-28 18:47:44.000000 html_text-0.5.1/PKG-INFO
--rw-r--r--   0 kmike      (501) staff       (20)     1079 2018-11-01 22:27:25.000000 html_text-0.5.1/LICENSE
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/
--rw-r--r--   0 kmike      (501) staff       (20)     9099 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/PKG-INFO
--rw-r--r--   0 kmike      (501) staff       (20)        1 2018-11-12 15:20:23.000000 html_text-0.5.1/html_text.egg-info/not-zip-safe
--rw-r--r--   0 kmike      (501) staff       (20)      997 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/SOURCES.txt
--rw-r--r--   0 kmike      (501) staff       (20)        5 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/requires.txt
--rw-r--r--   0 kmike      (501) staff       (20)       10 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/top_level.txt
--rw-r--r--   0 kmike      (501) staff       (20)        1 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text.egg-info/dependency_links.txt
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2019-05-28 18:47:44.000000 html_text-0.5.1/tests/
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2019-05-28 18:47:44.000000 html_text-0.5.1/tests/test_webpages/
--rw-r--r--   0 kmike      (501) staff       (20)     1228 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
--rw-r--r--   0 kmike      (501) staff       (20)     9279 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
--rw-r--r--   0 kmike      (501) staff       (20)     2852 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
--rw-r--r--   0 kmike      (501) staff       (20)     1539 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
--rw-r--r--   0 kmike      (501) staff       (20)    10856 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
--rw-r--r--   0 kmike      (501) staff       (20)    11694 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
--rw-r--r--   0 kmike      (501) staff       (20)     4635 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
--rw-r--r--   0 kmike      (501) staff       (20)    38239 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
--rw-r--r--   0 kmike      (501) staff       (20)    10225 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
--rw-r--r--   0 kmike      (501) staff       (20)    67149 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/test_webpages/Scrapinghub Enterprise Solutions.html
--rw-r--r--   0 kmike      (501) staff       (20)     7685 2019-05-25 21:55:19.000000 html_text-0.5.1/tests/test_html_text.py
--rw-r--r--   0 kmike      (501) staff       (20)       24 2018-11-01 22:27:25.000000 html_text-0.5.1/tests/__init__.py
--rw-r--r--   0 kmike      (501) staff       (20)      243 2018-11-01 22:27:25.000000 html_text-0.5.1/MANIFEST.in
--rwxr-xr-x   0 kmike      (501) staff       (20)     1182 2019-05-27 18:16:06.000000 html_text-0.5.1/setup.py
--rw-r--r--   0 kmike      (501) staff       (20)      381 2019-05-28 18:47:44.000000 html_text-0.5.1/setup.cfg
--rw-r--r--   0 kmike      (501) staff       (20)     4796 2018-11-19 17:56:02.000000 html_text-0.5.1/README.rst
--rw-r--r--   0 kmike      (501) staff       (20)     1897 2019-05-27 18:15:27.000000 html_text-0.5.1/CHANGES.rst
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2019-05-28 18:47:44.000000 html_text-0.5.1/html_text/
--rw-r--r--   0 kmike      (501) staff       (20)      240 2019-05-27 18:16:06.000000 html_text-0.5.1/html_text/__init__.py
--rw-r--r--   0 kmike      (501) staff       (20)     7136 2019-05-25 21:55:19.000000 html_text-0.5.1/html_text/html_text.py
+drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.716843 html_text-0.5.2/
+-rw-r--r--   0 kmike      (501) staff       (20)     2084 2020-07-22 19:11:16.000000 html_text-0.5.2/CHANGES.rst
+-rw-r--r--   0 kmike      (501) staff       (20)     1079 2018-11-01 22:27:25.000000 html_text-0.5.2/LICENSE
+-rw-r--r--   0 kmike      (501) staff       (20)      243 2018-11-01 22:27:25.000000 html_text-0.5.2/MANIFEST.in
+-rw-r--r--   0 kmike      (501) staff       (20)     9400 2020-07-22 19:12:24.717083 html_text-0.5.2/PKG-INFO
+-rw-r--r--   0 kmike      (501) staff       (20)     4796 2018-11-19 17:56:02.000000 html_text-0.5.2/README.rst
+drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.699226 html_text-0.5.2/html_text/
+-rw-r--r--   0 kmike      (501) staff       (20)      240 2020-07-22 19:12:07.000000 html_text-0.5.2/html_text/__init__.py
+-rw-r--r--   0 kmike      (501) staff       (20)     7290 2020-07-22 17:55:44.000000 html_text-0.5.2/html_text/html_text.py
+drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.704512 html_text-0.5.2/html_text.egg-info/
+-rw-r--r--   0 kmike      (501) staff       (20)     9400 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/PKG-INFO
+-rw-r--r--   0 kmike      (501) staff       (20)      997 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/SOURCES.txt
+-rw-r--r--   0 kmike      (501) staff       (20)        1 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/dependency_links.txt
+-rw-r--r--   0 kmike      (501) staff       (20)        1 2018-11-12 15:20:23.000000 html_text-0.5.2/html_text.egg-info/not-zip-safe
+-rw-r--r--   0 kmike      (501) staff       (20)        5 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/requires.txt
+-rw-r--r--   0 kmike      (501) staff       (20)       10 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/top_level.txt
+-rw-r--r--   0 kmike      (501) staff       (20)      381 2020-07-22 19:12:24.717984 html_text-0.5.2/setup.cfg
+-rwxr-xr-x   0 kmike      (501) staff       (20)     1231 2020-07-22 19:12:07.000000 html_text-0.5.2/setup.py
+drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.706049 html_text-0.5.2/tests/
+-rw-r--r--   0 kmike      (501) staff       (20)       24 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/__init__.py
+-rw-r--r--   0 kmike      (501) staff       (20)     7890 2020-07-22 17:55:44.000000 html_text-0.5.2/tests/test_html_text.py
+drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.716242 html_text-0.5.2/tests/test_webpages/
+-rw-r--r--   0 kmike      (501) staff       (20)     9279 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
+-rw-r--r--   0 kmike      (501) staff       (20)     1539 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
+-rw-r--r--   0 kmike      (501) staff       (20)    10225 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
+-rw-r--r--   0 kmike      (501) staff       (20)     2852 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
+-rw-r--r--   0 kmike      (501) staff       (20)    67149 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html
+-rw-r--r--   0 kmike      (501) staff       (20)     4635 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
+-rw-r--r--   0 kmike      (501) staff       (20)    38239 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
+-rw-r--r--   0 kmike      (501) staff       (20)    10856 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
+-rw-r--r--   0 kmike      (501) staff       (20)    11694 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
+-rw-r--r--   0 kmike      (501) staff       (20)     1228 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `html_text-0.5.1/PKG-INFO` & `html_text-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: html_text
-Version: 0.5.1
+Version: 0.5.2
 Summary: Extract text from HTML
 Home-page: https://github.com/TeamHG-Memex/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
 Description: ============
         HTML to Text
@@ -139,14 +139,22 @@
         	:alt: define hyperiongray
         
         
         =======
         History
         =======
         
+        0.5.2 (2020-07-22)
+        ------------------
+        
+        * Handle lxml Cleaner exceptions (a workaround for
+          https://bugs.launchpad.net/lxml/+bug/1838497 );
+        * Python 3.8 support;
+        * testing improvements.
+        
         0.5.1 (2019-05-27)
         ------------------
         
         Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
         producing unnecessary spaces after newlines.
         
         0.5.0 (2018-11-19)
@@ -223,7 +231,8 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.1 Name: html_text Version: 0.5.1 Summary: Extract text from
+Metadata-Version: 1.1 Name: html_text Version: 0.5.2 Summary: Extract text from
 HTML Home-page: https://github.com/TeamHG-Memex/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
 Description: ============ HTML to Text ============ .. image:: https://
 img.shields.io/pypi/v/html-text.svg :target: https://pypi.python.org/pypi/html-
 text :alt: PyPI Version .. image:: https://img.shields.io/travis/TeamHG-Memex/
 html-text.svg :target: https://travis-ci.org/TeamHG-Memex/html-text :alt: Build
 Status .. image:: http://codecov.io/github/TeamHG-Memex/soft404/
@@ -66,26 +66,28 @@
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
 webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
 hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
 www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.5.1 (2019-05-27) -----------------
-- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
---- Parsel dependency is removed in this release, though parsel is still
-supported. * ``parsel`` package is no longer required to install and use html-
-text; * ``html_text.etree_to_text`` function allows to extract text from lxml
-Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
-with options tuned for text extraction speed and quality; * test and
-documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
--------- Fixed a regression in 0.4.0 release: text was empty when
-``html_text.extract_text`` is called with a node with text, but without
-children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
+hyperiongray ======= History ======= 0.5.2 (2020-07-22) ------------------ *
+Handle lxml Cleaner exceptions (a workaround for https://bugs.launchpad.net/
+lxml/+bug/1838497 ); * Python 3.8 support; * testing improvements. 0.5.1 (2019-
+05-27) ------------------ Fixed whitespace handling when ``guess_punct_space``
+is False: html-text was producing unnecessary spaces after newlines. 0.5.0
+(2018-11-19) ------------------ Parsel dependency is removed in this release,
+though parsel is still supported. * ``parsel`` package is no longer required to
+install and use html-text; * ``html_text.etree_to_text`` function allows to
+extract text from lxml Elements; * ``html_text.cleaner`` is an
+``lxml.html.clean.Cleaner`` instance with options tuned for text extraction
+speed and quality; * test and documentation improvements; * Python 3.7 support.
+0.4.1 (2018-09-25) ------------------ Fixed a regression in 0.4.0 release: text
+was empty when ``html_text.extract_text`` is called with a node with text, but
+without children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
 incompatible release: by default html_text functions now add newlines after
 elements, if appropriate, to make the extracted text to look more like how it
 is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
 html_text functions. * ``guess_layout`` option to to make extracted text look
 more like how it is rendered in browser. * Add tests of layout extraction for
 real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
 operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
@@ -97,8 +99,8 @@
 (2016-09-27) ------------------ * First release on PyPI. Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `html_text-0.5.1/LICENSE` & `html_text-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/html_text.egg-info/PKG-INFO` & `html_text-0.5.2/html_text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: html-text
-Version: 0.5.1
+Version: 0.5.2
 Summary: Extract text from HTML
 Home-page: https://github.com/TeamHG-Memex/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
 Description: ============
         HTML to Text
@@ -139,14 +139,22 @@
         	:alt: define hyperiongray
         
         
         =======
         History
         =======
         
+        0.5.2 (2020-07-22)
+        ------------------
+        
+        * Handle lxml Cleaner exceptions (a workaround for
+          https://bugs.launchpad.net/lxml/+bug/1838497 );
+        * Python 3.8 support;
+        * testing improvements.
+        
         0.5.1 (2019-05-27)
         ------------------
         
         Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
         producing unnecessary spaces after newlines.
         
         0.5.0 (2018-11-19)
@@ -223,7 +231,8 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.1 Name: html-text Version: 0.5.1 Summary: Extract text from
+Metadata-Version: 1.1 Name: html-text Version: 0.5.2 Summary: Extract text from
 HTML Home-page: https://github.com/TeamHG-Memex/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
 Description: ============ HTML to Text ============ .. image:: https://
 img.shields.io/pypi/v/html-text.svg :target: https://pypi.python.org/pypi/html-
 text :alt: PyPI Version .. image:: https://img.shields.io/travis/TeamHG-Memex/
 html-text.svg :target: https://travis-ci.org/TeamHG-Memex/html-text :alt: Build
 Status .. image:: http://codecov.io/github/TeamHG-Memex/soft404/
@@ -66,26 +66,28 @@
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
 webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
 hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
 www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.5.1 (2019-05-27) -----------------
-- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
---- Parsel dependency is removed in this release, though parsel is still
-supported. * ``parsel`` package is no longer required to install and use html-
-text; * ``html_text.etree_to_text`` function allows to extract text from lxml
-Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
-with options tuned for text extraction speed and quality; * test and
-documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
--------- Fixed a regression in 0.4.0 release: text was empty when
-``html_text.extract_text`` is called with a node with text, but without
-children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
+hyperiongray ======= History ======= 0.5.2 (2020-07-22) ------------------ *
+Handle lxml Cleaner exceptions (a workaround for https://bugs.launchpad.net/
+lxml/+bug/1838497 ); * Python 3.8 support; * testing improvements. 0.5.1 (2019-
+05-27) ------------------ Fixed whitespace handling when ``guess_punct_space``
+is False: html-text was producing unnecessary spaces after newlines. 0.5.0
+(2018-11-19) ------------------ Parsel dependency is removed in this release,
+though parsel is still supported. * ``parsel`` package is no longer required to
+install and use html-text; * ``html_text.etree_to_text`` function allows to
+extract text from lxml Elements; * ``html_text.cleaner`` is an
+``lxml.html.clean.Cleaner`` instance with options tuned for text extraction
+speed and quality; * test and documentation improvements; * Python 3.7 support.
+0.4.1 (2018-09-25) ------------------ Fixed a regression in 0.4.0 release: text
+was empty when ``html_text.extract_text`` is called with a node with text, but
+without children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
 incompatible release: by default html_text functions now add newlines after
 elements, if appropriate, to make the extracted text to look more like how it
 is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
 html_text functions. * ``guess_layout`` option to to make extracted text look
 more like how it is rendered in browser. * Add tests of layout extraction for
 real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
 operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
@@ -97,8 +99,8 @@
 (2016-09-27) ------------------ * First release on PyPI. Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `html_text-0.5.1/html_text.egg-info/SOURCES.txt` & `html_text-0.5.2/html_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt` & `html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html` & `html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt` & `html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt` & `html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt` & `html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html` & `html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Scrapinghub Enterprise Solutions.txt` & `html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html` & `html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.html` & `html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_webpages/Scrapinghub Enterprise Solutions.html` & `html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/tests/test_html_text.py` & `html_text-0.5.2/tests/test_html_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,21 @@
 
 
 def test_inline_tags_whitespace(all_options):
     html = u'<span>field</span><span>value  of</span><span></span>'
     assert extract_text(html, **all_options) == u'field value of'
 
 
+def test_extract_text_from_fail_html():
+    html = "<html><frameset><frame></frameset></html>"
+    tree = parse_html(html)
+    node = tree.xpath('/html/frameset')[0]
+    assert extract_text(node) == u''
+
+
 def test_punct_whitespace():
     html = u'<div><span>field</span>, and more</div>'
     assert extract_text(html, guess_punct_space=False) == u'field , and more'
     assert extract_text(html, guess_punct_space=True) == u'field, and more'
 
 
 def test_punct_whitespace_preserved():
```

### Comparing `html_text-0.5.1/setup.py` & `html_text-0.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('CHANGES.rst') as history_file:
     history = history_file.read()
 
 
 setup(
     name='html_text',
-    version='0.5.1',
+    version='0.5.2',
     description="Extract text from HTML",
     long_description=readme + '\n\n' + history,
     author="Konstantin Lopukhin",
     author_email='kostia.lopuhin@gmail.com',
     url='https://github.com/TeamHG-Memex/html-text',
     packages=['html_text'],
     include_package_data=True,
@@ -30,11 +30,12 @@
         'Natural Language :: English',
         "Programming Language :: Python :: 2",
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
     ],
     test_suite='tests',
     tests_require=['pytest'],
 )
```

### Comparing `html_text-0.5.1/README.rst` & `html_text-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `html_text-0.5.1/CHANGES.rst` & `html_text-0.5.2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+0.5.2 (2020-07-22)
+------------------
+
+* Handle lxml Cleaner exceptions (a workaround for
+  https://bugs.launchpad.net/lxml/+bug/1838497 );
+* Python 3.8 support;
+* testing improvements.
+
 0.5.1 (2019-05-27)
 ------------------
 
 Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
 producing unnecessary spaces after newlines.
 
 0.5.0 (2018-11-19)
```

### Comparing `html_text-0.5.1/html_text/html_text.py` & `html_text-0.5.2/html_text/html_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,22 @@
 
 
 def _cleaned_html_tree(html):
     if isinstance(html, lxml.html.HtmlElement):
         tree = html
     else:
         tree = parse_html(html)
-    return cleaner.clean_html(tree)
+
+    # we need this as https://bugs.launchpad.net/lxml/+bug/1838497
+    try:
+        cleaned = cleaner.clean_html(tree)
+    except AssertionError:
+        cleaned = tree
+
+    return cleaned
 
 
 def parse_html(html):
     """ Create an lxml.html.HtmlElement from a string with html.
     XXX: mostly copy-pasted from parsel.selector.create_root_node
     """
     body = html.strip().replace('\x00', '').encode('utf8') or b'<html/>'
```


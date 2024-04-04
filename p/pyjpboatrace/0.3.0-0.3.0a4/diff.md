# Comparing `tmp/pyjpboatrace-0.3.0.tar.gz` & `tmp/pyjpboatrace-0.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjpboatrace-0.3.0.tar", last modified: Tue Oct 10 06:51:07 2023, max compression
+gzip compressed data, was "pyjpboatrace-0.3.0a4.tar", last modified: Thu Apr  4 13:27:51 2024, max compression
```

## Comparing `pyjpboatrace-0.3.0.tar` & `pyjpboatrace-0.3.0a4.tar`

### file list

```diff
@@ -1,64 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    47300 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46306 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.574437 pyjpboatrace-0.3.0/pyjpboatrace/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/certification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.578437 pyjpboatrace-0.3.0/pyjpboatrace/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/better.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/betting_limit_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/depositor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/operator/withdrawer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/pyjpboatrace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.578437 pyjpboatrace-0.3.0/pyjpboatrace/scraper/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_beforeinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_odds2tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_odds3f.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_odds3t.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_oddsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_oddstf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_raceindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_racelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/parse_html_raceresult.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/_parser/scrape_odds_update_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/exacta_quinella_odds_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/just_before_info_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/quinellaplace_odds_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/race_info_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/races_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/result_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/stadiums_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/trifecta_odds_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/trio_odds_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/scraper/win_placeshow_odds_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/user_information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/pyjpboatrace/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/utils/str2num.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/pyjpboatrace/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.578437 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47300 2023-10-10 06:51:07.000000 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-10-10 06:51:07.000000 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 06:51:07.000000 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-10 06:51:07.000000 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-10 06:51:07.000000 pyjpboatrace-0.3.0/pyjpboatrace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 06:51:07.582437 pyjpboatrace-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/tests/test_certification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/tests/test_pyjpboatrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-10-10 06:50:30.000000 pyjpboatrace-0.3.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49608 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47096 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.144098 pyjpboatrace-0.3.0a4/pyjpboatrace/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/certification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/pyjpboatrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/user_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49608 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_certification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_pyjpboatrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_validator.py
```

### Comparing `pyjpboatrace-0.3.0/LICENSE` & `pyjpboatrace-0.3.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/PKG-INFO` & `pyjpboatrace-0.3.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,71 @@
 Metadata-Version: 2.1
 Name: pyjpboatrace
-Version: 0.3.0
+Version: 0.3.0a4
 Summary: PyJPBoatrace: Python-based Japanese boatrace tools
-Home-page: http://github.com/hmasdev/pyjpboatrace
-Author: hmasdev
-Author-email: hmasuidev1com@gmail.com
+Author-email: hmasdev <hmasuidev1com@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020 hmasdev
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, http://github.com/hmasdev/pyjpboatrace
 Keywords: kyotei,boatrace,data analysis
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: selenium>=4.6.0
 Requires-Dist: types-beautifulsoup4
 Requires-Dist: types-requests
 Provides-Extra: dev
-Requires-Dist: pytest>=6.1.2; extra == "dev"
-Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
+Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: flake8>=3.8.4; extra == "dev"
 Requires-Dist: mypy>=0.812; extra == "dev"
+Requires-Dist: pytest>=6.1.2; extra == "dev"
+Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: types-pytz; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![Pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
+![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -54,16 +84,16 @@
 - python >= 3.8
 - requests>=2.28.1
 - beautifulsoup4>=4.11.1
 - selenium>=4.6
 
 ### User installation
 
-```
-    pip install -U pyjpboatrace
+```bash
+pip install -U pyjpboatrace
 ```
 
 ## How to use
 
 1. (optional) create an instance of UserInformation;
 2. (optional) create a selenium driver;
 3. create an instance of PyJPBoatrace;
@@ -1309,15 +1339,14 @@
 The map between integers and stadiums is given by `STADIUMS_MAP` in `pyjpboatrace.const`.
 
 ## Contribution Guide
 
 ### Requirement
 
 - Python >= 3.8
-- Pipenv (You can install pipenv by `pip install pipenv`)
 - Chrome
 - Firefox
 - bash
 - curl
 
 ### Issues
 
@@ -1334,73 +1363,114 @@
 3. Test codes according to [Test Subsection](#HowToTestAnchor);
 4. Commit your changes (`git commit -am 'Add xxxx feature`);
 5. Push to the branch (`git push origin feature/xxxx`);
 6. Create new Pull Request
 
 ### Setup the develop environment
 
-If you use `pipenv`, executing the following command to create your develop environment:
+First, fork this repository and clone it to your local machine.
 
 ```bash
-$ pipenv sync --dev
+$ git clone https://github.com/hmasdev/pyjpboatrace/
+$ cd pyjpboatrace
 ```
 
-If you do not `pipenv`, `venv` is an alternative library to create your develop environment:
+Then, create a virtual environment for your development,
+and install the required libraries.
 
 ```bash
 $ python -m venv venv
-$ source venv/Scripts/activate
+$ source venv/bin/activate  # for Linux or MacOS
+$ # venv\Scripts\activate  # for Windows
 $ pip install -e .[dev]
 ```
 
-Note that `pipenv` is recommended.
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ pipenv sync --dev
+```
+
+</details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
 $ ./download_html_for_test.sh  # Only 1 time
+$ pytest -m "not integrate and not spending_money" # unit tests
+$ pytest # unit tests and integration tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ ./download_html_for_test.sh  # Only 1 time
 $ pipenv run pytest -m "not integrate and not spending_money" # unit tests
 $ pipenv run pytest  # unit tests and integration tests
 ```
 
-`pipenv run pytest` does not test depositing, withdrawing or betting.
+</details>
+
+`pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
 ```json
 {
   "userid": "YOUR_USER_ID",
   "pin": "YOUR_PIN",
   "auth_pass": "YOUR_AUTHENTIFICATION_PASSWORD",
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
+$ pytest -m "spending_money"
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run pytest -m "spending_money"
 ```
 
+</details>
+
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
+$ flake8 pyjpboatrace tests
+$ mypy pyjpboatrace tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run flake8 pyjpboatrace
 $ pipenv run flake8 tests
 $ pipenv run mypy pyjpboatrace
 $ pipenv run mypy tests
 ```
 
+</details>
+
+
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
 
 [hmasdev](https://github.com/hmasdev)
```

### Comparing `pyjpboatrace-0.3.0/README.md` & `pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,71 @@
+Metadata-Version: 2.1
+Name: pyjpboatrace
+Version: 0.3.0a4
+Summary: PyJPBoatrace: Python-based Japanese boatrace tools
+Author-email: hmasdev <hmasuidev1com@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020 hmasdev
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, http://github.com/hmasdev/pyjpboatrace
+Keywords: kyotei,boatrace,data analysis
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.11.1
+Requires-Dist: requests>=2.28.1
+Requires-Dist: selenium>=4.6.0
+Requires-Dist: types-beautifulsoup4
+Requires-Dist: types-requests
+Provides-Extra: dev
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: flake8>=3.8.4; extra == "dev"
+Requires-Dist: mypy>=0.812; extra == "dev"
+Requires-Dist: pytest>=6.1.2; extra == "dev"
+Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: types-pytz; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![Pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
+![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -27,16 +84,16 @@
 - python >= 3.8
 - requests>=2.28.1
 - beautifulsoup4>=4.11.1
 - selenium>=4.6
 
 ### User installation
 
-```
-    pip install -U pyjpboatrace
+```bash
+pip install -U pyjpboatrace
 ```
 
 ## How to use
 
 1. (optional) create an instance of UserInformation;
 2. (optional) create a selenium driver;
 3. create an instance of PyJPBoatrace;
@@ -1282,15 +1339,14 @@
 The map between integers and stadiums is given by `STADIUMS_MAP` in `pyjpboatrace.const`.
 
 ## Contribution Guide
 
 ### Requirement
 
 - Python >= 3.8
-- Pipenv (You can install pipenv by `pip install pipenv`)
 - Chrome
 - Firefox
 - bash
 - curl
 
 ### Issues
 
@@ -1307,73 +1363,114 @@
 3. Test codes according to [Test Subsection](#HowToTestAnchor);
 4. Commit your changes (`git commit -am 'Add xxxx feature`);
 5. Push to the branch (`git push origin feature/xxxx`);
 6. Create new Pull Request
 
 ### Setup the develop environment
 
-If you use `pipenv`, executing the following command to create your develop environment:
+First, fork this repository and clone it to your local machine.
 
 ```bash
-$ pipenv sync --dev
+$ git clone https://github.com/hmasdev/pyjpboatrace/
+$ cd pyjpboatrace
 ```
 
-If you do not `pipenv`, `venv` is an alternative library to create your develop environment:
+Then, create a virtual environment for your development,
+and install the required libraries.
 
 ```bash
 $ python -m venv venv
-$ source venv/Scripts/activate
+$ source venv/bin/activate  # for Linux or MacOS
+$ # venv\Scripts\activate  # for Windows
 $ pip install -e .[dev]
 ```
 
-Note that `pipenv` is recommended.
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ pipenv sync --dev
+```
+
+</details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
 $ ./download_html_for_test.sh  # Only 1 time
+$ pytest -m "not integrate and not spending_money" # unit tests
+$ pytest # unit tests and integration tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ ./download_html_for_test.sh  # Only 1 time
 $ pipenv run pytest -m "not integrate and not spending_money" # unit tests
 $ pipenv run pytest  # unit tests and integration tests
 ```
 
-`pipenv run pytest` does not test depositing, withdrawing or betting.
+</details>
+
+`pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
 ```json
 {
   "userid": "YOUR_USER_ID",
   "pin": "YOUR_PIN",
   "auth_pass": "YOUR_AUTHENTIFICATION_PASSWORD",
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
+$ pytest -m "spending_money"
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run pytest -m "spending_money"
 ```
 
+</details>
+
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
+$ flake8 pyjpboatrace tests
+$ mypy pyjpboatrace tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run flake8 pyjpboatrace
 $ pipenv run flake8 tests
 $ pipenv run mypy pyjpboatrace
 $ pipenv run mypy tests
 ```
 
+</details>
+
+
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
 
 [hmasdev](https://github.com/hmasdev)
```

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/__init__.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import pyjpboatrace
 from . import scraper
 from . import user_information
 from . import utils
 from . import validator
 
 
-__version__ = '0.3.0'
+__version__ = 'v0.3.0a4'
 
 __all__ = [
     PyJPBoatrace.__name__,
     certification.__name__,
     const.__name__,
     drivers.__name__,
     exceptions.__name__,
```

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/certification.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/certification.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,24 +23,35 @@
     Args:
         driver (webdriver.remote.webdriver.WebDriver): webdriver.
         user (UserInformation): User information.
         timeout (int, optional): Timeout parameter. Defaults to 15.
         logger (Logger, optional): logger. Defaults to getLogger(__name__).
 
     Raises:
+        ValueError: Occurred when user.userid is None.
+        ValueError: Occurred when user.pin is None.
+        ValueError: Occurred when user.auth_pass is None.
         LoginFailException: Occurred when login failure.
 
     Returns:
         bool: Whether login is succeeded.
 
     NOTE:
         Behavior:
             Return True when login is succeeded;
             Raise LoginFailException when login is failed.
     """
+    # validate
+    if user.userid is None:
+        raise ValueError('User ID is not set.')
+    if user.pin is None:
+        raise ValueError('PIN is not set.')
+    if user.auth_pass is None:
+        raise ValueError('Authentification password is not set.')
+
     # get
     driver.get(BOATRACEJP_LOGIN_URL)
 
     # send keys
     WebDriverWait(driver, timeout).until(
         EC.presence_of_element_located((By.NAME, 'in_KanyusyaNo'))
     )
```

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/const.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/const.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/drivers.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/drivers.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/exceptions.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/pyjpboatrace.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/pyjpboatrace.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/user_information.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/user_information.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         pin: Optional[str] = None,
         auth_pass: Optional[str] = None,
         vote_pass: Optional[str] = None,  # TODO rename vote_pass -> bet_pass
         json_file: Optional[str] = None,
         logger: Logger = getLogger(__name__)
     ):
         # preparation
-        self.userid = None
-        self.pin = None
-        self.auth_pass = None
-        self.vote_pass = None
+        self.userid: Optional[str] = None
+        self.pin: Optional[str] = None
+        self.auth_pass: Optional[str] = None
+        self.vote_pass: Optional[str] = None
 
         # load json
         if json_file is not None and os.path.exists(json_file):
             with open(json_file, 'r', encoding='utf-8-sig') as f:
                 dic = json.load(f)
             self.userid = dic.get('userid', None)
             self.pin = dic.get('pin', None)
```

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace/validator.py` & `pyjpboatrace-0.3.0a4/pyjpboatrace/validator.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/pyjpboatrace.egg-info/PKG-INFO` & `pyjpboatrace-0.3.0a4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,16 @@
-Metadata-Version: 2.1
-Name: pyjpboatrace
-Version: 0.3.0
-Summary: PyJPBoatrace: Python-based Japanese boatrace tools
-Home-page: http://github.com/hmasdev/pyjpboatrace
-Author: hmasdev
-Author-email: hmasuidev1com@gmail.com
-Keywords: kyotei,boatrace,data analysis
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.11.1
-Requires-Dist: requests>=2.28.1
-Requires-Dist: selenium>=4.6.0
-Requires-Dist: types-beautifulsoup4
-Requires-Dist: types-requests
-Provides-Extra: dev
-Requires-Dist: pytest>=6.1.2; extra == "dev"
-Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
-Requires-Dist: flake8>=3.8.4; extra == "dev"
-Requires-Dist: mypy>=0.812; extra == "dev"
-
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![Pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
+![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
+![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -54,16 +29,16 @@
 - python >= 3.8
 - requests>=2.28.1
 - beautifulsoup4>=4.11.1
 - selenium>=4.6
 
 ### User installation
 
-```
-    pip install -U pyjpboatrace
+```bash
+pip install -U pyjpboatrace
 ```
 
 ## How to use
 
 1. (optional) create an instance of UserInformation;
 2. (optional) create a selenium driver;
 3. create an instance of PyJPBoatrace;
@@ -1309,15 +1284,14 @@
 The map between integers and stadiums is given by `STADIUMS_MAP` in `pyjpboatrace.const`.
 
 ## Contribution Guide
 
 ### Requirement
 
 - Python >= 3.8
-- Pipenv (You can install pipenv by `pip install pipenv`)
 - Chrome
 - Firefox
 - bash
 - curl
 
 ### Issues
 
@@ -1334,73 +1308,114 @@
 3. Test codes according to [Test Subsection](#HowToTestAnchor);
 4. Commit your changes (`git commit -am 'Add xxxx feature`);
 5. Push to the branch (`git push origin feature/xxxx`);
 6. Create new Pull Request
 
 ### Setup the develop environment
 
-If you use `pipenv`, executing the following command to create your develop environment:
+First, fork this repository and clone it to your local machine.
 
 ```bash
-$ pipenv sync --dev
+$ git clone https://github.com/hmasdev/pyjpboatrace/
+$ cd pyjpboatrace
 ```
 
-If you do not `pipenv`, `venv` is an alternative library to create your develop environment:
+Then, create a virtual environment for your development,
+and install the required libraries.
 
 ```bash
 $ python -m venv venv
-$ source venv/Scripts/activate
+$ source venv/bin/activate  # for Linux or MacOS
+$ # venv\Scripts\activate  # for Windows
 $ pip install -e .[dev]
 ```
 
-Note that `pipenv` is recommended.
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ pipenv sync --dev
+```
+
+</details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
 $ ./download_html_for_test.sh  # Only 1 time
+$ pytest -m "not integrate and not spending_money" # unit tests
+$ pytest # unit tests and integration tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
+$ ./download_html_for_test.sh  # Only 1 time
 $ pipenv run pytest -m "not integrate and not spending_money" # unit tests
 $ pipenv run pytest  # unit tests and integration tests
 ```
 
-`pipenv run pytest` does not test depositing, withdrawing or betting.
+</details>
+
+`pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
 ```json
 {
   "userid": "YOUR_USER_ID",
   "pin": "YOUR_PIN",
   "auth_pass": "YOUR_AUTHENTIFICATION_PASSWORD",
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
+$ pytest -m "spending_money"
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run pytest -m "spending_money"
 ```
 
+</details>
+
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
+$ flake8 pyjpboatrace tests
+$ mypy pyjpboatrace tests
+```
+
+<details>
+<summary>[Deprecated] when using `pipenv`</summary>
+
+```bash
 $ pipenv run flake8 pyjpboatrace
 $ pipenv run flake8 tests
 $ pipenv run mypy pyjpboatrace
 $ pipenv run mypy tests
 ```
 
+</details>
+
+
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
 
 [hmasdev](https://github.com/hmasdev)
```

### Comparing `pyjpboatrace-0.3.0/tests/test_certification.py` & `pyjpboatrace-0.3.0a4/tests/test_certification.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/tests/test_drivers.py` & `pyjpboatrace-0.3.0a4/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/tests/test_pyjpboatrace.py` & `pyjpboatrace-0.3.0a4/tests/test_pyjpboatrace.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0/tests/test_validator.py` & `pyjpboatrace-0.3.0a4/tests/test_validator.py`

 * *Files identical despite different names*


# Comparing `tmp/squaredown-1.4.3.tar.gz` & `tmp/squaredown-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaredown-1.4.3.tar", max compression
+gzip compressed data, was "squaredown-1.5.1.tar", max compression
```

## Comparing `squaredown-1.4.3.tar` & `squaredown-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1079 2020-08-22 21:27:12.749605 squaredown-1.4.3/LICENSE
--rw-r--r--   0        0        0     1405 2022-11-02 16:59:09.235680 squaredown-1.4.3/README.md
--rw-r--r--   0        0        0      884 2023-05-30 19:57:48.818305 squaredown-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      259 2023-05-30 19:58:01.902402 squaredown-1.4.3/squaredown/__init__.py
--rw-r--r--   0        0        0     5629 2022-11-03 03:18:23.859642 squaredown-1.4.3/squaredown/catalog.py
--rw-r--r--   0        0        0     3128 2022-11-03 03:03:40.528656 squaredown-1.4.3/squaredown/connector.py
--rw-r--r--   0        0        0    12628 2021-02-23 14:21:00.968617 squaredown-1.4.3/squaredown/i_square.py
--rw-r--r--   0        0        0     4088 2022-11-03 03:18:23.863642 squaredown-1.4.3/squaredown/itemizations.py
--rw-r--r--   0        0        0     2244 2022-11-03 03:18:23.863642 squaredown-1.4.3/squaredown/locations.py
--rw-r--r--   0        0        0      987 2021-02-23 14:21:00.968617 squaredown-1.4.3/squaredown/logging_config.json
--rw-r--r--   0        0        0    16660 2023-05-30 19:57:27.010138 squaredown-1.4.3/squaredown/orders.py
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 squaredown-1.4.3/setup.py
--rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 squaredown-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-01 04:26:49.305738 squaredown-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1405 2024-04-01 04:26:49.305738 squaredown-1.5.1/README.md
+-rw-r--r--   0        0        0      912 2024-04-01 04:26:49.305738 squaredown-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/__init__.py
+-rw-r--r--   0        0        0     5629 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/catalog.py
+-rw-r--r--   0        0        0     3128 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/connector.py
+-rw-r--r--   0        0        0    12628 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/i_square.py
+-rw-r--r--   0        0        0     4088 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/itemizations.py
+-rw-r--r--   0        0        0     2244 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/locations.py
+-rw-r--r--   0        0        0      987 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/logging_config.json
+-rw-r--r--   0        0        0    16660 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/orders.py
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.5.1/PKG-INFO
```

### Comparing `squaredown-1.4.3/LICENSE` & `squaredown-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/README.md` & `squaredown-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/pyproject.toml` & `squaredown-1.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaredown"
-version = "1.4.3"
+version = "1.5.1"
 description = "Customized Square interface"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/squaredown"
 keywords = ["python", "square", "mongodb"]
 packages = [{include = "squaredown"}]
@@ -24,13 +24,14 @@
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-addopts = "-p no:warnings --cov-report xml:tests/cov.xml --cov=i_mongodb tests/"
+addopts = "-p no:warnings --cov-report xml:tests/cov.xml --cov=squaredown tests/"
+#addopts = "-p no:warnings
 log_cli = true
 log_cli_level = "DEBUG"
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "logging-fstring-interpolation"
```

### Comparing `squaredown-1.4.3/squaredown/catalog.py` & `squaredown-1.5.1/squaredown/catalog.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/connector.py` & `squaredown-1.5.1/squaredown/connector.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/i_square.py` & `squaredown-1.5.1/squaredown/i_square.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/itemizations.py` & `squaredown-1.5.1/squaredown/itemizations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/locations.py` & `squaredown-1.5.1/squaredown/locations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/logging_config.json` & `squaredown-1.5.1/squaredown/logging_config.json`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/squaredown/orders.py` & `squaredown-1.5.1/squaredown/orders.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.3/setup.py` & `squaredown-1.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,70 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: squaredown
+Version: 1.5.1
+Summary: Customized Square interface
+Home-page: https://github.com/aracnid/squaredown
+License: MIT
+Keywords: python,square,mongodb
+Author: Jason Romano
+Author-email: aracnid@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aracnid-config (>=1.0,<2.0)
+Requires-Dist: aracnid-logger (>=1.0,<2.0)
+Requires-Dist: aracnid-utils (>=1.0,<2.0)
+Requires-Dist: i-mongodb (>=2.0,<3.0)
+Requires-Dist: squareup (>=19.1,<20.0)
+Requires-Dist: tqdm (>=4.64,<5.0)
+Project-URL: Repository, https://github.com/aracnid/squaredown
+Description-Content-Type: text/markdown
 
-packages = \
-['squaredown']
+# Squaredown
 
-package_data = \
-{'': ['*']}
+We use Square as our point of sale system for our businesses. It works really well for most applications, but it takes too long to produce reports in a way that meets our business needs and the process is just too manual. We needed an automated way to produce our customized reports either at a click of a button or on a schedule. To do that we download the Square data into a MongoDB database. This is the code that we use to connect Square to MongoDB.
 
-install_requires = \
-['aracnid-config>=1.0,<2.0',
- 'aracnid-logger>=1.0,<2.0',
- 'aracnid-utils>=1.0,<2.0',
- 'i-mongodb>=2.0,<3.0',
- 'squareup>=19.1,<20.0',
- 'tqdm>=4.64,<5.0']
-
-setup_kwargs = {
-    'name': 'squaredown',
-    'version': '1.4.3',
-    'description': 'Customized Square interface',
-    'long_description': '# Squaredown\n\nWe use Square as our point of sale system for our businesses. It works really well for most applications, but it takes too long to produce reports in a way that meets our business needs and the process is just too manual. We needed an automated way to produce our customized reports either at a click of a button or on a schedule. To do that we download the Square data into a MongoDB database. This is the code that we use to connect Square to MongoDB.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nThis package supports the following version of Python. It probably supports older versions, but they have not been tested.\n\n- Python 3.10 or later\n\n### Installing\n\nInstall the latest package using pip.\n\n```bash\n$ pip install squaredown\n```\n\nEnd with an example of getting some data out of the system or using it for a little demo\n\n## Running the tests\n\nExplain how to run the automated tests for this system\n\n```bash\n$ python -m pytest\n```\n\n## Usage\n\nTODO\n\n## Authors\n\n- **Jason Romano** - [Aracnid](https://github.com/aracnid)\n\nSee also the list of [contributors](https://github.com/lakeannebrewhouse/squaredown/contributors) who participated in this project.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
-    'author': 'Jason Romano',
-    'author_email': 'aracnid@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/aracnid/squaredown',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+## Getting Started
 
+These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
+
+### Prerequisites
+
+This package supports the following version of Python. It probably supports older versions, but they have not been tested.
+
+- Python 3.10 or later
+
+### Installing
+
+Install the latest package using pip.
+
+```bash
+$ pip install squaredown
+```
+
+End with an example of getting some data out of the system or using it for a little demo
+
+## Running the tests
+
+Explain how to run the automated tests for this system
+
+```bash
+$ python -m pytest
+```
+
+## Usage
+
+TODO
+
+## Authors
+
+- **Jason Romano** - [Aracnid](https://github.com/aracnid)
+
+See also the list of [contributors](https://github.com/lakeannebrewhouse/squaredown/contributors) who participated in this project.
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
-setup(**setup_kwargs)
```


# Comparing `tmp/pytouchline_extended-0.4.tar.gz` & `tmp/pytouchline_extended-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytouchline_extended-0.4.tar", last modified: Mon Mar 18 08:31:43 2024, max compression
+gzip compressed data, was "pytouchline_extended-0.4.4.tar", last modified: Thu Apr  4 17:37:05 2024, max compression
```

## Comparing `pytouchline_extended-0.4.tar` & `pytouchline_extended-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 peter.brondum   (502) staff       (20)        0 2024-03-18 08:31:43.471503 pytouchline_extended-0.4/
--rw-r--r--   0 peter.brondum   (502) staff       (20)     1064 2024-03-15 11:29:36.000000 pytouchline_extended-0.4/LICENSE
--rw-r--r--   0 peter.brondum   (502) staff       (20)      557 2024-03-18 08:31:43.471564 pytouchline_extended-0.4/PKG-INFO
--rw-r--r--   0 peter.brondum   (502) staff       (20)      442 2024-03-18 06:55:09.000000 pytouchline_extended-0.4/README.md
-drwxr-xr-x   0 peter.brondum   (502) staff       (20)        0 2024-03-18 08:31:43.470476 pytouchline_extended-0.4/pytouchline_extended/
--rw-r--r--   0 peter.brondum   (502) staff       (20)     7549 2024-03-18 07:35:55.000000 pytouchline_extended-0.4/pytouchline_extended/__init__.py
-drwxr-xr-x   0 peter.brondum   (502) staff       (20)        0 2024-03-18 08:31:43.471395 pytouchline_extended-0.4/pytouchline_extended.egg-info/
--rw-r--r--   0 peter.brondum   (502) staff       (20)      557 2024-03-18 08:31:43.000000 pytouchline_extended-0.4/pytouchline_extended.egg-info/PKG-INFO
--rw-r--r--   0 peter.brondum   (502) staff       (20)      288 2024-03-18 08:31:43.000000 pytouchline_extended-0.4/pytouchline_extended.egg-info/SOURCES.txt
--rw-r--r--   0 peter.brondum   (502) staff       (20)        1 2024-03-18 08:31:43.000000 pytouchline_extended-0.4/pytouchline_extended.egg-info/dependency_links.txt
--rw-r--r--   0 peter.brondum   (502) staff       (20)       24 2024-03-18 08:31:43.000000 pytouchline_extended-0.4/pytouchline_extended.egg-info/requires.txt
--rw-r--r--   0 peter.brondum   (502) staff       (20)       21 2024-03-18 08:31:43.000000 pytouchline_extended-0.4/pytouchline_extended.egg-info/top_level.txt
--rw-r--r--   0 peter.brondum   (502) staff       (20)       79 2024-03-18 08:31:43.471866 pytouchline_extended-0.4/setup.cfg
--rw-r--r--   0 peter.brondum   (502) staff       (20)      660 2024-03-18 08:31:15.000000 pytouchline_extended-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 17:37:01.000000 pytouchline_extended-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-04 17:37:01.000000 pytouchline_extended-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/pytouchline_extended/
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-04-04 17:37:01.000000 pytouchline_extended-0.4.4/pytouchline_extended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-04 17:37:05.000000 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-04 17:37:05.000000 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:37:05.000000 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:37:05.000000 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 17:37:05.000000 pytouchline_extended-0.4.4/pytouchline_extended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 17:37:03.000000 pytouchline_extended-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:37:05.723440 pytouchline_extended-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 17:37:01.000000 pytouchline_extended-0.4.4/tests/test_main.py
```

### Comparing `pytouchline_extended-0.4/LICENSE` & `pytouchline_extended-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytouchline_extended-0.4/PKG-INFO` & `pytouchline_extended-0.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pytouchline_extended
-Version: 0.4
+Version: 0.4.4
 Summary: A Roth Touchline interface library
 Home-page: https://github.com/brondum/pytouchline
 Author: Peter Brondum
 License: MIT
-Download-URL: https://github.com/brondum/pytouchline/archive/0.4.tar.gz
 Keywords: Roth,Touchline,Home Assistant,hassio,Heat pump
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: httplib2
+Requires-Dist: faust-cchardet
 
-UNKNOWN
-
+A simple helper library for controlling a Roth Touchline heat pump controller
```

### Comparing `pytouchline_extended-0.4/pytouchline_extended/__init__.py` & `pytouchline_extended-0.4.4/pytouchline_extended/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 import cchardet as chardet
 import xml.etree.ElementTree as ET
 
 __author__ = 'brondum'
 
 
 class PyTouchline(object):
-	def __init__(self, id=0, ip_address=""):
+	"""
+	A Python interface for controlling a Roth Touchline heat pump controller.
+
+	Attributes:
+			id (int): The ID of the sensor.
+			url (str): The URL of the heat pump controller.
+	"""
+
+	def __init__(self, id=0, url=""):
 		self._id = id
-		self._ip_address = ip_address
+		self._url = url
 		self._temp_scale = 100
 		self._header = {"Content-Type": "text/xml"}
 		self._read_path = "/cgi-bin/ILRReadValues.cgi"
 		self._write_path = "/cgi-bin/writeVal.cgi"
 		self._parameter = {}
 		self._xml_element_list = []
 		self._xml_element_list.append(
@@ -56,14 +64,15 @@
 	def get_status(self):
 		status_items = []
 		status_items.append("<i><n>R0.SystemStatus</n></i>")
 		request = self._get_touchline_request(status_items)
 		response = self._request_and_receive_xml(request)
 		return self._parse_number_of_devices(response)
 
+	# update the roth touchline device, and parse desc, id etc.
 	def update(self):
 		device_items = self._get_touchline_device_item(self._id)
 		request = self._get_touchline_request(device_items)
 		response = self._request_and_receive_xml(request)
 		return self._parse_device(response)
 
 	def _parse_device(self, response):
@@ -98,15 +107,15 @@
 		request += "</body>"
 		return request
 
 	def write_parameter(self, parameter, value):
 		try:
 			h = httplib2.Http()
 			(resp, content) = h.request(
-				uri=self._ip_address +
+				uri=self._url +
 					self._write_path + "?" +
 					"G" + str(self._parameter["Unique ID"]) +
 					"." + str(parameter) + "=" + str(value),
 				method="GET"
 			)
 		except httplib2.ServerNotFoundError:
 			print("PyTouchline not found")
@@ -116,15 +125,15 @@
 		else:
 			return content
 
 	def _request_and_receive_xml(self, req_key):
 		try:
 			h = httplib2.Http()
 			(resp, content) = h.request(
-				uri=self._ip_address + self._read_path,
+				uri=self._url + self._read_path,
 				method="POST",
 				body=req_key,
 				headers=self._header
 			)
 		except httplib2.ServerNotFoundError:
 			print("PyTouchline not found")
```

### Comparing `pytouchline_extended-0.4/pytouchline_extended.egg-info/PKG-INFO` & `pytouchline_extended-0.4.4/pytouchline_extended.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: pytouchline-extended
-Version: 0.4
+Name: pytouchline_extended
+Version: 0.4.4
 Summary: A Roth Touchline interface library
 Home-page: https://github.com/brondum/pytouchline
 Author: Peter Brondum
 License: MIT
-Download-URL: https://github.com/brondum/pytouchline/archive/0.4.tar.gz
 Keywords: Roth,Touchline,Home Assistant,hassio,Heat pump
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: httplib2
+Requires-Dist: faust-cchardet
 
-UNKNOWN
-
+A simple helper library for controlling a Roth Touchline heat pump controller
```

### Comparing `pytouchline_extended-0.4/setup.py` & `pytouchline_extended-0.4.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 setup(
   name = 'pytouchline_extended',
   packages = ['pytouchline_extended'],
-  version = '0.4',
+  version = "0.4.4",
   description = 'A Roth Touchline interface library',
+  long_description="A simple helper library for controlling a Roth Touchline heat pump controller",
   author = 'Peter Brondum',
   license='MIT',
   url = 'https://github.com/brondum/pytouchline',
-  download_url = 'https://github.com/brondum/pytouchline/archive/0.4.tar.gz',
   keywords = ['Roth', 'Touchline', 'Home Assistant', 'hassio', "Heat pump"],
   classifiers = [
 	'Development Status :: 3 - Alpha',
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python :: 3',
   ],
```


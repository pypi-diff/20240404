# Comparing `tmp/Drumpler-1.0.2.tar.gz` & `tmp/Drumpler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.2.tar", last modified: Wed Apr  3 21:36:27 2024, max compression
+gzip compressed data, was "Drumpler-1.0.3.tar", last modified: Thu Apr  4 18:16:55 2024, max compression
```

## Comparing `Drumpler-1.0.2.tar` & `Drumpler-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-03 21:36:27.591796 Drumpler-1.0.2/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-03 21:36:27.590049 Drumpler-1.0.2/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     3432 2024-04-03 21:36:27.000000 Drumpler-1.0.2/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-03 21:36:27.000000 Drumpler-1.0.2/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-03 21:36:27.000000 Drumpler-1.0.2/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-03 21:36:27.000000 Drumpler-1.0.2/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-03 21:36:27.000000 Drumpler-1.0.2/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.2/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     3432 2024-04-03 21:36:27.590929 Drumpler-1.0.2/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     2769 2024-04-03 21:36:11.000000 Drumpler-1.0.2/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-03 21:36:27.584597 Drumpler-1.0.2/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:23:08.000000 Drumpler-1.0.2/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      599 2024-04-03 21:23:08.000000 Drumpler-1.0.2/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6474 2024-04-03 21:27:11.000000 Drumpler-1.0.2/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6432 2024-04-03 21:23:09.000000 Drumpler-1.0.2/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:23:09.000000 Drumpler-1.0.2/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-03 21:36:27.591914 Drumpler-1.0.2/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-03 21:36:20.000000 Drumpler-1.0.2/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-03 21:36:27.589029 Drumpler-1.0.2/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.2/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.064829 Drumpler-1.0.3/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.062885 Drumpler-1.0.3/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.3/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:16:55.063812 Drumpler-1.0.3/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     2701 2024-04-04 18:14:59.000000 Drumpler-1.0.3/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.057236 Drumpler-1.0.3/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      599 2024-04-03 21:23:08.000000 Drumpler-1.0.3/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6474 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.3/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-04 18:16:55.065108 Drumpler-1.0.3/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-04 18:13:09.000000 Drumpler-1.0.3/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.061828 Drumpler-1.0.3/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.3/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.2/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.3/Drumpler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,34 +20,31 @@
 Requires-Dist: psycopg2-binary
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
+# High Level Overview
+
+![Image Description](https://github.com/KarelOmab/Drumpler/blob/main/model/Drumpler%20Framework.png?raw=true)
+
 ## Features
 
 -   **RESTful API Endpoints**: Secure and scalable endpoints for handling HTTP requests, including POST, GET, PUT, and DELETE operations.
--   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with the database, supporting a variety of database systems.
+-   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with Postgres.
 -   **Job Processing**: Facilitates the asynchronous processing of tasks with support for multi-threading and multi-processing, ensuring efficient workflow automation.
--   **Event Logging**: Detailed event logging for each job processed, allowing for easy tracking and management of tasks.
+-   **Event Logging**: Detailed event logging for each HTTP request, job processing and related events, allowing for easy tracking and management of tasks.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following installed:
 
 -   Python 3.6 or later
--   Flask
--   SQLAlchemy
--   Requests
-
-Additionally, you will need:
-
--   A PostgreSQL database or any SQL database supported by SQLAlchemy.
--   An `.env` file configured with your database URI and authorization key.
+-   PostgreSQL
 
 ## Installation
 
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
@@ -72,15 +69,15 @@
 # Now, you can create an instance of the Drumpler class
 app = drumpler.Drumpler(host="0.0.0.0", port=5000, debug=True)
 
 # And call the run method on this instance
 app.run()
 ```
 
-## API Endpoints
+## API Endpoints (Drumpler)
 
 The application exposes several endpoints for interacting with the system:
 
 -   **POST** `/request`: Submit a new request for processing.
 -   **GET** `/request/<int:request_id>`: Retrieve a specific request by its ID.
 -   **GET** `/request/next-unhandled`: Fetch the next unhandled request.
 -   **PUT** `/request/<int:request_id>`: Update the status of a request.
```

### Comparing `Drumpler-1.0.2/LICENSE` & `Drumpler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.2/PKG-INFO` & `Drumpler-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,34 +20,31 @@
 Requires-Dist: psycopg2-binary
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
+# High Level Overview
+
+![Image Description](https://github.com/KarelOmab/Drumpler/blob/main/model/Drumpler%20Framework.png?raw=true)
+
 ## Features
 
 -   **RESTful API Endpoints**: Secure and scalable endpoints for handling HTTP requests, including POST, GET, PUT, and DELETE operations.
--   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with the database, supporting a variety of database systems.
+-   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with Postgres.
 -   **Job Processing**: Facilitates the asynchronous processing of tasks with support for multi-threading and multi-processing, ensuring efficient workflow automation.
--   **Event Logging**: Detailed event logging for each job processed, allowing for easy tracking and management of tasks.
+-   **Event Logging**: Detailed event logging for each HTTP request, job processing and related events, allowing for easy tracking and management of tasks.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following installed:
 
 -   Python 3.6 or later
--   Flask
--   SQLAlchemy
--   Requests
-
-Additionally, you will need:
-
--   A PostgreSQL database or any SQL database supported by SQLAlchemy.
--   An `.env` file configured with your database URI and authorization key.
+-   PostgreSQL
 
 ## Installation
 
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
@@ -72,15 +69,15 @@
 # Now, you can create an instance of the Drumpler class
 app = drumpler.Drumpler(host="0.0.0.0", port=5000, debug=True)
 
 # And call the run method on this instance
 app.run()
 ```
 
-## API Endpoints
+## API Endpoints (Drumpler)
 
 The application exposes several endpoints for interacting with the system:
 
 -   **POST** `/request`: Submit a new request for processing.
 -   **GET** `/request/<int:request_id>`: Retrieve a specific request by its ID.
 -   **GET** `/request/next-unhandled`: Fetch the next unhandled request.
 -   **PUT** `/request/<int:request_id>`: Update the status of a request.
```

### Comparing `Drumpler-1.0.2/README.md` & `Drumpler-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
+# High Level Overview
+
+![Image Description](https://github.com/KarelOmab/Drumpler/blob/main/model/Drumpler%20Framework.png?raw=true)
+
 ## Features
 
 -   **RESTful API Endpoints**: Secure and scalable endpoints for handling HTTP requests, including POST, GET, PUT, and DELETE operations.
--   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with the database, supporting a variety of database systems.
+-   **Database Integration**: Utilizes SQLAlchemy for ORM-based interactions with Postgres.
 -   **Job Processing**: Facilitates the asynchronous processing of tasks with support for multi-threading and multi-processing, ensuring efficient workflow automation.
--   **Event Logging**: Detailed event logging for each job processed, allowing for easy tracking and management of tasks.
+-   **Event Logging**: Detailed event logging for each HTTP request, job processing and related events, allowing for easy tracking and management of tasks.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following installed:
 
 -   Python 3.6 or later
--   Flask
--   SQLAlchemy
--   Requests
-
-Additionally, you will need:
-
--   A PostgreSQL database or any SQL database supported by SQLAlchemy.
--   An `.env` file configured with your database URI and authorization key.
+-   PostgreSQL
 
 ## Installation
 
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
@@ -51,15 +48,15 @@
 # Now, you can create an instance of the Drumpler class
 app = drumpler.Drumpler(host="0.0.0.0", port=5000, debug=True)
 
 # And call the run method on this instance
 app.run()
 ```
 
-## API Endpoints
+## API Endpoints (Drumpler)
 
 The application exposes several endpoints for interacting with the system:
 
 -   **POST** `/request`: Submit a new request for processing.
 -   **GET** `/request/<int:request_id>`: Retrieve a specific request by its ID.
 -   **GET** `/request/next-unhandled`: Fetch the next unhandled request.
 -   **PUT** `/request/<int:request_id>`: Update the status of a request.
```

### Comparing `Drumpler-1.0.2/drumpler/constants.py` & `Drumpler-1.0.3/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.2/drumpler/drumpler.py` & `Drumpler-1.0.3/drumpler/drumpler.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.2/drumpler/mammoth.py` & `Drumpler-1.0.3/drumpler/mammoth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import requests
 import time
 import json
 from concurrent.futures import ThreadPoolExecutor
 import multiprocessing
-from request import Request
+from .request import Request
 import threading
 from datetime import datetime, timezone
 from sqlalchemy import create_engine, Column, Integer, String, DateTime, ForeignKey, Text
 from sqlalchemy.orm import sessionmaker, relationship
 from sqlalchemy.orm import declarative_base
-from constants import DATABASE_URI, AUTHORIZATION_KEY, DRUMPLER_URL, MAMMOTH_WORKERS
+from .constants import DATABASE_URI, AUTHORIZATION_KEY, DRUMPLER_URL, MAMMOTH_WORKERS
 import signal
 
 Base = declarative_base()
 
 class Job(Base):
     __tablename__ = 'jobs'
     id = Column(Integer, primary_key=True)
```

### Comparing `Drumpler-1.0.2/drumpler/request.py` & `Drumpler-1.0.3/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.2/setup.py` & `Drumpler-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.2',
+    version='1.0.3',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.2/test/test_drumpler.py` & `Drumpler-1.0.3/test/test_drumpler.py`

 * *Files identical despite different names*


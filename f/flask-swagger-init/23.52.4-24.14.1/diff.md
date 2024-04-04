# Comparing `tmp/flask-swagger-init-23.52.4.tar.gz` & `tmp/flask-swagger-init-24.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-swagger-init-23.52.4.tar", last modified: Fri Dec 29 13:10:43 2023, max compression
+gzip compressed data, was "flask-swagger-init-24.14.1.tar", last modified: Thu Apr  4 13:21:20 2024, max compression
```

## Comparing `flask-swagger-init-23.52.4.tar` & `flask-swagger-init-24.14.1.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.977055 flask-swagger-init-23.52.4/flask_swagger_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.977055 flask-swagger-init-23.52.4/flask_swagger_generator/components/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/swagger_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/operation_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/path_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/query_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/request_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/schema_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/flask_swagger_generator/generators/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/generators/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/generators/swagger_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/version_three_specifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/flask_swagger_generator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/parameter_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/property_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/request_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/schema_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/security_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/swagger_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/url_variable_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/flask_swagger_generator/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-29 13:10:43.000000 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-12-29 13:10:43.000000 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 13:10:43.000000 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-29 13:10:43.000000 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-29 13:10:43.000000 flask-swagger-init-23.52.4/flask_swagger_init.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-29 13:10:43.981055 flask-swagger-init-23.52.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-29 13:10:35.000000 flask-swagger-init-23.52.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.507345 flask-swagger-init-24.14.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-04 13:21:20.507345 flask-swagger-init-24.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.499345 flask-swagger-init-24.14.1/flask_swagger_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.499345 flask-swagger-init-24.14.1/flask_swagger_generator/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/swagger_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.499345 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/operation_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/path_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/query_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/schema_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.503345 flask-swagger-init-24.14.1/flask_swagger_generator/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/generators/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/generators/swagger_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.503345 flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/version_three_specifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.503345 flask-swagger-init-24.14.1/flask_swagger_generator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/parameter_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/property_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/schema_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/security_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/swagger_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/url_variable_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/flask_swagger_generator/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:21:20.507345 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-04 13:21:20.000000 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-04 13:21:20.000000 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:21:20.000000 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 13:21:20.000000 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 13:21:20.000000 flask-swagger-init-24.14.1/flask_swagger_init.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 13:21:20.507345 flask-swagger-init-24.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-04 13:21:14.000000 flask-swagger-init-24.14.1/setup.py
```

### Comparing `flask-swagger-init-23.52.4/PKG-INFO` & `flask-swagger-init-24.14.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 Metadata-Version: 2.1
 Name: flask-swagger-init
-Version: 23.52.4
+Version: 24.14.1
 Summary: A library for generating and publishing Swagger specifications for Flask applications.
 Home-page: https://github.com/krlsedu/flask-swagger-generator.git
 Author: Carlos Eduardo
 License: MIT
-Description: # Flask Swagger Generator
-        Flask swagger generator is a library to create Swagger Open API definitions 
-        for Flask based applications. Swagger is an Interface Description Language for describing REST 
-        APIs expressed using JSON and YAML. 
-        
-        ## Installing 
-        Install and update using pip:
-        
-        ```
-        pip install flask-swagger-init
-        ```
-        
-        ## Documentation and Examples
-        COMING SOON
-        
-        ## A Simple Example
-        
-        ```python
-        
-        from flask import Flask
-        from flask_swagger_generator.generators.swagger_view import SwaggerView
-        
-        
-        # Create the flask app
-        app = Flask(__name__)
-        ...
-        # Create all the routes for the app
-        ...
-        
-        # Note: The swagger view must be created after all the routes have been created
-        # Create and publish the swagger view
-        SwaggerView.init(app=app, 
-                         application_version='1.0.0', 
-                         application_name='My API', 
-                         application_description='My API description')
-        ```
-        
-        ## License
-        This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
-        
-        ## Based on
-        This application is based on the [flask-swagger-generator](https://github.com/coding-kitties/flask-swagger-generator) project by [Coding Kitties](https://github.com/coding-kitties).
-        
 Keywords: Flask,swagger,swagger generator,OpenAPI
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: flask~=3.0.0
+Requires-Dist: marshmallow>=3.0.0
+Requires-Dist: setuptools>=65.5.1
+Requires-Dist: flask_swagger_ui>=3.25.0
+
+# Flask Swagger Generator
+Flask swagger generator is a library to create Swagger Open API definitions 
+for Flask based applications. Swagger is an Interface Description Language for describing REST 
+APIs expressed using JSON and YAML. 
+
+## Installing 
+Install and update using pip:
+
+```
+pip install flask-swagger-init
+```
+
+## Documentation and Examples
+COMING SOON
+
+## A Simple Example
+
+```python
+
+from flask import Flask
+from flask_swagger_generator.generators.swagger_view import SwaggerView
+
+
+# Create the flask app
+app = Flask(__name__)
+...
+# Create all the routes for the app
+...
+
+# Note: The swagger view must be created after all the routes have been created
+# Create and publish the swagger view
+SwaggerView.init(app=app, 
+                 application_version='1.0.0', 
+                 application_name='My API', 
+                 application_description='My API description')
+```
+
+## License
+This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
+
+## Based on
+This application is based on the [flask-swagger-generator](https://github.com/coding-kitties/flask-swagger-generator) project by [Coding Kitties](https://github.com/coding-kitties).
```

### Comparing `flask-swagger-init-23.52.4/README.md` & `flask-swagger-init-24.14.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/swagger_models.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/swagger_models.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/swagger_version.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/swagger_version.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/__init__.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/path.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/path.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/path_parameter.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/path_parameter.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/query_parameter.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/query_parameter.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/request_body.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/request_body.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/request_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/request_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/response.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/response.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/schema_attribute.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/schema_attribute.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/schemas.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/security.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/security.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/components/version_three/tag.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/components/version_three/tag.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/generators/generator.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/generators/generator.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/generators/swagger_view.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/generators/swagger_view.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/swagger_specifier.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/specifiers/version_three_specifier.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/specifiers/version_three_specifier.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/__init__.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/input_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/parameter_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/property_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/property_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/request_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/security_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/swagger_version.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/swagger_version.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/url_variable_type.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/url_variable_type.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_generator/utils/utils.py` & `flask-swagger-init-24.14.1/flask_swagger_generator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask-swagger-init-23.52.4/flask_swagger_init.egg-info/PKG-INFO` & `flask-swagger-init-24.14.1/flask_swagger_init.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 Metadata-Version: 2.1
 Name: flask-swagger-init
-Version: 23.52.4
+Version: 24.14.1
 Summary: A library for generating and publishing Swagger specifications for Flask applications.
 Home-page: https://github.com/krlsedu/flask-swagger-generator.git
 Author: Carlos Eduardo
 License: MIT
-Description: # Flask Swagger Generator
-        Flask swagger generator is a library to create Swagger Open API definitions 
-        for Flask based applications. Swagger is an Interface Description Language for describing REST 
-        APIs expressed using JSON and YAML. 
-        
-        ## Installing 
-        Install and update using pip:
-        
-        ```
-        pip install flask-swagger-init
-        ```
-        
-        ## Documentation and Examples
-        COMING SOON
-        
-        ## A Simple Example
-        
-        ```python
-        
-        from flask import Flask
-        from flask_swagger_generator.generators.swagger_view import SwaggerView
-        
-        
-        # Create the flask app
-        app = Flask(__name__)
-        ...
-        # Create all the routes for the app
-        ...
-        
-        # Note: The swagger view must be created after all the routes have been created
-        # Create and publish the swagger view
-        SwaggerView.init(app=app, 
-                         application_version='1.0.0', 
-                         application_name='My API', 
-                         application_description='My API description')
-        ```
-        
-        ## License
-        This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
-        
-        ## Based on
-        This application is based on the [flask-swagger-generator](https://github.com/coding-kitties/flask-swagger-generator) project by [Coding Kitties](https://github.com/coding-kitties).
-        
 Keywords: Flask,swagger,swagger generator,OpenAPI
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: flask~=3.0.0
+Requires-Dist: marshmallow>=3.0.0
+Requires-Dist: setuptools>=65.5.1
+Requires-Dist: flask_swagger_ui>=3.25.0
+
+# Flask Swagger Generator
+Flask swagger generator is a library to create Swagger Open API definitions 
+for Flask based applications. Swagger is an Interface Description Language for describing REST 
+APIs expressed using JSON and YAML. 
+
+## Installing 
+Install and update using pip:
+
+```
+pip install flask-swagger-init
+```
+
+## Documentation and Examples
+COMING SOON
+
+## A Simple Example
+
+```python
+
+from flask import Flask
+from flask_swagger_generator.generators.swagger_view import SwaggerView
+
+
+# Create the flask app
+app = Flask(__name__)
+...
+# Create all the routes for the app
+...
+
+# Note: The swagger view must be created after all the routes have been created
+# Create and publish the swagger view
+SwaggerView.init(app=app, 
+                 application_version='1.0.0', 
+                 application_name='My API', 
+                 application_description='My API description')
+```
+
+## License
+This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
+
+## Based on
+This application is based on the [flask-swagger-generator](https://github.com/coding-kitties/flask-swagger-generator) project by [Coding Kitties](https://github.com/coding-kitties).
```

### Comparing `flask-swagger-init-23.52.4/flask_swagger_init.egg-info/SOURCES.txt` & `flask-swagger-init-24.14.1/flask_swagger_init.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS.md
+LICENSE
 README.md
 setup.cfg
 setup.py
 flask_swagger_generator/__init__.py
 flask_swagger_generator/exceptions.py
 flask_swagger_generator/components/__init__.py
 flask_swagger_generator/components/swagger_models.py
```

### Comparing `flask-swagger-init-23.52.4/setup.py` & `flask-swagger-init-24.14.1/setup.py`

 * *Files identical despite different names*


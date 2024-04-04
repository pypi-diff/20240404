# Comparing `tmp/glassflow-1.0.0.tar.gz` & `tmp/glassflow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassflow-1.0.0.tar", last modified: Thu Mar 21 18:54:41 2024, max compression
+gzip compressed data, was "glassflow-1.0.1.tar", last modified: Thu Apr  4 12:09:16 2024, max compression
```

## Comparing `glassflow-1.0.0.tar` & `glassflow-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.366208 glassflow-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-21 18:54:32.000000 glassflow-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-21 18:54:41.366208 glassflow-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-21 18:54:32.000000 glassflow-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-21 18:54:32.000000 glassflow-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 18:54:41.366208 glassflow-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-21 18:54:32.000000 glassflow-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.358208 glassflow-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.362208 glassflow-1.0.0/src/glassflow/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.362208 glassflow-1.0.0/src/glassflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.366208 glassflow-1.0.0/src/glassflow/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/errors/clienterror.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/errors/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.366208 glassflow-1.0.0/src/glassflow/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/operations/consumeevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/models/operations/publishevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.366208 glassflow-1.0.0/src/glassflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-03-21 18:54:32.000000 glassflow-1.0.0/src/glassflow/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:54:41.366208 glassflow-1.0.0/src/glassflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-21 18:54:41.000000 glassflow-1.0.0/src/glassflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-21 18:54:41.000000 glassflow-1.0.0/src/glassflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 18:54:41.000000 glassflow-1.0.0/src/glassflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-21 18:54:41.000000 glassflow-1.0.0/src/glassflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 18:54:41.000000 glassflow-1.0.0/src/glassflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 12:09:09.000000 glassflow-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-04 12:09:16.509062 glassflow-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-04 12:09:09.000000 glassflow-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 12:09:09.000000 glassflow-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:09:16.509062 glassflow-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 12:09:09.000000 glassflow-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.501062 glassflow-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/clienterror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/consumeevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/consumefailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/publishevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/src/glassflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/src/glassflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/top_level.txt
```

### Comparing `glassflow-1.0.0/LICENSE.md` & `glassflow-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/setup.py` & `glassflow-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,21 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="glassflow",
-    version="1.0.0",
+    version="1.0.1",
     author="glassflow",
     description="GlassFlow Python Client SDK",
+    url="https://learn.glassflow.dev/docs",
+    project_urls={
+        'Source': 'https://github.com/glassflow/glassflow-python-sdk',
+    },
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "urllib3==1.26.15", "certifi>=2023.7.22", "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4", "idna>=3.4", "jsonpath-python>=1.0.6 ",
         "marshmallow>=3.19.0", "mypy-extensions>=1.0.0", "packaging>=23.1",
```

### Comparing `glassflow-1.0.0/src/glassflow/client.py` & `glassflow-1.0.1/src/glassflow/client.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/config.py` & `glassflow-1.0.1/src/glassflow/config.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/models/errors/clienterror.py` & `glassflow-1.0.1/src/glassflow/models/errors/clienterror.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/models/errors/error.py` & `glassflow-1.0.1/src/glassflow/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/models/operations/consumeevent.py` & `glassflow-1.0.1/src/glassflow/models/operations/consumeevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/models/operations/publishevent.py` & `glassflow-1.0.1/src/glassflow/models/operations/publishevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow/pipelines.py` & `glassflow-1.0.1/src/glassflow/pipelines.py`

 * *Files 15% similar despite different names*

```diff
@@ -169,7 +169,82 @@
                     http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.ClientError('API error occurred',
                                      http_res.status_code, http_res.text,
                                      http_res)
 
         return res
+
+    def consume_failed(
+            self,
+            pipeline_access_token: str) -> operations.ConsumeFailedResponse:
+        """Consume the failed message from the pipeline
+
+        Args:
+            pipeline_access_token: The access token to access the pipeline
+
+        Returns:
+            ConsumeFailedResponse: Response object containing the status code and the raw response
+
+        Raises:
+            ClientError: If an error occurred while consuming the event
+
+        """
+        request = operations.ConsumeFailedRequest(
+            space_id=self.space_id,
+            pipeline_id=self.pipeline_id,
+            organization_id=self.organization_id,
+            x_pipeline_access_token=pipeline_access_token,
+        )
+
+        base_url = self.glassflow_client.glassflow_config.server_url
+
+        url = utils.generate_url(
+            operations.ConsumeFailedRequest, base_url,
+            '/pipelines/{pipeline_id}/topics/failed/events/consume', request)
+        headers = utils.get_headers(request)
+        query_params = utils.get_query_params(operations.ConsumeFailedRequest,
+                                              request)
+        headers['Accept'] = 'application/json'
+        headers[
+            'user-agent'] = self.glassflow_client.glassflow_config.user_agent
+        client = self.glassflow_client.glassflow_config.client
+        http_res = client.request('POST',
+                                  url,
+                                  params=query_params,
+                                  headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.ConsumeFailedResponse(
+            status_code=http_res.status_code,
+            content_type=content_type,
+            raw_response=http_res)
+
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                body = utils.unmarshal_json(
+                    http_res.text,
+                    Optional[operations.ConsumeFailedResponseBody])
+                res.body = body
+            else:
+                raise errors.ClientError(
+                    f'unknown content-type received: {content_type}',
+                    http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 204:
+            # No messages to be consumed. Return an empty response body
+            body = operations.ConsumeFailedResponseBody("", "", {})
+            res.body = body
+        elif http_res.status_code in [400, 500]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, errors.Error)
+                out.raw_response = http_res
+                raise out
+            else:
+                raise errors.ClientError(
+                    f'unknown content-type received: {content_type}',
+                    http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 401 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.ClientError('API error occurred',
+                                     http_res.status_code, http_res.text,
+                                     http_res)
+
+        return res
```

### Comparing `glassflow-1.0.0/src/glassflow/utils/utils.py` & `glassflow-1.0.1/src/glassflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.0/src/glassflow.egg-info/SOURCES.txt` & `glassflow-1.0.1/src/glassflow.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 src/glassflow.egg-info/top_level.txt
 src/glassflow/models/__init__.py
 src/glassflow/models/errors/__init__.py
 src/glassflow/models/errors/clienterror.py
 src/glassflow/models/errors/error.py
 src/glassflow/models/operations/__init__.py
 src/glassflow/models/operations/consumeevent.py
+src/glassflow/models/operations/consumefailed.py
 src/glassflow/models/operations/publishevent.py
 src/glassflow/utils/__init__.py
 src/glassflow/utils/utils.py
```


# Comparing `tmp/shadowdragon-0.0.4.tar.gz` & `tmp/shadowdragon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowdragon-0.0.4.tar", last modified: Thu Apr  4 21:35:32 2024, max compression
+gzip compressed data, was "shadowdragon-0.0.5.tar", last modified: Thu Apr  4 21:37:09 2024, max compression
```

## Comparing `shadowdragon-0.0.4.tar` & `shadowdragon-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:35:32.102326 shadowdragon-0.0.4/
--rw-r--r--   0 kojinglick   (501) staff       (20)     1067 2024-04-03 19:25:27.000000 shadowdragon-0.0.4/LICENSE
--rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-04 21:35:32.101894 shadowdragon-0.0.4/PKG-INFO
--rw-r--r--   0 kojinglick   (501) staff       (20)       49 2024-03-28 16:44:23.000000 shadowdragon-0.0.4/README.md
--rw-r--r--   0 kojinglick   (501) staff       (20)      518 2024-04-04 21:35:23.000000 shadowdragon-0.0.4/pyproject.toml
--rw-r--r--   0 kojinglick   (501) staff       (20)       38 2024-04-04 21:35:32.102420 shadowdragon-0.0.4/setup.cfg
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:35:32.093601 shadowdragon-0.0.4/src/
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:35:32.098231 shadowdragon-0.0.4/src/shadowdragon/
--rw-r--r--   0 kojinglick   (501) staff       (20)       61 2024-04-03 22:23:34.000000 shadowdragon-0.0.4/src/shadowdragon/__init__.py
--rw-r--r--   0 kojinglick   (501) staff       (20)     4328 2024-03-21 18:56:17.000000 shadowdragon-0.0.4/src/shadowdragon/archive.py
--rw-r--r--   0 kojinglick   (501) staff       (20)    23864 2024-04-04 21:35:08.000000 shadowdragon-0.0.4/src/shadowdragon/shadowdragon.py
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:35:32.101357 shadowdragon-0.0.4/src/shadowdragon.egg-info/
--rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-04 21:35:32.000000 shadowdragon-0.0.4/src/shadowdragon.egg-info/PKG-INFO
--rw-r--r--   0 kojinglick   (501) staff       (20)      282 2024-04-04 21:35:32.000000 shadowdragon-0.0.4/src/shadowdragon.egg-info/SOURCES.txt
--rw-r--r--   0 kojinglick   (501) staff       (20)        1 2024-04-04 21:35:32.000000 shadowdragon-0.0.4/src/shadowdragon.egg-info/dependency_links.txt
--rw-r--r--   0 kojinglick   (501) staff       (20)       13 2024-04-04 21:35:32.000000 shadowdragon-0.0.4/src/shadowdragon.egg-info/top_level.txt
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:37:09.588146 shadowdragon-0.0.5/
+-rw-r--r--   0 kojinglick   (501) staff       (20)     1067 2024-04-03 19:25:27.000000 shadowdragon-0.0.5/LICENSE
+-rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-04 21:37:09.587452 shadowdragon-0.0.5/PKG-INFO
+-rw-r--r--   0 kojinglick   (501) staff       (20)       49 2024-03-28 16:44:23.000000 shadowdragon-0.0.5/README.md
+-rw-r--r--   0 kojinglick   (501) staff       (20)      518 2024-04-04 21:36:59.000000 shadowdragon-0.0.5/pyproject.toml
+-rw-r--r--   0 kojinglick   (501) staff       (20)       38 2024-04-04 21:37:09.588292 shadowdragon-0.0.5/setup.cfg
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:37:09.579784 shadowdragon-0.0.5/src/
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:37:09.584157 shadowdragon-0.0.5/src/shadowdragon/
+-rw-r--r--   0 kojinglick   (501) staff       (20)       61 2024-04-03 22:23:34.000000 shadowdragon-0.0.5/src/shadowdragon/__init__.py
+-rw-r--r--   0 kojinglick   (501) staff       (20)     4328 2024-03-21 18:56:17.000000 shadowdragon-0.0.5/src/shadowdragon/archive.py
+-rw-r--r--   0 kojinglick   (501) staff       (20)    23865 2024-04-04 21:36:56.000000 shadowdragon-0.0.5/src/shadowdragon/shadowdragon.py
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-04 21:37:09.586874 shadowdragon-0.0.5/src/shadowdragon.egg-info/
+-rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-04 21:37:09.000000 shadowdragon-0.0.5/src/shadowdragon.egg-info/PKG-INFO
+-rw-r--r--   0 kojinglick   (501) staff       (20)      282 2024-04-04 21:37:09.000000 shadowdragon-0.0.5/src/shadowdragon.egg-info/SOURCES.txt
+-rw-r--r--   0 kojinglick   (501) staff       (20)        1 2024-04-04 21:37:09.000000 shadowdragon-0.0.5/src/shadowdragon.egg-info/dependency_links.txt
+-rw-r--r--   0 kojinglick   (501) staff       (20)       13 2024-04-04 21:37:09.000000 shadowdragon-0.0.5/src/shadowdragon.egg-info/top_level.txt
```

### Comparing `shadowdragon-0.0.4/LICENSE` & `shadowdragon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.4/PKG-INFO` & `shadowdragon-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.4
+Version: 0.0.5
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shadowdragon-0.0.4/pyproject.toml` & `shadowdragon-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shadowdragon"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Kojin Glick", email="kglick@middlebury.edu" },
 ]
 description = "An async wrapper for the ShadowDragon API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `shadowdragon-0.0.4/src/shadowdragon/archive.py` & `shadowdragon-0.0.5/src/shadowdragon/archive.py`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.4/src/shadowdragon/shadowdragon.py` & `shadowdragon-0.0.5/src/shadowdragon/shadowdragon.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,15 +524,15 @@
                     "limit": response.headers.get("X-Ratelimit-Limit"),
                     "remaining": response.headers.get("X-Ratelimit-Remaining"),
                     "reset_in": response.headers.get("X-Ratelimit-Reset")
                 }
                 return json
             
     @log_request
-    async def facebook_user_friends(self, user_id: str, limit: Union[int, None] = 1000, queue: Union[bool, None] = False) -> list[dict[str, Any]]:
+    async def facebook_posts_by_user(self, user_id: str, limit: Union[int, None] = 1000, queue: Union[bool, None] = False) -> list[dict[str, Any]]:
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=1200)) as session:
             url = f"{self.base_url}/users/{user_id}/posts_by"
 
             if limit:
                 url += f"?limit={limit}"
             if queue:
                 url += f"&queue={queue}"
```

### Comparing `shadowdragon-0.0.4/src/shadowdragon.egg-info/PKG-INFO` & `shadowdragon-0.0.5/src/shadowdragon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.4
+Version: 0.0.5
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


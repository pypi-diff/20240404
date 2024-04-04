# Comparing `tmp/stcog-0.0.5.tar.gz` & `tmp/stcog-0.0.6.tar.gz`

## Comparing `stcog-0.0.5.tar` & `stcog-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.5/src/stcog/__init__.py
--rw-r--r--   0        0        0    24906 2020-02-02 00:00:00.000000 stcog-0.0.5/src/stcog/auth.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.5/src/stcog/exceptions.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.5/src/stcog/session_provider.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.5/src/stcog/utils.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.5/tests/example.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.5/tests/example_hosted.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.5/LICENSE
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.5/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/__init__.py
+-rw-r--r--   0        0        0    24906 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/auth.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/exceptions.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/session_provider.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/utils.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.6/tests/example.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.6/tests/example_hosted.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.6/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.6/PKG-INFO
```

### Comparing `stcog-0.0.5/src/stcog/auth.py` & `stcog-0.0.6/src/stcog/auth.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         Returns None if no credentials were found."""
         try:
         
             try:
                 auth_id_token
             except NameError:
                 print("well, auth_id_token WASN'T defined after all!")
+                auth_id_token = ""
             else:
                 print("sure, auth_id_token was defined.")
-                auth_id_token = ""
     
             return Credentials(
                 id_token=st.session_state["auth_id_token"],
                 access_token=st.session_state["auth_access_token"],
                 refresh_token=st.session_state["auth_refresh_token"],
                 expires_in=st.session_state["auth_expires_in"],
                 token_type=st.session_state["auth_token_type"],
```

### Comparing `stcog-0.0.5/src/stcog/session_provider.py` & `stcog-0.0.6/src/stcog/session_provider.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/src/stcog/utils.py` & `stcog-0.0.6/src/stcog/utils.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/tests/example.py` & `stcog-0.0.6/tests/example.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/tests/example_hosted.py` & `stcog-0.0.6/tests/example_hosted.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/LICENSE` & `stcog-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/README.md` & `stcog-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `stcog-0.0.5/pyproject.toml` & `stcog-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stcog"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Pastoris Zumba", email="fcuy047@gmail.com" },
 ]
 description = "A package for streamlit and aws auth link"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stcog-0.0.5/PKG-INFO` & `stcog-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stcog
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for streamlit and aws auth link
 Project-URL: Homepage, https://github.com/pop-srw/streamlit-cognito-auth/
 Project-URL: Issues, https://github.com/pop-srw/streamlit-cognito-auth/issues
 Author-email: Pastoris Zumba <fcuy047@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

# Comparing `tmp/stcog-0.0.2.tar.gz` & `tmp/stcog-0.0.3.tar.gz`

## Comparing `stcog-0.0.2.tar` & `stcog-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/__init__.py
--rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/auth.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/exceptions.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/session_provider.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/utils.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.2/tests/example.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.2/tests/example_hosted.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.2/LICENSE
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.2/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.3/src/stcog/__init__.py
+-rw-r--r--   0        0        0    24633 2020-02-02 00:00:00.000000 stcog-0.0.3/src/stcog/auth.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.3/src/stcog/exceptions.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.3/src/stcog/session_provider.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.3/src/stcog/utils.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.3/tests/example.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.3/tests/example_hosted.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.3/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.3/PKG-INFO
```

### Comparing `stcog-0.0.2/src/stcog/auth.py` & `stcog-0.0.3/src/stcog/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         """Clears the password reset session from streamlit session state/"""
         st.session_state["auth_reset_password_session"] = ""
         st.session_state["auth_reset_password_username"] = ""
         st.session_state["auth_reset_password_password"] = ""
 
     def is_reset_password_session(self) -> bool:
         """Returns if password reset session is set in streamlit session state."""
+        st.session_state["auth_reset_password_session"] = ""
         return bool(st.session_state["auth_reset_password_session"])
 
     def reset_password_credentials(self) -> Tuple[Optional[str], Optional[str]]:
         """Returns the password reset username and password saved in streamlit session state."""
         username = st.session_state["auth_reset_password_username"] or None
         password = st.session_state["auth_reset_password_password"] or None
         return (username, password)
```

### Comparing `stcog-0.0.2/src/stcog/session_provider.py` & `stcog-0.0.3/src/stcog/session_provider.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/src/stcog/utils.py` & `stcog-0.0.3/src/stcog/utils.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/tests/example.py` & `stcog-0.0.3/tests/example.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/tests/example_hosted.py` & `stcog-0.0.3/tests/example_hosted.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/LICENSE` & `stcog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/README.md` & `stcog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stcog-0.0.2/pyproject.toml` & `stcog-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stcog"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Pastoris Zumba", email="fcuy047@gmail.com" },
 ]
 description = "A package for streamlit and aws auth link"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stcog-0.0.2/PKG-INFO` & `stcog-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stcog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for streamlit and aws auth link
 Project-URL: Homepage, https://github.com/pop-srw/streamlit-cognito-auth/
 Project-URL: Issues, https://github.com/pop-srw/streamlit-cognito-auth/issues
 Author-email: Pastoris Zumba <fcuy047@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


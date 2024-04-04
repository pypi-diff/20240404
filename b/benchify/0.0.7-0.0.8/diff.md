# Comparing `tmp/benchify-0.0.7.tar.gz` & `tmp/benchify-0.0.8.tar.gz`

## Comparing `benchify-0.0.7.tar` & `benchify-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 benchify-0.0.7/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.7/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.7/src/benchify/__init__.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 benchify-0.0.7/src/benchify/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 benchify-0.0.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 benchify-0.0.7/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 benchify-0.0.7/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 benchify-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 benchify-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 benchify-0.0.8/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.8/src/benchify/__init__.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 benchify-0.0.8/src/benchify/main.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 benchify-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 benchify-0.0.8/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 benchify-0.0.8/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 benchify-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 benchify-0.0.8/PKG-INFO
```

### Comparing `benchify-0.0.7/src/benchify/main.py` & `benchify-0.0.8/src/benchify/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,21 @@
     sv = AsymmetricSignatureVerifier(jwks_url)
     tv = TokenVerifier(
         signature_verifier=sv, 
         issuer=issuer, 
         audience=AUTH0_CLIENT_ID)
     tv.verify(id_token)
 
+class AuthTokens:
+    id_token: str = ""
+    access_token: str = ""
+    def __init__(self, id_token, access_token):
+        self.id_token = id_token
+        self.access_token = access_token
+
 def login():
     """
     Runs the device authorization flow and stores the user object in memory
     """
     device_code_payload = {
         'client_id': AUTH0_CLIENT_ID,
         'scope': 'openid profile'
@@ -92,14 +99,18 @@
             # Save the current_user.
 
         elif token_data['error'] not in ('authorization_pending', 'slow_down'):
             print(token_data['error_description'])
             raise typer.Exit(code=1)
         else:
             time.sleep(device_code_data['interval'])
+    return AuthTokens(
+        id_token=token_data['id_token'],
+        access_token=token_data['access_token']
+    )
 
 @app.command()
 def authenticate():
     if current_user is None:
         login()
     print("✅ Logged in " + str(current_user))
 
@@ -119,15 +130,15 @@
     if len(sys.argv) == 1:
         print("⬇️ Please specify the file to be analyzed.")
         return
 
     file = sys.argv[1]
     
     if current_user is None:
-        login()
+        auth_tokens = login()
         print(f"Welcome {current_user['name']}!")
     function_str = None
     
     try:
         print("Scanning " + file + " ...")
         with open(file, "r") as fr:
             function_str = fr.read()
@@ -154,15 +165,16 @@
         return
     if function_str == None:
         print(f"Error attempting to read {file}." + \
             " Cannot continue 😢.")
         return
     
     console = Console()
-    url = "https://api.benchify.cloud/analyze"
-    params = {'test_func': function_str} # TODO
+    url = "https://benchify.cloud/analyze"
+    params = {'test_func': function_str}
+    headers = {'Authorization': f'Bearer {auth_tokens.id_token}'}
     print("Analyzing.  Should take about 1 minute ...")
-    response = requests.get(url, params=params)
+    response = requests.get(url, params=params, headers=headers)
     console.print(response.text)
 
 if __name__ == "__main__":
     app()
```

### Comparing `benchify-0.0.7/LICENSE` & `benchify-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `benchify-0.0.7/pyproject.toml` & `benchify-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "benchify"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Max von Hippel", email="max@benchify.ai" },
   { name="Juan Castaño", email="juan@benchify.ai" },
+  { name="Tyler Gabb", email="tylerjgabb@gmail.com" },
 ]
 description = "Formal code intelligence"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `benchify-0.0.7/PKG-INFO` & `benchify-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: benchify
-Version: 0.0.7
+Version: 0.0.8
 Summary: Formal code intelligence
 Project-URL: Homepage, https://github.com/Benchify/benchify-api
 Project-URL: Issues, https://github.com/Benchify/benchify-api/issues
-Author-email: Max von Hippel <max@benchify.ai>, Juan Castaño <juan@benchify.ai>
+Author-email: Max von Hippel <max@benchify.ai>, Juan Castaño <juan@benchify.ai>, Tyler Gabb <tylerjgabb@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: auth0-python
 Requires-Dist: requests
```


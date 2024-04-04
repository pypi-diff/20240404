# Comparing `tmp/rciam-federation-registry-agent-3.3.2.tar.gz` & `tmp/rciam-federation-registry-agent-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rciam-federation-registry-agent-3.3.2.tar", last modified: Sat Dec  9 00:31:26 2023, max compression
+gzip compressed data, was "dist/rciam-federation-registry-agent-3.3.3.tar", last modified: Thu Apr  4 07:33:31 2024, max compression
```

## Comparing `rciam-federation-registry-agent-3.3.2.tar` & `rciam-federation-registry-agent-3.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.562924 rciam-federation-registry-agent-3.3.2/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.555924 rciam-federation-registry-agent-3.3.2/Keycloak/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11983 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/Keycloak/KeycloakClientApi.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/Keycloak/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11340 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/LICENSE
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.556924 rciam-federation-registry-agent-3.3.2/MitreidConnect/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7366 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/MitreidConnect/MitreidClientApi.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/MitreidConnect/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6178 2023-12-09 00:31:26.562924 rciam-federation-registry-agent-3.3.2/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5202 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.556924 rciam-federation-registry-agent-3.3.2/ServiceRegistryAms/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2400 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/ServiceRegistryAms/PullPublish.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/ServiceRegistryAms/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.557924 rciam-federation-registry-agent-3.3.2/Utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/Utils/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1493 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/Utils/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1531 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/Utils/oauth.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.558924 rciam-federation-registry-agent-3.3.2/bin/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19324 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/bin/deployer_keycloak
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7011 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/bin/deployer_mitreid
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6467 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/bin/deployer_ssp
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       30 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/pyproject.toml
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.561924 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6178 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      774 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      166 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       55 2023-12-09 00:31:26.000000 rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      154 2023-12-09 00:31:26.562924 rciam-federation-registry-agent-3.3.2/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1494 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/setup.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:31:26.561924 rciam-federation-registry-agent-3.3.2/tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25028 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/tests/test_deployer_keycloak.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6434 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/tests/test_deployer_mitreid.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7253 2023-12-09 00:30:15.000000 rciam-federation-registry-agent-3.3.2/tests/test_deployer_ssp.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.077987 rciam-federation-registry-agent-3.3.3/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.071987 rciam-federation-registry-agent-3.3.3/Keycloak/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11983 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/Keycloak/KeycloakClientApi.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/Keycloak/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11340 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/LICENSE
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.071987 rciam-federation-registry-agent-3.3.3/MitreidConnect/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7366 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/MitreidConnect/MitreidClientApi.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/MitreidConnect/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6178 2024-04-04 07:33:31.077987 rciam-federation-registry-agent-3.3.3/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5202 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.072986 rciam-federation-registry-agent-3.3.3/ServiceRegistryAms/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2400 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/ServiceRegistryAms/PullPublish.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/ServiceRegistryAms/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.072986 rciam-federation-registry-agent-3.3.3/Utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/Utils/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1493 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/Utils/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1531 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/Utils/oauth.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.073987 rciam-federation-registry-agent-3.3.3/bin/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19093 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/bin/deployer_keycloak
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7011 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/bin/deployer_mitreid
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6467 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/bin/deployer_ssp
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       30 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/pyproject.toml
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.076987 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6178 2024-04-04 07:33:30.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      774 2024-04-04 07:33:31.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-04-04 07:33:30.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-04-04 07:33:30.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      166 2024-04-04 07:33:30.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       55 2024-04-04 07:33:30.000000 rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      154 2024-04-04 07:33:31.078987 rciam-federation-registry-agent-3.3.3/setup.cfg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1494 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:33:31.076987 rciam-federation-registry-agent-3.3.3/tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25028 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/tests/test_deployer_keycloak.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6434 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/tests/test_deployer_mitreid.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     7253 2024-04-04 07:32:19.000000 rciam-federation-registry-agent-3.3.3/tests/test_deployer_ssp.py
```

### Comparing `rciam-federation-registry-agent-3.3.2/Keycloak/KeycloakClientApi.py` & `rciam-federation-registry-agent-3.3.3/Keycloak/KeycloakClientApi.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/LICENSE` & `rciam-federation-registry-agent-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/MitreidConnect/MitreidClientApi.py` & `rciam-federation-registry-agent-3.3.3/MitreidConnect/MitreidClientApi.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/PKG-INFO` & `rciam-federation-registry-agent-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rciam-federation-registry-agent
-Version: 3.3.2
+Version: 3.3.3
 Summary: A library that connects to ams using argo-ams-library and syncs with MITREid, SimpleSAMLphp and Keycloak
 Home-page: https://github.com/rciam/rciam-federation-registry-agent
 Author: grnet
 Author-email: faai@grnet.gr
 License: ASL 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: PHP
```

### Comparing `rciam-federation-registry-agent-3.3.2/README.md` & `rciam-federation-registry-agent-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/ServiceRegistryAms/PullPublish.py` & `rciam-federation-registry-agent-3.3.3/ServiceRegistryAms/PullPublish.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/Utils/common.py` & `rciam-federation-registry-agent-3.3.3/Utils/common.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/Utils/oauth.py` & `rciam-federation-registry-agent-3.3.3/Utils/oauth.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/bin/deployer_keycloak` & `rciam-federation-registry-agent-3.3.3/bin/deployer_keycloak`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             if "jwks" in msg:
                 new_msg["attributes"]["use.jwks.string"] = "true"
                 new_msg["attributes"]["jwks.string"] = json.dumps(msg.pop("jwks"))
             if "jwks_uri" in msg:
                 new_msg["attributes"]["use.jwks.url"] = True
                 new_msg["attributes"]["jwks.url"] = msg.pop("jwks_uri")
             if "refresh_token_validity_seconds" in msg:
-                new_msg["attributes"]["client.offline.session.idle.timeout"] = str(
+                new_msg["attributes"]["client.offline.session.max.lifespan"] = str(
                     msg["refresh_token_validity_seconds"]
                 )
                 if "reuse_refresh_token" in msg:
                     rotate_refresh_token = str(not msg.pop("reuse_refresh_token"))
                     new_msg["attributes"]["revoke.refresh.token"] = rotate_refresh_token.lower()
             if "code_challenge_method" in msg:
                 new_msg["attributes"]["pkce.code.challenge.method"] = msg.pop("code_challenge_method")
@@ -97,19 +97,14 @@
                     new_msg["attributes"]["access.token.lifespan"] = "60"
                 else:
                     new_msg["attributes"]["access.token.lifespan"] = str(msg.pop("access_token_validity_seconds"))
             if "id_token_timeout_seconds" in msg:
                 new_msg["attributes"]["id.token.lifespan"] = str(msg.pop("id_token_timeout_seconds"))
             if "device_code_validity_seconds" in msg:
                 new_msg["attributes"]["oauth2.device.code.lifespan"] = str(msg.pop("device_code_validity_seconds"))
-            if (
-                new_msg["standardFlowEnabled"] == True
-                or new_msg["attributes"]["oauth2.device.authorization.grant.enabled"] == True
-            ):
-                new_msg["consentRequired"] = True
         # Options for SAML clients
         elif msg["protocol"] == "saml":
             new_msg = json.loads(jsonSamlTemplate)
             new_msg["protocol"] = msg.pop("protocol")
             if "saml_consent" in keycloak_config:
                 new_msg["consentRequired"] = keycloak_config["saml_consent"]
             else:
```

### Comparing `rciam-federation-registry-agent-3.3.2/bin/deployer_mitreid` & `rciam-federation-registry-agent-3.3.3/bin/deployer_mitreid`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/bin/deployer_ssp` & `rciam-federation-registry-agent-3.3.3/bin/deployer_ssp`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/PKG-INFO` & `rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rciam-federation-registry-agent
-Version: 3.3.2
+Version: 3.3.3
 Summary: A library that connects to ams using argo-ams-library and syncs with MITREid, SimpleSAMLphp and Keycloak
 Home-page: https://github.com/rciam/rciam-federation-registry-agent
 Author: grnet
 Author-email: faai@grnet.gr
 License: ASL 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: PHP
```

### Comparing `rciam-federation-registry-agent-3.3.2/rciam_federation_registry_agent.egg-info/SOURCES.txt` & `rciam-federation-registry-agent-3.3.3/rciam_federation_registry_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/setup.py` & `rciam-federation-registry-agent-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 install_requires = [x.strip() for x in all_reqs if "git+" not in x]
 dependency_links = [x.strip().replace("git+", "") for x in all_reqs if x.startswith("git+")]
 
 setup(
     name="rciam-federation-registry-agent",
     author="grnet",
     author_email="faai@grnet.gr",
-    version="3.3.2",
+    version="3.3.3",
     license="ASL 2.0",
     url="https://github.com/rciam/rciam-federation-registry-agent",
     packages=find_packages(),
     scripts=["bin/deployer_ssp", "bin/deployer_mitreid", "bin/deployer_keycloak"],
     zip_safe=False,
     install_requires=install_requires,
     dependency_links=dependency_links,
```

### Comparing `rciam-federation-registry-agent-3.3.2/tests/test_deployer_keycloak.py` & `rciam-federation-registry-agent-3.3.3/tests/test_deployer_keycloak.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/tests/test_deployer_mitreid.py` & `rciam-federation-registry-agent-3.3.3/tests/test_deployer_mitreid.py`

 * *Files identical despite different names*

### Comparing `rciam-federation-registry-agent-3.3.2/tests/test_deployer_ssp.py` & `rciam-federation-registry-agent-3.3.3/tests/test_deployer_ssp.py`

 * *Files identical despite different names*


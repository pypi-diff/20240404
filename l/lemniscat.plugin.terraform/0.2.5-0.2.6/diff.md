# Comparing `tmp/lemniscat.plugin.terraform-0.2.5.tar.gz` & `tmp/lemniscat.plugin.terraform-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemniscat.plugin.terraform-0.2.5.tar", last modified: Mon Mar 25 17:14:47 2024, max compression
+gzip compressed data, was "lemniscat.plugin.terraform-0.2.6.tar", last modified: Thu Apr  4 15:07:18 2024, max compression
```

## Comparing `lemniscat.plugin.terraform-0.2.5.tar` & `lemniscat.plugin.terraform-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.232673 lemniscat.plugin.terraform-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-25 17:14:47.232673 lemniscat.plugin.terraform-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-25 17:14:35.000000 lemniscat.plugin.terraform-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 17:14:47.232673 lemniscat.plugin.terraform-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.228673 lemniscat.plugin.terraform-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.228673 lemniscat.plugin.terraform-0.2.5/src/lemniscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.228673 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.232673 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/azurecli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 17:14:34.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-25 17:14:04.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/tfstate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:14:47.232673 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-25 17:14:47.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-25 17:14:47.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 17:14:47.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 17:14:47.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-25 17:14:47.000000 lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-04 15:07:14.000000 lemniscat.plugin.terraform-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.078197 lemniscat.plugin.terraform-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/src/lemniscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/azurecli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 15:07:13.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-04 15:07:08.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/tfstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:07:18.082197 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-04 15:07:18.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-04 15:07:18.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:07:18.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:07:18.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 15:07:18.000000 lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/top_level.txt
```

### Comparing `lemniscat.plugin.terraform-0.2.5/LICENSE` & `lemniscat.plugin.terraform-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lemniscat.plugin.terraform-0.2.5/PKG-INFO` & `lemniscat.plugin.terraform-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemniscat.plugin.terraform
-Version: 0.2.5
+Version: 0.2.6
 Summary: A runtime to provide product oriented in DevOps approach
 Author-email: Philippe MORISSEAU <philippe.morisseau@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lemniscat-devops/lemniscat.plugin.terraform
 Project-URL: Issues, https://github.com/lemniscat-devops/lemniscat.plugin.terraform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lemniscat.plugin.terraform-0.2.5/README.md` & `lemniscat.plugin.terraform-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lemniscat.plugin.terraform-0.2.5/pyproject.toml` & `lemniscat.plugin.terraform-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lemniscat.plugin.terraform"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Philippe MORISSEAU", email="philippe.morisseau@outlook.com" },
 ]
 description = "A runtime to provide product oriented in DevOps approach"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/azurecli.py` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/azurecli.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,8 +89,9 @@
         self.cmd(['pwsh', '-Command', f"az login --service-principal -u {os.environ['ARM_CLIENT_ID']} -p {os.environ['ARM_CLIENT_SECRET']} --tenant {os.environ['ARM_TENANT_ID']}"], capture_output=False)
         self.cmd(['pwsh', '-Command', f"az account set --subscription {os.environ['ARM_SUBSCRIPTION_ID']}"], capture_output=False)
         
     def run(self, storage_account_name):
         log.info('Logging to Azure...')
         self.append_loginCommand()
         log.info('Getting storage account key...')
+        self.cmd(['pwsh', '-Command', f"az configure --defaults group="], capture_output=False)
         return self.cmd(['pwsh', '-Command', f'$result = az storage account keys list -n {storage_account_name} --query "[0].value" -o tsv; Write-Host "[lemniscat.pushvar] arm_access_key=$result"'], capture_output=True)
```

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/main.py` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/main.py`

 * *Files identical despite different names*

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/terraform.py` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/terraform.py`

 * *Files identical despite different names*

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat/plugin/terraform/tfstate.py` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat/plugin/terraform/tfstate.py`

 * *Files identical despite different names*

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/PKG-INFO` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemniscat.plugin.terraform
-Version: 0.2.5
+Version: 0.2.6
 Summary: A runtime to provide product oriented in DevOps approach
 Author-email: Philippe MORISSEAU <philippe.morisseau@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lemniscat-devops/lemniscat.plugin.terraform
 Project-URL: Issues, https://github.com/lemniscat-devops/lemniscat.plugin.terraform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lemniscat.plugin.terraform-0.2.5/src/lemniscat.plugin.terraform.egg-info/SOURCES.txt` & `lemniscat.plugin.terraform-0.2.6/src/lemniscat.plugin.terraform.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/fortiedr-3.0.0.tar.gz` & `tmp/fortiedr-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.0.0.tar", last modified: Thu Mar 28 20:20:38 2024, max compression
+gzip compressed data, was "fortiedr-3.5.tar", last modified: Wed Apr  3 22:19:01 2024, max compression
```

## Comparing `fortiedr-3.0.0.tar` & `fortiedr-3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-03-28 20:20:38.151852 fortiedr-3.0.0/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-03-26 20:15:27.000000 fortiedr-3.0.0/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       25 2024-03-28 20:06:06.000000 fortiedr-3.0.0/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2689 2024-03-28 20:20:38.151852 fortiedr-3.0.0/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     2076 2024-03-28 20:15:09.000000 fortiedr-3.0.0/README.md
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-03-28 20:20:38.147852 fortiedr-3.0.0/fortiedr/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       31 2024-03-26 20:15:27.000000 fortiedr-3.0.0/fortiedr/__init__.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1528 2024-03-26 20:15:27.000000 fortiedr-3.0.0/fortiedr/auth.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4977 2024-03-26 20:15:27.000000 fortiedr-3.0.0/fortiedr/connector.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)   250522 2024-03-26 20:15:27.000000 fortiedr-3.0.0/fortiedr/fortiedr.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-03-28 20:20:38.151852 fortiedr-3.0.0/fortiedr.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2689 2024-03-28 20:20:38.000000 fortiedr-3.0.0/fortiedr.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      279 2024-03-28 20:20:38.000000 fortiedr-3.0.0/fortiedr.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-03-28 20:20:38.000000 fortiedr-3.0.0/fortiedr.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-03-28 20:20:38.000000 fortiedr-3.0.0/fortiedr.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      573 2024-03-28 20:20:06.000000 fortiedr-3.0.0/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-03-28 19:25:38.000000 fortiedr-3.0.0/requirements.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-03-28 20:20:38.155852 fortiedr-3.0.0/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      731 2024-03-28 20:20:00.000000 fortiedr-3.0.0/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.054580 fortiedr-3.5/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-03-26 20:15:27.000000 fortiedr-3.5/LICENSE
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       24 2024-04-03 22:14:23.000000 fortiedr-3.5/MANIFEST.in
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-03 22:19:01.054580 fortiedr-3.5/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-04-03 22:14:23.000000 fortiedr-3.5/README.md
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.050580 fortiedr-3.5/fortiedr/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/__init__.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/auth.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/connector.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)   236357 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/fortiedr.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.054580 fortiedr-3.5/fortiedr.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      279 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/top_level.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      571 2024-04-03 22:18:48.000000 fortiedr-3.5/pyproject.toml
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-03-28 19:25:38.000000 fortiedr-3.5/requirements.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-04-03 22:19:01.054580 fortiedr-3.5/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      878 2024-04-03 22:14:23.000000 fortiedr-3.5/setup.py
```

### Comparing `fortiedr-3.0.0/LICENSE` & `fortiedr-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.0.0/PKG-INFO` & `fortiedr-3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.0.0
+Version: 3.5
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Fortiedr Python module
-An Open-source python package intended to help on interacting with FortiEDR API.
+# FortiEDR Python module
+An open-source Python package intended to help interact with FortiEDR API.
 
 It was based and tested in FortiEDR Cloud version 6.2.0.0436.
 
-## How do I install FortiEDR Python module?
+See [changelog](CHANGELOG.md) for more.
+
+## How do I install the FortiEDR Python module?
 
 Be sure you have at least Python 3.8 and PIP (https://pypi.org/project/pip/) installed.
 
-After downloading this tool, use pip for installing dependencies using the following command:
+After downloading this tool, use pip to install dependencies using the following command:
 
 ```
 pip install fortiedr
 ```
 
-Or you can download directly from this repo:
+Or you can download it directly from this repo:
 
 ```
 git clone https://github.com/rafaelfoster/fortiedr.git
 
 cd fortiedr
 
 pip3 install .
 ```
 
 ## First steps with fortiedr
 
 First of all, create a Rest API user on FortiEDR Management console:
- * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/5.2.1/administration-guide/776468/users
+ * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/6.2.0/administration-guide/776468/users
 
  * After creating the user, this newly created user must log in to the Central Manager console and change their initial password before they can be used by Rest API calls.
 
 After creating a user with privileges for interacting with FortiEDR API, you can start using the package by importing the modules you want to your code:
 
 `import fortiedr`
 
@@ -77,10 +79,10 @@
 After credentials are defined and successfully authenticated, you are now able to start consuming FortiEDR API.
 
 The "example.py" file contains some examples of how to use the package.
 
 
 ## How to contribute, provide feedback, or report bugs?
 
-You can e-mail me at fosterr at fortinet (.) com.
+You can e-mail me at rafaelgfoster at gmail (.) com.
 
 Enjoy it!
```

### Comparing `fortiedr-3.0.0/README.md` & `fortiedr-3.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-# Fortiedr Python module
-An Open-source python package intended to help on interacting with FortiEDR API.
+# FortiEDR Python module
+An open-source Python package intended to help interact with FortiEDR API.
 
 It was based and tested in FortiEDR Cloud version 6.2.0.0436.
 
-## How do I install FortiEDR Python module?
+See [changelog](CHANGELOG.md) for more.
+
+## How do I install the FortiEDR Python module?
 
 Be sure you have at least Python 3.8 and PIP (https://pypi.org/project/pip/) installed.
 
-After downloading this tool, use pip for installing dependencies using the following command:
+After downloading this tool, use pip to install dependencies using the following command:
 
 ```
 pip install fortiedr
 ```
 
-Or you can download directly from this repo:
+Or you can download it directly from this repo:
 
 ```
 git clone https://github.com/rafaelfoster/fortiedr.git
 
 cd fortiedr
 
 pip3 install .
 ```
 
 ## First steps with fortiedr
 
 First of all, create a Rest API user on FortiEDR Management console:
- * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/5.2.1/administration-guide/776468/users
+ * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/6.2.0/administration-guide/776468/users
 
  * After creating the user, this newly created user must log in to the Central Manager console and change their initial password before they can be used by Rest API calls.
 
 After creating a user with privileges for interacting with FortiEDR API, you can start using the package by importing the modules you want to your code:
 
 `import fortiedr`
 
@@ -62,10 +64,10 @@
 After credentials are defined and successfully authenticated, you are now able to start consuming FortiEDR API.
 
 The "example.py" file contains some examples of how to use the package.
 
 
 ## How to contribute, provide feedback, or report bugs?
 
-You can e-mail me at fosterr at fortinet (.) com.
+You can e-mail me at rafaelgfoster at gmail (.) com.
 
 Enjoy it!
```

### Comparing `fortiedr-3.0.0/fortiedr/auth.py` & `fortiedr-3.5/fortiedr/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+import json
 import base64
 import requests
 
 class Auth:
       
     @staticmethod
     def convert_to_base64(convert_string):
         string_bytes = convert_string.encode("ascii")
         b64_bytes = base64.b64encode(string_bytes)
         return b64_bytes.decode("ascii")
 
     @staticmethod
     def test_authentication(headers, host):
-        url = f'https://{host}/management-rest/admin/list-system-summary'
+        response_headers = None
+        url = f'https://{host}/management-rest/admin/ready'
 
         try:
             res = requests.get(url, headers=headers, verify=False)
             res_code = res.status_code
-
             status = False
             if res_code == 401:
                 data = "Unauthorized"
             elif res_code == 403:
                 data = "Forbidden"
             elif res_code == 404:
                 data = "Not Found"
             elif res_code == 500:
                 data = "Internal Server Error"
             else:
                 data = res
                 status = True
+                response_headers = res.headers
 
-            return status, data
+            return status, data, response_headers
 
         except requests.exceptions.RequestException as err:
             raise SystemExit(err) from err
 
     @staticmethod
     def get_headers(fedr_host, fedr_user, fedr_pass, fedr_org=None):
         if fedr_org:
             user_pass = f"{fedr_org}\\{fedr_user}:{fedr_pass}"
         else:
             user_pass = f"{fedr_user}:{fedr_pass}"
 
         auth_token = Auth.convert_to_base64(user_pass)
         headers = {"Authorization": f"Basic {auth_token}"}
-
-        status, data = Auth.test_authentication(headers, fedr_host)
-
+        status, data, res_headers = Auth.test_authentication(headers, fedr_host)
         return (headers, fedr_host) if status else (None, data)
```

### Comparing `fortiedr-3.0.0/fortiedr/fortiedr.py` & `fortiedr-3.5/fortiedr/fortiedr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,5110 +1,4969 @@
+
+import os
+import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
 fortiedr_connection = None
 
-class Admin:
-	'''Admin Rest Api Controller'''
-
-	def set_tray_notification_settings(self, organization: str, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None) -> tuple[bool, None]:
+class ApplicationControl:
+	'''Application Control Rest Api Controller'''
 
+	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: dict = None, tag: str = None) -> tuple[bool, None]:
 		'''
-		class Admin
-		Description: Update tray notification settings.
-
+		Class ApplicationControl
+		Description: Get application controls.
+        
 		Args:
-			adminSetTrayNotificationSettingsRequest: adminSetTrayNotificationSettingsRequest. 
-			enabledPopup: Enable popup. 
-			enabledTrayNotification: Enable tray notification. 
-			message: Specifies the message. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			fileName (str): Specifies the file name, if contains special characters - encode to HTML URL Encoding.
+			attributes.fileName (str): Specifies the file name, if contains special characters - encode to HTML URL Encoding.
+			path (str): Specifies the path, if contains special characters - encode to HTML URL Encoding.
+			attributes.path (str): Specifies the path, if contains special characters - encode to HTML URL Encoding.
+			signer (str): Specifies the value, if contains special characters - encode to HTML URL Encoding.
+			attributes.signer (str): Specifies the value, if contains special characters - encode to HTML URL Encoding.
+			currentPage (int): Specifies the current page.
+			enabled (bool): Specifies the state of the application control.
+			hash (str): Specifies the hash of the application control.
+			operatingSystem (str): Specifies the operating system of the application control.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyIds (dict): Specifies the IDs of the relevant policies for application control.
+			tag (str): Specifies the tag related to application control.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/api/admin/set-tray-notification-settings'
+		validate_params("get_applications", locals())
+
+		url = '/api/application-control/applications'
 		url_params = []
+		if fileName:
+			url_params.append('attributes.fileName=' + fileName)
+		if path:
+			url_params.append('attributes.path=' + path)
+		if signer:
+			url_params.append('attributes.signer=' + signer)
+		if currentPage:
+			url_params.append('currentPage=' + str(currentPage))
+		if enabled:
+			url_params.append('enabled=' + enabled)
+		if hash:
+			url_params.append('hash=' + hash)
+		if operatingSystem:
+			url_params.append('operatingSystem=' + operatingSystem)
+		if organization:
+			url_params.append('organization=' + organization)
+		if policyIds:
+			url_params.append('policyIds=' + policyIds)
+		if tag:
+			url_params.append('tag=' + tag)
 		url += '?' + '&'.join(url_params)
-		adminSetTrayNotificationSettingsRequest = {
-			'enabledPopup': enabledPopup,
-			'enabledTrayNotification': enabledTrayNotification,
-			'message': message,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, adminSetTrayNotificationSettingsRequest)
-
-class Administrator:
-	'''The Administrator module enables administrators to perform administrative operations, such as handling licenses and users.'''
-
-	def list_collector_installers(self, organization :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def send_applications(self, applicationControls: dict = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: This API call output the available collectors installers.
-
+		Class ApplicationControl
+		Description: Saves new application controls and returns a list of them.
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			applicationControlSaveRequest (Object): Check 'applicationControlSaveRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
+		'''
+		validate_params("send_applications", locals())
+
+		url = '/api/application-control/applications'
 
+		applicationControlSaveRequest = {
+			"applicationControls": applicationControls,
+			"organization": organization,
+		}
+		return fortiedr_connection.send(url, applicationControlSaveRequest)
+
+	def insert_applications(self, appIds: dict, organization: str, enabled: bool = None, groupIds: dict = None, isOverridePolicies: bool = None, policyIds: dict = None, tagId: int = None) -> tuple[bool, list]:
 		'''
-		url = '/management-rest/admin/list-collector-installers'
+		Class ApplicationControl
+		Description: Edits existing application control and returns the affected ones.
+        
+		Args:
+			appIds (dict): The relevant application IDs to edit.
+			modifiedFields (Object): Check 'modifiedFields' in the API documentation for further information.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("insert_applications", locals())
+
+		url = '/api/application-control/applications'
 		url_params = []
+		if appIds:
+			url_params.append('appIds=' + appIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
 
-	def list_system_summary(self, addLicenseBlob :bool = None, organization :str = None) -> tuple[bool, None]:
+		modifiedFields = {
+			"enabled": enabled,
+			"groupIds": groupIds,
+			"isOverridePolicies": isOverridePolicies,
+			"policyIds": policyIds,
+			"tagId": str(tagId),
+		}
+		return fortiedr_connection.insert(url, modifiedFields)
 
+	def delete_applications(self, organization: str, applicationIds: dict = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: Get System Summary.
-
+		Class ApplicationControl
+		Description: Deletes application controls.
+        
 		Args:
-			addLicenseBlob: Indicates whether to put license blob to response. By default addLicenseBlob is false. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			applicationIds (dict): The IDs of the applications to be deleted.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/admin/list-system-summary'
+		validate_params("delete_applications", locals())
+
+		url = '/api/application-control/applications'
 		url_params = []
-		if addLicenseBlob:
-			url_params.append('addLicenseBlob=' + str(addLicenseBlob))
+		if applicationIds:
+			url_params.append('applicationIds=' + applicationIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
+		return fortiedr_connection.delete(url)
 
-	def previous_registration_passwords(self, organization: str = None) -> tuple[bool, dict]:
+	def force_update_ootb_application_controls(self) -> tuple[bool, None]:
+		'''
+		Class ApplicationControl
+		Description: Trigger OOTB application control update.
+        
+		Args:
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Administrator
-		Description: This API retrieve previous registration passwords for given organization.
+		validate_params("force_update_ootb_application_controls", locals())
+
+		url = '/api/application-control/force-update-ootb-application-controls'
+		return fortiedr_connection.send(url)
 
+	def tags(self, name: str = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class ApplicationControl
+		Description: Create an application control tags.
+        
 		Args:
-			organizationRequest: organizationRequest. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			applicationControlTagCreateRequest (Object): Check 'applicationControlTagCreateRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/admin/previous-registration-passwords'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		organizationRequest = {
-			'organization': organization
-		}
-		return fortiedr_connection.get(url, organizationRequest)
+		validate_params("tags", locals())
 
+		url = '/api/application-control/tags'
 
-	def previous_registration_passwords(self, passwordId : int, organization: str = None) -> tuple[bool, str]:
+		applicationControlTagCreateRequest = {
+			"name": name,
+			"organization": organization,
+		}
+		return fortiedr_connection.send(url, applicationControlTagCreateRequest)
 
-		'''
-		class Administrator
-		Description: This API deletes previous registration password for given id.
+class Dashboard:
+	'''Dashboard Rest Api Controller'''
 
+	def most_targeted_items(self, organization: str, itemType: str = None, numOfColumns: int = None, numOfDays: int = None) -> tuple[bool, None]:
+		'''
+		Class Dashboard
+		Description: Returns most targeted devices or most targeted processes, depending on the itemType parameter.
+        
 		Args:
-			organizationRequest: organizationRequest. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			passwordId: passwordId. 
+			itemType (str): Specifies the type of items.
+			numOfColumns (int): Specifies the number of columns to present.
+			numOfDays (int): Specifies the number of days to present.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			str
-
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/admin/previous-registration-passwords/{passwordId}'
+		validate_params("most_targeted_items", locals())
+
+		url = '/api/dashboard/most-targeted-items'
 		url_params = []
+		if itemType:
+			url_params.append('itemType=' + itemType)
+		if numOfColumns:
+			url_params.append('numOfColumns=' + str(numOfColumns))
+		if numOfDays:
+			url_params.append('numOfDays=' + str(numOfDays))
+		if organization:
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.delete(url)
-
-
-	def ready(self) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def unhandled_items(self, organization: str, itemType: str = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: Get System Readiness.
-
+		Class Dashboard
+		Description: Returns unhandled devices or unhandled processes, depending on the itemType parameter.
+        
 		Args:
-			organizationRequest: organizationRequest. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			passwordId: passwordId. 
+			itemType (str): Specifies the type of items.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/admin/ready'
-		return fortiedr_connection.get(url)
+		validate_params("unhandled_items", locals())
 
+		url = '/api/dashboard/unhandled-items'
+		url_params = []
+		if itemType:
+			url_params.append('itemType=' + itemType)
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
 
-	def registration_password(self, password: str, organization: str = None) -> tuple[bool, None]:
+class Administrator:
+	'''The Administrator module enables administrators to perform administrative operations, such as handling licenses and users.'''
 
+	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: This API creates new registration password for given organization.
-
+		Class Administrator
+		Description: Update tray notification settings.
+        
 		Args:
-			request: request. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			password: New Registration Password. 
+			adminSetTrayNotificationSettingsRequest (Object): Check 'adminSetTrayNotificationSettingsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/admin/registration-password'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		request = {
-			'organization': organization,
-			'password': password
-		}
-		return fortiedr_connection.send(url, request)
+		validate_params("set_tray_notification_settings", locals())
 
+		url = '/api/admin/set-tray-notification-settings'
 
-	def set_system_mode(self, mode : str, forceAll :bool = None, organization :str = None) -> tuple[bool, None]:
+		adminSetTrayNotificationSettingsRequest = {
+			"enabledPopup": enabledPopup,
+			"enabledTrayNotification": enabledTrayNotification,
+			"message": message,
+			"organization": organization,
+		}
+		return fortiedr_connection.send(url, adminSetTrayNotificationSettingsRequest)
 
+	def list_collector_installers(self, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: Set system modeThis API call enables you to switch the system to Simulation mode.
-
+		Class Administrator
+		Description: This API call output the available collectors installers.
+        
 		Args:
-			forceAll: Indicates whether to force set all the policies in 'Prevention' mode. 
-			mode: Operation mode. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/admin/set-system-mode'
+		validate_params("list_collector_installers", locals())
+
+		url = '/management-rest/admin/list-collector-installers'
 		url_params = []
-		if forceAll:
-			url_params.append('forceAll=' + str(forceAll))
-		if mode:
-			url_params.append('mode=' + str(mode))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-
-	def update_collector_installer(self, collectorGroupIds :dict = None, collectorGroups :dict = None, organization :str = None, updateVersions: dict = None) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def list_system_summary(self, addLicenseBlob: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Administrator
-		Description: This API update collectors target version for collector groups.
-
+		Class Administrator
+		Description: Get System Summary.
+        
 		Args:
-			collectorGroupIds: Specifies the list of IDs of all the collector groups which should be updated.. 
-			collectorGroups: Specifies the list of all the collector groups which should be updated.. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			requestUpdateData: requestUpdateData. 
-			updateVersions: List of installer versions that should be applied in the collector groups. 
+			addLicenseBlob (bool): Indicates whether to put license blob to response. By default addLicenseBlob is false.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/admin/update-collector-installer'
+		validate_params("list_system_summary", locals())
+
+		url = '/management-rest/admin/list-system-summary'
 		url_params = []
-		if collectorGroupIds:
-			url_params.append('collectorGroupIds=' + str(collectorGroupIds))
-		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+		if addLicenseBlob:
+			url_params.append('addLicenseBlob=' + addLicenseBlob)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		requestUpdateData = {
-			'updateVersions': updateVersions
-		}
-		return fortiedr_connection.send(url, requestUpdateData)
-
-
-	def upload_content(self, file : BinaryIO) -> tuple[bool, str]:
+		return fortiedr_connection.get(url)
 
+	def previous_registration_passwords(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class Administrator
-		Description: Upload content to the system.
-
+		Class Administrator
+		Description: This API retrieve previous registration passwords for given organization.
+        
 		Args:
-			file: file. 
+			organizationRequest (Object): Check 'organizationRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			str
-
+			list
 		'''
-		url = '/management-rest/admin/upload-content'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
+		validate_params("previous_registration_passwords", locals())
 
+		url = '/management-rest/admin/previous-registration-passwords'
 
-	def upload_license(self, licenseBlob: str = None) -> tuple[bool, None]:
+		organizationRequest = {
+			"organization": organization,
+		}
+		return fortiedr_connection.get(url, organizationRequest)
 
+	def previous_registration_passwords(self, passwordId: int, organization: str = None) -> tuple[bool, str]:
 		'''
-		class Administrator
-		Description: Upload license to the system.
-
+		Class Administrator
+		Description: This API deletes previous registration password for given id.
+        
 		Args:
-			license: license. 
-			licenseBlob: License blob. 
+			organizationRequest (Object): Check 'organizationRequest' in the API documentation for further information.
+			passwordId (int): passwordId.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
+			str
 		'''
-		url = '/management-rest/admin/upload-license'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		license = {
-			'licenseBlob': licenseBlob
-		}
-		return fortiedr_connection.insert(url, license)
+		validate_params("previous_registration_passwords", locals())
 
-class ApplicationControl:
-	'''Application Control Rest Api Controller'''
+		url = f'/management-rest/admin/previous-registration-passwords/{passwordId}'
 
-	def get_applications(self, currentPage : int, organization : str, fileName :str = None, path :str = None, signer :str = None, enabled :bool = None, hash :str = None, operatingSystem :str = None, policyIds :dict = None, tag :str = None) -> tuple[bool, None]:
+		organizationRequest = {
+			"organization": organization,
+		}
+		return fortiedr_connection.delete(url, organizationRequest)
 
+	def ready(self) -> tuple[bool, None]:
 		'''
-		class ApplicationControl
-		Description: Get application controls.
-
+		Class Administrator
+		Description: Get System Readiness.
+        
 		Args:
-			fileName: Specifies the file name, if contains special characters - encode to HTML URL Encoding. 
-			path: Specifies the path, if contains special characters - encode to HTML URL Encoding. 
-			signer: Specifies the value, if contains special characters - encode to HTML URL Encoding. 
-			currentPage: Specifies the current page. 
-			enabled: Specifies the state of the application control. 
-			hash: Specifies the hash of the application control. 
-			operatingSystem: Specifies the operating system of the application control. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyIds: Specifies the IDs of the relevant policies for application control. 
-			tag: Specifies the tag related to application control. 
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/api/application-control/applications'
-		url_params = []
-		if fileName:
-			url_params.append('fileName=' + str(fileName))
-		if path:
-			url_params.append('path=' + str(path))
-		if signer:
-			url_params.append('signer=' + str(signer))
-		if currentPage:
-			url_params.append('currentPage=' + str(currentPage))
-		if enabled:
-			url_params.append('enabled=' + str(enabled))
-		if hash:
-			url_params.append('hash=' + str(hash))
-		if operatingSystem:
-			url_params.append('operatingSystem=' + str(operatingSystem))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if policyIds:
-			url_params.append('policyIds=' + str(policyIds))
-		if tag:
-			url_params.append('tag=' + str(tag))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		validate_params("ready", locals())
 
-	def send_applications(self, applicationControls: dict, organization: str) -> tuple[bool, None]:
+		url = '/management-rest/admin/ready'
+		return fortiedr_connection.get(url)
 
+	def registration_password(self, organization: str = None, password: str = None) -> tuple[bool, None]:
 		'''
-		class ApplicationControl
-		Description: Get application controls.
-
+		Class Administrator
+		Description: This API creates new registration password for given organization.
+        
 		Args:
-			applicationControlSaveRequest: applicationControlSaveRequest. 
-			applicationControls: Specifies the list of applications to add. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			request (Object): Check 'request' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/api/application-control/applications'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		applicationControlSaveRequest = {
-			'applicationControls': applicationControls,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, applicationControlSaveRequest)
+		validate_params("registration_password", locals())
 
-	def insert_applications(self, appIds : dict, organization : str, enabled: bool = None, groupIds: dict = None, isOverridePolicies: bool = None, policyIds: dict = None, tagId: int = None) -> tuple[bool, dict]:
+		url = '/management-rest/admin/registration-password'
 
-		'''
-		class ApplicationControl
-		Description: Get application controls.
+		request = {
+			"organization": organization,
+			"password": password,
+		}
+		return fortiedr_connection.send(url, request)
 
+	def set_system_mode(self, mode: str, forceAll: bool = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class Administrator
+		Description: Set system modeThis API call enables you to switch the system to Simulation mode.
+        
 		Args:
-			appIds: The relevant application IDs to edit. 
-			modifiedFields: modifiedFields. 
-			enabled: Specifies the state of the application. 
-			groupIds: Specifies the IDs of the groups to assign the application. 
-			isOverridePolicies: Set true to override all current policies, if false or not specified they will be added to the current policies. 
-			policyIds: Specifies the IDs of the policies to assign the application. 
-			tagId: Specifies the new tag ID of the application. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			forceAll (bool): Indicates whether to force set all the policies in 'Prevention' mode.
+			mode (str): Operation mode.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			None: This function does not return any data.
 		'''
-		url = '/api/application-control/applications'
+		validate_params("set_system_mode", locals())
+
+		url = '/management-rest/admin/set-system-mode'
 		url_params = []
-		if appIds:
-			url_params.append('appIds=' + str(appIds))
+		if forceAll:
+			url_params.append('forceAll=' + forceAll)
+		if mode:
+			url_params.append('mode=' + mode)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def delete_applications(self, organization : str, applicationIds :dict = None) -> tuple[bool, None]:
-
+	def update_collector_installer(self, collectorGroupIds: dict = None, collectorGroups: dict = None, organization: str = None, updateVersions: dict = None) -> tuple[bool, None]:
 		'''
-		class ApplicationControl
-		Description: Get application controls.
-
+		Class Administrator
+		Description: This API update collectors target version for collector groups.
+        
 		Args:
-			applicationIds: The IDs of the applications to be deleted. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			collectorGroupIds (dict): Specifies the list of IDs of all the collector groups which should be updated..
+			collectorGroups (dict): Specifies the list of all the collector groups which should be updated..
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			requestUpdateData (Object): Check 'requestUpdateData' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/api/application-control/applications'
+		validate_params("update_collector_installer", locals())
+
+		url = '/management-rest/admin/update-collector-installer'
 		url_params = []
-		if applicationIds:
-			url_params.append('applicationIds=' + str(applicationIds))
+		if collectorGroupIds:
+			url_params.append('collectorGroupIds=' + collectorGroupIds)
+		if collectorGroups:
+			url_params.append('collectorGroups=' + collectorGroups)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.delete(url)
-
 
-	def force_update_ootb_application_controls(self) -> tuple[bool, None]:
+		requestUpdateData = {
+			"updateVersions": updateVersions,
+		}
+		return fortiedr_connection.send(url, requestUpdateData)
 
+	def upload_content(self, file: BinaryIO, ) -> tuple[bool, str]:
 		'''
-		class ApplicationControl
-		Description: Trigger OOTB application control update.
-
+		Class Administrator
+		Description: Upload content to the system.
+        
 		Args:
-			applicationIds: The IDs of the applications to be deleted. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			file (BinaryIO): file.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			str
 		'''
-		url = '/api/application-control/force-update-ootb-application-controls'
-		return fortiedr_connection.send(url)
-
+		validate_params("upload_content", locals())
 
-	def tags(self, name: str, organization: str) -> tuple[bool, None]:
+		url = '/management-rest/admin/upload-content'
+		if file:
+			file = {'file': file}
+		return fortiedr_connection.upload(url, file, request_type="multipart/form-data")
 
+	def upload_license(self, licenseBlob: str = None) -> tuple[bool, None]:
 		'''
-		class ApplicationControl
-		Description: Create an application control tags.
-
+		Class Administrator
+		Description: Upload license to the system.
+        
 		Args:
-			applicationControlTagCreateRequest: applicationControlTagCreateRequest. 
-			name: Specifies the name of the application control tag. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			license (Object): Check 'license' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/api/application-control/tags'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		applicationControlTagCreateRequest = {
-			'name': name,
-			'organization': organization
+		validate_params("upload_license", locals())
+
+		url = '/management-rest/admin/upload-license'
+
+		license = {
+			"licenseBlob": licenseBlob,
 		}
-		return fortiedr_connection.send(url, applicationControlTagCreateRequest)
+		return fortiedr_connection.insert(url, license)
 
 class Audit:
 	'''The Audit module enables you to retrieve system audit based on given dates'''
 
-	def get_audit(self, fromTime :str = None, organization :str = None, toTime :str = None) -> tuple[bool, dict]:
-
+	def get_audit(self, fromTime: str = None, organization: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
-		class Audit
+		Class Audit
 		Description: This API retrieve the audit between 2 dates.
-
+        
 		Args:
-			fromTime: Retrieves audit that were written after the given date. Date Format: yyyy-MM-dd (Default is current date). 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			toTime: Retrieves audit that were written before the given date. Date Format: yyyy-MM-dd (Default is current date). 
+			fromTime (str): Retrieves audit that were written after the given date. Date Format: yyyy-MM-dd (Default is current date).
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			toTime (str): Retrieves audit that were written before the given date. Date Format: yyyy-MM-dd (Default is current date).
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("get_audit", locals())
+
 		url = '/management-rest/audit/get-audit'
 		url_params = []
 		if fromTime:
-			url_params.append('fromTime=' + str(fromTime))
+			url_params.append('fromTime=' + fromTime)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if toTime:
-			url_params.append('toTime=' + str(toTime))
+			url_params.append('toTime=' + toTime)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 class CommunicationControl:
 	'''Fortinet Endpoint Protection and Response Platform’s Communication Control module is responsible for monitoring and handling non-disguised security events. The module uses a set of policies that contain recommendations about whether an application should be approved or denied from communicating outside your organization.'''
 
-	def assign_collector_group(self, collectorGroups : dict, policyName : str, forceAssign :bool = None, organization :str = None) -> tuple[bool, None]:
-
+	def assign_collector_group(self, collectorGroups: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: Assign collector group to application policy.
-
+        
 		Args:
-			collectorGroups:  Specifies the collector groups whose collector reported the events. 
-			forceAssign: Indicates whether to force the assignment even if the group is assigned to similar policies. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies the list of policies. 
+			collectorGroups (dict):  Specifies the collector groups whose collector reported the events.
+			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies the list of policies.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("assign_collector_group", locals())
+
 		url = '/management-rest/comm-control/assign-collector-group'
 		url_params = []
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if forceAssign:
-			url_params.append('forceAssign=' + str(forceAssign))
+			url_params.append('forceAssign=' + forceAssign)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def clone_policy(self, newPolicyName : str, sourcePolicyName : str, organization :str = None) -> tuple[bool, None]:
-
+	def clone_policy(self, newPolicyName: str, sourcePolicyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: application clone policy.
-
+        
 		Args:
-			newPolicyName: Specifies security policy target name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			sourcePolicyName: Specifies security policy source name. 
+			newPolicyName (str): Specifies security policy target name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			sourcePolicyName (str): Specifies security policy source name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("clone_policy", locals())
+
 		url = '/management-rest/comm-control/clone-policy'
 		url_params = []
 		if newPolicyName:
-			url_params.append('newPolicyName=' + str(newPolicyName))
+			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if sourcePolicyName:
-			url_params.append('sourcePolicyName=' + str(sourcePolicyName))
+			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def list_policies(self, decisions : dict, itemsPerPage :int = None, organization :str = None, pageNumber :int = None, policies :dict = None, rules :dict = None, sorting :str = None, sources :dict = None, state :str = None, strictMode :bool = None) -> tuple[bool, dict]:
+		return fortiedr_connection.upload(url)
 
+	def list_policies(self, decisions: dict, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, policies: dict = None, rules: dict = None, sorting: str = None, sources: dict = None, state: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: This API call outputs a list of all the communication control policies in the system, and information about each of them.
-
+        
 		Args:
-			decisions: Indicates the action. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			policies: Specifies the list of policy names. 
-			rules: Specifies the list of rules. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			sources: Specifies who created the policy. 
-			state: Policy rule state. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+			decisions (dict): Indicates the action.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			policies (dict): Specifies the list of policy names.
+			rules (dict): Specifies the list of rules.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			sources (dict): Specifies who created the policy.
+			state (str): Policy rule state.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_policies", locals())
+
 		url = '/management-rest/comm-control/list-policies'
 		url_params = []
 		if decisions:
-			url_params.append('decisions=' + str(decisions))
+			url_params.append('decisions=' + decisions)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if policies:
-			url_params.append('policies=' + str(policies))
+			url_params.append('policies=' + policies)
 		if rules:
-			url_params.append('rules=' + str(rules))
+			url_params.append('rules=' + rules)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if sources:
-			url_params.append('sources=' + str(sources))
+			url_params.append('sources=' + sources)
 		if state:
-			url_params.append('state=' + str(state))
+			url_params.append('state=' + state)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_products(self, action :str = None, collectorGroups :dict = None, cveIdentifier :str = None, destinationIp :dict = None, devices :dict = None, firstConnectionTimeEnd :str = None, firstConnectionTimeStart :str = None, handled :bool = None, includeStatistics :bool = None, ips :dict = None, itemsPerPage :int = None, lastConnectionTimeEnd :str = None, lastConnectionTimeStart :str = None, organization :str = None, os :dict = None, pageNumber :int = None, policies :dict = None, processHash :str = None, processes :dict = None, product :str = None, products :dict = None, reputation :dict = None, rule :str = None, rulePolicy :str = None, seen :bool = None, sorting :str = None, strictMode :bool = None, vendor :str = None, vendors :dict = None, version :str = None, versions :dict = None, vulnerabilities :dict = None) -> tuple[bool, dict]:
-
+	def list_products(self, action: str = None, collectorGroups: dict = None, cveIdentifier: str = None, destinationIp: dict = None, devices: dict = None, firstConnectionTimeEnd: str = None, firstConnectionTimeStart: str = None, handled: bool = None, includeStatistics: bool = None, ips: dict = None, itemsPerPage: int = None, lastConnectionTimeEnd: str = None, lastConnectionTimeStart: str = None, organization: str = None, os: dict = None, pageNumber: int = None, policies: dict = None, processHash: str = None, processes: dict = None, product: str = None, products: dict = None, reputation: dict = None, rule: str = None, rulePolicy: str = None, seen: bool = None, sorting: str = None, strictMode: bool = None, vendor: str = None, vendors: dict = None, version: str = None, versions: dict = None, vulnerabilities: dict = None) -> tuple[bool, list]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: This API call outputs a list of all the communicating applications in the system, and information about each of them.
-
+        
 		Args:
-			action: Indicates the action: Allow/Deny. This parameter is irrelevant without policies parameter. 
-			collectorGroups: Specifies the list of collector groups where the products were seen. 
-			cveIdentifier: Specifies the CVE identifier. 
-			destinationIp: Destination IPs. 
-			devices: Specifies the list of device names where the products were seen. 
-			firstConnectionTimeEnd:  Retrieves products whose first connection time is less than the value assigned to this date. 
-			firstConnectionTimeStart:  Retrieves products whose first connection time is greater than the value assigned to this date. 
-			handled: A true/false parameter indicating whether events were handled/unhandled. 
-			includeStatistics: A true/false parameter indicating including statistics data. 
-			ips: Specifies the list of IPs where the products were seen. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastConnectionTimeEnd:  Retrieves products whose last connection time is less than the value assigned to this date. 
-			lastConnectionTimeStart:  Retrieves products whose last connection time is greater than the value assigned to this date. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			os: Specifies the list of operating system families where the products were seen. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			policies: Specifies the list of policy names whose products have a specific decision, as specified in the action parameter. 
-			processHash: Specifies the process hash name. 
-			processes: Specifies the list of process names running alongside the products. 
-			product: Specifies a single value for the product name. By default, strictMode is false. 
-			products: Specifies the list of product names. Names must match exactly (strictMode is always true). 
-			reputation: Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good. 
-			rule: Indicates the rule. This parameter is irrelevant without rulePolicy parameter. 
-			rulePolicy: Specifies the policy name whose products have a specific rule, as specified in the rule parameter. 
-			seen: A true/false parameter indicating whether events were read/unread by the user operating the API. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			vendor: Specifies a single value for the vendor name. By default, strictMode is false. 
-			vendors: Specifies the list of vendor names. Names must match exactly (strictMode is always true). 
-			version: Specifies a single value for the version name. By default, strictMode is false. 
-			versions: Specifies the list of versions. Names must match exactly (strictMode is always true). 
-			vulnerabilities: Specifies the list of vulnerabilities where the products were seen. 
+			action (str): Indicates the action: Allow/Deny. This parameter is irrelevant without policies parameter.
+			collectorGroups (dict): Specifies the list of collector groups where the products were seen.
+			cveIdentifier (str): Specifies the CVE identifier.
+			destinationIp (dict): Destination IPs.
+			devices (dict): Specifies the list of device names where the products were seen.
+			firstConnectionTimeEnd (str):  Retrieves products whose first connection time is less than the value assigned to this date.
+			firstConnectionTimeStart (str):  Retrieves products whose first connection time is greater than the value assigned to this date.
+			handled (bool): A true/false parameter indicating whether events were handled/unhandled.
+			includeStatistics (bool): A true/false parameter indicating including statistics data.
+			ips (dict): Specifies the list of IPs where the products were seen.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastConnectionTimeEnd (str):  Retrieves products whose last connection time is less than the value assigned to this date.
+			lastConnectionTimeStart (str):  Retrieves products whose last connection time is greater than the value assigned to this date.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			os (dict): Specifies the list of operating system families where the products were seen.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			policies (dict): Specifies the list of policy names whose products have a specific decision, as specified in the action parameter.
+			processHash (str): Specifies the process hash name.
+			processes (dict): Specifies the list of process names running alongside the products.
+			product (str): Specifies a single value for the product name. By default, strictMode is false.
+			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			reputation (dict): Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good.
+			rule (str): Indicates the rule. This parameter is irrelevant without rulePolicy parameter.
+			rulePolicy (str): Specifies the policy name whose products have a specific rule, as specified in the rule parameter.
+			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			vendor (str): Specifies a single value for the vendor name. By default, strictMode is false.
+			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			version (str): Specifies a single value for the version name. By default, strictMode is false.
+			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			vulnerabilities (dict): Specifies the list of vulnerabilities where the products were seen.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_products", locals())
+
 		url = '/management-rest/comm-control/list-products'
 		url_params = []
 		if action:
-			url_params.append('action=' + str(action))
+			url_params.append('action=' + action)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if cveIdentifier:
-			url_params.append('cveIdentifier=' + str(cveIdentifier))
+			url_params.append('cveIdentifier=' + cveIdentifier)
 		if destinationIp:
-			url_params.append('destinationIp=' + str(destinationIp))
+			url_params.append('destinationIp=' + destinationIp)
 		if devices:
-			url_params.append('devices=' + str(devices))
+			url_params.append('devices=' + devices)
 		if firstConnectionTimeEnd:
-			url_params.append('firstConnectionTimeEnd=' + str(firstConnectionTimeEnd))
+			url_params.append('firstConnectionTimeEnd=' + firstConnectionTimeEnd)
 		if firstConnectionTimeStart:
-			url_params.append('firstConnectionTimeStart=' + str(firstConnectionTimeStart))
+			url_params.append('firstConnectionTimeStart=' + firstConnectionTimeStart)
 		if handled:
-			url_params.append('handled=' + str(handled))
+			url_params.append('handled=' + handled)
 		if includeStatistics:
-			url_params.append('includeStatistics=' + str(includeStatistics))
+			url_params.append('includeStatistics=' + includeStatistics)
 		if ips:
-			url_params.append('ips=' + str(ips))
+			url_params.append('ips=' + ips)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastConnectionTimeEnd:
-			url_params.append('lastConnectionTimeEnd=' + str(lastConnectionTimeEnd))
+			url_params.append('lastConnectionTimeEnd=' + lastConnectionTimeEnd)
 		if lastConnectionTimeStart:
-			url_params.append('lastConnectionTimeStart=' + str(lastConnectionTimeStart))
+			url_params.append('lastConnectionTimeStart=' + lastConnectionTimeStart)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if os:
-			url_params.append('os=' + str(os))
+			url_params.append('os=' + os)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if policies:
-			url_params.append('policies=' + str(policies))
+			url_params.append('policies=' + policies)
 		if processHash:
-			url_params.append('processHash=' + str(processHash))
+			url_params.append('processHash=' + processHash)
 		if processes:
-			url_params.append('processes=' + str(processes))
+			url_params.append('processes=' + processes)
 		if product:
-			url_params.append('product=' + str(product))
+			url_params.append('product=' + product)
 		if products:
-			url_params.append('products=' + str(products))
+			url_params.append('products=' + products)
 		if reputation:
-			url_params.append('reputation=' + str(reputation))
+			url_params.append('reputation=' + reputation)
 		if rule:
-			url_params.append('rule=' + str(rule))
+			url_params.append('rule=' + rule)
 		if rulePolicy:
-			url_params.append('rulePolicy=' + str(rulePolicy))
+			url_params.append('rulePolicy=' + rulePolicy)
 		if seen:
-			url_params.append('seen=' + str(seen))
+			url_params.append('seen=' + seen)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		if vendor:
-			url_params.append('vendor=' + str(vendor))
+			url_params.append('vendor=' + vendor)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		if version:
-			url_params.append('version=' + str(version))
+			url_params.append('version=' + version)
 		if versions:
-			url_params.append('versions=' + str(versions))
+			url_params.append('versions=' + versions)
 		if vulnerabilities:
-			url_params.append('vulnerabilities=' + str(vulnerabilities))
+			url_params.append('vulnerabilities=' + vulnerabilities)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def resolve_applications(self, applyNested :bool = None, comment :str = None, organization :str = None, products :dict = None, resolve :bool = None, signed :bool = None, vendors :dict = None, versions :dict = None) -> tuple[bool, None]:
-
+	def resolve_applications(self, applyNested: bool = None, comment: str = None, organization: str = None, products: dict = None, resolve: bool = None, signed: bool = None, vendors: dict = None, versions: dict = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: Enable resolving/unresolving applications.
-
+        
 		Args:
-			applyNested: A true/false parameter indicating updating inherited. 
-			comment: Specifies a user-defined string to attach to the policy. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			products: Specifies the list of product names. Names must match exactly (strictMode is always true). 
-			resolve: A true/false parameter indicating update the application resolve/unresolve. 
-			signed: A true/false parameter indicating if the policy is signed. 
-			vendors: Specifies the list of vendor names. Names must match exactly (strictMode is always true). 
-			versions: Specifies the list of versions. Names must match exactly (strictMode is always true). 
+			applyNested (bool): A true/false parameter indicating updating inherited.
+			comment (str): Specifies a user-defined string to attach to the policy.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			resolve (bool): A true/false parameter indicating update the application resolve/unresolve.
+			signed (bool): A true/false parameter indicating if the policy is signed.
+			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("resolve_applications", locals())
+
 		url = '/management-rest/comm-control/resolve-applications'
 		url_params = []
 		if applyNested:
-			url_params.append('applyNested=' + str(applyNested))
+			url_params.append('applyNested=' + applyNested)
 		if comment:
-			url_params.append('comment=' + str(comment))
+			url_params.append('comment=' + comment)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if products:
-			url_params.append('products=' + str(products))
+			url_params.append('products=' + products)
 		if resolve:
-			url_params.append('resolve=' + str(resolve))
+			url_params.append('resolve=' + resolve)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		if versions:
-			url_params.append('versions=' + str(versions))
+			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def set_policy_mode(self, mode : str, policyNames : dict, organization :str = None) -> tuple[bool, None]:
-
+	def set_policy_mode(self, mode: str, policyNames: dict, organization: str = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: Set policy to simulation/prevention.
-
+        
 		Args:
-			mode: Operation mode. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyNames: Specifies the list of policies. 
+			mode (str): Operation mode.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyNames (dict): Specifies the list of policies.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_policy_mode", locals())
+
 		url = '/management-rest/comm-control/set-policy-mode'
 		url_params = []
 		if mode:
-			url_params.append('mode=' + str(mode))
+			url_params.append('mode=' + mode)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyNames:
-			url_params.append('policyNames=' + str(policyNames))
+			url_params.append('policyNames=' + policyNames)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def set_policy_permission(self, decision : str, policies : dict, applyNested :bool = None, organization :str = None, products :dict = None, signed :bool = None, vendors :dict = None, versions :dict = None) -> tuple[bool, None]:
-
+	def set_policy_permission(self, decision: str, policies: dict, applyNested: bool = None, organization: str = None, products: dict = None, signed: bool = None, vendors: dict = None, versions: dict = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: Set the application allow/deny.
-
+        
 		Args:
-			applyNested: A true/false parameter indicating updating inherited. 
-			decision: Indicates the action. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policies: Specifies the list of policies names. 
-			products: Specifies the list of product names. Names must match exactly (strictMode is always true). 
-			signed: A true/false parameter indicating if the policy is signed. 
-			vendors: Specifies the list of vendor names. Names must match exactly (strictMode is always true). 
-			versions: Specifies the list of versions. Names must match exactly (strictMode is always true). 
+			applyNested (bool): A true/false parameter indicating updating inherited.
+			decision (str): Indicates the action.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policies (dict): Specifies the list of policies names.
+			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			signed (bool): A true/false parameter indicating if the policy is signed.
+			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_policy_permission", locals())
+
 		url = '/management-rest/comm-control/set-policy-permission'
 		url_params = []
 		if applyNested:
-			url_params.append('applyNested=' + str(applyNested))
+			url_params.append('applyNested=' + applyNested)
 		if decision:
-			url_params.append('decision=' + str(decision))
+			url_params.append('decision=' + decision)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policies:
-			url_params.append('policies=' + str(policies))
+			url_params.append('policies=' + policies)
 		if products:
-			url_params.append('products=' + str(products))
+			url_params.append('products=' + products)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		if versions:
-			url_params.append('versions=' + str(versions))
+			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def set_policy_rule_state(self, policyName : str, ruleName : str, state : str, organization :str = None) -> tuple[bool, None]:
-
+	def set_policy_rule_state(self, policyName: str, ruleName: str, state: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class CommunicationControl
+		Class CommunicationControl
 		Description: Set rule in policy to enable/disable.
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies policy name. 
-			ruleName: Specifies rule name. 
-			state: Policy rule state. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies policy name.
+			ruleName (str): Specifies rule name.
+			state (str): Policy rule state.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_policy_rule_state", locals())
+
 		url = '/management-rest/comm-control/set-policy-rule-state'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		if ruleName:
-			url_params.append('ruleName=' + str(ruleName))
+			url_params.append('ruleName=' + ruleName)
 		if state:
-			url_params.append('state=' + str(state))
+			url_params.append('state=' + state)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class Events:
 	'''This API call outputs all the events in the system that match the condition(s) you specify in the call. An AND relationship exists when specifying multiple input parameters. When no input parameters are matched, an empty result set is returned'''
 
-	def insert_events(self, actions :dict = None, applicationControl :bool = None, archived :bool = None, classifications :dict = None, collectorGroups :dict = None, destinations :dict = None, device :str = None, deviceControl :bool = None, deviceIps :dict = None, eventIds :dict = None, eventType :dict = None, expired :bool = None, fileHash :str = None, firstSeen :str = None, firstSeenFrom :str = None, firstSeenTo :str = None, handled :bool = None, itemsPerPage :int = None, lastSeen :str = None, lastSeenFrom :str = None, lastSeenTo :str = None, loggedUser :str = None, macAddresses :dict = None, muted :bool = None, operatingSystems :dict = None, organization :str = None, pageNumber :int = None, paths :dict = None, process :str = None, rule :str = None, seen :bool = None, severities :dict = None, signed :bool = None, sorting :str = None, strictMode :bool = None, archive: bool = None, classification: str = None, comment: str = None, familyName: str = None, forceUnmute: bool = None, handle: bool = None, malwareType: str = None, mute: bool = None, muteDuration: str = None, read: bool = None, threatName: str = None) -> tuple[bool, None]:
-
+	def insert_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None, archive: bool = None, classification: str = None, comment: str = None, familyName: str = None, forceUnmute: bool = None, handle: bool = None, malwareType: str = None, mute: bool = None, muteDuration: str = None, read: bool = None, threatName: str = None) -> tuple[bool, None]:
 		'''
-		class Events
+		Class Events
 		Description: This API call updates the read/unread, handled/unhandled or archived/unarchived state of an event. The output of this call is a message indicating whether the update succeeded or failed.
-
+        
 		Args:
-			actions: Specifies the action of the event. 
-			applicationControl: A true/false parameter indicating whether to include only application control events. 
-			archived: A true/false parameter indicating whether to include only archived events. 
-			classifications: Specifies the classification of the event. 
-			collectorGroups: Specifies the collector groups whose collector reported the events. 
-			destinations: Specifies the connection destination(s) of the events. 
-			device: Specifies the device name where the events occurred. 
-			deviceControl: A true/false parameter indicating whether to include only device control events. 
-			deviceIps: Specifies the IPs of the devices where the event occurred. 
-			eventIds: Specifies the required event IDs. 
-			eventType: Specifies the type of the event. 
-			expired: A true/false parameter indicating whether to include only expired events. 
-			fileHash: Specifies the hash signature of the main process of the event. 
-			firstSeen:  Specifies the date when the event was first seen (Deprecated). 
-			firstSeenFrom: Specifies the from date when the event was first seen. 
-			firstSeenTo: Specifies the to date when the event was first seen. 
-			handled:  A true/false parameter indicating whether events were handled/unhandled. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeen:  Specifies the date when the event was last seen (Deprecated). 
-			lastSeenFrom: Specifies the from date when the event was last seen. 
-			lastSeenTo: Specifies the to date when the event was last seen. 
-			loggedUser: Specifies the logged user. 
-			macAddresses: Specifies the mac addresses where the event occurred. 
-			muted: A true/false parameter indicating if the event is muted. 
-			operatingSystems: Specifies the operating system of the devices where the events occurred. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			paths: Specifies the paths of the processes related to the event. 
-			process: Specifies the main process of the event. 
-			rule: Specifies the short rule name of the rule that triggered the events. 
-			seen: A true/false parameter indicating whether events were read/unread by the user operating the API. 
-			severities: Specifies the severity of the event (Deprecated). 
-			signed: A true/false parameter indicating if the event is signed. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			updateEventsRequest: updateEventsRequest. 
-			archive: A true/false parameter indicating whether to update archived events. 
-			classification: Specifies the event classification. 
-			comment: Specifies a user-defined string attached to the event. 
-			familyName: Specifies the event family name. 
-			forceUnmute: Indicates whether to force archive even if the event is muted. 
-			handle: A true/false parameter indicating update the events handled/unhandled. 
-			malwareType: Specifies the event malware type. 
-			mute: A true/false parameter indicating whether to mute events. 
-			muteDuration: Specifies the mute duration time. 
-			read: A true/false parameter indicating whether the events are read/unread by the user operating the API. 
-			threatName: Specifies the event threat name. 
+			actions (dict): Specifies the action of the event.
+			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
+			archived (bool): A true/false parameter indicating whether to include only archived events.
+			classifications (dict): Specifies the classification of the event.
+			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
+			destinations (dict): Specifies the connection destination(s) of the events.
+			device (str): Specifies the device name where the events occurred.
+			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
+			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			eventIds (dict): Specifies the required event IDs.
+			eventType (dict): Specifies the type of the event.
+			expired (bool): A true/false parameter indicating whether to include only expired events.
+			fileHash (str): Specifies the hash signature of the main process of the event.
+			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
+			firstSeenFrom (str): Specifies the from date when the event was first seen.
+			firstSeenTo (str): Specifies the to date when the event was first seen.
+			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
+			lastSeenFrom (str): Specifies the from date when the event was last seen.
+			lastSeenTo (str): Specifies the to date when the event was last seen.
+			loggedUser (str): Specifies the logged user.
+			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			muted (bool): A true/false parameter indicating if the event is muted.
+			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			paths (dict): Specifies the paths of the processes related to the event.
+			process (str): Specifies the main process of the event.
+			rule (str): Specifies the short rule name of the rule that triggered the events.
+			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
+			severities (dict): Specifies the severity of the event (Deprecated).
+			signed (bool): A true/false parameter indicating if the event is signed.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			updateEventsRequest (Object): Check 'updateEventsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("insert_events", locals())
+
 		url = '/management-rest/events'
 		url_params = []
 		if actions:
-			url_params.append('actions=' + str(actions))
+			url_params.append('actions=' + actions)
 		if applicationControl:
-			url_params.append('applicationControl=' + str(applicationControl))
+			url_params.append('applicationControl=' + applicationControl)
 		if archived:
-			url_params.append('archived=' + str(archived))
+			url_params.append('archived=' + archived)
 		if classifications:
-			url_params.append('classifications=' + str(classifications))
+			url_params.append('classifications=' + classifications)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceControl:
-			url_params.append('deviceControl=' + str(deviceControl))
+			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
-			url_params.append('deviceIps=' + str(deviceIps))
+			url_params.append('deviceIps=' + deviceIps)
 		if eventIds:
-			url_params.append('eventIds=' + str(eventIds))
+			url_params.append('eventIds=' + eventIds)
 		if eventType:
-			url_params.append('eventType=' + str(eventType))
+			url_params.append('eventType=' + eventType)
 		if expired:
-			url_params.append('expired=' + str(expired))
+			url_params.append('expired=' + expired)
 		if fileHash:
-			url_params.append('fileHash=' + str(fileHash))
+			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
+			url_params.append('firstSeen=' + firstSeen)
 		if firstSeenFrom:
-			url_params.append('firstSeenFrom=' + str(firstSeenFrom))
+			url_params.append('firstSeenFrom=' + firstSeenFrom)
 		if firstSeenTo:
-			url_params.append('firstSeenTo=' + str(firstSeenTo))
+			url_params.append('firstSeenTo=' + firstSeenTo)
 		if handled:
-			url_params.append('handled=' + str(handled))
+			url_params.append('handled=' + handled)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeen:
-			url_params.append('lastSeen=' + str(lastSeen))
+			url_params.append('lastSeen=' + lastSeen)
 		if lastSeenFrom:
-			url_params.append('lastSeenFrom=' + str(lastSeenFrom))
+			url_params.append('lastSeenFrom=' + lastSeenFrom)
 		if lastSeenTo:
-			url_params.append('lastSeenTo=' + str(lastSeenTo))
+			url_params.append('lastSeenTo=' + lastSeenTo)
 		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
+			url_params.append('loggedUser=' + loggedUser)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if muted:
-			url_params.append('muted=' + str(muted))
+			url_params.append('muted=' + muted)
 		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
+			url_params.append('operatingSystems=' + operatingSystems)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if paths:
-			url_params.append('paths=' + str(paths))
+			url_params.append('paths=' + paths)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rule:
-			url_params.append('rule=' + str(rule))
+			url_params.append('rule=' + rule)
 		if seen:
-			url_params.append('seen=' + str(seen))
+			url_params.append('seen=' + seen)
 		if severities:
-			url_params.append('severities=' + str(severities))
+			url_params.append('severities=' + severities)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
+
 		updateEventsRequest = {
-			'archive': archive,
-			'classification': classification,
-			'comment': comment,
-			'familyName': familyName,
-			'forceUnmute': forceUnmute,
-			'handle': handle,
-			'malwareType': malwareType,
-			'mute': mute,
-			'muteDuration': muteDuration,
-			'read': read,
-			'threatName': threatName
+			"archive": archive,
+			"classification": classification,
+			"comment": comment,
+			"familyName": familyName,
+			"forceUnmute": forceUnmute,
+			"handle": handle,
+			"malwareType": malwareType,
+			"mute": mute,
+			"muteDuration": muteDuration,
+			"read": read,
+			"threatName": threatName,
 		}
 		return fortiedr_connection.insert(url, updateEventsRequest)
 
-	def delete_events(self, actions :dict = None, applicationControl :bool = None, archived :bool = None, classifications :dict = None, collectorGroups :dict = None, deleteAll :bool = None, destinations :dict = None, device :str = None, deviceControl :bool = None, deviceIps :dict = None, eventIds :dict = None, eventType :dict = None, expired :bool = None, fileHash :str = None, firstSeen :str = None, firstSeenFrom :str = None, firstSeenTo :str = None, handled :bool = None, itemsPerPage :int = None, lastSeen :str = None, lastSeenFrom :str = None, lastSeenTo :str = None, loggedUser :str = None, macAddresses :dict = None, muted :bool = None, operatingSystems :dict = None, organization :str = None, pageNumber :int = None, paths :dict = None, process :str = None, rule :str = None, seen :bool = None, severities :dict = None, signed :bool = None, sorting :str = None, strictMode :bool = None) -> tuple[bool, None]:
-
+	def delete_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, deleteAll: bool = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, None]:
 		'''
-		class Events
-		Description: This API call updates the read/unread, handled/unhandled or archived/unarchived state of an event. The output of this call is a message indicating whether the update succeeded or failed.
-
-		Args:
-			actions: Specifies the action of the event. 
-			applicationControl: A true/false parameter indicating whether to include only application control events. 
-			archived: A true/false parameter indicating whether to include only archived events. 
-			classifications: Specifies the classification of the event. 
-			collectorGroups: Specifies the collector groups whose collector reported the events. 
-			deleteAll: A true/false parameter indicating if all events should be deleted. 
-			destinations: Specifies the connection destination(s) of the events. 
-			device: Specifies the device name where the events occurred. 
-			deviceControl: A true/false parameter indicating whether to include only device control events. 
-			deviceIps: Specifies the IPs of the devices where the event occurred. 
-			eventIds: Specifies the required event IDs. 
-			eventType: Specifies the type of the event. 
-			expired: A true/false parameter indicating whether to include only expired events. 
-			fileHash: Specifies the hash signature of the main process of the event. 
-			firstSeen:  Specifies the date when the event was first seen (Deprecated). 
-			firstSeenFrom: Specifies the from date when the event was first seen. 
-			firstSeenTo: Specifies the to date when the event was first seen. 
-			handled:  A true/false parameter indicating whether events were handled/unhandled. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeen:  Specifies the date when the event was last seen (Deprecated). 
-			lastSeenFrom: Specifies the from date when the event was last seen. 
-			lastSeenTo: Specifies the to date when the event was last seen. 
-			loggedUser: Specifies the logged user. 
-			macAddresses: Specifies the mac addresses where the event occurred. 
-			muted: A true/false parameter indicating if the event is muted. 
-			operatingSystems: Specifies the operating system of the devices where the events occurred. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			paths: Specifies the paths of the processes related to the event. 
-			process: Specifies the main process of the event. 
-			rule: Specifies the short rule name of the rule that triggered the events. 
-			seen: A true/false parameter indicating whether events were read/unread by the user operating the API. 
-			severities: Specifies the severity of the event (Deprecated). 
-			signed: A true/false parameter indicating if the event is signed. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+		Class Events
+		Description: This API call delete events.
+        
+		Args:
+			actions (dict): Specifies the action of the event.
+			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
+			archived (bool): A true/false parameter indicating whether to include only archived events.
+			classifications (dict): Specifies the classification of the event.
+			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
+			deleteAll (bool): A true/false parameter indicating if all events should be deleted.
+			destinations (dict): Specifies the connection destination(s) of the events.
+			device (str): Specifies the device name where the events occurred.
+			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
+			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			eventIds (dict): Specifies the required event IDs.
+			eventType (dict): Specifies the type of the event.
+			expired (bool): A true/false parameter indicating whether to include only expired events.
+			fileHash (str): Specifies the hash signature of the main process of the event.
+			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
+			firstSeenFrom (str): Specifies the from date when the event was first seen.
+			firstSeenTo (str): Specifies the to date when the event was first seen.
+			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
+			lastSeenFrom (str): Specifies the from date when the event was last seen.
+			lastSeenTo (str): Specifies the to date when the event was last seen.
+			loggedUser (str): Specifies the logged user.
+			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			muted (bool): A true/false parameter indicating if the event is muted.
+			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			paths (dict): Specifies the paths of the processes related to the event.
+			process (str): Specifies the main process of the event.
+			rule (str): Specifies the short rule name of the rule that triggered the events.
+			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
+			severities (dict): Specifies the severity of the event (Deprecated).
+			signed (bool): A true/false parameter indicating if the event is signed.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_events", locals())
+
 		url = '/management-rest/events'
 		url_params = []
 		if actions:
-			url_params.append('actions=' + str(actions))
+			url_params.append('actions=' + actions)
 		if applicationControl:
-			url_params.append('applicationControl=' + str(applicationControl))
+			url_params.append('applicationControl=' + applicationControl)
 		if archived:
-			url_params.append('archived=' + str(archived))
+			url_params.append('archived=' + archived)
 		if classifications:
-			url_params.append('classifications=' + str(classifications))
+			url_params.append('classifications=' + classifications)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if deleteAll:
-			url_params.append('deleteAll=' + str(deleteAll))
+			url_params.append('deleteAll=' + deleteAll)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceControl:
-			url_params.append('deviceControl=' + str(deviceControl))
+			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
-			url_params.append('deviceIps=' + str(deviceIps))
+			url_params.append('deviceIps=' + deviceIps)
 		if eventIds:
-			url_params.append('eventIds=' + str(eventIds))
+			url_params.append('eventIds=' + eventIds)
 		if eventType:
-			url_params.append('eventType=' + str(eventType))
+			url_params.append('eventType=' + eventType)
 		if expired:
-			url_params.append('expired=' + str(expired))
+			url_params.append('expired=' + expired)
 		if fileHash:
-			url_params.append('fileHash=' + str(fileHash))
+			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
+			url_params.append('firstSeen=' + firstSeen)
 		if firstSeenFrom:
-			url_params.append('firstSeenFrom=' + str(firstSeenFrom))
+			url_params.append('firstSeenFrom=' + firstSeenFrom)
 		if firstSeenTo:
-			url_params.append('firstSeenTo=' + str(firstSeenTo))
+			url_params.append('firstSeenTo=' + firstSeenTo)
 		if handled:
-			url_params.append('handled=' + str(handled))
+			url_params.append('handled=' + handled)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeen:
-			url_params.append('lastSeen=' + str(lastSeen))
+			url_params.append('lastSeen=' + lastSeen)
 		if lastSeenFrom:
-			url_params.append('lastSeenFrom=' + str(lastSeenFrom))
+			url_params.append('lastSeenFrom=' + lastSeenFrom)
 		if lastSeenTo:
-			url_params.append('lastSeenTo=' + str(lastSeenTo))
+			url_params.append('lastSeenTo=' + lastSeenTo)
 		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
+			url_params.append('loggedUser=' + loggedUser)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if muted:
-			url_params.append('muted=' + str(muted))
+			url_params.append('muted=' + muted)
 		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
+			url_params.append('operatingSystems=' + operatingSystems)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if paths:
-			url_params.append('paths=' + str(paths))
+			url_params.append('paths=' + paths)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rule:
-			url_params.append('rule=' + str(rule))
+			url_params.append('rule=' + rule)
 		if seen:
-			url_params.append('seen=' + str(seen))
+			url_params.append('seen=' + seen)
 		if severities:
-			url_params.append('severities=' + str(severities))
+			url_params.append('severities=' + severities)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def count_events(self, actions :dict = None, applicationControl :bool = None, archived :bool = None, classifications :dict = None, collectorGroups :dict = None, destinations :dict = None, device :str = None, deviceControl :bool = None, deviceIps :dict = None, eventIds :dict = None, eventType :dict = None, expired :bool = None, fileHash :str = None, firstSeen :str = None, firstSeenFrom :str = None, firstSeenTo :str = None, handled :bool = None, itemsPerPage :int = None, lastSeen :str = None, lastSeenFrom :str = None, lastSeenTo :str = None, loggedUser :str = None, macAddresses :dict = None, muted :bool = None, operatingSystems :dict = None, organization :str = None, pageNumber :int = None, paths :dict = None, process :str = None, rule :str = None, seen :bool = None, severities :dict = None, signed :bool = None, sorting :str = None, strictMode :bool = None) -> tuple[bool, int]:
-
+	def count_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, int]:
 		'''
-		class Events
+		Class Events
 		Description: Count Events.
-
+        
 		Args:
-			actions: Specifies the action of the event. 
-			applicationControl: A true/false parameter indicating whether to include only application control events. 
-			archived: A true/false parameter indicating whether to include only archived events. 
-			classifications: Specifies the classification of the event. 
-			collectorGroups: Specifies the collector groups whose collector reported the events. 
-			destinations: Specifies the connection destination(s) of the events. 
-			device: Specifies the device name where the events occurred. 
-			deviceControl: A true/false parameter indicating whether to include only device control events. 
-			deviceIps: Specifies the IPs of the devices where the event occurred. 
-			eventIds: Specifies the required event IDs. 
-			eventType: Specifies the type of the event. 
-			expired: A true/false parameter indicating whether to include only expired events. 
-			fileHash: Specifies the hash signature of the main process of the event. 
-			firstSeen:  Specifies the date when the event was first seen (Deprecated). 
-			firstSeenFrom: Specifies the from date when the event was first seen. 
-			firstSeenTo: Specifies the to date when the event was first seen. 
-			handled:  A true/false parameter indicating whether events were handled/unhandled. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeen:  Specifies the date when the event was last seen (Deprecated). 
-			lastSeenFrom: Specifies the from date when the event was last seen. 
-			lastSeenTo: Specifies the to date when the event was last seen. 
-			loggedUser: Specifies the logged user. 
-			macAddresses: Specifies the mac addresses where the event occurred. 
-			muted: A true/false parameter indicating if the event is muted. 
-			operatingSystems: Specifies the operating system of the devices where the events occurred. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			paths: Specifies the paths of the processes related to the event. 
-			process: Specifies the main process of the event. 
-			rule: Specifies the short rule name of the rule that triggered the events. 
-			seen: A true/false parameter indicating whether events were read/unread by the user operating the API. 
-			severities: Specifies the severity of the event (Deprecated). 
-			signed: A true/false parameter indicating if the event is signed. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+			actions (dict): Specifies the action of the event.
+			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
+			archived (bool): A true/false parameter indicating whether to include only archived events.
+			classifications (dict): Specifies the classification of the event.
+			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
+			destinations (dict): Specifies the connection destination(s) of the events.
+			device (str): Specifies the device name where the events occurred.
+			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
+			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			eventIds (dict): Specifies the required event IDs.
+			eventType (dict): Specifies the type of the event.
+			expired (bool): A true/false parameter indicating whether to include only expired events.
+			fileHash (str): Specifies the hash signature of the main process of the event.
+			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
+			firstSeenFrom (str): Specifies the from date when the event was first seen.
+			firstSeenTo (str): Specifies the to date when the event was first seen.
+			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
+			lastSeenFrom (str): Specifies the from date when the event was last seen.
+			lastSeenTo (str): Specifies the to date when the event was last seen.
+			loggedUser (str): Specifies the logged user.
+			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			muted (bool): A true/false parameter indicating if the event is muted.
+			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			paths (dict): Specifies the paths of the processes related to the event.
+			process (str): Specifies the main process of the event.
+			rule (str): Specifies the short rule name of the rule that triggered the events.
+			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
+			severities (dict): Specifies the severity of the event (Deprecated).
+			signed (bool): A true/false parameter indicating if the event is signed.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			int
-
 		'''
+		validate_params("count_events", locals())
+
 		url = '/management-rest/events/count-events'
 		url_params = []
 		if actions:
-			url_params.append('actions=' + str(actions))
+			url_params.append('actions=' + actions)
 		if applicationControl:
-			url_params.append('applicationControl=' + str(applicationControl))
+			url_params.append('applicationControl=' + applicationControl)
 		if archived:
-			url_params.append('archived=' + str(archived))
+			url_params.append('archived=' + archived)
 		if classifications:
-			url_params.append('classifications=' + str(classifications))
+			url_params.append('classifications=' + classifications)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceControl:
-			url_params.append('deviceControl=' + str(deviceControl))
+			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
-			url_params.append('deviceIps=' + str(deviceIps))
+			url_params.append('deviceIps=' + deviceIps)
 		if eventIds:
-			url_params.append('eventIds=' + str(eventIds))
+			url_params.append('eventIds=' + eventIds)
 		if eventType:
-			url_params.append('eventType=' + str(eventType))
+			url_params.append('eventType=' + eventType)
 		if expired:
-			url_params.append('expired=' + str(expired))
+			url_params.append('expired=' + expired)
 		if fileHash:
-			url_params.append('fileHash=' + str(fileHash))
+			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
+			url_params.append('firstSeen=' + firstSeen)
 		if firstSeenFrom:
-			url_params.append('firstSeenFrom=' + str(firstSeenFrom))
+			url_params.append('firstSeenFrom=' + firstSeenFrom)
 		if firstSeenTo:
-			url_params.append('firstSeenTo=' + str(firstSeenTo))
+			url_params.append('firstSeenTo=' + firstSeenTo)
 		if handled:
-			url_params.append('handled=' + str(handled))
+			url_params.append('handled=' + handled)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeen:
-			url_params.append('lastSeen=' + str(lastSeen))
+			url_params.append('lastSeen=' + lastSeen)
 		if lastSeenFrom:
-			url_params.append('lastSeenFrom=' + str(lastSeenFrom))
+			url_params.append('lastSeenFrom=' + lastSeenFrom)
 		if lastSeenTo:
-			url_params.append('lastSeenTo=' + str(lastSeenTo))
+			url_params.append('lastSeenTo=' + lastSeenTo)
 		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
+			url_params.append('loggedUser=' + loggedUser)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if muted:
-			url_params.append('muted=' + str(muted))
+			url_params.append('muted=' + muted)
 		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
+			url_params.append('operatingSystems=' + operatingSystems)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if paths:
-			url_params.append('paths=' + str(paths))
+			url_params.append('paths=' + paths)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rule:
-			url_params.append('rule=' + str(rule))
+			url_params.append('rule=' + rule)
 		if seen:
-			url_params.append('seen=' + str(seen))
+			url_params.append('seen=' + seen)
 		if severities:
-			url_params.append('severities=' + str(severities))
+			url_params.append('severities=' + severities)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def create_exception(self, allCollectorGroups :bool = None, allDestinations :bool = None, allOrganizations :bool = None, allUsers :bool = None, collectorGroups :dict = None, comment :str = None, destinations :dict = None, eventId :int = None, exceptionId :int = None, forceCreate :bool = None, organization :str = None, users :dict = None, useAnyPath: object = None, useInException: object = None, wildcardFiles: object = None, wildcardPaths: object = None) -> tuple[bool, str]:
-
+	def create_exception(self, allCollectorGroups: bool = None, allDestinations: bool = None, allOrganizations: bool = None, allUsers: bool = None, collectorGroups: dict = None, comment: str = None, destinations: dict = None, eventId: int = None, exceptionId: int = None, useAnyPath: object = None, useInException: object = None, wildcardFiles: object = None, wildcardPaths: object = None, forceCreate: bool = None, organization: str = None, users: dict = None) -> tuple[bool, str]:
 		'''
-		class Events
+		Class Events
 		Description: This API call adds an exception to a specific event. The output of this call is a message indicating whether the creation of the exception .
-
+        
 		Args:
-			allCollectorGroups: A true/false parameter indicating whether the exception should be applied to all collector groups. When not used, all collector groups are selected. 
-			allDestinations: A true/false parameter indicating whether the exception should be applied to all destinations. When not used, all destinations are selected. 
-			allOrganizations: A true/false parameter indicating whether the exception should be applied to all the organizations (tenants). This parameter is only relevant in multi-tenancy environment. This parameter is only allowed for user with Hoster privilege (general admin). 
-			allUsers: A true/false parameter indicating whether the exception should be applied to all users. When not used, all users are selected. 
-			collectorGroups: Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected. 
-			comment: Specifies a user-defined string to attach to the exception. 
-			destinations: A list of IPs to which the exception applies and/or the value all internal destinations. 
-			eventId: Specifies the event ID on which to create the exception. 
-			exceptionId: Specifies the exception ID to edit. 
-			exceptionRequest: exceptionRequest. 
-			useAnyPath: For each relevant process in each relevant rule, the user must indicate true/false to set an exception on the path that was seen in the event or for any path. 
-			useInException: For each relevant process in each relevant rule, the user must indicate true/false in order to include it in the exception. 
-			wildcardFiles: For each relevant process in each relevant rule filename, check if pattern matches the file value, and according to action (true/false) attach/remove the exception wildcard field. 
-			wildcardPaths: For each relevant process in each relevant rule path name, check if pattern matches the file value, and according to action (true/false) attach/remove the exception wildcard field. 
-			forceCreate: A true/false parameter indicating whether to create the exception, even if there are already exceptions that cover this given event. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			users: A list of users to which the exception. 
+			allCollectorGroups (bool): A true/false parameter indicating whether the exception should be applied to all collector groups. When not used, all collector groups are selected.
+			allDestinations (bool): A true/false parameter indicating whether the exception should be applied to all destinations. When not used, all destinations are selected.
+			allOrganizations (bool): A true/false parameter indicating whether the exception should be applied to all the organizations (tenants). This parameter is only relevant in multi-tenancy environment. This parameter is only allowed for user with Hoster privilege (general admin).
+			allUsers (bool): A true/false parameter indicating whether the exception should be applied to all users. When not used, all users are selected.
+			collectorGroups (dict): Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected.
+			comment (str): Specifies a user-defined string to attach to the exception.
+			destinations (dict): A list of IPs to which the exception applies and/or the value all internal destinations.
+			eventId (int): Specifies the event ID on which to create the exception.
+			exceptionId (int): Specifies the exception ID to edit.
+			exceptionRequest (Object): Check 'exceptionRequest' in the API documentation for further information.
+			forceCreate (bool): A true/false parameter indicating whether to create the exception, even if there are already exceptions that cover this given event.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			users (dict): A list of users to which the exception.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			str
-
 		'''
+		validate_params("create_exception", locals())
+
 		url = '/management-rest/events/create-exception'
 		url_params = []
 		if allCollectorGroups:
-			url_params.append('allCollectorGroups=' + str(allCollectorGroups))
+			url_params.append('allCollectorGroups=' + allCollectorGroups)
 		if allDestinations:
-			url_params.append('allDestinations=' + str(allDestinations))
+			url_params.append('allDestinations=' + allDestinations)
 		if allOrganizations:
-			url_params.append('allOrganizations=' + str(allOrganizations))
+			url_params.append('allOrganizations=' + allOrganizations)
 		if allUsers:
-			url_params.append('allUsers=' + str(allUsers))
+			url_params.append('allUsers=' + allUsers)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if comment:
-			url_params.append('comment=' + str(comment))
+			url_params.append('comment=' + comment)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if eventId:
 			url_params.append('eventId=' + str(eventId))
 		if exceptionId:
 			url_params.append('exceptionId=' + str(exceptionId))
 		if forceCreate:
-			url_params.append('forceCreate=' + str(forceCreate))
+			url_params.append('forceCreate=' + forceCreate)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if users:
-			url_params.append('users=' + str(users))
+			url_params.append('users=' + users)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
 
-	def export_raw_data_items_json(self, organization :str = None, rawItemIds :str = None) -> tuple[bool, None]:
+		exceptionRequest = {
+			"useAnyPath": useAnyPath,
+			"useInException": useInException,
+			"wildcardFiles": wildcardFiles,
+			"wildcardPaths": wildcardPaths,
+		}
+		return fortiedr_connection.upload(url, exceptionRequest)
 
+	def export_raw_data_items_json(self, organization: str = None, rawItemIds: str = None) -> tuple[bool, None]:
 		'''
-		class Events
+		Class Events
 		Description: Get event as Json format.
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			rawItemIds: Specifies the raw data item event IDs. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			rawItemIds (str): Specifies the raw data item event IDs.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("export_raw_data_items_json", locals())
+
 		url = '/management-rest/events/export-raw-data-items-json'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if rawItemIds:
-			url_params.append('rawItemIds=' + str(rawItemIds))
+			url_params.append('rawItemIds=' + rawItemIds)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.download(url)
-
-
-	def list_events(self, actions :dict = None, applicationControl :bool = None, archived :bool = None, classifications :dict = None, collectorGroups :dict = None, destinations :dict = None, device :str = None, deviceControl :bool = None, deviceIps :dict = None, eventIds :dict = None, eventType :dict = None, expired :bool = None, fileHash :str = None, firstSeen :str = None, firstSeenFrom :str = None, firstSeenTo :str = None, handled :bool = None, itemsPerPage :int = None, lastSeen :str = None, lastSeenFrom :str = None, lastSeenTo :str = None, loggedUser :str = None, macAddresses :dict = None, muted :bool = None, operatingSystems :dict = None, organization :str = None, pageNumber :int = None, paths :dict = None, process :str = None, rule :str = None, seen :bool = None, severities :dict = None, signed :bool = None, sorting :str = None, strictMode :bool = None) -> tuple[bool, dict]:
+		return fortiedr_connection.get(url)
 
+	def list_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
-		class Events
+		Class Events
 		Description: List Events.
-
+        
 		Args:
-			actions: Specifies the action of the event. 
-			applicationControl: A true/false parameter indicating whether to include only application control events. 
-			archived: A true/false parameter indicating whether to include only archived events. 
-			classifications: Specifies the classification of the event. 
-			collectorGroups: Specifies the collector groups whose collector reported the events. 
-			destinations: Specifies the connection destination(s) of the events. 
-			device: Specifies the device name where the events occurred. 
-			deviceControl: A true/false parameter indicating whether to include only device control events. 
-			deviceIps: Specifies the IPs of the devices where the event occurred. 
-			eventIds: Specifies the required event IDs. 
-			eventType: Specifies the type of the event. 
-			expired: A true/false parameter indicating whether to include only expired events. 
-			fileHash: Specifies the hash signature of the main process of the event. 
-			firstSeen:  Specifies the date when the event was first seen (Deprecated). 
-			firstSeenFrom: Specifies the from date when the event was first seen. 
-			firstSeenTo: Specifies the to date when the event was first seen. 
-			handled:  A true/false parameter indicating whether events were handled/unhandled. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeen:  Specifies the date when the event was last seen (Deprecated). 
-			lastSeenFrom: Specifies the from date when the event was last seen. 
-			lastSeenTo: Specifies the to date when the event was last seen. 
-			loggedUser: Specifies the logged user. 
-			macAddresses: Specifies the mac addresses where the event occurred. 
-			muted: A true/false parameter indicating if the event is muted. 
-			operatingSystems: Specifies the operating system of the devices where the events occurred. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			paths: Specifies the paths of the processes related to the event. 
-			process: Specifies the main process of the event. 
-			rule: Specifies the short rule name of the rule that triggered the events. 
-			seen: A true/false parameter indicating whether events were read/unread by the user operating the API. 
-			severities: Specifies the severity of the event (Deprecated). 
-			signed: A true/false parameter indicating if the event is signed. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+			actions (dict): Specifies the action of the event.
+			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
+			archived (bool): A true/false parameter indicating whether to include only archived events.
+			classifications (dict): Specifies the classification of the event.
+			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
+			destinations (dict): Specifies the connection destination(s) of the events.
+			device (str): Specifies the device name where the events occurred.
+			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
+			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			eventIds (dict): Specifies the required event IDs.
+			eventType (dict): Specifies the type of the event.
+			expired (bool): A true/false parameter indicating whether to include only expired events.
+			fileHash (str): Specifies the hash signature of the main process of the event.
+			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
+			firstSeenFrom (str): Specifies the from date when the event was first seen.
+			firstSeenTo (str): Specifies the to date when the event was first seen.
+			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
+			lastSeenFrom (str): Specifies the from date when the event was last seen.
+			lastSeenTo (str): Specifies the to date when the event was last seen.
+			loggedUser (str): Specifies the logged user.
+			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			muted (bool): A true/false parameter indicating if the event is muted.
+			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			paths (dict): Specifies the paths of the processes related to the event.
+			process (str): Specifies the main process of the event.
+			rule (str): Specifies the short rule name of the rule that triggered the events.
+			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
+			severities (dict): Specifies the severity of the event (Deprecated).
+			signed (bool): A true/false parameter indicating if the event is signed.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_events", locals())
+
 		url = '/management-rest/events/list-events'
 		url_params = []
 		if actions:
-			url_params.append('actions=' + str(actions))
+			url_params.append('actions=' + actions)
 		if applicationControl:
-			url_params.append('applicationControl=' + str(applicationControl))
+			url_params.append('applicationControl=' + applicationControl)
 		if archived:
-			url_params.append('archived=' + str(archived))
+			url_params.append('archived=' + archived)
 		if classifications:
-			url_params.append('classifications=' + str(classifications))
+			url_params.append('classifications=' + classifications)
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceControl:
-			url_params.append('deviceControl=' + str(deviceControl))
+			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
-			url_params.append('deviceIps=' + str(deviceIps))
+			url_params.append('deviceIps=' + deviceIps)
 		if eventIds:
-			url_params.append('eventIds=' + str(eventIds))
+			url_params.append('eventIds=' + eventIds)
 		if eventType:
-			url_params.append('eventType=' + str(eventType))
+			url_params.append('eventType=' + eventType)
 		if expired:
-			url_params.append('expired=' + str(expired))
+			url_params.append('expired=' + expired)
 		if fileHash:
-			url_params.append('fileHash=' + str(fileHash))
+			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
+			url_params.append('firstSeen=' + firstSeen)
 		if firstSeenFrom:
-			url_params.append('firstSeenFrom=' + str(firstSeenFrom))
+			url_params.append('firstSeenFrom=' + firstSeenFrom)
 		if firstSeenTo:
-			url_params.append('firstSeenTo=' + str(firstSeenTo))
+			url_params.append('firstSeenTo=' + firstSeenTo)
 		if handled:
-			url_params.append('handled=' + str(handled))
+			url_params.append('handled=' + handled)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeen:
-			url_params.append('lastSeen=' + str(lastSeen))
+			url_params.append('lastSeen=' + lastSeen)
 		if lastSeenFrom:
-			url_params.append('lastSeenFrom=' + str(lastSeenFrom))
+			url_params.append('lastSeenFrom=' + lastSeenFrom)
 		if lastSeenTo:
-			url_params.append('lastSeenTo=' + str(lastSeenTo))
+			url_params.append('lastSeenTo=' + lastSeenTo)
 		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
+			url_params.append('loggedUser=' + loggedUser)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if muted:
-			url_params.append('muted=' + str(muted))
+			url_params.append('muted=' + muted)
 		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
+			url_params.append('operatingSystems=' + operatingSystems)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if paths:
-			url_params.append('paths=' + str(paths))
+			url_params.append('paths=' + paths)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rule:
-			url_params.append('rule=' + str(rule))
+			url_params.append('rule=' + rule)
 		if seen:
-			url_params.append('seen=' + str(seen))
+			url_params.append('seen=' + seen)
 		if severities:
-			url_params.append('severities=' + str(severities))
+			url_params.append('severities=' + severities)
 		if signed:
-			url_params.append('signed=' + str(signed))
+			url_params.append('signed=' + signed)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_raw_data_items(self, eventId : int, collectorGroups :dict = None, destinations :dict = None, device :str = None, deviceIps :dict = None, firstSeen :str = None, firstSeenFrom :str = None, firstSeenTo :str = None, fullDataRequested :bool = None, itemsPerPage :int = None, lastSeen :str = None, lastSeenFrom :str = None, lastSeenTo :str = None, loggedUser :str = None, organization :str = None, pageNumber :int = None, rawEventIds :dict = None, sorting :str = None, strictMode :bool = None) -> tuple[bool, dict]:
-
+	def list_raw_data_items(self, eventId: int, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceIps: dict = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, fullDataRequested: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, organization: str = None, pageNumber: int = None, rawEventIds: dict = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
-		class Events
+		Class Events
 		Description: List raw data items.
-
+        
 		Args:
-			collectorGroups: Specifies the collector groups whose collector reported the raw events. 
-			destinations: Specifies the connection destination(s) of the events. 
-			device: Specifies the name of the device where the raw event occurred. 
-			deviceIps: Specifies the IPs of the devices where the event occurred. 
-			eventId: Specifies the ID of the event that holds the raw data items. 
-			firstSeen: Specifies the date when the raw data item was first seen (Deprecated). 
-			firstSeenFrom: Specifies the from date when the raw data item was first seen. 
-			firstSeenTo: Specifies the to date when the raw data item was first seen. 
-			fullDataRequested: A true/false parameter indicating whether to include the event internal information. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeen: Specifies the date when the raw data item was last seen (Deprecated). 
-			lastSeenFrom: Specifies the from date when the raw data item was last seen. 
-			lastSeenTo: Specifies the to date when the raw data item was last seen. 
-			loggedUser: Specifies the logged user. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			rawEventIds: Specifies the list of raw data item event IDs. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+			collectorGroups (dict): Specifies the collector groups whose collector reported the raw events.
+			destinations (dict): Specifies the connection destination(s) of the events.
+			device (str): Specifies the name of the device where the raw event occurred.
+			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			eventId (int): Specifies the ID of the event that holds the raw data items.
+			firstSeen (str): Specifies the date when the raw data item was first seen (Deprecated).
+			firstSeenFrom (str): Specifies the from date when the raw data item was first seen.
+			firstSeenTo (str): Specifies the to date when the raw data item was first seen.
+			fullDataRequested (bool): A true/false parameter indicating whether to include the event internal information.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeen (str): Specifies the date when the raw data item was last seen (Deprecated).
+			lastSeenFrom (str): Specifies the from date when the raw data item was last seen.
+			lastSeenTo (str): Specifies the to date when the raw data item was last seen.
+			loggedUser (str): Specifies the logged user.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			rawEventIds (dict): Specifies the list of raw data item event IDs.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_raw_data_items", locals())
+
 		url = '/management-rest/events/list-raw-data-items'
 		url_params = []
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if destinations:
-			url_params.append('destinations=' + str(destinations))
+			url_params.append('destinations=' + destinations)
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceIps:
-			url_params.append('deviceIps=' + str(deviceIps))
+			url_params.append('deviceIps=' + deviceIps)
 		if eventId:
 			url_params.append('eventId=' + str(eventId))
 		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
+			url_params.append('firstSeen=' + firstSeen)
 		if firstSeenFrom:
-			url_params.append('firstSeenFrom=' + str(firstSeenFrom))
+			url_params.append('firstSeenFrom=' + firstSeenFrom)
 		if firstSeenTo:
-			url_params.append('firstSeenTo=' + str(firstSeenTo))
+			url_params.append('firstSeenTo=' + firstSeenTo)
 		if fullDataRequested:
-			url_params.append('fullDataRequested=' + str(fullDataRequested))
+			url_params.append('fullDataRequested=' + fullDataRequested)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeen:
-			url_params.append('lastSeen=' + str(lastSeen))
+			url_params.append('lastSeen=' + lastSeen)
 		if lastSeenFrom:
-			url_params.append('lastSeenFrom=' + str(lastSeenFrom))
+			url_params.append('lastSeenFrom=' + lastSeenFrom)
 		if lastSeenTo:
-			url_params.append('lastSeenTo=' + str(lastSeenTo))
+			url_params.append('lastSeenTo=' + lastSeenTo)
 		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
+			url_params.append('loggedUser=' + loggedUser)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if rawEventIds:
-			url_params.append('rawEventIds=' + str(rawEventIds))
+			url_params.append('rawEventIds=' + rawEventIds)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 class Exceptions:
 	'''This API call outputs all exceptions in the system'''
 
-	def create_or_edit_exception(self, confirmEdit :bool = None, exceptionJSON :str = None, organization :str = None) -> tuple[bool, int]:
-
+	def create_or_edit_exception(self, confirmEdit: bool = None, exceptionJSON: str = None, organization: str = None) -> tuple[bool, int]:
 		'''
-		class Exceptions
+		Class Exceptions
 		Description: This API call creates a new exception or updates an existing exception based on the given exception JSON body parameter.
-
+        
 		Args:
-			confirmEdit: Confirm editing an existing exception in case of providing an exception ID in the body JSON. By default confirmEdit is false. 
-			exceptionJSON: exceptionJSON. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			confirmEdit (bool): Confirm editing an existing exception in case of providing an exception ID in the body JSON. By default confirmEdit is false.
+			exceptionJSON (str): exceptionJSON.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			int
-
 		'''
+		validate_params("create_or_edit_exception", locals())
+
 		url = '/management-rest/exceptions/create-or-edit-exception'
 		url_params = []
 		if confirmEdit:
-			url_params.append('confirmEdit=' + str(confirmEdit))
+			url_params.append('confirmEdit=' + confirmEdit)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def delete(self, collectorGroups :dict = None, comment :str = None, createdAfter :str = None, createdBefore :str = None, deleteAll :bool = None, destination :str = None, exceptionId :int = None, exceptionIds :dict = None, organization :str = None, path :str = None, process :str = None, rules :dict = None, updatedAfter :str = None, updatedBefore :str = None, user :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, exceptionJSON)
 
+	def delete(self, collectorGroups: dict = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, deleteAll: bool = None, destination: str = None, exceptionId: int = None, exceptionIds: dict = None, organization: str = None, path: str = None, process: str = None, rules: dict = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, None]:
 		'''
-		class Exceptions
+		Class Exceptions
 		Description: Delete exceptions.
-
+        
 		Args:
-			collectorGroups: Specifies the list of all the collector groups to which the exception applied. 
-			comment: Specifies a comment attach to the exception. 
-			createdAfter: Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			createdBefore: Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			deleteAll: A true/false parameter indicating if all exception should be deleted. 
-			destination: Specifies a destination IP of the exception. 
-			exceptionId: Specifies the required exception ID. 
-			exceptionIds: Specifies a list of exception ids. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			path: Specifies the path of the exception. 
-			process: Specifies the process of the exception. 
-			rules: Specifies a list of rule names. 
-			updatedAfter: Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			updatedBefore: Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			user: Specifies a user of the exception. 
+			collectorGroups (dict): Specifies the list of all the collector groups to which the exception applied.
+			comment (str): Specifies a comment attach to the exception.
+			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			deleteAll (bool): A true/false parameter indicating if all exception should be deleted.
+			destination (str): Specifies a destination IP of the exception.
+			exceptionId (int): Specifies the required exception ID.
+			exceptionIds (dict): Specifies a list of exception ids.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			path (str): Specifies the path of the exception.
+			process (str): Specifies the process of the exception.
+			rules (dict): Specifies a list of rule names.
+			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			user (str): Specifies a user of the exception.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete", locals())
+
 		url = '/management-rest/exceptions/delete'
 		url_params = []
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if comment:
-			url_params.append('comment=' + str(comment))
+			url_params.append('comment=' + comment)
 		if createdAfter:
-			url_params.append('createdAfter=' + str(createdAfter))
+			url_params.append('createdAfter=' + createdAfter)
 		if createdBefore:
-			url_params.append('createdBefore=' + str(createdBefore))
+			url_params.append('createdBefore=' + createdBefore)
 		if deleteAll:
-			url_params.append('deleteAll=' + str(deleteAll))
+			url_params.append('deleteAll=' + deleteAll)
 		if destination:
-			url_params.append('destination=' + str(destination))
+			url_params.append('destination=' + destination)
 		if exceptionId:
 			url_params.append('exceptionId=' + str(exceptionId))
 		if exceptionIds:
-			url_params.append('exceptionIds=' + str(exceptionIds))
+			url_params.append('exceptionIds=' + exceptionIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if path:
-			url_params.append('path=' + str(path))
+			url_params.append('path=' + path)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rules:
-			url_params.append('rules=' + str(rules))
+			url_params.append('rules=' + rules)
 		if updatedAfter:
-			url_params.append('updatedAfter=' + str(updatedAfter))
+			url_params.append('updatedAfter=' + updatedAfter)
 		if updatedBefore:
-			url_params.append('updatedBefore=' + str(updatedBefore))
+			url_params.append('updatedBefore=' + updatedBefore)
 		if user:
-			url_params.append('user=' + str(user))
+			url_params.append('user=' + user)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def get_event_exceptions(self, eventId : int, organization :str = None) -> tuple[bool, dict]:
-
+	def get_event_exceptions(self, eventId: int, organization: str = None) -> tuple[bool, list]:
 		'''
-		class Exceptions
+		Class Exceptions
 		Description: Show exceptions.
-
+        
 		Args:
-			eventId: Specifies the required event ID. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			eventId (int): Specifies the required event ID.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("get_event_exceptions", locals())
+
 		url = '/management-rest/exceptions/get-event-exceptions'
 		url_params = []
 		if eventId:
 			url_params.append('eventId=' + str(eventId))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_exceptions(self, collectorGroups :dict = None, comment :str = None, createdAfter :str = None, createdBefore :str = None, destination :str = None, exceptionIds :dict = None, organization :str = None, path :str = None, process :str = None, rules :dict = None, updatedAfter :str = None, updatedBefore :str = None, user :str = None) -> tuple[bool, dict]:
-
+	def list_exceptions(self, collectorGroups: dict = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, destination: str = None, exceptionIds: dict = None, organization: str = None, path: str = None, process: str = None, rules: dict = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, list]:
 		'''
-		class Exceptions
+		Class Exceptions
 		Description: List of exceptions.
-
+        
 		Args:
-			collectorGroups: Specifies the list of all the collector groups to which the exception applied. 
-			comment: Specifies a comment attach to the exception. 
-			createdAfter: Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			createdBefore: Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			destination: Specifies a destination IP of the exception. 
-			exceptionIds: Specifies a list of exception ids. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			path: Specifies the path of the exception. 
-			process: Specifies the process of the exception. 
-			rules: Specifies a list of rule names. 
-			updatedAfter: Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			updatedBefore: Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format. 
-			user: Specifies a user of the exception. 
+			collectorGroups (dict): Specifies the list of all the collector groups to which the exception applied.
+			comment (str): Specifies a comment attach to the exception.
+			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			destination (str): Specifies a destination IP of the exception.
+			exceptionIds (dict): Specifies a list of exception ids.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			path (str): Specifies the path of the exception.
+			process (str): Specifies the process of the exception.
+			rules (dict): Specifies a list of rule names.
+			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
+			user (str): Specifies a user of the exception.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_exceptions", locals())
+
 		url = '/management-rest/exceptions/list-exceptions'
 		url_params = []
 		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
+			url_params.append('collectorGroups=' + collectorGroups)
 		if comment:
-			url_params.append('comment=' + str(comment))
+			url_params.append('comment=' + comment)
 		if createdAfter:
-			url_params.append('createdAfter=' + str(createdAfter))
+			url_params.append('createdAfter=' + createdAfter)
 		if createdBefore:
-			url_params.append('createdBefore=' + str(createdBefore))
+			url_params.append('createdBefore=' + createdBefore)
 		if destination:
-			url_params.append('destination=' + str(destination))
+			url_params.append('destination=' + destination)
 		if exceptionIds:
-			url_params.append('exceptionIds=' + str(exceptionIds))
+			url_params.append('exceptionIds=' + exceptionIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if path:
-			url_params.append('path=' + str(path))
+			url_params.append('path=' + path)
 		if process:
-			url_params.append('process=' + str(process))
+			url_params.append('process=' + process)
 		if rules:
-			url_params.append('rules=' + str(rules))
+			url_params.append('rules=' + rules)
 		if updatedAfter:
-			url_params.append('updatedAfter=' + str(updatedAfter))
+			url_params.append('updatedAfter=' + updatedAfter)
 		if updatedBefore:
-			url_params.append('updatedBefore=' + str(updatedBefore))
+			url_params.append('updatedBefore=' + updatedBefore)
 		if user:
-			url_params.append('user=' + str(user))
+			url_params.append('user=' + user)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-class Exclusions:
-	'''API to create EDR exclusions.'''
 class Forensics:
 	'''The Forensics module facilitates deep analysis into the actual internals of the communicating devices operating system that led up to an event.'''
 
-	def get_event_file(self, rawEventId : int, disk :bool = None, endRange :str = None, filePaths :dict = None, memory :bool = None, organization :str = None, processId :int = None, startRange :str = None) -> tuple[bool, None]:
-
+	def get_event_file(self, rawEventId: int, disk: bool = None, endRange: str = None, filePaths: dict = None, memory: bool = None, organization: str = None, processId: int = None, startRange: str = None) -> tuple[bool, None]:
 		'''
-		class Forensics
+		Class Forensics
 		Description: This API call retrieves a file or memory.
-
+        
 		Args:
-			disk: A true/false parameter indicating whether find in the disk. 
-			endRange: Specifies the memory end range, in Hexadecimal format. 
-			filePaths: Specifies the list of file paths. 
-			memory: A true/false parameter indicating whether find in the memory. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			processId: Specifies the ID of the process from which to take a memory image. required for memory base action. 
-			rawEventId: Specifies the ID of the raw event on which to perform the memory retrieval. 
-			startRange: Specifies the memory start range, in Hexadecimal format. 
+			disk (bool): A true/false parameter indicating whether find in the disk.
+			endRange (str): Specifies the memory end range, in Hexadecimal format.
+			filePaths (dict): Specifies the list of file paths.
+			memory (bool): A true/false parameter indicating whether find in the memory.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			processId (int): Specifies the ID of the process from which to take a memory image. required for memory base action.
+			rawEventId (int): Specifies the ID of the raw event on which to perform the memory retrieval.
+			startRange (str): Specifies the memory start range, in Hexadecimal format.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("get_event_file", locals())
+
 		url = '/management-rest/forensics/get-event-file'
 		url_params = []
 		if disk:
-			url_params.append('disk=' + str(disk))
+			url_params.append('disk=' + disk)
 		if endRange:
-			url_params.append('endRange=' + str(endRange))
+			url_params.append('endRange=' + endRange)
 		if filePaths:
-			url_params.append('filePaths=' + str(filePaths))
+			url_params.append('filePaths=' + filePaths)
 		if memory:
-			url_params.append('memory=' + str(memory))
+			url_params.append('memory=' + memory)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if processId:
 			url_params.append('processId=' + str(processId))
 		if rawEventId:
 			url_params.append('rawEventId=' + str(rawEventId))
 		if startRange:
-			url_params.append('startRange=' + str(startRange))
+			url_params.append('startRange=' + startRange)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.download(url)
-
-
-	def get_file(self, device : str, filePaths : dict, type : str, organization :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def get_file(self, device: str, filePaths: dict, type: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Forensics
+		Class Forensics
 		Description: This API call retrieves a file or memory.
-
+        
 		Args:
-			device: Specifies the name or id of the device to remediate. 
-			filePaths: Specifies the list of file paths. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			type: Specifies the device parameter type used in the request : Name or ID. 
+			device (str): Specifies the name or id of the device to remediate.
+			filePaths (dict): Specifies the list of file paths.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			type (str): Specifies the device parameter type used in the request : Name or ID.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("get_file", locals())
+
 		url = '/management-rest/forensics/get-file'
 		url_params = []
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if filePaths:
-			url_params.append('filePaths=' + str(filePaths))
+			url_params.append('filePaths=' + filePaths)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if type:
-			url_params.append('type=' + str(type))
+			url_params.append('type=' + type)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.download(url)
-
-
-	def remediate_device(self, terminatedProcessId : int, device :str = None, deviceId :int = None, executablesToRemove :dict = None, organization :str = None, persistenceDataAction :str = None, persistenceDataNewContent :str = None, persistenceDataPath :str = None, persistenceDataValueName :str = None, persistenceDataValueNewType :str = None, processName :str = None, threadId :int = None) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def remediate_device(self, terminatedProcessId: int, device: str = None, deviceId: int = None, executablesToRemove: dict = None, organization: str = None, persistenceDataAction: str = None, persistenceDataNewContent: str = None, persistenceDataPath: str = None, persistenceDataValueName: str = None, persistenceDataValueNewType: str = None, processName: str = None, threadId: int = None) -> tuple[bool, None]:
 		'''
-		class Forensics
+		Class Forensics
 		Description: This API kill process / delete file / clean persistence, File and persistence paths must be specified in a logical format.
-
+        
 		Args:
-			device: Specifies the name of the device to remediate. You must specify a value for either device or deviceId (see below). 
-			deviceId: Specifies the unique identifier (ID) of the device to remediate. You must specify a value for either deviceId or device (see above). 
-			executablesToRemove: Specifies the list of full paths of executable files (*.exe) to delete on thegiven device. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			persistenceDataAction: persistence data desired action. 
-			persistenceDataNewContent: persistence data new content. 
-			persistenceDataPath: persistence data path. 
-			persistenceDataValueName: persistence data value name. 
-			persistenceDataValueNewType: persistence data value new type. 
-			processName: Specifies the process name. 
-			terminatedProcessId: Represents the process ID to terminate on the device. 
-			threadId: Specifies the thread ID. 
+			device (str): Specifies the name of the device to remediate. You must specify a value for either device or deviceId (see below).
+			deviceId (int): Specifies the unique identifier (ID) of the device to remediate. You must specify a value for either deviceId or device (see above).
+			executablesToRemove (dict): Specifies the list of full paths of executable files (*.exe) to delete on the
+given device.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			persistenceDataAction (str): persistence data desired action.
+			persistenceDataNewContent (str): persistence data new content.
+			persistenceDataPath (str): persistence data path.
+			persistenceDataValueName (str): persistence data value name.
+			persistenceDataValueNewType (str): persistence data value new type.
+			processName (str): Specifies the process name.
+			terminatedProcessId (int): Represents the process ID to terminate on the device.
+			threadId (int): Specifies the thread ID.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("remediate_device", locals())
+
 		url = '/management-rest/forensics/remediate-device'
 		url_params = []
 		if device:
-			url_params.append('device=' + str(device))
+			url_params.append('device=' + device)
 		if deviceId:
 			url_params.append('deviceId=' + str(deviceId))
 		if executablesToRemove:
-			url_params.append('executablesToRemove=' + str(executablesToRemove))
+			url_params.append('executablesToRemove=' + executablesToRemove)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if persistenceDataAction:
-			url_params.append('persistenceDataAction=' + str(persistenceDataAction))
+			url_params.append('persistenceDataAction=' + persistenceDataAction)
 		if persistenceDataNewContent:
-			url_params.append('persistenceDataNewContent=' + str(persistenceDataNewContent))
+			url_params.append('persistenceDataNewContent=' + persistenceDataNewContent)
 		if persistenceDataPath:
-			url_params.append('persistenceDataPath=' + str(persistenceDataPath))
+			url_params.append('persistenceDataPath=' + persistenceDataPath)
 		if persistenceDataValueName:
-			url_params.append('persistenceDataValueName=' + str(persistenceDataValueName))
+			url_params.append('persistenceDataValueName=' + persistenceDataValueName)
 		if persistenceDataValueNewType:
-			url_params.append('persistenceDataValueNewType=' + str(persistenceDataValueNewType))
+			url_params.append('persistenceDataValueNewType=' + persistenceDataValueNewType)
 		if processName:
-			url_params.append('processName=' + str(processName))
+			url_params.append('processName=' + processName)
 		if terminatedProcessId:
 			url_params.append('terminatedProcessId=' + str(terminatedProcessId))
 		if threadId:
 			url_params.append('threadId=' + str(threadId))
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class HashSearch:
 	'''The Hash Search API'''
 
-	def search(self, fileHashes : dict, organization :str = None) -> tuple[bool, None]:
-
+	def search(self, fileHashes: dict, organization: str = None) -> tuple[bool, None]:
 		'''
-		class HashSearch
+		Class HashSearch
 		Description: This API enables the user to search a file hash among the current events, threat hunting repository and communicating applications that exist in the system.
-
+        
 		Args:
-			fileHashes: Specifies the list of files hashes. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			fileHashes (dict): Specifies the list of files hashes.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("search", locals())
+
 		url = '/management-rest/hash/search'
 		url_params = []
 		if fileHashes:
-			url_params.append('fileHashes=' + str(fileHashes))
+			url_params.append('fileHashes=' + fileHashes)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-class IPsets:
-	'''API to define IPs sets and use them for exceptions'''
-
-	def create_ip_set(self, include: dict, name: str, description: str = None, exclude: dict = None, organization: str = None) -> tuple[bool, None]:
+class Integrations:
+	'''API to create and test connectors.'''
 
+	def connectors_metadata(self, organization: str = None) -> tuple[bool, None]:
 		'''
-		class IPsets
-		Description: This API create IP sets in the system.
-	Use the input parameter organization=All organizations to create for all the organization. (only for Admin role.
-
+		Class Integrations
+		Description: Get connectors metadata, describing the valid values for connector fields definition and on-premise cores..
+        
 		Args:
-			ipGroupsRequest: ipGroupsRequest. 
-			description: Specifies the IP set description. 
-			exclude: List of IPs, ranges and mask that excluded in the IP set. 
-			include: Specifies List of IPs, ranges and mask that included in the IP set. 
-			name: Specifies the IP set name. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies: ��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly. ��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations. ��� each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately.. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/ip-sets/create-ip-set'
+		validate_params("connectors_metadata", locals())
+
+		url = '/management-rest/integrations/connectors-metadata'
 		url_params = []
+		if organization:
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		ipGroupsRequest = {
-			'description': description,
-			'exclude': exclude,
-			'include': include,
-			'name': name,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, ipGroupsRequest)
-
+		return fortiedr_connection.get(url)
 
-	def delete_ip_set(self, ipSets : dict, organization :str = None) -> tuple[bool, None]:
+	def create_connector(self, apiKey: str = None, connectorActions: dict = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
+		'''
+		Class Integrations
+		Description: Creates a new connector. Please note: Creation of Custom connectors/actions is not yet support..
+        
+		Args:
+			createConnectorRequest (Object): Check 'createConnectorRequest' in the API documentation for further information.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class IPsets
-		Description: This API delete IP sets from the system. Use the input parameters to filter organization.
+		validate_params("create_connector", locals())
 
+		url = '/management-rest/integrations/create-connector'
+
+		createConnectorRequest = {
+			"apiKey": apiKey,
+			"connectorActions": connectorActions,
+			"coreId": str(coreId),
+			"enabled": enabled,
+			"host": host,
+			"name": name,
+			"organization": organization,
+			"password": password,
+			"port": port,
+			"type": type,
+			"username": username,
+			"vendor": vendor,
+		}
+		return fortiedr_connection.upload(url, createConnectorRequest)
+
+	def delete_connector(self, connectorName: str, connectorType: str, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class Integrations
+		Description: Deletes a connector.
+        
 		Args:
-			ipSets: Specifies the list of IP name to delete. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			connectorName (str): Specifies the connector's name (case sensitive).
+			connectorType (str): Specifies the connector's type..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/ip-sets/delete-ip-set'
+		validate_params("delete_connector", locals())
+
+		url = '/management-rest/integrations/delete-connector'
 		url_params = []
-		if ipSets:
-			url_params.append('ipSets=' + str(ipSets))
+		if connectorName:
+			url_params.append('connectorName=' + connectorName)
+		if connectorType:
+			url_params.append('connectorType=' + connectorType)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
+	def list_connectors(self, onlyValidConnectors: bool = None, organization: str = None) -> tuple[bool, list]:
+		'''
+		Class Integrations
+		Description: List all organization connectors.
+        
+		Args:
+			onlyValidConnectors (bool): Set to true to retrieve enabled, non-failing connectors..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-	def list_ip_sets(self, ip :str = None, organization :str = None) -> tuple[bool, dict]:
-
+		Returns:
+			bool: Status of the request (True or False). 
+			list
 		'''
-		class IPsets
-		Description: This API call outputs a list of the IP sets in the system. Use the input parameters to filter the list.
+		validate_params("list_connectors", locals())
+
+		url = '/management-rest/integrations/list-connectors'
+		url_params = []
+		if onlyValidConnectors:
+			url_params.append('onlyValidConnectors=' + onlyValidConnectors)
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
 
+	def test_connector(self, connectorName: str, connectorType: str, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class Integrations
+		Description: Tests a connector.
+        
 		Args:
-			ip: Specifies the IP of the requested sets. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			connectorName (str): Specifies the connector's name (case sensitive).
+			connectorType (str): Specifies the connector's type..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/ip-sets/list-ip-sets'
+		validate_params("test_connector", locals())
+
+		url = '/management-rest/integrations/test-connector'
 		url_params = []
-		if ip:
-			url_params.append('ip=' + str(ip))
+		if connectorName:
+			url_params.append('connectorName=' + connectorName)
+		if connectorType:
+			url_params.append('connectorType=' + connectorType)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
+	def update_connector(self, apiKey: str = None, connectorActions: dict = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
+		'''
+		Class Integrations
+		Description: Updates an existing connector based on (name, type, organization). Please note: Modification of Custom connectors/actions is not yet support..
+        
+		Args:
+			updateConnectorRequest (Object): Check 'updateConnectorRequest' in the API documentation for further information.
 
-	def update_ip_set(self, include: dict, name: str, organization :str = None, description: str = None, exclude: dict = None) -> tuple[bool, None]:
-
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class IPsets
-		Description: This API update IP sets in the system. Use the input parameters to filter organization.
+		validate_params("update_connector", locals())
+
+		url = '/management-rest/integrations/update-connector'
+
+		updateConnectorRequest = {
+			"apiKey": apiKey,
+			"connectorActions": connectorActions,
+			"coreId": str(coreId),
+			"enabled": enabled,
+			"host": host,
+			"name": name,
+			"organization": organization,
+			"password": password,
+			"port": port,
+			"type": type,
+			"username": username,
+			"vendor": vendor,
+		}
+		return fortiedr_connection.insert(url, updateConnectorRequest)
 
+class SystemInventory:
+	'''The System Inventory module enables you to monitor the health of Fortinet Endpoint Protection and Response Platform components and to create Collector Groups.'''
+
+	def aggregator_logs(self, device: str = None, deviceId: int = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call retrieves a aggregator logs.
+        
 		Args:
-			ipGroupsRequest: ipGroupsRequest. 
-			description: Specifies the IP set description. 
-			exclude: List of IPs, ranges and mask that excluded in the IP set. 
-			include: Specifies List of IPs, ranges and mask that included in the IP set. 
-			name: Specifies the IP set name. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.��� each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately.. 
+			device (str): Specifies the name of the device.
+			deviceId (int): Specifies the ID of the device.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/ip-sets/update-ip-set'
+		validate_params("aggregator_logs", locals())
+
+		url = '/management-rest/inventory/aggregator-logs'
 		url_params = []
+		if device:
+			url_params.append('device=' + device)
+		if deviceId:
+			url_params.append('deviceId=' + str(deviceId))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-class Integrations:
-	'''API to create and test connectors.'''
+		return fortiedr_connection.get(url)
 
-	def connectors_metadata(self, organization :str = None) -> tuple[bool, None]:
+	def check_custom_installer(self, customInstallerID: str, ) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call for checking the results for an custom installer request and getting the installer url.
+        
+		Args:
+			customInstallerID (str): customInstallerID.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Integrations
-		Description: Get connectors metadata, describing the valid values for connector fields definition and on-premise cores..
+		validate_params("check_custom_installer", locals())
+
+		url = '/management-rest/inventory/check-custom-installer'
+		url_params = []
+		if customInstallerID:
+			url_params.append('customInstallerID=' + customInstallerID)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
 
+	def collector_logs(self, device: str = None, deviceId: int = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call retrieves a collector logs.
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			device (str): Specifies the name of the device.
+			deviceId (int): Specifies the ID of the device.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/integrations/connectors-metadata'
+		validate_params("collector_logs", locals())
+
+		url = '/management-rest/inventory/collector-logs'
 		url_params = []
+		if device:
+			url_params.append('device=' + device)
+		if deviceId:
+			url_params.append('deviceId=' + str(deviceId))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
+	def core_logs(self, device: str = None, deviceId: int = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call retrieves a core logs.
+        
+		Args:
+			device (str): Specifies the name of the device.
+			deviceId (int): Specifies the ID of the device.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-	def create_connector(self, connectorActions: dict, enabled: bool, host: str, name: str, organization: str, port: str, type: str, vendor: str, apiKey: str = None, coreId: int = None, password: str = None, username: str = None) -> tuple[bool, None]:
-
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Integrations
-		Description: Creates a new connector. Please note: Creation of Custom connectors/actions is not yet support..
+		validate_params("core_logs", locals())
 
+		url = '/management-rest/inventory/core-logs'
+		url_params = []
+		if device:
+			url_params.append('device=' + device)
+		if deviceId:
+			url_params.append('deviceId=' + str(deviceId))
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
+
+	def create_collector_group(self, name: str, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call create collector group.
+        
 		Args:
-			createConnectorRequest: createConnectorRequest. 
-			apiKey: Specifies the connector's API key (API key authentication mode). Should be empty if username and passwords are used.. 
-			connectorActions: Specifies the connector's actions' definition. Use connectors-metadata API for supported values. 
-			coreId: Specifies the ID of the connector's on-premise core. 
-			enabled: Specifies whether or not the connector is enabled.. Example: enabled=True.
-			host: Specifies the connector host address.. Example: host=127.0.0.1.
-			name: Specifies the connector name.. Example: name=Connector Name.
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			password: Specifies the connector's user's password (credentials authentication mode). Should be empty if apiKey is used.. 
-			port: Specifies the connector port.. Example: port=443.
-			type: Specifies the connector type. See /connectors-metadata for valid types.. Example: type=Firewall.
-			username: Specifies the connector's user's username (credentials authentication mode). Should be empty if apiKey is used.. 
-			vendor: Specifies the connector's vendor. See /connectors-metadata for valid values.. Example: vendor=FortiGate.
+			name (str): Collector group name.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/integrations/create-connector'
+		validate_params("create_collector_group", locals())
+
+		url = '/management-rest/inventory/create-collector-group'
 		url_params = []
+		if name:
+			url_params.append('name=' + name)
+		if organization:
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		createConnectorRequest = {
-			'apiKey': apiKey,
-			'connectorActions': connectorActions,
-			'coreId': coreId,
-			'enabled': enabled,
-			'host': host,
-			'name': name,
-			'organization': organization,
-			'password': password,
-			'port': port,
-			'type': type,
-			'username': username,
-			'vendor': vendor
-		}
-		return fortiedr_connection.send(url, createConnectorRequest)
-
+		return fortiedr_connection.upload(url)
 
-	def delete_connector(self, connectorName : str, connectorType : str, organization :str = None) -> tuple[bool, None]:
+	def create_ems_custom_installer(self, osType: str, aggregatorAddress: str = None, aggregatorPort: int = None, citrixPVS: bool = None, collectorGroup: str = None, collectorVersion: str = None, distro: str = None, is64bit: bool = None, organization: str = None, proxy: bool = None, vdi: bool = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call sends request for creating custom-installer for EMS integration.
+        
+		Args:
+			aggregatorAddress (str): Specifies the aggregator ip or dns address.
+			aggregatorPort (int): Specifies the aggregator port.
+			citrixPVS (bool): Specifies whether the collector installed with citrix in pvs mode.
+			collectorGroup (str): Specifies the requested collector group.
+			collectorVersion (str): Specifies the requested collector version.
+			distro (str): Specifies the Linux distribution. For example: CentOS_6, CentOS_7, CentOS_8, CentOS_9, Amazon, Oracle_6, Oracle_7, Oracle_8, SLES_12, SLES_15, Ubuntu_16.04, Ubuntu_18.04, Ubuntu_20.04, Ubuntu_22.04.
+			is64bit (bool): Specifies the Windows os bit version.
+			organization (str): Specifies the requested organization.
+			osType (str): Specifies the operating system type.
+			proxy (bool): Specifies the system proxy settings (Only applies to Collector versions 3.1 and above).
+			vdi (bool): Specifies the VDI (Virtual Desktop Infrastructure) installation.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Integrations
-		Description: Deletes a connector.
+		validate_params("create_ems_custom_installer", locals())
+
+		url = '/management-rest/inventory/create-ems-custom-installer'
+		url_params = []
+		if aggregatorAddress:
+			url_params.append('aggregatorAddress=' + aggregatorAddress)
+		if aggregatorPort:
+			url_params.append('aggregatorPort=' + str(aggregatorPort))
+		if citrixPVS:
+			url_params.append('citrixPVS=' + citrixPVS)
+		if collectorGroup:
+			url_params.append('collectorGroup=' + collectorGroup)
+		if collectorVersion:
+			url_params.append('collectorVersion=' + collectorVersion)
+		if distro:
+			url_params.append('distro=' + distro)
+		if is64bit:
+			url_params.append('is64bit=' + is64bit)
+		if organization:
+			url_params.append('organization=' + organization)
+		if osType:
+			url_params.append('osType=' + osType)
+		if proxy:
+			url_params.append('proxy=' + proxy)
+		if vdi:
+			url_params.append('vdi=' + vdi)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.upload(url)
 
+	def delete_collectors(self, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, confirmDeletion: bool = None, deleteAll: bool = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call deletes a Collector(s).
+        
 		Args:
-			connectorName: Specifies the connector's name (case sensitive). 
-			connectorType: Specifies the connector's type.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			cloudAccounts (dict): Specifies the list cloud account names.
+			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (dict): Specifies the list of cluster.
+			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+given groups.
+			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
+			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
+			confirmDeletion (bool): A true/false parameter indicating if to detach/delete relevant exceptions from Collector groups about to be deleted.
+			deleteAll (bool): A true/false parameter indicating if all collectors should be deleted.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
+			ips (dict): Specifies the list of IP values.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			loggedUser (str): Specifies the user that was logged when the event occurred.
+			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			versions (dict): Specifies the list of collector versions.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/integrations/delete-connector'
+		validate_params("delete_collectors", locals())
+
+		url = '/management-rest/inventory/delete-collectors'
 		url_params = []
-		if connectorName:
-			url_params.append('connectorName=' + str(connectorName))
-		if connectorType:
-			url_params.append('connectorType=' + str(connectorType))
+		if cloudAccounts:
+			url_params.append('cloudAccounts=' + cloudAccounts)
+		if cloudProviders:
+			url_params.append('cloudProviders=' + cloudProviders)
+		if clusters:
+			url_params.append('clusters=' + clusters)
+		if collectorGroups:
+			url_params.append('collectorGroups=' + collectorGroups)
+		if collectorGroupsIds:
+			url_params.append('collectorGroupsIds=' + collectorGroupsIds)
+		if collectorType:
+			url_params.append('collectorType=' + collectorType)
+		if confirmDeletion:
+			url_params.append('confirmDeletion=' + confirmDeletion)
+		if deleteAll:
+			url_params.append('deleteAll=' + deleteAll)
+		if devices:
+			url_params.append('devices=' + devices)
+		if devicesIds:
+			url_params.append('devicesIds=' + devicesIds)
+		if firstSeen:
+			url_params.append('firstSeen=' + firstSeen)
+		if hasCrashDumps:
+			url_params.append('hasCrashDumps=' + hasCrashDumps)
+		if ips:
+			url_params.append('ips=' + ips)
+		if itemsPerPage:
+			url_params.append('itemsPerPage=' + str(itemsPerPage))
+		if lastSeenEnd:
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
+		if lastSeenStart:
+			url_params.append('lastSeenStart=' + lastSeenStart)
+		if loggedUser:
+			url_params.append('loggedUser=' + loggedUser)
+		if operatingSystems:
+			url_params.append('operatingSystems=' + operatingSystems)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
+		if osFamilies:
+			url_params.append('osFamilies=' + osFamilies)
+		if pageNumber:
+			url_params.append('pageNumber=' + str(pageNumber))
+		if showExpired:
+			url_params.append('showExpired=' + showExpired)
+		if sorting:
+			url_params.append('sorting=' + sorting)
+		if states:
+			url_params.append('states=' + states)
+		if strictMode:
+			url_params.append('strictMode=' + strictMode)
+		if versions:
+			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
+	def isolate_collectors(self, devices: dict = None, devicesIds: dict = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call isolate collector functionality.
+        
+		Args:
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-	def list_connectors(self, onlyValidConnectors :bool = None, organization :str = None) -> tuple[bool, dict]:
-
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Integrations
-		Description: List all organization connectors.
+		validate_params("isolate_collectors", locals())
 
+		url = '/management-rest/inventory/isolate-collectors'
+		url_params = []
+		if devices:
+			url_params.append('devices=' + devices)
+		if devicesIds:
+			url_params.append('devicesIds=' + devicesIds)
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.insert(url)
+
+	def list_aggregators(self, ip: str = None, names: dict = None, organization: str = None, versions: dict = None) -> tuple[bool, list]:
+		'''
+		Class SystemInventory
+		Description: This API call output the list of aggregators.
+        
 		Args:
-			onlyValidConnectors: Set to true to retrieve enabled, non-failing connectors.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			ip (str): IP.
+			names (dict): List of aggregators names.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			versions (dict): List of aggregators versions.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
+			list
+		'''
+		validate_params("list_aggregators", locals())
+
+		url = '/management-rest/inventory/list-aggregators'
+		url_params = []
+		if ip:
+			url_params.append('ip=' + ip)
+		if names:
+			url_params.append('names=' + names)
+		if organization:
+			url_params.append('organization=' + organization)
+		if versions:
+			url_params.append('versions=' + versions)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
 
+	def list_collector_groups(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		url = '/management-rest/integrations/list-connectors'
+		Class SystemInventory
+		Description: This API call output the collectors groups.
+        
+		Args:
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("list_collector_groups", locals())
+
+		url = '/management-rest/inventory/list-collector-groups'
 		url_params = []
-		if onlyValidConnectors:
-			url_params.append('onlyValidConnectors=' + str(onlyValidConnectors))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
+	def list_collectors(self, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, list]:
+		'''
+		Class SystemInventory
+		Description: This API call outputs a list of the Collectors in the system. Use the input parameters to filter the list.
+        
+		Args:
+			cloudAccounts (dict): Specifies the list cloud account names.
+			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (dict): Specifies the list of cluster.
+			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+given groups.
+			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
+			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
+			ips (dict): Specifies the list of IP values.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			loggedUser (str): Specifies the user that was logged when the event occurred.
+			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			versions (dict): Specifies the list of collector versions.
 
-	def test_connector(self, connectorName : str, connectorType : str, organization :str = None) -> tuple[bool, None]:
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("list_collectors", locals())
 
+		url = '/management-rest/inventory/list-collectors'
+		url_params = []
+		if cloudAccounts:
+			url_params.append('cloudAccounts=' + cloudAccounts)
+		if cloudProviders:
+			url_params.append('cloudProviders=' + cloudProviders)
+		if clusters:
+			url_params.append('clusters=' + clusters)
+		if collectorGroups:
+			url_params.append('collectorGroups=' + collectorGroups)
+		if collectorGroupsIds:
+			url_params.append('collectorGroupsIds=' + collectorGroupsIds)
+		if collectorType:
+			url_params.append('collectorType=' + collectorType)
+		if devices:
+			url_params.append('devices=' + devices)
+		if devicesIds:
+			url_params.append('devicesIds=' + devicesIds)
+		if firstSeen:
+			url_params.append('firstSeen=' + firstSeen)
+		if hasCrashDumps:
+			url_params.append('hasCrashDumps=' + hasCrashDumps)
+		if ips:
+			url_params.append('ips=' + ips)
+		if itemsPerPage:
+			url_params.append('itemsPerPage=' + str(itemsPerPage))
+		if lastSeenEnd:
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
+		if lastSeenStart:
+			url_params.append('lastSeenStart=' + lastSeenStart)
+		if loggedUser:
+			url_params.append('loggedUser=' + loggedUser)
+		if operatingSystems:
+			url_params.append('operatingSystems=' + operatingSystems)
+		if organization:
+			url_params.append('organization=' + organization)
+		if osFamilies:
+			url_params.append('osFamilies=' + osFamilies)
+		if pageNumber:
+			url_params.append('pageNumber=' + str(pageNumber))
+		if showExpired:
+			url_params.append('showExpired=' + showExpired)
+		if sorting:
+			url_params.append('sorting=' + sorting)
+		if states:
+			url_params.append('states=' + states)
+		if strictMode:
+			url_params.append('strictMode=' + strictMode)
+		if versions:
+			url_params.append('versions=' + versions)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
+
+	def list_cores(self, deploymentModes: dict = None, hasCrashDumps: bool = None, ip: str = None, names: dict = None, organization: str = None, versions: dict = None) -> tuple[bool, list]:
 		'''
-		class Integrations
-		Description: Tests a connector.
+		Class SystemInventory
+		Description: This API call output the list of cores.
+        
+		Args:
+			deploymentModes (dict): List of cores deployments modes.
+			hasCrashDumps (bool): Has crash dumps.
+			ip (str): IP.
+			names (dict): List of cores names.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			versions (dict): List of cores versions.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("list_cores", locals())
+
+		url = '/management-rest/inventory/list-cores'
+		url_params = []
+		if deploymentModes:
+			url_params.append('deploymentModes=' + deploymentModes)
+		if hasCrashDumps:
+			url_params.append('hasCrashDumps=' + hasCrashDumps)
+		if ip:
+			url_params.append('ip=' + ip)
+		if names:
+			url_params.append('names=' + names)
+		if organization:
+			url_params.append('organization=' + organization)
+		if versions:
+			url_params.append('versions=' + versions)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.get(url)
 
+	def list_repositories(self) -> tuple[bool, list]:
+		'''
+		Class SystemInventory
+		Description: This API call output the list of repositories (edrs).
+        
 		Args:
-			connectorName: Specifies the connector's name (case sensitive). 
-			connectorType: Specifies the connector's type.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
+			list
+		'''
+		validate_params("list_repositories", locals())
 
+		url = '/management-rest/inventory/list-repositories'
+		return fortiedr_connection.get(url)
+
+	def list_unmanaged_devices(self, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
-		url = '/management-rest/integrations/test-connector'
+		Class SystemInventory
+		Description: This API call outputs a list of the unmanaged devices in the system.
+        
+		Args:
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("list_unmanaged_devices", locals())
+
+		url = '/management-rest/inventory/list-unmanaged-devices'
 		url_params = []
-		if connectorName:
-			url_params.append('connectorName=' + str(connectorName))
-		if connectorType:
-			url_params.append('connectorType=' + str(connectorType))
+		if itemsPerPage:
+			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
+		if pageNumber:
+			url_params.append('pageNumber=' + str(pageNumber))
+		if sorting:
+			url_params.append('sorting=' + sorting)
+		if strictMode:
+			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
+	def move_collectors(self, targetCollectorGroup: str, collectorIds: dict = None, collectorSIDs: dict = None, collectors: dict = None, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call move collector between groups.
+        
+		Args:
+			collectorIds (dict): value = Array of collectors Ids. To move collectors from one organization to another.
+			collectorSIDs (dict): value = Array of collectors SIDS. To move collectors from one organization to another.
+			collectors (dict): Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>).
+			forceAssign (bool): Indicates whether to force the assignment even if the organization of the target Collector group is under migration.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			targetCollectorGroup (str): Collector group. To move collectors from one organization to another, please add the organization name before the target collector group (<organization-name>\\<collector-group-name>).
 
-	def update_connector(self, connectorActions: dict, enabled: bool, host: str, name: str, organization: str, port: str, type: str, vendor: str, apiKey: str = None, coreId: int = None, password: str = None, username: str = None) -> tuple[bool, None]:
-
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Integrations
-		Description: Updates an existing connector based on (name, type, organization). Please note: Modification of Custom connectors/actions is not yet support..
+		validate_params("move_collectors", locals())
 
+		url = '/management-rest/inventory/move-collectors'
+		url_params = []
+		if collectorIds:
+			url_params.append('collectorIds=' + collectorIds)
+		if collectorSIDs:
+			url_params.append('collectorSIDs=' + collectorSIDs)
+		if collectors:
+			url_params.append('collectors=' + collectors)
+		if forceAssign:
+			url_params.append('forceAssign=' + forceAssign)
+		if organization:
+			url_params.append('organization=' + organization)
+		if targetCollectorGroup:
+			url_params.append('targetCollectorGroup=' + targetCollectorGroup)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.insert(url)
+
+	def system_logs(self) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call retrieves a system logs.
+        
 		Args:
-			updateConnectorRequest: updateConnectorRequest. 
-			apiKey: Specifies the connector's API key (API key authentication mode). Should be empty if username and passwords are used.. 
-			connectorActions: Specifies the connector's actions' definition. Use connectors-metadata API for supported values. 
-			coreId: Specifies the ID of the connector's on-premise core. 
-			enabled: Specifies whether or not the connector is enabled.. Example: enabled=True.
-			host: Specifies the connector host address.. Example: host=127.0.0.1.
-			name: Specifies the connector name.. Example: name=Connector Name.
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			password: Specifies the connector's user's password (credentials authentication mode). Should be empty if apiKey is used.. 
-			port: Specifies the connector port.. Example: port=443.
-			type: Specifies the connector type. See /connectors-metadata for valid types.. Example: type=Firewall.
-			username: Specifies the connector's user's username (credentials authentication mode). Should be empty if apiKey is used.. 
-			vendor: Specifies the connector's vendor. See /connectors-metadata for valid values.. Example: vendor=FortiGate.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
+		'''
+		validate_params("system_logs", locals())
+
+		url = '/management-rest/inventory/system-logs'
+		return fortiedr_connection.get(url)
 
+	def toggle_collectors(self, enable: bool, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, str]:
 		'''
-		url = '/management-rest/integrations/update-connector'
+		Class SystemInventory
+		Description: This API call enables/disables a Collector(s). You must specify whether the Collector is to be enabled or disabled.
+        
+		Args:
+			cloudAccounts (dict): Specifies the list cloud account names.
+			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (dict): Specifies the list of cluster.
+			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+given groups.
+			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
+			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			enable (bool): Toggle enable.
+			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
+			ips (dict): Specifies the list of IP values.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			loggedUser (str): Specifies the user that was logged when the event occurred.
+			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			versions (dict): Specifies the list of collector versions.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			str
+		'''
+		validate_params("toggle_collectors", locals())
+
+		url = '/management-rest/inventory/toggle-collectors'
 		url_params = []
+		if cloudAccounts:
+			url_params.append('cloudAccounts=' + cloudAccounts)
+		if cloudProviders:
+			url_params.append('cloudProviders=' + cloudProviders)
+		if clusters:
+			url_params.append('clusters=' + clusters)
+		if collectorGroups:
+			url_params.append('collectorGroups=' + collectorGroups)
+		if collectorGroupsIds:
+			url_params.append('collectorGroupsIds=' + collectorGroupsIds)
+		if collectorType:
+			url_params.append('collectorType=' + collectorType)
+		if devices:
+			url_params.append('devices=' + devices)
+		if devicesIds:
+			url_params.append('devicesIds=' + devicesIds)
+		if enable:
+			url_params.append('enable=' + enable)
+		if firstSeen:
+			url_params.append('firstSeen=' + firstSeen)
+		if hasCrashDumps:
+			url_params.append('hasCrashDumps=' + hasCrashDumps)
+		if ips:
+			url_params.append('ips=' + ips)
+		if itemsPerPage:
+			url_params.append('itemsPerPage=' + str(itemsPerPage))
+		if lastSeenEnd:
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
+		if lastSeenStart:
+			url_params.append('lastSeenStart=' + lastSeenStart)
+		if loggedUser:
+			url_params.append('loggedUser=' + loggedUser)
+		if operatingSystems:
+			url_params.append('operatingSystems=' + operatingSystems)
+		if organization:
+			url_params.append('organization=' + organization)
+		if osFamilies:
+			url_params.append('osFamilies=' + osFamilies)
+		if pageNumber:
+			url_params.append('pageNumber=' + str(pageNumber))
+		if showExpired:
+			url_params.append('showExpired=' + showExpired)
+		if sorting:
+			url_params.append('sorting=' + sorting)
+		if states:
+			url_params.append('states=' + states)
+		if strictMode:
+			url_params.append('strictMode=' + strictMode)
+		if versions:
+			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
-		updateConnectorRequest = {
-			'apiKey': apiKey,
-			'connectorActions': connectorActions,
-			'coreId': coreId,
-			'enabled': enabled,
-			'host': host,
-			'name': name,
-			'organization': organization,
-			'password': password,
-			'port': port,
-			'type': type,
-			'username': username,
-			'vendor': vendor
-		}
-		return fortiedr_connection.insert(url, updateConnectorRequest)
+		return fortiedr_connection.insert(url)
+
+	def unisolate_collectors(self, devices: dict = None, devicesIds: dict = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class SystemInventory
+		Description: This API call isolate collector functionality.
+        
+		Args:
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
+		'''
+		validate_params("unisolate_collectors", locals())
+
+		url = '/management-rest/inventory/unisolate-collectors'
+		url_params = []
+		if devices:
+			url_params.append('devices=' + devices)
+		if devicesIds:
+			url_params.append('devicesIds=' + devicesIds)
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.insert(url)
 
-class Integrationssupport:
-	'''The Integrations support module enables integration with hoster environments, e.g. EMS.'''
 class IoT:
 	'''The IoT module enables you to monitor the devices found in IoT scans and create/move IoT Groups.'''
 
-	def create_iot_group(self, name : str, organization :str = None) -> tuple[bool, None]:
-
+	def create_iot_group(self, name: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call create IoT group.
-
+        
 		Args:
-			name: IoT group name. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			name (str): IoT group name.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("create_iot_group", locals())
+
 		url = '/management-rest/iot/create-iot-group'
 		url_params = []
 		if name:
-			url_params.append('name=' + str(name))
+			url_params.append('name=' + name)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def delete_devices(self, categories :dict = None, devices :dict = None, devicesIds :dict = None, firstSeenEnd :str = None, firstSeenStart :str = None, internalIps :dict = None, iotGroups :dict = None, iotGroupsIds :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, locations :dict = None, macAddresses :dict = None, models :dict = None, organization :str = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, strictMode :bool = None, vendors :dict = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url)
 
+	def delete_devices(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, None]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call deletes a IoT device(s).
-
+        
 		Args:
-			categories: Specifies the list of categories values. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			firstSeenEnd: Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			firstSeenStart: Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			internalIps: Specifies the list of IP values. 
-			iotGroups: Specifies the list of collector group names and retrieves collectors under the given groups. 
-			iotGroupsIds: Specifies the list of collector group ids and retrieves collectors under the given groups. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			locations: Specifies the list of locations values. 
-			macAddresses: Specifies the list of mac address values. 
-			models: Specifies the list of models values. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			vendors: Specifies the list of vendors values. 
+			categories (dict): Specifies the list of categories values.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			internalIps (dict): Specifies the list of IP values.
+			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			locations (dict): Specifies the list of locations values.
+			macAddresses (dict): Specifies the list of mac address values.
+			models (dict): Specifies the list of models values.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			vendors (dict): Specifies the list of vendors values.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_devices", locals())
+
 		url = '/management-rest/iot/delete-devices'
 		url_params = []
 		if categories:
-			url_params.append('categories=' + str(categories))
+			url_params.append('categories=' + categories)
 		if devices:
-			url_params.append('devices=' + str(devices))
+			url_params.append('devices=' + devices)
 		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
+			url_params.append('devicesIds=' + devicesIds)
 		if firstSeenEnd:
-			url_params.append('firstSeenEnd=' + str(firstSeenEnd))
+			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
-			url_params.append('firstSeenStart=' + str(firstSeenStart))
+			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
-			url_params.append('internalIps=' + str(internalIps))
+			url_params.append('internalIps=' + internalIps)
 		if iotGroups:
-			url_params.append('iotGroups=' + str(iotGroups))
+			url_params.append('iotGroups=' + iotGroups)
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + str(iotGroupsIds))
+			url_params.append('iotGroupsIds=' + iotGroupsIds)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
+			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
-			url_params.append('locations=' + str(locations))
+			url_params.append('locations=' + locations)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if models:
-			url_params.append('models=' + str(models))
+			url_params.append('models=' + models)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
+			url_params.append('showExpired=' + showExpired)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def export_iot_json(self, iotDeviceIds : dict, organization :str = None) -> tuple[bool, None]:
-
+	def export_iot_json(self, iotDeviceIds: dict, organization: str = None) -> tuple[bool, None]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call outputs a list of the IoT devices info.
-
+        
 		Args:
-			iotDeviceIds: Specifies the list of device ids. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			iotDeviceIds (dict): Specifies the list of device ids.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("export_iot_json", locals())
+
 		url = '/management-rest/iot/export-iot-json'
 		url_params = []
 		if iotDeviceIds:
-			url_params.append('iotDeviceIds=' + str(iotDeviceIds))
+			url_params.append('iotDeviceIds=' + iotDeviceIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_iot_devices(self, categories :dict = None, devices :dict = None, devicesIds :dict = None, firstSeenEnd :str = None, firstSeenStart :str = None, internalIps :dict = None, iotGroups :dict = None, iotGroupsIds :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, locations :dict = None, macAddresses :dict = None, models :dict = None, organization :str = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, strictMode :bool = None, vendors :dict = None) -> tuple[bool, dict]:
-
+	def list_iot_devices(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, list]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call outputs a list of the IoT devices in the system. Use the input parameters to filter the list.
-
+        
 		Args:
-			categories: Specifies the list of categories values. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			firstSeenEnd: Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			firstSeenStart: Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			internalIps: Specifies the list of IP values. 
-			iotGroups: Specifies the list of collector group names and retrieves collectors under the given groups. 
-			iotGroupsIds: Specifies the list of collector group ids and retrieves collectors under the given groups. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			locations: Specifies the list of locations values. 
-			macAddresses: Specifies the list of mac address values. 
-			models: Specifies the list of models values. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			vendors: Specifies the list of vendors values. 
+			categories (dict): Specifies the list of categories values.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			internalIps (dict): Specifies the list of IP values.
+			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			locations (dict): Specifies the list of locations values.
+			macAddresses (dict): Specifies the list of mac address values.
+			models (dict): Specifies the list of models values.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			vendors (dict): Specifies the list of vendors values.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_iot_devices", locals())
+
 		url = '/management-rest/iot/list-iot-devices'
 		url_params = []
 		if categories:
-			url_params.append('categories=' + str(categories))
+			url_params.append('categories=' + categories)
 		if devices:
-			url_params.append('devices=' + str(devices))
+			url_params.append('devices=' + devices)
 		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
+			url_params.append('devicesIds=' + devicesIds)
 		if firstSeenEnd:
-			url_params.append('firstSeenEnd=' + str(firstSeenEnd))
+			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
-			url_params.append('firstSeenStart=' + str(firstSeenStart))
+			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
-			url_params.append('internalIps=' + str(internalIps))
+			url_params.append('internalIps=' + internalIps)
 		if iotGroups:
-			url_params.append('iotGroups=' + str(iotGroups))
+			url_params.append('iotGroups=' + iotGroups)
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + str(iotGroupsIds))
+			url_params.append('iotGroupsIds=' + iotGroupsIds)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
+			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
-			url_params.append('locations=' + str(locations))
+			url_params.append('locations=' + locations)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if models:
-			url_params.append('models=' + str(models))
+			url_params.append('models=' + models)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
+			url_params.append('showExpired=' + showExpired)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_iot_groups(self, organization :str = None) -> tuple[bool, dict]:
-
+	def list_iot_groups(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call output the IoT devices groups.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_iot_groups", locals())
+
 		url = '/management-rest/iot/list-iot-groups'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def move_iot_devices(self, iotDeviceIds : dict, targetIotGroup : str, organization :str = None) -> tuple[bool, None]:
-
+	def move_iot_devices(self, iotDeviceIds: dict, targetIotGroup: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call move IoT devices between groups.
-
+        
 		Args:
-			iotDeviceIds: Array of IoT device ids. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			targetIotGroup: IoT target group name. 
+			iotDeviceIds (dict): Array of IoT device ids.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			targetIotGroup (str): IoT target group name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("move_iot_devices", locals())
+
 		url = '/management-rest/iot/move-iot-devices'
 		url_params = []
 		if iotDeviceIds:
-			url_params.append('iotDeviceIds=' + str(iotDeviceIds))
+			url_params.append('iotDeviceIds=' + iotDeviceIds)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if targetIotGroup:
-			url_params.append('targetIotGroup=' + str(targetIotGroup))
+			url_params.append('targetIotGroup=' + targetIotGroup)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def rescan_iot_device_details(self, categories :dict = None, devices :dict = None, devicesIds :dict = None, firstSeenEnd :str = None, firstSeenStart :str = None, internalIps :dict = None, iotGroups :dict = None, iotGroupsIds :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, locations :dict = None, macAddresses :dict = None, models :dict = None, organization :str = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, strictMode :bool = None, vendors :dict = None) -> tuple[bool, str]:
-
+	def rescan_iot_device_details(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, str]:
 		'''
-		class IoT
+		Class IoT
 		Description: This API call device details scan on IoT device(s).
-
+        
 		Args:
-			categories: Specifies the list of categories values. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			firstSeenEnd: Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			firstSeenStart: Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			internalIps: Specifies the list of IP values. 
-			iotGroups: Specifies the list of collector group names and retrieves collectors under the given groups. 
-			iotGroupsIds: Specifies the list of collector group ids and retrieves collectors under the given groups. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			locations: Specifies the list of locations values. 
-			macAddresses: Specifies the list of mac address values. 
-			models: Specifies the list of models values. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			vendors: Specifies the list of vendors values. 
+			categories (dict): Specifies the list of categories values.
+			devices (dict): Specifies the list of device names.
+			devicesIds (dict): Specifies the list of device ids.
+			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			internalIps (dict): Specifies the list of IP values.
+			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
+			locations (dict): Specifies the list of locations values.
+			macAddresses (dict): Specifies the list of mac address values.
+			models (dict): Specifies the list of models values.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+.
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			vendors (dict): Specifies the list of vendors values.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			str
-
 		'''
+		validate_params("rescan_iot_device_details", locals())
+
 		url = '/management-rest/iot/rescan-iot-device-details'
 		url_params = []
 		if categories:
-			url_params.append('categories=' + str(categories))
+			url_params.append('categories=' + categories)
 		if devices:
-			url_params.append('devices=' + str(devices))
+			url_params.append('devices=' + devices)
 		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
+			url_params.append('devicesIds=' + devicesIds)
 		if firstSeenEnd:
-			url_params.append('firstSeenEnd=' + str(firstSeenEnd))
+			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
-			url_params.append('firstSeenStart=' + str(firstSeenStart))
+			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
-			url_params.append('internalIps=' + str(internalIps))
+			url_params.append('internalIps=' + internalIps)
 		if iotGroups:
-			url_params.append('iotGroups=' + str(iotGroups))
+			url_params.append('iotGroups=' + iotGroups)
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + str(iotGroupsIds))
+			url_params.append('iotGroupsIds=' + iotGroupsIds)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
+			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
+			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
-			url_params.append('locations=' + str(locations))
+			url_params.append('locations=' + locations)
 		if macAddresses:
-			url_params.append('macAddresses=' + str(macAddresses))
+			url_params.append('macAddresses=' + macAddresses)
 		if models:
-			url_params.append('models=' + str(models))
+			url_params.append('models=' + models)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
+			url_params.append('showExpired=' + showExpired)
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		if vendors:
-			url_params.append('vendors=' + str(vendors))
+			url_params.append('vendors=' + vendors)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-class Organizations:
-	'''Organizations API'''
+class IPsets:
+	'''API to define IPs sets and use them for exceptions'''
 
-	def create_organization(self, expirationDate: str, name: str, password: str, passwordConfirmation: str, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, forensics: bool = None, iotAllocated: int = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None) -> tuple[bool, None]:
+	def create_ip_set(self, description: str = None, exclude: dict = None, include: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class IPsets
+		Description: This API create IP sets in the system.
+	Use the input parameter organization=All organizations to create for all the organization. (only for Admin role.
+        
+		Args:
+			ipGroupsRequest (Object): Check 'ipGroupsRequest' in the API documentation for further information.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		class Organizations
-		Description: This API creates organization in the system (only for Admin role).
+		validate_params("create_ip_set", locals())
+
+		url = '/management-rest/ip-sets/create-ip-set'
+
+		ipGroupsRequest = {
+			"description": description,
+			"exclude": exclude,
+			"include": include,
+			"name": name,
+			"organization": organization,
+		}
+		return fortiedr_connection.upload(url, ipGroupsRequest)
 
+	def delete_ip_set(self, ipSets: dict, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class IPsets
+		Description: This API delete IP sets from the system. Use the input parameters to filter organization.
+        
 		Args:
-			createAccountRequest: createAccountRequest. 
-			eXtendedDetection: A true/false parameter indication if the eXtended Detection is enabled for the organization. 
-			edr: A true/false parameter indicating whether the organization support Threat Hunting. 
-			edrAddOnsAllocated: Specifies the EDR storage add-ons allocated to this account. 
-			edrBackupEnabled: A true/false parameter indication if the EDR backup is enabled for the organization. 
-			edrEnabled: A true/false parameter indication if the EDR is enabled for the organization. 
-			edrNumberOfShards: Specifies the EDR shards per index, should be above 1 only for very large environments. 
-			edrStorageAllocatedInMb: Specifies the EDR storage allocation in MB, used when edrStorageAllocatedPercents is empty. 
-			expirationDate: Specifies the license expiration date. Specify the date using the following date format yyyy-MM-dd. 
-			forensics: A true/false parameter indicating whether the organization support Forensics. 
-			iotAllocated: Specifies the IoT device���s license capacity. 
-			name: Specifies the organization name. 
-			password: Specifies the device registration password name. 
-			passwordConfirmation: Specifies the confirm device registration password name. 
-			requestPolicyEngineLibUpdates: A true/false parameter indicating whether the organization collectors should request for policy engine lib updates. 
-			serialNumber: Specifies the serial number. 
-			serversAllocated: Specifies the server collector���s license capacity. 
-			vulnerabilityAndIoT: A true/false parameter indicating whether the organization support Vulnerability And IoT. 
-			workstationsAllocated: Specifies the workstation collector���s license capacity. 
+			ipSets (dict): Specifies the list of IP name to delete.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
+		'''
+		validate_params("delete_ip_set", locals())
+
+		url = '/management-rest/ip-sets/delete-ip-set'
+		url_params = []
+		if ipSets:
+			url_params.append('ipSets=' + ipSets)
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+		return fortiedr_connection.delete(url)
 
+	def list_ip_sets(self, ip: str = None, organization: str = None) -> tuple[bool, list]:
 		'''
-		url = '/management-rest/organizations/create-organization'
+		Class IPsets
+		Description: This API call outputs a list of the IP sets in the system. Use the input parameters to filter the list.
+        
+		Args:
+			ip (str): Specifies the IP of the requested sets.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+
+		Returns:
+			bool: Status of the request (True or False). 
+			list
+		'''
+		validate_params("list_ip_sets", locals())
+
+		url = '/management-rest/ip-sets/list-ip-sets'
 		url_params = []
+		if ip:
+			url_params.append('ip=' + ip)
+		if organization:
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		createAccountRequest = {
-			'eXtendedDetection': eXtendedDetection,
-			'edr': edr,
-			'edrAddOnsAllocated': edrAddOnsAllocated,
-			'edrBackupEnabled': edrBackupEnabled,
-			'edrEnabled': edrEnabled,
-			'edrNumberOfShards': edrNumberOfShards,
-			'edrStorageAllocatedInMb': edrStorageAllocatedInMb,
-			'expirationDate': expirationDate,
-			'forensics': forensics,
-			'iotAllocated': iotAllocated,
-			'name': name,
-			'password': password,
-			'passwordConfirmation': passwordConfirmation,
-			'requestPolicyEngineLibUpdates': requestPolicyEngineLibUpdates,
-			'serialNumber': serialNumber,
-			'serversAllocated': serversAllocated,
-			'vulnerabilityAndIoT': vulnerabilityAndIoT,
-			'workstationsAllocated': workstationsAllocated
+		return fortiedr_connection.get(url)
+
+	def update_ip_set(self, description: str = None, exclude: dict = None, include: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
+		'''
+		Class IPsets
+		Description: This API update IP sets in the system. Use the input parameters to filter organization.
+        
+		Args:
+			ipGroupsRequest (Object): Check 'ipGroupsRequest' in the API documentation for further information.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
+���	each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately..
+
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
+		'''
+		validate_params("update_ip_set", locals())
+
+		url = '/management-rest/ip-sets/update-ip-set'
+		url_params = []
+		if organization:
+			url_params.append('organization=' + organization)
+		url += '?' + '&'.join(url_params)
+
+		ipGroupsRequest = {
+			"description": description,
+			"exclude": exclude,
+			"include": include,
+			"name": name,
 		}
-		return fortiedr_connection.send(url, createAccountRequest)
+		return fortiedr_connection.insert(url, ipGroupsRequest)
+
+class Organizations:
+	'''Organizations API'''
 
+	def create_organization(self, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, expirationDate: str = None, forensics: bool = None, iotAllocated: int = None, name: str = None, password: str = None, passwordConfirmation: str = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None) -> tuple[bool, None]:
+		'''
+		Class Organizations
+		Description: This API creates organization in the system (only for Admin role).
+        
+		Args:
+			createAccountRequest (Object): Check 'createAccountRequest' in the API documentation for further information.
+
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
+		'''
+		validate_params("create_organization", locals())
 
-	def delete_organization(self, organization :str = None) -> tuple[bool, None]:
+		url = '/management-rest/organizations/create-organization'
+
+		createAccountRequest = {
+			"eXtendedDetection": eXtendedDetection,
+			"edr": edr,
+			"edrAddOnsAllocated": str(edrAddOnsAllocated),
+			"edrBackupEnabled": edrBackupEnabled,
+			"edrEnabled": edrEnabled,
+			"edrNumberOfShards": str(edrNumberOfShards),
+			"edrStorageAllocatedInMb": str(edrStorageAllocatedInMb),
+			"expirationDate": expirationDate,
+			"forensics": forensics,
+			"iotAllocated": str(iotAllocated),
+			"name": name,
+			"password": password,
+			"passwordConfirmation": passwordConfirmation,
+			"requestPolicyEngineLibUpdates": requestPolicyEngineLibUpdates,
+			"serialNumber": serialNumber,
+			"serversAllocated": str(serversAllocated),
+			"vulnerabilityAndIoT": vulnerabilityAndIoT,
+			"workstationsAllocated": str(workstationsAllocated),
+		}
+		return fortiedr_connection.upload(url, createAccountRequest)
 
+	def delete_organization(self, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: This API delete organization in the system (only for Admin role).
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_organization", locals())
+
 		url = '/management-rest/organizations/delete-organization'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def export_organization(self, destinationName :str = None, organization :str = None) -> tuple[bool, None]:
-
+	def export_organization(self, destinationName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: Export organization data as zip file.
-
+        
 		Args:
-			destinationName: The organization destination name. 
-			organization: Organization to export. 
+			destinationName (str): The organization destination name.
+			organization (str): Organization to export.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("export_organization", locals())
+
 		url = '/management-rest/organizations/export-organization'
 		url_params = []
 		if destinationName:
-			url_params.append('destinationName=' + str(destinationName))
+			url_params.append('destinationName=' + destinationName)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.download(url)
-
-
-	def import_organization(self, file :BinaryIO = None) -> tuple[bool, None]:
+		return fortiedr_connection.get(url)
 
+	def import_organization(self, file: BinaryIO = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: Import organization.
-
+        
 		Args:
-			file: Export zip file. 
+			file (BinaryIO): Export zip file.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/organizations/import-organization'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
+		validate_params("import_organization", locals())
 
+		url = '/management-rest/organizations/import-organization'
+		if file:
+			file = {'file': file}
+		return fortiedr_connection.upload(url, file, request_type="multipart/form-data")
 
-	def list_organizations(self) -> tuple[bool, dict]:
-
+	def list_organizations(self) -> tuple[bool, list]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: This API call outputs a list of the accounts in the system..
-
+        
 		Args:
-			file: Export zip file. 
 
+		Returns:
+			bool: Status of the request (True or False). 
+			list
 		'''
+		validate_params("list_organizations", locals())
+
 		url = '/management-rest/organizations/list-organizations'
 		return fortiedr_connection.get(url)
 
-
-	def transfer_collectors(self, aggregatorsMap: dict, sourceOrganization: str, targetOrganization: str, verificationCode: str) -> tuple[bool, None]:
-
+	def transfer_collectors(self, aggregatorsMap: dict = None, sourceOrganization: str = None, targetOrganization: str = None, verificationCode: str = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: Transfer collectors from aggregator to aggregator as the organization migration process.
-
+        
 		Args:
-			transferCollectorRequests: transferCollectorRequests. 
-			aggregatorsMap: Specifies aggregators transfer mapping. 
-			sourceOrganization: Specifies the organization which collectors will be transferred from.. 
-			targetOrganization: Specifies the organization which collectors will be transferred to.. 
-			verificationCode: Specifies the verification code to validate the import step was finished successfully.. 
+			transferCollectorRequests (Object): Check 'transferCollectorRequests' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("transfer_collectors", locals())
+
 		url = '/management-rest/organizations/transfer-collectors'
-		url_params = []
-		url += '?' + '&'.join(url_params)
+
 		transferCollectorRequests = {
-			'aggregatorsMap': aggregatorsMap,
-			'sourceOrganization': sourceOrganization,
-			'targetOrganization': targetOrganization,
-			'verificationCode': verificationCode
+			"aggregatorsMap": aggregatorsMap,
+			"sourceOrganization": sourceOrganization,
+			"targetOrganization": targetOrganization,
+			"verificationCode": verificationCode,
 		}
-		return fortiedr_connection.send(url, transferCollectorRequests)
-
-
-	def transfer_collectors_stop(self, organization :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, transferCollectorRequests)
 
+	def transfer_collectors_stop(self, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: Transfer collector stop.
-
+        
 		Args:
-			organization: Specifies the organization which the migration process should stop. 
+			organization (str): Specifies the organization which the migration process should stop.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("transfer_collectors_stop", locals())
+
 		url = '/management-rest/organizations/transfer-collectors-stop'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def update_organization(self, organization :str = None, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, expirationDate: str = None, forensics: bool = None, iotAllocated: int = None, name: str = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url)
 
+	def update_organization(self, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, expirationDate: str = None, forensics: bool = None, iotAllocated: int = None, name: str = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Organizations
+		Class Organizations
 		Description: This API update organization in the system (only for Admin role).
-
+        
 		Args:
-			accountRequest: accountRequest. 
-			eXtendedDetection: A true/false parameter indication if the eXtended Detection is enabled for the organization. 
-			edr: A true/false parameter indicating whether the organization support Threat Hunting. 
-			edrAddOnsAllocated: Specifies the EDR storage add-ons allocated to this account. 
-			edrBackupEnabled: A true/false parameter indication if the EDR backup is enabled for the organization. 
-			edrEnabled: A true/false parameter indication if the EDR is enabled for the organization. 
-			edrNumberOfShards: Specifies the EDR shards per index, should be above 1 only for very large environments. 
-			edrStorageAllocatedInMb: Specifies the EDR storage allocation in MB, used when edrStorageAllocatedPercents is empty. 
-			expirationDate: Specifies the license expiration date. Specify the date using the following date format yyyy-MM-dd. 
-			forensics: A true/false parameter indicating whether the organization support Forensics. 
-			iotAllocated: Specifies the IoT device���s license capacity. 
-			name: Specifies the organization name. 
-			requestPolicyEngineLibUpdates: A true/false parameter indicating whether the organization collectors should request for policy engine lib updates. 
-			serialNumber: Specifies the serial number. 
-			serversAllocated: Specifies the server collector���s license capacity. 
-			vulnerabilityAndIoT: A true/false parameter indicating whether the organization support Vulnerability And IoT. 
-			workstationsAllocated: Specifies the workstation collector���s license capacity. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			accountRequest (Object): Check 'accountRequest' in the API documentation for further information.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("update_organization", locals())
+
 		url = '/management-rest/organizations/update-organization'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
+
+		accountRequest = {
+			"eXtendedDetection": eXtendedDetection,
+			"edr": edr,
+			"edrAddOnsAllocated": str(edrAddOnsAllocated),
+			"edrBackupEnabled": edrBackupEnabled,
+			"edrEnabled": edrEnabled,
+			"edrNumberOfShards": str(edrNumberOfShards),
+			"edrStorageAllocatedInMb": str(edrStorageAllocatedInMb),
+			"expirationDate": expirationDate,
+			"forensics": forensics,
+			"iotAllocated": str(iotAllocated),
+			"name": name,
+			"requestPolicyEngineLibUpdates": requestPolicyEngineLibUpdates,
+			"serialNumber": serialNumber,
+			"serversAllocated": str(serversAllocated),
+			"vulnerabilityAndIoT": vulnerabilityAndIoT,
+			"workstationsAllocated": str(workstationsAllocated),
+		}
+		return fortiedr_connection.insert(url, accountRequest)
 
 class Playbookspolicies:
 	'''Playbooks-policies API'''
 
-	def assign_collector_group(self, collectorGroupNames : dict, policyName : str, forceAssign :bool = None, organization :str = None) -> tuple[bool, None]:
-
+	def assign_collector_group(self, collectorGroupNames: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: Assign collector group to air policy.
-
+        
 		Args:
-			collectorGroupNames: Specifies the list of collector group names. 
-			forceAssign: Indicates whether to force the assignment even if the group is assigned to similar policies. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies policy name. 
+			collectorGroupNames (dict): Specifies the list of collector group names.
+			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies policy name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("assign_collector_group", locals())
+
 		url = '/management-rest/playbooks-policies/assign-collector-group'
 		url_params = []
 		if collectorGroupNames:
-			url_params.append('collectorGroupNames=' + str(collectorGroupNames))
+			url_params.append('collectorGroupNames=' + collectorGroupNames)
 		if forceAssign:
-			url_params.append('forceAssign=' + str(forceAssign))
+			url_params.append('forceAssign=' + forceAssign)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def clone(self, newPolicyName : str, sourcePolicyName : str, organization :str = None) -> tuple[bool, None]:
-
+	def clone(self, newPolicyName: str, sourcePolicyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: clone policy.
-
+        
 		Args:
-			newPolicyName: Specifies security policy target name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			sourcePolicyName: Specifies security policy source name. 
+			newPolicyName (str): Specifies security policy target name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			sourcePolicyName (str): Specifies security policy source name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("clone", locals())
+
 		url = '/management-rest/playbooks-policies/clone'
 		url_params = []
 		if newPolicyName:
-			url_params.append('newPolicyName=' + str(newPolicyName))
+			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if sourcePolicyName:
-			url_params.append('sourcePolicyName=' + str(sourcePolicyName))
+			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def list_policies(self, organization :str = None) -> tuple[bool, dict]:
+		return fortiedr_connection.upload(url)
 
+	def list_policies(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: List policies.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_policies", locals())
+
 		url = '/management-rest/playbooks-policies/list-policies'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def map_connectors_to_actions(self, policyName: str, organization :str = None, customActionsToConnectorsMaps: dict = None, fortinetActionsToConnectorsMaps: dict = None) -> tuple[bool, None]:
-
+	def map_connectors_to_actions(self, customActionsToConnectorsMaps: dict = None, fortinetActionsToConnectorsMaps: dict = None, policyName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: Assign policy actions with connectors..
-
+        
 		Args:
-			assignAIRActionsWithConnectorsRequest: assignAIRActionsWithConnectorsRequest. 
-			customActionsToConnectorsMaps: Specifies which connectors are to be used during a custom action invocation.. 
-			fortinetActionsToConnectorsMaps: Specifies which connectors are to be used during an Fortinet action invocation.. 
-			policyName: Specifies the policy name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			assignAIRActionsWithConnectorsRequest (Object): Check 'assignAIRActionsWithConnectorsRequest' in the API documentation for further information.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("map_connectors_to_actions", locals())
+
 		url = '/management-rest/playbooks-policies/map-connectors-to-actions'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
 
-	def set_action_classification(self, policyName: str, organization :str = None, customActionsToClassificationMaps: dict = None, fortinetActionsToClassificationMaps: dict = None) -> tuple[bool, None]:
+		assignAIRActionsWithConnectorsRequest = {
+			"customActionsToConnectorsMaps": customActionsToConnectorsMaps,
+			"fortinetActionsToConnectorsMaps": fortinetActionsToConnectorsMaps,
+			"policyName": policyName,
+		}
+		return fortiedr_connection.insert(url, assignAIRActionsWithConnectorsRequest)
 
+	def set_action_classification(self, organization: str = None, customActionsToClassificationMaps: dict = None, fortinetActionsToClassificationMaps: dict = None, policyName: str = None) -> tuple[bool, None]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: Set the air policy actions' classifications..
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			setActionsClassificationRequest: setActionsClassificationRequest. 
-			customActionsToClassificationMaps: Specifies which custom actions' classifications should be enabled. Missing classifications are disabled.. 
-			fortinetActionsToClassificationMaps: Specifies which Fortinet actions' classifications should be enabled. Missing classifications are disabled.. 
-			policyName: Specifies the policy name.. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			setActionsClassificationRequest (Object): Check 'setActionsClassificationRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_action_classification", locals())
+
 		url = '/management-rest/playbooks-policies/set-action-classification'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
+
 		setActionsClassificationRequest = {
-			'customActionsToClassificationMaps': customActionsToClassificationMaps,
-			'fortinetActionsToClassificationMaps': fortinetActionsToClassificationMaps,
-			'policyName': policyName
+			"customActionsToClassificationMaps": customActionsToClassificationMaps,
+			"fortinetActionsToClassificationMaps": fortinetActionsToClassificationMaps,
+			"policyName": policyName,
 		}
 		return fortiedr_connection.insert(url, setActionsClassificationRequest)
 
-
-	def set_mode(self, mode : str, policyName : str, organization :str = None) -> tuple[bool, None]:
-
+	def set_mode(self, mode: str, policyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Playbookspolicies
+		Class Playbookspolicies
 		Description: Set playbook to simulation/prevention.
-
+        
 		Args:
-			mode: Operation mode. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies security policy name. 
+			mode (str): Operation mode.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies security policy name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_mode", locals())
+
 		url = '/management-rest/playbooks-policies/set-mode'
 		url_params = []
 		if mode:
-			url_params.append('mode=' + str(mode))
+			url_params.append('mode=' + mode)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class Policies:
 	'''Policies API'''
 
-	def assign_collector_group(self, collectorsGroupName : dict, policyName : str, forceAssign :bool = None, organization :str = None) -> tuple[bool, None]:
-
+	def assign_collector_group(self, collectorsGroupName: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: Assign collector group to policy.
-
+        
 		Args:
-			collectorsGroupName: Specifies the list of collector group names. 
-			forceAssign: Indicates whether to force the assignment even if the group is assigned to similar policies. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies security policy name. 
+			collectorsGroupName (dict): Specifies the list of collector group names.
+			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies security policy name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("assign_collector_group", locals())
+
 		url = '/management-rest/policies/assign-collector-group'
 		url_params = []
 		if collectorsGroupName:
-			url_params.append('collectorsGroupName=' + str(collectorsGroupName))
+			url_params.append('collectorsGroupName=' + collectorsGroupName)
 		if forceAssign:
-			url_params.append('forceAssign=' + str(forceAssign))
+			url_params.append('forceAssign=' + forceAssign)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def clone(self, newPolicyName : str, sourcePolicyName : str, organization :str = None) -> tuple[bool, None]:
-
+	def clone(self, newPolicyName: str, sourcePolicyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: clone policy.
-
+        
 		Args:
-			newPolicyName: Specifies security policy target name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			sourcePolicyName: Specifies security policy source name. 
+			newPolicyName (str): Specifies security policy target name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			sourcePolicyName (str): Specifies security policy source name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("clone", locals())
+
 		url = '/management-rest/policies/clone'
 		url_params = []
 		if newPolicyName:
-			url_params.append('newPolicyName=' + str(newPolicyName))
+			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if sourcePolicyName:
-			url_params.append('sourcePolicyName=' + str(sourcePolicyName))
+			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def list_policies(self, organization :str = None) -> tuple[bool, dict]:
+		return fortiedr_connection.upload(url)
 
+	def list_policies(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class Policies
+		Class Policies
 		Description: List policies.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_policies", locals())
+
 		url = '/management-rest/policies/list-policies'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def scan_files(self, applyRecursiveScan : bool, executableFilesOnly : bool, origin : str, scanBy : str, filePaths :dict = None, organization :str = None, scanSelection :dict = None) -> tuple[bool, None]:
-
+	def scan_files(self, applyRecursiveScan: bool, executableFilesOnly: bool, origin: str, scanBy: str, filePaths: dict = None, organization: str = None, scanSelection: dict = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: Scan Files.
-
+        
 		Args:
-			applyRecursiveScan: Specifies if execution includes recursive scan. 
-			executableFilesOnly: Specifies if execution includes only files. 
-			filePaths: Specifies file path. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			origin: Specifies scan origin. 
-			scanBy: Specifies scan by choice. 
-			scanSelection: Specifies scan selection. 
+			applyRecursiveScan (bool): Specifies if execution includes recursive scan.
+			executableFilesOnly (bool): Specifies if execution includes only files.
+			filePaths (dict): Specifies file path.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			origin (str): Specifies scan origin.
+			scanBy (str): Specifies scan by choice.
+			scanSelection (dict): Specifies scan selection.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("scan_files", locals())
+
 		url = '/management-rest/policies/scan-files'
 		url_params = []
 		if applyRecursiveScan:
-			url_params.append('applyRecursiveScan=' + str(applyRecursiveScan))
+			url_params.append('applyRecursiveScan=' + applyRecursiveScan)
 		if executableFilesOnly:
-			url_params.append('executableFilesOnly=' + str(executableFilesOnly))
+			url_params.append('executableFilesOnly=' + executableFilesOnly)
 		if filePaths:
-			url_params.append('filePaths=' + str(filePaths))
+			url_params.append('filePaths=' + filePaths)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if origin:
-			url_params.append('origin=' + str(origin))
+			url_params.append('origin=' + origin)
 		if scanBy:
-			url_params.append('scanBy=' + str(scanBy))
+			url_params.append('scanBy=' + scanBy)
 		if scanSelection:
-			url_params.append('scanSelection=' + str(scanSelection))
+			url_params.append('scanSelection=' + scanSelection)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def set_mode(self, mode : str, policyName : str, organization :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url)
 
+	def set_mode(self, mode: str, policyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: Set policy to simulation/prevention.
-
+        
 		Args:
-			mode: Operation mode. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies security policy name. 
+			mode (str): Operation mode.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies security policy name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_mode", locals())
+
 		url = '/management-rest/policies/set-mode'
 		url_params = []
 		if mode:
-			url_params.append('mode=' + str(mode))
+			url_params.append('mode=' + mode)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def set_policy_rule_action(self, action : str, policyName : str, ruleName : str, organization :str = None) -> tuple[bool, None]:
-
+	def set_policy_rule_action(self, action: str, policyName: str, ruleName: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: Set rule in policy to block/log.
-
+        
 		Args:
-			action: Specifies the policy action. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies security policy name. 
-			ruleName: Specifies rule name. 
+			action (str): Specifies the policy action.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies security policy name.
+			ruleName (str): Specifies rule name.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_policy_rule_action", locals())
+
 		url = '/management-rest/policies/set-policy-rule-action'
 		url_params = []
 		if action:
-			url_params.append('action=' + str(action))
+			url_params.append('action=' + action)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		if ruleName:
-			url_params.append('ruleName=' + str(ruleName))
+			url_params.append('ruleName=' + ruleName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def set_policy_rule_state(self, policyName : str, ruleName : str, state : str, organization :str = None) -> tuple[bool, None]:
-
+	def set_policy_rule_state(self, policyName: str, ruleName: str, state: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Policies
+		Class Policies
 		Description: Set rule in policy to enable/disable.
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			policyName: Specifies security policy name. 
-			ruleName: Specifies rule name. 
-			state: Policy rule state. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			policyName (str): Specifies security policy name.
+			ruleName (str): Specifies rule name.
+			state (str): Policy rule state.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_policy_rule_state", locals())
+
 		url = '/management-rest/policies/set-policy-rule-state'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if policyName:
-			url_params.append('policyName=' + str(policyName))
+			url_params.append('policyName=' + policyName)
 		if ruleName:
-			url_params.append('ruleName=' + str(ruleName))
+			url_params.append('ruleName=' + ruleName)
 		if state:
-			url_params.append('state=' + str(state))
+			url_params.append('state=' + state)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class SendableEntities:
 	'''API to create and test sendable entities'''
 
-	def set_mail_format(self, format : str, organization :str = None) -> tuple[bool, None]:
-
+	def set_mail_format(self, format: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class SendableEntities
+		Class SendableEntities
 		Description: set mail format.
-
+        
 		Args:
-			format: Specifies email format type. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			format (str): Specifies email format type.
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_mail_format", locals())
+
 		url = '/management-rest/sendable-entities/set-mail-format'
 		url_params = []
 		if format:
-			url_params.append('format=' + str(format))
+			url_params.append('format=' + format)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-
-	def syslog(self, host: str, name: str, port: int, protocol: str, syslogFormat: str, organization :str = None, certificateBlob: str = None, privateKeyFile: str = None, privateKeyPassword: str = None, useClientCertificate: bool = None, useSSL: bool = None) -> tuple[bool, None]:
-
+	def syslog(self, organization: str = None, certificateBlob: str = None, host: str = None, name: str = None, port: int = None, privateKeyFile: str = None, privateKeyPassword: str = None, protocol: str = None, syslogFormat: str = None, useClientCertificate: bool = None, useSSL: bool = None) -> tuple[bool, None]:
 		'''
-		class SendableEntities
+		Class SendableEntities
 		Description: This API creates syslog.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately.. 
-			syslogRequest: syslogRequest. 
-			certificateBlob: Specifies client certificate in Base64. 
-			host: Specifies the syslog host. 
-			name: Specifies the syslog name. 
-			port: Specifies the syslog port. 
-			privateKeyFile: Specifies client private key in Base64. 
-			privateKeyPassword: Specifies client private key password. 
-			protocol: Specifies syslog protocol type. 
-			syslogFormat: Specifies syslog format type. 
-			useClientCertificate: Specifies whether use client certificate. False by default. 
-			useSSL: Specifies whether to use SSL. False by default. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately..
+			syslogRequest (Object): Check 'syslogRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("syslog", locals())
+
 		url = '/management-rest/sendable-entities/syslog'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
+
 		syslogRequest = {
-			'certificateBlob': certificateBlob,
-			'host': host,
-			'name': name,
-			'port': port,
-			'privateKeyFile': privateKeyFile,
-			'privateKeyPassword': privateKeyPassword,
-			'protocol': protocol,
-			'syslogFormat': syslogFormat,
-			'useClientCertificate': useClientCertificate,
-			'useSSL': useSSL
+			"certificateBlob": certificateBlob,
+			"host": host,
+			"name": name,
+			"port": str(port),
+			"privateKeyFile": privateKeyFile,
+			"privateKeyPassword": privateKeyPassword,
+			"protocol": protocol,
+			"syslogFormat": syslogFormat,
+			"useClientCertificate": useClientCertificate,
+			"useSSL": useSSL,
 		}
-		return fortiedr_connection.send(url, syslogRequest)
+		return fortiedr_connection.upload(url, syslogRequest)
 
 class SystemEvents:
 	'''System Events API'''
 
-	def list_system_events(self, componentNames :dict = None, componentTypes :dict = None, fromDate :str = None, itemsPerPage :int = None, organization :str = None, pageNumber :int = None, sorting :str = None, strictMode :bool = None, toDate :str = None) -> tuple[bool, dict]:
-
+	def list_system_events(self, componentNames: dict = None, componentTypes: dict = None, fromDate: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None, toDate: str = None) -> tuple[bool, list]:
 		'''
-		class SystemEvents
+		Class SystemEvents
 		Description: Retrieve system events.
-
+        
 		Args:
-			componentNames:  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events. 
-			componentTypes: Specifies one or more component type. 
-			fromDate: Searches for system events that occurred after this date. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			toDate: Searches for system events that occurred before this date. 
+			componentNames (dict):  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events.
+			componentTypes (dict): Specifies one or more component type.
+			fromDate (str): Searches for system events that occurred after this date.
+			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			pageNumber (int): An integer used for paging that indicates the required page number.
+			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
+			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
+			toDate (str): Searches for system events that occurred before this date.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_system_events", locals())
+
 		url = '/management-rest/system-events/list-system-events'
 		url_params = []
 		if componentNames:
-			url_params.append('componentNames=' + str(componentNames))
+			url_params.append('componentNames=' + componentNames)
 		if componentTypes:
-			url_params.append('componentTypes=' + str(componentTypes))
+			url_params.append('componentTypes=' + componentTypes)
 		if fromDate:
-			url_params.append('fromDate=' + str(fromDate))
+			url_params.append('fromDate=' + fromDate)
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + str(itemsPerPage))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + str(pageNumber))
 		if sorting:
-			url_params.append('sorting=' + str(sorting))
+			url_params.append('sorting=' + sorting)
 		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('strictMode=' + strictMode)
 		if toDate:
-			url_params.append('toDate=' + str(toDate))
+			url_params.append('toDate=' + toDate)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-class SystemInventory:
-	'''The System Inventory module enables you to monitor the health of Fortinet Endpoint Protection and Response Platform components and to create Collector Groups.'''
-
-	def aggregator_logs(self, device :str = None, deviceId :int = None, organization :str = None) -> tuple[bool, None]:
+class ThreatHuntingExclusions:
+	'''API to create Threat Hunting exclusions.'''
 
+	def upload_exclusion(self, exclusionListName: str = None, exclusions: dict = None, organization: str = None) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call retrieves a aggregator logs.
-
+		Class ThreatHuntingExclusions
+		Description: Creates exclusions..
+        
 		Args:
-			device: Specifies the name of the device. 
-			deviceId: Specifies the ID of the device. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			createExclusionsRequest (Object): Check 'createExclusionsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
+			list
 		'''
-		url = '/management-rest/inventory/aggregator-logs'
-		url_params = []
-		if device:
-			url_params.append('device=' + str(device))
-		if deviceId:
-			url_params.append('deviceId=' + str(deviceId))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		validate_params("upload_exclusion", locals())
 
+		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-	def check_custom_installer(self, customInstallerID : str) -> tuple[bool, None]:
+		createExclusionsRequest = {
+			"exclusionListName": exclusionListName,
+			"exclusions": exclusions,
+			"organization": organization,
+		}
+		return fortiedr_connection.upload(url, createExclusionsRequest)
 
+	def insert_exclusions(self, exclusionListName: str = None, exclusions: dict = None, organization: str = None) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call for checking the results for an custom installer request and getting the installer url.
-
+		Class ThreatHuntingExclusions
+		Description: Update exclusions..
+        
 		Args:
-			customInstallerID: customInstallerID. 
+			updateExclusionsRequest (Object): Check 'updateExclusionsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
+			list
 		'''
-		url = '/management-rest/inventory/check-custom-installer'
-		url_params = []
-		if customInstallerID:
-			url_params.append('customInstallerID=' + str(customInstallerID))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		validate_params("insert_exclusions", locals())
 
+		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-	def collector_logs(self, device :str = None, deviceId :int = None, organization :str = None) -> tuple[bool, None]:
+		updateExclusionsRequest = {
+			"exclusionListName": exclusionListName,
+			"exclusions": exclusions,
+			"organization": organization,
+		}
+		return fortiedr_connection.insert(url, updateExclusionsRequest)
 
+	def delete_exclusion(self, exclusionIds: dict = None, organization: str = None) -> tuple[bool, str]:
 		'''
-		class SystemInventory
-		Description: This API call retrieves a collector logs.
-
+		Class ThreatHuntingExclusions
+		Description: Deletes one or more exclusions by Id..
+        
 		Args:
-			device: Specifies the name of the device. 
-			deviceId: Specifies the ID of the device. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			deleteExclusionsRequest (Object): Check 'deleteExclusionsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
+			str
 		'''
-		url = '/management-rest/inventory/collector-logs'
-		url_params = []
-		if device:
-			url_params.append('device=' + str(device))
-		if deviceId:
-			url_params.append('deviceId=' + str(deviceId))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		validate_params("delete_exclusion", locals())
 
+		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-	def core_logs(self, device :str = None, deviceId :int = None, organization :str = None) -> tuple[bool, None]:
+		deleteExclusionsRequest = {
+			"exclusionIds": exclusionIds,
+			"organization": organization,
+		}
+		return fortiedr_connection.delete(url, deleteExclusionsRequest)
 
+	def get_exclusions_list(self, organization: str, ) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call retrieves a core logs.
-
+		Class ThreatHuntingExclusions
+		Description: Get the list of Exclusions lists..
+        
 		Args:
-			device: Specifies the name of the device. 
-			deviceId: Specifies the ID of the device. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
+			list
 		'''
-		url = '/management-rest/inventory/core-logs'
+		validate_params("get_exclusions_list", locals())
+
+		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 		url_params = []
-		if device:
-			url_params.append('device=' + str(device))
-		if deviceId:
-			url_params.append('deviceId=' + str(deviceId))
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def create_collector_group(self, name : str, organization :str = None) -> tuple[bool, None]:
-
+	def upload_exclusions_list(self, collectorGroupIds: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call create collector group.
-
+		Class ThreatHuntingExclusions
+		Description: Creates an exclusions list.
+        
 		Args:
-			name: Collector group name. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
+			createExclusionListRequest (Object): Check 'createExclusionListRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/inventory/create-collector-group'
-		url_params = []
-		if name:
-			url_params.append('name=' + str(name))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
+		validate_params("upload_exclusions_list", locals())
 
+		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 
-	def create_ems_custom_installer(self, osType : str, aggregatorAddress :str = None, aggregatorPort :int = None, citrixPVS :bool = None, collectorGroup :str = None, collectorVersion :str = None, distro :str = None, is64bit :bool = None, organization :str = None, proxy :bool = None, vdi :bool = None) -> tuple[bool, None]:
+		createExclusionListRequest = {
+			"collectorGroupIds": collectorGroupIds,
+			"name": name,
+			"organization": organization,
+		}
+		return fortiedr_connection.upload(url, createExclusionListRequest)
 
+	def insert_exclusions_list(self, collectorGroupIds: dict = None, listName: str = None, newName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call sends request for creating custom-installer for EMS integration.
-
+		Class ThreatHuntingExclusions
+		Description: Updates an exclusions list.
+        
 		Args:
-			aggregatorAddress: Specifies the aggregator ip or dns address. 
-			aggregatorPort: Specifies the aggregator port. 
-			citrixPVS: Specifies whether the collector installed with citrix in pvs mode. 
-			collectorGroup: Specifies the requested collector group. 
-			collectorVersion: Specifies the requested collector version. 
-			distro: Specifies the Linux distribution. For example: CentOS_6, CentOS_7, CentOS_8, CentOS_9, Amazon, Oracle_6, Oracle_7, Oracle_8, SLES_12, SLES_15, Ubuntu_16.04, Ubuntu_18.04, Ubuntu_20.04, Ubuntu_22.04. 
-			is64bit: Specifies the Windows os bit version. 
-			organization: Specifies the requested organization. 
-			osType: Specifies the operating system type. 
-			proxy: Specifies the system proxy settings (Only applies to Collector versions 3.1 and above). 
-			vdi: Specifies the VDI (Virtual Desktop Infrastructure) installation. 
+			updateExclusionListRequest (Object): Check 'updateExclusionListRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/inventory/create-ems-custom-installer'
-		url_params = []
-		if aggregatorAddress:
-			url_params.append('aggregatorAddress=' + str(aggregatorAddress))
-		if aggregatorPort:
-			url_params.append('aggregatorPort=' + str(aggregatorPort))
-		if citrixPVS:
-			url_params.append('citrixPVS=' + str(citrixPVS))
-		if collectorGroup:
-			url_params.append('collectorGroup=' + str(collectorGroup))
-		if collectorVersion:
-			url_params.append('collectorVersion=' + str(collectorVersion))
-		if distro:
-			url_params.append('distro=' + str(distro))
-		if is64bit:
-			url_params.append('is64bit=' + str(is64bit))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if osType:
-			url_params.append('osType=' + str(osType))
-		if proxy:
-			url_params.append('proxy=' + str(proxy))
-		if vdi:
-			url_params.append('vdi=' + str(vdi))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
+		validate_params("insert_exclusions_list", locals())
 
+		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 
-	def delete_collectors(self, cloudAccounts :dict = None, cloudProviders :dict = None, clusters :dict = None, collectorGroups :dict = None, collectorGroupsIds :dict = None, collectorType :str = None, confirmDeletion :bool = None, deleteAll :bool = None, devices :dict = None, devicesIds :dict = None, firstSeen :str = None, hasCrashDumps :bool = None, ips :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, loggedUser :str = None, operatingSystems :dict = None, organization :str = None, osFamilies :dict = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, states :dict = None, strictMode :bool = None, versions :dict = None) -> tuple[bool, None]:
+		updateExclusionListRequest = {
+			"collectorGroupIds": collectorGroupIds,
+			"listName": listName,
+			"newName": newName,
+			"organization": organization,
+		}
+		return fortiedr_connection.insert(url, updateExclusionListRequest)
 
+	def delete_exclusions_list(self, listName: str, organization: str, ) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call deletes a Collector(s).
-
+		Class ThreatHuntingExclusions
+		Description: Deletes an exclusions list..
+        
 		Args:
-			cloudAccounts: Specifies the list cloud account names. 
-			cloudProviders: Specifies the list of cloud providers: AWS, Azure, GCP. 
-			clusters: Specifies the list of cluster. 
-			collectorGroups: Specifies the list of collector group names and retrieves collectors under thegiven groups. 
-			collectorGroupsIds: Specifies the list of collector group Ids and retrieves collectors under thegiven groups. 
-			collectorType: Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default. 
-			confirmDeletion: A true/false parameter indicating if to detach/delete relevant exceptions from Collector groups about to be deleted. 
-			deleteAll: A true/false parameter indicating if all collectors should be deleted. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			firstSeen: Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			hasCrashDumps: Retrieves collectors that have crash dumps. 
-			ips: Specifies the list of IP values. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			loggedUser: Specifies the user that was logged when the event occurred. 
-			operatingSystems: Specifies the list of specific operating systems. For example, Windows 7 Pro. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			osFamilies: Specifies the list of operating system families: Windows, Windows Server or OS X. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			states: Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, Pending Reboot, Isolated, Expired, Migrated or Pending Migration. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			versions: Specifies the list of collector versions. 
+			listName (str): Exclusions list name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/inventory/delete-collectors'
+		validate_params("delete_exclusions_list", locals())
+
+		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 		url_params = []
-		if cloudAccounts:
-			url_params.append('cloudAccounts=' + str(cloudAccounts))
-		if cloudProviders:
-			url_params.append('cloudProviders=' + str(cloudProviders))
-		if clusters:
-			url_params.append('clusters=' + str(clusters))
-		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
-		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + str(collectorGroupsIds))
-		if collectorType:
-			url_params.append('collectorType=' + str(collectorType))
-		if confirmDeletion:
-			url_params.append('confirmDeletion=' + str(confirmDeletion))
-		if deleteAll:
-			url_params.append('deleteAll=' + str(deleteAll))
-		if devices:
-			url_params.append('devices=' + str(devices))
-		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
-		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
-		if hasCrashDumps:
-			url_params.append('hasCrashDumps=' + str(hasCrashDumps))
-		if ips:
-			url_params.append('ips=' + str(ips))
-		if itemsPerPage:
-			url_params.append('itemsPerPage=' + str(itemsPerPage))
-		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
-		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
-		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
-		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
+		if listName:
+			url_params.append('listName=' + listName)
 		if organization:
-			url_params.append('organization=' + str(organization))
-		if osFamilies:
-			url_params.append('osFamilies=' + str(osFamilies))
-		if pageNumber:
-			url_params.append('pageNumber=' + str(pageNumber))
-		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
-		if sorting:
-			url_params.append('sorting=' + str(sorting))
-		if states:
-			url_params.append('states=' + str(states))
-		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
-		if versions:
-			url_params.append('versions=' + str(versions))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def isolate_collectors(self, devices :dict = None, devicesIds :dict = None, organization :str = None) -> tuple[bool, None]:
-
+	def exclusions_metadata(self) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call isolate collector functionality.
-
+		Class ThreatHuntingExclusions
+		Description: Get the metadata and available properties for exclusions configuration. When creating/modifying an exclusion, use the response of this API as a guide for the valid attribute names and values, and their corresponding EDR event types. Every attribute corresponds to an EDR category (for example, Filename attribute corresponds with the File category), and each category is a set of EDR event types. .
+        
 		Args:
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/inventory/isolate-collectors'
-		url_params = []
-		if devices:
-			url_params.append('devices=' + str(devices))
-		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-
-	def list_aggregators(self, ip :str = None, names :dict = None, organization :str = None, versions :dict = None) -> tuple[bool, dict]:
-
-		'''
-		class SystemInventory
-		Description: This API call output the list of aggregators.
-
-		Args:
-			ip: IP. 
-			names: List of aggregators names. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			versions: List of aggregators versions. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
+		validate_params("exclusions_metadata", locals())
 
-		'''
-		url = '/management-rest/inventory/list-aggregators'
-		url_params = []
-		if ip:
-			url_params.append('ip=' + str(ip))
-		if names:
-			url_params.append('names=' + str(names))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if versions:
-			url_params.append('versions=' + str(versions))
-		url += '?' + '&'.join(url_params)
+		url = '/management-rest/threat-hunting-exclusions/exclusions-metadata'
 		return fortiedr_connection.get(url)
 
-
-	def list_collector_groups(self, organization :str = None) -> tuple[bool, dict]:
-
+	def exclusions_search(self, searchText: str, organization: str = None, os: dict = None) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call output the collectors groups.
-
+		Class ThreatHuntingExclusions
+		Description: Free-text search of exclusions.
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			os (dict): OS identifiers list..
+			searchText (str): The free text search string. The API will return every exclusion list that contains this string, or contains an exclusion with any field that contains it..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
-		url = '/management-rest/inventory/list-collector-groups'
+		validate_params("exclusions_search", locals())
+
+		url = '/management-rest/threat-hunting-exclusions/exclusions-search'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
+		if os:
+			url_params.append('os=' + os)
+		if searchText:
+			url_params.append('searchText=' + searchText)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
+class ThreatHuntingSettings:
+	'''API to configure Threat Hunting Settings.'''
 
-	def list_collectors(self, cloudAccounts :dict = None, cloudProviders :dict = None, clusters :dict = None, collectorGroups :dict = None, collectorGroupsIds :dict = None, collectorType :str = None, devices :dict = None, devicesIds :dict = None, firstSeen :str = None, hasCrashDumps :bool = None, ips :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, loggedUser :str = None, operatingSystems :dict = None, organization :str = None, osFamilies :dict = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, states :dict = None, strictMode :bool = None, versions :dict = None) -> tuple[bool, dict]:
-
+	def threat_hunting_metadata(self) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call outputs a list of the Collectors in the system. Use the input parameters to filter the list.
-
+		Class ThreatHuntingSettings
+		Description: Get the Threat Hunting Settings metadata object, listing the available configuration options (Category and Event Types)..
+        
 		Args:
-			cloudAccounts: Specifies the list cloud account names. 
-			cloudProviders: Specifies the list of cloud providers: AWS, Azure, GCP. 
-			clusters: Specifies the list of cluster. 
-			collectorGroups: Specifies the list of collector group names and retrieves collectors under thegiven groups. 
-			collectorGroupsIds: Specifies the list of collector group Ids and retrieves collectors under thegiven groups. 
-			collectorType: Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			firstSeen: Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			hasCrashDumps: Retrieves collectors that have crash dumps. 
-			ips: Specifies the list of IP values. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			loggedUser: Specifies the user that was logged when the event occurred. 
-			operatingSystems: Specifies the list of specific operating systems. For example, Windows 7 Pro. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			osFamilies: Specifies the list of operating system families: Windows, Windows Server or OS X. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			states: Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, Pending Reboot, Isolated, Expired, Migrated or Pending Migration. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			versions: Specifies the list of collector versions. 
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
-		url = '/management-rest/inventory/list-collectors'
-		url_params = []
-		if cloudAccounts:
-			url_params.append('cloudAccounts=' + str(cloudAccounts))
-		if cloudProviders:
-			url_params.append('cloudProviders=' + str(cloudProviders))
-		if clusters:
-			url_params.append('clusters=' + str(clusters))
-		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
-		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + str(collectorGroupsIds))
-		if collectorType:
-			url_params.append('collectorType=' + str(collectorType))
-		if devices:
-			url_params.append('devices=' + str(devices))
-		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
-		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
-		if hasCrashDumps:
-			url_params.append('hasCrashDumps=' + str(hasCrashDumps))
-		if ips:
-			url_params.append('ips=' + str(ips))
-		if itemsPerPage:
-			url_params.append('itemsPerPage=' + str(itemsPerPage))
-		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
-		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
-		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
-		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if osFamilies:
-			url_params.append('osFamilies=' + str(osFamilies))
-		if pageNumber:
-			url_params.append('pageNumber=' + str(pageNumber))
-		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
-		if sorting:
-			url_params.append('sorting=' + str(sorting))
-		if states:
-			url_params.append('states=' + str(states))
-		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
-		if versions:
-			url_params.append('versions=' + str(versions))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
+		validate_params("threat_hunting_metadata", locals())
 
-	def list_cores(self, deploymentModes :dict = None, hasCrashDumps :bool = None, ip :str = None, names :dict = None, organization :str = None, versions :dict = None) -> tuple[bool, dict]:
+		url = '/management-rest/threat-hunting-settings/threat-hunting-metadata'
+		return fortiedr_connection.get(url)
 
+	def get_threat_hunting_profile(self, organization: str, ) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call output the list of cores.
-
+		Class ThreatHuntingSettings
+		Description: Get the list of Threat Hunting Setting profiles..
+        
 		Args:
-			deploymentModes: List of cores deployments modes. 
-			hasCrashDumps: Has crash dumps. 
-			ip: IP. 
-			names: List of cores names. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			versions: List of cores versions. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
-		url = '/management-rest/inventory/list-cores'
+		validate_params("get_threat_hunting_profile", locals())
+
+		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 		url_params = []
-		if deploymentModes:
-			url_params.append('deploymentModes=' + str(deploymentModes))
-		if hasCrashDumps:
-			url_params.append('hasCrashDumps=' + str(hasCrashDumps))
-		if ip:
-			url_params.append('ip=' + str(ip))
-		if names:
-			url_params.append('names=' + str(names))
 		if organization:
-			url_params.append('organization=' + str(organization))
-		if versions:
-			url_params.append('versions=' + str(versions))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_repositories(self) -> tuple[bool, dict]:
-
+	def upload_threat_hunting_profile(self, associatedCollectorGroupIds: dict = None, name: str = None, newName: str = None, organization: str = None, threatHuntingCategoryList: dict = None) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call output the list of repositories (edrs).
-
+		Class ThreatHuntingSettings
+		Description: Update Threat Hunting profile.
+        
 		Args:
-			deploymentModes: List of cores deployments modes. 
-			hasCrashDumps: Has crash dumps. 
-			ip: IP. 
-			names: List of cores names. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			versions: List of cores versions. 
+			threatHuntingUpdateRequest (Object): Check 'threatHuntingUpdateRequest' in the API documentation for further information.
 
+		Returns:
+			bool: Status of the request (True or False). 
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/inventory/list-repositories'
-		return fortiedr_connection.get(url)
+		validate_params("upload_threat_hunting_profile", locals())
 
+		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 
-	def list_unmanaged_devices(self, itemsPerPage :int = None, organization :str = None, pageNumber :int = None, sorting :str = None, strictMode :bool = None) -> tuple[bool, dict]:
+		threatHuntingUpdateRequest = {
+			"associatedCollectorGroupIds": associatedCollectorGroupIds,
+			"name": name,
+			"newName": newName,
+			"organization": organization,
+			"threatHuntingCategoryList": threatHuntingCategoryList,
+		}
+		return fortiedr_connection.upload(url, threatHuntingUpdateRequest)
 
+	def delete_threat_hunting_profile(self, name: str, organization: str, ) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call outputs a list of the unmanaged devices in the system.
-
+		Class ThreatHuntingSettings
+		Description: Deletes a Threat Hunting profile..
+        
 		Args:
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
+			name (str): To be deleted profile's name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			None: This function does not return any data.
 		'''
-		url = '/management-rest/inventory/list-unmanaged-devices'
+		validate_params("delete_threat_hunting_profile", locals())
+
+		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 		url_params = []
-		if itemsPerPage:
-			url_params.append('itemsPerPage=' + str(itemsPerPage))
+		if name:
+			url_params.append('name=' + name)
 		if organization:
-			url_params.append('organization=' + str(organization))
-		if pageNumber:
-			url_params.append('pageNumber=' + str(pageNumber))
-		if sorting:
-			url_params.append('sorting=' + str(sorting))
-		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
-
-	def move_collectors(self, targetCollectorGroup : str, collectorIds :dict = None, collectorSIDs :dict = None, collectors :dict = None, forceAssign :bool = None, organization :str = None) -> tuple[bool, None]:
+		return fortiedr_connection.delete(url)
 
+	def threat_hunting_profile_clone(self, cloneProfileName: str, existingProfileName: str, organization: str, ) -> tuple[bool, None]:
 		'''
-		class SystemInventory
-		Description: This API call move collector between groups.
-
+		Class ThreatHuntingSettings
+		Description: Clone a Threat Hunting Settings profile..
+        
 		Args:
-			collectorIds: value = Array of collectors Ids. To move collectors from one organization to another. 
-			collectorSIDs: value = Array of collectors SIDS. To move collectors from one organization to another. 
-			collectors: Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>). 
-			forceAssign: Indicates whether to force the assignment even if the organization of the target Collector group is under migration. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			targetCollectorGroup: Collector group. To move collectors from one organization to another, please add the organization name before the target collector group (<organization-name>\\<collector-group-name>). 
+			cloneProfileName (str): Cloned profile name..
+			existingProfileName (str): Existing profile name..
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/inventory/move-collectors'
+		validate_params("threat_hunting_profile_clone", locals())
+
+		url = '/management-rest/threat-hunting-settings/threat-hunting-profile-clone'
 		url_params = []
-		if collectorIds:
-			url_params.append('collectorIds=' + str(collectorIds))
-		if collectorSIDs:
-			url_params.append('collectorSIDs=' + str(collectorSIDs))
-		if collectors:
-			url_params.append('collectors=' + str(collectors))
-		if forceAssign:
-			url_params.append('forceAssign=' + str(forceAssign))
+		if cloneProfileName:
+			url_params.append('cloneProfileName=' + cloneProfileName)
+		if existingProfileName:
+			url_params.append('existingProfileName=' + existingProfileName)
 		if organization:
-			url_params.append('organization=' + str(organization))
-		if targetCollectorGroup:
-			url_params.append('targetCollectorGroup=' + str(targetCollectorGroup))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-
-	def system_logs(self) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url)
 
+	def threat_hunting_profile_assign_collector_groups(self, associatedCollectorGroupIds: dict = None, name: str = None, organization: str = None) -> tuple[bool, list]:
 		'''
-		class SystemInventory
-		Description: This API call retrieves a system logs.
-
-		Args:
-			collectorIds: value = Array of collectors Ids. To move collectors from one organization to another. 
-			collectorSIDs: value = Array of collectors SIDS. To move collectors from one organization to another. 
-			collectors: Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>). 
-			forceAssign: Indicates whether to force the assignment even if the organization of the target Collector group is under migration. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			targetCollectorGroup: Collector group. To move collectors from one organization to another, please add the organization name before the target collector group (<organization-name>\\<collector-group-name>). 
-
-		'''
-		url = '/management-rest/inventory/system-logs'
-		return fortiedr_connection.get(url)
-
-
-	def toggle_collectors(self, enable : bool, cloudAccounts :dict = None, cloudProviders :dict = None, clusters :dict = None, collectorGroups :dict = None, collectorGroupsIds :dict = None, collectorType :str = None, devices :dict = None, devicesIds :dict = None, firstSeen :str = None, hasCrashDumps :bool = None, ips :dict = None, itemsPerPage :int = None, lastSeenEnd :str = None, lastSeenStart :str = None, loggedUser :str = None, operatingSystems :dict = None, organization :str = None, osFamilies :dict = None, pageNumber :int = None, showExpired :bool = None, sorting :str = None, states :dict = None, strictMode :bool = None, versions :dict = None) -> tuple[bool, str]:
-
-		'''
-		class SystemInventory
-		Description: This API call enables/disables a Collector(s). You must specify whether the Collector is to be enabled or disabled.
-
+		Class ThreatHuntingSettings
+		Description: Update Threat Hunting profile assigned collector groups. Returns the updated list of assigned collector groups..
+        
 		Args:
-			cloudAccounts: Specifies the list cloud account names. 
-			cloudProviders: Specifies the list of cloud providers: AWS, Azure, GCP. 
-			clusters: Specifies the list of cluster. 
-			collectorGroups: Specifies the list of collector group names and retrieves collectors under thegiven groups. 
-			collectorGroupsIds: Specifies the list of collector group Ids and retrieves collectors under thegiven groups. 
-			collectorType: Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default. 
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			enable: Toggle enable. 
-			firstSeen: Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			hasCrashDumps: Retrieves collectors that have crash dumps. 
-			ips: Specifies the list of IP values. 
-			itemsPerPage: An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000. 
-			lastSeenEnd: Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			lastSeenStart: Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss. 
-			loggedUser: Specifies the user that was logged when the event occurred. 
-			operatingSystems: Specifies the list of specific operating systems. For example, Windows 7 Pro. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			osFamilies: Specifies the list of operating system families: Windows, Windows Server or OS X. 
-			pageNumber: An integer used for paging that indicates the required page number. 
-			showExpired: Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired. 
-			sorting: Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on. 
-			states: Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, Pending Reboot, Isolated, Expired, Migrated or Pending Migration. 
-			strictMode: A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False. 
-			versions: Specifies the list of collector versions. 
+			threatHuntingAssignGroupsRequest (Object): Check 'threatHuntingAssignGroupsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			str
-
-		'''
-		url = '/management-rest/inventory/toggle-collectors'
-		url_params = []
-		if cloudAccounts:
-			url_params.append('cloudAccounts=' + str(cloudAccounts))
-		if cloudProviders:
-			url_params.append('cloudProviders=' + str(cloudProviders))
-		if clusters:
-			url_params.append('clusters=' + str(clusters))
-		if collectorGroups:
-			url_params.append('collectorGroups=' + str(collectorGroups))
-		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + str(collectorGroupsIds))
-		if collectorType:
-			url_params.append('collectorType=' + str(collectorType))
-		if devices:
-			url_params.append('devices=' + str(devices))
-		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
-		if enable:
-			url_params.append('enable=' + str(enable))
-		if firstSeen:
-			url_params.append('firstSeen=' + str(firstSeen))
-		if hasCrashDumps:
-			url_params.append('hasCrashDumps=' + str(hasCrashDumps))
-		if ips:
-			url_params.append('ips=' + str(ips))
-		if itemsPerPage:
-			url_params.append('itemsPerPage=' + str(itemsPerPage))
-		if lastSeenEnd:
-			url_params.append('lastSeenEnd=' + str(lastSeenEnd))
-		if lastSeenStart:
-			url_params.append('lastSeenStart=' + str(lastSeenStart))
-		if loggedUser:
-			url_params.append('loggedUser=' + str(loggedUser))
-		if operatingSystems:
-			url_params.append('operatingSystems=' + str(operatingSystems))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if osFamilies:
-			url_params.append('osFamilies=' + str(osFamilies))
-		if pageNumber:
-			url_params.append('pageNumber=' + str(pageNumber))
-		if showExpired:
-			url_params.append('showExpired=' + str(showExpired))
-		if sorting:
-			url_params.append('sorting=' + str(sorting))
-		if states:
-			url_params.append('states=' + str(states))
-		if strictMode:
-			url_params.append('strictMode=' + str(strictMode))
-		if versions:
-			url_params.append('versions=' + str(versions))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-
-	def unisolate_collectors(self, devices :dict = None, devicesIds :dict = None, organization :str = None) -> tuple[bool, None]:
-
+			list
 		'''
-		class SystemInventory
-		Description: This API call isolate collector functionality.
+		validate_params("threat_hunting_profile_assign_collector_groups", locals())
 
-		Args:
-			devices: Specifies the list of device names. 
-			devicesIds: Specifies the list of device ids. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
+		url = '/management-rest/threat-hunting-settings/threat-hunting-profile/collector-groups'
 
-		'''
-		url = '/management-rest/inventory/unisolate-collectors'
-		url_params = []
-		if devices:
-			url_params.append('devices=' + str(devices))
-		if devicesIds:
-			url_params.append('devicesIds=' + str(devicesIds))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
+		threatHuntingAssignGroupsRequest = {
+			"associatedCollectorGroupIds": associatedCollectorGroupIds,
+			"name": name,
+			"organization": organization,
+		}
+		return fortiedr_connection.upload(url, threatHuntingAssignGroupsRequest)
 
 class ThreatHunting:
 	'''API for Activity events'''
 
 	def counts(self, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
-
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API call outputs EDR total events for every EDR category.
-
+        
 		Args:
-			edrRequest: edrRequest. 
-			accountId: Account ID. 
-			category: Specifies the category name. All is the default value. 
-			devices: Specifies the devices name list. 
-			filters: Specifies the filters list that available for the user based on the category selected 2. Specifies filters to add to the query.. 
-			fromTime: Specifies events start at creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
-			itemsPerPage: Specifies the Threat Hunting chunck size to retrieve with each call. The default value is 100. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies: ��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly. ��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: Specifies the Threat Hunting start index number to retrieve from. The default value is 0. 
-			query: Specifies the search lucene like query. 
-			sorting: Specifies the Threat Hunting sorting. 
-			time: Specifies the time period of the events. 
-			toTime: Specifies events up to a creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
+			edrRequest (Object): Check 'edrRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("counts", locals())
+
 		url = '/management-rest/threat-hunting/counts'
-		url_params = []
-		url += '?' + '&'.join(url_params)
+
 		edrRequest = {
-			'accountId': accountId,
-			'category': category,
-			'devices': devices,
-			'filters': filters,
-			'fromTime': fromTime,
-			'itemsPerPage': itemsPerPage,
-			'organization': organization,
-			'pageNumber': pageNumber,
-			'query': query,
-			'sorting': sorting,
-			'time': time,
-			'toTime': toTime
+			"accountId": str(accountId),
+			"category": category,
+			"devices": devices,
+			"filters": filters,
+			"fromTime": fromTime,
+			"itemsPerPage": str(itemsPerPage),
+			"organization": organization,
+			"pageNumber": str(pageNumber),
+			"query": query,
+			"sorting": sorting,
+			"time": time,
+			"toTime": toTime,
 		}
-		return fortiedr_connection.send(url, edrRequest)
-
-
-	def create_or_edit_tag(self, newTagName: str, organization: str = None, tagId: int = None, tagName: str = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, edrRequest)
 
+	def create_or_edit_tag(self, newTagName: str = None, organization: str = None, tagId: int = None, tagName: str = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API creates or edits the saved queries tag.
-
+        
 		Args:
-			createOrEditTagRequest: createOrEditTagRequest. 
-			newTagName: Specifies the new tag name. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies: ��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly. ��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			tagId: Specifies the tag ID for editing.. 
-			tagName: Specifies the tag name for editing.. 
+			createOrEditTagRequest (Object): Check 'createOrEditTagRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("create_or_edit_tag", locals())
+
 		url = '/management-rest/threat-hunting/create-or-edit-tag'
-		url_params = []
-		url += '?' + '&'.join(url_params)
+
 		createOrEditTagRequest = {
-			'newTagName': newTagName,
-			'organization': organization,
-			'tagId': tagId,
-			'tagName': tagName
+			"newTagName": newTagName,
+			"organization": organization,
+			"tagId": str(tagId),
+			"tagName": tagName,
 		}
-		return fortiedr_connection.send(url, createOrEditTagRequest)
-
-
-	def customize_fortinet_query(self, id :int = None, queryToEdit :str = None, dayOfMonth: int = None, dayOfWeek: int = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, organization: str = None, scheduled: bool = None, state: bool = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, createOrEditTagRequest)
 
+	def customize_fortinet_query(self, id: int = None, dayOfMonth: int = None, dayOfWeek: int = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, organization: str = None, scheduled: bool = None, state: bool = None, time: str = None, toTime: str = None, queryToEdit: str = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API customizes the scheduling properties of a Fortinet query.
-
+        
 		Args:
-			id: Specifies the query ID to edit. 
-			ootbQueryCustomizeRequest: ootbQueryCustomizeRequest. 
-			dayOfMonth: Specifies the day of the month for the scheduled query. The value must be between 1 and 28. The properties scheduled and frequencyUnit must be true and Month respectively. 
-			dayOfWeek: Specifies the day of the week for the scheduled query. The value must be between 0 and 6. 0 is Sunday and 6 is Saturday. The properties scheduled and frequencyUnit must be true and Week respectively. 
-			forceSaving: A true/false parameter indicating whether to force the save, even when there is a large quantity of query results. 
-			frequency: Specifies the query frequency for the scheduled query. The scheduled property must be true. 
-			frequencyUnit: Specifies the query frequency unit. The scheduled property must be true. 
-			fromTime: Specifies events starting from this creation time. Specify the timestamp using the yyyy-MM-dd HH:mm:ss format. The 'time' value must be 'custom'. 
-			hour: Specifies the hour of the week for the scheduled query. The value must be between 0 and 23. The properties scheduled and frequencyUnit must be true and Day/Week/Month respectively. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			scheduled: Specifies whether the query is scheduled. False by default. 
-			state: A true/false parameter indicating whether the query state is enabled. True by default. 
-			time: Specifies the time period of the Threat Hunting events. The scheduled property must be false. 
-			toTime: Specifies events up to a creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
-			queryToEdit: Specifies the query name to edit. 
+			id (int): Specifies the query ID to edit.
+			ootbQueryCustomizeRequest (Object): Check 'ootbQueryCustomizeRequest' in the API documentation for further information.
+			queryToEdit (str): Specifies the query name to edit.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("customize_fortinet_query", locals())
+
 		url = '/management-rest/threat-hunting/customize-fortinet-query'
 		url_params = []
 		if id:
 			url_params.append('id=' + str(id))
 		if queryToEdit:
-			url_params.append('queryToEdit=' + str(queryToEdit))
+			url_params.append('queryToEdit=' + queryToEdit)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
 
-	def delete_saved_queries(self, deleteAll :bool = None, deleteFromCommunity :bool = None, organization :str = None, queryIds :dict = None, queryNames :dict = None, scheduled :bool = None, source :dict = None) -> tuple[bool, None]:
+		ootbQueryCustomizeRequest = {
+			"dayOfMonth": str(dayOfMonth),
+			"dayOfWeek": str(dayOfWeek),
+			"forceSaving": forceSaving,
+			"frequency": str(frequency),
+			"frequencyUnit": frequencyUnit,
+			"fromTime": fromTime,
+			"hour": str(hour),
+			"organization": organization,
+			"scheduled": scheduled,
+			"state": state,
+			"time": time,
+			"toTime": toTime,
+		}
+		return fortiedr_connection.upload(url, ootbQueryCustomizeRequest)
 
+	def delete_saved_queries(self, deleteAll: bool = None, deleteFromCommunity: bool = None, organization: str = None, queryIds: dict = None, queryNames: dict = None, scheduled: bool = None, source: dict = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API deletes the saved queries.
-
+        
 		Args:
-			deleteAll: A true/false parameter indicating whether all queries should be deleted. False by default. 
-			deleteFromCommunity: A true/false parameter indicating if whether to delete a query from the FortiEDR Community also. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			queryIds: Specifies the query IDs list. 
-			queryNames: Specifies the query names list. 
-			scheduled: A true/false parameter indicating whether the query is scheduled. 
-			source: Specifies the query source list. 
+			deleteAll (bool): A true/false parameter indicating whether all queries should be deleted. False by default.
+			deleteFromCommunity (bool): A true/false parameter indicating if whether to delete a query from the FortiEDR Community also.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			queryIds (dict): Specifies the query IDs list.
+			queryNames (dict): Specifies the query names list.
+			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
+			source (dict): Specifies the query source list.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_saved_queries", locals())
+
 		url = '/management-rest/threat-hunting/delete-saved-queries'
 		url_params = []
 		if deleteAll:
-			url_params.append('deleteAll=' + str(deleteAll))
+			url_params.append('deleteAll=' + deleteAll)
 		if deleteFromCommunity:
-			url_params.append('deleteFromCommunity=' + str(deleteFromCommunity))
+			url_params.append('deleteFromCommunity=' + deleteFromCommunity)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if queryIds:
-			url_params.append('queryIds=' + str(queryIds))
+			url_params.append('queryIds=' + queryIds)
 		if queryNames:
-			url_params.append('queryNames=' + str(queryNames))
+			url_params.append('queryNames=' + queryNames)
 		if scheduled:
-			url_params.append('scheduled=' + str(scheduled))
+			url_params.append('scheduled=' + scheduled)
 		if source:
-			url_params.append('source=' + str(source))
+			url_params.append('source=' + source)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def delete_tags(self, organization :str = None, tagIds :dict = None, tagNames :dict = None) -> tuple[bool, None]:
-
+	def delete_tags(self, organization: str = None, tagIds: dict = None, tagNames: dict = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API deletes the saved queries tags.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			tagIds: Specifies the tag ID list. 
-			tagNames: Specifies the tag name list. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			tagIds (dict): Specifies the tag ID list.
+			tagNames (dict): Specifies the tag name list.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_tags", locals())
+
 		url = '/management-rest/threat-hunting/delete-tags'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if tagIds:
-			url_params.append('tagIds=' + str(tagIds))
+			url_params.append('tagIds=' + tagIds)
 		if tagNames:
-			url_params.append('tagNames=' + str(tagNames))
+			url_params.append('tagNames=' + tagNames)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def facets(self, facets: dict, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, dict]:
-
+	def facets(self, accountId: int = None, category: str = None, devices: dict = None, facets: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API retrieves EDR total events for every EDR facet item.
-
+        
 		Args:
-			facetsRequest: facetsRequest. 
-			accountId: Account ID. 
-			category: Specifies the category name. All is the default value. 
-			devices: Specifies the devices name list. 
-			facets: Specifies the facets list that available for the user based on the category selected 2. Specifies facets to add to the query.. 
-			filters: Specifies the filters list that available for the user based on the category selected 2. Specifies filters to add to the query.. 
-			fromTime: Specifies events start at creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
-			itemsPerPage: Specifies the Threat Hunting chunck size to retrieve with each call. The default value is 100. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies: ��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly. ��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: Specifies the Threat Hunting start index number to retrieve from. The default value is 0. 
-			query: Specifies the search lucene like query. 
-			sorting: Specifies the Threat Hunting sorting. 
-			time: Specifies the time period of the events. 
-			toTime: Specifies events up to a creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
+			facetsRequest (Object): Check 'facetsRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("facets", locals())
+
 		url = '/management-rest/threat-hunting/facets'
-		url_params = []
-		url += '?' + '&'.join(url_params)
+
 		facetsRequest = {
-			'accountId': accountId,
-			'category': category,
-			'devices': devices,
-			'facets': facets,
-			'filters': filters,
-			'fromTime': fromTime,
-			'itemsPerPage': itemsPerPage,
-			'organization': organization,
-			'pageNumber': pageNumber,
-			'query': query,
-			'sorting': sorting,
-			'time': time,
-			'toTime': toTime
+			"accountId": str(accountId),
+			"category": category,
+			"devices": devices,
+			"facets": facets,
+			"filters": filters,
+			"fromTime": fromTime,
+			"itemsPerPage": str(itemsPerPage),
+			"organization": organization,
+			"pageNumber": str(pageNumber),
+			"query": query,
+			"sorting": sorting,
+			"time": time,
+			"toTime": toTime,
 		}
-		return fortiedr_connection.send(url, facetsRequest)
-
-
-	def list_saved_queries(self, organization :str = None, scheduled :bool = None, source :dict = None) -> tuple[bool, dict]:
+		return fortiedr_connection.upload(url, facetsRequest)
 
+	def list_saved_queries(self, organization: str = None, scheduled: bool = None, source: dict = None) -> tuple[bool, list]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API retrieves the existing saved queries list.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			scheduled: A true/false parameter indicating whether the query is scheduled. 
-			source: Specifies the query source list. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
+			source (dict): Specifies the query source list.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_saved_queries", locals())
+
 		url = '/management-rest/threat-hunting/list-saved-queries'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if scheduled:
-			url_params.append('scheduled=' + str(scheduled))
+			url_params.append('scheduled=' + scheduled)
 		if source:
-			url_params.append('source=' + str(source))
+			url_params.append('source=' + source)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_tags(self, organization :str = None) -> tuple[bool, dict]:
-
+	def list_tags(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API retrieves the existing saved queries tag list.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_tags", locals())
+
 		url = '/management-rest/threat-hunting/list-tags'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def save_query(self, id :int = None, queryToEdit :str = None, category: str = None, classification: str = None, collectorNames: dict = None, community: bool = None, dayOfMonth: int = None, dayOfWeek: int = None, description: str = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, name: str = None, organization: str = None, query: str = None, scheduled: bool = None, state: bool = None, tagIds: dict = None, tagNames: dict = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
-
+	def save_query(self, id: int = None, queryToEdit: str = None, category: str = None, classification: str = None, collectorNames: dict = None, community: bool = None, dayOfMonth: int = None, dayOfWeek: int = None, description: str = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, name: str = None, organization: str = None, query: str = None, scheduled: bool = None, state: bool = None, tagIds: dict = None, tagNames: dict = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API saves the query.
-
+        
 		Args:
-			id: Specifies the query ID to edit. 
-			queryToEdit: Specifies the query name to edit. 
-			saveQueryRequest: saveQueryRequest. 
-			category: Specifies the category name. All is the default value. 
-			classification: Specifies the event classification. The scheduled property must be true. 
-			collectorNames: Specifies the Collector names. 
-			community: A true/false parameter indicating whether the query is available to the entire FortiEDR Community. False by default. 
-			dayOfMonth: Specifies the day of the month for the scheduled query. The value must be between 1 and 28. The properties scheduled and frequencyUnit must be true and Month respectively. 
-			dayOfWeek: Specifies the day of the week for the scheduled query. The value must be between 0 and 6. 0 is Sunday and 6 is Saturday. The properties scheduled and frequencyUnit must be true and Week respectively. 
-			description: Specifies the description. 
-			forceSaving: A true/false parameter indicating whether to force the save, even when there is a large quantity of query results. 
-			frequency: Specifies the query frequency for the scheduled query. The scheduled property must be true. 
-			frequencyUnit: Specifies the query frequency unit. The scheduled property must be true. 
-			fromTime: Specifies events starting from this creation time. Specify the timestamp using the yyyy-MM-dd HH:mm:ss format. The 'time' value must be 'custom'. 
-			hour: Specifies the hour of the day for the scheduled query. The value must be between 0 and 23. The properties scheduled and frequencyUnit must be true and Day/Week/Month respectively. 
-			name: Specifies the name of the query being saved. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			query: Specifies the Lucene-like search query. 
-			scheduled: Specifies whether the query is scheduled. False by default. 
-			state: A true/false parameter indicating whether the query state is enabled. True by default. 
-			tagIds: Specifies the query tag ids. 
-			tagNames: Specifies the query tag names. 
-			time: Specifies the time period of the Threat Hunting events. The scheduled property must be false. 
-			toTime: Specifies events up to a creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
+			id (int): Specifies the query ID to edit.
+			queryToEdit (str): Specifies the query name to edit.
+			saveQueryRequest (Object): Check 'saveQueryRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("save_query", locals())
+
 		url = '/management-rest/threat-hunting/save-query'
 		url_params = []
 		if id:
 			url_params.append('id=' + str(id))
 		if queryToEdit:
-			url_params.append('queryToEdit=' + str(queryToEdit))
+			url_params.append('queryToEdit=' + queryToEdit)
 		url += '?' + '&'.join(url_params)
+
 		saveQueryRequest = {
-			'category': category,
-			'classification': classification,
-			'collectorNames': collectorNames,
-			'community': community,
-			'dayOfMonth': dayOfMonth,
-			'dayOfWeek': dayOfWeek,
-			'description': description,
-			'forceSaving': forceSaving,
-			'frequency': frequency,
-			'frequencyUnit': frequencyUnit,
-			'fromTime': fromTime,
-			'hour': hour,
-			'name': name,
-			'organization': organization,
-			'query': query,
-			'scheduled': scheduled,
-			'state': state,
-			'tagIds': tagIds,
-			'tagNames': tagNames,
-			'time': time,
-			'toTime': toTime
+			"category": category,
+			"classification": classification,
+			"collectorNames": collectorNames,
+			"community": community,
+			"dayOfMonth": str(dayOfMonth),
+			"dayOfWeek": str(dayOfWeek),
+			"description": description,
+			"forceSaving": forceSaving,
+			"frequency": str(frequency),
+			"frequencyUnit": frequencyUnit,
+			"fromTime": fromTime,
+			"hour": str(hour),
+			"name": name,
+			"organization": organization,
+			"query": query,
+			"scheduled": scheduled,
+			"state": state,
+			"tagIds": tagIds,
+			"tagNames": tagNames,
+			"time": time,
+			"toTime": toTime,
 		}
-		return fortiedr_connection.send(url, saveQueryRequest)
-
-
-	def search(self, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, dict]:
+		return fortiedr_connection.upload(url, saveQueryRequest)
 
+	def search(self, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API call outputs a list of Activity events from middleware..
-
+        
 		Args:
-			edrRequest: edrRequest. 
-			accountId: Account ID. 
-			category: Specifies the category name. All is the default value. 
-			devices: Specifies the devices name list. 
-			filters: Specifies the filters list that available for the user based on the category selected 2. Specifies filters to add to the query.. 
-			fromTime: Specifies events start at creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
-			itemsPerPage: Specifies the Threat Hunting chunck size to retrieve with each call. The default value is 100. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies: ��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly. ��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			pageNumber: Specifies the Threat Hunting start index number to retrieve from. The default value is 0. 
-			query: Specifies the search lucene like query. 
-			sorting: Specifies the Threat Hunting sorting. 
-			time: Specifies the time period of the events. 
-			toTime: Specifies events up to a creation time. Specify the date using the yyyy-MM-dd HH:mm:ss format. The 'time' filed must be 'custom'. 
+			edrRequest (Object): Check 'edrRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("search", locals())
+
 		url = '/management-rest/threat-hunting/search'
-		url_params = []
-		url += '?' + '&'.join(url_params)
+
 		edrRequest = {
-			'accountId': accountId,
-			'category': category,
-			'devices': devices,
-			'filters': filters,
-			'fromTime': fromTime,
-			'itemsPerPage': itemsPerPage,
-			'organization': organization,
-			'pageNumber': pageNumber,
-			'query': query,
-			'sorting': sorting,
-			'time': time,
-			'toTime': toTime
+			"accountId": str(accountId),
+			"category": category,
+			"devices": devices,
+			"filters": filters,
+			"fromTime": fromTime,
+			"itemsPerPage": str(itemsPerPage),
+			"organization": organization,
+			"pageNumber": str(pageNumber),
+			"query": query,
+			"sorting": sorting,
+			"time": time,
+			"toTime": toTime,
 		}
-		return fortiedr_connection.send(url, edrRequest)
-
-
-	def set_query_state(self, state : bool, markAll :bool = None, organization :str = None, queryIds :dict = None, queryNames :dict = None, source :dict = None) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, edrRequest)
 
+	def set_query_state(self, state: bool, markAll: bool = None, organization: str = None, queryIds: dict = None, queryNames: dict = None, source: dict = None) -> tuple[bool, None]:
 		'''
-		class ThreatHunting
+		Class ThreatHunting
 		Description: This API updates the scheduled saved query state.
-
+        
 		Args:
-			markAll: A true/false parameter indicating whether all queries should be marked with the same value as 'state' property. False by default. 
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
-			queryIds: Specifies the query ID list. 
-			queryNames: Specifies the query name list. 
-			source: Specifies the query source list. 
-			state: A true/false parameter indicating whether to save the query as enabled. 
+			markAll (bool): A true/false parameter indicating whether all queries should be marked with the same value as 'state' property. False by default.
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
+			queryIds (dict): Specifies the query ID list.
+			queryNames (dict): Specifies the query name list.
+			source (dict): Specifies the query source list.
+			state (bool): A true/false parameter indicating whether to save the query as enabled.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("set_query_state", locals())
+
 		url = '/management-rest/threat-hunting/set-query-state'
 		url_params = []
 		if markAll:
-			url_params.append('markAll=' + str(markAll))
+			url_params.append('markAll=' + markAll)
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if queryIds:
-			url_params.append('queryIds=' + str(queryIds))
+			url_params.append('queryIds=' + queryIds)
 		if queryNames:
-			url_params.append('queryNames=' + str(queryNames))
+			url_params.append('queryNames=' + queryNames)
 		if source:
-			url_params.append('source=' + str(source))
+			url_params.append('source=' + source)
 		if state:
-			url_params.append('state=' + str(state))
+			url_params.append('state=' + state)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-class ThreatHuntingExclusions:
-	'''API to create Threat Hunting exclusions.'''
-
-	def send_exclusion(self, exclusionListName: str, exclusions: dict, organization: str) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Creates exclusions..
-
-		Args:
-			createExclusionsRequest: createExclusionsRequest. 
-			exclusionListName: Exclusions created in the request will be associated with this list.. 
-			exclusions: List of exclusions definitions to be created.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusion'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		createExclusionsRequest = {
-			'exclusionListName': exclusionListName,
-			'exclusions': exclusions,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, createExclusionsRequest)
-
-	def insert_exclusions(self, exclusionListName: str, exclusions: dict, organization: str) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Creates exclusions..
-
-		Args:
-			updateExclusionsRequest: updateExclusionsRequest. 
-			exclusionListName: Exclusions created in the request will be associated with this list.. 
-			exclusions: List of exclusions definitions to update.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusion'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		updateExclusionsRequest = {
-			'exclusionListName': exclusionListName,
-			'exclusions': exclusions,
-			'organization': organization
-		}
-		return fortiedr_connection.insert(url, updateExclusionsRequest)
-
-	def delete_exclusion(self, exclusionIds: dict, organization: str) -> tuple[bool, str]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Creates exclusions..
-
-		Args:
-			deleteExclusionsRequest: deleteExclusionsRequest. 
-			exclusionIds: List of exclusion Ids for deletion.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			str
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusion'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		deleteExclusionsRequest = {
-			'exclusionIds': exclusionIds,
-			'organization': organization
-		}
-		return fortiedr_connection.delete(url, deleteExclusionsRequest)
-
-
-	def get_exclusions_list(self, organization : str) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Get the list of Exclusions lists..
-
-		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
-		url_params = []
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
-	def send_exclusions_list(self, name: str, organization: str, collectorGroupIds: dict = None) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Get the list of Exclusions lists..
-
-		Args:
-			createExclusionListRequest: createExclusionListRequest. 
-			collectorGroupIds: The list of Collector group Ids associated with this exclusion list.. 
-			name: Exclusion list name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		createExclusionListRequest = {
-			'collectorGroupIds': collectorGroupIds,
-			'name': name,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, createExclusionListRequest)
-
-	def insert_exclusions_list(self, collectorGroupIds: dict, listName: str, organization: str, newName: str = None) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Get the list of Exclusions lists..
-
-		Args:
-			updateExclusionListRequest: updateExclusionListRequest. 
-			collectorGroupIds: The list of Collector group Ids associated with this exclusion list.. 
-			listName: Exclusions list name.. 
-			newName: Exclusion list new name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		updateExclusionListRequest = {
-			'collectorGroupIds': collectorGroupIds,
-			'listName': listName,
-			'newName': newName,
-			'organization': organization
-		}
-		return fortiedr_connection.insert(url, updateExclusionListRequest)
-
-	def delete_exclusions_list(self, listName : str, organization : str) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Get the list of Exclusions lists..
-
-		Args:
-			listName: Exclusions list name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
-		url_params = []
-		if listName:
-			url_params.append('listName=' + str(listName))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.delete(url)
-
-
-	def exclusions_metadata(self) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Get the metadata and available properties for exclusions configuration. When creating/modifying an exclusion, use the response of this API as a guide for the valid attribute names and values, and their corresponding EDR event types. Every attribute corresponds to an EDR category (for example, Filename attribute corresponds with the File category), and each category is a set of EDR event types. .
-
-		Args:
-			listName: Exclusions list name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-metadata'
-		return fortiedr_connection.get(url)
-
-
-	def exclusions_search(self, searchText : str, organization :str = None, os :dict = None) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingExclusions
-		Description: Free-text search of exclusions.
-
-		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			os: OS identifiers list.. 
-			searchText: The free text search string. The API will return every exclusion list that contains this string, or contains an exclusion with any field that contains it.. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-exclusions/exclusions-search'
-		url_params = []
-		if organization:
-			url_params.append('organization=' + str(organization))
-		if os:
-			url_params.append('os=' + str(os))
-		if searchText:
-			url_params.append('searchText=' + str(searchText))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
-class ThreatHuntingSettings:
-	'''API to configure Threat Hunting Settings.'''
-
-	def threat_hunting_metadata(self) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Get the Threat Hunting Settings metadata object, listing the available configuration options (Category and Event Types)..
-
-		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			os: OS identifiers list.. 
-			searchText: The free text search string. The API will return every exclusion list that contains this string, or contains an exclusion with any field that contains it.. 
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-metadata'
-		return fortiedr_connection.get(url)
-
-
-	def get_threat_hunting_profile(self, organization : str) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Get the list of Threat Hunting Setting profiles..
-
-		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
-		url_params = []
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
-	def send_threat_hunting_profile(self, associatedCollectorGroupIds: dict, name: str, organization: str, threatHuntingCategoryList: dict, newName: str = None) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Get the list of Threat Hunting Setting profiles..
-
-		Args:
-			threatHuntingUpdateRequest: threatHuntingUpdateRequest. 
-			associatedCollectorGroupIds: List of associated collector groups Ids, for example [1,2,3].. 
-			name: Threat Hunting profile name.. 
-			newName: New profile name. Optional.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			threatHuntingCategoryList: Threat Hunting Categories. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		threatHuntingUpdateRequest = {
-			'associatedCollectorGroupIds': associatedCollectorGroupIds,
-			'name': name,
-			'newName': newName,
-			'organization': organization,
-			'threatHuntingCategoryList': threatHuntingCategoryList
-		}
-		return fortiedr_connection.send(url, threatHuntingUpdateRequest)
-
-	def delete_threat_hunting_profile(self, name : str, organization : str) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Get the list of Threat Hunting Setting profiles..
-
-		Args:
-			name: To be deleted profile's name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
-		url_params = []
-		if name:
-			url_params.append('name=' + str(name))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.delete(url)
-
-
-	def threat_hunting_profile_clone(self, cloneProfileName : str, existingProfileName : str, organization : str) -> tuple[bool, None]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Clone a Threat Hunting Settings profile..
-
-		Args:
-			cloneProfileName: Cloned profile name.. 
-			existingProfileName: Existing profile name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-profile-clone'
-		url_params = []
-		if cloneProfileName:
-			url_params.append('cloneProfileName=' + str(cloneProfileName))
-		if existingProfileName:
-			url_params.append('existingProfileName=' + str(existingProfileName))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
-
-	def threat_hunting_profile_assign_collector_groups(self, associatedCollectorGroupIds: dict, name: str, organization: str = None) -> tuple[bool, dict]:
-
-		'''
-		class ThreatHuntingSettings
-		Description: Update Threat Hunting profile assigned collector groups. Returns the updated list of assigned collector groups..
-
-		Args:
-			threatHuntingAssignGroupsRequest: threatHuntingAssignGroupsRequest. 
-			associatedCollectorGroupIds: List of associated collector groups Ids, for example [1,2,3].. 
-			name: Threat Hunting profile name.. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			dict
-
-		'''
-		url = '/management-rest/threat-hunting-settings/threat-hunting-profile/collector-groups'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		threatHuntingAssignGroupsRequest = {
-			'associatedCollectorGroupIds': associatedCollectorGroupIds,
-			'name': name,
-			'organization': organization
-		}
-		return fortiedr_connection.send(url, threatHuntingAssignGroupsRequest)
-
 class Users:
 	'''API to define user'''
 
-	def create_user(self, confirmPassword: str, email: str, firstName: str, lastName: str, password: str, role: str, username: str, organization :str = None, customScript: bool = None, remoteShell: bool = None, restApi: bool = None, title: str = None) -> tuple[bool, None]:
-
+	def create_user(self, organization: str = None, confirmPassword: str = None, customScript: bool = None, email: str = None, firstName: str = None, lastName: str = None, password: str = None, remoteShell: bool = None, restApi: bool = None, role: str = None, title: str = None, username: str = None) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: This API create user in the system. (only for Admin role.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately.. 
-			userRequest: userRequest. 
-			confirmPassword: Specifies the confirm login password. 
-			customScript: Is user can upload custom scripts. 
-			email: Specifies the email of user. 
-			firstName: Specifies the first name of user. 
-			lastName: Specifies the last name of user. 
-			password: Specifies the login password. 
-			remoteShell: Is user can use remote shell. 
-			restApi: Is user can access by rest to the api. 
-			role: Specifies the roles of the user. 
-			title: Specifies the title of user. 
-			username: Specifies the login username of the user. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately..
+			userRequest (Object): Check 'userRequest' in the API documentation for further information.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("create_user", locals())
+
 		url = '/management-rest/users/create-user'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
+
 		userRequest = {
-			'confirmPassword': confirmPassword,
-			'customScript': customScript,
-			'email': email,
-			'firstName': firstName,
-			'lastName': lastName,
-			'password': password,
-			'remoteShell': remoteShell,
-			'restApi': restApi,
-			'role': role,
-			'title': title,
-			'username': username
+			"confirmPassword": confirmPassword,
+			"customScript": customScript,
+			"email": email,
+			"firstName": firstName,
+			"lastName": lastName,
+			"password": password,
+			"remoteShell": remoteShell,
+			"restApi": restApi,
+			"role": role,
+			"title": title,
+			"username": username,
 		}
-		return fortiedr_connection.send(url, userRequest)
-
-
-	def delete_saml_settings(self, organizationNameRequest : str) -> tuple[bool, None]:
+		return fortiedr_connection.upload(url, userRequest)
 
+	def delete_saml_settings(self, organizationNameRequest: str, ) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: Delete SAML authentication settings per organization.
-
+        
 		Args:
-			organizationNameRequest: organizationNameRequest. 
+			organizationNameRequest (str): organizationNameRequest.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_saml_settings", locals())
+
 		url = '/management-rest/users/delete-saml-settings'
 		url_params = []
 		if organizationNameRequest:
-			url_params.append('organizationNameRequest=' + str(organizationNameRequest))
+			url_params.append('organizationNameRequest=' + organizationNameRequest)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def delete_user(self, username : str, organization :str = None) -> tuple[bool, None]:
-
+	def delete_user(self, username: str, organization: str = None) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: This API delete user from the system. Use the input parameters to filter organization.
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			username: Specifies the name of the user. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			username (str): Specifies the name of the user.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("delete_user", locals())
+
 		url = '/management-rest/users/delete-user'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if username:
-			url_params.append('username=' + str(username))
+			url_params.append('username=' + username)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-
-	def get_sp_metadata(self, organization : str) -> tuple[bool, str]:
-
+	def get_sp_metadata(self, organization: str, ) -> tuple[bool, str]:
 		'''
-		class Users
+		Class Users
 		Description: This API call retrieve the FortiEdr metadata by organization.
-
+        
 		Args:
-			organization: organization. 
+			organization (str): organization.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			str
-
 		'''
+		validate_params("get_sp_metadata", locals())
+
 		url = '/management-rest/users/get-sp-metadata'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def list_users(self, organization :str = None) -> tuple[bool, dict]:
-
+	def list_users(self, organization: str = None) -> tuple[bool, list]:
 		'''
-		class Users
+		Class Users
 		Description: This API call outputs a list of the users in the system. Use the input parameters to filter the list.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
-			dict
-
+			list
 		'''
+		validate_params("list_users", locals())
+
 		url = '/management-rest/users/list-users'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-
-	def reset_password(self, username : str, confirmPassword: str, password: str, organization :str = None) -> tuple[bool, None]:
-
+	def reset_password(self, username: str, organization: str = None, confirmPassword: str = None, password: str = None) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: This API reset user password. Use the input parameters to filter organization.
-
+        
 		Args:
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-			userRequest: userRequest. 
-			confirmPassword: Specifies the confirm login password. 
-			password: Specifies the login password. 
-			username: Specifies the name of the user. 
+			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			userRequest (Object): Check 'userRequest' in the API documentation for further information.
+			username (str): Specifies the name of the user.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("reset_password", locals())
+
 		url = '/management-rest/users/reset-password'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if username:
-			url_params.append('username=' + str(username))
+			url_params.append('username=' + username)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
 
+		userRequest = {
+			"confirmPassword": confirmPassword,
+			"password": password,
+		}
+		return fortiedr_connection.insert(url, userRequest)
 
-	def update_saml_settings(self, idpMetadataFile : BinaryIO) -> tuple[bool, None]:
-
+	def update_saml_settings(self, idpMetadataFile: BinaryIO, ) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: Create / Update SAML authentication settings per organization.
-
+        
 		Args:
-			idpMetadataFile: idpMetadataFile. 
+			idpMetadataFile (BinaryIO): idpMetadataFile.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
-		url = '/management-rest/users/update-saml-settings'
-		url_params = []
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
+		validate_params("update_saml_settings", locals())
 
+		url = '/management-rest/users/update-saml-settings'
+		if idpMetadataFile:
+			idpMetadataFile = {'idpMetadataFile': idpMetadataFile}
+		return fortiedr_connection.upload(url, idpMetadataFile, request_type="multipart/form-data")
 
-	def update_user(self, username : str, email: str, firstName: str, lastName: str, role: str, organization :str = None, customScript: bool = None, remoteShell: bool = None, restApi: bool = None, title: str = None) -> tuple[bool, None]:
-
+	def update_user(self, username: str, organization: str = None, customScript: bool = None, email: str = None, firstName: str = None, lastName: str = None, remoteShell: bool = None, restApi: bool = None, role: str = None, title: str = None) -> tuple[bool, None]:
 		'''
-		class Users
+		Class Users
 		Description: This API update user in the system. Use the input parameters to filter organization.
-
+        
 		Args:
-			organization: Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:��� Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.��� each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately.. 
-			userRequest: userRequest. 
-			customScript: Is user can upload custom scripts. 
-			email: Specifies the email of user. 
-			firstName: Specifies the first name of user. 
-			lastName: Specifies the last name of user. 
-			remoteShell: Is user can use remote shell. 
-			restApi: Is user can access by rest to the api. 
-			role: Specifies the roles of the user. 
-			title: Specifies the title of user. 
-			username: Specifies the name of the user. 
+			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
+���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
+���	each ��� Indicates that the operation applies independently to each organization. For example, let's assume that the same user exists in multiple organizations. When each is specified in the organization parameter, then each organization can update this user separately..
+			userRequest (Object): Check 'userRequest' in the API documentation for further information.
+			username (str): Specifies the name of the user.
 
-		Returns: 
+		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
-
 		'''
+		validate_params("update_user", locals())
+
 		url = '/management-rest/users/update-user'
 		url_params = []
 		if organization:
-			url_params.append('organization=' + str(organization))
+			url_params.append('organization=' + organization)
 		if username:
-			url_params.append('username=' + str(username))
+			url_params.append('username=' + username)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.insert(url)
-
-class WorkloadGroups:
-	'''API to define workload groups'''
-
-class Dashboard:
-	'''Dashboard Rest Api Controller'''
-
-	def most_targeted_items(self, organization : str, itemType :str = None, numOfColumns :int = None, numOfDays :int = None) -> tuple[bool, None]:
-
-		'''
-		class dashboardrestapicontroller
-		Description: Returns most targeted devices or most targeted processes, depending on the itemType parameter.
 
-		Args:
-			itemType: Specifies the type of items. 
-			numOfColumns: Specifies the number of columns to present. 
-			numOfDays: Specifies the number of days to present. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/api/dashboard/most-targeted-items'
-		url_params = []
-		if itemType:
-			url_params.append('itemType=' + str(itemType))
-		if numOfColumns:
-			url_params.append('numOfColumns=' + str(numOfColumns))
-		if numOfDays:
-			url_params.append('numOfDays=' + str(numOfDays))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
-
-
-	def unhandled_items(self, organization : str, itemType :str = None) -> tuple[bool, None]:
-
-		'''
-		class dashboardrestapicontroller
-		Description: Returns unhandled devices or unhandled processes, depending on the itemType parameter.
-
-		Args:
-			itemType: Specifies the type of items. 
-			organization: Specifies the name of a specific organization. The value that you specify here must match exactly. 
-
-		Returns: 
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-
-		'''
-		url = '/api/dashboard/unhandled-items'
-		url_params = []
-		if itemType:
-			url_params.append('itemType=' + str(itemType))
-		if organization:
-			url_params.append('organization=' + str(organization))
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		userRequest = {
+			"customScript": customScript,
+			"email": email,
+			"firstName": firstName,
+			"lastName": lastName,
+			"remoteShell": remoteShell,
+			"restApi": restApi,
+			"role": role,
+			"title": title,
+			"username": username,
+		}
+		return fortiedr_connection.insert(url, userRequest)
 
 
 debug = None
 ssl_enabled = True
+organization = None
+api_json_params = None
 
-def disable_ssl():
+def validate_params(function_name, local_params):
+	global api_json_params
+	data_types = {
+		'int': int,
+		'str': str,
+		'dict': dict,
+		'list': list,
+		'set': set
+	}
+	json_params = api_json_params[function_name]
+	for key, value in local_params.items():
+		if key == "self" or value is None: continue
+		t = data_types[json_params[key]]
+		r = str(type(value))
+		if not isinstance(value, t):
+			print(f"Error on defined params!")
+			print(f"Function: {function_name}()")
+			print(f"Param '{key}' should be defined as type '{json_params[key]}', not {r}")
+			exit()
+                        
+def ignore_certificate():
 	global ssl_enabled
 	ssl_enabled = False
 	print("[!] - We strongly advise you to enable SSL validations. Use this at your own risk!")
 
 def enable_debug():
 	global debug
 	debug = True
 
+def set_organization(orgname):
+	global organization
+	organization = orgname
+
 def auth( host: str, user: str, passw: str, org: str = None):
 	global debug
+	global api_json_params
 	global fortiedr_connection
 	login = fedrAuth()
+
+	if org:
+		set_organization(org)
+
 	headers, host = login.get_headers(
 		fedr_host=host,
 		fedr_user=user,
 		fedr_pass=passw,
 		fedr_org=org
 	)
 
 	if headers is None:
 		status = False
 		data = host
 	else:
 		status = True
 		data = 'AUTHENTICATION_SUCCEEDED'
 
-	fortiedr_connection = FortiEDR_API_GW()
-	authentication = fortiedr_connection.conn(headers, host, debug, ssl_enabled)
+		fortiedr_connection = FortiEDR_API_GW()
+		authentication = fortiedr_connection.conn(headers, host, debug, ssl_enabled, organization)
+
+		cur_dir = os.path.dirname(__file__)
+		json_file = f'{cur_dir}/api_parameters.json'
+		with open(json_file, 'r') as fp:
+			api_json_params = json.loads(fp.read())
+
 	return {
 		'status': status,
 		'data': data
-	}
+	}
```

### Comparing `fortiedr-3.0.0/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.5/fortiedr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.0.0
+Version: 3.5
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Fortiedr Python module
-An Open-source python package intended to help on interacting with FortiEDR API.
+# FortiEDR Python module
+An open-source Python package intended to help interact with FortiEDR API.
 
 It was based and tested in FortiEDR Cloud version 6.2.0.0436.
 
-## How do I install FortiEDR Python module?
+See [changelog](CHANGELOG.md) for more.
+
+## How do I install the FortiEDR Python module?
 
 Be sure you have at least Python 3.8 and PIP (https://pypi.org/project/pip/) installed.
 
-After downloading this tool, use pip for installing dependencies using the following command:
+After downloading this tool, use pip to install dependencies using the following command:
 
 ```
 pip install fortiedr
 ```
 
-Or you can download directly from this repo:
+Or you can download it directly from this repo:
 
 ```
 git clone https://github.com/rafaelfoster/fortiedr.git
 
 cd fortiedr
 
 pip3 install .
 ```
 
 ## First steps with fortiedr
 
 First of all, create a Rest API user on FortiEDR Management console:
- * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/5.2.1/administration-guide/776468/users
+ * Create a user with Rest API permissions on FortiEDR Console. You can check this doc for help: https://docs.fortinet.com/document/fortiedr/6.2.0/administration-guide/776468/users
 
  * After creating the user, this newly created user must log in to the Central Manager console and change their initial password before they can be used by Rest API calls.
 
 After creating a user with privileges for interacting with FortiEDR API, you can start using the package by importing the modules you want to your code:
 
 `import fortiedr`
 
@@ -77,10 +79,10 @@
 After credentials are defined and successfully authenticated, you are now able to start consuming FortiEDR API.
 
 The "example.py" file contains some examples of how to use the package.
 
 
 ## How to contribute, provide feedback, or report bugs?
 
-You can e-mail me at fosterr at fortinet (.) com.
+You can e-mail me at rafaelgfoster at gmail (.) com.
 
 Enjoy it!
```

### Comparing `fortiedr-3.0.0/pyproject.toml` & `fortiedr-3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.0.0"
+version = "3.5"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" },
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```


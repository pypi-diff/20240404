# Comparing `tmp/dspace_rest_client-0.1.8-py3-none-any.whl.zip` & `tmp/dspace_rest_client-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17679 bytes, number of entries: 8
+Zip file size: 18786 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       16 b- defN 23-Oct-06 22:49 dspace_rest_client/__init__.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Oct-06 23:09 dspace_rest_client/client.py
+-rw-rw-r--  2.0 unx    46480 b- defN 23-Dec-03 01:17 dspace_rest_client/client.py
 -rw-rw-r--  2.0 unx    18483 b- defN 23-Oct-06 22:49 dspace_rest_client/models.py
--rw-rw-r--  2.0 unx     1475 b- defN 23-Oct-06 23:10 dspace_rest_client-0.1.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     4441 b- defN 23-Oct-06 23:10 dspace_rest_client-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Oct-06 23:10 dspace_rest_client-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 23-Oct-06 23:10 dspace_rest_client-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      702 b- defN 23-Oct-06 23:10 dspace_rest_client-0.1.8.dist-info/RECORD
-8 files, 66637 bytes uncompressed, 16441 bytes compressed:  75.3%
+-rw-rw-r--  2.0 unx     1475 b- defN 23-Dec-03 01:30 dspace_rest_client-0.1.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     4441 b- defN 23-Dec-03 01:30 dspace_rest_client-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Dec-03 01:30 dspace_rest_client-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       19 b- defN 23-Dec-03 01:30 dspace_rest_client-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      702 b- defN 23-Dec-03 01:30 dspace_rest_client-0.1.9.dist-info/RECORD
+8 files, 71708 bytes uncompressed, 17548 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dspace_rest_client/client.py
 Comment: 
 
 Filename: dspace_rest_client/models.py
 Comment: 
 
-Filename: dspace_rest_client-0.1.8.dist-info/LICENSE.txt
+Filename: dspace_rest_client-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.8.dist-info/METADATA
+Filename: dspace_rest_client-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dspace_rest_client-0.1.8.dist-info/WHEEL
+Filename: dspace_rest_client-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dspace_rest_client-0.1.8.dist-info/top_level.txt
+Filename: dspace_rest_client-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.8.dist-info/RECORD
+Filename: dspace_rest_client-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspace_rest_client/client.py

```diff
@@ -10,42 +10,40 @@
 system to a new DSpace 7 repository.
 
 It needs a lot of expansion: resource policies and permissions, validation of prepared objects and responses,
 better abstracting and handling of HAL-like API responses, plus just all the other endpoints and operations implemented.
 
 @author Kim Shepherd <kim@shepherd.nz>
 """
-import code
 import json
 import logging
-import sys
 
 import requests
 from requests import Request
 import pysolr
 import os
 from uuid import UUID
 from .models import *
 
 __all__ = ['DSpaceClient']
 
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
 
+
 def parse_json(response):
     """
     Simple static method to handle ValueError if JSON is invalid in response body
-    TODO: More logging, not just console output
-    @param response:
-    @return:
+    @param response: the http response object (which should contain JSON)
+    @return: parsed JSON object
     """
     response_json = None
     try:
         response_json = response.json()
     except ValueError as err:
-        print(f'Error parsing response JSON: {err}. Body text: {response.text}')
+        logging.error(f'Error parsing response JSON: {err}. Body text: {response.text}')
     return response_json
 
 
 class DSpaceClient:
     """
     Main class of the API client itself. This client uses request sessions to connect and authenticate to
     the REST API, maintain XSRF tokens, and all GET, POST, PUT, PATCH operations.
@@ -54,117 +52,154 @@
     Higher level get, create, update, partial_update (patch) functions are implemented for each DSO type
     """
     # Set up basic environment, variables
     session = None
     API_ENDPOINT = 'http://localhost:8080/server/api'
     SOLR_ENDPOINT = 'http://localhost:8983/solr'
     SOLR_AUTH = None
+    USER_AGENT = 'DSpace Python REST Client'
     if 'DSPACE_API_ENDPOINT' in os.environ:
         API_ENDPOINT = os.environ['DSPACE_API_ENDPOINT']
     LOGIN_URL = f'{API_ENDPOINT}/authn/login'
     USERNAME = 'username@test.system.edu'
     if 'DSPACE_API_USERNAME' in os.environ:
         USERNAME = os.environ['DSPACE_API_USERNAME']
     PASSWORD = 'password'
     if 'DSPACE_API_PASSWORD' in os.environ:
         PASSWORD = os.environ['DSPACE_API_PASSWORD']
     if 'SOLR_ENDPOINT' in os.environ:
         SOLR_ENDPOINT = os.environ['SOLR_ENDPOINT']
     if 'SOLR_AUTH' in os.environ:
         SOLR_AUTH = os.environ['SOLR_AUTH']
+    if 'USER_AGENT' in os.environ:
+        USER_AGENT = os.environ['USER_AGENT']
     verbose = False
 
     # Simple enum for patch operation types
     class PatchOperation:
         ADD = 'add'
         REMOVE = 'remove'
         REPLACE = 'replace'
         MOVE = 'move'
 
     def __init__(self, api_endpoint=API_ENDPOINT, username=USERNAME, password=PASSWORD, solr_endpoint=SOLR_ENDPOINT,
-                 solr_auth=SOLR_AUTH):
+                 solr_auth=SOLR_AUTH, fake_user_agent=False):
         """
         Accept optional API endpoint, username, password arguments using the OS environment variables as defaults
         :param api_endpoint:    base path to DSpace REST API, eg. http://localhost:8080/server/api
         :param username:        username with appropriate privileges to perform operations on REST API
         :param password:        password for the above username
         """
         self.session = requests.Session()
         self.API_ENDPOINT = api_endpoint
         self.LOGIN_URL = f'{self.API_ENDPOINT}/authn/login'
         self.USERNAME = username
         self.PASSWORD = password
         self.SOLR_ENDPOINT = solr_endpoint
         self.solr = pysolr.Solr(url=solr_endpoint, always_commit=True, timeout=300, auth=solr_auth)
+        # If fake_user_agent was specified, use this string that is known (as of 2023-12-03) to succeed with
+        # requests to Cloudfront-protected API endpoints (tested on demo.dspace.org)
+        # Otherwise, the user agent will be the more helpful and accurate default of 'DSpace Python REST Client'
+        # To override the user agent to your own string, instead set the USER_AGENT environment variable first
+        # eg `export USER_AGENT="My Custom Agent String / 1.0`, and don't specify a value for fake_user_agent
+        if fake_user_agent:
+            self.USER_AGENT = 'Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
+                              'Chrome/39.0.2171.95 Safari/537.36'
+        # Set headers based on this
+        self.auth_request_headers = {'User-Agent': self.USER_AGENT}
+        self.request_headers = {'Content-type': 'application/json', 'User-Agent': self.USER_AGENT}
+        self.list_request_headers = {'Content-type': 'text-uri-list', 'User-Agent': self.USER_AGENT}
 
-    def authenticate(self):
+    def authenticate(self, retry=False):
         """
         Authenticate with the DSpace REST API. As with other operations, perform XSRF refreshes when necessary.
         After POST, check /authn/status and log success if the authenticated json property is true
         @return: response object
         """
+        # Set headers for requests made during authentication
         # Get and update CSRF token
-        r = self.session.post(self.LOGIN_URL)
+        r = self.session.post(self.LOGIN_URL, data={'user': self.USERNAME, 'password': self.PASSWORD},
+                              headers=self.auth_request_headers)
         self.update_token(r)
 
-        # POST Login
-        r = self.session.post(self.LOGIN_URL, data={'user': self.USERNAME, 'password': self.PASSWORD})
+        if r.status_code == 403:
+            # 403 Forbidden
+            # If we had a CSRF failure, retry the request with the updated token
+            # After speaking in #dev it seems that these do need occasional refreshes but I suspect
+            # it's happening too often for me, so check for accidentally triggering it
+            if retry:
+                logging.error(f'Too many retries updating token: {r.status_code}: {r.text}')
+                return False
+            else:
+                logging.debug("Retrying request with updated CSRF token")
+                return self.authenticate(retry=True)
+
+        if r.status_code == 401:
+            # 401 Unauthorized
+            # If we get a 401, this means a general authentication failure
+            logging.error(f'Authentication failure: invalid credentials for user {self.USERNAME}')
+            return False
+
+        # Update headers with new bearer token if present
         if 'Authorization' in r.headers:
             self.session.headers.update({'Authorization': r.headers.get('Authorization')})
 
         # Get and check authentication status
-        r = self.session.get(f'{self.API_ENDPOINT}/authn/status')
-        r_json = r.json()
-        if 'authenticated' in r_json and r_json['authenticated'] is True:
-            logging.info(f'Authenticated successfully as {self.USERNAME}')
-        else:
-            return False
+        r = self.session.get(f'{self.API_ENDPOINT}/authn/status', headers=self.request_headers)
+        if r.status_code == 200:
+            r_json = parse_json(r)
+            if 'authenticated' in r_json and r_json['authenticated'] is True:
+                logging.info(f'Authenticated successfully as {self.USERNAME}')
+                return r_json['authenticated']
 
-        return r_json['authenticated']
+        # Default, return false
+        return False
 
     def refresh_token(self):
         """
         If the DSPACE-XSRF-TOKEN appears, we need to update our local stored token and re-send our API request
         @return: None
         """
         r = self.api_post(self.LOGIN_URL, None, None)
         self.update_token(r)
 
-    def api_get(self, url, params=None, data=None):
+    def api_get(self, url, params=None, data=None, headers=None):
         """
         Perform a GET request. Refresh XSRF token if necessary.
         @param url:     DSpace REST API URL
         @param params:  any parameters to include (eg ?page=0)
         @param data:    any data to supply (typically not relevant for GET)
+        @param headers: any override headers (eg. with short-lived token for download)
         @return:        Response from API
         """
-        r = self.session.get(url, params=params, data=data)
+        if headers is None:
+            headers = self.request_headers
+        r = self.session.get(url, params=params, data=data, headers=headers)
         self.update_token(r)
         return r
 
     def api_post(self, url, params, json, retry=False):
         """
         Perform a POST request. Refresh XSRF token if necessary.
         POSTs are typically used to create objects.
         @param url:     DSpace REST API URL
         @param params:  Any parameters to include (eg ?parent=abbc-....)
         @param json:    Data in json-ready form (dict) to send as POST body (eg. item.as_dict())
         @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
         @return:        Response from API
         """
-        h = {'Content-type': 'application/json'}
-        r = self.session.post(url, json=json, params=params, headers=h)
+        r = self.session.post(url, json=json, params=params, headers=self.request_headers)
         self.update_token(r)
 
         if r.status_code == 403:
             # 403 Forbidden
             # If we had a CSRF failure, retry the request with the updated token
             # After speaking in #dev it seems that these do need occasional refreshes but I suspect
             # it's happening too often for me, so check for accidentally triggering it
-            r_json = r.json()
+            r_json = parse_json(r)
             if 'message' in r_json and 'CSRF token' in r_json['message']:
                 if retry:
                     logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
                 else:
                     logging.debug("Retrying request with updated CSRF token")
                     return self.api_post(url, params=params, json=json, retry=True)
 
@@ -176,16 +211,15 @@
         POSTs are typically used to create objects.
         @param url:     DSpace REST API URL
         @param params:  Any parameters to include (eg ?parent=abbc-....)
         @param uri_list: One or more URIs referencing objects
         @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
         @return:        Response from API
         """
-        h = {'Content-type': 'text/uri-list'}
-        r = self.session.post(url, data=uri_list, params=params, headers=h)
+        r = self.session.post(url, data=uri_list, params=params, headers=self.list_request_headers)
         self.update_token(r)
 
         if r.status_code == 403:
             # 403 Forbidden
             # If we had a CSRF failure, retry the request with the updated token
             # After speaking in #dev it seems that these do need occasional refreshes but I suspect
             # it's happening too often for me, so check for accidentally triggering it
@@ -205,25 +239,25 @@
         PUTs are typically used to update objects.
         @param url:     DSpace REST API URL
         @param params:  Any parameters to include (eg ?parent=abbc-....)
         @param json:    Data in json-ready form (dict) to send as PUT body (eg. item.as_dict())
         @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
         @return:        Response from API
         """
-        h = {'Content-type': 'application/json'}
-        r = self.session.put(url, params=params, json=json, headers=h)
+        r = self.session.put(url, params=params, json=json, headers=self.request_headers)
         self.update_token(r)
 
         if r.status_code == 403:
             # 403 Forbidden
             # If we had a CSRF failure, retry the request with the updated token
             # After speaking in #dev it seems that these do need occasional refreshes but I suspect
             # it's happening too often for me, so check for accidentally triggering it
-            print(r.text)
-            r_json = r.json()
+            logging.debug(r.text)
+            # Parse response
+            r_json = parse_json(r)
             if 'message' in r_json and 'CSRF token' in r_json['message']:
                 if retry:
                     logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
                 else:
                     logging.debug("Retrying request with updated CSRF token")
                     return self.api_put(url, params=params, json=json, retry=True)
 
@@ -234,25 +268,25 @@
         Perform a DELETE request. Refresh XSRF token if necessary.
         DELETES are typically used to update objects.
         @param url:     DSpace REST API URL
         @param params:  Any parameters to include (eg ?parent=abbc-....)
         @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
         @return:        Response from API
         """
-        h = {'Content-type': 'application/json'}
-        r = self.session.delete(url, params=params, headers=h)
+        r = self.session.delete(url, params=params, headers=self.request_headers)
         self.update_token(r)
 
         if r.status_code == 403:
             # 403 Forbidden
             # If we had a CSRF failure, retry the request with the updated token
             # After speaking in #dev it seems that these do need occasional refreshes but I suspect
             # it's happening too often for me, so check for accidentally triggering it
-            print(r.text)
-            r_json = r.json()
+            logging.debug(r.text)
+            # Parse response
+            r_json = parse_json(r)
             if 'message' in r_json and 'CSRF token' in r_json['message']:
                 if retry:
                     logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
                 else:
                     logging.debug("Retrying request with updated CSRF token")
                     return self.api_delete(url, params=params, retry=True)
 
@@ -265,84 +299,86 @@
         @param path: path to perform operation - eg, metadata, withdrawn, etc.
         @param value: new value for add or replace operations, or 'original' path for move operations
         @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
         @return:
         @see https://github.com/DSpace/RestContract/blob/main/metadata-patch.md
         """
         if url is None:
-            print(f'Missing required URL argument')
+            logging.error(f'Missing required URL argument')
             return None
         if path is None:
-            print(f'Need valid path eg. /withdrawn or /metadata/dc.title/0/language')
+            logging.error(f'Need valid path eg. /withdrawn or /metadata/dc.title/0/language')
             return None
         if (operation == self.PatchOperation.ADD or operation == self.PatchOperation.REPLACE
                 or operation == self.PatchOperation.MOVE) and value is None:
             # missing value required for add/replace/move operations
-            print(f'Missing required "value" argument for add/replace/move operations')
+            logging.error(f'Missing required "value" argument for add/replace/move operations')
             return None
 
         # compile patch data
         data = {
             "op": operation,
             "path": path
         }
         if value is not None:
             if operation == self.PatchOperation.MOVE:
                 data["from"] = value
             else:
                 data["value"] = value
 
         # set headers
-        h = {'Content-type': 'application/json'}
         # perform patch request
-        r = self.session.patch(url, json=[data], headers=h)
+        r = self.session.patch(url, json=[data], headers=self.request_headers)
         self.update_token(r)
 
         if r.status_code == 403:
             # 403 Forbidden
             # If we had a CSRF failure, retry the request with the updated token
             # After speaking in #dev it seems that these do need occasional refreshes but I suspect
             # it's happening too often for me, so check for accidentally triggering it
-            print(r.text)
+            logging.debug(r.text)
             r_json = parse_json(r)
             if 'message' in r_json and 'CSRF token' in r_json['message']:
                 if retry:
                     logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
                 else:
                     logging.debug("Retrying request with updated CSRF token")
                     return self.api_patch(url, operation, path, value, True)
         elif r.status_code == 200:
             # 200 Success
-            print(f'successful patch update to {r.json()["type"]} {r.json()["id"]}')
+            logging.info(f'successful patch update to {r.json()["type"]} {r.json()["id"]}')
 
         # Return the raw API response
         return r
 
     # PAGINATION
-    def search_objects(self, query=None, filters=None, page=0, size=20, sort=None, dsoType=None):
+    def search_objects(self, query=None, scope=None, filters=None, page=0, size=20, sort=None, dso_type=None):
         """
         Do a basic search with optional query, filters and dsoType params.
         @param query:   query string
+        @param scope:   uuid to limit search scope, eg. owning collection, parent community, etc.
         @param filters: discovery filters as dict eg. {'f.entityType': 'Publication,equals', ... }
         @param page: page number (not like 'start' as this is not row number, but page number of size {size})
         @param size: size of page (aka. 'rows'), affects the page parameter above
         @param sort: sort eg. 'title,asc'
-        @param dsoType: DSO type to further filter results
+        @param dso_type: DSO type to further filter results
         @return:        list of DspaceObject objects constructed from API resources
         """
         dsos = []
         if filters is None:
             filters = {}
         url = f'{self.API_ENDPOINT}/discover/search/objects'
         # we will add params to filters, so
         params = {}
         if query is not None:
             params['query'] = query
-        if dsoType is not None:
-            params['dsoType'] = dsoType
+        if scope is not None:
+            params['scope'] = scope
+        if dso_type is not None:
+            params['dsoType'] = dso_type
         if size is not None:
             params['size'] = size
         if page is not None:
             params['page'] = page
         if sort is not None:
             params['sort'] = sort
 
@@ -352,29 +388,29 @@
         try:
             results = r_json['_embedded']['searchResult']['_embedded']['objects']
             for result in results:
                 resource = result['_embedded']['indexableObject']
                 dso = DSpaceObject(resource)
                 dsos.append(dso)
         except (TypeError, ValueError) as err:
-            print(f'error parsing search result json {err}')
+            logging.error(f'error parsing search result json {err}')
 
         return dsos
 
     def fetch_resource(self, url, params=None):
         """
         Simple function for higher-level 'get' functions to use whenever they want
         to retrieve JSON resources from the API
         @param url:     DSpace REST API URL
         @param params:  Optional params
         @return:        JSON parsed from API response or None if error
         """
         r = self.api_get(url, params, None)
         if r.status_code != 200:
-            print(f'Error encountered fetching resource: {r.text}')
+            logging.error(f'Error encountered fetching resource: {r.text}')
             return None
         # ValueError / JSON handling moved to static method
         return parse_json(r)
 
     def get_dso(self, url, uuid):
         """
         Base 'get DSpace Object' function.
@@ -385,15 +421,15 @@
         """
         try:
             # Try to get UUID version to test validity
             id = UUID(uuid).version
             url = f'{url}/{uuid}'
             return self.api_get(url, None, None)
         except ValueError:
-            print(f'Invalid DSO UUID: {uuid}')
+            logging.error(f'Invalid DSO UUID: {uuid}')
             return None
 
     def create_dso(self, url, params, data):
         """
         Base 'create DSpace Object' function.
         Takes JSON data and some POST parameters and returns the response.
         @param url:     DSpace REST API URL
@@ -401,18 +437,18 @@
         @param data:    JSON data expected by the REST API to create the new resource
         @return:        Raw API response. New DSO *could* be returned but for error checking purposes, raw response
                         is nice too and can always be parsed from this response later.
         """
         r = self.api_post(url, params, data)
         if r.status_code == 201:
             # 201 Created - success!
-            new_dso = r.json()
-            print(f'{new_dso["type"]} {new_dso["uuid"]} created successfully!')
+            new_dso = parse_json(r)
+            logging.info(f'{new_dso["type"]} {new_dso["uuid"]} created successfully!')
         else:
-            print(f'create operation failed: {r.status_code}: {r.text} ({url})')
+            logging.error(f'create operation failed: {r.status_code}: {r.text} ({url})')
         return r
 
     def update_dso(self, dso, params=None):
         """
         Update DSpaceObject. Takes a DSpaceObject and any optional parameters. Will send a PUT update to the remote
         object and return the updated object, typed correctly.
         :param dso:     DSpaceObject with locally updated data, to send in PUT request
@@ -420,15 +456,15 @@
         :return:
 
         """
         if dso is None:
             return None
         dso_type = type(dso)
         if not isinstance(dso, SimpleDSpaceObject):
-            print(f'Only SimpleDSpaceObject types (eg Item, Collection, Community) '
+            logging.error(f'Only SimpleDSpaceObject types (eg Item, Collection, Community) '
                   f'are supported by generic update_dso PUT.')
             return dso
         try:
             # Get self URI from HAL links
             url = dso.links['self']['href']
             # Get and clean data - there are some unalterable fields that could cause errors
             data = dso.as_dict()
@@ -445,18 +481,18 @@
             if 'type' in data:
                 data.pop('type')
             """
             r = self.api_put(url, params=params, json=data)
             if r.status_code == 200:
                 # 200 OK - success!
                 updated_dso = dso_type(parse_json(r))
-                print(f'{updated_dso.type} {updated_dso.uuid} updated sucessfully!')
+                logging.info(f'{updated_dso.type} {updated_dso.uuid} updated sucessfully!')
                 return updated_dso
             else:
-                print(f'update operation failed: {r.status_code}: {r.text} ({url})')
+                logging.error(f'update operation failed: {r.status_code}: {r.text} ({url})')
                 return None
 
         except ValueError as e:
             logging.error("Error parsing DSO response", exc_info=True)
             return None
 
     def delete_dso(self, dso=None, url=None, params=None):
@@ -467,36 +503,35 @@
         :param params:  Optional parameters
         :param url:     URI if not deleting from DSO
         :return:
 
         """
         if dso is None:
             if url is None:
-                print(f'Need a DSO or a URL to delete')
+                logging.error(f'Need a DSO or a URL to delete')
                 return None
         else:
             if not isinstance(dso, SimpleDSpaceObject):
-                print(f'Only SimpleDSpaceObject types (eg Item, Collection, Community, EPerson) '
+                logging.error(f'Only SimpleDSpaceObject types (eg Item, Collection, Community, EPerson) '
                       f'are supported by generic update_dso PUT.')
                 return dso
             # Get self URI from HAL links
             url = dso.links['self']['href']
 
         try:
             r = self.api_delete(url, params=params)
             if r.status_code == 204:
                 # 204 No Content - success!
-                print(f'{url} was deleted sucessfully!')
+                logging.info(f'{url} was deleted sucessfully!')
                 return r
             else:
-                print(f'update operation failed: {r.status_code}: {r.text} ({url})')
+                logging.error(f'update operation failed: {r.status_code}: {r.text} ({url})')
                 return None
-
         except ValueError as e:
-            print(f'{e}')
+            logging.error(f'Error deleting DSO {dso.uuid}: {e}')
             return None
 
     # PAGINATION
     def get_bundles(self, parent=None, uuid=None, page=0, size=20, sort=None):
         """
         Get bundles for an item
         @param parent:  python Item object, from which the UUID will be referenced in the URL.
@@ -527,15 +562,15 @@
             if single_result:
                 bundles.append(Bundle(r_json))
             if not single_result:
                 resources = r_json['_embedded']['bundles']
                 for resource in resources:
                     bundles.append(Bundle(resource))
         except ValueError as err:
-            print(f'error parsing bundle results: {err}')
+            logging.error(f'error parsing bundle results: {err}')
 
         return bundles
 
     def create_bundle(self, parent=None, name='ORIGINAL'):
         """
         Create new bundle in the specified item
         @param parent:  Parent python Item, the UUID of which will be used in the URL path
@@ -564,15 +599,15 @@
         if uuid is None and bundle is None:
             return list()
         if uuid is None and isinstance(bundle, Bundle):
             if 'bitstreams' in bundle.links:
                 url = bundle.links['bitstreams']['href']
             else:
                 url = f'{self.API_ENDPOINT}/core/bundles/{bundle.uuid}/bitstreams'
-                print(f'Cannot find bundle bitstream links, will try to construct manually: {url}')
+                logging.warning(f'Cannot find bundle bitstream links, will try to construct manually: {url}')
         # Perform the actual request. By now, our URL and parameter should be properly set
         params = {}
         if size is not None:
             params['size'] = size
         if page is not None:
             params['page'] = page
         if sort is not None:
@@ -609,39 +644,51 @@
             metadata = {}
         url = f'{self.API_ENDPOINT}/core/bundles/{bundle.uuid}/bitstreams'
         file = (name, open(path, 'rb'), mime)
         files = {'file': file}
         properties = {'name': name, 'metadata': metadata, 'bundleName': bundle.name}
         payload = {'properties': json.dumps(properties) + ';application/json'}
         h = self.session.headers
-        h.update({'Content-Encoding': 'gzip'})
+        h.update({'Content-Encoding': 'gzip', 'User-Agent': self.USER_AGENT})
         req = Request('POST', url, data=payload, headers=h, files=files)
         prepared_req = self.session.prepare_request(req)
         r = self.session.send(prepared_req)
         if 'DSPACE-XSRF-TOKEN' in r.headers:
             t = r.headers['DSPACE-XSRF-TOKEN']
-            print('Updating token to ' + t)
+            logging.debug('Updating token to ' + t)
             self.session.headers.update({'X-XSRF-Token': t})
             self.session.cookies.update({'X-XSRF-Token': t})
         if r.status_code == 403:
-            r_json = r.json()
+            r_json = parse_json(r)
             if 'message' in r_json and 'CSRF token' in r_json['message']:
                 if retry:
-                    print('Already retried... something must be wrong')
+                    logging.error('Already retried... something must be wrong')
                 else:
-                    print("Retrying request with updated CSRF token")
+                    logging.debug("Retrying request with updated CSRF token")
                     return self.create_bitstream(bundle, name, path, mime, metadata, True)
 
         if r.status_code == 201 or r.status_code == 200:
             # Success
             return Bitstream(api_resource=parse_json(r))
         else:
-            print(f'Error creating bitstream: {r.status_code}: {r.text}')
+            logging.error(f'Error creating bitstream: {r.status_code}: {r.text}')
             return None
 
+    def download_bitstream(self, uuid=None):
+        """
+        Download bitstream and return full response object including headers, and content
+        @param uuid:
+        @return: full response object including headers, and content
+        """
+        url = f'{self.API_ENDPOINT}/core/bitstreams/{uuid}/content'
+        h = {'User-Agent': self.USER_AGENT, 'Authorization': self.get_short_lived_token()}
+        r = self.api_get(url, headers=h)
+        if r.status_code == 200:
+            return r
+
     # PAGINATION
     def get_communities(self, uuid=None, page=0, size=20, sort=None, top=False):
         """
         Get communities - either all, for single UUID, or all top-level (ie no sub-communities)
         @param uuid:    string UUID if getting single community
         @param page:    integer page (default: 0)
         @param size:    integer size (default: 20)
@@ -660,22 +707,22 @@
             try:
                 # This isn't used, but it'll throw a ValueError if not a valid UUID
                 id = UUID(uuid).version
                 # Set URL and parameters
                 url = f'{url}/{uuid}'
                 params = None
             except ValueError:
-                print(f'Invalid community UUID: {uuid}')
+                logging.error(f'Invalid community UUID: {uuid}')
                 return None
 
         if top:
             # Set new URL
             url = f'{url}/search/top'
 
-        print(f'Performing get on {url}')
+        logging.debug(f'Performing get on {url}')
         # Perform actual get
         r_json = self.fetch_resource(url, params)
         # Empty list
         communities = list()
         if '_embedded' in r_json:
             if 'communities' in r_json['_embedded']:
                 for community_resource in r_json['_embedded']['communities']:
@@ -723,15 +770,15 @@
         if uuid is not None:
             try:
                 id = UUID(uuid).version
                 # Update URL and parameters
                 url = f'{url}/{uuid}'
                 params = None
             except ValueError:
-                print(f'Invalid collection UUID: {uuid}')
+                logging.error(f'Invalid collection UUID: {uuid}')
                 return None
 
         if community is not None:
             if 'collections' in community.links and 'href' in community.links['collections']:
                 # Update URL
                 url = community.links['collections']['href']
 
@@ -775,43 +822,68 @@
         # TODO - return constructed Item object instead, handling errors here?
         url = f'{self.API_ENDPOINT}/core/items'
         try:
             id = UUID(uuid).version
             url = f'{url}/{uuid}'
             return self.api_get(url, None, None)
         except ValueError:
-            print(f'Invalid item UUID: {uuid}')
+            logging.error(f'Invalid item UUID: {uuid}')
             return None
 
+    def get_items(self):
+        """
+        Get all archived items for a logged-in administrator. Admin only! Usually you will want to
+        use search or browse methods instead of this method
+        @return: A list of items, or an error
+        """
+        url = f'{self.API_ENDPOINT}/core/items'
+        # Empty item list
+        items = list()
+        # Perform the actual request
+        r_json = self.fetch_resource(url)
+        # Empty list
+        items = list()
+        if '_embedded' in r_json:
+            # This is a list of items
+            if 'collections' in r_json['_embedded']:
+                for item_resource in r_json['_embedded']['items']:
+                    items.append(Item(item_resource))
+        elif 'uuid' in r_json:
+            # This is a single item
+            items.append(Item(r_json))
+
+        # Return list (populated or empty)
+        return items
+
     def create_item(self, parent, item):
         """
         Create an item beneath the given parent collection
         @param parent:  UUID of parent collection to pass as a parameter to create_dso
         @param item:    python Item object containing all the data and links expected by the REST API
         @return:        Item object constructed from the API response
         """
         url = f'{self.API_ENDPOINT}/core/items'
         if parent is None:
-            print('Need a parent UUID!')
+            logging.error('Need a parent UUID!')
             return None
         params = {'owningCollection': parent}
         if not isinstance(item, Item):
-            print('Need a valid item')
+            logging.error('Need a valid item')
             return None
         return Item(api_resource=parse_json(self.create_dso(url, params=params, data=item.as_dict())))
 
     def update_item(self, item):
         """
         Update item. The Item passed to this method contains all the data, identifiers, links necessary to
         perform the update to the API. Note this is a full update, not a patch / partial update operation.
         @param item: python Item object
         @return:
         """
         if not isinstance(item, Item):
-            print('Need a valid item')
+            logging.error('Need a valid item')
             return None
         return self.update_dso(item, params=None)
 
     def add_metadata(self, dso, field, value, language=None, authority=None, confidence=-1, place=''):
         """
         Add metadata to a DSO using the api_patch method (PUT, with path and operation and value)
         :param dso:
@@ -821,15 +893,15 @@
         :param authority:
         :param confidence:
         :param place:
         :return:
         """
         if dso is None or field is None or value is None or not isinstance(dso, DSpaceObject):
             # TODO: separate these tests, and add better error handling
-            print('Invalid or missing DSpace object, field or value string')
+            logging.error('Invalid or missing DSpace object, field or value string')
             return self
 
         dso_type = type(dso)
 
         # Place can be 0+ integer, or a hyphen - meaning "last"
         path = f'/metadata/{field}/{place}'
         patch_value = {
@@ -862,15 +934,15 @@
         params = None
         if token is not None:
             params = {'token': token}
         return User(api_resource=parse_json(self.create_dso(url, params=params, data=data)))
 
     def delete_user(self, user):
         if not isinstance(user, User):
-            print(f'Must be a valid user')
+            logging.error(f'Must be a valid user')
             return None
         return self.delete_dso(user)
 
     # PAGINATION
     def get_users(self, page=0, size=20, sort=None):
         url = f'{self.API_ENDPOINT}/eperson/epersons'
         users = list()
@@ -902,15 +974,16 @@
             # TODO: Validation. Note, at least here I will just allow a dict instead of the pointless cast<->cast
             # that you see for other DSO types - still figuring out the best way
         return Group(api_resource=parse_json(self.create_dso(url, params=None, data=data)))
 
     def start_workflow(self, workspace_item):
         url = f'{self.API_ENDPOINT}/workflow/workflowitems'
         res = parse_json(self.api_post_uri(url, params=None, uri_list=workspace_item))
-        print(res)
+        logging.debug(res)
+        # TODO: WIP
 
     def update_token(self, r):
         """
         Refresh / update the XSRF (aka. CSRF) token if DSPACE-XSRF-TOKEN found in response headers
         This is used by all the base methods like api_put,
         See: https://github.com/DSpace/RestContract/blob/main/csrf-tokens.md
         :param r:
@@ -918,19 +991,37 @@
         """
         if not self.session:
             logging.debug('Session state not found, setting...')
             self.session = requests.Session()
         if 'DSPACE-XSRF-TOKEN' in r.headers:
             t = r.headers['DSPACE-XSRF-TOKEN']
             logging.debug(f'Updating XSRF token to {t}')
+            # Update headers and cookies
             self.session.headers.update({'X-XSRF-Token': t})
             self.session.cookies.update({'X-XSRF-Token': t})
 
-    #WRAPPER
+    def get_short_lived_token(self):
+        """
+        Get a short-lived (2 min) token in order to request restricted bitstream downloads
+        @return: short lived Authorization token
+        """
+        if not self.session:
+            logging.debug('Session state not found, setting...')
+            self.session = requests.Session()
+
+        url = f'{self.API_ENDPOINT}/authn/shortlivedtokens'
+        r = self.api_post(url, json=None, params=None)
+        r_json = parse_json(r)
+        if r_json is not None and 'token' in r_json:
+            return r_json['token']
+
+        logging.error('Could not retrieve short-lived token')
+        return None
+
     def solr_query(self, query, filters=None, fields=None, start=0, rows=999999999):
         if fields is None:
             fields = []
         if filters is None:
             filters = []
         return self.solr.search(query, fq=filters, start=start, rows=rows, **{
             'fl': ','.join(fields)
-        })
+        })
```

## Comparing `dspace_rest_client-0.1.8.dist-info/LICENSE.txt` & `dspace_rest_client-0.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dspace_rest_client-0.1.8.dist-info/METADATA` & `dspace_rest_client-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace-rest-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DSpace 7 REST API client library
 Home-page: https://github.com/the-library-code/dspace-rest-client
 Author: Kim Shepherd
 Author-email: kim@the-library-code.de
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/the-library-code/dspace-rest-python/blob/main/README.md
 Project-URL: GitHub, https://github.com/the-library-code/dspace-rest-python
```

## Comparing `dspace_rest_client-0.1.8.dist-info/RECORD` & `dspace_rest_client-0.1.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 dspace_rest_client/__init__.py,sha256=Il5Q9ATdX8yXqVxtP_nYqUhExzxPC_qk_WXQ_4h0exg,16
-dspace_rest_client/client.py,sha256=2G8Q-3Hb--KsBNQ_uUOXklmbiVCk8wa7T-ppQsLxXg4,41409
+dspace_rest_client/client.py,sha256=r8gnu6gGFCEVIOxB2i5vVy_Ym1PkBvFu5ScnVxyrw0E,46480
 dspace_rest_client/models.py,sha256=nWdPbXvaabbsUtpsQaWzOtfwOj_8yWap62SwqpFfDxY,18483
-dspace_rest_client-0.1.8.dist-info/LICENSE.txt,sha256=D_YfO8FXUsXKnidXIpVw-G8F190GLqtsWYqmrb5w8pw,1475
-dspace_rest_client-0.1.8.dist-info/METADATA,sha256=ERmspldWrOKlfHhI40MeoD9fCRtbDFTSJCdEyNgJ6k0,4441
-dspace_rest_client-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dspace_rest_client-0.1.8.dist-info/top_level.txt,sha256=NyNlqh1QKmVdtI188gUy3xXEMdHvPT3dhiCCiLhZIJ8,19
-dspace_rest_client-0.1.8.dist-info/RECORD,,
+dspace_rest_client-0.1.9.dist-info/LICENSE.txt,sha256=D_YfO8FXUsXKnidXIpVw-G8F190GLqtsWYqmrb5w8pw,1475
+dspace_rest_client-0.1.9.dist-info/METADATA,sha256=h2zJIRvGy9lNYM4-FDMav_Pbvaz3z487yMabiPzbDR8,4441
+dspace_rest_client-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dspace_rest_client-0.1.9.dist-info/top_level.txt,sha256=NyNlqh1QKmVdtI188gUy3xXEMdHvPT3dhiCCiLhZIJ8,19
+dspace_rest_client-0.1.9.dist-info/RECORD,,
```


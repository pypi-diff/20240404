# Comparing `tmp/ansys_grantami_recordlists-1.0.0.post1.tar.gz` & `tmp/ansys_grantami_recordlists-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_grantami_recordlists-1.0.0.post1.tar", max compression
+gzip compressed data, was "ansys_grantami_recordlists-1.1.0.tar", max compression
```

## Comparing `ansys_grantami_recordlists-1.0.0.post1.tar` & `ansys_grantami_recordlists-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-20 07:30:12.117982 ansys_grantami_recordlists-1.0.0.post1/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-20 07:30:12.117982 ansys_grantami_recordlists-1.0.0.post1/README.rst
--rw-r--r--   0        0        0     2319 2023-06-20 07:30:12.117982 ansys_grantami_recordlists-1.0.0.post1/pyproject.toml
--rw-r--r--   0        0        0      591 2023-06-20 07:30:12.121982 ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/__init__.py
--rw-r--r--   0        0        0    25391 2023-06-20 07:30:12.121982 ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/_connection.py
--rw-r--r--   0        0        0      114 2023-06-20 07:30:12.121982 ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/_logger.py
--rw-r--r--   0        0        0    26419 2023-06-20 07:30:12.121982 ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/_models.py
--rw-r--r--   0        0        0        0 2023-06-20 07:30:12.121982 ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/py.typed
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.0.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3640 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/README.rst
+-rw-r--r--   0        0        0     2315 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/__init__.py
+-rw-r--r--   0        0        0    25688 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/_connection.py
+-rw-r--r--   0        0        0      114 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/_logger.py
+-rw-r--r--   0        0        0    26619 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/_models.py
+-rw-r--r--   0        0        0        0 2024-01-17 16:22:47.174138 ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/py.typed
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.1.0/PKG-INFO
```

### Comparing `ansys_grantami_recordlists-1.0.0.post1/LICENSE` & `ansys_grantami_recordlists-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0.post1/README.rst` & `ansys_grantami_recordlists-1.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,20 +24,22 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. _after-badges:
-
 
 PyGranta RecordLists
 ====================
 
+..
+   _after-badges
+
+
 A Python wrapper for the Granta MI Lists API.
 
 To avoid ambiguity with the Python object ``list``, lists available via the Granta MI Lists API are referred to as
 ``record lists``. Granta MI users might also know the feature as ``Favorites Lists``.
 
 Using the Granta MI Lists API requires the user to have necessary permissions on the Granta MI Server. Some
 operations on record lists require additional permissions, specific to record lists. For more information,
@@ -46,15 +48,15 @@
 
 Dependencies
 ------------
 .. readme_software_requirements
 
 To use the ``ansys.grantami.recordlists`` package you must have access to a Granta MI 2023 R2 deployment.
 
-The ``ansys.grantami.recordlists`` package currently supports Python from version 3.8 to version 3.11.
+The ``ansys.grantami.recordlists`` package currently supports Python from version 3.9 to version 3.12.
 
 .. readme_software_requirements_end
 
 
 
 Installation
 --------------
@@ -63,14 +65,20 @@
 To install the latest release from `PyPI <https://pypi.org/project/ansys-grantami-recordlists/>`_, use
 this code:
 
 .. code::
 
     pip install ansys-grantami-recordlists
 
+To install a release compatible with a specific version of Granta MI, use the
+`PyGranta <https://grantami.docs.pyansys.com/>`_ meta-package with a requirement specifier:
+
+.. code::
+
+    pip install pygranta==2023.2.0
 
 Alternatively, to install the latest from ``ansys-grantami-recordlists`` `GitHub <https://github.com/ansys/grantami-recordlists>`_,
 use this code:
 
 .. code::
 
     pip install git:https://github.com/ansys/grantami-recordlists.git
```

### Comparing `ansys_grantami_recordlists-1.0.0.post1/pyproject.toml` & `ansys_grantami_recordlists-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-grantami-recordlists"
-version = "1.0.0.post1"
+version = "1.1.0"
 description = "A python wrapper for the Granta MI RecordLists API"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/grantami-recordlists"
 documentation = "https://recordlists.grantami.docs.pyansys.com"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-ansys-openapi-common = "^1.2.0"
-ansys-grantami-serverapi-openapi = "1.0.0"
+python = ">=3.9,<4.0"
+ansys-openapi-common = "^1.2.2"
+ansys-grantami-serverapi-openapi = "2.0.0"
 requests = "^2.26"
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 Sphinx = "^7.0.1"
 numpydoc = "^1.4.0"
-ansys-sphinx-theme = "^0.9.5"
+ansys-sphinx-theme = "^0.13.0"
 sphinx-copybutton = "^0.5.0"
 jupytext = "^1.14.4"
 nbsphinx = "^0.9.0"
 ipykernel = "^6.21.2" # required by nbsphinx to run notebooks.
 sphinx-jinja = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/__init__.py` & `ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/_connection.py` & `ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
             Unique identifier of the record list.
 
         Returns
         -------
         :class:`.RecordList`
         """
         logger.info(f"Getting list with identifier {identifier} with connection {self}")
-        record_list = self.list_management_api.api_v1_lists_list_list_identifier_get(identifier)
+        record_list = self.list_management_api.api_v1_lists_list_list_identifier_get(
+            list_identifier=identifier
+        )
         return RecordList._from_model(record_list)
 
     def search_for_lists(
         self, criterion: Union[BooleanCriterion, SearchCriterion], include_items: bool = False
     ) -> List[SearchResult]:
         """
         Search for record lists matching the provided criteria.
@@ -141,15 +143,15 @@
                 search_criterion=criterion._to_model(),
                 response_options=response_options,
             )
         )
 
         search_results = (
             self.list_management_api.api_v1_lists_search_results_result_resource_identifier_get(
-                search_info.search_result_identifier
+                result_resource_identifier=search_info.search_result_identifier
             )
         )
         return [
             SearchResult._from_model(search_result, include_items)
             for search_result in search_results
         ]
 
@@ -167,15 +169,15 @@
         Returns
         -------
         list of :class:`.RecordListItem`
             List of items included in the record list.
         """
         logger.info(f"Getting items in list {record_list} with connection {self}")
         items = self.list_item_api.api_v1_lists_list_list_identifier_items_get(
-            record_list.identifier
+            list_identifier=record_list.identifier
         )
         return [RecordListItem._from_model(item) for item in items.items]
 
     def add_items_to_list(
         self, record_list: RecordList, items: List[RecordListItem]
     ) -> List[RecordListItem]:
         """
@@ -195,15 +197,15 @@
         Returns
         -------
         list of :class:`.RecordListItem`
            List of items included in the record list.
         """
         logger.info(f"Adding {len(items)} items to list {record_list} with connection {self}")
         response_items = self.list_item_api.api_v1_lists_list_list_identifier_items_add_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
             body=models.GrantaServerApiListsDtoRecordListItems(
                 items=[item._to_model() for item in items]
             ),
         )
         return [RecordListItem._from_model(item) for item in response_items.items]
 
     def remove_items_from_list(
@@ -225,15 +227,15 @@
         Returns
         -------
         list of :class:`.RecordListItem`
            List of items included in the record list.
         """
         logger.info(f"Removing {len(items)} items from list {record_list} with connection {self}")
         response_items = self.list_item_api.api_v1_lists_list_list_identifier_items_remove_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
             body=models.GrantaServerApiListsDtoRecordListItems(
                 items=[item._to_model() for item in items]
             ),
         )
         return [RecordListItem._from_model(item) for item in response_items.items]
 
     def create_list(
@@ -289,15 +291,17 @@
 
         Parameters
         ----------
         record_list : RecordList
             Record list to delete.
         """
         logger.info(f"Removing list {record_list} with connection {self}")
-        self.list_management_api.api_v1_lists_list_list_identifier_delete(record_list.identifier)
+        self.list_management_api.api_v1_lists_list_list_identifier_delete(
+            list_identifier=record_list.identifier
+        )
 
     def update_list(
         self,
         record_list: RecordList,
         *,
         name: str = _ArgNotProvided,
         description: Union[str, None] = _ArgNotProvided,
@@ -340,15 +344,15 @@
             body.append(self._create_patch_operation(name, "name"))
         if description != _ArgNotProvided:
             body.append(self._create_patch_operation(description, "description"))
         if notes != _ArgNotProvided:
             body.append(self._create_patch_operation(notes, "notes"))
 
         updated_resource = self.list_management_api.api_v1_lists_list_list_identifier_patch(
-            record_list.identifier, body=body
+            list_identifier=record_list.identifier, body=body
         )
         return RecordList._from_model(updated_resource)
 
     def copy_list(self, record_list: RecordList) -> RecordList:
         """
         Create a copy of a record list.
 
@@ -363,15 +367,15 @@
         Returns
         -------
         :class:`.RecordList`
             Record list created by the copy operation.
         """
         logger.info(f"Copying list {record_list} with connection {self}")
         list_copy = self.list_management_api.api_v1_lists_list_list_identifier_copy_post(
-            record_list.identifier
+            list_identifier=record_list.identifier
         )
         return RecordList._from_model(list_copy)
 
     def revise_list(self, record_list: RecordList) -> RecordList:
         """
         Revise a record list.
 
@@ -388,15 +392,15 @@
         Returns
         -------
         :class:`.RecordList`
             Record list created by the revision operation.
         """
         logger.info(f"Creating revision of list {record_list} with connection {self}")
         list_revision = self.list_management_api.api_v1_lists_list_list_identifier_revise_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
         )
         return RecordList._from_model(list_revision)
 
     def request_list_approval(self, record_list: RecordList) -> RecordList:
         """
         Request approval for a record list.
 
@@ -412,15 +416,15 @@
         -------
         :class:`.RecordList`
             Updated representation of the record list.
         """
         logger.info(f"Requesting approval for list {record_list} with connection {self}")
         updated_list = (
             self.list_management_api.api_v1_lists_list_list_identifier_request_approval_post(
-                record_list.identifier
+                list_identifier=record_list.identifier,
             )
         )
         return RecordList._from_model(updated_list)
 
     def publish_list(self, record_list: RecordList) -> RecordList:
         """
         Publish a record list.
@@ -439,15 +443,15 @@
         Returns
         -------
         :class:`.RecordList`
             Updated representation of the record list.
         """
         logger.info(f"Publishing list {record_list} with connection {self}")
         updated_list = self.list_management_api.api_v1_lists_list_list_identifier_publish_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
         )
         return RecordList._from_model(updated_list)
 
     def unpublish_list(self, record_list: RecordList) -> RecordList:
         """
         Withdraw a record list.
 
@@ -464,15 +468,15 @@
         Returns
         -------
         :class:`.RecordList`
             Updated representation of the record list.
         """
         logger.info(f"Withdrawing list {record_list} with connection {self}")
         updated_list = self.list_management_api.api_v1_lists_list_list_identifier_unpublish_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
         )
         return RecordList._from_model(updated_list)
 
     def cancel_list_approval_request(self, record_list: RecordList) -> RecordList:
         """
         Cancel a pending request for approval on a record list.
 
@@ -488,15 +492,15 @@
         Returns
         -------
         :class:`.RecordList`
             Updated representation of the record list.
         """
         logger.info(f"Cancelling request to approve list {record_list} with connection {self}")
         updated_list = self.list_management_api.api_v1_lists_list_list_identifier_reset_post(
-            record_list.identifier,
+            list_identifier=record_list.identifier,
         )
         return RecordList._from_model(updated_list)
 
     def subscribe_to_list(self, record_list: RecordList) -> None:
         """
         Subscribe the current user to a record list.
 
@@ -509,15 +513,15 @@
             Record list to subscribe to.
 
         Returns
         -------
         None
         """
         self.list_permissions_api.api_v1_lists_list_list_identifier_permissions_subscribe_post(
-            record_list.identifier
+            list_identifier=record_list.identifier
         )
 
     def unsubscribe_from_list(self, record_list: RecordList) -> None:
         """
         Unsubscribe the current user from a record list.
 
         Performs an HTTP request against the Granta MI Server API.
@@ -528,15 +532,15 @@
             Record list to unsubscribe from.
 
         Returns
         -------
         None
         """
         self.list_permissions_api.api_v1_lists_list_list_identifier_permissions_unsubscribe_post(
-            record_list.identifier
+            list_identifier=record_list.identifier,
         )
 
     @staticmethod
     def _create_patch_operation(
         value: Optional[str], name: str, op: str = "replace"
     ) -> models.JsonPatchDocument:
         return models.JsonPatchDocument(
```

### Comparing `ansys_grantami_recordlists-1.0.0.post1/src/ansys/grantami/recordlists/_models.py` & `ansys_grantami_recordlists-1.1.0/src/ansys/grantami/recordlists/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,17 +524,22 @@
     @user_can_add_or_remove_items.setter
     def user_can_add_or_remove_items(self, value: Optional[bool]) -> None:
         self._user_can_add_or_remove_items = value
 
     def _to_model(self) -> models.GrantaServerApiListsDtoRecordListSearchCriterion:
         """Generate the DTO for use with the auto-generated client code."""
         logger.debug("Serializing SearchCriterion to API model")
+        user_role = (
+            models.GrantaServerApiListsDtoUserRole(self.user_role.value)
+            if self.user_role is not None
+            else None
+        )
         model = models.GrantaServerApiListsDtoRecordListSearchCriterion(
             name_contains=self.name_contains,
-            user_role=self.user_role,
+            user_role=user_role,
             is_published=self.is_published,
             is_awaiting_approval=self.is_awaiting_approval,
             is_internal_use=self.is_internal_use,
             is_revision=self.is_revision,
             contains_records_in_databases=self.contains_records_in_databases,
             contains_records_in_integration_schemas=self.contains_records_in_integration_schemas,
             contains_records_in_tables=self.contains_records_in_tables,
@@ -646,22 +651,22 @@
 
 class UserRole(str, Enum):
     """Roles a user can have on a record list.
 
     Can be used in :attr:`SearchCriterion.user_role`.
     """
 
-    NONE = models.GrantaServerApiListsDtoUserRole.NONE
+    NONE = models.GrantaServerApiListsDtoUserRole.NONE.value
     """:class:`UserRole` is currently only supported in searches. Searching for lists with user
     role = :attr:`.NONE` as criteria would exclude all lists from the results."""
-    OWNER = models.GrantaServerApiListsDtoUserRole.OWNER
-    SUBSCRIBER = models.GrantaServerApiListsDtoUserRole.SUBSCRIBER
-    CURATOR = models.GrantaServerApiListsDtoUserRole.CURATOR
-    ADMINISTRATOR = models.GrantaServerApiListsDtoUserRole.ADMINISTRATOR
-    PUBLISHER = models.GrantaServerApiListsDtoUserRole.PUBLISHER
+    OWNER = models.GrantaServerApiListsDtoUserRole.OWNER.value
+    SUBSCRIBER = models.GrantaServerApiListsDtoUserRole.SUBSCRIBER.value
+    CURATOR = models.GrantaServerApiListsDtoUserRole.CURATOR.value
+    ADMINISTRATOR = models.GrantaServerApiListsDtoUserRole.ADMINISTRATOR.value
+    PUBLISHER = models.GrantaServerApiListsDtoUserRole.PUBLISHER.value
 
 
 class SearchResult:
     """Describes the result of a search.
 
     Read-only - do not directly instantiate or modify instances of this class.
     """
```

### Comparing `ansys_grantami_recordlists-1.0.0.post1/PKG-INFO` & `ansys_grantami_recordlists-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ansys-grantami-recordlists
-Version: 1.0.0.post1
+Version: 1.1.0
 Summary: A python wrapper for the Granta MI RecordLists API
 Home-page: https://github.com/ansys/grantami-recordlists
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ansys-grantami-serverapi-openapi (==1.0.0)
-Requires-Dist: ansys-openapi-common (>=1.2.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ansys-grantami-serverapi-openapi (==2.0.0)
+Requires-Dist: ansys-openapi-common (>=1.2.2,<2.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Project-URL: Documentation, https://recordlists.grantami.docs.pyansys.com
 Project-URL: Repository, https://github.com/ansys/grantami-recordlists
 Description-Content-Type: text/x-rst
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
@@ -50,20 +50,22 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. _after-badges:
-
 
 PyGranta RecordLists
 ====================
 
+..
+   _after-badges
+
+
 A Python wrapper for the Granta MI Lists API.
 
 To avoid ambiguity with the Python object ``list``, lists available via the Granta MI Lists API are referred to as
 ``record lists``. Granta MI users might also know the feature as ``Favorites Lists``.
 
 Using the Granta MI Lists API requires the user to have necessary permissions on the Granta MI Server. Some
 operations on record lists require additional permissions, specific to record lists. For more information,
@@ -72,15 +74,15 @@
 
 Dependencies
 ------------
 .. readme_software_requirements
 
 To use the ``ansys.grantami.recordlists`` package you must have access to a Granta MI 2023 R2 deployment.
 
-The ``ansys.grantami.recordlists`` package currently supports Python from version 3.8 to version 3.11.
+The ``ansys.grantami.recordlists`` package currently supports Python from version 3.9 to version 3.12.
 
 .. readme_software_requirements_end
 
 
 
 Installation
 --------------
@@ -89,14 +91,20 @@
 To install the latest release from `PyPI <https://pypi.org/project/ansys-grantami-recordlists/>`_, use
 this code:
 
 .. code::
 
     pip install ansys-grantami-recordlists
 
+To install a release compatible with a specific version of Granta MI, use the
+`PyGranta <https://grantami.docs.pyansys.com/>`_ meta-package with a requirement specifier:
+
+.. code::
+
+    pip install pygranta==2023.2.0
 
 Alternatively, to install the latest from ``ansys-grantami-recordlists`` `GitHub <https://github.com/ansys/grantami-recordlists>`_,
 use this code:
 
 .. code::
 
     pip install git:https://github.com/ansys/grantami-recordlists.git
```


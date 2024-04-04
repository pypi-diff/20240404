# Comparing `tmp/igz_mgmt-0.1.0.tar.gz` & `tmp/igz_mgmt-0.1.1.tar.gz`

## Comparing `igz_mgmt-0.1.0.tar` & `igz_mgmt-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/client.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/constants.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/operations.py
--rw-r--r--   0        0        0    81587 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/schemas/events.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/client.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    88337 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/schemas/events.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/README.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.1/PKG-INFO
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/__init__.py` & `igz_mgmt-0.1.1/igz_mgmt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 #
 from igz_mgmt.schemas.app_services import (
     AppServiceBase,
     AppServiceSpec,
     AppServiceStatus,
     CustomAppServiceSpec,
+    FilebeatSpec,
     JupyterSpec,
     ScaleResource,
     ScaleToZeroSpec,
 )
 from igz_mgmt.schemas.app_services import (
     ScaleToZeroSpecPresets as AppServiceScaleToZeroSpecPresets,
 )
@@ -30,16 +31,18 @@
     ApplyServicesMode,
     AppServiceDesiredStates,
     AppServicePriorityClass,
     ForceApplyAllMode,
     JupyterAppServicePrebakedImage,
     ProjectDeletionStrategies,
     ScaleToZeroMode,
+    SslVerificationMode,
     TenantManagementRoles,
     UserAdminStatuses,
+    UserAuthenticationMethods,
     UserOperationalStatuses,
 )
 from .cruds import ResourceListPagingQueryParams
 from .logger import get_or_create_logger
 from .operations import AppServices, ClusterConfigurations, ManualEvents
 from .resources import (
     AccessKey,
@@ -87,8 +90,11 @@
     "JupyterAppServicePrebakedImage",
     "AppServices",
     "get_or_create_logger",
     "ManualEvents",
     "ManualEventSchema",
     "ProjectDeletionStrategies",
     "Project",
+    "SslVerificationMode",
+    "UserAuthenticationMethods",
+    "FilebeatSpec",
 ]
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/__version__.py` & `igz_mgmt-0.1.1/igz_mgmt/logger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# version can be either one of the following:
-# x.y.z
-# x.y.z.rcN
+from .logger import Logger, get_or_create_logger
 
-__version__ = "0.1.0"
+__all__ = ["get_or_create_logger", "Logger"]
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/client.py` & `igz_mgmt-0.1.1/igz_mgmt/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """The API client used to communicate with the Iguazio backend."""
 import base64
 import copy
+import logging
 import os
 import typing
 from http import HTTPStatus
 
 import httpx
 import inflection
 import semver
@@ -161,46 +162,48 @@
         *,
         endpoint: str = "",
         timeout: int = 60,
         retries: int = 3,
         username: str = "",
         password: str = "",
         access_key: str = "",
+        logger: typing.Optional[logging.Logger] = None,
     ):
         if password and access_key:
             raise ValueError("Must provide either password or access key")
 
         if not username and not access_key:
             username = os.getenv("V3IO_USERNAME")
         if password and not username:
             raise ValueError("Must provide username when providing password")
 
         if not password and not access_key:
             access_key = os.getenv("V3IO_ACCESS_KEY")
 
-        self._logger = igz_mgmt.get_or_create_logger(level="INFO", name="apic")
+        self._logger = igz_mgmt.get_or_create_logger(
+            level="INFO", name="apic", logger=logger
+        )
 
         # enriched once authenticated
         self._tenant_id: typing.Optional[str] = None
 
         self._client = _BaseHTTPClient(
             self._logger,
             igz_mgmt.common.helpers.get_endpoint(endpoint, default_scheme="https"),
             timeout=timeout,
             retries=retries,
         )
 
         self._version = None
         self._authenticated = False
+        self._username = username
+        self._password = password
         if access_key:
             self._set_auth(username=username, access_key=access_key)
             self._authenticated = True
-        self._username = username
-        self._password = password
-        self._access_key = access_key
 
     def close(self):
         """Closes the client connection."""
         self._client.close()
 
     def login(self, *, username: str = "", password: str = ""):
         """Authenticates to the API server using username and password.
@@ -228,16 +231,16 @@
 
         Args:
             access_key (str): The new access key.
 
         Returns:
             APIClient: The client protocol.
         """
-        self._access_key = access_key
         self._set_auth(access_key=access_key)
+        self._authenticated = True
         return self
 
     def create(self, resource_name: str, attributes, relationships=None, **kwargs):
         """Creates a new resource.
 
         Args:
             resource_name (str): The resource name.
@@ -390,15 +393,15 @@
                 "utf-8"
             )
             self._client._headers[
                 igz_mgmt.constants._RequestHeaders.authorization_header
             ] = f"Basic {base64_encoded_auth}"
 
         self._version = self._get_external_versions()
-        self._enrich_tenant_id()
+        self._session_verification()
 
     def _try_resolve_external_version(self, node):
         try:
             # get external version via tunnel
             response = self._client.get(
                 "/tunnel/{0}.version.0/external_versions/{0}".format(node),
                 "Failed to get external version from node {0}".format(node),
@@ -423,36 +426,47 @@
         self._logger.info(
             "Failed to resolve auto detect iguazio external version, use `client.version = x.y.z` for explicitness"
         )
 
         # oldest supported GA version
         return self.__DEFAULT_EXTERNAL_VERSION_NUMBER
 
-    def _enrich_tenant_id(self):
+    def _session_verification(self):
         response = self.request("POST", "/sessions/verifications/planes/any/internal")
+        response_attributes = response.get("data", {}).get("attributes", {})
         self._tenant_id = (
-            response.get("data", {})
-            .get("attributes", {})
-            .get("context", {})
+            response_attributes.get("context", {})
             .get("authentication", {})
             .get("tenant_id")
         )
+        self._username = response_attributes.get("username", self._username)
 
     @property
     def tenant_id(self) -> str:
         """Authenticated session tenant id.
 
         Returns:
             tenant id
         """
         if not self._authenticated:
             raise RuntimeError("Must .login() first")
         return self._tenant_id
 
     @property
+    def username(self) -> str:
+        """Authenticated username.
+
+        Returns:
+            username
+        """
+        if not self._authenticated:
+            raise RuntimeError("Must .login() first")
+        return self._username
+
+    @property
     def version(self) -> semver.VersionInfo:
         """Iguazio system version info.
 
         Returns:
             semver.VersionInfo: Iguazio version
         """
         return self._version
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/constants.py` & `igz_mgmt-0.1.1/igz_mgmt/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,26 @@
 class SessionPlanes(_BaseEnumStr):
     """Session plane types."""
 
     data = "data"
     control = "control"
 
 
+class UserAuthenticationMethods(_BaseEnumStr):
+    """User authentication methods types."""
+
+    password = "password"
+    sso = "sso"
+
+
 class TenantManagementRoles(_BaseEnumStr):
     """Tenant management roles types."""
 
     it_admin = "IT Admin"
+    it_admin_read_only = "IT Admin Read Only"
     application_admin = "Application Admin"
     security_admin = "Security Admin"
     project_security_admin = "Project Security Admin"
     project_read_only = "Project Read Only"
     application_read_only = "Application Read Only"
     data = "Data"
     tenant_admin = "Tenant Admin"
@@ -181,14 +189,28 @@
     gpu_cuda = "jupyter-gpu-cuda"
     """Full stack with GPU."""
 
     full_stack = "jupyter-all"
     """Full stack without GPU"""
 
 
+class SslVerificationMode(_BaseEnumStr):
+    """Controls the verification of filebeat server certificates."""
+
+    none = "none"
+    """Performs no verification of the server’s certificate.
+    This mode disables many of the security benefits of SSL/TLS and should only be used after cautious consideration.
+    It is primarily intended as a temporary diagnostic mechanism when attempting to resolve TLS errors.
+    Its use in production environments is strongly discouraged."""
+
+    full = "full"
+    """Verifies that the provided certificate is signed by a trusted authority (CA)
+    and also verifies that the server’s hostname (or IP address) matches the names identified within the certificate."""
+
+
 class EventSeverity(_BaseEnumStr):
     """Severity types."""
 
     unknown = "unknown"
     debug = "debug"
     info = "info"
     warning = "warning"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/cruds.py` & `igz_mgmt-0.1.1/igz_mgmt/cruds.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/igz_mgmt/exceptions.py` & `igz_mgmt-0.1.1/igz_mgmt/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,7 +83,18 @@
     def __init__(self, member, role_name):
         if member.type == "user":
             prefix = f"User: {member.username}"
         else:
             prefix = f"Group: {member.name}"
         self.message = f"{prefix} already exists in project with role: {role_name}"
         super().__init__(self.message)
+
+
+class UserIsInPrimaryGroupError(Exception):
+    """The user is in primary group."""
+
+    def __init__(self, user, group):
+        self.message = (
+            f"Cannot remove user: {user.username} from {group.name} because it is the user's primary group."
+            f"Set force=True to override it."
+        )
+        super().__init__(self.message)
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/operations.py` & `igz_mgmt-0.1.1/igz_mgmt/operations.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/igz_mgmt/resources.py` & `igz_mgmt-0.1.1/igz_mgmt/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 
 Most of the resources support all CRUD methods.
 """
 import collections
 import contextlib
 import http
 import json
+import re
 import time
 import typing
 
 import inflection
 import pydantic.utils
 import semver
+from deprecated import deprecated
 
 import igz_mgmt.client
 import igz_mgmt.common.helpers
 import igz_mgmt.constants
 import igz_mgmt.cruds
 import igz_mgmt.exceptions
 import igz_mgmt.schemas
@@ -273,14 +275,17 @@
     first_name: str = ""
     last_name: str = ""
     email: str = ""
     uid: int = 0
     created_at: str = ""
     data_access_mode: str = ""
     authentication_scheme: str = ""
+    authentication_methods: typing.List[
+        igz_mgmt.constants.UserAuthenticationMethods
+    ] = []
     send_password_on_creation: bool = False
     assigned_policies: typing.List[igz_mgmt.constants.TenantManagementRoles] = []
     operational_status: str = igz_mgmt.constants.UserOperationalStatuses.up
     admin_status: str = igz_mgmt.constants.UserAdminStatuses.up
     password: pydantic.SecretStr = None
     phone_number: str = ""
     job_title: str = ""
@@ -301,14 +306,15 @@
         primary_group: typing.Union[str, "Group", None] = None,
         groups: typing.Union[typing.List[str], typing.List["Group"], None] = None,
         timeout: int = 30,
         wait_for_completion=True,
         phone_number: str = "",
         job_title: str = "",
         department: str = "",
+        authentication_methods: igz_mgmt.constants.UserAuthenticationMethods = None,
     ) -> "User":
         """Creates a new User.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
             password (str, optional): The user password. None by default. (if not provided, an email is automatically
@@ -319,14 +325,16 @@
             groups (typing.Union[typing.List[str], typing.List["Group"], None], optional): A list of group objects
             or group ids to add user to the groups. None by default.
             timeout (int, optional): The default is 30.
             wait_for_completion (bool): Whether to wait for the job to complete
             phone_number (str, optional): The user phone number.
             job_title (str, optional): The user job title.
             department (str, optional): The user department.
+            authentication_methods (typing.List[UserAuthenticationMethods], optional): The authentication method
+            type to log in with. None by default.
 
         Returns:
             User
         """
         assigned_policies = assigned_policies or [
             igz_mgmt.constants.TenantManagementRoles.developer.value,
             igz_mgmt.constants.TenantManagementRoles.application_read_only.value,
@@ -342,14 +350,23 @@
             "department": department,
         }
         if uid is not None:
             attributes["uid"] = uid
         if password is not None:
             attributes["password"] = password
 
+        if authentication_methods is not None:
+            # authentication_methods field exists only in version 3.5.5 and higher
+            if http_client.version >= semver.VersionInfo.parse("3.5.5"):
+                attributes["authentication_methods"] = authentication_methods
+            else:
+                http_client._logger.warn_with(
+                    "The 'authentication_methods' field is only permitted in versions 3.5.5 and above - ignoring"
+                )
+
         relationships = collections.defaultdict(dict)
         if primary_group:
             primary_group_id = (
                 primary_group.id if isinstance(primary_group, Group) else primary_group
             )
             relationships["primary_group"] = {
                 "data": {
@@ -504,65 +521,95 @@
             http_client (APIClient): The client to use.
             project_name (str): The project name.
 
         Returns:
             list: The effective roles of the user in the project.
         """
         project = Project.get_by_name(http_client, project_name)
-        return project.get_user_effective_role(self)
+        return project.get_user_effective_role(http_client, self)
 
     def add_to_group(
         self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
     ):
         """Adds a user to a group.
 
         1. get the user
         2. add the group to the user
         3. update the user
 
         Args:
             http_client (APIClient): The client to use.
-            group (str or Group): The group id or group instance to add user into it.
+            group (str or Group): The group id or group name or group instance to add user into it.
         """
         user = self.get(http_client, self.id, include=["user_groups"])
         if "user_groups" not in user.relationships:
             user.relationships["user_groups"] = {"data": []}
 
-        group_id = group.id if isinstance(group, Group) else group
-        if User._ensure_user_in_group(user, group_id):
+        group = Group._get_from_arg(http_client, group)
+        if User._ensure_user_in_group(user, group.id):
             user.update(http_client, relationships=user.relationships)
 
     def remove_from_group(
-        self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
+        self,
+        http_client: igz_mgmt.client.APIClient,
+        group: typing.Union[str, "Group"],
+        force=False,
     ):
         """Removes a user from a group.
 
         Args:
             http_client (APIClient): The client to use.
-            group (str or Group): The group id or group instance to remove user from it.
+            group (str or Group): The group id or group name or group instance to remove user from it.
+            force (bool): force (bool): Whether to force the removal of the user from the group (for example, from its
+                                        primary group).
         """
         user = self.get(http_client, self.id, include=["user_groups"])
-        group_id = group.id if isinstance(group, Group) else group
+        group_id = Group._get_from_arg(http_client, group).id
+        primary_group = self.get_primary_group(http_client)
+        if primary_group and primary_group.id == group_id:
+            if force:
+                user.set_primary_group(http_client, "")
+            else:
+                raise igz_mgmt.exceptions.UserIsInPrimaryGroupError(self, primary_group)
+
         if "user_groups" in user.relationships:
             user.relationships["user_groups"]["data"] = [
                 group
                 for group in user.relationships["user_groups"]["data"]
                 if group["id"] != group_id
             ]
             user.update(http_client, relationships=user.relationships)
 
+    def get_primary_group(
+        self, http_client: igz_mgmt.client.APIClient
+    ) -> typing.Optional["Group"]:
+        """Gets the primary group of a user.
+
+        Args:
+            http_client (APIClient): The client to use.
+
+        Returns:
+            Group: The primary group of the user.
+        """
+        user = self.get(http_client, self.id, include=["primary_group"])
+        if "primary_group" in user.relationships:
+            return Group.get(
+                http_client, user.relationships["primary_group"]["data"]["id"]
+            )
+
     def set_primary_group(
         self, http_client: igz_mgmt.client.APIClient, group: typing.Union[str, "Group"]
     ):
         """Sets the primary group of a user.
 
         Args:
             http_client (APIClient): The client to use.
-            group (str or Group): The primary group id or group instance.
+            group (str or Group): The primary group id or group name or group instance.
         """
+        group = Group._get_from_arg(http_client, group)
         group_id = group.id if isinstance(group, Group) else group
 
         # we need primary group
         user = self.get(http_client, self.id, include=["user_groups"])
         if "primary_group" not in user.relationships:
             user.relationships["primary_group"] = {"data": None}
         if "user_groups" not in user.relationships:
@@ -581,66 +628,112 @@
         Args:
             http_client (APIClient): The client to use.
         """
         self.admin_status = igz_mgmt.constants.UserAdminStatuses.down
         return self.update(http_client)
 
     @classmethod
+    @deprecated(reason="Use disable_user instead")
     def disable_by_username(cls, http_client: igz_mgmt.client.APIClient, username: str):
         """Disables the user by username.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
         """
-        user = cls.get_by_username(http_client, username)
-        return user.disable(http_client)
+        return cls.disable_user(http_client, username)
 
     @classmethod
+    @deprecated(reason="Use disable_user instead")
     def disable_by_id(cls, http_client: igz_mgmt.client.APIClient, user_id: str):
         """Disables the user by user id.
 
         Args:
             http_client (APIClient): The client to use.
             user_id (str): The user id.
         """
-        user = cls.get(http_client, user_id)
+        return cls.disable_user(http_client, user_id)
+
+    @classmethod
+    def disable_user(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        user: typing.Union[str, int, "User"],
+    ):
+        """Disables the user.
+
+        Args:
+            http_client (APIClient): The client to use.
+            user (str or int or User): The user id, username or user instance.
+        """
+        user = cls._get_from_arg(http_client, user)
         return user.disable(http_client)
 
     def enable(self, http_client: igz_mgmt.client.APIClient):
         """Enables the user instance.
 
         Args:
             http_client (APIClient): The client to use.
         """
         self.admin_status = igz_mgmt.constants.UserAdminStatuses.up
         return self.update(http_client)
 
     @classmethod
+    @deprecated(reason="Use enable_user instead")
     def enable_by_username(cls, http_client: igz_mgmt.client.APIClient, username: str):
         """Enables the user by username.
 
         Args:
             http_client (APIClient): The client to use.
             username (str): The user username.
         """
-        user = cls.get_by_username(http_client, username)
-        return user.enable(http_client)
+        return cls.enable_user(http_client, username)
 
     @classmethod
+    @deprecated(reason="Use enable_user instead")
     def enable_by_id(cls, http_client: igz_mgmt.client.APIClient, user_id: str):
         """Enables the user by user id.
 
         Args:
             http_client (APIClient): The client to use.
             user_id (str): The user id.
         """
-        user = cls.get(http_client, user_id)
+        return cls.enable_user(http_client, user_id)
+
+    @classmethod
+    def enable_user(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        user: typing.Union[str, int, "User"],
+    ):
+        """Enables the user.
+
+        Args:
+            http_client (APIClient): The client to use.
+            user (str or int or User): The user id, username or user instance.
+        """
+        user = cls._get_from_arg(http_client, user)
         return user.enable(http_client)
 
+    @classmethod
+    def _get_from_arg(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        user: typing.Union[str, int, "User"],
+    ):
+        if isinstance(user, User):
+            return user
+
+        # check if we got a user id
+        if igz_mgmt.common.helpers.is_uuid4(user):
+            return cls.get(http_client, user)
+
+        # here we assume that we want to get user by username
+        return cls.get_by_username(http_client, user)
+
     @staticmethod
     def _ensure_user_in_group(user, group_id: str) -> bool:
         """Ensures that a user has a group in its relationships.
 
         e.g.:
         If group is not in user relationships, add it and return True
         Alternatively, if group is in user relationships, return False
@@ -751,37 +844,58 @@
 
         1. get the user
         2. add the group to the user
         3. update the group
 
         Args:
             http_client (APIClient): The client to use.
-            user (str or int or User): The user id or user instance to add.
+            user (str or int or User): The user id or username or user instance to add.
         """
-        if not isinstance(user, User):
-            user = User.get(http_client, user)
+        user = User._get_from_arg(http_client, user)
         user.add_to_group(http_client, self)
         self.__dict__.update(Group.get(http_client, self.id))
 
     def remove_user(
         self,
         http_client: igz_mgmt.client.APIClient,
         user: typing.Union[str, int, "User"],
+        force=False,
     ):
         """Removes a user from group.
 
         Args:
             http_client (APIClient): The client to use.
-            user (str ot int or User): The user id or user instance to remove.
+            user (str ot int or User): The user id or username or user instance to remove.
+            force (bool): force (bool): Whether to force the removal of the user from the group(for example, from its
+                                        primary group).
         """
-        if not isinstance(user, User):
-            user = User.get(http_client, user)
-        user.remove_from_group(http_client, self)
+        user = User._get_from_arg(http_client, user)
+        user.remove_from_group(http_client, self, force)
         self.__dict__.update(Group.get(http_client, self.id))
 
+    @classmethod
+    def _get_from_arg(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        group: typing.Union[str, int, "Group"],
+    ):
+        if not group:
+            # in case group is None or empty string we want to return it (for example to unset primary group)
+            return group
+
+        if isinstance(group, Group):
+            return group
+
+        # check if we got a group id
+        if igz_mgmt.common.helpers.is_uuid4(group):
+            return cls.get(http_client, group)
+
+        # here we assume that we want to get user by username
+        return cls.get_by_name(http_client, group)
+
 
 class AccessKey(BaseResource):
     """AccessKey resource represents access key in the system."""
 
     type: str = "access_key"
     tenant_id: str = ""
     ttl: int = 315360000  # 10 years
@@ -981,15 +1095,15 @@
     _skip_apply: bool = False
 
     @staticmethod
     @contextlib.contextmanager
     def apply_services(
         http_client: igz_mgmt.client.APIClient,
         force_apply_all_mode: igz_mgmt.constants.ForceApplyAllMode = igz_mgmt.constants.ForceApplyAllMode.disabled,
-    ):
+    ) -> typing.ContextManager["AppServicesManifest"]:
         """A context manager to apply services with multiple changes at once.
 
         Args:
             http_client (APIClient): The client to use.
             force_apply_all_mode (ForceApplyAllMode, optional): Disabled by default.
 
         Returns:
@@ -1427,15 +1541,15 @@
 
     @contextlib.contextmanager
     def apply(
         self,
         http_client: igz_mgmt.client.APIClient,
         wait_for_job: bool = True,
         notify_by_email: bool = False,
-    ) -> "ProjectAuthorizationRoleSet":
+    ) -> typing.ContextManager["ProjectAuthorizationRoleSet"]:
         """Apply the changes made to the roles.
 
         This function allows multiple membership changes with a single api call by context manager.
         It sets skip apply, yields itself for the context manager so user can run any function without applying,
         sets the value back and applies when context manager exists.
 
         Args:
@@ -1557,50 +1671,67 @@
     admin_status: str = igz_mgmt.constants.ProjectAdminStatuses.online
     operational_status: str = igz_mgmt.constants.ProjectOperationalStatuses.creating
 
     # e.g.: [{"name":"", "value":""}, ...]
     labels: typing.List[typing.Dict[str, str]] = []
     annotations: typing.List[typing.Dict[str, str]] = []
 
+    # e.g.: [{"name":"", "value":""}, ...]
+    # NOTE: Supported on Iguazio systems >= 3.5.5
+    default_function_node_selector: typing.List[typing.Dict[str, str]] = []
+
     mlrun_project: str = ""
     nuclio_project: str = ""
 
     @classmethod
     def create(
         cls,
         http_client: igz_mgmt.client.APIClient,
         name: str,
         description: str = "",
         labels: typing.List[typing.Dict[str, str]] = None,
         annotations: typing.List[typing.Dict[str, str]] = None,
         owner: typing.Union[str, "User", None] = None,
         wait_for_completion=True,
+        default_function_node_selector: typing.List[typing.Dict[str, str]] = None,
     ) -> "Project":
         """Creates a new project.
 
         Args:
             http_client (APIClient): The client to use.
             name (str): The project name.
             description (str, optional): The project description.
             labels (typing.List[typing.Dict[str, str]], optional): The project labels.
             annotations (typing.List[typing.Dict[str, str]], optional): The project annotations.
             owner (str or User or None): The project owner. None by default
             wait_for_completion (bool): Whether to wait for the job to complete
+            default_function_node_selector (typing.List[typing.Dict[str, str]], optional): The default node
+            selectors to be used for functions in the project. (Supported on Iguazio systems >= 3.5.5)
 
         Returns:
             Project: The project instance.
         """
         attributes = {
             "name": name,
             "description": description,
             "labels": labels,
             "annotations": annotations,
+            "default_function_node_selector": default_function_node_selector,
         }
 
-        relationships = cls._fill_relationships(owner=owner)
+        if http_client.version < semver.VersionInfo.parse("3.5.5"):
+            attributes.pop("default_function_node_selector", None)
+            if default_function_node_selector:
+                http_client._logger.warn_with(
+                    "default_function_node_selector is not supported on this Iguazio version, ignoring",
+                    default_function_node_selector=default_function_node_selector,
+                    iguazio_version=http_client.version.__str__(),
+                )
+
+        relationships = cls._fill_relationships(http_client, owner=owner)
 
         created_resource = cls._get_crud().create(
             http_client,
             attributes=attributes,
             relationships=relationships,
             headers=cls._resolve_project_header(),
         )
@@ -1720,47 +1851,55 @@
     def set_owner(
         self, http_client: igz_mgmt.client.APIClient, owner: typing.Union[str, "User"]
     ):
         """Sets the owner of the project.
 
         Args:
             http_client (APIClient): The client to use.
-            owner (str or User): The user id or user instance.
+            owner (str or User): The user id or user name or user instance.
 
         Returns:
             Project: The project instance.
         """
-        relationships = self._fill_relationships(owner=owner)
-        return self.update(http_client, relationships=relationships)
+        relationships = self._fill_relationships(http_client, owner=owner)
+        try:
+            return self.update(http_client, relationships=relationships)
+        except igz_mgmt.exceptions.ResourceNotFoundException:
+            # we return None here because if we reach ResourceNotFoundException it means that current user have
+            # no access to this project anymore
+            return
 
     def get_user_effective_role(
-        self, user: typing.Union[str, "User"]
+        self, http_client: igz_mgmt.client.APIClient, user: typing.Union[str, "User"]
     ) -> typing.Optional[igz_mgmt.constants.ProjectAuthorizationRoles]:
         """Returns the effective role of the user.
 
         Args:
-            user (str or User): The user id or user instance.
+            http_client (APIClient): The client to use.
+            user (str or User): The user id or username or user instance.
 
         Returns:
             str: The effective role of the user.
         """
-        user = user if isinstance(user, User) else User.get(self._http_client, user)
+        # in general case we should have _http_client set, but in case we don't we use the one passed
+        client = self._http_client or http_client
+        user = User._get_from_arg(client, user)
 
         authorization_roles = self._authorization_roles
 
         # first we try to resolve member role without checking in groups
         member_role = authorization_roles.resolve_member_role(user)
         if member_role:
             member_role = member_role.name
         # we try to resolve the role by checking in groups from high role to low
         for role in igz_mgmt.constants.ROLE_ORDER:
             current_role = authorization_roles.roles.get(role, None)
             if current_role:
                 for group in current_role.groups:
-                    if user.in_group(self._http_client, group):
+                    if user.in_group(client, group):
                         member_role = igz_mgmt.common.helpers.get_highest_role(
                             current_role.name, member_role
                         )
         return member_role
 
     def get_viewer_users(self):
         """Returns the project viewer users."""
@@ -1935,15 +2074,15 @@
 
     @contextlib.contextmanager
     def apply_authorization_roles(
         self,
         http_client: igz_mgmt.client.APIClient,
         wait_for_job: bool = True,
         notify_by_email: bool = False,
-    ) -> "ProjectAuthorizationRoleSet":
+    ) -> typing.ContextManager["ProjectAuthorizationRoleSet"]:
         """Returns a context manager that applies the authorization roles.
 
         Args:
             http_client (APIClient): The client to use.
             wait_for_job (bool, optional): Wait for job completion. Defaults to True.
             notify_by_email (bool, optional): Notify by email. Defaults to False.
 
@@ -1953,14 +2092,39 @@
         authorization_roles = self._authorization_roles
         yield authorization_roles
         with authorization_roles.apply(
             http_client, wait_for_job, notify_by_email
         ) as authorization_roles:
             authorization_roles.apply(http_client, wait_for_job, notify_by_email)
 
+    @classmethod
+    def _get_from_arg(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        project: typing.Union[str, int, "Project"],
+    ):
+        if isinstance(project, Project):
+            return project
+
+        # check if we got a group id
+        if cls._is_project_id(http_client.version, project):
+            return Project.get(http_client, project)
+
+        # here we assume that we want to get user by username
+        return Project.get_by_name(http_client, project)
+
+    @classmethod
+    def _is_project_id(
+        cls, iguazio_system_version: semver.VersionInfo, project_id: str
+    ):
+        if iguazio_system_version >= semver.VersionInfo.parse("3.5.4"):
+            project_pattern = r"[\w.-]+@[\w.-]+"
+            return re.match(project_pattern, project_id) is not None
+        return igz_mgmt.common.helpers.is_uuid4(project_id)
+
     @property
     def _authorization_roles(self):
         """Returns the project authorization roles."""
         project = self.get(
             self._http_client,
             self.id,
             include=[
@@ -2028,22 +2192,22 @@
         if deletion_strategy:
             headers[
                 igz_mgmt.constants._RequestHeaders.deletion_strategy_header
             ] = deletion_strategy
         return headers
 
     @staticmethod
-    def _fill_relationships(owner: typing.Union[str, "User", None]):
+    def _fill_relationships(http_client, owner: typing.Union[str, "User", None]):
         relationships = collections.defaultdict(dict)
         if owner:
-            user_id = owner.id if isinstance(owner, User) else owner
+            owner = User._get_from_arg(http_client, owner)
             relationships["owner"] = {
                 "data": {
                     "type": "user",
-                    "id": user_id,
+                    "id": owner.id,
                 },
             }
         return relationships
 
 
 class Event(BaseResource):
     """Event resource represents events in the system.
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/common/__init__.py` & `igz_mgmt-0.1.1/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/igz_mgmt/common/helpers.py` & `igz_mgmt-0.1.1/igz_mgmt/common/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import os
 import random
 import string
 import time
 import traceback
 import typing
+import uuid
 
 import igz_mgmt.constants
 
 # lazy load namespace resolution
 _running_namespace = None
 
 
@@ -215,7 +216,15 @@
     if not (role1 and role2):
         return role1 or role2
     role_index = min(
         igz_mgmt.constants.ROLE_ORDER.index(role1),
         igz_mgmt.constants.ROLE_ORDER.index(role2),
     )
     return igz_mgmt.constants.ROLE_ORDER[role_index]
+
+
+def is_uuid4(s):
+    try:
+        uuid.UUID(s, version=4)
+        return True
+    except ValueError:
+        return False
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.1.1/igz_mgmt/__version__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,10 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from .logger import Logger, get_or_create_logger
+# version can be either one of the following:
+# x.y.z
+# x.y.z.rcN
+# x.y.zrcN
 
-__all__ = ["get_or_create_logger", "Logger"]
+__version__ = "0.1.1"
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/logger/logger.py` & `igz_mgmt-0.1.1/igz_mgmt/logger/logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,35 +17,31 @@
 import sys
 
 
 class HumanReadableFormatter(logging.Formatter):
     def __init__(self):
         super(HumanReadableFormatter, self).__init__()
 
-    def format(self, record):
-        record_with = getattr(record, "with", {})
-        if record_with:
-            more = ": {0}".format(record_with)
-        else:
-            more = ""
-
-        # take last 30 chars of logger name, if shorter, take all, if longer, take last 30
+    def format(
+        self, record
+    ):  # take last 30 chars of logger name, if shorter, take all, if longer, take last 30
         logger_name = record.name[-30:]
-        return "{0} {1:30} [{2}] {3}{4}".format(
+        return "{0} {1:30} [{2}] {3}".format(
             self.formatTime(record, self.datefmt),
             logger_name,
             record.levelname.lower(),
             record.getMessage(),
-            more,
         )
 
 
 class Logger(object):
-    def __init__(self, level="DEBUG", logger_name=None):
-        self._logger = logging.getLogger("root" if not logger_name else logger_name)
+    def __init__(self, level="DEBUG", logger_name=None, logger=None):
+        self._logger = logger or logging.getLogger(
+            "root" if not logger_name else logger_name
+        )
         self.set_level(level)
         self._handlers = {}
 
     def set_handler(self, handler_name, file, formatter):
         # check if there's a handler by this name
         if handler_name in self._handlers:
             self._logger.removeHandler(self._handlers[handler_name])
@@ -85,30 +81,35 @@
     def warn(self, message, *args):
         self._logger.warning(message, *args)
 
     def error(self, message, *args):
         self._logger.error(message, *args)
 
     def debug_with(self, message, *args, **kw_args):
-        self._logger.debug(message, *args, extra={"with": kw_args})
+        self._logger.debug(self._add_kw_args_to_message(message, kw_args), *args)
 
     def info_with(self, message, *args, **kw_args):
-        self._logger.info(message, *args, extra={"with": kw_args})
+        self._logger.info(self._add_kw_args_to_message(message, kw_args), *args)
 
     def warn_with(self, message, *args, **kw_args):
-        self._logger.warning(message, *args, extra={"with": kw_args})
+        self._logger.warning(self._add_kw_args_to_message(message, kw_args), *args)
 
     def error_with(self, message, *args, **kw_args):
-        self._logger.error(message, *args, extra={"with": kw_args})
+        self._logger.error(self._add_kw_args_to_message(message, kw_args), *args)
+
+    @staticmethod
+    def _add_kw_args_to_message(message, kw_args):
+        return "{0}: {1}".format(message, kw_args) if kw_args else message
 
 
 _logger = None
 
 
-def get_or_create_logger(level="DEBUG", name="root"):
+def get_or_create_logger(level="DEBUG", name="root", logger=None):
     global _logger
     if not _logger:
-        _logger = Logger(level=level, logger_name=name)
-        _logger.set_handler("stdout", sys.stdout, HumanReadableFormatter())
+        _logger = Logger(level=level, logger_name=name, logger=logger)
+        if not logger:
+            _logger.set_handler("stdout", sys.stdout, HumanReadableFormatter())
     if _logger._logger.name != name:
         return _logger.get_child(name)
     return _logger
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.1.1/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.1.1/igz_mgmt/schemas/app_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,14 +251,40 @@
     ]
     demos_datasets_archive_address: typing.Optional[str]
     docker_registry_name: typing.Optional[str]
     ssh_enabled: typing.Optional[bool]
     ssh_server: typing.Optional[SSHServerSpec]
 
 
+class FilebeatSpec(CustomAppServiceSpec):
+    """Filebeat app service spec."""
+
+    elasticsearch_url: typing.Optional[str] = pydantic.Field(
+        description="Elasticsearch node to connect to"
+    )
+    elasticsearch_username: typing.Optional[str] = pydantic.Field(
+        description="The basic authentication username for connecting to Elasticsearch"
+    )
+    elasticsearch_password: typing.Optional[str] = pydantic.Field(
+        description="The basic authentication password for connecting to Elasticsearch"
+    )
+    elasticsearch_ssl_verification_mode: typing.Optional[
+        igz_mgmt.constants.SslVerificationMode
+    ] = pydantic.Field(
+        igz_mgmt.constants.SslVerificationMode.full,
+        description="Controls the verification of server certificates",
+    )
+    update_index_template: typing.Optional[bool] = pydantic.Field(
+        True,
+        description="When this option is True, the platform updates the Elasticsearch index "
+        "template that's used for Log Forwarder indices. Send False if you wish to "
+        "configure the index template yourself",
+    )
+
+
 class AppServiceSpec(AppServicesOperationBaseModel):
     """App service spec."""
 
     name: str = pydantic.Field(description="The name of the app service")
     kind: str = pydantic.Field(description="The app service kind (jupyter / shell .. )")
 
     # optional fields
@@ -303,23 +329,23 @@
     authentication_mode: typing.Optional[str]
     security_context: typing.Optional[SecurityContextSpec]
     persistency_mode: typing.Optional[str]
     advanced: typing.Optional[AdvancedSpec]
 
     # app services
     jupyter: typing.Optional[JupyterSpec]
+    filebeat: typing.Optional[FilebeatSpec]
 
     # TODO: add service specs
     webapi: typing.Optional[CustomAppServiceSpec]
     v3io_prometheus: typing.Optional[CustomAppServiceSpec]
     nuclio: typing.Optional[CustomAppServiceSpec]
     docker_registry: typing.Optional[CustomAppServiceSpec]
     shell: typing.Optional[CustomAppServiceSpec]
     presto: typing.Optional[CustomAppServiceSpec]
-    filebeat: typing.Optional[CustomAppServiceSpec]
     grafana: typing.Optional[CustomAppServiceSpec]
     mariadb: typing.Optional[CustomAppServiceSpec]
     hive: typing.Optional[CustomAppServiceSpec]
     monitoring: typing.Optional[CustomAppServiceSpec]
     dex: typing.Optional[CustomAppServiceSpec]
     oauth2_proxy: typing.Optional[CustomAppServiceSpec]
     metrics_server_exporter: typing.Optional[CustomAppServiceSpec]
```

### Comparing `igz_mgmt-0.1.0/igz_mgmt/schemas/events.py` & `igz_mgmt-0.1.1/igz_mgmt/schemas/events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.1.1/igz_mgmt/schemas/manual_events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/LICENSE` & `igz_mgmt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.0/pyproject.toml` & `igz_mgmt-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "httpx~=0.24.1",
     "inflection~=0.5.1",
     "pydantic~=1.10.10",
     "semver~=3.0.1",
+    "deprecated~=1.2.14",
 ]
 
 [project.optional-dependencies]
 
 [project.urls]
 Homepage = "https://github.com/iguazio/igz-mgmt-sdk"
```

### Comparing `igz_mgmt-0.1.0/PKG-INFO` & `igz_mgmt-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: igz-mgmt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: deprecated~=1.2.14
 Requires-Dist: httpx~=0.24.1
 Requires-Dist: inflection~=0.5.1
 Requires-Dist: pydantic~=1.10.10
 Requires-Dist: semver~=3.0.1
 Description-Content-Type: text/markdown
 
 # igz-mgmt-sdk
```


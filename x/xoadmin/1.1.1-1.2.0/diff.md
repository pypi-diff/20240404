# Comparing `tmp/xoadmin-1.1.1.tar.gz` & `tmp/xoadmin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.1.1.tar", max compression
+gzip compressed data, was "xoadmin-1.2.0.tar", max compression
```

## Comparing `xoadmin-1.1.1.tar` & `xoadmin-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,30 @@
--rw-r--r--   0        0        0    11336 2024-04-03 18:28:34.045574 xoadmin-1.1.1/LICENSE
--rw-r--r--   0        0        0     1904 2024-04-03 18:28:34.045574 xoadmin-1.1.1/README.md
--rw-r--r--   0        0        0      788 2024-04-03 18:28:34.049574 xoadmin-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/__init__.py
--rw-r--r--   0        0        0      631 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/__main__.py
--rw-r--r--   0        0        0     4536 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/api.py
--rw-r--r--   0        0        0      389 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/error.py
--rw-r--r--   0        0        0     1249 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/host.py
--rw-r--r--   0        0        0     5138 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/manager.py
--rw-r--r--   0        0        0      816 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/storage.py
--rw-r--r--   0        0        0     2381 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/user.py
--rw-r--r--   0        0        0     1523 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/vm.py
--rw-r--r--   0        0        0     5719 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/websocket.py
--rw-r--r--   0        0        0        0 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/__init__.py
--rw-r--r--   0        0        0      614 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/config.py
--rw-r--r--   0        0        0     1287 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/configurator.py
--rw-r--r--   0        0        0      274 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/loader.py
--rw-r--r--   0        0        0     1822 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/utils.py
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 xoadmin-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-04 20:24:18.997663 xoadmin-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5934 2024-04-04 20:24:18.997663 xoadmin-1.2.0/README.md
+-rw-r--r--   0        0        0      787 2024-04-04 20:24:18.997663 xoadmin-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     2192 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     6696 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0     1418 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     3824 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1586 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5724 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/apply.py
+-rw-r--r--   0        0        0     2199 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/auth.py
+-rw-r--r--   0        0        0     1433 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/cli.py
+-rw-r--r--   0        0        0     4542 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/config.py
+-rw-r--r--   0        0        0     2002 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/hosts.py
+-rw-r--r--   0        0        0     1751 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/model.py
+-rw-r--r--   0        0        0      784 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/options.py
+-rw-r--r--   0        0        0     1937 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/storage.py
+-rw-r--r--   0        0        0     2046 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/users.py
+-rw-r--r--   0        0        0     6103 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/utils.py
+-rw-r--r--   0        0        0     1940 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/vms.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      692 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1462 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      277 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     6798 1970-01-01 00:00:00.000000 xoadmin-1.2.0/PKG-INFO
```

### Comparing `xoadmin-1.1.1/LICENSE` & `xoadmin-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.1/src/xoadmin/api/api.py` & `xoadmin-1.2.0/src/xoadmin/api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,37 @@
 
 
 class XOAPI:
     """An asynchronous client for interacting with Xen Orchestra's REST API."""
 
     def __init__(
         self,
-        base_url: str,
+        rest_base_url: str,
         ws_url: str = None,
         credentials: Dict[str, str] = None,
         verify_ssl: bool = True,
     ) -> None:
-        self.base_url = base_url
+        self.verify_ssl = verify_ssl
+        self.rest_base_url = rest_base_url
         self.session = httpx.AsyncClient(verify=verify_ssl, follow_redirects=True)
         self.auth_token = None
         # Initialize WebSocket connection for authentication
         self.ws_url = ws_url or "ws://localhost"
         self.credentials = credentials or {
             "email": "admin@admin.net",
             "password": "admin",
         }
         self.ws = XOSocket(url=self.ws_url, verify_ssl=verify_ssl)
 
     def get_socket(self) -> XOSocket:
         return self.ws
 
-    def verify_ssl(self, enabled: bool):
+    def set_verify_ssl(self, enabled: bool):
         self.ws = XOSocket(url=self.ws_url, verify_ssl=enabled)
+        self.verify_ssl = self.ws.verify_ssl
 
     def set_credentials(self, username: str, password: str):
         self.credentials = {"email": str(username), "password": str(password)}
         self.ws.set_credentials(username=username, password=password)
 
     async def authenticate_with_websocket(self, username: str, password: str) -> None:
         self.set_credentials(username=username, password=password)
@@ -74,19 +76,19 @@
             logger.error("No credentials stored for refreshing the token.")
             raise AuthenticationError(
                 "Unable to refresh token due to missing credentials."
             )
         await self.authenticate_with_websocket(
             self.credentials["email"], self.credentials["password"]
         )
-        logger.info("Authentication token refreshed.")
+        logger.debug("Authentication token refreshed.")
 
     async def _request(self, method: str, endpoint: str, **kwargs: Any) -> Any:
         # Prepare the URL
-        url = f"{self.base_url}/{endpoint}"
+        url = f"{self.rest_base_url}/{endpoint}"
         # Ensure cookies are correctly set for the session
         if self.auth_token:
             self.session.cookies.set("authenticationToken", self.auth_token)
         else:
             logger.error("No authentication token available.")
             raise AuthenticationError("Authentication required.")
         # Make the request
```

### Comparing `xoadmin-1.1.1/src/xoadmin/api/host.py` & `xoadmin-1.2.0/src/xoadmin/api/host.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,7 +34,34 @@
 
         # Ensure you're opening and closing the WebSocket connection appropriately.
         socket = self.xo_api.get_socket()
         await socket.open()
         result = await socket.call("server.add", params)
         await socket.close()
         return result
+
+    async def list_hosts(self):
+        """
+        Retrieves a list of all registered Xen servers.
+
+        :return: A list of dictionaries containing host information.
+        """
+        # Ensure you're opening and closing the WebSocket connection appropriately.
+        socket = self.xo_api.get_socket()
+        await socket.open()
+        result = await socket.call("server.getAll", {})  # Empty params for all hosts
+        await socket.close()
+        return result
+
+    async def delete_host(self, host_id: str):
+        """
+        Deletes a Xen server by its ID.
+
+        :param host_id: The ID of the host to be deleted.
+        """
+        # Ensure you're opening and closing the WebSocket connection appropriately.
+        socket = self.xo_api.get_socket()
+        await socket.open()
+        params = {"id": host_id}
+        result = await socket.call("server.remove", params)
+        await socket.close()
+        return result
```

### Comparing `xoadmin-1.1.1/src/xoadmin/api/manager.py` & `xoadmin-1.2.0/src/xoadmin/api/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,55 +2,98 @@
 from typing import Any
 
 from xoadmin.api.api import XOAPI
 from xoadmin.api.error import AuthenticationError, ServerError, XOSocketError
 from xoadmin.api.host import HostManagement
 from xoadmin.api.storage import StorageManagement
 from xoadmin.api.user import UserManagement
-from xoadmin.utils import get_logger
 from xoadmin.api.vm import VMManagement
+from xoadmin.utils import get_logger
 
 logger = get_logger(__name__)
 
 
 class XOAManager:
     """
     A manager class for orchestrating interactions with the Xen Orchestra API,
     handling authentication, and managing resources.
     """
 
-    def __init__(self, base_url: str, verify_ssl: bool = True):
-        self.base_url = base_url
-        self.ws_url = self._convert_http_to_ws(base_url)
-        self.api = XOAPI(self.base_url, ws_url=self.ws_url, verify_ssl=verify_ssl)
+    def __init__(
+        self,
+        host: str,
+        rest_base_url: str = None,
+        ws_url: str = None,
+        verify_ssl: bool = True,
+    ):
+        self.host = host
+        self.verify_ssl = verify_ssl
+        self.rest_base_url = self._sanitize_rest_base_url(rest_base_url, host)
+        self.ws_url = self._sanitize_ws(ws_url)
+        self.api = XOAPI(
+            self.rest_base_url, ws_url=self.ws_url, verify_ssl=self.verify_ssl
+        )
         # The management classes will be initialized after authentication
         self.user_management = None
         self.vm_management = None
         self.storage_management = None
 
-    def _convert_http_to_ws(self, url: str) -> str:
+    def _sanitize_rest_base_url(self, rest_base_url: str, host: str) -> str:
         """
-        Converts an HTTP or HTTPS URL to its WebSocket equivalent (WS or WSS).
+        Sanitizes the REST base URL, ensuring it includes the protocol and default port.
 
         Parameters:
-            url (str): The HTTP or HTTPS URL.
+            rest_base_url (str): The REST base URL.
+            host (str): The host address.
+            verify_ssl (bool): Whether to verify SSL certificates.
 
         Returns:
-            str: The converted WS or WSS URL.
+            str: The sanitized REST base URL.
         """
-        if url.startswith("https://"):
-            return url.replace("https://", "wss://", 1)
-        elif url.startswith("http://"):
-            return url.replace("http://", "ws://", 1)
+        if not rest_base_url:
+            protocol = "https" if self.verify_ssl else "http"
+            return f"{protocol}://{host}"
+        elif rest_base_url.startswith(("http://", "https://")):
+            return rest_base_url
         else:
             raise ValueError("URL must start with http:// or https://")
 
-    def verify_ssl(self, enabled: bool) -> None:
-        self.api.verify_ssl(enabled)
-        logger.info(
+    def _sanitize_ws(self, ws_url: str) -> str:
+        """
+        Sanitizes the WebSocket URL, ensuring it follows the correct format.
+
+        Parameters:
+            ws_url (str): The WebSocket URL or hostname.
+
+        Returns:
+            str: The sanitized WebSocket URL.
+        """
+        protocol = "wss" if self.verify_ssl else "ws"
+        if not ws_url:
+            return f"{protocol}://{self.host}"
+
+        if "://" in ws_url:
+            if ws_url.startswith(("ws://", "wss://", "http://", "https://")):
+                # Replace http/https with appropriate WebSocket protocol
+                ws_url = ws_url.replace("http://", "ws://").replace(
+                    "https://", "wss://"
+                )
+                return ws_url  # URL already contains correct protocol
+            else:
+                raise ValueError(
+                    "WebSocket URL must start with http://, https://, ws://, or wss://"
+                )
+        else:
+            # If ws_url is a simple hostname or hostname:port
+            return f"{protocol}://{ws_url}"
+
+    def set_verify_ssl(self, enabled: bool) -> None:
+        self.api.set_verify_ssl(enabled)
+        self.verify_ssl = self.api.ws.verify_ssl
+        logger.debug(
             f"SSL verification {'enabled' if self.api.ws.verify_ssl else 'disabled'}."
         )
 
     async def authenticate(self, username: str, password: str) -> None:
         """
         Authenticates with the Xen Orchestra API using the provided credentials
         and initializes the management classes.
@@ -58,15 +101,15 @@
         await self.api.authenticate_with_websocket(username, password)
 
         # Initialize management classes with the authenticated API instance
         self.user_management = UserManagement(self.api)
         self.vm_management = VMManagement(self.api)
         self.storage_management = StorageManagement(self.api)
         self.host_management = HostManagement(self.api)
-        logger.info("Authenticated and ready to manage Xen Orchestra.")
+        logger.debug("Authenticated and ready to manage Xen Orchestra.")
 
     async def create_user(
         self, email: str, password: str, permission: str = "none"
     ) -> Any:
         """
         Creates a new user with the specified email, password, and permission level."""
         # Directly use the method from UserManagement
@@ -129,15 +172,15 @@
         Closes the session.
         """
         await self.api.close()
 
 
 # Example usage
 async def main():
-    manager = XOAManager("http://localhost:80", verify_ssl=False)
+    manager = XOAManager("localhost", "http://localhost:80", verify_ssl=False)
     await manager.authenticate(username="admin", password="password")
     vms = await manager.list_all_vms()
     print(vms)
     await manager.close()
 
 
 if __name__ == "__main__":
```

### Comparing `xoadmin-1.1.1/src/xoadmin/api/user.py` & `xoadmin-1.2.0/src/xoadmin/api/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 
 class UserManagement:
     """Manage user operations within Xen Orchestra."""
 
     def __init__(self, api: XOAPI) -> None:
         self.api = api
 
-    async def list_users(self) -> List[Dict[str, Any]]:
-        """List all users."""
-        # Assuming listing users still works via REST API
+    async def list_users(self) -> List[str]:
+        """List all users by their API paths."""
         return await self.api.get("rest/v0/users")
 
+    async def get_user_details(self, user_path: str) -> Dict[str, Any]:
+        """Fetch detailed information for a user given their API path."""
+        user_id = user_path.split("/")[-1]
+        return await self.api.get(f"rest/v0/users/{user_id}")
+
     async def create_user(
         self, email: str, password: str, permission: str = "none"
     ) -> Dict[str, Any]:
         """
         Create a new user with the specified details.
         This method now uses WebSocket and JSON-RPC for user creation.
         """
@@ -56,10 +60,39 @@
 
         except Exception as e:
             # Catch all for any other unexpected errors
             logger.error(f"Unexpected error occurred: {e}")
             raise
 
     async def delete_user(self, user_id: str) -> bool:
-        """Delete a user by their ID."""
-        # Assuming delete still works via REST API
-        return await self.api.delete(f"rest/v0/users/{user_id}")
+        """
+        Delete a user by their ID using WebSocket and JSON-RPC.
+        """
+        try:
+            # Prepare the parameters for the JSON-RPC call
+            params = {"id": user_id}
+            # Utilize the WebSocket connection from the api instance
+            socket = self.api.get_socket()
+            await socket.open()  # Ensure the socket is open
+            # Make the JSON-RPC call to delete the user
+            result = await socket.call("user.delete", params)
+            await socket.close()  # Close the socket after the call
+            # Check the result for success or failure
+            if "result" in result and result["result"]:
+                # Assuming the 'result' contains success information
+                return True
+            else:
+                # Handle potential errors returned by the call
+                error_msg = result.get("error", {}).get(
+                    "message", "Unknown error during user deletion"
+                )
+                raise XOSocketError(f"Failed to delete user: {error_msg}")
+
+        except XOSocketError as e:
+            # Log or handle the specific WebSocket error
+            logger.error(f"WebSocket error occurred: {e}")
+            raise
+
+        except Exception as e:
+            # Catch all for any other unexpected errors
+            logger.error(f"Unexpected error occurred: {e}")
+            raise
```

### Comparing `xoadmin-1.1.1/src/xoadmin/api/vm.py` & `xoadmin-1.2.0/src/xoadmin/api/vm.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,27 +7,28 @@
     """Handles VM operations within Xen Orchestra."""
 
     def __init__(self, api: XOAPI) -> None:
         self.api = api
 
     async def list_vms(self) -> List[Dict[str, Any]]:
         """List all VMs."""
-        return self.api.get("rest/v0/vms")
+        vms = await self.api.get("rest/v0/vms?fields=id,name_label")
+        return vms
 
     async def start_vm(self, vm_id: str) -> Dict[str, Any]:
         """Start a specified VM."""
-        return self.api.post(f"rest/v0/vms/{vm_id}/start", json_data={})
+        return await self.api.post(f"rest/v0/vms/{vm_id}/start", json_data={})
 
     async def stop_vm(self, vm_id: str) -> Dict[str, Any]:
         """Stop a specified VM."""
-        return self.api.post(f"rest/v0/vms/{vm_id}/stop", json_data={})
+        return await self.api.post(f"rest/v0/vms/{vm_id}/stop", json_data={})
 
     async def delete_vm(self, vm_id: str) -> bool:
         """Delete a specified VM."""
-        return self.api.delete(f"rest/v0/vms/{vm_id}")
+        return await self.api.delete(f"rest/v0/vms/{vm_id}")
 
     async def create_vm_from_template(
         self, template_id: str, name: str, description: str = ""
     ) -> Dict[str, Any]:
         """Create a new VM from a specified template."""
         # This method would need to construct the appropriate payload
         # based on your Xen Orchestra's API requirements for VM creation
```

### Comparing `xoadmin-1.1.1/src/xoadmin/api/websocket.py` & `xoadmin-1.2.0/src/xoadmin/api/websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import ssl
-import websockets
 import uuid
 from typing import Dict
 from uuid import uuid4
 
+import websockets
 
 from xoadmin.api.error import AuthenticationError, ServerError, XOSocketError
 from xoadmin.utils import get_logger
 
 logger = get_logger()
 
 
@@ -56,30 +56,30 @@
             ssl_context.check_hostname = False
             ssl_context.verify_mode = ssl.CERT_NONE
 
         try:
             self.websocket = await websockets.connect(
                 self.url, ssl=ssl_context if self.url.startswith("wss://") else None
             )
-            logger.info("Connection opened.")
+            logger.debug("Connection opened.")
             if self.credentials:
                 await self.sign_in(self.credentials)
-                logger.info("Sign in successful.")
+                logger.debug("Sign in successful.")
         except Exception as e:
             logger.error(f"Error opening WebSocket connection: {e}")
             raise
 
         return True
 
     async def close(self):
         """
         Closes the WebSocket connection.
         """
         await self.websocket.close()
-        logger.info("Connection closed.")
+        logger.debug("Connection closed.")
 
     async def call(self, method: str, params: dict = None):
         """
         Performs a JSON-RPC call over the WebSocket connection.
 
         :param method: The JSON-RPC method name to call.
         :param params: A dictionary of parameters to pass with the method call.
@@ -109,15 +109,15 @@
 
         return response_data
 
     async def sign_in(self, credentials: dict):
         response = await self.call("session.signIn", credentials)
         if "result" in response and "authenticationToken" in response["result"]:
             self.user = response["result"]
-            logger.info("Signed in as:", self.user)
+            logger.debug("Signed in as:", self.user)
         elif "error" in response:
             raise XOSocketError(f"Failed to sign in: {response['error']}")
 
     async def create_token(self, description="xoadmin token"):
         """
         Creates an authentication token, including client information.
         """
@@ -127,15 +127,15 @@
         params = {
             "description": description,
             "client": client_info,
         }
         response = await self.call("token.create", params)
         if "result" in response:
             token_id = response["result"]
-            logger.info("Token created successfully")
+            logger.debug("Token created successfully")
             return token_id
         else:
             error_msg = response.get("error", {}).get("message", "Unknown error")
             logger.error(f"Failed to create token: {error_msg}")
             raise XOSocketError(f"Failed to create token: {error_msg}")
```

### Comparing `xoadmin-1.1.1/src/xoadmin/configurator/configurator.py` & `xoadmin-1.2.0/src/xoadmin/configurator/configurator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 from typing import Optional
-from xoadmin.configurator.loader import load_config
-from xoadmin.configurator.config import AppConfig
+
 from xoadmin.api.manager import XOAManager
+from xoadmin.configurator.config import AppConfig
+from xoadmin.configurator.loader import load_config
+
 
 class XOAConfigurator:
     def __init__(self, config_path: str):
         self.config_path = config_path
         self.app_config: Optional[AppConfig] = None
 
     async def load_and_apply_configuration(self):
         self.app_config = load_config(self.config_path)
 
         # Initialize XOAManager with XOA instance details
-        xoa_manager = XOAManager(self.app_config.xoa.host, verify_ssl=False)
-        await xoa_manager.authenticate(username=self.app_config.xoa.username, password=self.app_config.xoa.password)
+        xoa_manager = XOAManager(
+            self.app_config.xoa.host,
+            self.app_config.xoa.rest_api,
+            self.app_config.xoa.websocket,
+            verify_ssl=False,
+        )
+        await xoa_manager.authenticate(
+            username=self.app_config.xoa.username, password=self.app_config.xoa.password
+        )
         # Create users
         for user in self.app_config.users:
-            await xoa_manager.create_user(email=user.username, password=user.password, permission=user.permission)
+            await xoa_manager.create_user(
+                email=user.username, password=user.password, permission=user.permission
+            )
 
         # Add hypervisors
         for hypervisor in self.app_config.hypervisors:
             await xoa_manager.add_host(
                 host=hypervisor.host,
                 username=hypervisor.username,
                 password=hypervisor.password,
                 autoConnect=hypervisor.autoConnect,
                 allowUnauthorized=hypervisor.allowUnauthorized,
             )
 
-        await xoa_manager.close()
+        await xoa_manager.close()
```

### Comparing `xoadmin-1.1.1/src/xoadmin/utils.py` & `xoadmin-1.2.0/src/xoadmin/utils.py`

 * *Files identical despite different names*


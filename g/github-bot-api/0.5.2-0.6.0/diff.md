# Comparing `tmp/github_bot_api-0.5.2.tar.gz` & `tmp/github_bot_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_bot_api-0.5.2.tar", max compression
+gzip compressed data, was "github_bot_api-0.6.0.tar", max compression
```

## Comparing `github_bot_api-0.5.2.tar` & `github_bot_api-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      998 2023-03-09 22:36:46.439504 github_bot_api-0.5.2/LICENSE
--rw-r--r--   0        0        0     1002 2023-03-09 22:36:46.439504 github_bot_api-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     2124 2023-03-15 22:49:34.865741 github_bot_api-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1713 2023-03-15 22:38:54.027862 github_bot_api-0.5.2/readme.md
--rw-r--r--   0        0        0      209 2023-03-15 22:49:34.865741 github_bot_api-0.5.2/src/github_bot_api/__init__.py
--rw-r--r--   0        0        0       59 2023-03-15 22:48:05.860258 github_bot_api-0.5.2/src/github_bot_api/__init__test.py
--rw-r--r--   0        0        0     7160 2023-03-15 22:39:58.754032 github_bot_api-0.5.2/src/github_bot_api/app.py
--rw-r--r--   0        0        0      541 2023-03-15 22:47:56.932510 github_bot_api-0.5.2/src/github_bot_api/app_test.py
--rw-r--r--   0        0        0     3132 2023-03-15 22:38:54.027862 github_bot_api-0.5.2/src/github_bot_api/event.py
--rw-r--r--   0        0        0     1583 2023-03-15 22:38:54.031862 github_bot_api-0.5.2/src/github_bot_api/flask.py
--rw-r--r--   0        0        0        0 2023-03-09 22:36:46.439504 github_bot_api-0.5.2/src/github_bot_api/py.typed
--rw-r--r--   0        0        0     1680 2023-03-15 22:38:54.031862 github_bot_api-0.5.2/src/github_bot_api/signature.py
--rw-r--r--   0        0        0     4498 2023-03-15 22:41:51.962831 github_bot_api-0.5.2/src/github_bot_api/token.py
--rw-r--r--   0        0        0        5 2023-03-09 22:36:46.439504 github_bot_api-0.5.2/src/github_bot_api/utils/__init__.py
--rw-r--r--   0        0        0      738 2023-03-15 22:38:54.031862 github_bot_api-0.5.2/src/github_bot_api/utils/mime.py
--rw-r--r--   0        0        0      233 2023-03-15 22:38:54.031862 github_bot_api-0.5.2/src/github_bot_api/utils/types.py
--rw-r--r--   0        0        0     2103 2023-03-15 22:38:54.031862 github_bot_api-0.5.2/src/github_bot_api/webhook.py
--rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 github_bot_api-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-04-04 18:05:58.973585 github_bot_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0      807 2024-04-04 19:20:23.311817 github_bot_api-0.6.0/README.md
+-rw-r--r--   0        0        0     1980 2024-04-04 19:21:03.100649 github_bot_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      239 2024-04-04 19:21:03.100885 github_bot_api-0.6.0/src/github_bot_api/__init__.py
+-rw-r--r--   0        0        0     6575 2024-04-04 19:18:47.788217 github_bot_api-0.6.0/src/github_bot_api/app.py
+-rw-r--r--   0        0        0      541 2024-04-04 18:05:58.975274 github_bot_api-0.6.0/src/github_bot_api/app_test.py
+-rw-r--r--   0        0        0     3253 2024-04-04 19:18:47.789245 github_bot_api-0.6.0/src/github_bot_api/event.py
+-rw-r--r--   0        0        0     1583 2024-04-04 18:05:58.975595 github_bot_api-0.6.0/src/github_bot_api/flask.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:05:58.975707 github_bot_api-0.6.0/src/github_bot_api/py.typed
+-rw-r--r--   0        0        0     1675 2024-04-04 18:05:58.975894 github_bot_api-0.6.0/src/github_bot_api/signature.py
+-rw-r--r--   0        0        0       59 2024-04-04 18:05:58.974891 github_bot_api-0.6.0/src/github_bot_api/tests/test_import.py
+-rw-r--r--   0        0        0     4493 2024-04-04 18:05:58.976523 github_bot_api-0.6.0/src/github_bot_api/token.py
+-rw-r--r--   0        0        0        5 2024-04-04 18:05:58.976825 github_bot_api-0.6.0/src/github_bot_api/utils/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-04 18:12:22.299825 github_bot_api-0.6.0/src/github_bot_api/utils/functions.py
+-rw-r--r--   0        0        0      738 2024-04-04 18:05:58.977014 github_bot_api-0.6.0/src/github_bot_api/utils/mime.py
+-rw-r--r--   0        0        0      233 2024-04-04 18:05:58.977187 github_bot_api-0.6.0/src/github_bot_api/utils/types.py
+-rw-r--r--   0        0        0     2055 2024-04-04 18:05:58.977349 github_bot_api-0.6.0/src/github_bot_api/webhook.py
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 github_bot_api-0.6.0/PKG-INFO
```

### Comparing `github_bot_api-0.5.2/LICENSE` & `github_bot_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `github_bot_api-0.5.2/pyproject.toml` & `github_bot_api-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "github-bot-api"
-version = "0.5.2"
+version = "0.6.0"
 description = "API for creating GitHub bots and webhooks in Python."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
-readme = "readme.md"
+readme = "README.md"
 packages = [{ include = "github_bot_api", from = "src" }]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -20,35 +20,31 @@
     "Programming Language :: Python :: 3.11"
 ]
 keywords = []
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-github-bot-api/issues"
 Documentation = "https://niklasrosenstein.github.io/python-github-bot-api/"
-Homepage = "https://github.com/NiklasRosenstein/python-github-bot-api"
 Repository = "https://github.com/NiklasRosenstein/python-github-bot-api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"nr.functional" = "^0.2.0"
-cryptography = "^39.0.2"
-Deprecated = "^1.2.13"
+cryptography = "^42.0.5"
 flask = { version = "*", optional = true }
 PyGithub = { version = "^1.58", optional = true }
 PyJWT = "^2.6.0"
 requests = "^2.28.2"
 urllib3 = "^1.26.15"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pytest = "*"
-types-deprecated = "*"
 types-flask = "*"
 types-requests = "*"
 
 [tool.slap]
 typed = true
 
 [tool.slap.test]
```

### Comparing `github_bot_api-0.5.2/src/github_bot_api/app.py` & `github_bot_api-0.6.0/src/github_bot_api/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 import dataclasses
 import logging
 import sys
 import threading
 import typing as t
 
-import deprecated
 import requests
 import urllib3
-from nr.functional import coalesce
 
 from . import __version__
 from .token import InstallationTokenSupplier, JwtSupplier, TokenInfo
+from .utils.functions import coalesce
 
 T = t.TypeVar("T")
 logger = logging.getLogger(__name__)
 user_agent = f"python/{sys.version.split()[0]} github-bot-api/{__version__}"
 
 if t.TYPE_CHECKING:
     import github
@@ -62,46 +61,29 @@
         )
 
 
 @dataclasses.dataclass
 class GithubApp:
     """
     Represents a GitHub application and all the required details.
-
-    # Example
-
-    ```py
-    import os
-    from github_bot_api import GithubApp
-
-    with open(os.environ['PRIVATE_KEY_FILE']) as fp:
-      private_key = fp.read()
-
-    app = GithubApp(
-      user_agent='my-bot/0.0.0',
-      app_id=int(os.environ['APP_ID']),
-      private_key=private_key)
-
-    print(app.app_client().get_app().owner)
-    ```
     """
 
     PUBLIC_GITHUB_V3_API_URL = "https://api.github.com"
 
-    #: User agent of the application. This will be respected in #get_user_agent().
     user_agent: str
+    """User agent of the application. This will be respected in #get_user_agent()."""
 
-    #: GitHub Application ID.
     app_id: int
+    """GitHub Application ID."""
 
-    #: RSA private key to sign the JWT with.
     private_key: str
+    """RSA private key to sign the JWT with."""
 
-    #: GitHub API base URL. Defaults to the public GitHub API.
     v3_api_url: str = PUBLIC_GITHUB_V3_API_URL
+    """GitHub API base URL. Defaults to the public GitHub API."""
 
     def __post_init__(self):
         self._jwt_supplier = JwtSupplier(self.app_id, self.private_key)
         self._lock = threading.Lock()
         self._installation_tokens: t.Dict[int, InstallationTokenSupplier] = {}
 
     def _get_base_github_client_settings(self) -> GithubClientSettings:
@@ -129,23 +111,14 @@
     def jwt_supplier(self) -> JwtSupplier:
         """
         Returns a new #JwtSupplier that is used for generating JWT tokens for your GitHub application.
         """
 
         return JwtSupplier(self.app_id, self.private_key)
 
-    @property
-    @deprecated.deprecated(reason="use GithubApp.app_client() instead", version="0.4.0")
-    def client(self) -> "github.Github":
-        """
-        Use #app_client() instead.
-        """
-
-        return self.app_client()
-
     def app_client(self, settings: t.Union[GithubClientSettings, t.Dict[str, t.Any], None] = None) -> "github.Github":
         """
         Returns a PyGithub client for your GitHub application.
 
         Note that the client's token will expire after 10 minutes and you will have to create a new client or update the
         client's token with the value returned by #jwt. It is recommended that you create a new client for each atomic
         operation you perform.
```

### Comparing `github_bot_api-0.5.2/src/github_bot_api/app_test.py` & `github_bot_api-0.6.0/src/github_bot_api/app_test.py`

 * *Files identical despite different names*

### Comparing `github_bot_api-0.5.2/src/github_bot_api/event.py` & `github_bot_api-0.6.0/src/github_bot_api/event.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,58 +17,58 @@
 
 @dataclass
 class Event:
     """
     Represents a GitHub webhook event.
     """
 
-    #: The name of the event. Could be `pull_request`, for example.
     name: str
+    """ The name of the event. Could be `pull_request`, for example."""
 
-    #: The delivery ID of the event.
     delivery_id: str
+    """The delivery ID of the event."""
 
-    #: The signature of the event. Will only be set if a Webhook-secret is configured on the
-    #: client side (e.g. in #Webhook.secret / if the *webhook_secret* parameter is passed to
-    #: #accept_event()).
     signature: t.Optional[str]
+    """The signature of the event. Will only be set if a Webhook-secret is configured on the
+    client side (e.g. in [`Webhook.secret`][github_bot_api.webhook.Webhook] / if the *webhook_secret* parameter is
+    passed to [`accept_event()`][github_bot_api.event.accept_event])."""
 
-    #: The user agent invoking the webhook.
     user_agent: str
+    """The user agent invoking the webhook."""
 
-    #: The event payload.
     payload: t.Dict[str, t.Any]
+    """The event payload."""
 
 
 def accept_event(
     headers: t.Mapping[str, str],
     raw_body: bytes,
     webhook_secret: t.Optional[str] = None,
 ) -> Event:
     """
     Converts thee HTTP *headers* and the *raw_body* to an #Event object.
 
-    # Arguments
-    headers: The HTTP headers. Must have `X-Github-Event`, `X-Github-Delivery`, `User-Agent`, `Content-Type`.
-      May have `X-Hub-Signature` or `X-Hub-Signature-256`.
-    raw_body: The raw request body for the event. This is converted into a JSON payload.
-    webhook_secret: If specified, the `X-Hub-Signature` or `X-Hub-Signature-256` headers are used to verify
-      the signature of the payload. If not specified, the client does not validate the signature.
+    Args:
+        headers: The HTTP headers. Must have `X-Github-Event`, `X-Github-Delivery`, `User-Agent`, `Content-Type`.
+                 May have `X-Hub-Signature` or `X-Hub-Signature-256`.
+        raw_body: The raw request body for the event. This is converted into a JSON payload.
+        webhook_secret: If specified, the `X-Hub-Signature` or `X-Hub-Signature-256` headers are used to verify
+                        the signature of the payload. If not specified, the client does not validate the signature.
     """
 
     event_name = headers.get("X-GitHub-Event")
     delivery_id = headers.get("X-GitHub-Delivery")
     signature_1 = headers.get("X-Hub-Signature")
     signature_256 = headers.get("X-Hub-Signature-256")
     user_agent = headers.get("User-Agent")
     content_type = headers.get("Content-Type")
 
     if not event_name or not delivery_id or not user_agent or not content_type:
         raise InvalidRequest("missing required headers")
-    if webhook_secret is not None and not (signature_1 or signature_256):
+    if webhook_secret is not None and not signature_1 and not signature_256:
         raise InvalidRequest("webhook secret is configured but no signature header was received")
 
     mime_type, parameters = get_mime_components(content_type)
     if mime_type != "application/json":
         raise InvalidRequest(f"expected Content-Type: application/json, got {content_type}")
     encoding = dict(parameters).get("encoding", "UTF-8")
```

### Comparing `github_bot_api-0.5.2/src/github_bot_api/flask.py` & `github_bot_api-0.6.0/src/github_bot_api/flask.py`

 * *Files identical despite different names*

### Comparing `github_bot_api-0.5.2/src/github_bot_api/signature.py` & `github_bot_api-0.6.0/src/github_bot_api/signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
     # Parmeters
     payload: The payload for which the signature should be computed.
     secret: The secret string that is used in conjunction to generate the signature.
     algo: The hash algorithm to use, must be `sha1` or `sha256`.
     """
 
-    if algo not in ("sha1", "sha256"):
-        raise ValueError(f"algo must be {{sha1, sha256}}, got {algo!r}")
-    return f"{algo}=" + hmac.new(secret, payload, algo).hexdigest()
+    if algo in {"sha1", "sha256"}:
+        return f"{algo}={hmac.new(secret, payload, algo).hexdigest()}"
+    raise ValueError(f"algo must be {{sha1, sha256}}, got {algo!r}")
 
 
 def check_signature(sig: str, payload: bytes, secret: bytes, algo: str = "sha256") -> None:
     """
     Compares the provided signature *sig* with the computed signature of the *payload* and
     raises a #SignatureMismatchException if they do not match. This function uses constant-time
     string comparison to prevent timing analysis.
```

### Comparing `github_bot_api-0.5.2/src/github_bot_api/token.py` & `github_bot_api-0.6.0/src/github_bot_api/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     # Returns
     The JWT as a #TokenInfo object.
     """
 
     now = int(time.time())
     exp = now + expires_in
-    payload = {"iss": int(app_id), "iat": now, "exp": exp}
+    payload = {"iss": app_id, "iat": now, "exp": exp}
     token = jwt.encode(payload, private_key, algorithm="RS256")
     return TokenInfo(exp, "Bearer", token)
 
 
 class RefreshableTokenSupplier(Supplier[TokenInfo], metaclass=abc.ABCMeta):
     """
     Base class for token suppliers.
```

### Comparing `github_bot_api-0.5.2/src/github_bot_api/utils/mime.py` & `github_bot_api-0.6.0/src/github_bot_api/utils/mime.py`

 * *Files identical despite different names*

### Comparing `github_bot_api-0.5.2/src/github_bot_api/webhook.py` & `github_bot_api-0.6.0/src/github_bot_api/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,13 +63,10 @@
         matched = False
 
         for handler in self.handlers:
             if fnmatch.fnmatch(event.name, handler.event):
                 matched = True
                 if handler.func(event):
                     return True
-        else:
-            logger.info(
-                f'Event %r (id: %r) goes {"unhandled" if matched else "unmatched"}.', event.name, event.delivery_id
-            )
+        logger.info(f'Event %r (id: %r) goes {"unhandled" if matched else "unmatched"}.', event.name, event.delivery_id)
 
         return matched
```


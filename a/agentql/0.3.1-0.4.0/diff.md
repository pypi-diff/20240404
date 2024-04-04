# Comparing `tmp/agentql-0.3.1.tar.gz` & `tmp/agentql-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.3.1.tar", max compression
+gzip compressed data, was "agentql-0.4.0.tar", max compression
```

## Comparing `agentql-0.3.1.tar` & `agentql-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2024-04-03 04:03:14.917107 agentql-0.3.1/LICENSE
--rw-r--r--   0        0        0      111 2024-04-03 04:03:14.917107 agentql-0.3.1/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-04-03 04:03:15.005108 agentql-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/__init__.py
--rw-r--r--   0        0        0      183 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/core.py
--rw-r--r--   0        0        0     1605 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/popup.py
--rw-r--r--   0        0        0     5520 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/response_proxy.py
--rw-r--r--   0        0        0    10846 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/session.py
--rw-r--r--   0        0        0      301 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/__init__.py
--rw-r--r--   0        0        0     3813 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/network_monitor.py
--rw-r--r--   0        0        0    26961 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/playwright_driver.py
--rw-r--r--   0        0        0     5806 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/web_driver.py
--rw-r--r--   0        0        0        0 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/__init__.py
--rw-r--r--   0        0        0       78 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/api_constants.py
--rw-r--r--   0        0        0      247 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/aria_constants.py
--rw-r--r--   0        0        0      193 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/driver_constants.py
--rw-r--r--   0        0        0      367 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/driver_settings.py
--rw-r--r--   0        0        0     4741 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/errors.py
--rw-r--r--   0        0        0     1980 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/html_constants.py
--rw-r--r--   0        0        0        0 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     5986 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/character_utils.py
--rw-r--r--   0        0        0     5011 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/node.py
--rw-r--r--   0        0        0     4695 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/source.py
--rw-r--r--   0        0        0     1602 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/token.py
--rw-r--r--   0        0        0      213 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/token_kind.py
--rw-r--r--   0        0        0      192 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/utils.py
--rw-r--r--   0        0        0      183 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     1759 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/core.py
--rw-r--r--   0        0        0     1525 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/popup.py
--rw-r--r--   0        0        0     4976 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/response_proxy.py
--rw-r--r--   0        0        0    10597 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/session.py
--rw-r--r--   0        0        0      301 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/__init__.py
--rw-r--r--   0        0        0    26810 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/playwright_driver.py
--rw-r--r--   0        0        0     4922 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/web_driver.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 00:16:44.754820 agentql-0.4.0/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-04 00:16:44.754820 agentql-0.4.0/PACKAGE_README.md
+-rw-r--r--   0        0        0      771 2024-04-04 00:16:44.842820 agentql-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     4741 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     5986 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      145 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     4997 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     2431 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     4686 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      213 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      468 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0      204 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     1853 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     1605 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     5460 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0    10787 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     5331 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      290 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     3813 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    26759 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    26608 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     1813 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1525 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     4917 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0    10540 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     4770 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.0/PKG-INFO
```

### Comparing `agentql-0.3.1/LICENSE` & `agentql-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/pyproject.toml` & `agentql-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.3.1"
+version = "0.4.0"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.3.1/src/agentql/async_api/core.py` & `agentql-0.4.0/src/agentql/sync_api/_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 This module is an entrypoint to AgentQL service
 """
 
 import logging
 from typing import Any
 
-from agentql.async_api.web import InteractiveItemTypeT, PageTypeT, PlaywrightWebDriver, WebDriver
+from agentql.ext.playwright import PlaywrightWebDriverSync as PlaywrightWebDriver
 
-from .session import Session
+from ._session import Session
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
 
-async def start_async_session(
+def start_session(
     url: str = "",
     *,
     web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightWebDriver(),
     user_auth_session: Any = None,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
-    """Start a new asynchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
+    """Start a new synchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
     web_driver (webDriver) (optional): Web driver is responsible for interacting with the browser and page. Defaults to Playwright web driver, which is built on top of the [Playwright framework](https://playwright.dev/python/).
     user_auth_session (dict) (optional): The user authentication session that contains previous login session. Users could retrieve authentication session by starting a session, logging into desired website, and calling `session.get_user_auth_session()`, which will return a `auth_session` object defined in web driver.
 
     Returns:
     -------
-    Session: An instance of AgentQL Session class for asynchronous environment.
+    Session: An instance of AgentQL Session class for synchronous environment.
     """
-    log.debug(f"Starting asynchronous session with {url}")
+    log.debug(f"Starting session with {url}")
 
-    await web_driver.start_browser(user_auth_session=user_auth_session)
+    web_driver.start_browser(user_auth_session=user_auth_session)
     if url:
-        await web_driver.open_url(url)
+        web_driver.open_url(url)
     session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
     return session
```

### Comparing `agentql-0.3.1/src/agentql/async_api/popup.py` & `agentql-0.4.0/src/agentql/async_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/async_api/response_proxy.py` & `agentql-0.4.0/src/agentql/async_api/_response_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import json
 import logging
 from typing import Generic, Union
 
-from agentql.async_api.web import InteractiveItemTypeT, WebDriver
-from agentql.common.errors import AttributeNotFoundError
-from agentql.common.syntax.node import ContainerListNode, ContainerNode, IdListNode, IdNode
+from agentql import AttributeNotFoundError, ContainerListNode, ContainerNode, IdListNode, IdNode
+
+from ._web_driver import InteractiveItemTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 
 class AQLResponseProxy(Generic[InteractiveItemTypeT]):
     """
     AQLResponseProxy class acts as a dynamic proxy to the response received from AgentQL server. It allows users to interact with resulting web elements and to retrieve their text contents. This class is designed to work with the web driver to fetch and process query results.
```

### Comparing `agentql-0.3.1/src/agentql/async_api/session.py` & `agentql-0.4.0/src/agentql/async_api/_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import copy
 import logging
 import os
 from typing import Callable, Generic, List, Literal, Optional
 
 import httpx
 
-from agentql.async_api.popup import Popup
-from agentql.async_api.web import InteractiveItemTypeT, PageTypeT, WebDriver
-from agentql.common.api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
-from agentql.common.errors import (
+from agentql import (
     AgentQLServerError,
     AgentQLServerTimeoutError,
     APIKeyError,
     AttributeNotFoundError,
+    QueryParser,
     UnableToClosePopupError,
 )
-from agentql.common.syntax.parser import Parser
+from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
 
-from .response_proxy import AQLResponseProxy
+from ._popup import Popup
+from ._response_proxy import AQLResponseProxy
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
 AGENTQL_API_KEY = os.getenv("AGENTQL_API_KEY")
 
 
@@ -97,15 +97,15 @@
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         log.debug(f"querying {query}")
 
         self._last_query = query
-        parser = Parser(query)
+        parser = QueryParser(query)
         query_tree = parser.parse()
 
         await self._web_driver.wait_for_page_ready_state(
             wait_for_network_idle=wait_for_network_idle
         )
 
         accessibility_tree = await self._web_driver.prepare_accessibility_tree(
@@ -262,15 +262,15 @@
         query = """
             {
                 popup {
                     close_btn
                 }
             }
         """
-        parser = Parser(query)
+        parser = QueryParser(query)
         query_tree = parser.parse()
         try:
             response = await self._query(query, tree, 500)
             agentql_response = AQLResponseProxy[InteractiveItemTypeT](
                 response, self._web_driver, query_tree
             )
             await agentql_response.popup.close_btn.click()
```

### Comparing `agentql-0.3.1/src/agentql/async_api/web/network_monitor.py` & `agentql-0.4.0/src/agentql/ext/playwright/_network_monitor.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/async_api/web/playwright_driver.py` & `agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import asyncio
 import time
 from typing import Optional, Union
 
 from playwright.async_api import Error, Frame, Locator, Page, StorageState, async_playwright
 from playwright_stealth import StealthConfig, stealth_async
 
-from agentql.async_api.web.network_monitor import PageActivityMonitor
-from agentql.async_api.web.web_driver import WebDriver
-from agentql.common.driver_constants import RENDERER, USER_AGENT, VENDOR
-from agentql.common.driver_settings import ProxySettings, ScrollDirection, StealthModeConfig
-from agentql.common.errors import (
+from agentql._core._errors import (
     AccessibilityTreeError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
 )
-from agentql.common.html_constants import HTML_ROLE_MAPPING
-from agentql.common.js_snippets.snippet_loader import load_js
-from agentql.common.utils import ensure_url_scheme
-
-from .web_driver import WebDriver
+from agentql._core._js_snippets.snippet_loader import load_js
+from agentql._core._utils import ensure_url_scheme
+from agentql.async_api import ScrollDirection, WebDriver
+
+from ._driver_constants import RENDERER, USER_AGENT, VENDOR
+from ._driver_settings import ProxySettings, StealthModeConfig
+from ._html_constants import HTML_ROLE_MAPPING
+from ._network_monitor import PageActivityMonitor
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
     """
     PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
     """
 
-    def __init__(self, headless=True, proxy: ProxySettings = None) -> None:
+    def __init__(self, headless=False, proxy: ProxySettings = None) -> None:
         """
         Construct the PlaywrightWebDriver instance.
 
         Parameters:
         -----------
         headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
         proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
@@ -309,15 +308,15 @@
         await self._remove_page_event_listeners()
 
     async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         await self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
```

### Comparing `agentql-0.3.1/src/agentql/async_api/web/web_driver.py` & `agentql-0.4.0/src/agentql/async_api/_web_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-from typing import Any, TypeVar
+from enum import Enum
+from typing import Any
 
 from typing_extensions import Protocol
 
-from agentql.common.driver_settings import ScrollDirection
+from agentql import InteractiveItemTypeT, PageTypeT
 
-InteractiveItemTypeT = TypeVar("InteractiveItemTypeT")
-"""
-A type variable representing the type of interactive items in a web driver session.
-Used in type hints where the exact type depends on the specific web driver library used.
-"""
-
-PageTypeT = TypeVar("PageTypeT")
-"""
-A type variable representing the type of a page in a web driver session.
-Used in type hints where the exact type depends on the specific web driver library used.
-"""
+
+class ScrollDirection(Enum):
+    UP = 1
+    DOWN = 2
 
 
 class WebDriver(Protocol[InteractiveItemTypeT, PageTypeT]):
     """
     The WebDriver protocol is a part of the AgentQL SDK, designed to facilitate custom web driver implementations. This protocol outlines the necessary interface for a web driver compatible with AgentQL, enabling interaction with web elements, page navigation, and accessibility tree manipulation.
     """
 
@@ -121,15 +115,15 @@
         """
 
     async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
 
     async def scroll_to_bottom(self):
         """Scrolls to the bottom of the current page."""
 
     async def scroll_to_top(self):
```

### Comparing `agentql-0.3.1/src/agentql/common/errors.py` & `agentql-0.4.0/src/agentql/_core/_errors.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/html_constants.py` & `agentql-0.4.0/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/js_snippets/generate_accessibility_tree.js` & `agentql-0.4.0/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/js_snippets/set_iframe_path.js` & `agentql-0.4.0/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/syntax/character_utils.py` & `agentql-0.4.0/src/agentql/_core/_syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/syntax/lexer.py` & `agentql-0.4.0/src/agentql/_core/_syntax/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agentql.common.errors import QuerySyntaxError
+from agentql import QuerySyntaxError
 
 from .character_utils import is_identifier_continue, is_identifier_start
 from .source import Source
 from .token import Token
 from .token_kind import TokenKind
 
 IGNORED_TOKENS = [TokenKind.NEWLINE]
```

### Comparing `agentql-0.3.1/src/agentql/common/syntax/node.py` & `agentql-0.4.0/src/agentql/_core/_syntax/node.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/syntax/parser.py` & `agentql-0.4.0/src/agentql/_core/_syntax/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Union
 
-from agentql.common.errors import QuerySyntaxError
+from agentql import QuerySyntaxError
 
 from .lexer import Lexer
 from .node import ContainerListNode, ContainerNode, IdListNode, IdNode, Node
 from .source import Source
 from .token import Token
 from .token_kind import TokenKind
 
 
-class Parser:
+class QueryParser:
     """A parser for AgentQL queries. It is a recursive descent parser, which is a top-down parser that
     uses a set of recursive procedures to process the input."""
 
     def __init__(self, source: Union[Source, str]) -> None:
         """Initialize the parser.
 
         Parameters:
```

### Comparing `agentql-0.3.1/src/agentql/common/syntax/source.py` & `agentql-0.4.0/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/common/syntax/token.py` & `agentql-0.4.0/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/sync_api/core.py` & `agentql-0.4.0/src/agentql/async_api/_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 This module is an entrypoint to AgentQL service
 """
 
 import logging
 from typing import Any
 
-from agentql.sync_api.web import InteractiveItemTypeT, PageTypeT, PlaywrightWebDriver, WebDriver
+from agentql.ext.playwright import PlaywrightWebDriverAsync as PlaywrightWebDriver
 
-from .session import Session
+from ._session import Session
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
 
-def start_session(
+async def start_async_session(
     url: str = "",
     *,
     web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightWebDriver(),
     user_auth_session: Any = None,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
-    """Start a new synchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
+    """Start a new asynchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
     web_driver (webDriver) (optional): Web driver is responsible for interacting with the browser and page. Defaults to Playwright web driver, which is built on top of the [Playwright framework](https://playwright.dev/python/).
     user_auth_session (dict) (optional): The user authentication session that contains previous login session. Users could retrieve authentication session by starting a session, logging into desired website, and calling `session.get_user_auth_session()`, which will return a `auth_session` object defined in web driver.
 
     Returns:
     -------
-    Session: An instance of AgentQL Session class for synchronous environment.
+    Session: An instance of AgentQL Session class for asynchronous environment.
     """
-    log.debug(f"Starting session with {url}")
+    log.debug(f"Starting asynchronous session with {url}")
 
-    web_driver.start_browser(user_auth_session=user_auth_session)
+    await web_driver.start_browser(user_auth_session=user_auth_session)
     if url:
-        web_driver.open_url(url)
+        await web_driver.open_url(url)
     session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
     return session
```

### Comparing `agentql-0.3.1/src/agentql/sync_api/popup.py` & `agentql-0.4.0/src/agentql/sync_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.1/src/agentql/sync_api/response_proxy.py` & `agentql-0.4.0/src/agentql/sync_api/_response_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from typing import Generic, Union
 
-from agentql.common.errors import AttributeNotFoundError
-from agentql.common.syntax.node import ContainerListNode, ContainerNode, IdListNode, IdNode
-from agentql.sync_api.web import InteractiveItemTypeT, WebDriver
+from agentql import AttributeNotFoundError, ContainerListNode, ContainerNode, IdListNode, IdNode
+
+from ._web_driver import InteractiveItemTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
 
 class AQLResponseProxy(Generic[InteractiveItemTypeT]):
     """
     AQLResponseProxy class acts as a dynamic proxy to the response received from AgentQL server. It allows users to interact with resulting web elements and to retrieve their text contents. This class is designed to work with the web driver to fetch and process query results.
```

### Comparing `agentql-0.3.1/src/agentql/sync_api/session.py` & `agentql-0.4.0/src/agentql/sync_api/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import json
 import logging
 import os
 from typing import Callable, Generic, List, Literal, Optional
 
 import requests
 
-from agentql.common.api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
-from agentql.common.errors import (
+from agentql import (
     AgentQLServerError,
     AgentQLServerTimeoutError,
     APIKeyError,
     AttributeNotFoundError,
+    QueryParser,
     UnableToClosePopupError,
 )
-from agentql.common.syntax.parser import Parser
-from agentql.sync_api.popup import Popup
-from agentql.sync_api.web import InteractiveItemTypeT, PageTypeT, WebDriver
+from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
 
-from .response_proxy import AQLResponseProxy
+from ._popup import Popup
+from ._response_proxy import AQLResponseProxy
+from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
 
 
 class Session(Generic[InteractiveItemTypeT, PageTypeT]):
@@ -106,15 +106,15 @@
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         log.debug(f"querying {query}")
 
         self._last_query = query
-        parser = Parser(query)
+        parser = QueryParser(query)
         query_tree = parser.parse()
 
         self._web_driver.wait_for_page_ready_state(wait_for_network_idle)
 
         accessibility_tree = self._web_driver.prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
@@ -257,15 +257,15 @@
         query = """
             {
                 popup {
                     close_btn
                 }
             }
         """
-        parser = Parser(query)
+        parser = QueryParser(query)
         query_tree = parser.parse()
         try:
             response = self._query(query, tree, 500)
             agentql_response = AQLResponseProxy[InteractiveItemTypeT](
                 response, self._web_driver, query_tree
             )
             agentql_response.popup.close_btn.click()
```

### Comparing `agentql-0.3.1/src/agentql/sync_api/web/playwright_driver.py` & `agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import time
 from typing import Optional, Union
 
 from playwright.sync_api import Error, Frame, Locator, Page, StorageState, sync_playwright
 from playwright_stealth import StealthConfig, stealth_sync
 
-from agentql.async_api.web.network_monitor import PageActivityMonitor
-from agentql.common.driver_constants import RENDERER, USER_AGENT, VENDOR
-from agentql.common.driver_settings import ProxySettings, ScrollDirection, StealthModeConfig
-from agentql.common.errors import (
+from agentql._core._errors import (
     AccessibilityTreeError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
 )
-from agentql.common.html_constants import HTML_ROLE_MAPPING
-from agentql.common.js_snippets.snippet_loader import load_js
-from agentql.common.utils import ensure_url_scheme
-from agentql.sync_api.web.web_driver import WebDriver
-
-from .web_driver import WebDriver
+from agentql._core._js_snippets.snippet_loader import load_js
+from agentql._core._utils import ensure_url_scheme
+from agentql.sync_api import ScrollDirection, WebDriver
+
+from ._driver_constants import RENDERER, USER_AGENT, VENDOR
+from ._driver_settings import ProxySettings, StealthModeConfig
+from ._html_constants import HTML_ROLE_MAPPING
+from ._network_monitor import PageActivityMonitor
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
     """
     PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
     """
 
-    def __init__(self, headless=True, proxy: ProxySettings = None) -> None:
+    def __init__(self, headless=False, proxy: ProxySettings = None) -> None:
         """
         Construct the PlaywrightWebDriver instance.
 
         Parameters:
         -----------
         headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
         proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
@@ -336,15 +335,15 @@
         self._remove_page_event_listeners()
 
     def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
```

### Comparing `agentql-0.3.1/src/agentql/sync_api/web/web_driver.py` & `agentql-0.4.0/src/agentql/sync_api/_web_driver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 
 from typing_extensions import Protocol
 
-from agentql.async_api.web.web_driver import InteractiveItemTypeT, PageTypeT
-from agentql.common.driver_settings import ScrollDirection
+from agentql.async_api import InteractiveItemTypeT, PageTypeT, ScrollDirection
 
 
 class WebDriver(Protocol[InteractiveItemTypeT, PageTypeT]):
     def locate_interactive_element(self, response_data: dict) -> InteractiveItemTypeT:
         """
         Locates an interactive element in the web page.
 
@@ -107,15 +106,15 @@
         """
 
     def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
-        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
 
     def scroll_to_bottom(self):
         """Scrolls to the bottom of the current page."""
 
     def scroll_to_top(self):
```

### Comparing `agentql-0.3.1/PKG-INFO` & `agentql-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.3.1
+Version: 0.4.0
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


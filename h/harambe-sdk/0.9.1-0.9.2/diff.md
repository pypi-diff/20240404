# Comparing `tmp/harambe_sdk-0.9.1.tar.gz` & `tmp/harambe_sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harambe_sdk-0.9.1.tar", max compression
+gzip compressed data, was "harambe_sdk-0.9.2.tar", max compression
```

## Comparing `harambe_sdk-0.9.1.tar` & `harambe_sdk-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     5215 2024-02-13 20:36:52.623924 harambe_sdk-0.9.1/README.md
--rw-r--r--   0        0        0      278 2024-03-20 19:15:38.076398 harambe_sdk-0.9.1/harambe/__init__.py
--rw-r--r--   0        0        0    13067 2024-03-21 22:42:20.666399 harambe_sdk-0.9.1/harambe/core.py
--rw-r--r--   0        0        0     2397 2024-03-01 06:10:42.180072 harambe_sdk-0.9.1/harambe/handlers.py
--rw-r--r--   0        0        0     3038 2024-02-13 21:36:24.521887 harambe_sdk-0.9.1/harambe/meta.py
--rw-r--r--   0        0        0     2457 2024-03-20 19:15:38.077026 harambe_sdk-0.9.1/harambe/normalize_url.py
--rw-r--r--   0        0        0     4647 2024-03-22 01:26:52.984095 harambe_sdk-0.9.1/harambe/observer.py
--rw-r--r--   0        0        0        0 2023-11-14 19:41:29.582523 harambe_sdk-0.9.1/harambe/py.typed
--rw-r--r--   0        0        0     3907 2024-02-13 20:42:32.059875 harambe_sdk-0.9.1/harambe/tracker.py
--rw-r--r--   0        0        0      256 2024-02-13 20:43:06.638853 harambe_sdk-0.9.1/harambe/types.py
--rw-r--r--   0        0        0     3049 2024-02-02 23:16:39.870857 harambe_sdk-0.9.1/harambe/utils.py
--rw-r--r--   0        0        0      801 2024-03-22 01:28:19.602097 harambe_sdk-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 harambe_sdk-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     5141 2024-04-04 00:50:22.029190 harambe_sdk-0.9.2/README.md
+-rw-r--r--   0        0        0      278 2024-03-17 22:34:41.210967 harambe_sdk-0.9.2/harambe/__init__.py
+-rw-r--r--   0        0        0    13631 2024-03-29 19:10:57.314846 harambe_sdk-0.9.2/harambe/core.py
+-rw-r--r--   0        0        0     2397 2024-03-01 06:20:44.777193 harambe_sdk-0.9.2/harambe/handlers.py
+-rw-r--r--   0        0        0     3038 2024-03-01 05:38:05.074579 harambe_sdk-0.9.2/harambe/meta.py
+-rw-r--r--   0        0        0     2457 2024-03-17 23:05:42.149184 harambe_sdk-0.9.2/harambe/normalize_url.py
+-rw-r--r--   0        0        0     5014 2024-03-28 23:00:00.635703 harambe_sdk-0.9.2/harambe/observer.py
+-rw-r--r--   0        0        0     2269 2024-03-29 19:10:57.314547 harambe_sdk-0.9.2/harambe/parser/parser.py
+-rw-r--r--   0        0        0        0 2023-11-16 20:05:34.307080 harambe_sdk-0.9.2/harambe/py.typed
+-rw-r--r--   0        0        0     3907 2024-03-01 05:38:05.074901 harambe_sdk-0.9.2/harambe/tracker.py
+-rw-r--r--   0        0        0      256 2024-03-01 05:38:05.075229 harambe_sdk-0.9.2/harambe/types.py
+-rw-r--r--   0        0        0     3049 2024-03-01 05:43:34.226033 harambe_sdk-0.9.2/harambe/utils.py
+-rw-r--r--   0        0        0      835 2024-04-04 00:50:34.319790 harambe_sdk-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 harambe_sdk-0.9.2/PKG-INFO
```

### Comparing `harambe_sdk-0.9.1/README.md` & `harambe_sdk-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 }
 
 
 # Annotation registers the scraper with the SDK
 @SDK.scraper(domain="https://apprhs.org/our-locations/", stage="detail")
 async def scrape(sdk: SDK, url: str, *args: Any, **kwargs: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     locations = await page.locator(SELECTORS["list_view"]).all()
     for location in locations:        
         # Save the data to the database or file
         await sdk.save_data(
             {
                 "name": await Pu.get_text(location, SELECTORS["name"]),
@@ -109,15 +108,14 @@
 
 SELECTORS = {}
 
 
 @SDK.scraper(domain="https://example.org", stage="listing")
 async def scrape(sdk: SDK, url: str, *args: Any, **kwargs: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     for url in [
         "https://example.org/1",
         "https://example.org/2",
         "https://example.org/3",
     ]:  # Imagine these are locators
         await sdk.enqueue(
@@ -130,15 +128,14 @@
             },
         )
 
 
 @SDK.scraper(domain="https://example.org", stage="detail")
 async def scrape_detail(sdk: SDK, url: str, context: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     # Grab all properties from the context
     detail = {**context}
 
     detail["fax"] = "123-456-7890"  # Some data grabbed from the detail page
     detail["type"] = "Hospital"  # Some data grabbed from the detail page
     await sdk.save_data(detail)  # Save the data to the database
@@ -165,8 +162,8 @@
 Before submitting a PR, please run the following commands to ensure
 that your code is formatted correctly.
 
 ```shell
 ./format.sh
 ```
 
-Happy extraction! 🦍
+Happy extraction! 🦍
```

### Comparing `harambe_sdk-0.9.1/harambe/core.py` & `harambe_sdk-0.9.2/harambe/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,44 @@
 from typing import Any, Callable, List, Optional, Protocol, Union, Awaitable
 
 import aiohttp
 from playwright.async_api import (
     Page,
     async_playwright,
     ElementHandle,
+    TimeoutError as PlaywrightTimeoutError,
 )
 from playwright_stealth import stealth_async
 
 from harambe.handlers import (
     ResourceRequestHandler,
     ResourceType,
     UnnecessaryResourceHandler,
 )
 from harambe.normalize_url import normalize_url
 from harambe.observer import (
     LocalStorageObserver,
     LoggingObserver,
     OutputObserver,
     DownloadMeta,
-    StopPaginationObserver,
+    DuplicateHandler,
     ObservationTrigger,
 )
 from harambe.tracker import FileDataTracker
 from harambe.types import URL, AsyncScraperType, Context, ScrapeResult, Stage
 
 
 class AsyncScraper(Protocol):
     """
     Protocol that all classed based scrapers should implement.
     Note that scrapers in harambe should be functions, not classes.
     """
 
-    async def scrape(self, sdk: "SDK", url: URL, context: Context) -> None: ...
+    async def scrape(self, sdk: "SDK", url: URL, context: Context) -> None:
+        ...
 
 
 class SDK:
     """
     All Harambe scrapers should use this SDK to scrape data. It provides
     a number of useful methods for saving data and enqueuing urls to be scraped later.
 
@@ -68,24 +70,29 @@
 
         if not observer:
             observer = [LoggingObserver()]
 
         if not isinstance(observer, list):
             observer = [observer]
 
-        observer.insert(0, StopPaginationObserver())
         self._observers = observer
+        self._deduper = DuplicateHandler()
 
     async def save_data(self, *data: ScrapeResult) -> None:
         """
         Save scraped data. This will be passed to the on_save_data callback.
         Generally, this should only be called on the detail page.
 
         :param data: one or more dicts of details to save
         """
+        if len(data) == 1 and isinstance(data[0], list):
+            raise TypeError(
+                "`SDK.save_data` should be called with one dict at a time, not a list of dicts."
+            )
+
         url = self.page.url
         for d in data:
             d["__url"] = url
             await self._notify_observers("on_save_data", d)
 
     async def enqueue(self, *urls: URL, context: Optional[Context] = None) -> None:
         """
@@ -129,20 +136,23 @@
                 if next_url.startswith("?"):
                     # TODO: merge query params
                     next_url = self.page.url.split("?")[0] + next_url
                     await self.page.goto(next_url)
                     await self.page.wait_for_timeout(timeout)
 
             if next_url:
-                for o in self._observers:
-                    o.on_paginate(self.page.url)
+                await self._notify_observers("on_paginate", next_url)
 
                 await self._scraper(
                     self, next_url, self._context
                 )  # TODO: eventually fix this to not be recursive
+        except PlaywrightTimeoutError as e:
+            raise TimeoutError(
+                f"{e.args[0]} You may increase the timeout by passing `timeout` in ms to `SDK.paginate`. Alternatively, this may mean that the next page element or URL was not found and pagination is complete."
+            ) from e
         except (TimeoutError, StopAsyncIteration):
             return
 
     async def capture_url(
         self, clickable: ElementHandle, resource_type: ResourceType = "document"
     ) -> URL | None:
         """
@@ -211,18 +221,19 @@
         the first observer is the stop pagination observer, so it will always be called separately so that we can stop
         pagination if needed.
         :param method: observation trigger
         :param args: arguments to pass to the method
         :param kwargs: keyword arguments to pass to the method
         :return: the result of the method call
         """
-        await getattr(self._observers[0], method)(*args, **kwargs)
-        return await asyncio.gather(
-            *[getattr(o, method)(*args, **kwargs) for o in self._observers[1:]]
-        )
+        duplicated = await getattr(self._deduper, method)(*args, **kwargs)
+        if not duplicated:
+            return await asyncio.gather(
+                *[getattr(o, method)(*args, **kwargs) for o in self._observers]
+            )
 
     @staticmethod
     async def run(
         scraper: AsyncScraperType,
         url: Optional[str] = None,
         context: Optional[Context] = None,
         headless: bool = False,
```

### Comparing `harambe_sdk-0.9.1/harambe/handlers.py` & `harambe_sdk-0.9.2/harambe/handlers.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.1/harambe/meta.py` & `harambe_sdk-0.9.2/harambe/meta.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.1/harambe/normalize_url.py` & `harambe_sdk-0.9.2/harambe/normalize_url.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.1/harambe/observer.py` & `harambe_sdk-0.9.2/harambe/observer.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 )
 from urllib.parse import quote
 
 from harambe.tracker import FileDataTracker
 from harambe.types import URL, Context, Stage
 
 
-ObservationTrigger = Literal["on_save_data", "on_queue_url", "on_download", "on_paginate"]
+ObservationTrigger = Literal[
+    "on_save_data", "on_queue_url", "on_download", "on_paginate"
+]
 
 
 @runtime_checkable
 class OutputObserver(Protocol):
     @abstractmethod
     async def on_save_data(self, data: Dict[str, Any]):
         raise NotImplementedError()
@@ -33,15 +35,15 @@
     @abstractmethod
     async def on_download(
         self, download_url: str, filename: str, content: bytes
     ) -> "DownloadMeta":
         raise NotImplementedError()
 
     @abstractmethod
-    def on_paginate(self, next_url: str) -> None:
+    async def on_paginate(self, next_url: str) -> None:
         raise NotImplementedError()
 
 
 class LoggingObserver(OutputObserver):
     async def on_save_data(self, data: Dict[str, Any]):
         print(data)
 
@@ -53,15 +55,15 @@
     ) -> "DownloadMeta":
         print(f"Downloading file: {filename}")  # TODO: use logger
         return {
             "url": f"{download_url}/{quote(filename)}",
             "filename": filename,
         }
 
-    def on_paginate(self, next_url: str) -> None:
+    async def on_paginate(self, next_url: str) -> None:
         pass
 
 
 class LocalStorageObserver(OutputObserver):
     def __init__(self, domain: str, stage: Stage):
         self._tracker = FileDataTracker(domain, stage)
 
@@ -77,15 +79,15 @@
         data = {
             "url": f"{download_url}/{quote(filename)}",
             "filename": filename,
         }
         self._tracker.save_data(data)
         return data
 
-    def on_paginate(self, next_url: str) -> None:
+    async def on_paginate(self, next_url: str) -> None:
         pass
 
 
 class InMemoryObserver(OutputObserver):
     def __init__(self):
         self._data: List[Dict[str, Any]] = []
         self._urls: List[Tuple[URL, Context]] = []
@@ -103,15 +105,15 @@
         data = {
             "url": f"{download_url}/{quote(filename)}",
             "filename": filename,
         }
         self._files.append((filename, content))
         return data
 
-    def on_paginate(self, next_url: str) -> None:
+    async def on_paginate(self, next_url: str) -> None:
         pass
 
     @property
     def data(self) -> List[Dict[str, Any]]:
         return self._data
 
     @property
@@ -119,47 +121,56 @@
         return self._urls
 
     @property
     def files(self) -> List[Tuple[str, bytes]]:
         return self._files
 
 
-class StopPaginationObserver(OutputObserver):
+class DuplicateHandler:
     def __init__(self):
         self._saved_data: set[bytes] = set()
-        self._paginator_called = False
+        self.rows_on_page = 0
+        self.previously_saved_rows_on_page = 0
 
-    async def on_save_data(self, data: dict[str, Any]):
-        self._add_data(data)
+    async def on_save_data(self, data: dict[str, Any]) -> bool:
+        return self._add_data(data)
 
-    async def on_queue_url(self, url: URL, context: dict[str, Any]) -> None:
-        self._add_data(url)
+    async def on_queue_url(self, url: URL, context: dict[str, Any]) -> bool:
+        return self._add_data(url)
 
     # noinspection PyTypeChecker
     async def on_download(
         self, download_url: str, filename: str, content: bytes
-    ) -> "DownloadMeta":
-        self._add_data((download_url, filename))
+    ) -> bool:
+        return self._add_data((download_url, filename))
 
-    def on_paginate(self, next_url: str) -> None:
-        self._paginator_called = True
+    async def on_paginate(self, next_url: str) -> bool:
+        if self.rows_on_page == self.previously_saved_rows_on_page:
+            raise StopAsyncIteration()
 
-    def _add_data(self, data: Any):
-        hash_value = self.compute_hash(data)
+        self.rows_on_page = 0
+        self.previously_saved_rows_on_page = 0
+        return False
 
-        if self._paginator_called and hash_value in self._saved_data:
-            raise StopAsyncIteration()
+    def _add_data(self, data: Any) -> bool:
+        self.rows_on_page += 1
 
-        self._saved_data.add(hash_value)
+        hash_value = self.compute_hash(data)
+        if hash_value in self._saved_data:
+            self.previously_saved_rows_on_page += 1
+            return True  # return True if data is duplicated
+        else:
+            self._saved_data.add(hash_value)
+            return False
 
     @staticmethod
     def compute_hash(data: Any) -> bytes:
         if isinstance(data, dict):
             data = {k: v for k, v in data.items() if not k.startswith("__")}
 
-        data_str = json.dumps(data, separators=(',', ':'), sort_keys=True)
+        data_str = json.dumps(data, separators=(",", ":"), sort_keys=True)
         return hashlib.md5(data_str.encode()).digest()
 
 
 class DownloadMeta(TypedDict):
     url: str
     filename: str
```

### Comparing `harambe_sdk-0.9.1/harambe/tracker.py` & `harambe_sdk-0.9.2/harambe/tracker.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.1/harambe/utils.py` & `harambe_sdk-0.9.2/harambe/utils.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.1/pyproject.toml` & `harambe_sdk-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "harambe-sdk"
-version = "0.9.1"
+version = "0.9.2"
 description = "Data extraction SDK for Playwright 🐒🍌"
 authors = ["awtkns <hello@awtkns.com>"]
 readme = "README.md"
 packages = [
     { include = "harambe", from = "." },
 ]
 
 
 [tool.poetry.dependencies]
+pydantic = { version = "^2.6.4" }
 python = "^3.11"
 playwright = "^1.39.0"
 setuptools = "^69.0.2"
 beautifulsoup4 = "^4.12.2"
 requests = "^2.31.0"
 playwright-stealth = "^1.0.6" # TODO: self host this package
 aiohttp = "^3.9.3"
```

### Comparing `harambe_sdk-0.9.1/PKG-INFO` & `harambe_sdk-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: harambe-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Data extraction SDK for Playwright 🐒🍌
 Author: awtkns
 Author-email: hello@awtkns.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: playwright (>=1.39.0,<2.0.0)
 Requires-Dist: playwright-stealth (>=1.0.6,<2.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="./.github/assets/banner.png" height="200" alt="Tarsier Monkey" />
 </p>
@@ -88,15 +89,14 @@
 }
 
 
 # Annotation registers the scraper with the SDK
 @SDK.scraper(domain="https://apprhs.org/our-locations/", stage="detail")
 async def scrape(sdk: SDK, url: str, *args: Any, **kwargs: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     locations = await page.locator(SELECTORS["list_view"]).all()
     for location in locations:        
         # Save the data to the database or file
         await sdk.save_data(
             {
                 "name": await Pu.get_text(location, SELECTORS["name"]),
@@ -127,15 +127,14 @@
 
 SELECTORS = {}
 
 
 @SDK.scraper(domain="https://example.org", stage="listing")
 async def scrape(sdk: SDK, url: str, *args: Any, **kwargs: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     for url in [
         "https://example.org/1",
         "https://example.org/2",
         "https://example.org/3",
     ]:  # Imagine these are locators
         await sdk.enqueue(
@@ -148,15 +147,14 @@
             },
         )
 
 
 @SDK.scraper(domain="https://example.org", stage="detail")
 async def scrape_detail(sdk: SDK, url: str, context: Any) -> None:
     page: Page = sdk.page
-    await page.goto(url)
 
     # Grab all properties from the context
     detail = {**context}
 
     detail["fax"] = "123-456-7890"  # Some data grabbed from the detail page
     detail["type"] = "Hospital"  # Some data grabbed from the detail page
     await sdk.save_data(detail)  # Save the data to the database
@@ -184,7 +182,8 @@
 that your code is formatted correctly.
 
 ```shell
 ./format.sh
 ```
 
 Happy extraction! 🦍
+
```


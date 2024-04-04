# Comparing `tmp/w-render-0.2.2.tar.gz` & `tmp/w-render-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w-render-0.2.2.tar", last modified: Sun Sep  3 20:30:59 2023, max compression
+gzip compressed data, was "w-render-0.2.3.tar", last modified: Thu Apr  4 21:00:23 2024, max compression
```

## Comparing `w-render-0.2.2.tar` & `w-render-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/
--rw-rw-r--   0 repente   (1000) repente   (1000)      823 2023-09-03 20:30:59.919899 w-render-0.2.2/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      605 2023-08-31 19:42:54.000000 w-render-0.2.2/README.md
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2023-09-03 20:30:59.919899 w-render-0.2.2/setup.cfg
--rw-rw-r--   0 repente   (1000) repente   (1000)     3227 2023-09-03 20:30:28.000000 w-render-0.2.2/setup.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.915899 w-render-0.2.2/w_render.egg-info/
--rw-rw-r--   0 repente   (1000) repente   (1000)      823 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      763 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/SOURCES.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        1 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/dependency_links.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)      158 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/entry_points.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       80 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/requires.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       11 2023-09-03 20:30:59.000000 w-render-0.2.2/w_render.egg-info/top_level.txt
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.915899 w-render-0.2.2/web_render/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/base/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w-render-0.2.2/web_render/base/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2337 2023-09-03 20:30:16.000000 w-render-0.2.2/web_render/base/__main__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     8213 2023-09-01 20:23:35.000000 w-render-0.2.2/web_render/base/abstract.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1125 2023-08-24 07:40:40.000000 w-render-0.2.2/web_render/base/client.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     4320 2023-08-24 21:59:25.000000 w-render-0.2.2/web_render/base/server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     3666 2023-08-28 08:54:18.000000 w-render-0.2.2/web_render/base/test_webrender.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1508 2023-08-24 07:24:47.000000 w-render-0.2.2/web_render/config.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/flask/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-07-28 09:55:28.000000 w-render-0.2.2/web_render/flask/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1817 2023-08-28 08:31:02.000000 w-render-0.2.2/web_render/flask/__main__.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/flask/core/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/flask/core/main/
--rw-rw-r--   0 repente   (1000) repente   (1000)      837 2023-08-24 07:40:41.000000 w-render-0.2.2/web_render/flask/core/main/view.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/flask/core/render_api/
--rw-rw-r--   0 repente   (1000) repente   (1000)     1372 2023-08-24 07:40:41.000000 w-render-0.2.2/web_render/flask/core/render_api/logic.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1075 2023-08-24 07:24:47.000000 w-render-0.2.2/web_render/flask/core/render_api/view.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      207 2023-08-24 07:24:47.000000 w-render-0.2.2/web_render/flask/core/routing.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/flask/core/service/
--rw-rw-r--   0 repente   (1000) repente   (1000)      389 2023-08-24 07:24:47.000000 w-render-0.2.2/web_render/flask/core/service/interface.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      377 2023-08-24 07:24:47.000000 w-render-0.2.2/web_render/interface.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-09-03 20:30:59.919899 w-render-0.2.2/web_render/script/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:28:05.000000 w-render-0.2.2/web_render/script/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1507 2023-08-24 08:38:56.000000 w-render-0.2.2/web_render/script/render_server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1498 2023-08-24 12:59:54.000000 w-render-0.2.2/web_render/tool.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.887713 w-render-0.2.3/
+-rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-04 21:00:23.887713 w-render-0.2.3/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      605 2023-08-31 19:42:54.000000 w-render-0.2.3/README.md
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2024-04-04 21:00:23.887713 w-render-0.2.3/setup.cfg
+-rw-rw-r--   0 repente   (1000) repente   (1000)     3227 2024-04-04 20:59:29.000000 w-render-0.2.3/setup.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.887713 w-render-0.2.3/w_render.egg-info/
+-rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      763 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/SOURCES.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        1 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/dependency_links.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)      158 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/entry_points.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       80 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/requires.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       11 2024-04-04 21:00:23.000000 w-render-0.2.3/w_render.egg-info/top_level.txt
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.803715 w-render-0.2.3/web_render/
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.827715 w-render-0.2.3/web_render/base/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w-render-0.2.3/web_render/base/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2337 2023-09-03 20:30:16.000000 w-render-0.2.3/web_render/base/__main__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     8366 2024-04-04 20:59:13.000000 w-render-0.2.3/web_render/base/abstract.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1125 2023-08-24 07:40:40.000000 w-render-0.2.3/web_render/base/client.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     4320 2023-08-24 21:59:25.000000 w-render-0.2.3/web_render/base/server.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     3666 2023-08-28 08:54:18.000000 w-render-0.2.3/web_render/base/test_webrender.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1508 2023-08-24 07:24:47.000000 w-render-0.2.3/web_render/config.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.835714 w-render-0.2.3/web_render/flask/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-07-28 09:55:28.000000 w-render-0.2.3/web_render/flask/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1817 2023-08-28 08:31:02.000000 w-render-0.2.3/web_render/flask/__main__.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.847714 w-render-0.2.3/web_render/flask/core/
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.847714 w-render-0.2.3/web_render/flask/core/main/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      837 2023-08-24 07:40:41.000000 w-render-0.2.3/web_render/flask/core/main/view.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.871713 w-render-0.2.3/web_render/flask/core/render_api/
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1372 2023-08-24 07:40:41.000000 w-render-0.2.3/web_render/flask/core/render_api/logic.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1075 2023-08-24 07:24:47.000000 w-render-0.2.3/web_render/flask/core/render_api/view.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      207 2023-08-24 07:24:47.000000 w-render-0.2.3/web_render/flask/core/routing.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.887713 w-render-0.2.3/web_render/flask/core/service/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      389 2023-08-24 07:24:47.000000 w-render-0.2.3/web_render/flask/core/service/interface.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      377 2023-08-24 07:24:47.000000 w-render-0.2.3/web_render/interface.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-04 21:00:23.887713 w-render-0.2.3/web_render/script/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:28:05.000000 w-render-0.2.3/web_render/script/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1507 2023-08-24 08:38:56.000000 w-render-0.2.3/web_render/script/render_server.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1498 2023-08-24 12:59:54.000000 w-render-0.2.3/web_render/tool.py
```

### Comparing `w-render-0.2.2/PKG-INFO` & `w-render-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: w-render
-Version: 0.2.2
+Version: 0.2.3
 Summary: Render a dynamical sites.
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: flask
+Requires-Dist: webdriver-manager
+Requires-Dist: waitress
+Requires-Dist: undetected-chromedriver
+Requires-Dist: python-dotenv
 
 ### Description
 
 Web-render is a method of rendering dynamic web pages using Selenium.
 
 ### Commands
```

### Comparing `w-render-0.2.2/README.md` & `w-render-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/setup.py` & `w-render-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     long_description = fh.read()
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setup(
     # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
     name="w-render",
     # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-    version="0.2.2",
+    version="0.2.3",
     # Имя автора.
     author="Andrey Plugin",
     # Его почта.
     author_email="9keepa@gmail.com",
     # Краткое описание, которое будет показано на странице PyPi.
     description="Render a dynamical sites.",
     # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
```

### Comparing `w-render-0.2.2/w_render.egg-info/PKG-INFO` & `w-render-0.2.3/w_render.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: w-render
-Version: 0.2.2
+Version: 0.2.3
 Summary: Render a dynamical sites.
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: flask
+Requires-Dist: webdriver-manager
+Requires-Dist: waitress
+Requires-Dist: undetected-chromedriver
+Requires-Dist: python-dotenv
 
 ### Description
 
 Web-render is a method of rendering dynamic web pages using Selenium.
 
 ### Commands
```

### Comparing `w-render-0.2.2/w_render.egg-info/SOURCES.txt` & `w-render-0.2.3/w_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/base/__main__.py` & `w-render-0.2.3/web_render/base/__main__.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/base/abstract.py` & `w-render-0.2.3/web_render/base/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,17 @@
     if config.get('HEADLESS'):
         co.add_argument('--headless=new')
 
     co.add_argument('--disable-blink-features=AutomationControlled')
     co.add_argument('--no-sandbox')
     co.add_argument('--disable-dev-shm-usage')
     co.add_argument("start-maximized")
+    if config.get("LANGUAGE"):
+        # example en,en_US
+        co.add_experimental_option('prefs', {'intl.accept_languages': config.get("LANGUAGE")})
     if config.get('INCOGNITO'):
         co.add_argument("--incognito")
     if config.get('USER_DATA_DIR'):
         co.add_argument(f"user-data-dir={config.get('USER_DATA_DIR')}")
     co.add_experimental_option("excludeSwitches", ["ignore-certificate-errors"])
     co.add_experimental_option("excludeSwitches", ["enable-automation"])
     co.add_experimental_option('useAutomationExtension', False)
```

### Comparing `w-render-0.2.2/web_render/base/client.py` & `w-render-0.2.3/web_render/base/client.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/base/server.py` & `w-render-0.2.3/web_render/base/server.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/base/test_webrender.py` & `w-render-0.2.3/web_render/base/test_webrender.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/config.py` & `w-render-0.2.3/web_render/config.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/flask/__main__.py` & `w-render-0.2.3/web_render/flask/__main__.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/flask/core/main/view.py` & `w-render-0.2.3/web_render/flask/core/main/view.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/flask/core/render_api/logic.py` & `w-render-0.2.3/web_render/flask/core/render_api/logic.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/flask/core/render_api/view.py` & `w-render-0.2.3/web_render/flask/core/render_api/view.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/script/render_server.py` & `w-render-0.2.3/web_render/script/render_server.py`

 * *Files identical despite different names*

### Comparing `w-render-0.2.2/web_render/tool.py` & `w-render-0.2.3/web_render/tool.py`

 * *Files identical despite different names*


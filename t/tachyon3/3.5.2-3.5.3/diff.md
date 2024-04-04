# Comparing `tmp/tachyon3-3.5.2.tar.gz` & `tmp/tachyon3-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tachyon3-3.5.2.tar", last modified: Wed Apr  3 15:30:41 2024, max compression
+gzip compressed data, was "tachyon3-3.5.3.tar", last modified: Thu Apr  4 15:02:28 2024, max compression
```

## Comparing `tachyon3-3.5.2.tar` & `tachyon3-3.5.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.884801 tachyon3-3.5.2/
--rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2021-09-02 14:41:30.000000 tachyon3-3.5.2/LICENSE.md
--rw-rw-r--   0 lph       (1000) lph       (1000)      220 2024-04-03 15:30:41.884801 tachyon3-3.5.2/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)     3398 2021-09-02 14:41:30.000000 tachyon3-3.5.2/README.md
--rw-rw-r--   0 lph       (1000) lph       (1000)      108 2024-04-03 15:30:41.884801 tachyon3-3.5.2/setup.cfg
--rw-rw-r--   0 lph       (1000) lph       (1000)      573 2024-04-03 14:25:44.000000 tachyon3-3.5.2/setup.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.880801 tachyon3-3.5.2/tachyon/
--rw-rw-r--   0 lph       (1000) lph       (1000)      953 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)    13352 2022-02-15 17:31:06.000000 tachyon3-3.5.2/tachyon/__main__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      911 2024-04-03 15:30:16.000000 tachyon3-3.5.2/tachyon/__version__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1434 2022-02-15 17:31:06.000000 tachyon3-3.5.2/tachyon/conf.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5759 2024-04-03 14:25:44.000000 tachyon3-3.5.2/tachyon/config.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.880801 tachyon3-3.5.2/tachyon/data/
--rw-rw-r--   0 lph       (1000) lph       (1000)    45377 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/data/files.json
--rw-rw-r--   0 lph       (1000) lph       (1000)    29008 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/data/paths.json
--rw-rw-r--   0 lph       (1000) lph       (1000)     1286 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/database.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1880 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/dbutils.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2493 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/directoryfetcher.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2814 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/filefetcher.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5207 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/generator.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      984 2024-04-03 15:28:16.000000 tachyon3-3.5.2/tachyon/har.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.880801 tachyon3-3.5.2/tachyon/heuristics/
--rw-rw-r--   0 lph       (1000) lph       (1000)     1152 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/heuristics/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1358 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/heuristics/logbehaviorchange.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1673 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/heuristics/matchstring.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3804 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/heuristics/rejectignoredquery.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      337 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/heuristics/striptag.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1933 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/loaders.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3330 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/output.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.880801 tachyon3-3.5.2/tachyon/plugins/
--rw-rw-r--   0 lph       (1000) lph       (1000)      851 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/__init__.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.880801 tachyon3-3.5.2/tachyon/plugins/file/
--rw-rw-r--   0 lph       (1000) lph       (1000)      893 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/file/__init__.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.884801 tachyon3-3.5.2/tachyon/plugins/host/
--rw-rw-r--   0 lph       (1000) lph       (1000)     3581 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/HostProcessor.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2693 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/PathGenerator.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2506 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/Robots.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3131 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/SitemapXML.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     4739 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/Svn.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      956 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/plugins/host/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3274 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/result.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1467 2021-09-02 14:41:30.000000 tachyon3-3.5.2/tachyon/textutils.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-03 15:30:41.884801 tachyon3-3.5.2/tachyon3.egg-info/
--rw-rw-r--   0 lph       (1000) lph       (1000)      220 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)     1021 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/SOURCES.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        1 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/dependency_links.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       51 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/entry_points.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       79 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/requires.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        8 2024-04-03 15:30:41.000000 tachyon3-3.5.2/tachyon3.egg-info/top_level.txt
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/
+-rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2021-09-02 14:41:30.000000 tachyon3-3.5.3/LICENSE.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      220 2024-04-04 15:02:28.645937 tachyon3-3.5.3/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3398 2021-09-02 14:41:30.000000 tachyon3-3.5.3/README.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      108 2024-04-04 15:02:28.645937 tachyon3-3.5.3/setup.cfg
+-rw-rw-r--   0 lph       (1000) lph       (1000)      573 2024-04-03 14:25:44.000000 tachyon3-3.5.3/setup.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.641937 tachyon3-3.5.3/tachyon/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      953 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)    13610 2024-04-04 14:09:50.000000 tachyon3-3.5.3/tachyon/__main__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      911 2024-04-04 15:01:53.000000 tachyon3-3.5.3/tachyon/__version__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1434 2022-02-15 17:31:06.000000 tachyon3-3.5.3/tachyon/conf.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5905 2024-04-04 13:46:02.000000 tachyon3-3.5.3/tachyon/config.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.641937 tachyon3-3.5.3/tachyon/data/
+-rw-rw-r--   0 lph       (1000) lph       (1000)    45377 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/data/files.json
+-rw-rw-r--   0 lph       (1000) lph       (1000)    29008 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/data/paths.json
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1286 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/database.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1880 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/dbutils.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2493 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/directoryfetcher.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2814 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/filefetcher.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5207 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/generator.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      984 2024-04-03 15:28:16.000000 tachyon3-3.5.3/tachyon/har.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/tachyon/heuristics/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1152 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/heuristics/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1358 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/heuristics/logbehaviorchange.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1673 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/heuristics/matchstring.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3804 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/heuristics/rejectignoredquery.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      337 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/heuristics/striptag.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1933 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/loaders.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3330 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/output.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/tachyon/plugins/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      851 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/__init__.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/tachyon/plugins/file/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      893 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/file/__init__.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/tachyon/plugins/host/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3581 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/HostProcessor.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2693 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/PathGenerator.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2506 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/Robots.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3131 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/SitemapXML.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     4739 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/Svn.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      956 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/plugins/host/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3274 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/result.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1467 2021-09-02 14:41:30.000000 tachyon3-3.5.3/tachyon/textutils.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-04 15:02:28.645937 tachyon3-3.5.3/tachyon3.egg-info/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      220 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1021 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/SOURCES.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        1 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/dependency_links.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       51 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/entry_points.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       79 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/requires.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        8 2024-04-04 15:02:28.000000 tachyon3-3.5.3/tachyon3.egg-info/top_level.txt
```

### Comparing `tachyon3-3.5.2/LICENSE.md` & `tachyon3-3.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/README.md` & `tachyon3-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/setup.py` & `tachyon3-3.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/__init__.py` & `tachyon3-3.5.3/tachyon/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/__main__.py` & `tachyon3-3.5.3/tachyon/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,65 +259,72 @@
         output_manager.output_error("Invald URL provided.")
         return
 
     # Set conf values
     conf.target_host = parsed_url.netloc
     conf.base_url = "%s://%s" % (parsed_url.scheme, parsed_url.netloc)
     conf.pre_crawled_paths = pre_crawled_path or []
-    
-    hammertime = None
+
     accumulator = ResultAccumulator(output_manager=output_manager)
 
     output_manager.output_info('Starting Discovery on ' + conf.base_url)
 
     conf.allow_download = allow_download
     for option in plugin_settings:
         plugin, value = option.split(':', 1)
         conf.plugin_settings[plugin].append(value)
 
-    try:
-        root_path = conf.path_template.copy()
-        root_path['url'] = '/'
-        database.valid_paths.append(root_path)
-        for crawled_path in conf.pre_crawled_paths:
-            new_path = conf.path_template.copy()
-            new_path['url'] = crawled_path
-            database.valid_paths.append(new_path)
-        load_target_paths()
-        load_target_files()
-        conf.cookies = loaders.load_cookie_file(cookie_file)
-        conf.user_agent = user_agent
-        conf.proxy_url = proxy
-        conf.forge_vhost = vhost
-        loop = custom_event_loop()
-        hammertime = loop.run_until_complete(
-            configure_hammertime(cookies=conf.cookies, proxy=conf.proxy_url, retry_count=max_retry_count,
-                                 user_agent=conf.user_agent, vhost=conf.forge_vhost,
-                                 confirmation_factor=confirmation_factor,
-                                 concurrency=concurrency,
-                                 har_output_dir=har_output_dir))
-        t = loop.create_task(stat_on_input(hammertime))
-        loop.run_until_complete(scan(hammertime, accumulator=accumulator,
-                                     cookies=conf.cookies, directories_only=directories_only,
-                                     files_only=files_only, plugins_only=plugins_only, depth_limit=depth_limit,
-                                     recursive=recursive))
-        t.cancel()
-        output_manager.output_info('Scan completed')
-
-    except (KeyboardInterrupt, asyncio.CancelledError):
-        output_manager.output_error('Keyboard Interrupt Received')
-    except (OfflineHostException, StopRequest):
-        output_manager.output_error("Target host seems to be offline.")
-    except ImportError as e:
-        output_manager.output_error("Additional module is required for the requested options: %s" % e)
-    finally:
-        if hammertime is not None:
-            textutils.output_info(format_stats(hammertime.stats))
+    loop = custom_event_loop()
+
+    async def async_main():
+        hammertime = None
+        try:
+            root_path = conf.path_template.copy()
+            root_path['url'] = '/'
+            database.valid_paths.append(root_path)
+            for crawled_path in conf.pre_crawled_paths:
+                new_path = conf.path_template.copy()
+                new_path['url'] = crawled_path
+                database.valid_paths.append(new_path)
+            load_target_paths()
+            load_target_files()
+            conf.cookies = loaders.load_cookie_file(cookie_file)
+            conf.user_agent = user_agent
+            conf.proxy_url = proxy
+            conf.forge_vhost = vhost
+
+            async with configure_hammertime(cookies=conf.cookies, proxy=conf.proxy_url, retry_count=max_retry_count,
+                                            user_agent=conf.user_agent, vhost=conf.forge_vhost,
+                                            confirmation_factor=confirmation_factor,
+                                            concurrency=concurrency,
+                                            har_output_dir=har_output_dir) as hammertime:
+                try:
+                    t = loop.create_task(stat_on_input(hammertime))
+                    await scan(hammertime, accumulator=accumulator,
+                               cookies=conf.cookies, directories_only=directories_only,
+                               files_only=files_only, plugins_only=plugins_only, depth_limit=depth_limit,
+                               recursive=recursive)
+                finally:
+                    t.cancel()
+
+            output_manager.output_info('Scan completed')
+
+        except (KeyboardInterrupt, asyncio.CancelledError):
+            output_manager.output_error('Keyboard Interrupt Received')
+        except (OfflineHostException, StopRequest):
+            output_manager.output_error("Target host seems to be offline.")
+        except ImportError as e:
+            output_manager.output_error("Additional module is required for the requested options: %s" % e)
+        finally:
+            if hammertime is not None:
+                textutils.output_info(format_stats(hammertime.stats))
+
+            output_manager.flush()
 
-        output_manager.flush()
+    loop.run_until_complete(async_main())
 
 
 async def stat_on_input(hammertime):
     import sys
     from datetime import datetime, timedelta
 
     if sys.stdin is None or not sys.stdin.readable() or not sys.stdin.isatty():
@@ -326,15 +333,15 @@
     loop = asyncio.get_event_loop()
     reader = asyncio.StreamReader()
     reader_protocol = asyncio.StreamReaderProtocol(reader)
 
     await loop.connect_read_pipe(lambda: reader_protocol, sys.stdin)
 
     expiry = datetime.now()
-    while True:
+    while not hammertime.is_closed:
         await reader.readline()
 
         # Throttle stats printing
         if expiry < datetime.now():
             textutils.output_info(format_stats(hammertime.stats))
             expiry = datetime.now() + timedelta(seconds=2)
```

### Comparing `tachyon3-3.5.2/tachyon/__version__.py` & `tachyon3-3.5.3/tachyon/plugins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Tachyon - Fast Multi-Threaded Web Discovery Tool
 # Copyright (c) 2011 Gabriel Tremblay - initnull hat gmail.com
-# Copyright (C) 2018-  Delve Labs inc.
 #
 # GNU General Public Licence (GPL)
 #
 # This program is free software; you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation; either version 2 of the License, or (at your option) any later
 # version.
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
-
-__version__ = "3.5.2"
+#
```

### Comparing `tachyon3-3.5.2/tachyon/conf.py` & `tachyon3-3.5.3/tachyon/conf.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/config.py` & `tachyon3-3.5.3/tachyon/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
 
 
 from aiohttp import ClientSession, TCPConnector
 from aiohttp.cookiejar import DummyCookieJar
+from contextlib import asynccontextmanager
 from hammertime import HammerTime
 from hammertime.config import custom_event_loop
 from hammertime.engine import AioHttpEngine
 from hammertime.engine.scaling import SlowStartPolicy, StaticPolicy
 from hammertime.kb import KnowledgeBase
 from hammertime.ruleset import StopRequest
 from hammertime.rules.sampling import ContentHashSampling, ContentSampling, ContentSimhashSampling
@@ -36,14 +37,15 @@
 
 heuristics_with_child = []
 initial_limit = 5120
 default_user_agent = 'Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                      'Chrome/41.0.2228.0 Safari/537.36'
 
 
+@asynccontextmanager
 async def configure_hammertime(proxy=None, retry_count=3, cookies=None, concurrency=0, **kwargs):
     loop = custom_event_loop()
     engine = AioHttpEngine(loop=loop, verify_ssl=False, proxy=proxy)
     await engine.session.close()
     connector = TCPConnector(loop=loop, ssl=False, use_dns_cache=True, ttl_dns_cache=None)
     if cookies is not None:
         engine.session = ClientSession(loop=loop, connector=connector, cookie_jar=DummyCookieJar(loop=loop))
@@ -51,20 +53,23 @@
         engine.session = ClientSession(loop=loop, connector=connector)
 
     scale_policy = SlowStartPolicy(initial=3)
     if concurrency > 0:
         scale_policy = StaticPolicy(concurrency)
 
     kb = KnowledgeBase()
-    hammertime = HammerTime(loop=loop, request_engine=engine, retry_count=retry_count, proxy=proxy, kb=kb,
-                            scale_policy=scale_policy)
-    setup_hammertime_heuristics(hammertime, **kwargs)
-    hammertime.collect_successful_requests()
-    hammertime.kb = kb
-    return hammertime
+    try:
+        hammertime = HammerTime(loop=loop, request_engine=engine, retry_count=retry_count, proxy=proxy, kb=kb,
+                                scale_policy=scale_policy)
+        setup_hammertime_heuristics(hammertime, **kwargs)
+        hammertime.collect_successful_requests()
+        hammertime.kb = kb
+        yield hammertime
+    finally:
+        await engine.session.close()
 
 
 def setup_hammertime_heuristics(hammertime, *,
                                 user_agent=default_user_agent, vhost=None, confirmation_factor=1,
                                 har_output_dir=None):
     global heuristics_with_child
     dead_host_detection = DeadHostDetection(threshold=200)
```

### Comparing `tachyon3-3.5.2/tachyon/data/files.json` & `tachyon3-3.5.3/tachyon/data/files.json`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/data/paths.json` & `tachyon3-3.5.3/tachyon/data/paths.json`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/database.py` & `tachyon3-3.5.3/tachyon/database.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/dbutils.py` & `tachyon3-3.5.3/tachyon/dbutils.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/directoryfetcher.py` & `tachyon3-3.5.3/tachyon/directoryfetcher.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/filefetcher.py` & `tachyon3-3.5.3/tachyon/filefetcher.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/generator.py` & `tachyon3-3.5.3/tachyon/generator.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/har.py` & `tachyon3-3.5.3/tachyon/har.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/heuristics/__init__.py` & `tachyon3-3.5.3/tachyon/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/heuristics/logbehaviorchange.py` & `tachyon3-3.5.3/tachyon/heuristics/logbehaviorchange.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/heuristics/matchstring.py` & `tachyon3-3.5.3/tachyon/heuristics/matchstring.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/heuristics/rejectignoredquery.py` & `tachyon3-3.5.3/tachyon/heuristics/rejectignoredquery.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/loaders.py` & `tachyon3-3.5.3/tachyon/loaders.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/output.py` & `tachyon3-3.5.3/tachyon/output.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/__init__.py` & `tachyon3-3.5.3/tachyon/plugins/file/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
 #
+
+# Add all path plugins here
+__all__ = []
```

### Comparing `tachyon3-3.5.2/tachyon/plugins/file/__init__.py` & `tachyon3-3.5.3/tachyon/plugins/host/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
-# Add all path plugins here
-__all__ = []
+# Add all host plugins here
+__all__ = ["Robots", "SitemapXML", "PathGenerator", "HostProcessor", "Svn"]
```

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/HostProcessor.py` & `tachyon3-3.5.3/tachyon/plugins/host/HostProcessor.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/PathGenerator.py` & `tachyon3-3.5.3/tachyon/plugins/host/PathGenerator.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/Robots.py` & `tachyon3-3.5.3/tachyon/plugins/host/Robots.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/SitemapXML.py` & `tachyon3-3.5.3/tachyon/plugins/host/SitemapXML.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/Svn.py` & `tachyon3-3.5.3/tachyon/plugins/host/Svn.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/plugins/host/__init__.py` & `tachyon3-3.5.3/tachyon/__version__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Tachyon - Fast Multi-Threaded Web Discovery Tool
 # Copyright (c) 2011 Gabriel Tremblay - initnull hat gmail.com
+# Copyright (C) 2018-  Delve Labs inc.
 #
 # GNU General Public Licence (GPL)
 #
 # This program is free software; you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation; either version 2 of the License, or (at your option) any later
 # version.
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
-#
 
-# Add all host plugins here
-__all__ = ["Robots", "SitemapXML", "PathGenerator", "HostProcessor", "Svn"]
+__version__ = "3.5.3"
```

### Comparing `tachyon3-3.5.2/tachyon/result.py` & `tachyon3-3.5.3/tachyon/result.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon/textutils.py` & `tachyon3-3.5.3/tachyon/textutils.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.5.2/tachyon3.egg-info/SOURCES.txt` & `tachyon3-3.5.3/tachyon3.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/cubicweb-tsfacets-0.6.1.tar.gz` & `tmp/cubicweb-tsfacets-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-tsfacets-0.6.1.tar", last modified: Mon Sep 11 11:50:33 2023, max compression
+gzip compressed data, was "cubicweb-tsfacets-0.7.0.tar", last modified: Thu Apr  4 08:39:32 2024, max compression
```

## Comparing `cubicweb-tsfacets-0.6.1.tar` & `cubicweb-tsfacets-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.889562 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/
--rw-rw-rw-   0 root         (0) root         (0)     3670 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/ccplugin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-09-11 11:50:33.000000 cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2681 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-11 11:50:33.893562 cubicweb-tsfacets-0.6.1/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/test/test_tsfacets.py
--rw-rw-rw-   0 root         (0) root         (0)     1342 2023-09-11 11:50:26.000000 cubicweb-tsfacets-0.6.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3498 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    12923 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3498 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 08:39:32.000000 cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2681 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:39:32.297334 cubicweb-tsfacets-0.7.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/test/test_tsfacets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-04 08:39:23.000000 cubicweb-tsfacets-0.7.0/tox.ini
```

### Comparing `cubicweb-tsfacets-0.6.1/PKG-INFO` & `cubicweb-tsfacets-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: cubicweb-tsfacets
-Version: 0.6.1
+Version: 0.7.0
 Summary: This cube implements facets using postgresql text search vectors.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/tsfacets
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
+Requires-Dist: cubicweb>=3.31.1
+Requires-Dist: typing_extensions
 
 Summary
 -------
 This cube implements facets using postgresql text search vectors.
 
 What does this cube offer ?
 ---------------------------
```

### Comparing `cubicweb-tsfacets-0.6.1/README.md` & `cubicweb-tsfacets-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/__init__.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """cubicweb-tsfacets application package
 
 This cube implements facets using postgresql text search vectors.
 """
+
 import re
 import string
 
 from rql import RQLHelper
 
 from cubicweb.server.querier import QuerierHelper, manual_build_descr
 from cubicweb.server.sources.rql2sql import SQLGenerator
```

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/__pkginfo__.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/__pkginfo__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=W0622
 """cubicweb-tsfacets application packaging information"""
 
 
 modname = "cubicweb_tsfacets"
 distname = "cubicweb-tsfacets"
 
-numversion = (0, 6, 1)
+numversion = (0, 7, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "This cube implements facets using postgresql text search vectors."
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/tsfacets"
```

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/ccplugin.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/entities.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/hooks.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/importer.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,19 @@
             cnx.system_sql(f"DROP TABLE IF EXISTS {mapping_table_name}")
             cnx.system_sql(
                 f"""
                 CREATE TABLE
                     {mapping_table_name} (id serial PRIMARY KEY, value varchar)
                 """
             )
+
             if all_values:
                 insert = f"""
                 INSERT INTO {mapping_table_name} (value)
-                values {",".join(["(%s)"]*len(all_values))}
+                values {",".join(["(%s)"] * len(all_values))}
                 """
                 cnx.system_sql(insert, list(all_values))
             cnx.system_sql(f"CREATE INDEX ON {mapping_table_name}(value)")
             from_parts.append(
                 f"""
                 LEFT OUTER JOIN (
                     SELECT
@@ -60,16 +61,16 @@
                     FROM
                         ({sql}) as _f{facet_key}_to_be_mapped(target_eid,value)
                         JOIN {mapping_table_name} ON (
                             {mapping_table_name}.value = _f{facet_key}_to_be_mapped.value
                         )
                 ) as _f{facet_key}(target_eid,value)
                 ON entities.eid = _f{facet_key}.target_eid
-                """  # noqa
-            )
+                """
+            )  # noqa
         else:
             from_parts.append(
                 f"""
                 LEFT OUTER JOIN ({sql}) as _f{facet_key}(target_eid,value)
                 ON entities.eid = _f{facet_key}.target_eid
                 """
             )
```

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/migration/postcreate.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/schema.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets/views.py` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,22 +152,24 @@
 
     def get_facets_values_with_count(
         self,
         rql_restriction: str = None,
         rql_args: Dict = None,
         selected_facets: Dict[str, List[str]] = None,
         text_search: str = None,
+        keep_selected: bool = False,
     ) -> Dict[str, List[FacetItemType]]:
         """
         Retrieve all facet values with target entities count for each of them.
         :param rql_restriction: A RQL with a single variable in the Any close corresponding
         to the target entities.
         :param rql_args: arguments of rql_restriction.
         :param selected_facets: all selected facets as Dict[facet_key, [facet values]].
         :param text_search: a string to filter results.
+        :param keep_selected: if you want to remove count from already selected values.
         :return: a dictionary of the type Dict[facet_key, Dict[value, target entity count]]
         """
         selected_facets = selected_facets or {}
         sql_restriction_part, where_sql_part, sql_args = self._build_sql_parts(
             rql_restriction,
             rql_args,
             selected_facets,
@@ -193,15 +195,15 @@
             sql_args,
         )
 
         all_facets: Dict[str, List[FacetItemType]] = {}
         for code, value, count in crs.fetchall():
             if code not in self.key_names_to_rql_definition:
                 continue
-            if value in selected_facets.get(code, []):
+            if not keep_selected and value in selected_facets.get(code, []):
                 continue
 
             all_facets.setdefault(code, []).append(
                 {
                     "value": value,
                     "count": count,
                 }
```

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/PKG-INFO` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: cubicweb-tsfacets
-Version: 0.6.1
+Version: 0.7.0
 Summary: This cube implements facets using postgresql text search vectors.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/tsfacets
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
+Requires-Dist: cubicweb>=3.31.1
+Requires-Dist: typing_extensions
 
 Summary
 -------
 This cube implements facets using postgresql text search vectors.
 
 What does this cube offer ?
 ---------------------------
```

### Comparing `cubicweb-tsfacets-0.6.1/cubicweb_tsfacets.egg-info/SOURCES.txt` & `cubicweb-tsfacets-0.7.0/cubicweb_tsfacets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/setup.py` & `cubicweb-tsfacets-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/test/test_tsfacets.py` & `cubicweb-tsfacets-0.7.0/test/test_tsfacets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.6.1/tox.ini` & `cubicweb-tsfacets-0.7.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   {envpython} -m pytest {posargs:test}
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
   flake8 >= 3.6
-commands = flake8
+commands = flake8 --show-source
 
 [testenv:check-manifest]
 skip_install = true
 deps =
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
```


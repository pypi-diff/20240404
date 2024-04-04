# Comparing `tmp/sashimi_domains-0.9.6.tar.gz` & `tmp/sashimi_domains-0.9.7.tar.gz`

## Comparing `sashimi_domains-0.9.6.tar` & `sashimi_domains-0.9.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/TODO
--rw-r--r--   0        0        0    26084 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/blockology.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/corporalogy.py
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/graphology.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/config.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/entropies.py
--rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/ioio.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/misc.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/naming.py
--rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/scorology.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/vector_models.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/w2v_score.py
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/__init__.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/annotations.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/area_rank_chart.py
--rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/better_network_map.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/block_ext_map.py
--rw-r--r--   0        0        0    55047 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map_help.html
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/link_maps.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/network_map.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/util.py
--rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/zmethods.py
--rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables.css
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_html.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_plots.py
--rw-r--r--   0        0        0    37389 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/__init__.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/nlp.py
--rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/parsers.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/wos.py
--rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/blockstate_to_dataframes.py
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/domain_chained_model.py
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/domain_topic_model.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/util.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/asco_clean.py
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/pubmed_clean.py
--rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/pubmed_get.sh
--rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/scan_bugtrap.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/wos_lam/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/wos_lam/wos_api_request.tpl
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/tests/test_basic_usage.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/tests/test_pclabel_bfield.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/.gitignore
--rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/LICENSE
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/README.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/TODO
+-rw-r--r--   0        0        0    26084 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/limbo/blockology.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/limbo/corporalogy.py
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/limbo/graphology.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/config.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/entropies.py
+-rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/ioio.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/misc.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/naming.py
+-rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/scorology.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/vector_models.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/w2v_score.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/__init__.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/annotations.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/area_rank_chart.py
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/better_network_map.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/block_ext_map.py
+-rw-r--r--   0        0        0    55047 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/hierarchical_block_map.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/hierarchical_block_map_help.html
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/link_maps.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/network_map.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/util.py
+-rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/zmethods.py
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/tables/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables.css
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables_html.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables_plots.py
+-rw-r--r--   0        0        0    37389 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/corpus/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/corpus/nlp.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/corpus/parsers.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/corpus/wos.py
+-rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/graph_models/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/graph_models/blockstate_to_dataframes.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/graph_models/domain_chained_model.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/graph_models/domain_topic_model.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/graph_models/util.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/asco_clean.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/pubmed_clean.py
+-rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/pubmed_get.sh
+-rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/scan_bugtrap.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/wos_lam/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/src/sashimi/util/wos_lam/wos_api_request.tpl
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/tests/test_basic_usage.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/tests/test_pclabel_bfield.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/.gitignore
+-rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/LICENSE
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    10378 2020-02-02 00:00:00.000000 sashimi_domains-0.9.7/PKG-INFO
```

### Comparing `sashimi_domains-0.9.6/TODO` & `sashimi_domains-0.9.7/TODO`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/limbo/blockology.py` & `sashimi_domains-0.9.7/src/limbo/blockology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/limbo/corporalogy.py` & `sashimi_domains-0.9.7/src/limbo/corporalogy.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/limbo/graphology.py` & `sashimi_domains-0.9.7/src/limbo/graphology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 
 __author__ = "Alexandre Hannud Abdo <abdo@member.fsf.org>"
 __copyright__ = "Copyright 2016-2024 Alexandre Hannud Abdo"
 __license__ = "GNU GPL version 3 or above"
 __URL__ = "https://gitlab.com/solstag/sashimi/"
 
-__version__ = "0.9.6"
+__version__ = "0.9.7"
 
 #######################
 # Expose main classes #
 #######################
 
 __all__ = ["Corpus", "GraphModels", "VectorModels"]
```

### Comparing `sashimi_domains-0.9.6/src/sashimi/config.py` & `sashimi_domains-0.9.7/src/sashimi/config.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/entropies.py` & `sashimi_domains-0.9.7/src/sashimi/entropies.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/ioio.py` & `sashimi_domains-0.9.7/src/sashimi/ioio.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/misc.py` & `sashimi_domains-0.9.7/src/sashimi/misc.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/naming.py` & `sashimi_domains-0.9.7/src/sashimi/naming.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/scorology.py` & `sashimi_domains-0.9.7/src/sashimi/scorology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/vector_models.py` & `sashimi_domains-0.9.7/src/sashimi/vector_models.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/w2v_score.py` & `sashimi_domains-0.9.7/src/sashimi/w2v_score.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/annotations.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/annotations.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/area_rank_chart.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/area_rank_chart.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/better_network_map.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/better_network_map.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/block_ext_map.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/block_ext_map.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/hierarchical_block_map.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map_help.html` & `sashimi_domains-0.9.7/src/sashimi/blocks/hierarchical_block_map_help.html`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/link_maps.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/link_maps.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/network_map.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/network_map.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/util.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/util.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/zmethods.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/zmethods.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/tables/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables.css` & `sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables.css`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_html.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables_html.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_plots.py` & `sashimi_domains-0.9.7/src/sashimi/blocks/tables/tables_plots.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/corpus/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/corpus/nlp.py` & `sashimi_domains-0.9.7/src/sashimi/corpus/nlp.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/corpus/parsers.py` & `sashimi_domains-0.9.7/src/sashimi/corpus/parsers.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/corpus/wos.py` & `sashimi_domains-0.9.7/src/sashimi/corpus/wos.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/graph_models/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/graph_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/graph_models/blockstate_to_dataframes.py` & `sashimi_domains-0.9.7/src/sashimi/graph_models/blockstate_to_dataframes.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/graph_models/domain_chained_model.py` & `sashimi_domains-0.9.7/src/sashimi/graph_models/domain_chained_model.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/graph_models/domain_topic_model.py` & `sashimi_domains-0.9.7/src/sashimi/graph_models/domain_topic_model.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/graph_models/util.py` & `sashimi_domains-0.9.7/src/sashimi/graph_models/util.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/util/asco_clean.py` & `sashimi_domains-0.9.7/src/sashimi/util/asco_clean.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/util/pubmed_get.sh` & `sashimi_domains-0.9.7/src/sashimi/util/pubmed_get.sh`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/util/scan_bugtrap.py` & `sashimi_domains-0.9.7/src/sashimi/util/scan_bugtrap.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/util/wos_lam/__init__.py` & `sashimi_domains-0.9.7/src/sashimi/util/wos_lam/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/src/sashimi/util/wos_lam/wos_api_request.tpl` & `sashimi_domains-0.9.7/src/sashimi/util/wos_lam/wos_api_request.tpl`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/tests/test_basic_usage.py` & `sashimi_domains-0.9.7/tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/tests/test_pclabel_bfield.py` & `sashimi_domains-0.9.7/tests/test_pclabel_bfield.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/LICENSE` & `sashimi_domains-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.6/README.md` & `sashimi_domains-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Sashimi — study the organization and evolution of corpora
 
-`sashimi` is a Python module for mixed-methods qualitative studies of large
-textual or symbolic corpora, providing applications of statistical models
-accompanied by tailored interactive visualizations. It affords the detection of
-both textual and metadata structures by employing stochastic block modeling
-(SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently
-deprecated) word embedding from `gensim`.
+A Python module for mixed-methods qualitative studies of large textual or
+symbolic corpora, providing applications of statistical models accompanied by
+tailored interactive visualizations. It affords the detection of both textual
+and metadata structures by employing stochastic block modeling (SBM) from
+`graph-tool` or (currently deprecated) word embedding from `gensim`.
 
 ### Statistical models
 - Domain-topic models
   - Synthesizes document clustering (domain modeling) and topic modeling (term clustering).
 - Domain-chained models
   - Extrapolates modeled domains to partition other dimensions of the corpus such as time, people, institutions, categories or places.
 
@@ -169,15 +168,15 @@
 
 - **Better network map**: An entirely new network map function with many improvements and new features is under development and can be tried from `from sashimi.blocks.better_network_map import network_map`. It will eventually replace the current network map.
 
 <div align="center">
 <img
   alt="Domain-authors network"
   src="https://docs.cortext.net/wp-content/uploads/Image-2.png"
-  width="50%">
+  width="62%">
 </div>
 
 Development
 -----------
 
 This module provides four main classes:
```

### Comparing `sashimi_domains-0.9.6/pyproject.toml` & `sashimi_domains-0.9.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sashimi-domains"
-description = "`sashimi` is a Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently deprecated) word embedding from `gensim`."
+description = "A Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from `graph-tool` or (currently deprecated) word embedding from `gensim`."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "Ale Abdo", email = "abdo@member.fsf.org" },
 ]
```

### Comparing `sashimi_domains-0.9.6/PKG-INFO` & `sashimi_domains-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: sashimi-domains
-Version: 0.9.6
-Summary: `sashimi` is a Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently deprecated) word embedding from `gensim`.
+Version: 0.9.7
+Summary: A Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from `graph-tool` or (currently deprecated) word embedding from `gensim`.
 Project-URL: Documentation, https://gitlab.com/solstag/sashimi/
 Project-URL: Issues, https://gitlab.com/solstag/sashimi/-/issues
 Project-URL: Source, https://gitlab.com/solstag/sashimi/
 Author-email: Ale Abdo <abdo@member.fsf.org>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -24,20 +24,19 @@
 Requires-Dist: scipy
 Requires-Dist: spacy
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Sashimi — study the organization and evolution of corpora
 
-`sashimi` is a Python module for mixed-methods qualitative studies of large
-textual or symbolic corpora, providing applications of statistical models
-accompanied by tailored interactive visualizations. It affords the detection of
-both textual and metadata structures by employing stochastic block modeling
-(SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently
-deprecated) word embedding from `gensim`.
+A Python module for mixed-methods qualitative studies of large textual or
+symbolic corpora, providing applications of statistical models accompanied by
+tailored interactive visualizations. It affords the detection of both textual
+and metadata structures by employing stochastic block modeling (SBM) from
+`graph-tool` or (currently deprecated) word embedding from `gensim`.
 
 ### Statistical models
 - Domain-topic models
   - Synthesizes document clustering (domain modeling) and topic modeling (term clustering).
 - Domain-chained models
   - Extrapolates modeled domains to partition other dimensions of the corpus such as time, people, institutions, categories or places.
 
@@ -197,15 +196,15 @@
 
 - **Better network map**: An entirely new network map function with many improvements and new features is under development and can be tried from `from sashimi.blocks.better_network_map import network_map`. It will eventually replace the current network map.
 
 <div align="center">
 <img
   alt="Domain-authors network"
   src="https://docs.cortext.net/wp-content/uploads/Image-2.png"
-  width="50%">
+  width="62%">
 </div>
 
 Development
 -----------
 
 This module provides four main classes:
```


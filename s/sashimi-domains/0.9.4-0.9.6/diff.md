# Comparing `tmp/sashimi_domains-0.9.4.tar.gz` & `tmp/sashimi_domains-0.9.6.tar.gz`

## Comparing `sashimi_domains-0.9.4.tar` & `sashimi_domains-0.9.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/blockology.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/corporalogy.py
--rw-r--r--   0        0        0    15649 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/graphology.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/config.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/entropies.py
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/ioio.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/misc.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/naming.py
--rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/scorology.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/vectorology.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/w2v_score.py
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/__init__.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/annotations.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/area_rank_chart.py
--rw-r--r--   0        0        0    14781 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/better_network_map.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/block_ext_map.py
--rw-r--r--   0        0        0    55053 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map_help.html
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/link_maps.py
--rw-r--r--   0        0        0    11655 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/network_map.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/util.py
--rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/zmethods.py
--rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables.css
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_html.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_plots.py
--rw-r--r--   0        0        0    37395 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/__init__.py
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/nlp.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/parsers.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/wos.py
--rw-r--r--   0        0        0    14648 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/blockstate_to_dataframes.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/domain_chained_model.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/domain_topic_model.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/util.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/asco_clean.py
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/pubmed_clean.py
--rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/pubmed_get.sh
--rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/scan_bugtrap.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/wos_lam/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/wos_lam/wos_api_request.tpl
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/tests/test_basic_usage.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/tests/test_pclabel_bfield.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/.gitignore
--rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/LICENSE
--rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/README.md
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/TODO
+-rw-r--r--   0        0        0    26084 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/blockology.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/corporalogy.py
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/limbo/graphology.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/config.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/entropies.py
+-rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/ioio.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/misc.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/naming.py
+-rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/scorology.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/vector_models.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/w2v_score.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/__init__.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/annotations.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/area_rank_chart.py
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/better_network_map.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/block_ext_map.py
+-rw-r--r--   0        0        0    55047 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map_help.html
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/link_maps.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/network_map.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/util.py
+-rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/zmethods.py
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables.css
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_html.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_plots.py
+-rw-r--r--   0        0        0    37389 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/nlp.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/parsers.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/corpus/wos.py
+-rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/blockstate_to_dataframes.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/domain_chained_model.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/domain_topic_model.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/graph_models/util.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/asco_clean.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/pubmed_clean.py
+-rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/pubmed_get.sh
+-rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/scan_bugtrap.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/wos_lam/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/src/sashimi/util/wos_lam/wos_api_request.tpl
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/tests/test_basic_usage.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/tests/test_pclabel_bfield.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/.gitignore
+-rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/LICENSE
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 sashimi_domains-0.9.6/PKG-INFO
```

### Comparing `sashimi_domains-0.9.4/src/limbo/blockology.py` & `sashimi_domains-0.9.6/src/limbo/blockology.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
 import graph_tool.all as gt
 import multiprocessing, numpy, os, pandas, pickle, colorcet
 from functools import cache, partial
```

### Comparing `sashimi_domains-0.9.4/src/limbo/corporalogy.py` & `sashimi_domains-0.9.6/src/limbo/corporalogy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 ########################
 # Document-Term Matrix #
 ########################
 # Seemed like a good idea once upon a time, but turns out to be useless.
```

### Comparing `sashimi_domains-0.9.4/src/limbo/graphology.py` & `sashimi_domains-0.9.6/src/limbo/graphology.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
 class GraphologyLimbo(Blockology, Scorology, Corporalogy):
     def __init__(self):
         self.sext = ".score"
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 """
 See README.md for usage information.
 """
 
 __author__ = "Alexandre Hannud Abdo <abdo@member.fsf.org>"
 __copyright__ = "Copyright 2016-2024 Alexandre Hannud Abdo"
 __license__ = "GNU GPL version 3 or above"
 __URL__ = "https://gitlab.com/solstag/sashimi/"
 
-__version__ = "0.9.4"
-
-__all__ = ["Corpus", "GraphModels", "Vectorology"]
-
-import graph_tool  # to avoid import order issues with pandas # noqa
+__version__ = "0.9.6"
 
 #######################
 # Expose main classes #
 #######################
 
+__all__ = ["Corpus", "GraphModels", "VectorModels"]
+
 from .corpus import Corpus
 from .graph_models import GraphModels
-from .vectorology import Vectorology
+from .vector_models import VectorModels
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/config.py` & `sashimi_domains-0.9.6/src/sashimi/config.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/entropies.py` & `sashimi_domains-0.9.6/src/sashimi/entropies.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/ioio.py` & `sashimi_domains-0.9.6/src/sashimi/ioio.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
 import pickle
 import json
 import gzip
@@ -257,15 +257,17 @@
 
         # json doesn't handle tuples, so we must find and convert our tokens
         if fmt == "json" and doc_as_tuple:
             df = df.transform(
                 lambda x: x.map(lambda y: tuple(map(tuple, y)), na_action="ignore")
                 if all(
                     type(y) is list
-                    and all(type(z) is list and all(type(w) is str for w in z) for z in y)
+                    and all(
+                        type(z) is list and all(type(w) is str for w in z) for z in y
+                    )
                     for y in x.loc[x.notna()]
                 )
                 else x
             )
         return df
 
     @classmethod
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/naming.py` & `sashimi_domains-0.9.6/src/sashimi/naming.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import re
 from os import path
 from itertools import chain
 
@@ -66,7 +66,21 @@
     def gen(cls, base, params, suffix):
         params = [tuple(map(str, x)) for x in params]
         cls.check(*chain(*params), suffix)
         base = cls.escape(base)
         params = (map(cls.escape, x) for x in params)
         name = cls.itemsep.join(chain([base], map(cls.valsep.join, params)))
         return path.extsep.join([name, suffix.lstrip(path.extsep)])
+
+
+def get_output_path(corpus, hash_dims, fname_base, fname_params, fname_suffix):
+    """
+    (hash_dims: list) dimensions for the sample hash, among "doc", "ter" and "ext".
+    """
+    if sample_hash := corpus.get_sample_hash({dim: True for dim in hash_dims}):
+        fname_params = [("sample", sample_hash), *fname_params]
+
+    target_dir = (
+        corpus.chained_dir if "ext" in hash_dims is True else corpus.blocks_adir
+    )
+    fpath = target_dir / naming.gen(fname_base, fname_params, fname_suffix)
+    return fpath
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/scorology.py` & `sashimi_domains-0.9.6/src/sashimi/scorology.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import numpy, os, pandas
 import lxml.html as html, lxml.html.builder as build
 from collections import OrderedDict
 from matplotlib import pyplot as plt, colors as colors
@@ -282,15 +282,15 @@
                 marks = {
                     scores.columns[1]: [1],
                     scores.columns[-2]: [len(scores.columns) - 1],
                 }.setdefault(self.data.loc[i, groupby], [])
                 plot_ext.update(marker="o", markevery=marks)
             plt.plot(scores.columns, scores.loc[i], **plot_ext)
             if (
-                str(type(self)) == "<class 'sashimi.Vectorology.Vectorology'>"
+                str(type(self)) == "<class 'sashimi.vector_models.VectorModels'>"
                 and len(index) == 1
                 and False
             ):
                 plot_ext["label"] = "pp-{}".format(plot_ext["label"])
                 sentence = self.data.loc[i, self.column][0]
                 mode = self.get_mode(mode)
                 plt.plot(
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/vectorology.py` & `sashimi_domains-0.9.6/src/sashimi/vector_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,39 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of_innovation_in
 #  _the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
-try:
-    import gensim
-except ImportError:
-    print("Warning: Failed to import `gensim`, some functions may not be available")
 
 import multiprocessing
 import os
-import pandas
 from os import path
 from pathlib import Path
 from collections import OrderedDict
 from copy import deepcopy
+import logging
+
+import pandas
 
+from .misc import _try_import
 from .ioio import ioio
 from .corpus import Corpus
 from .scorology import Scorology
 
+logger = logging.getLogger(__name__)
+gensim = _try_import("gensim")
+
 
-class Vectorology(Scorology, Corpus):
+class VectorModels(Scorology, Corpus):
     """
     Word embedding model training and scoring
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/w2v_score.py` & `sashimi_domains-0.9.6/src/sashimi/w2v_score.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from collections import Counter
 from functools import cache
 
 import pandas as pd
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/annotations.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/annotations.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/area_rank_chart.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/area_rank_chart.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/better_network_map.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/better_network_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,60 +7,61 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from functools import cache
 
 # from itertools import islice
 # import re
 
 import logging
 
-import graph_tool.all as gt
-
 # import numpy as np
 import pandas as pd
 
 from .. import GraphModels
+from ..misc import _try_import
 from .util import phi
 from .annotations import make_get_annotations
 
 from .network_map import area2radius, first_element
 
 # from ..naming import naming
 # from ..misc import get_hash
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
+gt = _try_import("graph_tool.all")
+
 # Characteristic edge threshold
 Y_KINDS_ENT_FRAC = {"ter": 0.5, "ext": 0.95}
 
 # Network map colors
 COLOR_TRANSPARENT = [0, 0, 0, 0]
 COLOR_DOMAIN = [1, 0, 0, 0.8]
 COLOR_DOMAIN_PURE = [1, 0, 0, 0]
 COLOR_TOPIC = [0, 0, 1, 0.8]
 COLOR_TOPIC_PURE = [0, 0, 1, 1]
 COLOR_EXTENDED = [0, 0.5, 0, 0.8]
 COLOR_EXTENDED_PURE = [0, 0.5, 0, 1]
 COLOR_BLACK = [0, 0, 0, 0.8]
 COLOR_BLACK_PURE = [0, 0, 0, 1]
-BLOCK_SIZE = 50
+BLOCK_SIZE = 50 * 2.5
 DOC_ELEMENT_SIZE = BLOCK_SIZE / phi**3
 ELEMENT_SIZE = BLOCK_SIZE / phi**2
-BLOCK_FONT_SIZE = 12
-ELEMENT_FONT_SIZE = 8
+BLOCK_FONT_SIZE = 12 * 2
+ELEMENT_FONT_SIZE = 8 * 2.5
 EDGE_FONT_SIZE = 10
 
 # BLOCK_PEN_WIDTH = 3
 # ELEMENT_PEN_WIDTH = 3/ / phi
 
 
 def network_map(
@@ -133,15 +134,15 @@
             elif vp_kind[v] == "ter":
                 vp_size[v] = ELEMENT_SIZE
                 vp_color[v] = COLOR_TRANSPARENT
                 vp_text_color[v] = COLOR_TOPIC_PURE
             elif vp_kind[v] == "ext":
                 vp_size[v] = ELEMENT_SIZE
                 vp_color[v] = COLOR_EXTENDED
-                vp_text_color[v] = COLOR_EXTENDED_PURE
+                vp_text_color[v] = COLOR_BLACK_PURE  # COLOR_EXTENDED_PURE
 
     # Edge properties
     ep_specificity = g.ep["specificity"]
     # min_specificity = min(ep_specificity[e] for v in g.edges() if ep_specificity[e] > 0)
     max_specificity = max(
         (ep_specificity[e] for e in g.edges() if ep_specificity[e] > 0), default=0
     )
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/block_ext_map.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/block_ext_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import os, numpy, pandas
 from itertools import chain
 import bokeh.plotting as bkp, bokeh.models as bkm, bokeh.layouts as bkl
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from pathlib import Path
 
 import colorcet
 import numpy as np
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map_help.html` & `sashimi_domains-0.9.6/src/sashimi/blocks/hierarchical_block_map_help.html`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/link_maps.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/link_maps.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/network_map.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/network_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from itertools import islice
+import logging
 import re
 
-import graph_tool.all as gt
 import numpy as np
 
 from ..naming import naming
 from .annotations import (
     get_xblock_yblocks_elements,
     get_subxblocks_yblocks_elements,
     load_annotations,
 )
-from ..misc import get_hash
+from ..misc import get_hash, _try_import
+
+logger = logging.getLogger(__name__)
+gt = _try_import("graph_tool.all")
 
 
 def first_element(yb_info_elements):
     return yb_info_elements[0][0] if yb_info_elements else ""
 
 
 def dblock_terext_graph(
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/util.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import numpy as np
 import pandas
 
 phi = (1 + 5**0.5) / 2  # the golden ratio
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/zmethods.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/zmethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import pandas
 from collections import Counter
 from tqdm import tqdm
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/tables/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/tables/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import re
 import logging
 from pathlib import Path
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables.css` & `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables.css`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_html.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_html.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_plots.py` & `sashimi_domains-0.9.6/src/sashimi/blocks/tables/tables_plots.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/corpus/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/corpus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 # stdlib
 from collections import Counter
 from copy import deepcopy
 from functools import cache
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/corpus/nlp.py` & `sashimi_domains-0.9.6/src/sashimi/corpus/nlp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """
 Routines to turn text into tokens suitable as graph nodes.
 """
 from itertools import chain
-from logging import getLogger
 import re
+import logging
 
 import pandas as pd
 
-log = getLogger(__name__)
+from ..misc import _try_import
 
-try:
-    import spacy
-    from spacy.util import compile_infix_regex
-except ImportError:
-    log.warning("Spacy could not be imported: tokenization will be unavailable.")
-
-try:
-    from gensim.models import phrases
-except ImportError:
-    log.warning("Gensim could not be imported: ngrams will be unavailable.")
+spacy = _try_import("spacy")
+compile_infix_regex = _try_import("spacy.util").compile_infix_regex
+phrases = _try_import("gensim.models.phrases")
+
+logger = logging.getLogger(__name__)
 
 
 def process_token_sources(token_sources, to_doc=None):
     to_doc = tokens_to_doc if to_doc is None else to_doc
     return token_sources.applymap(to_doc, na_action="ignore").agg(
         lambda row: [sen for doc in row.dropna() for sen in doc], axis=1
     )
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/corpus/parsers.py` & `sashimi_domains-0.9.6/src/sashimi/corpus/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import json
 import os
 from os import path
 
@@ -64,15 +64,15 @@
     fnames = [name for name in os.listdir(csv_dir) if name.endswith(".csv")]
     df = pandas.read_csv(path.join(csv_dir, fnames.pop(0)), **read_csv_args)
     for name in fnames:
         df = df.append(
             pandas.read_csv(path.join(csv_dir, name), low_memory=False),
             ignore_index=True,
             sort=False,
-            **read_csv_args
+            **read_csv_args,
         )
     return df
 
 
 def get_esmo(esmo_path):
     data = list()
     years = sorted(int(i) for i in os.listdir(esmo_path))
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/corpus/wos.py` & `sashimi_domains-0.9.6/src/sashimi/corpus/wos.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from ..util.wos_lam import WosLam
 
 
 def load_wos_citations(self, user=None, password=None, pmids=None):
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/graph_models/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/graph_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,43 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
-import graph_tool.all as gt
-import numpy
+import logging
 from pathlib import Path
 import shutil
 
+import numpy
+
 from ..misc import clearattrs, makep_fromdict, property_getfuncdir
 from ..ioio import ioio
 from ..corpus import Corpus
 from ..scorology import Scorology
 from ..blocks import Blocks
+from ..misc import _try_import
 
 from . import blockstate_to_dataframes
 from .domain_topic_model import create_docter_graph, calc_nested_blockstate
 from .domain_chained_model import (
     extend_graph,
     gen_doc_graph,
     calc_chained_nested_blockstate,
 )
 
+logger = logging.getLogger(__name__)
+gt = _try_import("graph_tool.all")
+
 
 class GraphModels(Blocks, Scorology, Corpus):
     """
     Build graphs from corpora and find optimal block models.
     """
 
     def __init__(self, *args, **kwargs):
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/graph_models/blockstate_to_dataframes.py` & `sashimi_domains-0.9.6/src/sashimi/graph_models/blockstate_to_dataframes.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/graph_models/domain_chained_model.py` & `sashimi_domains-0.9.6/src/sashimi/graph_models/domain_chained_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
+import logging
+
 import numpy
 from itertools import count
-import graph_tool.all as gt
 
 from ..naming import naming
+from ..misc import _try_import
 from .util import contiguous_map_nested_blockstate
 
+logger = logging.getLogger(__name__)
+gt = _try_import("graph_tool.all")
+
 
 def calc_chained_nested_blockstate(
     corpus, bext="max", niter=10, strategy=["anneal", "sweep"]
 ):
     """
     Calculates a chained nested blockstate for vertices derived from
     values of some property of the documents.
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/graph_models/domain_topic_model.py` & `sashimi_domains-0.9.6/src/sashimi/graph_models/domain_topic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
-import graph_tool.all as gt
-
+import logging
 from itertools import count
 
 import numpy as np
 from tqdm import tqdm
 
 from ..naming import naming
+from ..misc import _try_import
 from .util import contiguous_map_nested_blockstate
 
+logger = logging.getLogger(__name__)
+gt = _try_import("graph_tool.all")
+
 
 def create_docter_graph(corpus, by=None):
     """
     Creates one or more document term graphs, names it, stores it and
     sets as loaded.
 
     Parameters
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/graph_models/util.py` & `sashimi_domains-0.9.6/src/sashimi/graph_models/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
 def contiguous_map_nested_blockstate(ns, io_is_bs=False):
     bs = ns if io_is_bs else ns.get_bs()
     bs = [b.copy() for b in bs]
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/util/asco_clean.py` & `sashimi_domains-0.9.6/src/sashimi/util/asco_clean.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/util/pubmed_get.sh` & `sashimi_domains-0.9.6/src/sashimi/util/pubmed_get.sh`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/util/scan_bugtrap.py` & `sashimi_domains-0.9.6/src/sashimi/util/scan_bugtrap.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/src/sashimi/util/wos_lam/__init__.py` & `sashimi_domains-0.9.6/src/sashimi/util/wos_lam/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from urllib.parse import urlencode
 from urllib.request import Request, urlopen
 from lxml import etree
 import pkg_resources
```

### Comparing `sashimi_domains-0.9.4/src/sashimi/util/wos_lam/wos_api_request.tpl` & `sashimi_domains-0.9.6/src/sashimi/util/wos_lam/wos_api_request.tpl`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/tests/test_basic_usage.py` & `sashimi_domains-0.9.6/tests/test_basic_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if "BASE_DIR" not in locals():
     BASE_DIR = TemporaryDirectory(prefix="sashimi_test-")
     os.chdir(BASE_DIR.name)
     print(BASE_DIR.name)
 
 if "VALUES_EXAMPLE_DATA" not in locals():
     VALUES_EXAMPLE_DATA = [0, 1, 3]
+    # VALUES_EXAMPLE_DATA = [3]
 
 
 @cache
 def example_data():
     if EXAMPLE_DATA == 0:
         df = pd.DataFrame(
             {
```

### Comparing `sashimi_domains-0.9.4/tests/test_pclabel_bfield.py` & `sashimi_domains-0.9.6/tests/test_pclabel_bfield.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/LICENSE` & `sashimi_domains-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.4/README.md` & `sashimi_domains-0.9.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-# Sashimi - study the organisation and evolution of corpora
+# Sashimi — study the organization and evolution of corpora
 
-Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations
-for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual
-and metadata structures and shifts, by employing stochastic block modeling (SBM) from [graph-tool](https://graph-tool.skewed.de/) or
-[currently deprecated] word embedding from `Gensim`.
+`sashimi` is a Python module for mixed-methods qualitative studies of large
+textual or symbolic corpora, providing applications of statistical models
+accompanied by tailored interactive visualizations. It affords the detection of
+both textual and metadata structures by employing stochastic block modeling
+(SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently
+deprecated) word embedding from `gensim`.
 
-Models:
+### Statistical models
 - Domain-topic models
-- Domain-chained (metadata) models
-
-Model-based data interfaces (visualisations):
-- Interactive domain-topic maps and domain-chained maps
-- Domain-topic tables and domain-chained tables
-- Domain-topic, domain-chained and domain-topic-chained networks
-- Area rank charts (bump charts) of the evolution of domain sizes
-
-<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-10-56-41.png" width="50%">
-
-## Using Sashimi without programming (no code)
-
-Sashimi is available as a suite of methods in the [Cortext Manager](https://docs.cortext.net/) web service. See [SASHIMI](https://docs.cortext.net/sashimi/).
-
-## Savoring Sashimi
-Also for users of this library, the [documentation](https://docs.cortext.net/sashimi/) at Cortext serves as a good introduction to the methodology.
+  - Synthesizes document clustering (domain modeling) and topic modeling (term clustering).
+- Domain-chained models
+  - Extrapolates modeled domains to partition other dimensions of the corpus such as time, people, institutions, categories or places.
+
+### Human model-data interfaces
+- Domain maps
+  - An interactive HTML document to explore the corpus and its clusters, enhanced with histograms and a search function.
+- Domain tables
+  - Ideal for systematic annotation of clusters.
+- Domain networks
+  - To visualize relations between domains, topics and clusters of other dimensions.
+- Area rank charts
+  - Beautiful "bump charts" displaying the evolution of domains.
+
+<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Image-1.png" width="50%">
+
+## Eat in: "no code" usage
+
+Much of the functionality of `sashimi` is available as a suite of methods in the [Cortext
+Manager](https://docs.cortext.net/) web service. See their documentation for
+[SASHIMI](https://docs.cortext.net/sashimi/), which may also serve users of the Python module as an introduction to the methodology.
 
 ## Installation
 
-Install [graph-tool](https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions) according to your system.
+You must first ~~sharpen your knife~~ install `graph-tool` by following the [installation instructions](https://graph-tool.skewed.de/installation.html) according to your system.
 
 Then:
 
 `pip install sashimi-domains`
 
 ### Dependencies
 
+With the exception of graph-tool, dependencies will be automatically installed by `pip`.
+
 This project builds mainly on the following others:
-- [graph-tool](graph-tool.skewed.de/) (for Stochastic Block Model inference)
-- [pandas](https://pandas.pydata.org/)
+- [graph-tool](graph-tool.skewed.de/) (for stochastic block model inference)
+- [pandas](https://pandas.pydata.org/) (for tabular data manipulation)
 - [spacy](https://spacy.io/) (for tokenization)
-- [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
-- [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
-- [lxml](https://lxml.de/) (for building domain tables)
-- [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
-
-With the exception of graph-tool, dependencies will be automatically installed by `pip`.
+- [gensim](https://radimrehurek.com/gensim/) (for n-gram detection)
+- [bokeh](https://bokeh.org/) (for building interactive maps and plots)
+- [lxml](https://lxml.de/) (for building HTML documents)
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
 import pandas as pd
 
@@ -72,18 +78,18 @@
 ```python
 # Set the data column labels for text sources
 corpus.text_sources = ["title", "body"]
 
 # Set up how to process text sources, for example:
 text_sources_args = dict(ngrams=3, language="en", stop_words=True)
 ```
-The `language` is any valid `spacy` language, where `None` will use the English tokenizer with no stop_words. Our English tokenizer is slightly improved from spacy's original, in order to get ["hot-dog"] out of "hot-dog" (when spacy would split that), ["this", "that"] out of "this/that", and ["citation"] out of "citation[2,3]".
+The `language` is any valid language for `spacy`, where `None` will use the English tokenizer with no stop_words. Our English tokenizer is slightly improved from `spacy`'s original, in order to get ["hot-dog"] out of "hot-dog" (when spacy would split that), ["this", "that"] out of "this/that", and ["citation"] out of "citation[2,3]".
 
 #### Token data
-You may also directly use tokens that you've processed yourself, or from token data such as keywords, categories, or anything really, in addition or in place of textual data.
+You may also directly use tokens that you have processed yourself, or from token data such as keywords, categories, or anything really, in addition or in place of textual data.
 ```python
 # Set the data column labels for token sources
 corpus.token_sources = ["keyword", "category"]
 ```
 
 Token data for a document is expected to be in the form of a list, containing strings or lists containing strings: `List[str | List[str]]`. If your data differs, you must adjust it before processing.
 
@@ -147,37 +153,46 @@
 corpus.domain_network(doc_level=2, ter_level=1, ext_level=1, edges="common")
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ext")
 ```
 
 <img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-11-02-16.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
 
-## Advanced usages
+## Advanced usage
+
+- **Help:** the domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
+
+- **Filters:** Create filtered visualizations to show only a selected group of domains in maps and networks, with `Corpus.set_sample()` or with the `xb_selection` parameter to `domain_network()`.
 
-- The domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
+- **Filtered chaining**: With `Corpus.set_sample()`, perform selective chaining, whereby a domain-chained model is fit by considering only a selected group of domains, instead of the entire corpus, in order to understand the local associations of metadata dimensions.
 
-- Create filtered visualisations to show only a selected group of domains in maps and networks.
+- **Complex chaining**: Calls to `Corpus.set_chain()` may pass in the `matcher` parameter a path to a `.json` file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
 
-- Perform selective chaining, whereby a domain-chanied model is fit by considering only a selected group of domains, instead of to the entire corpus, in order to understand the local insertion of metadata dimensions.
+- **Better network map**: An entirely new network map function with many improvements and new features is under development and can be tried from `from sashimi.blocks.better_network_map import network_map`. It will eventually replace the current network map.
 
-- Calls to `Corpus.set_chain` may pass in the `matcher` parameter a path to a json file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
+<div align="center">
+<img
+  alt="Domain-authors network"
+  src="https://docs.cortext.net/wp-content/uploads/Image-2.png"
+  width="50%">
+</div>
 
 Development
 -----------
 
 This module provides four main classes:
 
 `class Corpus`
 
-Provides loading and preprocessing corpora, plus some descriptive statistics.
+Methods to load and preprocess corpora, plus some descriptive statistics.
 
 `class GraphModels` (user-facing class, inherits Corpus and Blocks)
 
-Provides Stochastic Block Models of corpora from their document-term and document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
+Methods to fit Stochastic Block Models to corpora through either document-term or document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
 
 `class Blocks`
 
-Provides interactive domain maps, networks, tables, and other interfaces.
+Methods to build interactive domain maps, networks, tables, and other interfaces.
 
-`class Vectorology` [currently deprecated]
+`class VectorModels` [currently deprecated]
 
-Provides models of corpora using word embedding and produces reports, statistics and visualisations.
+Methods to fit word embedding models to corpora and produce reports, statistics and visualizations.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sashimi_domains-0.9.4/pyproject.toml` & `sashimi_domains-0.9.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sashimi-domains"
-description = 'Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual and metadata structures and shifts, by employing stochastic block modeling (SBM) from graph-tool or [currently deprecated] word embedding from Gensim.'
+description = "`sashimi` is a Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently deprecated) word embedding from `gensim`."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "Ale Abdo", email = "abdo@member.fsf.org" },
 ]
 classifiers = [
-  "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Topic :: Sociology",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Visualization",
 ]
 dependencies = [
```

### Comparing `sashimi_domains-0.9.4/PKG-INFO` & `sashimi_domains-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: sashimi-domains
-Version: 0.9.4
-Summary: Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual and metadata structures and shifts, by employing stochastic block modeling (SBM) from graph-tool or [currently deprecated] word embedding from Gensim.
+Version: 0.9.6
+Summary: `sashimi` is a Python module for mixed-methods qualitative studies of large textual or symbolic corpora, providing applications of statistical models accompanied by tailored interactive visualizations. It affords the detection of both textual and metadata structures by employing stochastic block modeling (SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently deprecated) word embedding from `gensim`.
 Project-URL: Documentation, https://gitlab.com/solstag/sashimi/
 Project-URL: Issues, https://gitlab.com/solstag/sashimi/-/issues
 Project-URL: Source, https://gitlab.com/solstag/sashimi/
 Author-email: Ale Abdo <abdo@member.fsf.org>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Requires-Python: >=3.8
 Requires-Dist: bokeh
 Requires-Dist: colorcet
@@ -22,60 +22,66 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: spacy
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-# Sashimi - study the organisation and evolution of corpora
+# Sashimi — study the organization and evolution of corpora
 
-Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations
-for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual
-and metadata structures and shifts, by employing stochastic block modeling (SBM) from [graph-tool](https://graph-tool.skewed.de/) or
-[currently deprecated] word embedding from `Gensim`.
+`sashimi` is a Python module for mixed-methods qualitative studies of large
+textual or symbolic corpora, providing applications of statistical models
+accompanied by tailored interactive visualizations. It affords the detection of
+both textual and metadata structures by employing stochastic block modeling
+(SBM) from [`graph-tool`](https://graph-tool.skewed.de/) or (currently
+deprecated) word embedding from `gensim`.
 
-Models:
+### Statistical models
 - Domain-topic models
-- Domain-chained (metadata) models
-
-Model-based data interfaces (visualisations):
-- Interactive domain-topic maps and domain-chained maps
-- Domain-topic tables and domain-chained tables
-- Domain-topic, domain-chained and domain-topic-chained networks
-- Area rank charts (bump charts) of the evolution of domain sizes
-
-<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-10-56-41.png" width="50%">
-
-## Using Sashimi without programming (no code)
-
-Sashimi is available as a suite of methods in the [Cortext Manager](https://docs.cortext.net/) web service. See [SASHIMI](https://docs.cortext.net/sashimi/).
-
-## Savoring Sashimi
-Also for users of this library, the [documentation](https://docs.cortext.net/sashimi/) at Cortext serves as a good introduction to the methodology.
+  - Synthesizes document clustering (domain modeling) and topic modeling (term clustering).
+- Domain-chained models
+  - Extrapolates modeled domains to partition other dimensions of the corpus such as time, people, institutions, categories or places.
+
+### Human model-data interfaces
+- Domain maps
+  - An interactive HTML document to explore the corpus and its clusters, enhanced with histograms and a search function.
+- Domain tables
+  - Ideal for systematic annotation of clusters.
+- Domain networks
+  - To visualize relations between domains, topics and clusters of other dimensions.
+- Area rank charts
+  - Beautiful "bump charts" displaying the evolution of domains.
+
+<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Image-1.png" width="50%">
+
+## Eat in: "no code" usage
+
+Much of the functionality of `sashimi` is available as a suite of methods in the [Cortext
+Manager](https://docs.cortext.net/) web service. See their documentation for
+[SASHIMI](https://docs.cortext.net/sashimi/), which may also serve users of the Python module as an introduction to the methodology.
 
 ## Installation
 
-Install [graph-tool](https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions) according to your system.
+You must first ~~sharpen your knife~~ install `graph-tool` by following the [installation instructions](https://graph-tool.skewed.de/installation.html) according to your system.
 
 Then:
 
 `pip install sashimi-domains`
 
 ### Dependencies
 
+With the exception of graph-tool, dependencies will be automatically installed by `pip`.
+
 This project builds mainly on the following others:
-- [graph-tool](graph-tool.skewed.de/) (for Stochastic Block Model inference)
-- [pandas](https://pandas.pydata.org/)
+- [graph-tool](graph-tool.skewed.de/) (for stochastic block model inference)
+- [pandas](https://pandas.pydata.org/) (for tabular data manipulation)
 - [spacy](https://spacy.io/) (for tokenization)
-- [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
-- [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
-- [lxml](https://lxml.de/) (for building domain tables)
-- [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
-
-With the exception of graph-tool, dependencies will be automatically installed by `pip`.
+- [gensim](https://radimrehurek.com/gensim/) (for n-gram detection)
+- [bokeh](https://bokeh.org/) (for building interactive maps and plots)
+- [lxml](https://lxml.de/) (for building HTML documents)
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
 import pandas as pd
 
@@ -100,18 +106,18 @@
 ```python
 # Set the data column labels for text sources
 corpus.text_sources = ["title", "body"]
 
 # Set up how to process text sources, for example:
 text_sources_args = dict(ngrams=3, language="en", stop_words=True)
 ```
-The `language` is any valid `spacy` language, where `None` will use the English tokenizer with no stop_words. Our English tokenizer is slightly improved from spacy's original, in order to get ["hot-dog"] out of "hot-dog" (when spacy would split that), ["this", "that"] out of "this/that", and ["citation"] out of "citation[2,3]".
+The `language` is any valid language for `spacy`, where `None` will use the English tokenizer with no stop_words. Our English tokenizer is slightly improved from `spacy`'s original, in order to get ["hot-dog"] out of "hot-dog" (when spacy would split that), ["this", "that"] out of "this/that", and ["citation"] out of "citation[2,3]".
 
 #### Token data
-You may also directly use tokens that you've processed yourself, or from token data such as keywords, categories, or anything really, in addition or in place of textual data.
+You may also directly use tokens that you have processed yourself, or from token data such as keywords, categories, or anything really, in addition or in place of textual data.
 ```python
 # Set the data column labels for token sources
 corpus.token_sources = ["keyword", "category"]
 ```
 
 Token data for a document is expected to be in the form of a list, containing strings or lists containing strings: `List[str | List[str]]`. If your data differs, you must adjust it before processing.
 
@@ -175,37 +181,46 @@
 corpus.domain_network(doc_level=2, ter_level=1, ext_level=1, edges="common")
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ext")
 ```
 
 <img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-11-02-16.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
 
-## Advanced usages
+## Advanced usage
+
+- **Help:** the domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
+
+- **Filters:** Create filtered visualizations to show only a selected group of domains in maps and networks, with `Corpus.set_sample()` or with the `xb_selection` parameter to `domain_network()`.
 
-- The domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
+- **Filtered chaining**: With `Corpus.set_sample()`, perform selective chaining, whereby a domain-chained model is fit by considering only a selected group of domains, instead of the entire corpus, in order to understand the local associations of metadata dimensions.
 
-- Create filtered visualisations to show only a selected group of domains in maps and networks.
+- **Complex chaining**: Calls to `Corpus.set_chain()` may pass in the `matcher` parameter a path to a `.json` file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
 
-- Perform selective chaining, whereby a domain-chanied model is fit by considering only a selected group of domains, instead of to the entire corpus, in order to understand the local insertion of metadata dimensions.
+- **Better network map**: An entirely new network map function with many improvements and new features is under development and can be tried from `from sashimi.blocks.better_network_map import network_map`. It will eventually replace the current network map.
 
-- Calls to `Corpus.set_chain` may pass in the `matcher` parameter a path to a json file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
+<div align="center">
+<img
+  alt="Domain-authors network"
+  src="https://docs.cortext.net/wp-content/uploads/Image-2.png"
+  width="50%">
+</div>
 
 Development
 -----------
 
 This module provides four main classes:
 
 `class Corpus`
 
-Provides loading and preprocessing corpora, plus some descriptive statistics.
+Methods to load and preprocess corpora, plus some descriptive statistics.
 
 `class GraphModels` (user-facing class, inherits Corpus and Blocks)
 
-Provides Stochastic Block Models of corpora from their document-term and document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
+Methods to fit Stochastic Block Models to corpora through either document-term or document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
 
 `class Blocks`
 
-Provides interactive domain maps, networks, tables, and other interfaces.
+Methods to build interactive domain maps, networks, tables, and other interfaces.
 
-`class Vectorology` [currently deprecated]
+`class VectorModels` [currently deprecated]
 
-Provides models of corpora using word embedding and produces reports, statistics and visualisations.
+Methods to fit word embedding models to corpora and produce reports, statistics and visualizations.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


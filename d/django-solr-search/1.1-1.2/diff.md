# Comparing `tmp/django_solr_search-1.1-py3-none-any.whl.zip` & `tmp/django_solr_search-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 20537 bytes, number of entries: 21
+Zip file size: 21273 bytes, number of entries: 21
 -rw-r--r--  2.0 unx       54 b- defN 20-Feb-02 00:00 django_solr/__init__.py
 -rw-r--r--  2.0 unx     4506 b- defN 20-Feb-02 00:00 django_solr/admin.py
 -rw-r--r--  2.0 unx      183 b- defN 20-Feb-02 00:00 django_solr/apps.py
 -rw-r--r--  2.0 unx      864 b- defN 20-Feb-02 00:00 django_solr/models.py
 -rw-r--r--  2.0 unx      179 b- defN 20-Feb-02 00:00 django_solr/urls.py
 -rw-r--r--  2.0 unx     1546 b- defN 20-Feb-02 00:00 django_solr/views.py
 -rw-r--r--  2.0 unx     3389 b- defN 20-Feb-02 00:00 django_solr/django_solr/templates/index_list.html
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 django_solr/dsl/__init__.py
--rw-r--r--  2.0 unx    16397 b- defN 20-Feb-02 00:00 django_solr/dsl/backend.py
+-rw-r--r--  2.0 unx    18350 b- defN 20-Feb-02 00:00 django_solr/dsl/backend.py
 -rw-r--r--  2.0 unx      121 b- defN 20-Feb-02 00:00 django_solr/dsl/exception.py
 -rw-r--r--  2.0 unx     6054 b- defN 20-Feb-02 00:00 django_solr/dsl/fields.py
--rw-r--r--  2.0 unx    10573 b- defN 20-Feb-02 00:00 django_solr/dsl/indexes.py
+-rw-r--r--  2.0 unx    10597 b- defN 20-Feb-02 00:00 django_solr/dsl/indexes.py
 -rw-r--r--  2.0 unx     1290 b- defN 20-Feb-02 00:00 django_solr/migrations/0001_initial.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 django_solr/migrations/__init__.py
 -rw-r--r--  2.0 unx     3273 b- defN 20-Feb-02 00:00 django_solr/templates/admin/change_list.html
 -rw-r--r--  2.0 unx      399 b- defN 20-Feb-02 00:00 django_solr/templates/admin/django_solr/indexes/change_list.html
 -rw-r--r--  2.0 unx      531 b- defN 20-Feb-02 00:00 django_solr/templates/django_solr/index_list.html
-?rw-r--r--  2.0 unx     1200 b- defN 20-Feb-02 00:00 django_solr_search-1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 django_solr_search-1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1074 b- defN 20-Feb-02 00:00 django_solr_search-1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1828 b- defN 20-Feb-02 00:00 django_solr_search-1.1.dist-info/RECORD
-21 files, 53548 bytes uncompressed, 17521 bytes compressed:  67.3%
+?rw-r--r--  2.0 unx     1515 b- defN 20-Feb-02 00:00 django_solr_search-1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 django_solr_search-1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1074 b- defN 20-Feb-02 00:00 django_solr_search-1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1828 b- defN 20-Feb-02 00:00 django_solr_search-1.2.dist-info/RECORD
+21 files, 55840 bytes uncompressed, 18257 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: django_solr/templates/admin/django_solr/indexes/change_list.html
 Comment: 
 
 Filename: django_solr/templates/django_solr/index_list.html
 Comment: 
 
-Filename: django_solr_search-1.1.dist-info/METADATA
+Filename: django_solr_search-1.2.dist-info/METADATA
 Comment: 
 
-Filename: django_solr_search-1.1.dist-info/WHEEL
+Filename: django_solr_search-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_solr_search-1.1.dist-info/licenses/LICENSE
+Filename: django_solr_search-1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: django_solr_search-1.1.dist-info/RECORD
+Filename: django_solr_search-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_solr/dsl/backend.py

```diff
@@ -1,7 +1,9 @@
+import ast
+import datetime
 import time
 from http.client import HTTPException
 from typing import List, Tuple, Union
 
 import requests
 from django.utils.encoding import force_str
 from haystack.backends import SQ
@@ -10,24 +12,24 @@
     SolrSearchBackend,
     SolrSearchQuery,
 )
 from haystack.constants import DEFAULT_ALIAS, DOCUMENT_FIELD
 from haystack.exceptions import NotHandled
 from haystack.models import SearchResult
 from haystack.query import SearchQuerySet
-from pysolr import Solr, SolrError, force_bytes, force_unicode
+from pysolr import DATETIME_REGEX, IS_PY3, Solr, SolrError, force_bytes, force_unicode
 
 from django_solr.models import EmptySearchResult
 
 from .fields import NestedField
 
 MAX_LOG_LENGTH = 25000
 
 
-class LogSolr(Solr):
+class DjangoSolr(Solr):
     def _send_request(self, method, path="", body=None, headers=None, files=None):
         url = self._create_full_url(path)
         method = method.lower()
         log_body = body
 
         if headers is None:
             headers = {}
@@ -106,19 +108,77 @@
                     }
                 },
             )
             raise SolrError(error_message % (resp.status_code, solr_message))
 
         return force_unicode(resp.content)
 
+    def _to_python(self, value):
+        """
+        Converts values from Solr to native Python values.
+        """
+        if isinstance(value, (int, float, complex)):
+            return value
+
+        if isinstance(value, (list, tuple)):
+            result = [self._to_python(v) for v in value]
+            if isinstance(value, tuple):
+                result = tuple(result)
+            return result
+
+        if value == "true":
+            return True
+        elif value == "false":
+            return False
+
+        is_string = False
+
+        if IS_PY3:
+            if isinstance(value, bytes):
+                value = force_unicode(value)
+
+            if isinstance(value, str):
+                is_string = True
+        else:
+            if isinstance(value, str):
+                value = force_unicode(value)
+
+        if is_string:
+            possible_datetime = DATETIME_REGEX.search(value)
+
+            if possible_datetime:
+                date_values = possible_datetime.groupdict()
+
+                for dk, dv in date_values.items():
+                    date_values[dk] = int(dv)
+
+                return datetime.datetime(
+                    date_values["year"],
+                    date_values["month"],
+                    date_values["day"],
+                    date_values["hour"],
+                    date_values["minute"],
+                    date_values["second"],
+                )
+
+        try:
+            # This is slightly gross but it's hard to tell otherwise what the
+            # string's original type might have been.
+            return ast.literal_eval(value)
+        except (ValueError, SyntaxError):
+            # If it fails, continue on.
+            pass
+
+        return value
+
 
 class ProjectSolrSearchBackend(SolrSearchBackend):
     def __init__(self, connection_alias, **connection_options):
         super().__init__(connection_alias, **connection_options)
-        self.conn = LogSolr(connection_options["URL"], timeout=self.timeout, **connection_options.get("KWARGS", {}))
+        self.conn = DjangoSolr(connection_options["URL"], timeout=self.timeout, **connection_options.get("KWARGS", {}))
 
     TYPE_MAP = {
         "date": "pdate",
         "datetime": "pdate",
         "integer": "plong",
     }
 
@@ -385,14 +445,15 @@
 
 class EMPTY:
     pass
 
 
 class ParentSQ(SQ):
     def __init__(self, **kwargs):
+        self.exclude = kwargs.pop("exclude", False)
         super().__init__(**kwargs)
         self._full_path = EMPTY
         self._path = EMPTY
         self._value = EMPTY
         self._key = EMPTY
         if self.children:
             self._parse_args()
@@ -430,13 +491,16 @@
         return self._key
 
     def _repr_query_fragment_callback(self, field, filter_type, value):
         parent = '{!parent which="*:* -_nest_path_:*"}'
         nest_path = f"/{self.key}" if self.path == "/" else self.path
         queries = [f'+_nest_path_:"{nest_path}"']  # noqa E231
         if value:
-            queries.append(f"+{field}:({force_str(value)})")  # noqa E231
+            if self.exclude:
+                queries.append(f"-{field}:({force_str(value)})")  # noqa E231
+            else:
+                queries.append(f"+{field}:({force_str(value)})")  # noqa E231
         query = " ".join(queries)
         return f"{parent} ({query})"
 
     def as_query_string(self, *args, **kwargs):
         return self._repr_query_fragment_callback(self.key, self.connector, self.value)
```

## django_solr/dsl/indexes.py

```diff
@@ -1,11 +1,11 @@
 from django.db import models as django_models
 from django.db.models.fields import NOT_PROVIDED as DJANGO_NOT_PROVIDED
 from haystack.constants import DJANGO_ID, DOCUMENT_FIELD, ID
-from haystack.indexes import SearchIndex
+from haystack.indexes import Indexable, SearchIndex  # noqa F401
 
 from .backend import SolrSearchQuerySet
 from .exception import MultipleResultError, NotFoundError
 from .fields import NestedField, TextGeneralField
 
 
 class SolrDocument(SearchIndex):
```

## Comparing `django_solr_search-1.1.dist-info/licenses/LICENSE` & `django_solr_search-1.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `django_solr_search-1.1.dist-info/RECORD` & `django_solr_search-1.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 django_solr/admin.py,sha256=GFVUgL_1mkHBERncHezs26B4Xi9CkFH-L4Q7rE4YeJA,4506
 django_solr/apps.py,sha256=GXO3IVUYfwYip7H4632DFAM3pgjZZTNGER8hhEqImxo,183
 django_solr/models.py,sha256=NHd3RTUDzuKfza8Ea4CqSffzabc-sPky414rWowS1Vg,864
 django_solr/urls.py,sha256=dRHuNA8DObU29iCh3dtbdNA7N7m0oiVdHugArtYXf4k,179
 django_solr/views.py,sha256=LCDoVhbhCEokj_4fpU5oclUD0GIy4zgcVrxwIyZa9a8,1546
 django_solr/django_solr/templates/index_list.html,sha256=ZOyFUKwIZoWAJrQG-PtZy_hg2zmZ9oY0Od7HnwQaLMY,3389
 django_solr/dsl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_solr/dsl/backend.py,sha256=8D9opp0nQzNCVhOEUmVm2LufP-QIL1LisZZkzZEbqWQ,16397
+django_solr/dsl/backend.py,sha256=UnMq9GinyQwwLeIndCsBO7fkytVwMg1YfuQHXnrvnkI,18350
 django_solr/dsl/exception.py,sha256=GBFsMHGsBI07HN1ZBFbpB-cRS8a8cEZU5_3eKWMWolg,121
 django_solr/dsl/fields.py,sha256=JduF3sxRfvKwKCnrEhQfqbAzTtdTfpXxXqly3iowmIs,6054
-django_solr/dsl/indexes.py,sha256=m2QLqRk6DRpdXtAlSFLYKHmScVL295D3OnTqXdNhRLY,10573
+django_solr/dsl/indexes.py,sha256=TW330Voq00RTU2JHjwHsRp-zIq08Sw-8WBIxRzMFqlM,10597
 django_solr/migrations/0001_initial.py,sha256=u7NZYNxQxmiRXucgYqe0Acvr1WeqRYu9abCZGYRXvVQ,1290
 django_solr/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_solr/templates/admin/change_list.html,sha256=JP4rXbR8vRzls00JtYjRihiTR48NNAD6ZwJ4Lbg6pR8,3273
 django_solr/templates/admin/django_solr/indexes/change_list.html,sha256=RpsUJrOHVQPKtXU7mDjdd5s8JDlIDnk_LbZgnbVkB8M,399
 django_solr/templates/django_solr/index_list.html,sha256=HXJGQ_5TvcMvvB8ZAUTMExCOp8bi08Liqmv8V0TFBAU,531
-django_solr_search-1.1.dist-info/METADATA,sha256=e6a_x7tq1fIaSfnlS1hEO-5ZYrQ33qjZoHcFB_ttK9Y,1200
-django_solr_search-1.1.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-django_solr_search-1.1.dist-info/licenses/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-django_solr_search-1.1.dist-info/RECORD,,
+django_solr_search-1.2.dist-info/METADATA,sha256=Rv7UnZVXbOHBOzy70T5aXdjIUL2B6QmiRhjuF69arMg,1515
+django_solr_search-1.2.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+django_solr_search-1.2.dist-info/licenses/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+django_solr_search-1.2.dist-info/RECORD,,
```


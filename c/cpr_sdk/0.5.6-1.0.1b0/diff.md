# Comparing `tmp/cpr_sdk-0.5.6.tar.gz` & `tmp/cpr_sdk-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpr_sdk-0.5.6.tar", max compression
+gzip compressed data, was "cpr_sdk-1.0.1b0.tar", max compression
```

## Comparing `cpr_sdk-0.5.6.tar` & `cpr_sdk-1.0.1b0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     6189 2024-04-03 09:56:37.652945 cpr_sdk-0.5.6/README.md
--rw-r--r--   0        0        0     2334 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/__init__.py
--rw-r--r--   0        0        0     5693 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/data_adaptors.py
--rw-r--r--   0        0        0     1118 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/embedding.py
--rw-r--r--   0        0        0      797 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/exceptions.py
--rw-r--r--   0        0        0    50630 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/models/__init__.py
--rw-r--r--   0        0        0    11754 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/models/search.py
--rw-r--r--   0        0        0    12721 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/parser_models.py
--rw-r--r--   0        0        0     2679 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/pipeline_general_models.py
--rw-r--r--   0        0        0    71013 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/resources/sensitive_query_terms.tsv
--rw-r--r--   0        0        0     2791 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/s3.py
--rw-r--r--   0        0        0     4584 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/search_adaptors.py
--rw-r--r--   0        0        0     4044 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/utils.py
--rw-r--r--   0        0        0     6979 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/vespa.py
--rw-r--r--   0        0        0     6732 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/yql_builder.py
--rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 cpr_sdk-0.5.6/setup.py
--rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 cpr_sdk-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-04 08:43:53.717755 cpr_sdk-1.0.1b0/LICENSE
+-rw-r--r--   0        0        0     6189 2024-04-04 08:21:44.786349 cpr_sdk-1.0.1b0/README.md
+-rw-r--r--   0        0        0     3399 2024-04-04 15:41:04.459661 cpr_sdk-1.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-04 08:43:53.718256 cpr_sdk-1.0.1b0/src/cpr_sdk/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-04 08:21:44.787454 cpr_sdk-1.0.1b0/src/cpr_sdk/data_adaptors.py
+-rw-r--r--   0        0        0     1118 2024-04-04 08:21:44.787610 cpr_sdk-1.0.1b0/src/cpr_sdk/embedding.py
+-rw-r--r--   0        0        0      797 2024-04-04 08:21:44.787736 cpr_sdk-1.0.1b0/src/cpr_sdk/exceptions.py
+-rw-r--r--   0        0        0    50630 2024-04-04 08:21:44.788829 cpr_sdk-1.0.1b0/src/cpr_sdk/models/__init__.py
+-rw-r--r--   0        0        0    11979 2024-04-04 08:36:18.478495 cpr_sdk-1.0.1b0/src/cpr_sdk/models/search.py
+-rw-r--r--   0        0        0    12721 2024-04-04 08:21:44.789706 cpr_sdk-1.0.1b0/src/cpr_sdk/parser_models.py
+-rw-r--r--   0        0        0     2679 2024-04-04 08:21:44.789891 cpr_sdk-1.0.1b0/src/cpr_sdk/pipeline_general_models.py
+-rw-r--r--   0        0        0    71013 2024-04-04 08:21:44.790397 cpr_sdk-1.0.1b0/src/cpr_sdk/resources/sensitive_query_terms.tsv
+-rw-r--r--   0        0        0     2791 2024-04-04 08:21:44.790575 cpr_sdk-1.0.1b0/src/cpr_sdk/s3.py
+-rw-r--r--   0        0        0     4584 2024-04-04 08:21:44.791101 cpr_sdk-1.0.1b0/src/cpr_sdk/search_adaptors.py
+-rw-r--r--   0        0        0     4143 2024-04-04 08:36:18.478881 cpr_sdk-1.0.1b0/src/cpr_sdk/utils.py
+-rw-r--r--   0        0        0      169 2024-04-04 12:13:54.393379 cpr_sdk-1.0.1b0/src/cpr_sdk/version.py
+-rw-r--r--   0        0        0     6979 2024-04-04 08:21:44.791948 cpr_sdk-1.0.1b0/src/cpr_sdk/vespa.py
+-rw-r--r--   0        0        0     7015 2024-04-04 08:36:18.479372 cpr_sdk-1.0.1b0/src/cpr_sdk/yql_builder.py
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 cpr_sdk-1.0.1b0/PKG-INFO
```

### Comparing `cpr_sdk-0.5.6/README.md` & `cpr_sdk-1.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/data_adaptors.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/data_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/embedding.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/embedding.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/exceptions.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/models/__init__.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/models/search.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
 class SearchParameters(BaseModel):
     """Parameters for a search request"""
 
     query_string: Optional[str] = ""
     exact_match: bool = False
     all_results: bool = False
+    documents_only: bool = False
     limit: int = Field(ge=0, default=100)
     max_hits_per_family: int = Field(
         validation_alias=AliasChoices("max_passages_per_doc", "max_hits_per_family"),
         default=10,
         ge=0,
     )
 
@@ -93,14 +94,18 @@
     continuation_tokens: Optional[Sequence[str]] = None
 
     @model_validator(mode="after")
     def validate(self):
         """Validate against mutually exclusive fields"""
         if self.exact_match and self.all_results:
             raise QueryError("`exact_match` and `all_results` are mutually exclusive")
+        if self.documents_only and not self.all_results:
+            raise QueryError(
+                "`documents_only` requires `all_results`, other queries are not supported"
+            )
         return self
 
     @field_validator("continuation_tokens")
     def continuation_tokens_must_be_upper_strings(cls, continuation_tokens):
         """Validate continuation_tokens match the expected format"""
         if not continuation_tokens:
             return continuation_tokens
```

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/parser_models.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/parser_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/pipeline_general_models.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/pipeline_general_models.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/resources/sensitive_query_terms.tsv` & `cpr_sdk-1.0.1b0/src/cpr_sdk/resources/sensitive_query_terms.tsv`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/s3.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/s3.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/search_adaptors.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/search_adaptors.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/utils.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,23 @@
     This updated version builds on the above to avoid a loophole where a string of
     sensitive terms can be incorrectly flagged as not being sensitive. This happens
     because it is the shortest sensitive term that is compared to the rest of the
     query, and the rest of the query at that point can contain other sensitive terms.
 
     """
     sensitive_terms_in_query = [
-        term
-        for term in sensitive_terms
-        if re.findall(r"\b" + re.escape(term) + r"\b", text.lower())
+        term for term in sensitive_terms if re.findall(term, text.lower())
     ]
 
     if sensitive_terms_in_query:
-        shortest_sensitive_term = min(sensitive_terms_in_query, key=len)
+        terms = [term.pattern.strip("\\b") for term in sensitive_terms_in_query]
+        shortest_sensitive_term = min(terms, key=len)
         shortest_sensitive_word_count = len(shortest_sensitive_term.split(" "))
-
         remaining_sensitive_word_count = sum(
-            [
-                len(term.split())
-                for term in sensitive_terms_in_query
-                if term != shortest_sensitive_term
-            ]
+            [len(term.split()) for term in terms if term != shortest_sensitive_term]
         )
 
         query_word_count = len(text.split())
         remaining_query_word_count = query_word_count - remaining_sensitive_word_count
 
         if remaining_query_word_count <= 0:
             return True
@@ -50,29 +44,31 @@
         )
         if proportion_sensitive >= 0.5:
             return True
 
     return False
 
 
-def load_sensitive_query_terms() -> set[str]:
+def load_sensitive_query_terms() -> set[re.Pattern]:
     """
     Return sensitive query terms from the first column of a TSV file.
 
     Outputs are lowercased for case-insensitive matching.
 
     :return [set[str]]: sensitive query terms
     """
     tsv_path = Path(__file__).parent / "resources" / "sensitive_query_terms.tsv"
     with open(tsv_path, "r") as tsv_file:
         reader = csv.DictReader(tsv_file, delimiter="\t")
-
-        sensitive_terms = set([row["keyword"].lower().strip() for row in reader])
-
-    return sensitive_terms
+        sensitive_terms = []
+        for row in reader:
+            keyword = row["keyword"].lower().strip()
+            keyword_regex = re.compile(r"\b" + re.escape(keyword) + r"\b")
+            sensitive_terms.append(keyword_regex)
+    return set(sensitive_terms)
 
 
 def dig(obj: Union[list, dict], *fields: Any, default: Any = None) -> Any:
     """
     An interface for retrieving data from complicated objects
 
     Behaviour is to return the default if the path is invalid thereby avoiding errors
```

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/vespa.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/vespa.py`

 * *Files identical despite different names*

### Comparing `cpr_sdk-0.5.6/src/cpr_sdk/yql_builder.py` & `cpr_sdk-1.0.1b0/src/cpr_sdk/yql_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class YQLBuilder:
     """Used to assemble yql queries"""
 
     yql_base = Template(
         """
-        select * from sources family_document, document_passage
+        select * from sources $SOURCES
             where $WHERE_CLAUSE
         limit 0 
         |
             $CONTINUATION
         all(
             group(family_import_id)
             output(count())
@@ -32,14 +32,21 @@
     """
     )
 
     def __init__(self, params: SearchParameters, sensitive: bool = False) -> None:
         self.params = params
         self.sensitive = sensitive
 
+    def build_sources(self) -> str:
+        """Creates the part of the query that determines which sources to search"""
+        if self.params.documents_only:
+            return "family_document"
+        else:
+            return "family_document, document_passage"
+
     def build_search_term(self) -> str:
         """Create the part of the query that matches a users search text"""
         if self.params.all_results:
             return "( true )"
         if self.params.exact_match:
             return """
                 (
@@ -154,14 +161,15 @@
     def build_max_hits_per_family(self) -> int:
         """Create the part of the query limiting passages within a family returned"""
         return self.params.max_hits_per_family
 
     def to_str(self) -> str:
         """Assemble the yql from parts using the template"""
         yql = self.yql_base.substitute(
+            SOURCES=self.build_sources(),
             WHERE_CLAUSE=self.build_where_clause(),
             CONTINUATION=self.build_continuation(),
             LIMIT=self.build_limit(),
             SORT=self.build_sort(),
             MAX_HITS_PER_FAMILY=self.build_max_hits_per_family(),
         )
         return " ".join(yql.split())
```

### Comparing `cpr_sdk-0.5.6/PKG-INFO` & `cpr_sdk-1.0.1b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
-Name: cpr-sdk
-Version: 0.5.6
+Name: cpr_sdk
+Version: 1.0.1b0
 Summary: 
+License: LICENSE
 Author: CPR Tech
 Author-email: tech@climatepolicyradar.org
 Requires-Python: >=3.9,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: spacy
 Provides-Extra: vespa
 Requires-Dist: aws-error-utils (>=2.7.0,<3.0.0)
 Requires-Dist: boto3 (>=1.26.16,<2.0.0)
 Requires-Dist: datasets (>=2.14.0,<3.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
```


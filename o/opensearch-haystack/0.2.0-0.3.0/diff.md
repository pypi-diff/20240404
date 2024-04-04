# Comparing `tmp/opensearch_haystack-0.2.0.tar.gz` & `tmp/opensearch_haystack-0.3.0.tar.gz`

## Comparing `opensearch_haystack-0.2.0.tar` & `opensearch_haystack-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/docker-compose.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/document_stores/opensearch/__init__.py
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/document_stores/opensearch/document_store.py
--rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/src/haystack_integrations/document_stores/opensearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    15570 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/LICENSE
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/README.md
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 opensearch_haystack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/docker-compose.yml
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/pydoc/config.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/__init__.py
+-rw-r--r--   0        0        0    13587 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/document_store.py
+-rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/LICENSE
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/README.md
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/PKG-INFO
```

### Comparing `opensearch_haystack-0.2.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py` & `opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,25 +42,40 @@
         self._filters = filters or {}
         self._fuzziness = fuzziness
         self._top_k = top_k
         self._scale_score = scale_score
         self._all_terms_must_match = all_terms_must_match
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             filters=self._filters,
             fuzziness=self._fuzziness,
             top_k=self._top_k,
             scale_score=self._scale_score,
             document_store=self._document_store.to_dict(),
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "OpenSearchBM25Retriever":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+
+        :returns:
+            Deserialized component.
+        """
         data["init_parameters"]["document_store"] = OpenSearchDocumentStore.from_dict(
             data["init_parameters"]["document_store"]
         )
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
@@ -78,15 +93,19 @@
         :param query: The query string
         :param filters: Optional filters to narrow down the search space.
         :param all_terms_must_match: If True, all terms in the query string must be present in the retrieved documents.
         :param top_k: Maximum number of Documents to return.
         :param fuzziness: Fuzziness parameter for full-text queries.
         :param scale_score: Whether to scale the score of retrieved documents between 0 and 1.
             This is useful when comparing documents across different indexes.
-        :return: A dictionary containing the retrieved documents.
+
+        :returns:
+            A dictionary containing the retrieved documents with the following structure:
+            - documents: List of retrieved Documents.
+
         """
         if filters is None:
             filters = self._filters
         if all_terms_must_match is None:
             all_terms_must_match = self._all_terms_must_match
         if top_k is None:
             top_k = self._top_k
```

### Comparing `opensearch_haystack-0.2.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py` & `opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,37 +37,54 @@
             raise ValueError(msg)
 
         self._document_store = document_store
         self._filters = filters or {}
         self._top_k = top_k
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             filters=self._filters,
             top_k=self._top_k,
             document_store=self._document_store.to_dict(),
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "OpenSearchEmbeddingRetriever":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+
+        :returns:
+            Deserialized component.
+        """
         data["init_parameters"]["document_store"] = OpenSearchDocumentStore.from_dict(
             data["init_parameters"]["document_store"]
         )
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(self, query_embedding: List[float], filters: Optional[Dict[str, Any]] = None, top_k: Optional[int] = None):
         """
         Retrieve documents using a vector similarity metric.
 
         :param query_embedding: Embedding of the query.
         :param filters: Optional filters to narrow down the search space.
         :param top_k: Maximum number of Documents to return.
-        :return: List of Document similar to `query_embedding`.
+        :returns:
+            Dictionary with key "documents" containing the retrieved Documents.
+            - documents: List of Document similar to `query_embedding`.
         """
         if filters is None:
             filters = self._filters
         if top_k is None:
             top_k = self._top_k
 
         docs = self._document_store._embedding_retrieval(
```

### Comparing `opensearch_haystack-0.2.0/src/haystack_integrations/document_stores/opensearch/document_store.py` & `opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/document_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,17 @@
         hosts: Optional[Hosts] = None,
         index: str = "default",
         **kwargs,
     ):
         """
         Creates a new OpenSearchDocumentStore instance.
 
-        For more information on connection parameters, see the official OpenSearch documentation:
-        https://opensearch.org/docs/latest/clients/python-low-level/#connecting-to-opensearch
+        For more information on connection parameters, see the [official OpenSearch documentation](https://opensearch.org/docs/latest/clients/python-low-level/#connecting-to-opensearch)
 
-        For the full list of supported kwargs, see the official OpenSearch reference:
-        https://opensearch-project.github.io/opensearch-py/api-ref/clients/opensearch_client.html
+        For the full list of supported kwargs, see the [official OpenSearch reference](https://opensearch-project.github.io/opensearch-py/api-ref/clients/opensearch_client.html)
 
         :param hosts: List of hosts running the OpenSearch client. Defaults to None
         :param index: Name of index in OpenSearch, if it doesn't exist it will be created. Defaults to "default"
         :param **kwargs: Optional arguments that ``OpenSearch`` takes.
         """
         self._hosts = hosts
         self._client = OpenSearch(hosts, **kwargs)
@@ -65,15 +63,14 @@
             "properties": {
                 "embedding": {"type": "knn_vector", "index": True, "dimension": embedding_dim},
                 "content": {"type": "text"},
             },
             "dynamic_templates": [
                 {
                     "strings": {
-                        "path_match": "*",
                         "match_mapping_type": "string",
                         "mapping": {
                             "type": "keyword",
                         },
                     }
                 }
             ],
@@ -90,23 +87,38 @@
         if not self._client.indices.exists(index=index):
             self._client.indices.create(index=index, body=body)
 
     def to_dict(self) -> Dict[str, Any]:
         # This is not the best solution to serialise this class but is the fastest to implement.
         # Not all kwargs types can be serialised to text so this can fail. We must serialise each
         # type explicitly to handle this properly.
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             hosts=self._hosts,
             index=self._index,
             **self._kwargs,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "OpenSearchDocumentStore":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+
+        :returns:
+            Deserialized component.
+        """
         return default_from_dict(cls, data)
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
         """
         return self._client.count(index=self._index)["count"]
@@ -164,14 +176,19 @@
             raise_on_error=False,
         )
 
         if errors:
             duplicate_errors_ids = []
             other_errors = []
             for e in errors:
+                # OpenSearch might not return a correctly formatted error, in that case we
+                # treat it as a generic error
+                if "create" not in e:
+                    other_errors.append(e)
+                    continue
                 error_type = e["create"]["error"]["type"]
                 if policy == DuplicatePolicy.FAIL and error_type == "version_conflict_engine_exception":
                     duplicate_errors_ids.append(e["create"]["_id"])
                 elif policy == DuplicatePolicy.SKIP and error_type == "version_conflict_engine_exception":
                     # when the policy is skip, duplication errors are OK and we should not raise an exception
                     continue
                 else:
@@ -226,30 +243,29 @@
         all_terms_must_match: bool = False,
     ) -> List[Document]:
         """
         OpenSearch by defaults uses BM25 search algorithm.
         Even though this method is called `bm25_retrieval` it searches for `query`
         using the search algorithm `_client` was configured with.
 
-        This method is not mean to be part of the public interface of
+        This method is not meant to be part of the public interface of
         `OpenSearchDocumentStore` nor called directly.
         `OpenSearchBM25Retriever` uses this method directly and is the public interface for it.
 
         `query` must be a non empty string, otherwise a `ValueError` will be raised.
 
         :param query: String to search in saved Documents' text.
         :param filters: Optional filters to narrow down the search space.
-        :param fuzziness: Fuzziness parameter passed to OpenSearch, defaults to "AUTO".
-                          see the official documentation for valid values:
-                          https://www.elastic.co/guide/en/OpenSearch/reference/current/common-options.html#fuzziness
+        :param fuzziness: Fuzziness parameter passed to OpenSearch, defaults to "AUTO". see the official documentation
+                          for valid [fuzziness values](https://www.elastic.co/guide/en/OpenSearch/reference/current/common-options.html#fuzziness)
         :param top_k: Maximum number of Documents to return, defaults to 10
         :param scale_score: If `True` scales the Document`s scores between 0 and 1, defaults to False
         :param all_terms_must_match: If `True` all terms in `query` must be present in the Document, defaults to False
         :raises ValueError: If `query` is an empty string
-        :return: List of Document that match `query`
+        :returns: List of Document that match `query`
         """
 
         if not query:
             msg = "query must be a non empty string"
             raise ValueError(msg)
 
         operator = "AND" if all_terms_must_match else "OR"
@@ -289,28 +305,24 @@
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
     ) -> List[Document]:
         """
         Retrieves documents that are most similar to the query embedding using a vector similarity metric.
         It uses the OpenSearch's Approximate k-Nearest Neighbors search algorithm.
 
-        This method is not mean to be part of the public interface of
+        This method is not meant to be part of the public interface of
         `OpenSearchDocumentStore` nor called directly.
         `OpenSearchEmbeddingRetriever` uses this method directly and is the public interface for it.
 
         :param query_embedding: Embedding of the query.
         :param filters: Filters applied to the retrieved Documents. Defaults to None.
             Filters are applied during the approximate kNN search to ensure that top_k matching documents are returned.
         :param top_k: Maximum number of Documents to return, defaults to 10
-        :param num_candidates: Number of approximate nearest neighbor candidates on each shard. Defaults to top_k * 10.
-            Increasing this value will improve search accuracy at the cost of slower search speeds.
-            You can read more about it in the OpenSearch documentation:
-            https://www.elastic.co/guide/en/OpenSearch/reference/current/knn-search.html#tune-approximate-knn-for-speed-accuracy
         :raises ValueError: If `query_embedding` is an empty list
-        :return: List of Document that are most similar to `query_embedding`
+        :returns: List of Document that are most similar to `query_embedding`
         """
 
         if not query_embedding:
             msg = "query_embedding must be a non-empty list of floats"
             raise ValueError(msg)
 
         body: Dict[str, Any] = {
```

### Comparing `opensearch_haystack-0.2.0/src/haystack_integrations/document_stores/opensearch/filters.py` & `opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/tests/test_bm25_retriever.py` & `opensearch_haystack-0.3.0/tests/test_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/tests/test_document_store.py` & `opensearch_haystack-0.3.0/tests/test_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,42 @@
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 from haystack_integrations.document_stores.opensearch import OpenSearchDocumentStore
 from opensearchpy.exceptions import RequestError
 
 
+@patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
+def test_to_dict(_mock_opensearch_client):
+    document_store = OpenSearchDocumentStore(hosts="some hosts")
+    res = document_store.to_dict()
+    assert res == {
+        "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
+        "init_parameters": {
+            "hosts": "some hosts",
+            "index": "default",
+        },
+    }
+
+
+@patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
+def test_from_dict(_mock_opensearch_client):
+    data = {
+        "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
+        "init_parameters": {
+            "hosts": "some hosts",
+            "index": "default",
+        },
+    }
+    document_store = OpenSearchDocumentStore.from_dict(data)
+    assert document_store._hosts == "some hosts"
+    assert document_store._index == "default"
+
+
+@pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
     """
     Common test cases will be provided by `DocumentStoreBaseTests` but
     you can add more to this class.
     """
 
     @pytest.fixture
@@ -83,39 +111,14 @@
             }
             expected_meta.append(r)
         for doc in received:
             doc.score = None
 
         super().assert_documents_are_equal(received, expected)
 
-    @patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
-    def test_to_dict(self, _mock_opensearch_client):
-        document_store = OpenSearchDocumentStore(hosts="some hosts")
-        res = document_store.to_dict()
-        assert res == {
-            "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
-            "init_parameters": {
-                "hosts": "some hosts",
-                "index": "default",
-            },
-        }
-
-    @patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
-    def test_from_dict(self, _mock_opensearch_client):
-        data = {
-            "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
-            "init_parameters": {
-                "hosts": "some hosts",
-                "index": "default",
-            },
-        }
-        document_store = OpenSearchDocumentStore.from_dict(data)
-        assert document_store._hosts == "some hosts"
-        assert document_store._index == "default"
-
     def test_write_documents(self, document_store: OpenSearchDocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
         with pytest.raises(DuplicateDocumentError):
             document_store.write_documents(docs, DuplicatePolicy.FAIL)
 
     def test_bm25_retrieval(self, document_store: OpenSearchDocumentStore):
@@ -317,7 +320,16 @@
         docs = [
             Document(content="Hello world", embedding=[0.1, 0.2, 0.3, 0.4]),
             Document(content="Hello world", embedding=[0.1, 0.2]),
         ]
 
         with pytest.raises(DocumentStoreError):
             document_store_embedding_dim_4.write_documents(docs)
+
+    @patch("haystack_integrations.document_stores.opensearch.document_store.bulk")
+    def test_write_documents_with_badly_formatted_bulk_errors(self, mock_bulk, document_store):
+        error = {"some_key": "some_value"}
+        mock_bulk.return_value = ([], [error])
+
+        with pytest.raises(DocumentStoreError) as e:
+            document_store.write_documents([Document(content="Hello world")])
+            e.match(f"{error}")
```

### Comparing `opensearch_haystack-0.2.0/tests/test_embedding_retriever.py` & `opensearch_haystack-0.3.0/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/tests/test_filters.py` & `opensearch_haystack-0.3.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/.gitignore` & `opensearch_haystack-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/LICENSE` & `opensearch_haystack-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/README.md` & `opensearch_haystack-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.2.0/pyproject.toml` & `opensearch_haystack-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -45,27 +45,32 @@
 git_describe_command = 'git describe --tags --match="integrations/opensearch-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-xdist",
+  "haystack-pydoc-tools",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
+docs = [
+  "pydoc-markdown pydoc/config.yml"
+]
+
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
@@ -88,20 +93,20 @@
   "typing",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -148,29 +153,29 @@
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
-[tool.coverage.paths]
-opensearch_haystack = ["src/haystack_integrations", "*/opensearch-haystack/src"]
-tests = ["tests", "*/opensearch-haystack/tests"]
 
 [tool.coverage.report]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 markers = [
   "unit: unit tests",
   "integration: integration tests"
 ]
```

### Comparing `opensearch_haystack-0.2.0/PKG-INFO` & `opensearch_haystack-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: opensearch-haystack
-Version: 0.2.0
+Version: 0.3.0
 Summary: Haystack 2.x Document Store for OpenSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch
 Author-email: deepset <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```


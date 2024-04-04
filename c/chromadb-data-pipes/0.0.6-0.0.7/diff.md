# Comparing `tmp/chromadb_data_pipes-0.0.6.tar.gz` & `tmp/chromadb_data_pipes-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb_data_pipes-0.0.6.tar", max compression
+gzip compressed data, was "chromadb_data_pipes-0.0.7.tar", max compression
```

## Comparing `chromadb_data_pipes-0.0.6.tar` & `chromadb_data_pipes-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1077 2024-01-30 13:46:25.010225 chromadb_data_pipes-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     4852 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/README.md
--rw-r--r--   0        0        0     1989 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/chroma/__init__.py
--rw-r--r--   0        0        0     5340 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/chroma/chroma_export.py
--rw-r--r--   0        0        0     5296 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/chroma/chroma_import.py
--rw-r--r--   0        0        0    15476 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/huggingface/__init__.py
--rw-r--r--   0        0        0     1798 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/huggingface/utils.py
--rw-r--r--   0        0        0     2821 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/main.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/__init__.py
--rw-r--r--   0        0        0     3061 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/chunk.py
--rw-r--r--   0        0        0     3056 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/embed.py
--rw-r--r--   0        0        0     4911 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/id.py
--rw-r--r--   0        0        0     1333 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/langchain_utils.py
--rw-r--r--   0        0        0     3838 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/metadata.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/misc/__init__.py
--rw-r--r--   0        0        0     2018 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/processor/misc/emoji_clean.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/file/__init__.py
--rw-r--r--   0        0        0     4159 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/file/csv.py
--rw-r--r--   0        0        0     2273 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/file/pdf.py
--rw-r--r--   0        0        0     2334 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/file/text.py
--rw-r--r--   0        0        0       97 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/langchain/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/url/__init__.py
--rw-r--r--   0        0        0     2871 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/producer/url/url_loader.py
--rw-r--r--   0        0        0      482 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/utils/__init__.py
--rw-r--r--   0        0        0     6234 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/utils/chroma.py
--rw-r--r--   0        0        0     2270 2024-01-30 13:46:25.014225 chromadb_data_pipes-0.0.6/chroma_dp/utils/embedding.py
--rw-r--r--   0        0        0     1560 2024-01-30 13:46:25.018225 chromadb_data_pipes-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     4852 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/README.md
+-rw-r--r--   0        0        0     1989 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/__init__.py
+-rw-r--r--   0        0        0     5356 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_export.py
+-rw-r--r--   0        0        0     5306 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_import.py
+-rw-r--r--   0        0        0    15486 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/huggingface/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/huggingface/utils.py
+-rw-r--r--   0        0        0     2866 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/main.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/__init__.py
+-rw-r--r--   0        0        0     3071 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/chunk.py
+-rw-r--r--   0        0        0     3066 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/embed.py
+-rw-r--r--   0        0        0     4921 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/id.py
+-rw-r--r--   0        0        0     1343 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/langchain_utils.py
+-rw-r--r--   0        0        0     4473 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/__init__.py
+-rw-r--r--   0        0        0     2028 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/emoji_clean.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/producer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/__init__.py
+-rw-r--r--   0        0        0     4188 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/csv.py
+-rw-r--r--   0        0        0     2302 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/pdf.py
+-rw-r--r--   0        0        0     2363 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/text.py
+-rw-r--r--   0        0        0       97 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/url/__init__.py
+-rw-r--r--   0        0        0     2900 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/url/url_loader.py
+-rw-r--r--   0        0        0      482 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/chroma.py
+-rw-r--r--   0        0        0     2918 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/embedding.py
+-rw-r--r--   0        0        0      608 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/templating.py
+-rw-r--r--   0        0        0     1604 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.7/PKG-INFO
```

### Comparing `chromadb_data_pipes-0.0.6/LICENSE.md` & `chromadb_data_pipes-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.6/README.md` & `chromadb_data_pipes-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/__init__.py` & `chromadb_data_pipes-0.0.7/chroma_dp/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/chroma/chroma_export.py` & `chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 from typing import Annotated, Optional, List, Dict, Any
 import typer
 from chromadb import GetResult, Where, WhereDocument
 from chromadb.api.models import Collection
 from chromadb.api.types import validate_where, validate_where_document
 
 from chroma_dp import EmbeddableTextResource
@@ -31,15 +31,15 @@
     id_feature: str = "id",
     meta_features: Optional[List[str]] = None,
 ) -> Dict[str, Any]:
     """Remaps EmbeddableTextResource features to a dictionary."""
 
     _metas = (
         doc.metadata
-        if meta_features is None
+        if meta_features is None or len(meta_features) == 0
         else {
             k: doc.metadata[k]
             for k in meta_features
             if doc.metadata is not None and k in doc.metadata
         }
     )
     return {
@@ -79,17 +79,15 @@
     append: Annotated[bool, typer.Option(help="Append to export file.")] = False,
     limit: Annotated[int, typer.Option(help="The limit.")] = -1,
     offset: Annotated[int, typer.Option(help="The offset.")] = 0,
     batch_size: Annotated[int, typer.Option(help="The batch size.")] = 100,
     embed_feature: Annotated[
         str, typer.Option(help="The embedding feature.")
     ] = "embedding",
-    meta_features: Annotated[
-        Optional[List[str]], typer.Option(help="The metadata features.")
-    ] = None,
+    meta_features: Optional[List[str]] = typer.Option(None,help="The metadata features."),
     id_feature: Annotated[str, typer.Option(help="The id feature.")] = "id",
     doc_feature: Annotated[
         str, typer.Option(help="The document feature.")
     ] = "text_chunk",
     where: Optional[str] = typer.Option(
         None,
         "--where",
@@ -143,11 +141,11 @@
                 meta_features=meta_features,
             )
             for doc in _results
         ]
         if export_file:
             with open(export_file, "a") as f:
                 for _doc in _final_results:
-                    f.write(json.dumps(_doc) + "\n")
+                    f.write(str(json.dumps(_doc)) + "\n")
         else:
             for _doc in _final_results:
                 typer.echo(json.dumps(_doc))
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/chroma/chroma_import.py` & `chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 import sys
 import uuid
 from concurrent.futures import ThreadPoolExecutor
 from typing import Annotated, Optional, List, Dict, Any
 
 import typer
 from chromadb import EmbeddingFunction
@@ -114,16 +114,16 @@
                     continue
                 if _limit != -1 and lc_count >= _limit:
                     break
                 doc = remap_features(
                     json.loads(line),
                     doc_feature,
                     embed_feature,
-                    meta_features,
                     id_feature,
+                    meta_features,
                 )
                 _batch["documents"].append(doc.text_chunk)
                 _batch["embeddings"].append(
                     doc.embedding if _embedding_function is None else None
                 )  # call EF?
                 _batch["metadatas"].append(doc.metadata)
                 _batch["ids"].append(doc.id if doc.id else uuid.uuid4())
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/huggingface/__init__.py` & `chromadb_data_pipes-0.0.7/chroma_dp/huggingface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 
 import sys
 from typing import Annotated, Optional, List, Generator, Union, Sequence, Any, Dict
 from urllib.parse import urlparse, parse_qs
 
 import datasets
 import typer
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/huggingface/utils.py` & `chromadb_data_pipes-0.0.7/chroma_dp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/main.py` & `chromadb_data_pipes-0.0.7/chroma_dp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import typer
+from dotenv import load_dotenv
 from chroma_dp.chroma.chroma_export import chroma_export
 from chroma_dp.chroma.chroma_import import chroma_import
 from chroma_dp.processor.chunk import chunk_process
 from chroma_dp.processor.embed import filter_embed
 from chroma_dp.huggingface import hf_import, hf_export
 from chroma_dp.processor.id import id_process
 from chroma_dp.processor.metadata import meta_process
 from chroma_dp.processor.misc.emoji_clean import emoji_clean
 from chroma_dp.producer.file.csv import csv_import
 from chroma_dp.producer.file.pdf import pdf_import
 from chroma_dp.producer.file.text import txt_import
 from chroma_dp.producer.url.url_loader import url_import
 
+load_dotenv()
 app = typer.Typer(no_args_is_help=True, help="ChromaDB Data Pipes commands.")
 
 # Import commands
 import_commands = typer.Typer(no_args_is_help=True, help="Import commands.")
 
 import_commands.command(
     name="pdf", help="Import PDF files from target dir.", no_args_is_help=True
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/processor/chunk.py` & `chromadb_data_pipes-0.0.7/chroma_dp/processor/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 import sys
 from typing import Any, Iterable, Annotated, Optional
 
 import typer
 
 from chroma_dp import EmbeddableTextResource, CdpProcessor
 from langchain.text_splitter import CharacterTextSplitter
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/processor/embed.py` & `chromadb_data_pipes-0.0.7/chroma_dp/processor/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 import sys
 from typing import Annotated, Optional, List, Dict, Any
 
 import typer
 
 from chroma_dp import EmbeddableTextResource
 from chroma_dp.utils.embedding import (
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/processor/id.py` & `chromadb_data_pipes-0.0.7/chroma_dp/processor/id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import hashlib
-import json
+import orjson as json
 import os
 import sys
 import uuid
 from abc import ABC, abstractmethod
 from typing import Any, Iterable, Annotated, Optional
 
 import typer
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/processor/langchain_utils.py` & `chromadb_data_pipes-0.0.7/chroma_dp/processor/langchain_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 import uuid
 from typing import Any, Dict, Optional, Union
 
 from langchain_core.documents import Document
 
 from chroma_dp import EmbeddableTextResource, Metadata
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/processor/misc/emoji_clean.py` & `chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/emoji_clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson as json
 import re
 import sys
 from typing import Optional, Iterable, Any
 
 import typer
 
 from chroma_dp import EmbeddableTextResource, CdpProcessor
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/producer/file/csv.py` & `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import orjson as json
 from typing import Dict, Any, Iterable, Optional, Annotated, List
 import csv
 import typer
 from langchain_community.document_loaders import CSVLoader
 from langchain_core.documents import Document
 
 from chroma_dp import CdpProducer, EmbeddableTextResource
@@ -114,8 +115,8 @@
         document_column=doc_feature,
         metadata_columns=meta_features,
         batch_size=batch_size,
         delimiter=delimiter,
         quotechar=quotechar,
     )
     for doc in producer.produce():
-        typer.echo(doc.model_dump_json())
+        typer.echo(json.dumps(doc.model_dump()))
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/producer/file/pdf.py` & `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import orjson as json
 from typing import Dict, Any, Iterable, Optional, Annotated
 
 import typer
 from langchain_community.document_loaders.pdf import PyPDFDirectoryLoader
 
 from chroma_dp import CdpProducer, EmbeddableTextResource
 from chroma_dp.processor.langchain_utils import convert_lc_doc_to_chroma_resource
@@ -70,8 +71,8 @@
     ] = 100,
 ) -> None:
     """Export PDF files from a directory to ChromaDB."""
     producer = LangchainPyPDFProducer(
         path=path, glob=glob, recursive=recursive, batch_size=batch_size
     )
     for doc in producer.produce():
-        typer.echo(doc.model_dump_json())
+        typer.echo(json.dumps(doc.model_dump()))
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/producer/file/text.py` & `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import orjson as json
 from typing import Dict, Any, Iterable, Optional, Annotated
 
 import typer
 from langchain_community.document_loaders import DirectoryLoader, TextLoader
 
 from chroma_dp import CdpProducer, EmbeddableTextResource
 from chroma_dp.processor.langchain_utils import convert_lc_doc_to_chroma_resource
@@ -73,8 +74,8 @@
     ] = 100,
 ) -> None:
     """Export text files from a directory to ChromaDB."""
     producer = LangchainTXTProducer(
         path=path, glob=glob, recursive=recursive, batch_size=batch_size
     )
     for doc in producer.produce():
-        typer.echo(doc.model_dump_json())
+        typer.echo(json.dumps(doc.model_dump()))
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/producer/url/url_loader.py` & `chromadb_data_pipes-0.0.7/chroma_dp/producer/url/url_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+import orjson as json
 import sys
 from typing import Optional, Callable, Dict, Any, Iterable, Annotated
 
 import typer
 from langchain_community.document_loaders.recursive_url_loader import RecursiveUrlLoader
 
 from chroma_dp import CdpProducer, EmbeddableTextResource
@@ -84,11 +85,11 @@
     producer = URLProducer(url=url, max_depth=max_depth, batch_size=batch_size)
     start = offset
     count = 0
     max = limit if limit > 0 else sys.maxsize
     for doc in producer.produce():
         if count < start:
             continue
-        typer.echo(doc.model_dump_json())
+        typer.echo(json.dumps(doc.model_dump()))
         count += 1
         if count >= max:
             break
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/utils/chroma.py` & `chromadb_data_pipes-0.0.7/chroma_dp/utils/chroma.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,21 +160,26 @@
     return None
 
 
 def remap_features(
     in_dict: Dict[str, Any],
     doc_feature: str,
     embed_feature: str,
-    meta_features: Optional[List[str]],
     id_feature: str,
+    meta_features: Optional[List[str]] = None,
 ) -> EmbeddableTextResource:
+    # if standard metadata is present and no specific metadata is provided use the standard metadata
+    if "metadata" in in_dict and not meta_features:
+        # print("in_dict", in_dict)
+        _meta = get_default_metadata(in_dict)
+    elif "metadata" in in_dict and meta_features:
+        _meta = {k: in_dict["metadata"][k] for k in meta_features}
+    elif "metadata" not in in_dict and meta_features:
+        _meta = {k: None for k in meta_features}
+    else:
+        _meta = None
     _doc = in_dict[doc_feature]
     _embed = in_dict[embed_feature] if embed_feature else None
-    _meta = (
-        {k: in_dict[k] for k in meta_features}
-        if meta_features
-        else get_default_metadata(in_dict)
-    )
     _id = in_dict[id_feature] if id_feature else None
     return EmbeddableTextResource(
         text_chunk=_doc, embedding=_embed, metadata=_meta, id=_id
     )
```

### Comparing `chromadb_data_pipes-0.0.6/chroma_dp/utils/embedding.py` & `chromadb_data_pipes-0.0.7/chroma_dp/utils/embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from chromadb import EmbeddingFunction
 from chromadb.utils.embedding_functions import (
     ONNXMiniLM_L6_V2,
     OpenAIEmbeddingFunction,
     CohereEmbeddingFunction,
     HuggingFaceEmbeddingFunction,
     SentenceTransformerEmbeddingFunction,
+    GoogleGenerativeAiEmbeddingFunction,
 )
 
 
 class SupportedEmbeddingFunctions(str, Enum):
     default = "default"
     openai = "openai"
     cohere = "cohere"
     hf = "hf"
     st = "st"
+    gemini = "gemini"
 
 
 def get_embedding_function_for_name(
     name: Optional[SupportedEmbeddingFunctions], **kwargs: Any
 ) -> EmbeddingFunction:
     if name == SupportedEmbeddingFunctions.default:
         return ONNXMiniLM_L6_V2()
@@ -61,9 +63,25 @@
             else os.environ.get("ST_MODEL_NAME", "all-MiniLM-L6-v2")
         )
         return SentenceTransformerEmbeddingFunction(
             model_name=model,
             device=os.environ.get("ST_DEVICE", "cpu"),
             normalize_embeddings=os.environ.get("ST_NORMALIZE", "True") == "True",
         )
+    elif name == SupportedEmbeddingFunctions.gemini:
+        model = (
+            kwargs.get("model")
+            if kwargs.get("model")
+            else os.environ.get("GEMINI_MODEL_NAME", "models/embedding-001")
+        )
+        task_type = (
+            kwargs.get("task_type")
+            if kwargs.get("task_type")
+            else os.environ.get("GEMINI_TASK_TYPE", "RETRIEVAL_DOCUMENT")
+        )
+        return GoogleGenerativeAiEmbeddingFunction(
+            api_key=os.environ.get("GEMINI_API_KEY"),
+            model_name=model,
+            task_type=task_type,
+        )
     else:
         raise ValueError("Please provide a valid embedding function.")
```

### Comparing `chromadb_data_pipes-0.0.6/pyproject.toml` & `chromadb_data_pipes-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromadb-data-pipes"
-version = "0.0.6"
+version = "0.0.7"
 description = "ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "chroma_dp" }]
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/amikos-tech/chromadb-data-pipes/issues"
@@ -23,14 +23,16 @@
 typer = { extras = ["all"], version = "^0.9.0" }
 pydantic = "^2.5.3"
 tenacity = "^8.2.3"
 fastapi = "^0.108.0"
 langchain = "^0.1.0"
 pypdf = "^3.17.4"
 py-ulid = "^1.0.3"
+python-dotenv = "^1.0.1"
+orjson = "^3.9.12"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 black = "23.3.0"
 pre-commit = "^3.6.0"
 hypothesis = "^6.92.0"
```

### Comparing `chromadb_data_pipes-0.0.6/PKG-INFO` & `chromadb_data_pipes-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: chromadb-data-pipes
-Version: 0.0.6
+Version: 0.0.7
 Summary: ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (==0.4.22)
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: langchain (>=0.1.0,<0.2.0)
+Requires-Dist: orjson (>=3.9.12,<4.0.0)
 Requires-Dist: py-ulid (>=1.0.3,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pypdf (>=3.17.4,<4.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/amikos-tech/chromadb-data-pipes/issues
 Project-URL: Homepage, https://datapipes.chromadb.dev/
 Project-URL: Source, https://github.com/amikos-tech/chromadb-data-pipes/
```


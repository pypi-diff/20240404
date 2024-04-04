# Comparing `tmp/fondant-0.9.dev2.tar.gz` & `tmp/fondant-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondant-0.9.dev2.tar", max compression
+gzip compressed data, was "fondant-1.0.0.tar", max compression
```

## Comparing `fondant-0.9.dev2.tar` & `fondant-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0    11356 2024-01-15 10:13:24.020223 fondant-0.9.dev2/LICENSE
--rw-r--r--   0        0        0    11950 2024-01-15 10:13:24.020223 fondant-0.9.dev2/README.md
--rw-r--r--   0        0        0     4015 2024-01-15 10:50:38.494961 fondant-0.9.dev2/pyproject.toml
--rw-r--r--   0        0        0      130 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/__init__.py
--rw-r--r--   0        0        0     4030 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/build.py
--rw-r--r--   0        0        0    28694 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/cli.py
--rw-r--r--   0        0        0      432 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/component/__init__.py
--rw-r--r--   0        0        0     2297 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/component/component.py
--rw-r--r--   0        0        0     8474 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/component/data_io.py
--rw-r--r--   0        0        0    22347 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/component/executor.py
--rw-r--r--   0        0        0      589 2024-01-15 10:50:45.898879 fondant-0.9.dev2/src/fondant/components/caption_images/fondant_component.yaml
--rw-r--r--   0        0        0     1871 2024-01-15 10:50:46.574872 fondant-0.9.dev2/src/fondant/components/chunk_text/fondant_component.yaml
--rw-r--r--   0        0        0     1729 2024-01-15 10:50:45.942879 fondant-0.9.dev2/src/fondant/components/crop_images/fondant_component.yaml
--rw-r--r--   0        0        0     1770 2024-01-15 10:50:46.214876 fondant-0.9.dev2/src/fondant/components/download_images/fondant_component.yaml
--rw-r--r--   0        0        0      491 2024-01-15 10:50:45.762881 fondant-0.9.dev2/src/fondant/components/embed_images/fondant_component.yaml
--rw-r--r--   0        0        0     1245 2024-01-15 10:50:46.530872 fondant-0.9.dev2/src/fondant/components/embed_text/fondant_component.yaml
--rw-r--r--   0        0        0      791 2024-01-15 10:50:46.438874 fondant-0.9.dev2/src/fondant/components/evaluate_ragas/fondant_component.yaml
--rw-r--r--   0        0        0      316 2024-01-15 10:50:46.710871 fondant-0.9.dev2/src/fondant/components/extract_image_resolution/fondant_component.yaml
--rw-r--r--   0        0        0      415 2024-01-15 10:50:46.258875 fondant-0.9.dev2/src/fondant/components/filter_image_resolution/fondant_component.yaml
--rw-r--r--   0        0        0      329 2024-01-15 10:50:45.670882 fondant-0.9.dev2/src/fondant/components/filter_language/fondant_component.yaml
--rw-r--r--   0        0        0      363 2024-01-15 10:50:46.754870 fondant-0.9.dev2/src/fondant/components/filter_text_length/fondant_component.yaml
--rw-r--r--   0        0        0      378 2024-01-15 10:50:45.626882 fondant-0.9.dev2/src/fondant/components/generate_minhash/fondant_component.yaml
--rw-r--r--   0        0        0     1482 2024-01-15 10:50:46.078878 fondant-0.9.dev2/src/fondant/components/index_aws_opensearch/fondant_component.yaml
--rw-r--r--   0        0        0     2158 2024-01-15 10:50:45.718881 fondant-0.9.dev2/src/fondant/components/index_qdrant/fondant_component.yaml
--rw-r--r--   0        0        0     1575 2024-01-15 10:50:46.122877 fondant-0.9.dev2/src/fondant/components/index_weaviate/fondant_component.yaml
--rw-r--r--   0        0        0      836 2024-01-15 10:50:46.034878 fondant-0.9.dev2/src/fondant/components/load_from_csv/fondant_component.yaml
--rw-r--r--   0        0        0      449 2024-01-15 10:50:46.302875 fondant-0.9.dev2/src/fondant/components/load_from_files/fondant_component.yaml
--rw-r--r--   0        0        0     1005 2024-01-15 10:50:46.798869 fondant-0.9.dev2/src/fondant/components/load_from_hf_hub/fondant_component.yaml
--rw-r--r--   0        0        0      760 2024-01-15 10:50:45.986878 fondant-0.9.dev2/src/fondant/components/load_from_parquet/fondant_component.yaml
--rw-r--r--   0        0        0     1196 2024-01-15 10:50:46.346875 fondant-0.9.dev2/src/fondant/components/load_from_pdf/fondant_component.yaml
--rw-r--r--   0        0        0      893 2024-01-15 10:50:46.394874 fondant-0.9.dev2/src/fondant/components/load_from_pdf/tests/fondant_component.yaml
--rw-r--r--   0        0        0     1700 2024-01-15 10:50:45.538883 fondant-0.9.dev2/src/fondant/components/load_with_llamahub/fondant_component.yaml
--rw-r--r--   0        0        0     1742 2024-01-15 10:50:45.582883 fondant-0.9.dev2/src/fondant/components/load_with_llamahub/tests/fondant_component.yaml
--rw-r--r--   0        0        0     1395 2024-01-15 10:50:45.850880 fondant-0.9.dev2/src/fondant/components/normalize_text/fondant_component.yaml
--rw-r--r--   0        0        0      381 2024-01-15 10:50:46.618872 fondant-0.9.dev2/src/fondant/components/resize_images/fondant_component.yaml
--rw-r--r--   0        0        0      612 2024-01-15 10:50:46.482873 fondant-0.9.dev2/src/fondant/components/retrieve_from_weaviate/fondant_component.yaml
--rw-r--r--   0        0        0      857 2024-01-15 10:50:45.806880 fondant-0.9.dev2/src/fondant/components/retrieve_laion_by_embedding/fondant_component.yaml
--rw-r--r--   0        0        0     1142 2024-01-15 10:50:45.490884 fondant-0.9.dev2/src/fondant/components/retrieve_laion_by_prompt/fondant_component.yaml
--rw-r--r--   0        0        0      491 2024-01-15 10:50:46.662871 fondant-0.9.dev2/src/fondant/components/segment_images/fondant_component.yaml
--rw-r--r--   0        0        0      759 2024-01-15 10:50:46.166876 fondant-0.9.dev2/src/fondant/components/write_to_hf_hub/fondant_component.yaml
--rw-r--r--   0        0        0        0 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/__init__.py
--rw-r--r--   0        0        0    21289 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/component_spec.py
--rw-r--r--   0        0        0      877 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/exceptions.py
--rw-r--r--   0        0        0     9630 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/manifest.py
--rw-r--r--   0        0        0     6797 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/schema.py
--rw-r--r--   0        0        0     1541 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/schemas/common.json
--rw-r--r--   0        0        0     1894 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/schemas/component_spec.json
--rw-r--r--   0        0        0     1236 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/core/schemas/manifest.json
--rw-r--r--   0        0        0     5792 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/explore.py
--rw-r--r--   0        0        0      158 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/pipeline/__init__.py
--rw-r--r--   0        0        0     3448 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/pipeline/argument_inference.py
--rw-r--r--   0        0        0    28389 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/pipeline/compiler.py
--rw-r--r--   0        0        0    27878 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/pipeline/pipeline.py
--rw-r--r--   0        0        0    11877 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/pipeline/runner.py
--rw-r--r--   0        0        0     9606 2024-01-15 10:13:24.080222 fondant-0.9.dev2/src/fondant/testing.py
--rw-r--r--   0        0        0    14158 1970-01-01 00:00:00.000000 fondant-0.9.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-01-31 08:27:03.729496 fondant-1.0.0/LICENSE
+-rw-r--r--   0        0        0    11746 2024-01-31 08:27:03.729496 fondant-1.0.0/README.md
+-rw-r--r--   0        0        0     4012 2024-01-31 09:22:54.125634 fondant-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/__init__.py
+-rw-r--r--   0        0        0     4050 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/build.py
+-rw-r--r--   0        0        0    28694 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/cli.py
+-rw-r--r--   0        0        0      432 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/component/__init__.py
+-rw-r--r--   0        0        0     2211 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/component/component.py
+-rw-r--r--   0        0        0     8467 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/component/data_io.py
+-rw-r--r--   0        0        0    22815 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/component/executor.py
+-rw-r--r--   0        0        0      586 2024-01-31 09:23:02.537689 fondant-1.0.0/src/fondant/components/caption_images/fondant_component.yaml
+-rw-r--r--   0        0        0     1868 2024-01-31 09:23:03.477695 fondant-1.0.0/src/fondant/components/chunk_text/fondant_component.yaml
+-rw-r--r--   0        0        0     1726 2024-01-31 09:23:03.657696 fondant-1.0.0/src/fondant/components/crop_images/fondant_component.yaml
+-rw-r--r--   0        0        0     1767 2024-01-31 09:23:02.493689 fondant-1.0.0/src/fondant/components/download_images/fondant_component.yaml
+-rw-r--r--   0        0        0      488 2024-01-31 09:23:02.893691 fondant-1.0.0/src/fondant/components/embed_images/fondant_component.yaml
+-rw-r--r--   0        0        0     1242 2024-01-31 09:23:03.253693 fondant-1.0.0/src/fondant/components/embed_text/fondant_component.yaml
+-rw-r--r--   0        0        0      789 2024-01-31 09:23:03.165693 fondant-1.0.0/src/fondant/components/evaluate_ragas/fondant_component.yaml
+-rw-r--r--   0        0        0      313 2024-01-31 09:23:02.941691 fondant-1.0.0/src/fondant/components/extract_image_resolution/fondant_component.yaml
+-rw-r--r--   0        0        0      412 2024-01-31 09:23:03.701696 fondant-1.0.0/src/fondant/components/filter_image_resolution/fondant_component.yaml
+-rw-r--r--   0        0        0      326 2024-01-31 09:23:03.341694 fondant-1.0.0/src/fondant/components/filter_language/fondant_component.yaml
+-rw-r--r--   0        0        0      360 2024-01-31 09:23:03.433694 fondant-1.0.0/src/fondant/components/filter_text_length/fondant_component.yaml
+-rw-r--r--   0        0        0      375 2024-01-31 09:23:03.613696 fondant-1.0.0/src/fondant/components/generate_minhash/fondant_component.yaml
+-rw-r--r--   0        0        0     1479 2024-01-31 09:23:02.717690 fondant-1.0.0/src/fondant/components/index_aws_opensearch/fondant_component.yaml
+-rw-r--r--   0        0        0     2155 2024-01-31 09:23:03.389694 fondant-1.0.0/src/fondant/components/index_qdrant/fondant_component.yaml
+-rw-r--r--   0        0        0     3781 2024-01-31 09:23:03.209693 fondant-1.0.0/src/fondant/components/index_weaviate/fondant_component.yaml
+-rw-r--r--   0        0        0      833 2024-01-31 09:23:02.985692 fondant-1.0.0/src/fondant/components/load_from_csv/fondant_component.yaml
+-rw-r--r--   0        0        0      446 2024-01-31 09:23:02.445688 fondant-1.0.0/src/fondant/components/load_from_files/fondant_component.yaml
+-rw-r--r--   0        0        0     1002 2024-01-31 09:23:03.029692 fondant-1.0.0/src/fondant/components/load_from_hf_hub/fondant_component.yaml
+-rw-r--r--   0        0        0      757 2024-01-31 09:23:02.761690 fondant-1.0.0/src/fondant/components/load_from_parquet/fondant_component.yaml
+-rw-r--r--   0        0        0     1193 2024-01-31 09:23:02.805691 fondant-1.0.0/src/fondant/components/load_from_pdf/fondant_component.yaml
+-rw-r--r--   0        0        0      893 2024-01-31 09:23:02.849691 fondant-1.0.0/src/fondant/components/load_from_pdf/tests/fondant_component.yaml
+-rw-r--r--   0        0        0     1697 2024-01-31 09:23:02.581689 fondant-1.0.0/src/fondant/components/load_with_llamahub/fondant_component.yaml
+-rw-r--r--   0        0        0     1742 2024-01-31 09:23:02.625689 fondant-1.0.0/src/fondant/components/load_with_llamahub/tests/fondant_component.yaml
+-rw-r--r--   0        0        0     1392 2024-01-31 09:23:03.297694 fondant-1.0.0/src/fondant/components/normalize_text/fondant_component.yaml
+-rw-r--r--   0        0        0      378 2024-01-31 09:23:03.117693 fondant-1.0.0/src/fondant/components/resize_images/fondant_component.yaml
+-rw-r--r--   0        0        0     4292 2024-01-31 09:23:03.073692 fondant-1.0.0/src/fondant/components/retrieve_from_weaviate/fondant_component.yaml
+-rw-r--r--   0        0        0      854 2024-01-31 09:23:03.525695 fondant-1.0.0/src/fondant/components/retrieve_laion_by_embedding/fondant_component.yaml
+-rw-r--r--   0        0        0     1139 2024-01-31 09:23:02.401688 fondant-1.0.0/src/fondant/components/retrieve_laion_by_prompt/fondant_component.yaml
+-rw-r--r--   0        0        0      488 2024-01-31 09:23:03.569695 fondant-1.0.0/src/fondant/components/segment_images/fondant_component.yaml
+-rw-r--r--   0        0        0      756 2024-01-31 09:23:02.669690 fondant-1.0.0/src/fondant/components/write_to_hf_hub/fondant_component.yaml
+-rw-r--r--   0        0        0        0 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/__init__.py
+-rw-r--r--   0        0        0    19162 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/component_spec.py
+-rw-r--r--   0        0        0     1004 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/exceptions.py
+-rw-r--r--   0        0        0     9623 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/manifest.py
+-rw-r--r--   0        0        0     6797 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/schema.py
+-rw-r--r--   0        0        0     1541 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/schemas/common.json
+-rw-r--r--   0        0        0     1894 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/schemas/component_spec.json
+-rw-r--r--   0        0        0     1236 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/core/schemas/manifest.json
+-rw-r--r--   0        0        0     5792 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/explore.py
+-rw-r--r--   0        0        0      269 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/pipeline/__init__.py
+-rw-r--r--   0        0        0     3448 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/pipeline/argument_inference.py
+-rw-r--r--   0        0        0    34092 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/pipeline/compiler.py
+-rw-r--r--   0        0        0    10556 2024-01-31 08:27:03.781496 fondant-1.0.0/src/fondant/pipeline/lightweight_component.py
+-rw-r--r--   0        0        0    31355 2024-01-31 08:27:03.785496 fondant-1.0.0/src/fondant/pipeline/pipeline.py
+-rw-r--r--   0        0        0    11877 2024-01-31 08:27:03.785496 fondant-1.0.0/src/fondant/pipeline/runner.py
+-rw-r--r--   0        0        0     9705 2024-01-31 08:27:03.785496 fondant-1.0.0/src/fondant/testing.py
+-rw-r--r--   0        0        0    13951 1970-01-01 00:00:00.000000 fondant-1.0.0/PKG-INFO
```

### Comparing `fondant-0.9.dev2/LICENSE` & `fondant-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/README.md` & `fondant-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,14 @@
 
 🛋️ [**ControlNet Interior Design Pipeline**](https://github.com/ml6team/fondant-usecase-controlnet)  
 An end-to-end Fondant pipeline to collect and process data for the fine-tuning of a ControlNet model, focusing on images related to interior design.
 
 🖼️ [**Filter creative common license images**](https://github.com/ml6team/fondant-usecase-filter-creative-commons)  
 An end-to-end Fondant pipeline that starts from our Fondant-CC-25M creative commons image dataset and filters and downloads the desired images.
 
-🔢 [**Datacomp pipeline**](https://github.com/ml6team/fondant-usecase-datacomp)  
-An end-to-end Fondant pipeline filtering image-text data to train a CLIP model for the DataComp competition.
-
 ## ⚒️ Installation
 
 Fondant can be installed using pip:
 
 ```
 pip install fondant
 ```
@@ -186,15 +183,15 @@
 ```python
 import pandas as pd
 from fondant.component import PandasTransformComponent
 
 
 class ExampleComponent(PandasTransformComponent):
 
-    def __init__(self, *, argument1, argument2, **kwargs) -> None:
+    def __init__(self, *, argument1, argument2) -> None:
         """
         Args:
             argumentX: An argument passed to the component
         """
         # Initialize your component here based on the arguments
 
     def transform(self, dataframe: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `fondant-0.9.dev2/pyproject.toml` & `fondant-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fondant"
-version = '0.9.dev2'
+version = '1.0.0'
 description = "Fondant - Large-scale data processing made easy and reusable"
 readme = "README.md"
 keywords = ["data", "machine learning", "fine-tuning", "foundation models"]
 license = "Apache-2.0"
 authors = [
     "ML6 <fondant@ml6.eu>",
     "Simon Slangen <simon.slangen@ml6.eu>",
@@ -37,30 +37,30 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">= 3.8, <3.11"
+python = ">= 3.8, <3.12"
 
 fsspec = ">= 2023.4.0"
 importlib-resources = { version = ">= 1.3", python = "<3.9" }
 jsonschema = ">= 4.18"
 pyarrow = ">= 11.0.0"
 pyyaml = ">= 5.3.1"
 
 dask = { version = ">= 2023.4.1", extras = ["dataframe", "distributed", "diagnostics"], optional = true }
 
 gcsfs = { version = ">= 2023.10.0", optional = true }
 s3fs = { version = ">= 2023.4.0", optional = true }
 adlfs = { version = ">= 2023.4.0", optional = true }
 
 docker = {version = ">= 6.1.3", optional = true }
-kfp = { version = "2.3.0", optional = true, extras =["kubernetes"] }
+kfp = { version = "2.6.0", optional = true, extras =["kubernetes"] }
 google-cloud-aiplatform =  { version = "1.34.0", optional = true}
 sagemaker = {version = ">= 2.197.0", optional = true}
 boto3 = {version = "1.28.64", optional = true}
 
 [tool.poetry.extras]
 component = ["dask"]
```

### Comparing `fondant-0.9.dev2/src/fondant/build.py` & `fondant-1.0.0/src/fondant/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "You need to install `docker` to use the `fondant build` command, you can install "
             "it with `pip install fondant[docker]`"
         )
         raise SystemExit(
             msg,
         )
 
-    component_op = ComponentOp(component_dir)
+    component_op = ComponentOp.from_component_yaml(component_dir)
     component_spec = component_op.component_spec
 
     if component_op.dockerfile_path is None:
         msg = (
             f"Could not detect a `Dockerfile` in {component_dir}. Please make sure it is placed "
             f"at the root of your component_dir and named `Dockerfile`."
         )
```

### Comparing `fondant-0.9.dev2/src/fondant/cli.py` & `fondant-1.0.0/src/fondant/cli.py`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/component/data_io.py` & `fondant-1.0.0/src/fondant/component/data_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 msg,
             )
 
     def _write_dataframe(self, dataframe: dd.DataFrame) -> dd.core.Scalar:
         """Create dataframe writing task."""
         location = (
             f"{self.manifest.base_path}/{self.manifest.pipeline_name}/"
-            f"{self.manifest.run_id}/{self.operation_spec.component_folder_name}"
+            f"{self.manifest.run_id}/{self.operation_spec.component_name}"
         )
 
         schema = {
             field.name: field.type.value
             for field in self.operation_spec.outer_produces.values()
         }
         return self._create_write_task(dataframe, location=location, schema=schema)
```

### Comparing `fondant-0.9.dev2/src/fondant/component/executor.py` & `fondant-1.0.0/src/fondant/component/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,42 +260,34 @@
         data_writer = DaskDataWriter(
             manifest=manifest,
             operation_spec=self.operation_spec,
         )
 
         data_writer.write_dataframe(dataframe, self.client)
 
-    def _get_cached_manifest(self) -> t.Union[Manifest, None]:
+    def _get_cache_reference_content(self) -> t.Union[str, None]:
         """
-        Find and return the matching execution's Manifest for the component, if it exists.
-
-        This function searches for previous execution manifests that match the component's metadata.
+        Get the content of the cache reference file. This file contains the path to the cached
+        manifest or empty string if the component is cached without producing any manifest.
 
         Returns:
-            The Manifest object representing the most recent matching execution,
-            or None if no matching execution is found.
+            The content of the cache reference file.
         """
         manifest_reference_path = (
             f"{self.metadata.base_path}/{self.metadata.pipeline_name}/cache/"
             f"{self.metadata.cache_key}.txt"
         )
 
         try:
             with fs_open(
                 manifest_reference_path,
                 mode="rt",
                 encoding="utf-8",
             ) as file_:
-                cached_manifest_path = file_.read()
-                manifest = Manifest.from_file(cached_manifest_path)
-                logger.info(
-                    f"Matching execution detected for component. The last execution of the"
-                    f" component originated from `{manifest.run_id}`.",
-                )
-                return manifest
+                return file_.read()
 
         except FileNotFoundError:
             logger.info("No matching execution for component detected")
             return None
 
     def _is_previous_cached(self, input_manifest: Manifest) -> bool:
         """
@@ -331,23 +323,25 @@
 
     def _run_execution(
         self,
         component_cls: t.Type[Component],
         input_manifest: Manifest,
     ) -> Manifest:
         logging.info("Executing component")
-        component: Component = component_cls(
-            consumes=self.operation_spec.inner_consumes,
-            produces=self.operation_spec.inner_produces,
-            **self.user_arguments,
-        )
+
+        component: Component = component_cls(**self.user_arguments)
+
+        component.consumes = self.operation_spec.inner_consumes
+        component.produces = self.operation_spec.inner_produces
+
         output_df = self._execute_component(
             component,
             manifest=input_manifest,
         )
+
         output_manifest = input_manifest.evolve(
             operation_spec=self.operation_spec,
             run_id=self.metadata.run_id,
         )
         self._write_data(dataframe=output_df, manifest=output_manifest)
 
         component.teardown()
@@ -358,72 +352,96 @@
         """
         Execute a component.
 
         Args:
             component_cls: The class of the component to execute
         """
         input_manifest = self._load_or_create_manifest()
+        base_path = input_manifest.base_path
+        pipeline_name = input_manifest.pipeline_name
 
         if self.cache and self._is_previous_cached(input_manifest):
-            output_manifest = self._get_cached_manifest()
-            if output_manifest is not None:
+            cache_reference_content = self._get_cache_reference_content()
+
+            if cache_reference_content is not None:
                 logger.info("Skipping component execution")
+
+                if cache_reference_content:
+                    output_manifest = Manifest.from_file(cache_reference_content)
+
+                    logger.info(
+                        f"Matching execution detected for component. The last execution of the"
+                        f" component originated from `{output_manifest.run_id}`.",
+                    )
+                else:
+                    logger.info("Component is cached without producing a manifest")
+                    output_manifest = None
             else:
                 output_manifest = self._run_execution(component_cls, input_manifest)
 
         else:
             logger.info("Caching disabled for the component")
             output_manifest = self._run_execution(component_cls, input_manifest)
 
-        self.upload_manifest(output_manifest, save_path=self.output_manifest_path)
+        if output_manifest:
+            self.upload_manifest(output_manifest, save_path=self.output_manifest_path)
 
-    def _upload_cache_key(
+        self._upload_cache_reference_content(
+            base_path=base_path,
+            pipeline_name=pipeline_name,
+        )
+
+    def _upload_cache_reference_content(
         self,
-        manifest: Manifest,
-        manifest_save_path: t.Union[str, Path],
+        base_path: str,
+        pipeline_name: str,
     ):
         """
-        Write the cache key containing the reference to the location of the written manifest..
+        Write the cache key containing the reference to the location of the written manifest.
 
         This function creates a file with the format "<cache_key>.txt" at the specified
         'manifest_save_path' to store the manifest location for future retrieval of
         cached component executions.
 
         Args:
-            manifest: The reference manifest.
-            manifest_save_path (str): The path where the manifest is saved.
+            base_path: The base path of the pipeline.
+            pipeline_name: The name of the pipeline.
         """
-        manifest_reference_path = (
-            f"{manifest.base_path}/{manifest.pipeline_name}/cache/"
-            f"{self.metadata.cache_key}.txt"
+        cache_reference_path = (
+            f"{base_path}/{pipeline_name}/cache/{self.metadata.cache_key}.txt"
         )
 
-        logger.info(f"Writing cache key to {manifest_reference_path}")
+        logger.info(
+            f"Writing cache key with manifest reference to {cache_reference_path}",
+        )
 
         with fs_open(
-            manifest_reference_path,
+            cache_reference_path,
             mode="wt",
             encoding="utf-8",
             auto_mkdir=True,
         ) as file_:
-            file_.write(str(manifest_save_path))
+            file_.write(self.cache_reference_content)
+
+    @property
+    def cache_reference_content(self) -> str:
+        return str(self.output_manifest_path)
 
     def upload_manifest(self, manifest: Manifest, save_path: t.Union[str, Path]):
         """
         Uploads the manifest to the specified destination.
 
         Args:
             manifest: The Manifest object to be uploaded.
             save_path: The path where the Manifest object will be saved.
 
         """
         Path(save_path).parent.mkdir(parents=True, exist_ok=True)
         manifest.to_file(save_path)
         logger.info(f"Saving output manifest to {save_path}")
-        self._upload_cache_key(manifest=manifest, manifest_save_path=save_path)
 
 
 class DaskLoadExecutor(Executor[DaskLoadComponent]):
     """Base class for a Fondant load component."""
 
     def _is_previous_cached(self, input_manifest: Manifest) -> bool:
         return True
@@ -597,14 +615,18 @@
 
     def _write_data(self, dataframe: dd.DataFrame, *, manifest: Manifest):
         """Create a data writer given a manifest and writes out the index and subsets."""
 
     def upload_manifest(self, manifest: Manifest, save_path: t.Union[str, Path]):
         pass
 
+    @property
+    def cache_reference_content(self) -> str:
+        return ""
+
 
 class ExecutorFactory:
     def __init__(self, component: t.Type[Component]):
         self.component = component
         self.component_executor_mapping: t.Dict[str, t.Type[Executor]] = {
             "DaskLoadComponent": DaskLoadExecutor,
             "DaskTransformComponent": DaskTransformExecutor,
```

### Comparing `fondant-0.9.dev2/src/fondant/components/caption_images/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/caption_images/fondant_component.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Caption images
 description: This component captions images using a BLIP model from the Hugging Face hub
-image: fndnt/caption_images:0.9.dev2
+image: fndnt/caption_images:1.0.0
 tags:
   - Image processing
 
 consumes:
   image:
     type: binary
```

### Comparing `fondant-0.9.dev2/src/fondant/components/chunk_text/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/chunk_text/fondant_component.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   
   Different chunking strategies can be used. The default is to use the "recursive" strategy which
     recursively splits the text into smaller chunks until the chunk size is reached. 
   
   More information about the different chunking strategies can be here:
   - https://python.langchain.com/docs/modules/data_connection/document_transformers/
   - https://www.pinecone.io/learn/chunking-strategies/
-image: fndnt/chunk_text:0.9.dev2
+image: fndnt/chunk_text:1.0.0
 tags:
   - Text processing
 
 consumes:
   text:
     type: string
```

### Comparing `fondant-0.9.dev2/src/fondant/components/crop_images/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/crop_images/fondant_component.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Crop images
-image: fndnt/crop_images:0.9.dev2
+image: fndnt/crop_images:1.0.0
 description: |
   This component crops out image borders. This is typically useful when working with graphical 
   images that have single-color borders (e.g. logos, icons, etc.).
   
   The component takes an image and calculates which color is most present in the border. It then 
   crops the image in order to minimize this single-color border. The `padding` argument will add 
   extra border to the image before cropping it, in order to avoid cutting off parts of the image.
```

### Comparing `fondant-0.9.dev2/src/fondant/components/download_images/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/download_images/fondant_component.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   
   This component takes in image URLs as input and downloads the images, along with some metadata 
   (like their height and width). The images are stored in a new colum as bytes objects. This 
   component also resizes the images using the 
   [resizer](https://github.com/rom1504/img2dataset/blob/main/img2dataset/resizer.py) function 
   from the img2dataset library.
 
-image: fndnt/download_images:0.9.dev2
+image: fndnt/download_images:1.0.0
 tags:
   - Data retrieval
 
 consumes:
   image_url:
     type: string
```

### Comparing `fondant-0.9.dev2/src/fondant/components/embed_text/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/embed_text/fondant_component.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Embed text
 description: Component that generates embeddings of text passages.
-image: fndnt/embed_text:0.9.dev2
+image: fndnt/embed_text:1.0.0
 tags:
   - Text processing
 
 consumes:
   text:
     type: string
```

### Comparing `fondant-0.9.dev2/src/fondant/components/evaluate_ragas/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/evaluate_ragas/fondant_component.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-name: Evalute ragas
+name: Evaluate ragas
 description: Component that evaluates the retriever using RAGAS
-image: fndnt/evaluate_ragas:0.9.dev2
+image: fndnt/evaluate_ragas:1.0.0
 tags:
   - Text processing
 
 consumes:
   question:
     type: string
   retrieved_chunks:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/index_aws_opensearch/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/index_aws_opensearch/fondant_component.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Index AWS OpenSearch
 description: Component that takes embeddings of text snippets and indexes them into AWS OpenSearch vector database.
-image: fndnt/index_aws_opensearch:0.9.dev2
+image: fndnt/index_aws_opensearch:1.0.0
 tags:
   - Data writing
 
 consumes:
   text:
     type: string
   embedding:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/index_qdrant/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/index_qdrant/fondant_component.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Index Qdrant
 description: >-
   A Fondant component to load textual data and embeddings into a Qdrant database.
   NOTE: A Qdrant collection has to be created in advance with the appropriate configurations. https://qdrant.tech/documentation/concepts/collections/
-image: fndnt/index_qdrant:0.9.dev2
+image: fndnt/index_qdrant:1.0.0
 tags:
   - Data writing
 
 consumes:
   text:
     type: string
   embedding:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/index_weaviate/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_from_pdf/fondant_component.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,41 @@
-name: Index Weaviate
-description: Component that takes embeddings of text snippets and indexes them into a weaviate vector database.
-image: fndnt/index_weaviate:0.9.dev2
+name: Load from pdf
+description: |
+  Load pdf data stored locally or remote using langchain loaders.
+image: fndnt/load_from_pdf:1.0.0
 tags:
-  - Data writing
+  - Data loading
 
-consumes:
+produces:
+  pdf_path:
+    type: string
+  file_name:
+    type: string
   text:
     type: string
-  embedding:
-    type: array
-    items:
-      type: float32
 
 args:
-  weaviate_url:
-    description: The URL of the weaviate instance.
-    type: str
-    default: http://localhost:8080
-  batch_size:
-    description: |
-      The batch size to be used.
-      Parameter of weaviate.batch.Batch().configure().
-    type: int
-    default: 100
-  dynamic:
+  pdf_path:
     description: |
-      Whether to use dynamic batching or not.
-      Parameter of weaviate.batch.Batch().configure().
-    type: bool
-    default: True
-  num_workers:
+      The path to the a pdf file or a folder containing pdf files to load. 
+      Can be a local path or a remote path. If the path is remote, the loader class will be 
+      determined by the scheme of the path.
+    type: str
+  n_rows_to_load:
     description: |
-      The maximal number of concurrent threads to run batch import.
-      Parameter of weaviate.batch.Batch().configure().
+      Optional argument that defines the number of rows to load. Useful for testing pipeline runs 
+      on a small scale
     type: int
-    default: 2
-  overwrite:
-    description: Whether to overwrite/ re-create the existing weaviate class and its embeddings.
-    type: bool
-    default: False
-  class_name:
+    default: None
+  index_column:
     description: |
-      The name of the weaviate class that will be created and used to store the embeddings.
-      Should follow the weaviate naming conventions.
+      Column to set index to in the load component, if not specified a default globally unique 
+      index will be set
     type: str
-  vectorizer:
+    default: None
+  n_partitions:
     description: |
-      Which vectorizer to use. 
-      You can find the available vectorizers in the weaviate documentation: https://weaviate
-      .io/developers/weaviate/modules/retriever-vectorizer-modules
-      Set this to None if you want to insert your own embeddings.
-    type: str
+      Number of partitions of the dask dataframe. If not specified, the number of partitions will 
+      be equal to the number of CPU cores. Set to high values if the data is large and the pipeline
+      is running out of memory.
+    type: int
     default: None
-
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_from_csv/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_from_csv/fondant_component.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Load from csv
 description: Component that loads a dataset from a csv file
-image: fndnt/load_from_csv:0.9.dev2
+image: fndnt/load_from_csv:1.0.0
 tags:
   - Data loading
 
 produces:
   additionalProperties: true
 
 args:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_from_hf_hub/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_from_hf_hub/fondant_component.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Load from Hugging Face hub
 description: Component that loads a dataset from the hub
-image: fndnt/load_from_hf_hub:0.9.dev2
+image: fndnt/load_from_hf_hub:1.0.0
 tags:
   - Data loading
 
 produces:
   additionalProperties: true
 
 args:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_from_parquet/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_from_parquet/fondant_component.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Load from parquet
 description: Component that loads a dataset from a parquet uri
-image: fndnt/load_from_parquet:0.9.dev2
+image: fndnt/load_from_parquet:1.0.0
 tags:
   - Data loading
 
 produces:
   additionalProperties: true
 
 args:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_from_pdf/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_from_pdf/tests/fondant_component.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: Load from pdf
 description: |
   Load pdf data stored locally or remote using langchain loaders.
-image: fndnt/load_from_pdf:0.9.dev2
+image: fndnt/load_from_pdf:dev
 tags:
   - Data loading
 
 produces:
   pdf_path:
     type: string
   file_name:
@@ -28,14 +28,7 @@
     default: None
   index_column:
     description: |
       Column to set index to in the load component, if not specified a default globally unique 
       index will be set
     type: str
     default: None
-  n_partitions:
-    description: |
-      Number of partitions of the dask dataframe. If not specified, the number of partitions will 
-      be equal to the number of CPU cores. Set to high values if the data is large and the pipeline
-      is running out of memory.
-    type: int
-    default: None
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_from_pdf/tests/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/retrieve_laion_by_prompt/fondant_component.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-name: Load from pdf
+name: Retrieve LAION by prompt
 description: |
-  Load pdf data stored locally or remote using langchain loaders.
-image: fndnt/load_from_pdf:dev
+  This component retrieves image URLs from the [LAION-5B dataset](https://laion.ai/blog/laion-5b/) 
+  based on text prompts. The retrieval itself is done based on CLIP embeddings similarity between 
+  the prompt sentences and the captions in the LAION dataset. 
+  
+  This component doesn’t return the actual images, only URLs.
+image: fndnt/retrieve_laion_by_prompt:1.0.0
 tags:
-  - Data loading
+  - Data retrieval
 
-produces:
-  pdf_path:
+consumes:
+  prompt:
     type: string
-  file_name:
+
+produces:
+  image_url:
     type: string
-  text:
+  prompt_id:
     type: string
 
+previous_index: prompt_id
+
 args:
-  pdf_path:
-    description: |
-      The path to the a pdf file or a folder containing pdf files to load. 
-      Can be a local path or a remote path. If the path is remote, the loader class will be 
-      determined by the scheme of the path.
-    type: str
-  n_rows_to_load:
-    description: |
-      Optional argument that defines the number of rows to load. Useful for testing pipeline runs 
-      on a small scale
+  num_images:
+    description: Number of images to retrieve for each prompt
+    type: int
+  aesthetic_score:
+    description: Aesthetic embedding to add to the query embedding, between 0 and 9 (higher is prettier).
     type: int
-    default: None
-  index_column:
-    description: |
-      Column to set index to in the load component, if not specified a default globally unique 
-      index will be set
+    default: 9
+  aesthetic_weight:
+    description: Weight of the aesthetic embedding when added to the query, between 0 and 1
+    type: float
+    default: 0.5
+  url:
+    description: The url of the backend clip retrieval service, defaults to the public service
     type: str
-    default: None
+    default: https://knn.laion.ai/knn-service
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_with_llamahub/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_with_llamahub/fondant_component.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Load with LlamaHub
 description: |
   Load data using a LlamaHub loader. For available loaders, check the 
   [LlamaHub](https://llamahub.ai/).
-image: fndnt/load_with_llamahub:0.9.dev2
+image: fndnt/load_with_llamahub:1.0.0
 tags:
   - Data loading
 
 produces:
   additionalProperties: true
 
 args:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/load_with_llamahub/tests/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/load_with_llamahub/tests/fondant_component.yaml`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/components/normalize_text/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/normalize_text/fondant_component.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Normalize text
-image: fndnt/normalize_text:0.9.dev2
+image: fndnt/normalize_text:1.0.0
 description: |
   This component implements several text normalization techniques to clean and preprocess textual 
   data:
 
   - Apply lowercasing: Converts all text to lowercase
   - Remove unnecessary whitespaces: Eliminates extra spaces between words, e.g. tabs
   - Apply NFC normalization: Converts characters to their canonical representation
```

### Comparing `fondant-0.9.dev2/src/fondant/components/retrieve_laion_by_embedding/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/retrieve_laion_by_embedding/fondant_component.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Retrieve LAION by embedding
 description: |
   This component retrieves image URLs from LAION-5B based on a set of CLIP embeddings. It can be 
   used to find images similar to the embedded images / captions.
-image: fndnt/retrieve_laion_by_embedding:0.9.dev2
+image: fndnt/retrieve_laion_by_embedding:1.0.0
 tags:
   - Data retrieval
 
 consumes:
   embedding:
     type: array
     items:
```

### Comparing `fondant-0.9.dev2/src/fondant/components/write_to_hf_hub/fondant_component.yaml` & `fondant-1.0.0/src/fondant/components/write_to_hf_hub/fondant_component.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Write to Hugging Face hub
 description: Component that writes a dataset to the hub
-image: fndnt/write_to_hf_hub:0.9.dev2
+image: fndnt/write_to_hf_hub:1.0.0
 tags:
   - Data writing
 
 consumes:
   additionalProperties: true
 
 args:
```

### Comparing `fondant-0.9.dev2/src/fondant/core/component_spec.py` & `fondant-1.0.0/src/fondant/core/component_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module defines classes to represent an Fondant component specification."""
 import copy
 import json
 import pkgutil
 import pydoc
-import re
 import types
 import typing as t
 from dataclasses import dataclass
 from pathlib import Path
 
 import jsonschema.exceptions
 import pyarrow as pa
@@ -51,25 +50,83 @@
             float: "NUMBER_DOUBLE",
             bool: "BOOLEAN",
             dict: "STRUCT",
             list: "LIST",
         }
         return lookup[self.type]
 
+    def to_spec(self):
+        return {
+            k: v
+            for k, v in {
+                "description": self.description,
+                "type": self.type.__name__,
+                "default": self.default,
+            }.items()
+            if v is not None
+        }
+
 
 class ComponentSpec:
     """
     Class representing a Fondant component specification.
 
     Args:
-        specification: The fondant component specification as a Python dict
+        name: The name of the component
+        image: The docker image uri to use for the component
+        description: The description of the component
+            consumes: A mapping containing the fields consumed by the operation. The keys are the
+            names of the fields to be received by the component, while the values are the
+            type of the field.
+
+
+            produces: A mapping containing the fields produced by the operation. The keys are the
+                names of the fields to be produced by the component, while the values are the
+                type of the field to be written
+
+            arguments: A dictionary containing the argument name and value for the operation.
+
     """
 
-    def __init__(self, specification: t.Dict[str, t.Any]) -> None:
-        self._specification = copy.deepcopy(specification)
+    def __init__(
+        self,
+        name: str,
+        image: str,
+        *,
+        description: t.Optional[str] = None,
+        consumes: t.Optional[t.Mapping[str, t.Union[str, pa.DataType, bool]]] = None,
+        produces: t.Optional[t.Mapping[str, t.Union[str, pa.DataType, bool]]] = None,
+        previous_index: t.Optional[str] = None,
+        args: t.Optional[t.Dict[str, t.Any]] = None,
+        tags: t.Optional[t.List[str]] = None,
+    ):
+        spec_dict: t.Dict[str, t.Any] = {
+            "name": name,
+            "image": image,
+        }
+
+        if description:
+            spec_dict["description"] = description
+
+        if tags:
+            spec_dict["tags"] = tags
+
+        if consumes:
+            spec_dict["consumes"] = consumes
+
+        if produces:
+            spec_dict["produces"] = produces
+
+        if previous_index:
+            spec_dict["previous_index"] = previous_index
+
+        if args:
+            spec_dict["args"] = args
+
+        self._specification = spec_dict
         self._validate_spec()
 
     def _validate_spec(self) -> None:
         """Validate a component specification against the component schema.
 
         Raises: InvalidComponent when the component specification is not valid.
         """
@@ -98,46 +155,41 @@
             raise InvalidComponentSpec.create_from(e)
 
     @classmethod
     def from_file(cls, path: t.Union[str, Path]) -> "ComponentSpec":
         """Load the component spec from the file specified by the provided path."""
         with open(path, encoding="utf-8") as file_:
             specification = yaml.safe_load(file_)
-            return cls(specification)
+            return cls.from_dict(specification)
 
     def to_file(self, path) -> None:
         """Dump the component spec to the file specified by the provided path."""
         with open(path, "w", encoding="utf-8") as file_:
             yaml.dump(self._specification, file_)
 
+    @classmethod
+    def from_dict(cls, component_spec_dict: t.Dict[str, t.Any]) -> "ComponentSpec":
+        """Load the component spec from a dictionary."""
+        try:
+            return cls(**component_spec_dict)
+        except TypeError as e:
+            msg = f"Invalid component spec: {e}"
+            raise InvalidComponentSpec(msg)
+
     @property
     def name(self):
         return self._specification["name"]
 
     @property
-    def component_folder_name(self):
-        """Cleans and converts a name to a proper folder name."""
-        return self._specification["name"].lower().replace(" ", "_")
+    def safe_name(self):
+        return self.sanitized_component_name(self._specification["name"])
 
-    @property
-    def sanitized_component_name(self):
-        """Cleans and converts a name to be kfp V2 compatible.
-
-        Taken from https://github.com/kubeflow/pipelines/blob/
-        cfe671c485d4ee8514290ee81ca2785e8bda5c9b/sdk/python/kfp/dsl/utils.py#L52
-        """
-        return (
-            re.sub(
-                "-+",
-                "-",
-                re.sub("[^-0-9a-z]+", "-", self._specification["name"].lower()),
-            )
-            .lstrip("-")
-            .rstrip("-")
-        )
+    def sanitized_component_name(self, name) -> str:
+        """Cleans and converts a component name."""
+        return name.lower().replace(" ", "_")
 
     @property
     def description(self):
         return self._specification["description"]
 
     @property
     def image(self) -> str:
@@ -152,26 +204,26 @@
         return self._specification.get("tags", None)
 
     @property
     def consumes(self) -> t.Mapping[str, Field]:
         """The fields consumed by the component as an immutable mapping."""
         return types.MappingProxyType(
             {
-                name: Field(name=name, type=Type.from_json(field))
+                name: Field(name=name, type=Type.from_dict(field))
                 for name, field in self._specification.get("consumes", {}).items()
                 if name != "additionalProperties"
             },
         )
 
     @property
     def produces(self) -> t.Mapping[str, Field]:
         """The fields produced by the component as an immutable mapping."""
         return types.MappingProxyType(
             {
-                name: Field(name=name, type=Type.from_json(field))
+                name: Field(name=name, type=Type.from_dict(field))
                 for name, field in self._specification.get("produces", {}).items()
                 if name != "additionalProperties"
             },
         )
 
     def is_generic(self, mapping: str) -> bool:
         """Returns a boolean indicating whether the provided mapping is generic.
@@ -192,17 +244,17 @@
     @property
     def args(self) -> t.Mapping[str, Argument]:
         args = self.default_arguments
         args.update(
             {
                 name: Argument(
                     name=name,
-                    description=arg_info["description"],
+                    description=arg_info.get("description"),
                     type=pydoc.locate(arg_info["type"]),  # type: ignore
-                    default=arg_info["default"] if "default" in arg_info else None,
+                    default=arg_info.get("default"),
                     optional=arg_info.get("default") == "None",
                 )
                 for name, arg_info in self._specification.get("args", {}).items()
             },
         )
         return types.MappingProxyType(args)
 
@@ -258,18 +310,14 @@
             "output_manifest_path": Argument(
                 name="output_manifest_path",
                 description="Path to the output manifest",
                 type=str,
             ),
         }
 
-    @property
-    def kubeflow_specification(self) -> "KubeflowComponentSpec":
-        return KubeflowComponentSpec.from_fondant_component_spec(self)
-
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._specification!r})"
 
     def __eq__(self, other):
         if not isinstance(other, ComponentSpec):
             return False
         return self._specification == other._specification
@@ -297,48 +345,52 @@
         self._validate_mappings()
 
         self._inner_consumes: t.Optional[t.Mapping[str, Field]] = None
         self._outer_consumes: t.Optional[t.Mapping[str, Field]] = None
         self._inner_produces: t.Optional[t.Mapping[str, Field]] = None
         self._outer_produces: t.Optional[t.Mapping[str, Field]] = None
 
-    def to_json(self) -> str:
+    def to_dict(self) -> dict:
         def _dump_mapping(
             mapping: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]],
         ) -> dict:
             if mapping is None:
                 return {}
 
             serialized_mapping: t.Dict[str, t.Any] = mapping.copy()
             for key, value in mapping.items():
                 if isinstance(value, pa.DataType):
-                    serialized_mapping[key] = Type(value).to_json()
+                    serialized_mapping[key] = Type(value).to_dict()
             return serialized_mapping
 
-        specification_dict = {
+        return {
             "specification": self._component_spec.specification,
             "consumes": _dump_mapping(self._mappings["consumes"]),
             "produces": _dump_mapping(self._mappings["produces"]),
         }
 
+    def to_json(self) -> str:
+        specification_dict = self.to_dict()
         return json.dumps(specification_dict)
 
     @classmethod
     def from_dict(cls, operation_spec_dict: t.Dict[str, t.Any]) -> "OperationSpec":
         def _parse_mapping(
             json_mapping: dict,
         ) -> t.Optional[t.Dict[str, t.Union[str, pa.DataType]]]:
             """Parse a json mapping to a Python mapping with Fondant types."""
             for key, value in json_mapping.items():
                 if isinstance(value, dict):
-                    json_mapping[key] = Type.from_json(value).value
+                    json_mapping[key] = Type.from_dict(value).value
             return json_mapping
 
         return cls(
-            component_spec=ComponentSpec(operation_spec_dict["specification"]),
+            component_spec=ComponentSpec.from_dict(
+                operation_spec_dict["specification"],
+            ),
             consumes=_parse_mapping(operation_spec_dict["consumes"]),
             produces=_parse_mapping(operation_spec_dict["produces"]),
         )
 
     @classmethod
     def from_json(cls, operation_spec_json: str) -> "OperationSpec":
         return cls.from_dict(json.loads(operation_spec_json))
@@ -387,15 +439,15 @@
                 spec_type = spec_mapping[key].type.value
                 if spec_type == value:
                     # Same info in mapping and component spec, let it pass
                     pass
                 else:
                     msg = (
                         f"Received pyarrow DataType value {value} for key {key} in the "
-                        f"`{name}` argument passed to the operation, but {key} is "
+                        f"`{name}` argument passed to the operation, but `{key}` is "
                         f"already defined in the `{name}` section of the component spec "
                         f"with type {spec_type}"
                     )
                     raise InvalidPipelineDefinition(msg)
 
         return types.MappingProxyType(mapping)
 
@@ -419,16 +471,16 @@
             if not isinstance(value, str):
                 continue
 
             if key in spec_mapping:
                 mapping[value] = Field(name=value, type=mapping.pop(key).type)
             else:
                 msg = (
-                    f"Received a string value for key {key} in the `{name}` "
-                    f"argument passed to the operation, but {key} is not defined in "
+                    f"Received a string value for key `{key}` in the `{name}` "
+                    f"argument passed to the operation, but `{key}` is not defined in "
                     f"the `{name}` section of the component spec."
                 )
                 raise InvalidPipelineDefinition(msg)
 
         return types.MappingProxyType(mapping)
 
     @property
@@ -464,17 +516,17 @@
         """The "outer" `produces` mapping which the dataIO needs to read / write."""
         if self._outer_produces is None:
             self._outer_produces = self._outer_mapping("produces")
 
         return self._outer_produces
 
     @property
-    def component_folder_name(self) -> str:
-        """Cleans and converts a name to a proper folder name."""
-        return self._component_spec.component_folder_name
+    def component_name(self) -> str:
+        """Get the component name."""
+        return self._component_spec.safe_name
 
     @property
     def previous_index(self) -> t.Optional[str]:
         """The name of the index column of the previous component."""
         return self._component_spec.previous_index
 
     @property
@@ -491,111 +543,7 @@
             return False
 
         # Compare mappings attribute
         if self._mappings != other._mappings:
             return False
 
         return True
-
-
-class KubeflowComponentSpec:
-    """
-    Class representing a Kubeflow component specification.
-
-    Args:
-        specification: The kubeflow component specification as a Python dict
-    """
-
-    def __init__(self, specification: t.Dict[str, t.Any]) -> None:
-        self._specification = specification
-
-    @staticmethod
-    def convert_arguments(fondant_component: ComponentSpec):
-        args = {}
-        for arg in fondant_component.args.values():
-            arg_type_dict = {}
-
-            # Enable isOptional attribute in spec if arg is Optional and defaults to None
-            if arg.optional and arg.default is None:
-                arg_type_dict["isOptional"] = True
-            if arg.default is not None:
-                arg_type_dict["defaultValue"] = arg.default
-
-            args[arg.name] = {
-                "parameterType": arg.kubeflow_type,
-                "description": arg.description,
-                **arg_type_dict,  # type: ignore
-            }
-
-        return args
-
-    @classmethod
-    def from_fondant_component_spec(cls, fondant_component: ComponentSpec):
-        """Generate a Kubeflow component spec from a Fondant component spec."""
-        input_definitions = {
-            "parameters": {
-                **cls.convert_arguments(fondant_component),
-            },
-        }
-
-        cleaned_component_name = fondant_component.sanitized_component_name
-
-        specification = {
-            "components": {
-                "comp-"
-                + cleaned_component_name: {
-                    "executorLabel": "exec-" + cleaned_component_name,
-                    "inputDefinitions": input_definitions,
-                },
-            },
-            "deploymentSpec": {
-                "executors": {
-                    "exec-"
-                    + cleaned_component_name: {
-                        "container": {
-                            "command": ["fondant", "execute", "main"],
-                            "image": fondant_component.image,
-                        },
-                    },
-                },
-            },
-            "pipelineInfo": {"name": cleaned_component_name},
-            "root": {
-                "dag": {
-                    "tasks": {
-                        cleaned_component_name: {
-                            "cachingOptions": {"enableCache": True},
-                            "componentRef": {"name": "comp-" + cleaned_component_name},
-                            "inputs": {
-                                "parameters": {
-                                    param: {"componentInputParameter": param}
-                                    for param in input_definitions["parameters"]
-                                },
-                            },
-                            "taskInfo": {"name": cleaned_component_name},
-                        },
-                    },
-                },
-                "inputDefinitions": input_definitions,
-            },
-            "schemaVersion": "2.1.0",
-            "sdkVersion": "kfp-2.0.1",
-        }
-        return cls(specification)
-
-    def to_file(self, path: t.Union[str, Path]) -> None:
-        """Dump the component specification to the file specified by the provided path."""
-        with open(path, "w", encoding="utf-8") as file_:
-            yaml.dump(
-                self._specification,
-                file_,
-                indent=4,
-                default_flow_style=False,
-                sort_keys=False,
-            )
-
-    def to_string(self) -> str:
-        """Return the component specification as a string."""
-        return json.dumps(self._specification)
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self._specification!r})"
```

### Comparing `fondant-0.9.dev2/src/fondant/core/exceptions.py` & `fondant-1.0.0/src/fondant/core/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,7 +21,11 @@
 
 class InvalidTypeSchema(ValidationError, FondantException):
     """Thrown when a Type schema definition is invalid."""
 
 
 class UnsupportedTypeAnnotation(FondantException):
     """Thrown when an unsupported type annotation is encountered during type inference."""
+
+
+class InvalidLightweightComponent(FondantException):
+    """Thrown when a component is not a valid lightweight component."""
```

### Comparing `fondant-0.9.dev2/src/fondant/core/manifest.py` & `fondant-1.0.0/src/fondant/core/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     @property
     def fields(self) -> t.Mapping[str, Field]:
         """The fields of the manifest as an immutable mapping."""
         return types.MappingProxyType(
             {
                 name: Field(
                     name=name,
-                    type=Type.from_json(field),
+                    type=Type.from_dict(field),
                     location=field["location"],
                 )
                 for name, field in self._specification["fields"].items()
             },
         )
 
     def add_or_update_field(self, field: Field, overwrite: bool = False):
@@ -204,15 +204,15 @@
                 f"A field with name {field.name} already exists. Set overwrite to true, "
                 f"if you want to update the field."
             )
             raise ValueError(msg)
         else:
             self._specification["fields"][field.name] = {
                 "location": field.location,
-                **field.type.to_json(),
+                **field.type.to_dict(),
             }
 
     def _add_or_update_index(self, field: Field, overwrite: bool = True):
         """Add or update the manifest index."""
         if overwrite is False:
             msg = (
                 "The index already exists. Set overwrite to true, "
@@ -252,15 +252,15 @@
             operation_spec: the operation spec
             run_id: the run id to include in the evolved manifest. If no run id is provided,
             the run id from the original manifest is propagated.
         """
         evolved_manifest = self.copy()
 
         # Update `run_id` and `component_id` in the metadata
-        component_id = operation_spec.component_folder_name
+        component_id = operation_spec.component_name
         evolved_manifest.update_metadata(key="component_id", value=component_id)
         evolved_manifest.update_metadata(key="run_id", value=run_id)
 
         # Update index location as this is always rewritten
         evolved_manifest.add_or_update_field(
             Field(name="index", location=f"/{run_id}/{component_id}"),
         )
```

### Comparing `fondant-0.9.dev2/src/fondant/core/schema.py` & `fondant-1.0.0/src/fondant/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,44 +132,44 @@
         """
         data_type = cls._validate_data_type(data_type)
         return cls(
             pa.list_(data_type.value if isinstance(data_type, Type) else data_type),
         )
 
     @classmethod
-    def from_json(cls, json_schema: dict):
+    def from_dict(cls, json_schema: dict):
         """
         Creates a new `Type` instance based on a dictionary representation of the json schema
           of a data type (https://swagger.io/docs/specification/data-models/data-types/).
 
         Args:
             json_schema: The dictionary representation of the data type, can represent nested values
 
         Returns:
             A new `Type` instance representing the specified data type.
         """
         if json_schema["type"] == "array":
             items = json_schema["items"]
             if isinstance(items, dict):
-                return cls.list(cls.from_json(items))
+                return cls.list(cls.from_dict(items))
             return None
 
         return cls(json_schema["type"])
 
-    def to_json(self) -> dict:
+    def to_dict(self) -> dict:
         """
         Converts the `Type` instance to its JSON representation.
 
         Returns:
             A dictionary representing the JSON schema of the data type.
         """
         if isinstance(self.value, pa.ListType):
             items = self.value.value_type
             if isinstance(items, pa.DataType):
-                return {"type": "array", "items": Type(items).to_json()}
+                return {"type": "array", "items": Type(items).to_dict()}
 
         type_ = None
         for type_name, data_type in _TYPES.items():
             if self.value.equals(data_type):
                 type_ = type_name
                 break
```

### Comparing `fondant-0.9.dev2/src/fondant/core/schemas/common.json` & `fondant-1.0.0/src/fondant/core/schemas/common.json`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/core/schemas/component_spec.json` & `fondant-1.0.0/src/fondant/core/schemas/component_spec.json`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/core/schemas/manifest.json` & `fondant-1.0.0/src/fondant/core/schemas/manifest.json`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/explore.py` & `fondant-1.0.0/src/fondant/explore.py`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/pipeline/argument_inference.py` & `fondant-1.0.0/src/fondant/pipeline/argument_inference.py`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/pipeline/compiler.py` & `fondant-1.0.0/src/fondant/pipeline/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import json
 import logging
 import os
+import re
 import shlex
 import tempfile
+import textwrap
 import typing as t
 from abc import ABC, abstractmethod
 from dataclasses import asdict
 from pathlib import Path
 
 import yaml
 
+from fondant.core.component_spec import ComponentSpec
 from fondant.core.exceptions import InvalidPipelineDefinition
 from fondant.core.manifest import Metadata
 from fondant.core.schema import CloudCredentialsMount, DockerVolume
 from fondant.pipeline import (
     VALID_ACCELERATOR_TYPES,
     VALID_VERTEX_ACCELERATOR_TYPES,
+    Image,
     Pipeline,
 )
 
 logger = logging.getLogger(__name__)
 
 DASK_DIAGNOSTIC_DASHBOARD_PORT = 8787
 KubeflowCommandArguments = t.List[t.Union[str, t.Dict[str, str]]]
@@ -41,14 +45,45 @@
         for config_name, config_value in kwargs.items():
             if config_value is not None:
                 logger.warning(
                     f"Configuration `{config_name}` is set with `{config_value}` but has no effect"
                     f" for runner `{self.__class__.__name__}`.",
                 )
 
+    @staticmethod
+    def _build_entrypoint(image: Image) -> t.List[str]:
+        """Build the entrypoint to execute the provided image."""
+        if not image.script:
+            # Not a lightweight python component
+            return ["fondant", "execute", "main"]
+
+        command = ""
+        if image.extra_requires:
+            requirements = "\n".join(image.extra_requires)
+            command += textwrap.dedent(
+                f"""\
+                printf {shlex.quote(requirements)} > 'requirements.txt'
+                python3 -m pip install -r requirements.txt
+            """,
+            )
+
+        command += textwrap.dedent(
+            f"""\
+            printf {shlex.quote(image.script)} > 'main.py'
+            fondant execute main "$@"
+        """,
+        )
+
+        return [
+            "sh",
+            "-ec",
+            command,
+            "--",  # All arguments provided after this will be passed to `fondant execute main`
+        ]
+
 
 class DockerCompiler(Compiler):
     """Compiler that creates a docker-compose spec from a pipeline."""
 
     def compile(
         self,
         pipeline: Pipeline,
@@ -136,40 +171,42 @@
 
         services = {}
 
         pipeline.validate(run_id=run_id)
 
         component_cache_key = None
 
-        for component_name, component in pipeline._graph.items():
+        for component_id, component in pipeline._graph.items():
             component_op = component["operation"]
 
             component_cache_key = component_op.get_component_cache_key(
                 previous_component_cache=component_cache_key,
             )
 
             metadata = Metadata(
                 pipeline_name=pipeline.name,
                 run_id=run_id,
                 base_path=path,
-                component_id=component_name,
+                component_id=component_id,
                 cache_key=component_cache_key,
             )
 
-            logger.info(f"Compiling service for {component_name}")
+            logger.info(f"Compiling service for {component_id}")
+
+            entrypoint = self._build_entrypoint(component_op.image)
 
             # add metadata argument to command
             command = ["--metadata", metadata.to_json()]
 
             # add in and out manifest paths to command
             command.extend(
                 [
                     "--output_manifest_path",
                     f"{path}/{metadata.pipeline_name}/{metadata.run_id}/"
-                    f"{component_name}/manifest.json",
+                    f"{component_id}/manifest.json",
                 ],
             )
 
             # add arguments if any to command
             for key, value in component_op.arguments.items():
                 if isinstance(value, (dict, list)):
                     command.extend([f"--{key}", json.dumps(value)])
@@ -199,44 +236,45 @@
                 volumes.extend(extra_volumes)
 
             ports: t.List[t.Union[str, dict]] = []
             ports.append(
                 f"{DASK_DIAGNOSTIC_DASHBOARD_PORT}:{DASK_DIAGNOSTIC_DASHBOARD_PORT}",
             )
 
-            services[component_name] = {
+            services[component_id] = {
+                "entrypoint": entrypoint,
                 "command": command,
                 "depends_on": depends_on,
                 "volumes": volumes,
                 "ports": ports,
                 "labels": {
                     "pipeline_description": pipeline.description,
                 },
             }
 
-            self._set_configuration(services, component_op, component_name)
+            self._set_configuration(services, component_op, component_id)
 
             if component_op.dockerfile_path is not None:
                 logger.info(
-                    f"Found Dockerfile for {component_name}, adding build step.",
+                    f"Found Dockerfile for {component_id}, adding build step.",
                 )
-                services[component_name]["build"] = {
+                services[component_id]["build"] = {
                     "context": str(component_op.component_dir.absolute()),
                     "args": build_args,
                 }
             else:
-                services[component_name]["image"] = component_op.component_spec.image
+                services[component_id]["image"] = component_op.component_spec.image
 
         return {
             "name": pipeline.name,
             "version": "3.8",
             "services": services,
         }
 
-    def _set_configuration(self, services, fondant_component_operation, component_name):
+    def _set_configuration(self, services, fondant_component_operation, component_id):
         resources_dict = fondant_component_operation.resources.to_dict()
 
         accelerator_name = resources_dict.pop("accelerator_name")
         accelerator_number = resources_dict.pop("accelerator_number")
 
         # Unused configurations
         self.log_unused_configurations(**resources_dict)
@@ -247,15 +285,15 @@
                     f"Configured accelerator `{accelerator_name}`"
                     f" is not a valid accelerator type for Docker Compose compiler."
                     f" Available options: {VALID_VERTEX_ACCELERATOR_TYPES}"
                 )
                 raise InvalidPipelineDefinition(msg)
 
             if accelerator_name == "GPU":
-                services[component_name]["deploy"] = {
+                services[component_id]["deploy"] = {
                     "resources": {
                         "reservations": {
                             "devices": [
                                 {
                                     "driver": "nvidia",
                                     "count": accelerator_number,
                                     "capabilities": ["gpu"],
@@ -267,14 +305,130 @@
             elif accelerator_name == "TPU":
                 msg = "TPU configuration is not yet implemented for Docker Compose "
                 raise NotImplementedError(msg)
 
         return services
 
 
+class KubeflowComponentSpec:
+    """
+    Class representing a Kubeflow component specification.
+
+    Args:
+        specification: The kubeflow component specification as a Python dict
+    """
+
+    def __init__(self, specification: t.Dict[str, t.Any]) -> None:
+        self._specification = specification
+
+    @staticmethod
+    def convert_arguments(fondant_component: ComponentSpec):
+        args = {}
+        for arg in fondant_component.args.values():
+            arg_type_dict = {}
+
+            # Enable isOptional attribute in spec if arg is Optional and defaults to None
+            if arg.optional and arg.default is None:
+                arg_type_dict["isOptional"] = True
+            if arg.default is not None:
+                arg_type_dict["defaultValue"] = arg.default
+
+            args[arg.name] = {
+                "parameterType": arg.kubeflow_type,
+                "description": arg.description,
+                **arg_type_dict,  # type: ignore
+            }
+
+        return args
+
+    @classmethod
+    def from_fondant_component_spec(
+        cls,
+        fondant_component: ComponentSpec,
+        command: t.List[str],
+        image_uri: str,
+    ):
+        """Generate a Kubeflow component spec from a Fondant component spec."""
+        input_definitions = {
+            "parameters": {
+                **cls.convert_arguments(fondant_component),
+            },
+        }
+
+        kfp_safe_name = (
+            re.sub(
+                "-+",
+                "-",
+                re.sub("[^-0-9a-z]+", "-", fondant_component.safe_name.lower()),
+            )
+            .lstrip("-")
+            .rstrip("-")
+        )
+        specification = {
+            "components": {
+                "comp-"
+                + kfp_safe_name: {
+                    "executorLabel": "exec-" + kfp_safe_name,
+                    "inputDefinitions": input_definitions,
+                },
+            },
+            "deploymentSpec": {
+                "executors": {
+                    "exec-"
+                    + kfp_safe_name: {
+                        "container": {
+                            "command": command,
+                            "image": image_uri,
+                        },
+                    },
+                },
+            },
+            "pipelineInfo": {"name": kfp_safe_name},
+            "root": {
+                "dag": {
+                    "tasks": {
+                        kfp_safe_name: {
+                            "cachingOptions": {"enableCache": True},
+                            "componentRef": {"name": "comp-" + kfp_safe_name},
+                            "inputs": {
+                                "parameters": {
+                                    param: {"componentInputParameter": param}
+                                    for param in input_definitions["parameters"]
+                                },
+                            },
+                            "taskInfo": {"name": kfp_safe_name},
+                        },
+                    },
+                },
+                "inputDefinitions": input_definitions,
+            },
+            "schemaVersion": "2.1.0",
+            "sdkVersion": "kfp-2.6.0",
+        }
+        return cls(specification)
+
+    def to_file(self, path: t.Union[str, Path]) -> None:
+        """Dump the component specification to the file specified by the provided path."""
+        with open(path, "w", encoding="utf-8") as file_:
+            yaml.dump(
+                self._specification,
+                file_,
+                indent=4,
+                default_flow_style=False,
+                sort_keys=False,
+            )
+
+    def to_string(self) -> str:
+        """Return the component specification as a string."""
+        return json.dumps(self._specification)
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self._specification!r})"
+
+
 class KubeFlowCompiler(Compiler):
     """Compiler that creates a Kubeflow pipeline spec from a pipeline."""
 
     def __init__(self):
         self._resolve_imports()
 
     def _resolve_imports(self):
@@ -338,16 +492,24 @@
             component_cache_key = None
 
             for component_name, component in pipeline._graph.items():
                 logger.info(f"Compiling service for {component_name}")
 
                 component_op = component["operation"]
                 # convert ComponentOp to Kubeflow component
+                command = self._build_entrypoint(component_op.image)
+                image_uri = component_op.image.base_image
+                kubeflow_spec = KubeflowComponentSpec.from_fondant_component_spec(
+                    component_op.component_spec,
+                    command=command,
+                    image_uri=image_uri,
+                )
+
                 kubeflow_component_op = self.kfp.components.load_component_from_text(
-                    text=component_op.component_spec.kubeflow_specification.to_string(),
+                    text=kubeflow_spec.to_string(),
                 )
 
                 # Remove None values from arguments
                 component_args = {
                     k: v for k, v in component_op.arguments.items() if v is not None
                 }
 
@@ -531,15 +693,15 @@
         except ImportError:
             msg = """You need to install the sagemaker extras to use the sagemaker compiler,\n
                      you can install it with `pip install fondant[sagemaker]`"""
             raise ImportError(
                 msg,
             )
 
-    def _get_build_command(
+    def _build_command(
         self,
         metadata: Metadata,
         arguments: t.Dict[str, t.Any],
         dependencies: t.List[str] = [],
     ) -> t.List[str]:
         # add metadata argument to command
         command = ["--metadata", f"'{metadata.to_json()}'"]
@@ -599,27 +761,32 @@
             logging.info(
                 f"Pull through cache rule for '{self.ecr_namespace}' created successfully",
             )
 
     def _patch_uri(self, og_uri: str) -> str:
         full_ref, tag = og_uri.split(":")
 
-        ref, *_ = full_ref.split("/")
+        ref, *repo = full_ref.split("/")
 
-        if ref == "fndnt":
-            logging.info("Reusable component detected, patching URI")
-            # force pullthrough cache to be used
+        def pull_through(repository_name):
             _ = self.ecr_client.batch_get_image(
-                repositoryName=f"{self.ecr_namespace}/{full_ref}",
+                repositoryName=repository_name,
                 imageIds=[{"imageTag": tag}],
             )
             repo_response = self.ecr_client.describe_repositories(
-                repositoryNames=[f"{self.ecr_namespace}/{full_ref}"],
+                repositoryNames=[repository_name],
             )
-            uri = repo_response["repositories"][0]["repositoryUri"] + ":" + tag
+            return repo_response["repositories"][0]["repositoryUri"] + ":" + tag
+
+        if ref == "fndnt":
+            logging.info("Reusable component detected, patching URI")
+            uri = pull_through(f"{self.ecr_namespace}/{full_ref}")
+        elif ref == "public.ecr.aws":
+            logging.info("Public AWS ECR component detected, patching URI")
+            uri = pull_through(f"{self.ecr_namespace}/{'/'.join(repo)}")
         else:
             logging.info("Custom component detected")
             # the uri does not need patching
             uri = og_uri
         return uri
 
     def validate_base_path(self, base_path: str) -> None:
@@ -672,36 +839,40 @@
                     base_path=path,
                     component_id=component_name,
                     cache_key=component_cache_key,
                 )
 
                 logger.info(f"Compiling service for {component_name}")
 
-                command = self._get_build_command(
+                command = self._build_command(
                     metadata,
                     component_op.arguments,
                     component["dependencies"],
                 )
                 depends_on = [steps[-1]] if component["dependencies"] else []
 
+                image = component_op.image
+                entrypoint = self._build_entrypoint(image)
+
                 script_path = self.generate_component_script(
-                    component_name,
-                    command,
-                    tmpdirname,
+                    entrypoint=entrypoint,
+                    command=command,
+                    component_name=component_name,
+                    directory=tmpdirname,
                 )
 
                 if not role_arn:
                     # if no role is provided use the default sagemaker execution role
                     # https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-ex-role.html
                     role_arn = self.sagemaker.get_execution_role()
 
                 resources_dict = self._set_configuration(component_op)
 
                 processor = self.sagemaker.processing.ScriptProcessor(
-                    image_uri=self._patch_uri(component_op.component_spec.image),
+                    image_uri=self._patch_uri(image.base_image),
                     command=["bash"],
                     instance_count=1,
                     base_job_name=component_name,
                     role=role_arn,
                     **resources_dict,
                 )
 
@@ -745,27 +916,25 @@
             instance_type = "ml.t3.medium"
 
         # Unused configurations
         self.log_unused_configurations(**resources_dict)
 
         return {"instance_type": instance_type}
 
+    @staticmethod
     def generate_component_script(
-        self,
-        component_name: str,
+        *,
+        entrypoint: t.List[str],
         command: t.List[str],
+        component_name: str,
         directory: str,
     ) -> str:
         """Generate a bash script for a component to be used as input in a
         sagemaker pipeline step. Returns the path to the script.
         """
-        content = ["fondant", "execute", "main"]
-
         # use shlex.quote to escape special bash chars
-        for c in command:
-            content.append(c.replace("'", ""))
-
-        cleaned_content = shlex.join(content)
+        command_string = [arg.replace("'", "") for arg in command]
+        cleaned_script = shlex.join([*entrypoint, *command_string])
 
         with open(f"{directory}/{component_name}.sh", "w") as f:
-            f.write(cleaned_content)
+            f.write(cleaned_script)
         return f"{directory}/{component_name}.sh"
```

### Comparing `fondant-0.9.dev2/src/fondant/pipeline/pipeline.py` & `fondant-1.0.0/src/fondant/pipeline/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module defines classes to represent a Fondant Pipeline."""
 import datetime
 import hashlib
+import inspect
 import json
 import logging
 import re
 import typing as t
 from collections import OrderedDict
 from dataclasses import asdict, dataclass
 from pathlib import Path
@@ -12,18 +13,24 @@
 try:
     from importlib.resources import files  # type: ignore
 except ImportError:
     from importlib_resources import files  # type: ignore
 
 import pyarrow as pa
 
+from fondant.component import BaseComponent
 from fondant.core.component_spec import ComponentSpec, OperationSpec
-from fondant.core.exceptions import InvalidPipelineDefinition
+from fondant.core.exceptions import (
+    InvalidLightweightComponent,
+    InvalidPipelineDefinition,
+)
 from fondant.core.manifest import Manifest
 from fondant.core.schema import Field
+from fondant.pipeline import Image, LightweightComponent
+from fondant.pipeline.argument_inference import infer_arguments
 
 logger = logging.getLogger(__name__)
 
 VALID_ACCELERATOR_TYPES = [
     "GPU",
     "TPU",
 ]
@@ -127,38 +134,34 @@
           arguments.
     """
 
     COMPONENT_SPEC_NAME = "fondant_component.yaml"
 
     def __init__(
         self,
-        name_or_path: t.Union[str, Path],
+        image: Image,
+        component_spec: ComponentSpec,
         *,
         consumes: t.Optional[t.Dict[str, str]] = None,
         produces: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]] = None,
         arguments: t.Optional[t.Dict[str, t.Any]] = None,
         input_partition_rows: t.Optional[t.Union[str, int]] = None,
         cache: t.Optional[bool] = True,
         cluster_type: t.Optional[str] = "default",
         client_kwargs: t.Optional[dict] = None,
         resources: t.Optional[Resources] = None,
+        component_dir: t.Optional[Path] = None,
     ) -> None:
-        if self._is_custom_component(name_or_path):
-            self.component_dir = Path(name_or_path)
-        else:
-            self.component_dir = self._get_registry_path(str(name_or_path))
-
+        self.image = image
+        self.component_spec = component_spec
         self.input_partition_rows = input_partition_rows
-        self.component_spec = ComponentSpec.from_file(
-            self.component_dir / self.COMPONENT_SPEC_NAME,
-        )
-        self.name = self.component_spec.component_folder_name
         self.cache = self._configure_caching_from_image_tag(cache)
         self.cluster_type = cluster_type
         self.client_kwargs = client_kwargs
+        self.component_dir = component_dir
 
         self.operation_spec = OperationSpec(
             self.component_spec,
             consumes=consumes,
             produces=produces,
         )
 
@@ -177,14 +180,97 @@
             },
         )
 
         self.arguments.setdefault("operation_spec", self.operation_spec.to_json())
 
         self.resources = resources or Resources()
 
+    @classmethod
+    def from_component_yaml(cls, path, **kwargs) -> "ComponentOp":
+        if cls._is_custom_component(path):
+            component_dir = Path(path)
+        else:
+            component_dir = cls._get_registry_path(str(path))
+        component_spec = ComponentSpec.from_file(
+            component_dir / cls.COMPONENT_SPEC_NAME,
+        )
+
+        image = Image(
+            base_image=component_spec.image,
+        )
+        return cls(
+            image=image,
+            component_spec=component_spec,
+            component_dir=component_dir,
+            **kwargs,
+        )
+
+    @classmethod
+    def from_ref(
+        cls,
+        ref: t.Any,
+        fields: t.Optional[t.Mapping[str, Field]] = None,
+        **kwargs,
+    ) -> "ComponentOp":
+        """Create a ComponentOp from a reference. The reference can
+        be a reusable component name, a path to a custom component,
+        or a python component class.
+
+        Args:
+            ref: The name of a reusable component, or the path to the directory containing
+                a custom component, or a python component class.
+            fields: The fields of the dataset available to the component.
+            **kwargs: The provided user arguments are passed in as keyword arguments
+        """
+        if inspect.isclass(ref) and issubclass(ref, BaseComponent):
+            if issubclass(ref, LightweightComponent):
+                name = ref.__name__
+                image = ref.image()
+                description = ref.__doc__ or "lightweight component"
+                spec_produces = ref.get_spec_produces()
+
+                spec_consumes = (
+                    ref.get_spec_consumes(fields, kwargs["consumes"])
+                    if fields
+                    else {"additionalProperties": True}
+                )
+
+                component_spec = ComponentSpec(
+                    name,
+                    image.base_image,
+                    description=description,
+                    consumes=spec_consumes,
+                    produces=spec_produces,
+                    args={
+                        name: arg.to_spec()
+                        for name, arg in infer_arguments(ref).items()
+                    },
+                )
+
+                operation = cls(
+                    image,
+                    component_spec,
+                    **kwargs,
+                )
+            else:
+                msg = """Reference is not a valid lightweight component.
+                       Make sure the component is decorated properly."""
+                raise InvalidLightweightComponent(msg)
+
+        elif isinstance(ref, (str, Path)):
+            operation = cls.from_component_yaml(
+                ref,
+                **kwargs,
+            )
+        else:
+            msg = f"""Invalid reference type: {type(ref)}.
+                Expected a string, Path, or a lightweight component class."""
+            raise ValueError(msg)
+        return operation
+
     def _configure_caching_from_image_tag(
         self,
         cache: t.Optional[bool],
     ) -> t.Optional[bool]:
         """
         Adjusts the caching setting based on the image tag of the component.
 
@@ -201,26 +287,28 @@
 
         """
         if cache is True:
             image_tag = self.component_spec.image.rsplit(":")[-1]
 
             if image_tag == "latest":
                 logger.warning(
-                    f"Component `{self.name}` has an image tag set to latest. "
+                    f"Component `{self.component_spec.name}` has an image tag set to latest. "
                     f"Caching for the component will be disabled to prevent"
                     f" unpredictable behavior due to images updates",
                 )
                 return False
 
         return cache
 
     @property
     def dockerfile_path(self) -> t.Optional[Path]:
-        path = self.component_dir / "Dockerfile"
-        return path if path.exists() else None
+        if not self.component_dir:
+            return None
+        docker_path = self.component_dir / "Dockerfile"
+        return docker_path if docker_path.exists() else None
 
     @staticmethod
     def _is_custom_component(path_or_name: t.Union[str, Path]) -> bool:
         """Checks if name is a local path and a custom component."""
         component_dir: Path = Path(path_or_name)
         return component_dir.exists() and component_dir.is_dir()
 
@@ -229,14 +317,18 @@
         """Checks if name is a local path and a custom component."""
         component_dir: Path = t.cast(Path, files("fondant") / f"components/{name}")
         if not (component_dir.exists() and component_dir.is_dir()):
             msg = f"No reusable component with name {name} found."
             raise ValueError(msg)
         return component_dir
 
+    @property
+    def component_name(self) -> str:
+        return self.component_spec.safe_name
+
     def get_component_cache_key(
         self,
         previous_component_cache: t.Optional[str] = None,
     ) -> str:
         """Calculate a cache key representing the unique identity of this ComponentOp.
 
         The cache key is computed based on the component specification, image hash, arguments, and
@@ -256,26 +348,31 @@
             Returns:
                 The hash value (MD5 digest) of the nested dictionary.
             """
             sorted_json_string = json.dumps(input_dict, sort_keys=True)
             hash_object = hashlib.md5(sorted_json_string.encode())  # nosec
             return hash_object.hexdigest()
 
-        component_spec_dict = self.component_spec.specification
+        operation_spec_dict = self.operation_spec.to_dict()
+        image_dict = self.image.to_dict()
+
         arguments = (
             get_nested_dict_hash(self.arguments) if self.arguments is not None else None
         )
 
         component_op_uid_dict = {
-            "component_spec_hash": get_nested_dict_hash(component_spec_dict),
+            "operation_spec_hash": get_nested_dict_hash(operation_spec_dict),
+            "image": get_nested_dict_hash(image_dict),
             "arguments": arguments,
             "input_partition_rows": self.input_partition_rows,
             "number_of_accelerators": self.resources.accelerator_number,
             "accelerator_name": self.resources.accelerator_name,
             "node_pool_name": self.resources.node_pool_name,
+            "cluster_type": self.cluster_type,
+            "client_kwargs": self.client_kwargs,
         }
 
         if previous_component_cache is not None:
             component_op_uid_dict["previous_component_cache"] = previous_component_cache
 
         return get_nested_dict_hash(component_op_uid_dict)
 
@@ -309,42 +406,42 @@
         self,
         operation: ComponentOp,
         *,
         input_dataset: t.Optional["Dataset"],
         output_dataset: t.Optional["Dataset"],
     ) -> None:
         dependencies = []
-        for operation_name, info in self._graph.items():
+        for component_name, info in self._graph.items():
             if info["output_dataset"] == input_dataset:
-                dependencies.append(operation_name)
+                dependencies.append(component_name)
 
-        self._graph[operation.name] = {
+        self._graph[operation.component_name] = {
             "operation": operation,
             "dependencies": dependencies,
             "output_dataset": output_dataset,
         }
 
     def read(
         self,
-        name_or_path: t.Union[str, Path],
+        ref: t.Any,
         *,
         produces: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]] = None,
         arguments: t.Optional[t.Dict[str, t.Any]] = None,
         input_partition_rows: t.Optional[t.Union[int, str]] = None,
         resources: t.Optional[Resources] = None,
         cache: t.Optional[bool] = True,
         cluster_type: t.Optional[str] = "default",
         client_kwargs: t.Optional[dict] = None,
     ) -> "Dataset":
         """
         Read data using the provided component.
 
         Args:
-            name_or_path: The name of a reusable component, or the path to the directory containing
-                a custom component.
+            ref: The name of a reusable component, or the path to the directory containing
+                a containerized component, or a lightweight component class.
             produces: A mapping to update the fields produced by the operation as defined in the
                 component spec. The keys are the names of the fields to be received by the
                 component, while the values are the type of the field, or the name of the field to
                 map from the dataset.
             arguments: A dictionary containing the argument name and value for the operation.
             input_partition_rows: The number of rows to load per partition. Set to override the
             automatic partitioning
@@ -358,30 +455,29 @@
         """
         if self._graph:
             msg = "For now, at most one read component can be applied per pipeline."
             raise InvalidPipelineDefinition(
                 msg,
             )
 
-        operation = ComponentOp(
-            name_or_path,
+        operation = ComponentOp.from_ref(
+            ref,
             produces=produces,
             arguments=arguments,
             input_partition_rows=input_partition_rows,
             resources=resources,
             cache=cache,
             cluster_type=cluster_type,
             client_kwargs=client_kwargs,
         )
-
         manifest = Manifest.create(
             pipeline_name=self.name,
             base_path=self.base_path,
             run_id=self.get_run_id(),
-            component_id=operation.name,
+            component_id=operation.component_name,
         )
         dataset = Dataset(manifest, pipeline=self)
 
         return dataset._apply(operation)
 
     def sort_graph(self):
         """Sort the graph topologically based on task dependencies."""
@@ -466,16 +562,16 @@
                 # Check subset exists
                 for (
                     component_field_name,
                     component_field,
                 ) in operation_spec.outer_consumes.items():
                     if component_field_name not in manifest.fields:
                         msg = (
-                            f"Component '{component_op.name}' is trying to invoke the field "
-                            f"'{component_field_name}', which has not been defined or created "
+                            f"Component '{component_op.component_name}' is trying to invoke the"
+                            f"field '{component_field_name}', which has not been defined or created"
                             f"in the previous components. \n"
                             f"Available field names: {list(manifest.fields.keys())}"
                         )
                         raise InvalidPipelineDefinition(
                             msg,
                         )
 
@@ -542,31 +638,31 @@
                 output_dataset=evolved_dataset,
             )
 
         return evolved_dataset
 
     def apply(
         self,
-        name_or_path: t.Union[str, Path],
+        ref: t.Any,
         *,
         consumes: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]] = None,
         produces: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]] = None,
         arguments: t.Optional[t.Dict[str, t.Any]] = None,
         input_partition_rows: t.Optional[t.Union[int, str]] = None,
         resources: t.Optional[Resources] = None,
         cache: t.Optional[bool] = True,
         cluster_type: t.Optional[str] = "default",
         client_kwargs: t.Optional[dict] = None,
     ) -> "Dataset":
         """
         Apply the provided component on the dataset.
 
         Args:
-            name_or_path: The name of a reusable component, or the path to the directory containing
-                a custom component.
+            ref: The name of a reusable component, or the path to the directory containing
+                a custom component, or a lightweight component class.
             consumes: A mapping to update the fields consumed by the operation as defined in the
                 component spec. The keys are the names of the fields to be received by the
                 component, while the values are the type of the field, or the name of the field to
                 map from the input dataset.
 
                 Suppose we have a component spec that expects the following fields:
 
@@ -642,45 +738,47 @@
             cache: Set to False to disable caching, True by default.
             cluster_type: The type of cluster to use for distributed execution (default is "local").
             client_kwargs: Keyword arguments used to initialise the Dask client.
 
         Returns:
             An intermediate dataset.
         """
-        operation = ComponentOp(
-            name_or_path,
-            consumes=consumes,
+        operation = ComponentOp.from_ref(
+            ref,
+            fields=self.fields,
             produces=produces,
+            consumes=consumes,
             arguments=arguments,
             input_partition_rows=input_partition_rows,
             resources=resources,
             cache=cache,
             cluster_type=cluster_type,
             client_kwargs=client_kwargs,
         )
+
         return self._apply(operation)
 
     def write(
         self,
-        name_or_path: t.Union[str, Path],
+        ref: t.Any,
         *,
         consumes: t.Optional[t.Dict[str, t.Union[str, pa.DataType]]] = None,
         arguments: t.Optional[t.Dict[str, t.Any]] = None,
         input_partition_rows: t.Optional[t.Union[int, str]] = None,
         resources: t.Optional[Resources] = None,
         cache: t.Optional[bool] = True,
         cluster_type: t.Optional[str] = "default",
         client_kwargs: t.Optional[dict] = None,
     ) -> None:
         """
         Write the dataset using the provided component.
 
         Args:
-            name_or_path: The name of a reusable component, or the path to the directory containing
-                a custom component.
+            ref: The name of a reusable component, or the path to the directory containing
+                a custom component, or a lightweight component class.
             consumes: A mapping to update the fields consumed by the operation as defined in the
                 component spec. The keys are the names of the fields to be received by the
                 component, while the values are the type of the field, or the name of the field to
                 map from the input dataset.
             arguments: A dictionary containing the argument name and value for the operation.
             input_partition_rows: The number of rows to load per partition. Set to override the
             automatic partitioning
@@ -688,16 +786,17 @@
             cache: Set to False to disable caching, True by default.
             cluster_type: The type of cluster to use for distributed execution (default is "local").
             client_kwargs: Keyword arguments used to initialise the Dask client.
 
         Returns:
             An intermediate dataset.
         """
-        operation = ComponentOp(
-            name_or_path,
+        operation = ComponentOp.from_ref(
+            ref,
+            fields=self.fields,
             consumes=consumes,
             arguments=arguments,
             input_partition_rows=input_partition_rows,
             resources=resources,
             cache=cache,
             cluster_type=cluster_type,
             client_kwargs=client_kwargs,
```

### Comparing `fondant-0.9.dev2/src/fondant/pipeline/runner.py` & `fondant-1.0.0/src/fondant/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `fondant-0.9.dev2/src/fondant/testing.py` & `fondant-1.0.0/src/fondant/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         cpu_request: CPU request for the component.
         cpu_limit: CPU limit for the component.
         memory_request: Memory request for the component.
         memory_limit: Memory limit for the component.
     """
 
     image: t.Optional[str] = None
+    command: t.Optional[t.List[str]] = None
     arguments: t.Optional[t.Dict[str, t.Any]] = None
     dependencies: t.Optional[t.List[str]] = None
     accelerators: t.Optional[t.List[Accelerator]] = None
     cpu_request: t.Optional[str] = None
     cpu_limit: t.Optional[str] = None
     memory_request: t.Optional[str] = None
     memory_limit: t.Optional[str] = None
@@ -245,14 +246,15 @@
             if dependencies:
                 dependencies = [
                     dependency.replace("-", "_") for dependency in dependencies
                 ]
 
             component_config = KubeflowComponentConfig(
                 image=container_spec.get("image"),
+                command=container_spec.get("command"),
                 arguments=arguments,
                 dependencies=dependencies,
                 accelerators=accelerator_list,
                 cpu_request=component_configs.get("cpuRequest", None),
                 cpu_limit=component_configs.get("cpuLimit", None),
                 memory_request=component_configs.get("memoryRequest", None),
                 memory_limit=component_configs.get("memoryLimit", None),
```

### Comparing `fondant-0.9.dev2/PKG-INFO` & `fondant-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: fondant
-Version: 0.9.dev2
+Version: 1.0.0
 Summary: Fondant - Large-scale data processing made easy and reusable
 Home-page: https://github.com/ml6team/fondant
 License: Apache-2.0
 Keywords: data,machine learning,fine-tuning,foundation models
 Author: ML6
 Author-email: fondant@ml6.eu
 Maintainer: ML6
 Maintainer-email: fondant@ml6.eu
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: component
@@ -38,15 +38,15 @@
 Requires-Dist: dask[dataframe,diagnostics,distributed] (>=2023.4.1) ; extra == "component"
 Requires-Dist: docker (>=6.1.3) ; extra == "kfp" or extra == "vertex" or extra == "docker"
 Requires-Dist: fsspec (>=2023.4.0)
 Requires-Dist: gcsfs (>=2023.10.0) ; extra == "gcp"
 Requires-Dist: google-cloud-aiplatform (==1.34.0) ; extra == "vertex"
 Requires-Dist: importlib-resources (>=1.3) ; python_version < "3.9"
 Requires-Dist: jsonschema (>=4.18)
-Requires-Dist: kfp[kubernetes] (==2.3.0) ; extra == "kfp" or extra == "vertex"
+Requires-Dist: kfp[kubernetes] (==2.6.0) ; extra == "kfp" or extra == "vertex"
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: s3fs (>=2023.4.0) ; extra == "aws"
 Requires-Dist: sagemaker (>=2.197.0) ; extra == "sagemaker"
 Project-URL: Repository, https://github.com/ml6team/fondant
 Description-Content-Type: text/markdown
 
@@ -153,17 +153,14 @@
 
 🛋️ [**ControlNet Interior Design Pipeline**](https://github.com/ml6team/fondant-usecase-controlnet)  
 An end-to-end Fondant pipeline to collect and process data for the fine-tuning of a ControlNet model, focusing on images related to interior design.
 
 🖼️ [**Filter creative common license images**](https://github.com/ml6team/fondant-usecase-filter-creative-commons)  
 An end-to-end Fondant pipeline that starts from our Fondant-CC-25M creative commons image dataset and filters and downloads the desired images.
 
-🔢 [**Datacomp pipeline**](https://github.com/ml6team/fondant-usecase-datacomp)  
-An end-to-end Fondant pipeline filtering image-text data to train a CLIP model for the DataComp competition.
-
 ## ⚒️ Installation
 
 Fondant can be installed using pip:
 
 ```
 pip install fondant
 ```
@@ -238,15 +235,15 @@
 ```python
 import pandas as pd
 from fondant.component import PandasTransformComponent
 
 
 class ExampleComponent(PandasTransformComponent):
 
-    def __init__(self, *, argument1, argument2, **kwargs) -> None:
+    def __init__(self, *, argument1, argument2) -> None:
         """
         Args:
             argumentX: An argument passed to the component
         """
         # Initialize your component here based on the arguments
 
     def transform(self, dataframe: pd.DataFrame) -> pd.DataFrame:
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: fondant Version: 0.9.dev2 Summary: Fondant - Large-
+Metadata-Version: 2.1 Name: fondant Version: 1.0.0 Summary: Fondant - Large-
 scale data processing made easy and reusable Home-page: https://github.com/
 ml6team/fondant License: Apache-2.0 Keywords: data,machine learning,fine-
 tuning,foundation models Author: ML6 Author-email: fondant@ml6.eu Maintainer:
-ML6 Maintainer-email: fondant@ml6.eu Requires-Python: >=3.8,<3.11 Classifier:
+ML6 Maintainer-email: fondant@ml6.eu Requires-Python: >=3.8,<3.12 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.11 Classifier: Topic :: Software Development Classifier: Topic :: Software
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Typing :: Typed Provides-Extra: aws Provides-
 Extra: azure Provides-Extra: component Provides-Extra: docker Provides-Extra:
 gcp Provides-Extra: kfp Provides-Extra: sagemaker Provides-Extra: vertex
 Requires-Dist: adlfs (>=2023.4.0) ; extra == "azure" Requires-Dist: boto3
 (==1.28.64) ; extra == "sagemaker" Requires-Dist: dask
 [dataframe,diagnostics,distributed] (>=2023.4.1) ; extra == "component"
 Requires-Dist: docker (>=6.1.3) ; extra == "kfp" or extra == "vertex" or extra
 == "docker" Requires-Dist: fsspec (>=2023.4.0) Requires-Dist: gcsfs
 (>=2023.10.0) ; extra == "gcp" Requires-Dist: google-cloud-aiplatform
 (==1.34.0) ; extra == "vertex" Requires-Dist: importlib-resources (>=1.3) ;
 python_version < "3.9" Requires-Dist: jsonschema (>=4.18) Requires-Dist: kfp
-[kubernetes] (==2.3.0) ; extra == "kfp" or extra == "vertex" Requires-Dist:
+[kubernetes] (==2.6.0) ; extra == "kfp" or extra == "vertex" Requires-Dist:
 pyarrow (>=11.0.0) Requires-Dist: pyyaml (>=5.3.1) Requires-Dist: s3fs
 (>=2023.4.0) ; extra == "aws" Requires-Dist: sagemaker (>=2.197.0) ; extra ==
 "sagemaker" Project-URL: Repository, https://github.com/ml6team/fondant
 Description-Content-Type: text/markdown
        [https://raw.githubusercontent.com/ml6team/fondant/main/docs/art/
                               fondant_banner.svg]
            PPrroodduuccttiioonn--rreeaaddyy data processing made eeaassyy and sshhaarreeaabbllee
@@ -78,53 +78,50 @@
 RAG (Retrieval-Augmented Generation) systems. ðï¸ [**ControlNet Interior
 Design Pipeline**](https://github.com/ml6team/fondant-usecase-controlnet) An
 end-to-end Fondant pipeline to collect and process data for the fine-tuning of
 a ControlNet model, focusing on images related to interior design. ð¼ï¸
 [**Filter creative common license images**](https://github.com/ml6team/fondant-
 usecase-filter-creative-commons) An end-to-end Fondant pipeline that starts
 from our Fondant-CC-25M creative commons image dataset and filters and
-downloads the desired images. ð¢ [**Datacomp pipeline**](https://github.com/
-ml6team/fondant-usecase-datacomp) An end-to-end Fondant pipeline filtering
-image-text data to train a CLIP model for the DataComp competition. ## âï¸
-Installation Fondant can be installed using pip: ``` pip install fondant ```
-For more detailed installation options, check the [**installation page**]
-(https://fondant.ai/en/latest/guides/installation/) on our documentation. ##
-ð¨âð» Usage #### Pipeline Fondant allows you to easily define data
-pipelines comprised of both reusable and custom components. The following
-pipeline for instance uses the reusable `load_from_hf_hub` component to load a
-dataset from the Hugging Face Hub and process it using a custom component:
-**_pipeline.py_** ```python from fondant.pipeline import Pipeline pipeline =
-Pipeline(pipeline_name="example pipeline", base_path="fs://bucket") dataset =
-pipeline.read( "load_from_hf_hub", arguments={ "dataset_name": "lambdalabs/
-pokemon-blip-captions" }, ) dataset = dataset.apply( "components/
-custom_component", arguments={ "min_width": 600, "min_height": 600, }, ) ```
-#### Component To create a custom component, you first need to describe its
-contract as a yaml specification. It defines the data consumed and produced by
-the component and any arguments it takes. **_fondant_component.yaml_** ```yaml
-name: Custom component description: This is a custom component image:
-custom_component:latest consumes: image: type: binary produces: caption: type:
-utf8 args: argument1: description: An argument passed to the component at
-runtime type: str argument2: description: Another argument passed to the
-component at runtime type: str ``` Once you have your component specification,
-all you need to do is implement a constructor and a single `.transform` method
-and Fondant will do the rest. You will get the data defined in your
-specification partition by partition as a Pandas dataframe. **_component/src/
-main.py_** ```python import pandas as pd from fondant.component import
-PandasTransformComponent class ExampleComponent(PandasTransformComponent): def
-__init__(self, *, argument1, argument2, **kwargs) -> None: """ Args: argumentX:
-An argument passed to the component """ # Initialize your component here based
-on the arguments def transform(self, dataframe: pd.DataFrame) -> pd.DataFrame:
-"""Implement your custom logic in this single method Args: dataframe: A Pandas
-dataframe containing the data Returns: A pandas dataframe containing the
-transformed data """ ``` For more advanced use cases, you can use the
-`DaskTransformComponent` instead. ### Running your pipeline Once you have a
-pipeline you can easily run (and compile) it by using the built-in CLI: ```bash
-fondant run local pipeline.py ``` To see all available runner and arguments you
-can check the fondant CLI help pages ```bash fondant --help ``` Or for a
-subcommand: ```bash fondant --help ```
+downloads the desired images. ## âï¸ Installation Fondant can be installed
+using pip: ``` pip install fondant ``` For more detailed installation options,
+check the [**installation page**](https://fondant.ai/en/latest/guides/
+installation/) on our documentation. ## ð¨âð» Usage #### Pipeline Fondant
+allows you to easily define data pipelines comprised of both reusable and
+custom components. The following pipeline for instance uses the reusable
+`load_from_hf_hub` component to load a dataset from the Hugging Face Hub and
+process it using a custom component: **_pipeline.py_** ```python from
+fondant.pipeline import Pipeline pipeline = Pipeline(pipeline_name="example
+pipeline", base_path="fs://bucket") dataset = pipeline.read
+( "load_from_hf_hub", arguments={ "dataset_name": "lambdalabs/pokemon-blip-
+captions" }, ) dataset = dataset.apply( "components/custom_component",
+arguments={ "min_width": 600, "min_height": 600, }, ) ``` #### Component To
+create a custom component, you first need to describe its contract as a yaml
+specification. It defines the data consumed and produced by the component and
+any arguments it takes. **_fondant_component.yaml_** ```yaml name: Custom
+component description: This is a custom component image: custom_component:
+latest consumes: image: type: binary produces: caption: type: utf8 args:
+argument1: description: An argument passed to the component at runtime type:
+str argument2: description: Another argument passed to the component at runtime
+type: str ``` Once you have your component specification, all you need to do is
+implement a constructor and a single `.transform` method and Fondant will do
+the rest. You will get the data defined in your specification partition by
+partition as a Pandas dataframe. **_component/src/main.py_** ```python import
+pandas as pd from fondant.component import PandasTransformComponent class
+ExampleComponent(PandasTransformComponent): def __init__(self, *, argument1,
+argument2) -> None: """ Args: argumentX: An argument passed to the component
+""" # Initialize your component here based on the arguments def transform(self,
+dataframe: pd.DataFrame) -> pd.DataFrame: """Implement your custom logic in
+this single method Args: dataframe: A Pandas dataframe containing the data
+Returns: A pandas dataframe containing the transformed data """ ``` For more
+advanced use cases, you can use the `DaskTransformComponent` instead. ###
+Running your pipeline Once you have a pipeline you can easily run (and compile)
+it by using the built-in CLI: ```bash fondant run local pipeline.py ``` To see
+all available runner and arguments you can check the fondant CLI help pages
+```bash fondant --help ``` Or for a subcommand: ```bash fondant --help ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## ð­ Contributing We welcome contributions of different kinds: | | | |------
 ----------------------------|--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
```


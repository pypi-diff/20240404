# Comparing `tmp/imagespec_fast_builder-0.0.7.tar.gz` & `tmp/imagespec_fast_builder-0.0.8.tar.gz`

## Comparing `imagespec_fast_builder-0.0.7.tar` & `imagespec_fast_builder-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/.github/workflows/wheel.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile.base
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/experiments/build_wf.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/experiments/check_builder.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/__init__.py
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/_image_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/LICENSE
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/README.md
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/.github/workflows/wheel.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile.base
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/experiments/build_wf.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/experiments/check_builder.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/__init__.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/_image_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/README.md
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/PKG-INFO
```

### Comparing `imagespec_fast_builder-0.0.7/.github/workflows/wheel.yaml` & `imagespec_fast_builder-0.0.8/.github/workflows/wheel.yaml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile` & `imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/experiments/check_builder.py` & `imagespec_fast_builder-0.0.8/experiments/check_builder.py`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/_image_builder.py` & `imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/_image_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 )
 
 PYTHON_INSTALL_COMMAND = """\
 RUN --mount=type=cache,target=/root/.cache/uv,id=uv \
     --mount=type=bind,target=requirements.txt,src=requirements.txt \
     /root/.cargo/bin/uv \
     pip install --python /opt/conda/envs/dev/bin/python $PIP_INDEX \
-    --verbose \
     --requirement requirements.txt
 """
 
 APT_INSTALL_COMMAND_TEMPLATE = Template(
     """\
 RUN --mount=type=cache,target=/var/cache/apt,id=apt \
     apt-get update && apt-get install -y --no-install-recommends \
@@ -33,18 +32,22 @@
 
 DOCKER_FILE_TEMPLATE = Template(
     """\
 #syntax=docker/dockerfile:1.5
 FROM thomasjpfan/fast-builder-base:0.0.1 as build
 
 RUN --mount=type=cache,target=/opt/conda/pkgs,id=conda \
-    mamba create --verbose \
+    mamba create \
         -c conda-forge $CONDA_CHANNELS \
         -n dev -y python=$PYTHON_VERSION $CONDA_PACKAGES
 
+WORKDIR /root
+
+$COPY_COMMAND
+
 $PYTHON_INSTALL_COMMAND
 
 RUN /opt/conda/bin/conda-pack -n dev -o /tmp/env.tar && \
     mkdir /venv && cd /venv && tar xf /tmp/env.tar && \
     rm /tmp/env.tar
 
 RUN /venv/bin/conda-unpack
```

### Comparing `imagespec_fast_builder-0.0.7/.gitignore` & `imagespec_fast_builder-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/LICENSE` & `imagespec_fast_builder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/README.md` & `imagespec_fast_builder-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/pyproject.toml` & `imagespec_fast_builder-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.7/PKG-INFO` & `imagespec_fast_builder-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: imagespec-fast-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: A faster ImageSpec builder for flytekit
 Project-URL: Issues, https://github.com/thomasjpfan/imagespec-fast-builder/issues
 Project-URL: Source, https://github.com/thomasjpfan/imagespec-fast-builder
 Author-email: "Thomas J. Fan" <thomasjpfan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/jupyter_nebulagraph-0.10.0.tar.gz` & `tmp/jupyter_nebulagraph-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_nebulagraph-0.10.0.tar", last modified: Thu Apr  4 06:44:16 2024, max compression
+gzip compressed data, was "jupyter_nebulagraph-0.9.1.tar", last modified: Thu Apr  4 03:35:06 2024, max compression
```

## Comparing `jupyter_nebulagraph-0.10.0.tar` & `jupyter_nebulagraph-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:44:16.882446 jupyter_nebulagraph-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 06:44:13.000000 jupyter_nebulagraph-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-04 06:44:16.882446 jupyter_nebulagraph-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-04 06:44:13.000000 jupyter_nebulagraph-0.10.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:44:16.878446 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-04 06:44:16.000000 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 06:44:16.000000 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:44:16.000000 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 06:44:16.000000 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 06:44:16.000000 jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:44:16.878446 jupyter_nebulagraph-0.10.0/ngql/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 06:44:13.000000 jupyter_nebulagraph-0.10.0/ngql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36452 2024-04-04 06:44:13.000000 jupyter_nebulagraph-0.10.0/ngql/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:44:16.882446 jupyter_nebulagraph-0.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 06:44:13.000000 jupyter_nebulagraph-0.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/ngql/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36253 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/setup.py
```

### Comparing `jupyter_nebulagraph-0.10.0/LICENSE` & `jupyter_nebulagraph-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_nebulagraph-0.10.0/PKG-INFO` & `jupyter_nebulagraph-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyter_nebulagraph
-Version: 0.10.0
+Version: 0.9.1
 Summary: Jupyter extension for NebulaGraph
 Home-page: https://github.com/wey-gu/jupyter_nebulagraph
 Author: Wey Gu
 Author-email: weyl.gu@gmail.com
 Project-URL: Bug Tracker, https://github.com/wey-gu/jupyter_nebulagraph/issues
-Project-URL: Documentation, https://jupyter-nebulagraph.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2
@@ -18,35 +17,33 @@
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: pyvis
 
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
 [![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
-[![Documentation](https://img.shields.io/badge/docs-Read%20The%20Docs-blue)](https://jupyter-nebulagraph.readthedocs.io/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
-
 `jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
-Or check [Docs: Get Started](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started/).
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
 `jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
@@ -100,14 +97,16 @@
 
 ```python
 %%ngql
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
+> There will be other options in future, i.e. from a `.ngql` file.
+
 ### Query String with Variables
 
 `jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
@@ -244,15 +243,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here: [get_started.ipynb](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `jupyter_nebulagraph-0.10.0/README.md` & `jupyter_nebulagraph-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
 [![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
-[![Documentation](https://img.shields.io/badge/docs-Read%20The%20Docs-blue)](https://jupyter-nebulagraph.readthedocs.io/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
-
 `jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
-Or check [Docs: Get Started](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started/).
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
 `jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
@@ -79,14 +77,16 @@
 
 ```python
 %%ngql
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
+> There will be other options in future, i.e. from a `.ngql` file.
+
 ### Query String with Variables
 
 `jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
@@ -223,15 +223,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here: [get_started.ipynb](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `jupyter_nebulagraph-0.10.0/jupyter_nebulagraph.egg-info/PKG-INFO` & `jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyter_nebulagraph
-Version: 0.10.0
+Version: 0.9.1
 Summary: Jupyter extension for NebulaGraph
 Home-page: https://github.com/wey-gu/jupyter_nebulagraph
 Author: Wey Gu
 Author-email: weyl.gu@gmail.com
 Project-URL: Bug Tracker, https://github.com/wey-gu/jupyter_nebulagraph/issues
-Project-URL: Documentation, https://jupyter-nebulagraph.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2
@@ -18,35 +17,33 @@
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: pyvis
 
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
 [![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
-[![Documentation](https://img.shields.io/badge/docs-Read%20The%20Docs-blue)](https://jupyter-nebulagraph.readthedocs.io/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
-
 `jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
-Or check [Docs: Get Started](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started/).
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
 `jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
@@ -100,14 +97,16 @@
 
 ```python
 %%ngql
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
+> There will be other options in future, i.e. from a `.ngql` file.
+
 ### Query String with Variables
 
 `jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
@@ -244,15 +243,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here: [get_started.ipynb](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `jupyter_nebulagraph-0.10.0/ngql/magic.py` & `jupyter_nebulagraph-0.9.1/ngql/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -595,20 +595,18 @@
             else:
                 g_nx.add_node(node_id, **props)
         elif isinstance(item, Relationship):
             src_id = str(item.start_vertex_id().cast())
             dst_id = str(item.end_vertex_id().cast())
             edge_name = item.edge_name()
             props_raw = item.properties()
-            rank = item.ranking()
             props = {
                 k: str(v.cast()) if hasattr(v, "cast") else str(v)
                 for k, v in props_raw.items()
             }
-            props.update({"rank": rank})
             # ensure start and end vertex exist in graph
             if not src_id in g.node_ids:
                 g.add_node(
                     src_id,
                     label=str(src_id),
                     title=str(src_id),
                     color=get_color(src_id),
@@ -624,21 +622,15 @@
             for k in props:
                 if len(props_str_list) >= 1:
                     break
                 props_str_list.append(f"{truncate(k, 7)}: {truncate(str(props[k]), 8)}")
             props_str = "\n".join(props_str_list)
 
             label = f"{props_str}\n{edge_name}" if props else edge_name
-            g.add_edge(
-                src_id,
-                dst_id,
-                label=label,
-                title=str(props),
-                weight=props.get("rank", 0),
-            )
+            g.add_edge(src_id, dst_id, label=label, title=str(props))
             # networkx
             props["edge_type"] = edge_name
             g_nx.add_edge(src_id, dst_id, **props)
 
         elif isinstance(item, PathWrapper):
             for node in item.nodes():
                 self.render_pd_item(g, g_nx, node)
```

### Comparing `jupyter_nebulagraph-0.10.0/setup.py` & `jupyter_nebulagraph-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jupyter_nebulagraph",
-    version="0.10.0",
+    version="0.9.1",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
     description="Jupyter extension for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wey-gu/jupyter_nebulagraph",
     project_urls={
         "Bug Tracker": "https://github.com/wey-gu/jupyter_nebulagraph/issues",
-        "Documentation": "https://jupyter-nebulagraph.readthedocs.io/",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
```


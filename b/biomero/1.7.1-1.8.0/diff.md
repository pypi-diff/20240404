# Comparing `tmp/biomero-1.7.1.tar.gz` & `tmp/biomero-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-axp787tl/biomero-1.7.1.tar", last modified: Thu Apr  4 13:16:45 2024, max compression
+gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-dorewbl_/biomero-1.8.0.tar", last modified: Thu Apr  4 16:17:46 2024, max compression
```

## Comparing `biomero-1.7.1.tar` & `biomero-1.8.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 13:16:39.000000 biomero-1.7.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 13:16:39.000000 biomero-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 13:16:39.000000 biomero-1.7.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 13:16:39.000000 biomero-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 13:16:39.000000 biomero-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 13:16:45.000000 biomero-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-04 13:16:39.000000 biomero-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    78613 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/slurm_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/omero_slurm_client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/tutorial_link.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 13:16:39.000000 biomero-1.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_job_array.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_zarr_to_tiff.def
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_zarr_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/example.config
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/job_template.sh
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/pull_images.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/slurm-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/Cells.tif
--rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/cellexpansion.png
--rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/gc_allow_ssh.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/nuclei_labels.png
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_init_env.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_init_env_done.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_run_cellpose.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_run_workflow.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_Azure_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_GoogleCloud_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_cellexpansion.md
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_cellprofiler.md
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_local_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:16:45.000000 biomero-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45151 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/unit/test_slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 16:17:39.000000 biomero-1.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 16:17:39.000000 biomero-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 16:17:39.000000 biomero-1.8.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 16:17:39.000000 biomero-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:17:39.000000 biomero-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 16:17:46.000000 biomero-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-04 16:17:39.000000 biomero-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79394 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/omero_slurm_client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/tutorial_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 16:17:39.000000 biomero-1.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_job_array.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_zarr_to_tiff.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_zarr_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/job_template.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/pull_images.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/slurm-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/Cells.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/cellexpansion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/gc_allow_ssh.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/nuclei_labels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_init_env.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_init_env_done.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_run_cellpose.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_run_workflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_Azure_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_cellexpansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_cellprofiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_local_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:17:46.000000 biomero-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45207 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/unit/test_slurm_client.py
```

### Comparing `biomero-1.7.1/.github/workflows/python-package.yml` & `biomero-1.8.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/.github/workflows/python-publish.yml` & `biomero-1.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/.github/workflows/sphinx.yml` & `biomero-1.8.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/.gitignore` & `biomero-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/CITATION.cff` & `biomero-1.8.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/LICENSE` & `biomero-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/PKG-INFO` & `biomero-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.7.1
+Version: 1.8.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.7.1/README.md` & `biomero-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/biomero/constants.py` & `biomero-1.8.0/biomero/constants.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/biomero/slurm_client.py` & `biomero-1.8.0/biomero/slurm_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,4732 +183,4781 @@
 00000b60: 2020 2020 2020 2020 2020 2066 2259 6f75             f"You
 00000b70: 2063 616e 2067 6574 2074 6865 206c 6f67   can get the log
 00000b80: 6669 6c65 2075 7369 6e67 2060 536c 7572  file using `Slur
 00000b90: 6d20 4765 7420 5570 6461 7465 6020 6f6e  m Get Update` on
 00000ba0: 206a 6f62 207b 7365 6c66 2e6a 6f62 5f69   job {self.job_i
 00000bb0: 647d 2229 0a20 2020 2020 2020 2072 6574  d}").        ret
 00000bc0: 7572 6e20 7365 6c66 2e6a 6f62 5f73 7461  urn self.job_sta
-00000bd0: 7465 0a0a 2020 2020 6465 6620 636f 6d70  te..    def comp
-00000be0: 6c65 7465 6428 7365 6c66 293a 0a20 2020  leted(self):.   
-00000bf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00000c00: 2043 6865 636b 2069 6620 7468 6520 536c   Check if the Sl
-00000c10: 7572 6d20 6a6f 6220 6861 7320 636f 6d70  urm job has comp
-00000c20: 6c65 7465 6420 7375 6363 6573 7366 756c  leted successful
-00000c30: 6c79 2e0a 0a20 2020 2020 2020 2052 6574  ly...        Ret
-00000c40: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00000c50: 2020 626f 6f6c 3a20 5472 7565 2069 6620    bool: True if 
-00000c60: 7468 6520 6a6f 6220 6861 7320 636f 6d70  the job has comp
-00000c70: 6c65 7465 643b 2046 616c 7365 206f 7468  leted; False oth
-00000c80: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00000c90: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00000ca0: 726e 2073 656c 662e 6a6f 625f 7374 6174  rn self.job_stat
-00000cb0: 6520 3d3d 2022 434f 4d50 4c45 5445 4422  e == "COMPLETED"
-00000cc0: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-00000cd0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00000ce0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-00000cf0: 7572 6e20 6120 7374 7269 6e67 2072 6570  urn a string rep
-00000d00: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-00000d10: 6865 2053 6c75 726d 4a6f 6220 696e 7374  he SlurmJob inst
-00000d20: 616e 6365 2e0a 0a20 2020 2020 2020 2052  ance...        R
-00000d30: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00000d40: 2020 2020 7374 723a 2053 7472 696e 6720      str: String 
-00000d50: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
-00000d60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00000d70: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
-00000d80: 2027 2c20 272e 6a6f 696e 280a 2020 2020   ', '.join(.    
-00000d90: 2020 2020 2020 2020 6622 7b6b 6579 7d3d          f"{key}=
-00000da0: 7b76 616c 7565 7d22 2066 6f72 206b 6579  {value}" for key
-00000db0: 2c20 7661 6c75 6520 696e 2073 656c 662e  , value in self.
-00000dc0: 5f5f 6469 6374 5f5f 2e69 7465 6d73 2829  __dict__.items()
-00000dd0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00000de0: 2066 2253 6c75 726d 4a6f 6228 7b70 726f   f"SlurmJob({pro
-00000df0: 7065 7274 6965 737d 2922 0a0a 0a63 6c61  perties})"...cla
-00000e00: 7373 2053 6c75 726d 436c 6965 6e74 2843  ss SlurmClient(C
-00000e10: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
-00000e20: 2222 2241 2063 6c69 656e 7420 666f 7220  """A client for 
-00000e30: 636f 6e6e 6563 7469 6e67 2074 6f20 616e  connecting to an
-00000e40: 6420 696e 7465 7261 6374 696e 6720 7769  d interacting wi
-00000e50: 7468 2061 2053 6c75 726d 2063 6c75 7374  th a Slurm clust
-00000e60: 6572 206f 7665 720a 2020 2020 5353 482e  er over.    SSH.
-00000e70: 0a0a 2020 2020 5468 6973 2063 6c61 7373  ..    This class
-00000e80: 2065 7874 656e 6473 2074 6865 2043 6f6e   extends the Con
-00000e90: 6e65 6374 696f 6e20 636c 6173 732c 2061  nection class, a
-00000ea0: 6464 696e 6720 6d65 7468 6f64 7320 616e  dding methods an
-00000eb0: 640a 2020 2020 6174 7472 6962 7574 6573  d.    attributes
-00000ec0: 2073 7065 6369 6669 6320 746f 2077 6f72   specific to wor
-00000ed0: 6b69 6e67 2077 6974 6820 536c 7572 6d2e  king with Slurm.
-00000ee0: 0a0a 2020 2020 536c 7572 6d43 6c69 656e  ..    SlurmClien
-00000ef0: 7420 6163 6365 7074 7320 7468 6520 7361  t accepts the sa
-00000f00: 6d65 2061 7267 756d 656e 7473 2061 7320  me arguments as 
-00000f10: 436f 6e6e 6563 7469 6f6e 2e20 4265 6c6f  Connection. Belo
-00000f20: 7720 6f6e 6c79 0a20 2020 206d 656e 7469  w only.    menti
-00000f30: 6f6e 7320 7468 6520 6164 6465 6420 6f6e  ons the added on
-00000f40: 6573 3a0a 0a20 2020 2054 6865 2065 6173  es:..    The eas
-00000f50: 6965 7374 2077 6179 2074 6f20 7365 7420  iest way to set 
-00000f60: 7468 6973 2063 6c69 656e 7420 7570 2069  this client up i
-00000f70: 7320 6279 2075 7369 6e67 2061 2073 6c75  s by using a slu
-00000f80: 726d 2d63 6f6e 6669 672e 696e 690a 2020  rm-config.ini.  
-00000f90: 2020 616e 6420 7468 6520 6672 6f6d 2d63    and the from-c
-00000fa0: 6f6e 6669 6728 2920 6d65 7468 6f64 2e0a  onfig() method..
-00000fb0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
-00000fc0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
-00000fd0: 6174 615f 7061 7468 2028 7374 7229 3a20  ata_path (str): 
-00000fe0: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
-00000ff0: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
-00001000: 6e69 6e67 2074 6865 0a20 2020 2020 2020  ning the.       
-00001010: 2020 2020 2064 6174 6120 6669 6c65 7320       data files 
-00001020: 666f 7220 536c 7572 6d20 6a6f 6273 2e0a  for Slurm jobs..
-00001030: 2020 2020 2020 2020 736c 7572 6d5f 696d          slurm_im
-00001040: 6167 6573 5f70 6174 6820 2873 7472 293a  ages_path (str):
-00001050: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
-00001060: 2064 6972 6563 746f 7279 2063 6f6e 7461   directory conta
-00001070: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
-00001080: 2020 7468 6520 5369 6e67 756c 6172 6974    the Singularit
-00001090: 7920 696d 6167 6573 2066 6f72 2053 6c75  y images for Slu
-000010a0: 726d 206a 6f62 732e 0a20 2020 2020 2020  rm jobs..       
-000010b0: 2073 6c75 726d 5f63 6f6e 7665 7274 6572   slurm_converter
-000010c0: 735f 7061 7468 2028 7374 7229 3a20 5468  s_path (str): Th
-000010d0: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
-000010e0: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
-000010f0: 6e67 0a20 2020 2020 2020 2020 2020 2074  ng.            t
-00001100: 6865 2053 696e 6775 6c61 7269 7479 2069  he Singularity i
-00001110: 6d61 6765 7320 666f 7220 6669 6c65 2063  mages for file c
-00001120: 6f6e 7665 7274 6572 732e 0a20 2020 2020  onverters..     
-00001130: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-00001140: 6174 6873 2028 6469 6374 293a 2041 2064  aths (dict): A d
-00001150: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00001160: 6e69 6e67 2074 6865 2070 6174 6873 2074  ning the paths t
-00001170: 6f0a 2020 2020 2020 2020 2020 2020 7468  o.            th
-00001180: 6520 5369 6e67 756c 6172 6974 7920 696d  e Singularity im
-00001190: 6167 6573 2066 6f72 2073 7065 6369 6669  ages for specifi
-000011a0: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
-000011b0: 6c73 2e0a 2020 2020 2020 2020 736c 7572  ls..        slur
-000011c0: 6d5f 6d6f 6465 6c5f 7265 706f 7320 2864  m_model_repos (d
-000011d0: 6963 7429 3a20 4120 6469 6374 696f 6e61  ict): A dictiona
-000011e0: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
-000011f0: 6520 6769 740a 2020 2020 2020 2020 2020  e git.          
-00001200: 2020 7265 706f 7369 746f 7269 6573 206f    repositories o
-00001210: 6620 5369 6e67 756c 6172 6974 7920 696d  f Singularity im
-00001220: 6167 6573 2066 6f72 2073 7065 6369 6669  ages for specifi
-00001230: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
-00001240: 6c73 2e0a 2020 2020 2020 2020 736c 7572  ls..        slur
-00001250: 6d5f 6d6f 6465 6c5f 696d 6167 6573 2028  m_model_images (
-00001260: 6469 6374 293a 2041 2064 6963 7469 6f6e  dict): A diction
-00001270: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-00001280: 6865 2064 6f63 6b65 7268 7562 0a20 2020  he dockerhub.   
-00001290: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
-000012a0: 5369 6e67 756c 6172 6974 7920 696d 6167  Singularity imag
-000012b0: 6573 2066 6f72 2073 7065 6369 6669 6320  es for specific 
-000012c0: 536c 7572 6d20 6a6f 6220 6d6f 6465 6c73  Slurm job models
-000012d0: 2e0a 2020 2020 2020 2020 2020 2020 5769  ..            Wi
-000012e0: 6c6c 2066 696c 6c20 6175 746f 6d61 7469  ll fill automati
-000012f0: 6361 6c6c 7920 6672 6f6d 2074 6865 2064  cally from the d
-00001300: 6174 6120 696e 2074 6865 2067 6974 2072  ata in the git r
-00001310: 6570 6f73 6974 6f72 792c 0a20 2020 2020  epository,.     
-00001320: 2020 2020 2020 2069 6620 796f 7520 7365         if you se
-00001330: 7420 696e 6974 5f73 6c75 726d 2e0a 2020  t init_slurm..  
-00001340: 2020 2020 2020 736c 7572 6d5f 7363 7269        slurm_scri
-00001350: 7074 5f70 6174 6820 2873 7472 293a 2054  pt_path (str): T
-00001360: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
-00001370: 6972 6563 746f 7279 2063 6f6e 7461 696e  irectory contain
-00001380: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001390: 7468 6520 536c 7572 6d20 6a6f 6220 7375  the Slurm job su
-000013a0: 626d 6973 7369 6f6e 2073 6372 6970 7473  bmission scripts
-000013b0: 206f 6e20 536c 7572 6d2e 0a20 2020 2020   on Slurm..     
-000013c0: 2020 2073 6c75 726d 5f73 6372 6970 745f     slurm_script_
-000013d0: 7265 706f 2028 7374 7229 3a20 5468 6520  repo (str): The 
-000013e0: 6769 7420 6874 7470 7320 5552 4c20 666f  git https URL fo
-000013f0: 7220 636c 6f6e 696e 6720 7468 6520 7265  r cloning the re
-00001400: 706f 0a20 2020 2020 2020 2020 2020 2063  po.            c
-00001410: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
-00001420: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
-00001430: 6f6e 2073 6372 6970 7473 2e20 4f70 7469  on scripts. Opti
-00001440: 6f6e 616c 2e0a 0a20 2020 2045 7861 6d70  onal...    Examp
-00001450: 6c65 3a0a 2020 2020 2020 2020 2320 4372  le:.        # Cr
-00001460: 6561 7465 2061 2053 6c75 726d 436c 6965  eate a SlurmClie
-00001470: 6e74 206f 626a 6563 7420 6173 2063 6f6e  nt object as con
-00001480: 7465 7874 6d61 6e61 6765 720a 0a20 2020  textmanager..   
-00001490: 2020 2020 2077 6974 6820 536c 7572 6d43       with SlurmC
-000014a0: 6c69 656e 742e 6672 6f6d 5f63 6f6e 6669  lient.from_confi
-000014b0: 6728 2920 6173 2063 6c69 656e 743a 0a0a  g() as client:..
-000014c0: 2020 2020 2020 2020 2020 2020 2320 5275              # Ru
-000014d0: 6e20 6120 636f 6d6d 616e 6420 6f6e 2074  n a command on t
-000014e0: 6865 2072 656d 6f74 6520 686f 7374 0a0a  he remote host..
-000014f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00001500: 6c74 203d 2063 6c69 656e 742e 7275 6e28  lt = client.run(
-00001510: 2773 6261 7463 6820 6d79 6a6f 622e 7368  'sbatch myjob.sh
-00001520: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-00001530: 2320 4368 6563 6b20 7768 6574 6865 7220  # Check whether 
-00001540: 7468 6520 636f 6d6d 616e 6420 7375 6363  the command succ
-00001550: 6565 6465 640a 0a20 2020 2020 2020 2020  eeded..         
-00001560: 2020 2069 6620 7265 7375 6c74 2e6f 6b3a     if result.ok:
-00001570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001580: 2070 7269 6e74 2827 4a6f 6220 7375 626d   print('Job subm
-00001590: 6974 7465 6420 7375 6363 6573 7366 756c  itted successful
-000015a0: 6c79 2127 290a 0a20 2020 2020 2020 2020  ly!')..         
-000015b0: 2020 2023 2050 7269 6e74 2074 6865 206f     # Print the o
-000015c0: 7574 7075 7420 6f66 2074 6865 2063 6f6d  utput of the com
-000015d0: 6d61 6e64 0a0a 2020 2020 2020 2020 2020  mand..          
-000015e0: 2020 7072 696e 7428 7265 7375 6c74 2e73    print(result.s
-000015f0: 7464 6f75 7429 0a0a 2020 2020 4578 616d  tdout)..    Exam
-00001600: 706c 6520 323a 0a20 2020 2020 2020 2023  ple 2:.        #
-00001610: 2043 7265 6174 6520 6120 536c 7572 6d43   Create a SlurmC
-00001620: 6c69 656e 7420 616e 6420 7365 7475 7020  lient and setup 
-00001630: 536c 7572 6d20 2864 6f77 6e6c 6f61 6420  Slurm (download 
-00001640: 636f 6e74 6169 6e65 7273 2065 7463 2e29  containers etc.)
-00001650: 0a0a 2020 2020 2020 2020 7769 7468 2053  ..        with S
-00001660: 6c75 726d 436c 6965 6e74 2e66 726f 6d5f  lurmClient.from_
-00001670: 636f 6e66 6967 2869 6e69 745f 736c 7572  config(init_slur
-00001680: 6d3d 5472 7565 2920 6173 2063 6c69 656e  m=True) as clien
-00001690: 743a 0a0a 2020 2020 2020 2020 2020 2020  t:..            
-000016a0: 636c 6965 6e74 2e72 756e 5f77 6f72 6b66  client.run_workf
-000016b0: 6c6f 7728 2e2e 2e29 0a0a 2020 2020 2222  low(...)..    ""
-000016c0: 220a 2020 2020 5f44 4546 4155 4c54 5f43  ".    _DEFAULT_C
-000016d0: 4f4e 4649 475f 5041 5448 5f31 203d 2022  ONFIG_PATH_1 = "
-000016e0: 2f65 7463 2f73 6c75 726d 2d63 6f6e 6669  /etc/slurm-confi
-000016f0: 672e 696e 6922 0a20 2020 205f 4445 4641  g.ini".    _DEFA
-00001700: 554c 545f 434f 4e46 4947 5f50 4154 485f  ULT_CONFIG_PATH_
-00001710: 3220 3d20 227e 2f73 6c75 726d 2d63 6f6e  2 = "~/slurm-con
-00001720: 6669 672e 696e 6922 0a20 2020 205f 4445  fig.ini".    _DE
-00001730: 4641 554c 545f 484f 5354 203d 2022 736c  FAULT_HOST = "sl
-00001740: 7572 6d22 0a20 2020 205f 4445 4641 554c  urm".    _DEFAUL
-00001750: 545f 494e 4c49 4e45 5f53 5348 5f45 4e56  T_INLINE_SSH_ENV
-00001760: 203d 2054 7275 650a 2020 2020 5f44 4546   = True.    _DEF
-00001770: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
-00001780: 5041 5448 203d 2022 6d79 2d73 6372 6174  PATH = "my-scrat
-00001790: 6368 2f64 6174 6122 0a20 2020 205f 4445  ch/data".    _DE
-000017a0: 4641 554c 545f 534c 5552 4d5f 494d 4147  FAULT_SLURM_IMAG
-000017b0: 4553 5f50 4154 4820 3d20 226d 792d 7363  ES_PATH = "my-sc
-000017c0: 7261 7463 682f 7369 6e67 756c 6172 6974  ratch/singularit
-000017d0: 795f 696d 6167 6573 2f77 6f72 6b66 6c6f  y_images/workflo
-000017e0: 7773 220a 2020 2020 5f44 4546 4155 4c54  ws".    _DEFAULT
-000017f0: 5f53 4c55 524d 5f43 4f4e 5645 5254 4552  _SLURM_CONVERTER
-00001800: 535f 5041 5448 203d 2022 6d79 2d73 6372  S_PATH = "my-scr
-00001810: 6174 6368 2f73 696e 6775 6c61 7269 7479  atch/singularity
-00001820: 5f69 6d61 6765 732f 636f 6e76 6572 7465  _images/converte
-00001830: 7273 220a 2020 2020 5f44 4546 4155 4c54  rs".    _DEFAULT
-00001840: 5f53 4c55 524d 5f47 4954 5f53 4352 4950  _SLURM_GIT_SCRIP
-00001850: 545f 5041 5448 203d 2022 736c 7572 6d2d  T_PATH = "slurm-
-00001860: 7363 7269 7074 7322 0a20 2020 205f 4f55  scripts".    _OU
-00001870: 545f 5345 5020 3d20 222d 2d73 706c 6974  T_SEP = "--split
-00001880: 2d2d 220a 2020 2020 5f56 4552 5349 4f4e  --".    _VERSION
-00001890: 5f43 4d44 203d 2022 6c73 202d 6820 7b73  _CMD = "ls -h {s
-000018a0: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-000018b0: 7d2f 7b69 6d61 6765 5f70 6174 687d 207c  }/{image_path} |
-000018c0: 2067 7265 7020 2d6f 5020 2728 3f3c 3d5c   grep -oP '(?<=\
-000018d0: 2d7c 5c5f 2928 762e 2b7c 6c61 7465 7374  -|\_)(v.+|latest
-000018e0: 2928 3f3d 2e73 696d 677c 2e73 6966 2927  )(?=.simg|.sif)'
-000018f0: 220a 2020 2020 2320 4e6f 7465 2c20 6772  ".    # Note, gr
-00001900: 6570 2072 6574 7572 6e73 2065 7869 7463  ep returns exitc
-00001910: 6f64 6520 3120 6966 206e 6f20 6d61 7463  ode 1 if no matc
-00001920: 6820 6973 2066 6f75 6e64 210a 2020 2020  h is found!.    
-00001930: 2320 5468 6973 2077 696c 6c20 7472 616e  # This will tran
-00001940: 736c 6174 6520 696e 746f 2061 2055 6e65  slate into a Une
-00001950: 7870 6563 7465 6445 7869 7420 6572 726f  xpectedExit erro
-00001960: 722c 2073 6f20 6d75 7465 2074 6861 7420  r, so mute that 
-00001970: 6966 2079 6f75 0a20 2020 2023 2064 6f6e  if you.    # don
-00001980: 2774 2063 6172 6520 6162 6f75 7420 656d  't care about em
-00001990: 7074 792e 0a20 2020 2023 204c 696b 6520  pty..    # Like 
-000019a0: 6265 6c6f 7720 7769 7468 2074 6865 2022  below with the "
-000019b0: 7c7c 203a 222e 0a20 2020 2023 2044 6174  || :"..    # Dat
-000019c0: 6120 636f 756c 6420 6c65 6769 7420 6265  a could legit be
-000019d0: 2065 6d70 7479 2e0a 2020 2020 5f44 4154   empty..    _DAT
-000019e0: 415f 434d 4420 3d20 226c 7320 2d68 207b  A_CMD = "ls -h {
-000019f0: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-00001a00: 207c 2067 7265 7020 2d6f 5020 272e 2b28   | grep -oP '.+(
-00001a10: 3f3d 2e7a 6970 2927 207c 7c20 3a22 0a20  ?=.zip)' || :". 
-00001a20: 2020 205f 414c 4c5f 4a4f 4253 5f43 4d44     _ALL_JOBS_CMD
-00001a30: 203d 2022 7361 6363 7420 2d2d 7374 6172   = "sacct --star
-00001a40: 7474 696d 6520 7b73 7461 7274 5f74 696d  ttime {start_tim
-00001a50: 657d 202d 2d65 6e64 7469 6d65 207b 656e  e} --endtime {en
-00001a60: 645f 7469 6d65 7d20 2d2d 7374 6174 6520  d_time} --state 
-00001a70: 7b73 7461 7465 737d 202d 6f20 7b63 6f6c  {states} -o {col
-00001a80: 756d 6e73 7d20 2d6e 202d 5820 220a 2020  umns} -n -X ".  
-00001a90: 2020 5f5a 4950 5f43 4d44 203d 2022 377a    _ZIP_CMD = "7z
-00001aa0: 2061 202d 7920 7b66 696c 656e 616d 657d   a -y {filename}
-00001ab0: 202d 747a 6970 207b 6461 7461 5f6c 6f63   -tzip {data_loc
-00001ac0: 6174 696f 6e7d 2f64 6174 612f 6f75 7422  ation}/data/out"
-00001ad0: 0a20 2020 205f 4143 5449 5645 5f4a 4f42  .    _ACTIVE_JOB
-00001ae0: 535f 434d 4420 3d20 2273 7175 6575 6520  S_CMD = "squeue 
-00001af0: 2d75 2024 5553 4552 202d 2d6e 6f68 6561  -u $USER --nohea
-00001b00: 6420 2d2d 666f 726d 6174 2025 4622 0a20  d --format %F". 
-00001b10: 2020 205f 4a4f 425f 5354 4154 5553 5f43     _JOB_STATUS_C
-00001b20: 4d44 203d 2022 7361 6363 7420 2d6e 202d  MD = "sacct -n -
-00001b30: 6f20 4a6f 6249 642c 5374 6174 652c 456e  o JobId,State,En
-00001b40: 6420 2d58 202d 6a20 7b73 6c75 726d 5f6a  d -X -j {slurm_j
-00001b50: 6f62 5f69 647d 220a 2020 2020 2320 544f  ob_id}".    # TO
-00001b60: 444f 206d 6f76 6520 616c 6c20 636f 6d6d  DO move all comm
-00001b70: 616e 6473 2074 6f20 6120 7369 6d69 6c61  ands to a simila
-00001b80: 7220 666f 726d 6174 2e0a 2020 2020 2320  r format..    # 
-00001b90: 5468 656e 206d 6179 6265 2061 6c6c 6f77  Then maybe allow
-00001ba0: 206f 7665 7277 7269 7465 2066 726f 6d20   overwrite from 
-00001bb0: 736c 7572 6d2d 636f 6e66 6967 2e69 6e69  slurm-config.ini
-00001bc0: 0a20 2020 205f 4c4f 4746 494c 4520 3d20  .    _LOGFILE = 
-00001bd0: 226f 6d65 726f 2d7b 736c 7572 6d5f 6a6f  "omero-{slurm_jo
-00001be0: 625f 6964 7d2e 6c6f 6722 0a20 2020 205f  b_id}.log".    _
-00001bf0: 434f 4e56 4552 5445 525f 4c4f 4746 494c  CONVERTER_LOGFIL
-00001c00: 4520 3d20 2273 6c75 726d 2d7b 736c 7572  E = "slurm-{slur
-00001c10: 6d5f 6a6f 625f 6964 7d5f 2a2e 6f75 7422  m_job_id}_*.out"
-00001c20: 0a20 2020 205f 5441 494c 5f4c 4f47 5f43  .    _TAIL_LOG_C
-00001c30: 4d44 203d 2022 7461 696c 202d 6e20 7b6e  MD = "tail -n {n
-00001c40: 7d20 7b6c 6f67 5f66 696c 657d 207c 2073  } {log_file} | s
-00001c50: 7472 696e 6773 220a 2020 2020 5f4c 4f47  trings".    _LOG
-00001c60: 4649 4c45 5f44 4154 415f 434d 4420 3d20  FILE_DATA_CMD = 
-00001c70: 2263 6174 207b 6c6f 675f 6669 6c65 7d20  "cat {log_file} 
-00001c80: 7c20 7065 726c 202d 776e 6520 272f 5275  | perl -wne '/Ru
-00001c90: 6e6e 696e 6720 5b5c 772d 5d2b 3f20 4a6f  nning [\w-]+? Jo
-00001ca0: 6220 775c 2f20 2e2b 3f20 5c7c 202e 2b3f  b w\/ .+? \| .+?
-00001cb0: 205c 7c20 282e 2b3f 2920 5c7c 2e2a 2f69   \| (.+?) \|.*/i
-00001cc0: 2061 6e64 2070 7269 6e74 2431 2722 0a0a   and print$1'"..
-00001cd0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001ce0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00001cf0: 2020 2020 2020 2020 686f 7374 3d5f 4445          host=_DE
-00001d00: 4641 554c 545f 484f 5354 2c0a 2020 2020  FAULT_HOST,.    
-00001d10: 2020 2020 2020 2020 2020 2020 2075 7365               use
-00001d20: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
-00001d30: 2020 2020 2020 2020 2070 6f72 743d 4e6f           port=No
-00001d40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001d50: 2020 2020 2063 6f6e 6669 673d 4e6f 6e65       config=None
-00001d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001d70: 2020 2067 6174 6577 6179 3d4e 6f6e 652c     gateway=None,
-00001d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d90: 2020 666f 7277 6172 645f 6167 656e 743d    forward_agent=
-00001da0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001db0: 2020 2020 2020 2063 6f6e 6e65 6374 5f74         connect_t
-00001dc0: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001de0: 6e6e 6563 745f 6b77 6172 6773 3d4e 6f6e  nnect_kwargs=Non
-00001df0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001e00: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
-00001e10: 6e76 3d5f 4445 4641 554c 545f 494e 4c49  nv=_DEFAULT_INLI
-00001e20: 4e45 5f53 5348 5f45 4e56 2c0a 2020 2020  NE_SSH_ENV,.    
-00001e30: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00001e40: 726d 5f64 6174 615f 7061 7468 3a20 7374  rm_data_path: st
-00001e50: 7220 3d20 5f44 4546 4155 4c54 5f53 4c55  r = _DEFAULT_SLU
-00001e60: 524d 5f44 4154 415f 5041 5448 2c0a 2020  RM_DATA_PATH,.  
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001e80: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-00001e90: 3a20 7374 7220 3d20 5f44 4546 4155 4c54  : str = _DEFAULT
-00001ea0: 5f53 4c55 524d 5f49 4d41 4745 535f 5041  _SLURM_IMAGES_PA
-00001eb0: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
-00001ec0: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
-00001ed0: 7274 6572 735f 7061 7468 3a20 7374 7220  rters_path: str 
-00001ee0: 3d20 5f44 4546 4155 4c54 5f53 4c55 524d  = _DEFAULT_SLURM
-00001ef0: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
-00001f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f10: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-00001f20: 6174 6873 3a20 6469 6374 203d 204e 6f6e  aths: dict = Non
-00001f30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001f40: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00001f50: 7265 706f 733a 2064 6963 7420 3d20 4e6f  repos: dict = No
-00001f60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001f70: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-00001f80: 5f69 6d61 6765 733a 2064 6963 7420 3d20  _images: dict = 
-00001f90: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001fa0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00001fb0: 656c 5f6a 6f62 733a 2064 6963 7420 3d20  el_jobs: dict = 
-00001fc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001fd0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00001fe0: 656c 5f6a 6f62 735f 7061 7261 6d73 3a20  el_jobs_params: 
-00001ff0: 6469 6374 203d 204e 6f6e 652c 0a20 2020  dict = None,.   
-00002000: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00002010: 7572 6d5f 7363 7269 7074 5f70 6174 683a  urm_script_path:
-00002020: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
-00002030: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
-00002040: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
-00002050: 2020 2020 2020 2020 736c 7572 6d5f 7363          slurm_sc
-00002060: 7269 7074 5f72 6570 6f3a 2073 7472 203d  ript_repo: str =
-00002070: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002080: 2020 2020 2020 2020 696e 6974 5f73 6c75          init_slu
-00002090: 726d 3a20 626f 6f6c 203d 2046 616c 7365  rm: bool = False
-000020a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000020b0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000020c0: 2249 6e69 7469 616c 697a 6573 2061 206e  "Initializes a n
-000020d0: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
-000020e0: 6865 2053 6c75 726d 436c 6965 6e74 2063  he SlurmClient c
-000020f0: 6c61 7373 2e0a 0a20 2020 2020 2020 2049  lass...        I
-00002100: 7420 6973 2070 7265 6665 7261 626c 6520  t is preferable 
-00002110: 746f 2075 7365 2023 6672 6f6d 5f63 6f6e  to use #from_con
-00002120: 6669 6728 2e2e 2e29 206d 6574 686f 6420  fig(...) method 
-00002130: 746f 2069 6e69 7469 616c 697a 650a 2020  to initialize.  
-00002140: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
-00002150: 2066 726f 6d20 6120 636f 6e66 6967 2066   from a config f
-00002160: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
-00002170: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00002180: 686f 7374 2028 7374 722c 206f 7074 696f  host (str, optio
-00002190: 6e61 6c29 3a20 5468 6520 686f 7374 6e61  nal): The hostna
-000021a0: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
-000021b0: 206f 6620 7468 6520 7265 6d6f 7465 0a20   of the remote. 
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000021d0: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
-000021e0: 746f 205f 4445 4641 554c 545f 484f 5354  to _DEFAULT_HOST
-000021f0: 2e0a 2020 2020 2020 2020 2020 2020 7573  ..            us
-00002200: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-00002210: 6c29 3a20 5468 6520 7573 6572 6e61 6d65  l): The username
-00002220: 2074 6f20 7573 6520 7768 656e 2063 6f6e   to use when con
-00002230: 6e65 6374 696e 6720 746f 200a 2020 2020  necting to .    
-00002240: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00002250: 7265 6d6f 7465 2073 6572 7665 722e 2044  remote server. D
-00002260: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
-00002270: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
-00002280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002290: 2074 6f20 636f 6e66 6967 2e75 7365 722e   to config.user.
-000022a0: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
-000022b0: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-000022c0: 293a 2054 6865 2053 5348 2070 6f72 7420  ): The SSH port 
-000022d0: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
-000022e0: 6563 7469 6e67 2e0a 2020 2020 2020 2020  ecting..        
-000022f0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00002300: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
-00002310: 6465 6661 756c 7473 2074 6f20 636f 6e66  defaults to conf
-00002320: 6967 2e70 6f72 742e 0a20 2020 2020 2020  ig.port..       
-00002330: 2020 2020 2063 6f6e 6669 6720 2873 7472       config (str
-00002340: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
-00002350: 6820 746f 2074 6865 2053 5348 2063 6f6e  h to the SSH con
-00002360: 6669 6720 6669 6c65 2e0a 2020 2020 2020  fig file..      
-00002370: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00002380: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
-00002390: 6820 6465 6661 756c 7473 2074 6f20 796f  h defaults to yo
-000023a0: 7572 2053 5348 2063 6f6e 6669 6720 6669  ur SSH config fi
-000023b0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-000023c0: 6761 7465 7761 7920 2843 6f6e 6e65 6374  gateway (Connect
-000023d0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-000023e0: 416e 206f 7074 696f 6e61 6c20 6761 7465  An optional gate
-000023f0: 7761 7920 666f 7220 636f 6e6e 6563 7469  way for connecti
-00002400: 6e67 200a 2020 2020 2020 2020 2020 2020  ng .            
-00002410: 2020 2020 7468 726f 7567 6820 6120 6a75      through a ju
-00002420: 6d70 2068 6f73 742e 2044 6566 6175 6c74  mp host. Default
-00002430: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-00002440: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
-00002450: 6765 6e74 2028 626f 6f6c 2c20 6f70 7469  gent (bool, opti
-00002460: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
-00002470: 6f20 666f 7277 6172 6420 7468 6520 6c6f  o forward the lo
-00002480: 6361 6c20 5353 4820 0a20 2020 2020 2020  cal SSH .       
-00002490: 2020 2020 2020 2020 2061 6765 6e74 2074           agent t
-000024a0: 6f20 7468 6520 7265 6d6f 7465 2073 6572  o the remote ser
-000024b0: 7665 722e 2044 6566 6175 6c74 7320 746f  ver. Defaults to
-000024c0: 204e 6f6e 652c 2077 6869 6368 200a 2020   None, which .  
-000024d0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000024e0: 6661 756c 7473 2074 6f20 636f 6e66 6967  faults to config
-000024f0: 2e66 6f72 7761 7264 5f61 6765 6e74 2e0a  .forward_agent..
-00002500: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-00002510: 6563 745f 7469 6d65 6f75 7420 2869 6e74  ect_timeout (int
-00002520: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
-00002530: 656f 7574 2066 6f72 2065 7374 6162 6c69  eout for establi
-00002540: 7368 696e 6720 7468 6520 5353 4820 0a20  shing the SSH . 
-00002550: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002560: 6f6e 6e65 6374 696f 6e2e 2044 6566 6175  onnection. Defau
-00002570: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
-00002580: 6368 2064 6566 6175 6c74 7320 0a20 2020  ch defaults .   
-00002590: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-000025a0: 636f 6e66 6967 2e74 696d 656f 7574 732e  config.timeouts.
-000025b0: 636f 6e6e 6563 742e 0a20 2020 2020 2020  connect..       
-000025c0: 2020 2020 2063 6f6e 6e65 6374 5f6b 7761       connect_kwa
-000025d0: 7267 7320 2864 6963 742c 206f 7074 696f  rgs (dict, optio
-000025e0: 6e61 6c29 3a20 4164 6469 7469 6f6e 616c  nal): Additional
-000025f0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00002600: 7473 2066 6f72 200a 2020 2020 2020 2020  ts for .        
-00002610: 2020 2020 2020 2020 7468 6520 756e 6465          the unde
-00002620: 726c 7969 6e67 2053 5348 2063 6f6e 6e65  rlying SSH conne
-00002630: 6374 696f 6e2e 2048 616e 6465 6420 7665  ction. Handed ve
-00002640: 7262 6174 696d 2074 6f20 0a20 2020 2020  rbatim to .     
-00002650: 2020 2020 2020 2020 2020 2060 5353 4843             `SSHC
-00002660: 6c69 656e 742e 636f 6e6e 6563 7420 3c70  lient.connect <p
-00002670: 6172 616d 696b 6f2e 636c 6965 6e74 2e53  aramiko.client.S
-00002680: 5348 436c 6965 6e74 2e63 6f6e 6e65 6374  SHClient.connect
-00002690: 3e60 2e20 0a20 2020 2020 2020 2020 2020  >`. .           
-000026a0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-000026b0: 204e 6f6e 652e 200a 2020 2020 2020 2020   None. .        
-000026c0: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
-000026d0: 6e76 2028 626f 6f6c 2c20 6f70 7469 6f6e  nv (bool, option
-000026e0: 616c 293a 2057 6865 7468 6572 2074 6f20  al): Whether to 
-000026f0: 7573 6520 696e 6c69 6e65 2053 5348 0a20  use inline SSH. 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002710: 6e76 6972 6f6e 6d65 6e74 2e20 5468 6973  nvironment. This
-00002720: 2069 7320 6e65 6365 7373 6172 7920 6966   is necessary if
-00002730: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
-00002740: 6572 2068 6173 200a 2020 2020 2020 2020  er has .        
-00002750: 2020 2020 2020 2020 6120 7265 7374 7269          a restri
-00002760: 6374 6564 2060 6041 6363 6570 7445 6e76  cted ``AcceptEnv
-00002770: 6060 2073 6574 7469 6e67 2028 7768 6963  `` setting (whic
-00002780: 6820 6973 2074 6865 2063 6f6d 6d6f 6e20  h is the common 
-00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027a0: 2064 6566 6175 6c74 292e 2044 6566 6175   default). Defau
-000027b0: 6c74 7320 746f 205f 4445 4641 554c 545f  lts to _DEFAULT_
-000027c0: 494e 4c49 4e45 5f53 5348 5f45 4e56 2e0a  INLINE_SSH_ENV..
-000027d0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-000027e0: 6d5f 6461 7461 5f70 6174 6820 2873 7472  m_data_path (str
-000027f0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00002800: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
-00002810: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
-00002820: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-00002830: 6720 7468 6520 6461 7461 2066 696c 6573  g the data files
-00002840: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
-00002850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002860: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
-00002870: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
-00002880: 5f50 4154 482e 0a20 2020 2020 2020 2020  _PATH..         
-00002890: 2020 2073 6c75 726d 5f69 6d61 6765 735f     slurm_images_
-000028a0: 7061 7468 2028 7374 722c 206f 7074 696f  path (str, optio
-000028b0: 6e61 6c29 3a20 5468 6520 7061 7468 2074  nal): The path t
-000028c0: 6f20 7468 6520 6469 7265 6374 6f72 790a  o the directory.
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 636f 6e74 6169 6e69 6e67 2074 6865 2053  containing the S
-000028f0: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
-00002900: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
-00002910: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002920: 2020 4465 6661 756c 7473 2074 6f20 5f44    Defaults to _D
-00002930: 4546 4155 4c54 5f53 4c55 524d 5f49 4d41  EFAULT_SLURM_IMA
-00002940: 4745 535f 5041 5448 2e0a 2020 2020 2020  GES_PATH..      
-00002950: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
-00002960: 6572 7465 7273 5f70 6174 6820 2873 7472  erters_path (str
-00002970: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00002980: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
-00002990: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
-000029a0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-000029b0: 6720 7468 6520 5369 6e67 756c 6172 6974  g the Singularit
-000029c0: 7920 696d 6167 6573 2066 6f72 2066 696c  y images for fil
-000029d0: 6520 636f 6e76 6572 7465 7273 2e0a 2020  e converters..  
-000029e0: 2020 2020 2020 2020 2020 2020 2020 4465                De
-000029f0: 6661 756c 7473 2074 6f20 5f44 4546 4155  faults to _DEFAU
-00002a00: 4c54 5f53 4c55 524d 5f43 4f4e 5645 5254  LT_SLURM_CONVERT
-00002a10: 4552 535f 5041 5448 2e0a 2020 2020 2020  ERS_PATH..      
-00002a20: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00002a30: 6c5f 7061 7468 7320 2864 6963 742c 206f  l_paths (dict, o
-00002a40: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
-00002a50: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-00002a60: 6720 7468 6520 0a20 2020 2020 2020 2020  g the .         
-00002a70: 2020 2020 2020 2070 6174 6873 2074 6f20         paths to 
-00002a80: 7468 6520 5369 6e67 756c 6172 6974 7920  the Singularity 
-00002a90: 696d 6167 6573 2066 6f72 2073 7065 6369  images for speci
-00002aa0: 6669 6320 536c 7572 6d20 6a6f 6220 6d6f  fic Slurm job mo
-00002ab0: 6465 6c73 2e0a 2020 2020 2020 2020 2020  dels..          
-00002ac0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002ad0: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00002ae0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00002af0: 7265 706f 7320 2864 6963 742c 206f 7074  repos (dict, opt
-00002b00: 696f 6e61 6c29 3a20 4120 6469 6374 696f  ional): A dictio
-00002b10: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-00002b20: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
-00002b30: 2020 2020 2067 6974 2072 6570 6f73 6974       git reposit
-00002b40: 6f72 6965 7320 6f66 2053 696e 6775 6c61  ories of Singula
-00002b50: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
-00002b60: 7370 6563 6966 6963 2053 6c75 726d 200a  specific Slurm .
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
-00002b90: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00002ba0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00002bb0: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-00002bc0: 6d6f 6465 6c5f 696d 6167 6573 2028 6469  model_images (di
-00002bd0: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
-00002be0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-00002bf0: 6169 6e69 6e67 2074 6865 200a 2020 2020  aining the .    
-00002c00: 2020 2020 2020 2020 2020 2020 646f 636b              dock
-00002c10: 6572 6875 6220 6f66 2074 6865 2053 696e  erhub of the Sin
-00002c20: 6775 6c61 7269 7479 2069 6d61 6765 7320  gularity images 
-00002c30: 666f 7220 7370 6563 6966 6963 2053 6c75  for specific Slu
-00002c40: 726d 200a 2020 2020 2020 2020 2020 2020  rm .            
-00002c50: 2020 2020 6a6f 6220 6d6f 6465 6c73 2e20      job models. 
-00002c60: 5769 6c6c 2066 696c 6c20 6175 746f 6d61  Will fill automa
-00002c70: 7469 6361 6c6c 7920 6672 6f6d 2074 6865  tically from the
-00002c80: 2064 6174 6120 696e 2074 6865 2067 6974   data in the git
-00002c90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002ca0: 2020 7265 706f 7369 746f 7279 2069 6620    repository if 
-00002cb0: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
-00002cc0: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
-00002cd0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002ce0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002cf0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00002d00: 6273 2028 6469 6374 2c20 6f70 7469 6f6e  bs (dict, option
-00002d10: 616c 293a 2041 2064 6963 7469 6f6e 6172  al): A dictionar
-00002d20: 7920 636f 6e74 6169 6e69 6e67 0a20 2020  y containing.   
-00002d30: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00002d40: 6f72 6d61 7469 6f6e 2061 626f 7574 2073  ormation about s
-00002d50: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
-00002d60: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
-00002d70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00002d80: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00002d90: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00002da0: 6465 6c5f 6a6f 6273 5f70 6172 616d 7320  del_jobs_params 
-00002db0: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
-00002dc0: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
-00002dd0: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
-00002de0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
-00002df0: 7465 7273 2066 6f72 2073 7065 6369 6669  ters for specifi
-00002e00: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
-00002e10: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
-00002e20: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002e30: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002e40: 2020 736c 7572 6d5f 7363 7269 7074 5f70    slurm_script_p
-00002e50: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
-00002e60: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
-00002e70: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002e90: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
-00002ea0: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
-00002eb0: 6f6e 2073 6372 6970 7473 206f 6e20 536c  on scripts on Sl
-00002ec0: 7572 6d2e 0a20 2020 2020 2020 2020 2020  urm..           
-00002ed0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00002ee0: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
-00002ef0: 4749 545f 5343 5249 5054 5f50 4154 482e  GIT_SCRIPT_PATH.
-00002f00: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
-00002f10: 726d 5f73 6372 6970 745f 7265 706f 2028  rm_script_repo (
-00002f20: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00002f30: 5468 6520 6769 7420 6874 7470 7320 5552  The git https UR
-00002f40: 4c20 666f 7220 636c 6f6e 696e 670a 2020  L for cloning.  
-00002f50: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00002f60: 6520 7265 706f 2063 6f6e 7461 696e 696e  e repo containin
-00002f70: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
-00002f80: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
-00002f90: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00002fa0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002fb0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002fc0: 2020 696e 6974 5f73 6c75 726d 2028 626f    init_slurm (bo
-00002fd0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
-00002fe0: 7365 7420 7570 2074 6865 2072 6571 7569  set up the requi
-00002ff0: 7265 6420 7374 7275 6374 7572 6573 200a  red structures .
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 6f6e 2053 6c75 726d 2061 6674 6572 2069  on Slurm after i
-00003020: 6e69 7469 6174 696e 6720 7468 6973 2063  nitiating this c
-00003030: 6c69 656e 742e 2054 6869 7320 696e 636c  lient. This incl
-00003040: 7564 6573 2063 7265 6174 696e 6720 0a20  udes creating . 
-00003050: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00003060: 6973 7369 6e67 2066 6f6c 6465 7273 2c20  issing folders, 
-00003070: 646f 776e 6c6f 6164 696e 6720 636f 6e74  downloading cont
-00003080: 6169 6e65 7220 696d 6167 6573 2c20 636c  ainer images, cl
-00003090: 6f6e 696e 6720 6769 742c 6574 632e 0a20  oning git,etc.. 
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000030b0: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
-000030c0: 7768 696c 6520 6174 2066 6972 7374 2062  while at first b
-000030d0: 7574 2077 696c 6c20 7661 6c69 6461 7465  ut will validate
-000030e0: 2079 6f75 7220 7365 7475 702e 0a20 2020   your setup..   
-000030f0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00003100: 6175 6c74 7320 746f 2046 616c 7365 2074  aults to False t
-00003110: 6f20 7361 7665 2074 696d 652e 0a20 2020  o save time..   
-00003120: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003130: 2073 7570 6572 2853 6c75 726d 436c 6965   super(SlurmClie
-00003140: 6e74 2c20 7365 6c66 292e 5f5f 696e 6974  nt, self).__init
-00003150: 5f5f 2868 6f73 742c 0a20 2020 2020 2020  __(host,.       
-00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2075 7365 722c 0a20 2020 2020 2020     user,.       
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2020 2070 6f72 742c 0a20 2020 2020 2020     port,.       
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031e0: 2020 2063 6f6e 6669 672c 0a20 2020 2020     config,.     
-000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 2020 2067 6174 6577 6179 2c0a 2020       gateway,.  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 2020 2020 666f 7277 6172 645f          forward_
-00003250: 6167 656e 742c 0a20 2020 2020 2020 2020  agent,.         
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003280: 2063 6f6e 6e65 6374 5f74 696d 656f 7574   connect_timeout
-00003290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000bd0: 7465 0a20 2020 200a 2020 2020 6465 6620  te.    .    def 
+00000be0: 636c 6561 6e75 7028 7365 6c66 2c20 736c  cleanup(self, sl
+00000bf0: 7572 6d43 6c69 656e 7429 202d 3e20 5265  urmClient) -> Re
+00000c00: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
+00000c10: 220a 2020 2020 2020 2020 436c 6561 6e75  ".        Cleanu
+00000c20: 7020 7265 6d61 696e 696e 6720 6c6f 6720  p remaining log 
+00000c30: 6669 6c65 732e 0a0a 2020 2020 2020 2020  files...        
+00000c40: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00000c50: 2020 736c 7572 6d43 6c69 656e 743a 2054    slurmClient: T
+00000c60: 6865 2053 6c75 726d 2063 6c69 656e 742e  he Slurm client.
+00000c70: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00000c80: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+00000c90: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
+00000ca0: 7420 6f66 2074 6865 2063 6c65 616e 7570  t of the cleanup
+00000cb0: 206f 7065 7261 7469 6f6e 2e0a 2020 2020   operation..    
+00000cc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00000cd0: 7265 7475 726e 2073 6c75 726d 436c 6965  return slurmClie
+00000ce0: 6e74 2e63 6c65 616e 7570 5f74 6d70 5f66  nt.cleanup_tmp_f
+00000cf0: 696c 6573 2873 656c 662e 6a6f 625f 6964  iles(self.job_id
+00000d00: 290a 0a20 2020 2064 6566 2063 6f6d 706c  )..    def compl
+00000d10: 6574 6564 2873 656c 6629 3a0a 2020 2020  eted(self):.    
+00000d20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00000d30: 4368 6563 6b20 6966 2074 6865 2053 6c75  Check if the Slu
+00000d40: 726d 206a 6f62 2068 6173 2063 6f6d 706c  rm job has compl
+00000d50: 6574 6564 2073 7563 6365 7373 6675 6c6c  eted successfull
+00000d60: 792e 0a0a 2020 2020 2020 2020 5265 7475  y...        Retu
+00000d70: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00000d80: 2062 6f6f 6c3a 2054 7275 6520 6966 2074   bool: True if t
+00000d90: 6865 206a 6f62 2068 6173 2063 6f6d 706c  he job has compl
+00000da0: 6574 6564 3b20 4661 6c73 6520 6f74 6865  eted; False othe
+00000db0: 7277 6973 652e 0a20 2020 2020 2020 2022  rwise..        "
+00000dc0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00000dd0: 6e20 7365 6c66 2e6a 6f62 5f73 7461 7465  n self.job_state
+00000de0: 203d 3d20 2243 4f4d 504c 4554 4544 220a   == "COMPLETED".
+00000df0: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+00000e00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00000e10: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+00000e20: 726e 2061 2073 7472 696e 6720 7265 7072  rn a string repr
+00000e30: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+00000e40: 6520 536c 7572 6d4a 6f62 2069 6e73 7461  e SlurmJob insta
+00000e50: 6e63 652e 0a0a 2020 2020 2020 2020 5265  nce...        Re
+00000e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00000e70: 2020 2073 7472 3a20 5374 7269 6e67 2072     str: String r
+00000e80: 6570 7265 7365 6e74 6174 696f 6e2e 0a20  epresentation.. 
+00000e90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000ea0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
+00000eb0: 272c 2027 2e6a 6f69 6e28 0a20 2020 2020  ', '.join(.     
+00000ec0: 2020 2020 2020 2066 227b 6b65 797d 3d7b         f"{key}={
+00000ed0: 7661 6c75 657d 2220 666f 7220 6b65 792c  value}" for key,
+00000ee0: 2076 616c 7565 2069 6e20 7365 6c66 2e5f   value in self._
+00000ef0: 5f64 6963 745f 5f2e 6974 656d 7328 2929  _dict__.items())
+00000f00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000f10: 6622 536c 7572 6d4a 6f62 287b 7072 6f70  f"SlurmJob({prop
+00000f20: 6572 7469 6573 7d29 220a 0a0a 636c 6173  erties})"...clas
+00000f30: 7320 536c 7572 6d43 6c69 656e 7428 436f  s SlurmClient(Co
+00000f40: 6e6e 6563 7469 6f6e 293a 0a20 2020 2022  nnection):.    "
+00000f50: 2222 4120 636c 6965 6e74 2066 6f72 2063  ""A client for c
+00000f60: 6f6e 6e65 6374 696e 6720 746f 2061 6e64  onnecting to and
+00000f70: 2069 6e74 6572 6163 7469 6e67 2077 6974   interacting wit
+00000f80: 6820 6120 536c 7572 6d20 636c 7573 7465  h a Slurm cluste
+00000f90: 7220 6f76 6572 0a20 2020 2053 5348 2e0a  r over.    SSH..
+00000fa0: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
+00000fb0: 6578 7465 6e64 7320 7468 6520 436f 6e6e  extends the Conn
+00000fc0: 6563 7469 6f6e 2063 6c61 7373 2c20 6164  ection class, ad
+00000fd0: 6469 6e67 206d 6574 686f 6473 2061 6e64  ding methods and
+00000fe0: 0a20 2020 2061 7474 7269 6275 7465 7320  .    attributes 
+00000ff0: 7370 6563 6966 6963 2074 6f20 776f 726b  specific to work
+00001000: 696e 6720 7769 7468 2053 6c75 726d 2e0a  ing with Slurm..
+00001010: 0a20 2020 2053 6c75 726d 436c 6965 6e74  .    SlurmClient
+00001020: 2061 6363 6570 7473 2074 6865 2073 616d   accepts the sam
+00001030: 6520 6172 6775 6d65 6e74 7320 6173 2043  e arguments as C
+00001040: 6f6e 6e65 6374 696f 6e2e 2042 656c 6f77  onnection. Below
+00001050: 206f 6e6c 790a 2020 2020 6d65 6e74 696f   only.    mentio
+00001060: 6e73 2074 6865 2061 6464 6564 206f 6e65  ns the added one
+00001070: 733a 0a0a 2020 2020 5468 6520 6561 7369  s:..    The easi
+00001080: 6573 7420 7761 7920 746f 2073 6574 2074  est way to set t
+00001090: 6869 7320 636c 6965 6e74 2075 7020 6973  his client up is
+000010a0: 2062 7920 7573 696e 6720 6120 736c 7572   by using a slur
+000010b0: 6d2d 636f 6e66 6967 2e69 6e69 0a20 2020  m-config.ini.   
+000010c0: 2061 6e64 2074 6865 2066 726f 6d2d 636f   and the from-co
+000010d0: 6e66 6967 2829 206d 6574 686f 642e 0a0a  nfig() method...
+000010e0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+000010f0: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
+00001100: 7461 5f70 6174 6820 2873 7472 293a 2054  ta_path (str): T
+00001110: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
+00001120: 6972 6563 746f 7279 2063 6f6e 7461 696e  irectory contain
+00001130: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
+00001140: 2020 2020 6461 7461 2066 696c 6573 2066      data files f
+00001150: 6f72 2053 6c75 726d 206a 6f62 732e 0a20  or Slurm jobs.. 
+00001160: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
+00001170: 6765 735f 7061 7468 2028 7374 7229 3a20  ges_path (str): 
+00001180: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
+00001190: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
+000011a0: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
+000011b0: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
+000011c0: 2069 6d61 6765 7320 666f 7220 536c 7572   images for Slur
+000011d0: 6d20 6a6f 6273 2e0a 2020 2020 2020 2020  m jobs..        
+000011e0: 736c 7572 6d5f 636f 6e76 6572 7465 7273  slurm_converters
+000011f0: 5f70 6174 6820 2873 7472 293a 2054 6865  _path (str): The
+00001200: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00001210: 6563 746f 7279 2063 6f6e 7461 696e 696e  ectory containin
+00001220: 670a 2020 2020 2020 2020 2020 2020 7468  g.            th
+00001230: 6520 5369 6e67 756c 6172 6974 7920 696d  e Singularity im
+00001240: 6167 6573 2066 6f72 2066 696c 6520 636f  ages for file co
+00001250: 6e76 6572 7465 7273 2e0a 2020 2020 2020  nverters..      
+00001260: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
+00001270: 7468 7320 2864 6963 7429 3a20 4120 6469  ths (dict): A di
+00001280: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+00001290: 696e 6720 7468 6520 7061 7468 7320 746f  ing the paths to
+000012a0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+000012b0: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
+000012c0: 6765 7320 666f 7220 7370 6563 6966 6963  ges for specific
+000012d0: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
+000012e0: 732e 0a20 2020 2020 2020 2073 6c75 726d  s..        slurm
+000012f0: 5f6d 6f64 656c 5f72 6570 6f73 2028 6469  _model_repos (di
+00001300: 6374 293a 2041 2064 6963 7469 6f6e 6172  ct): A dictionar
+00001310: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
+00001320: 2067 6974 0a20 2020 2020 2020 2020 2020   git.           
+00001330: 2072 6570 6f73 6974 6f72 6965 7320 6f66   repositories of
+00001340: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
+00001350: 6765 7320 666f 7220 7370 6563 6966 6963  ges for specific
+00001360: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
+00001370: 732e 0a20 2020 2020 2020 2073 6c75 726d  s..        slurm
+00001380: 5f6d 6f64 656c 5f69 6d61 6765 7320 2864  _model_images (d
+00001390: 6963 7429 3a20 4120 6469 6374 696f 6e61  ict): A dictiona
+000013a0: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
+000013b0: 6520 646f 636b 6572 6875 620a 2020 2020  e dockerhub.    
+000013c0: 2020 2020 2020 2020 6f66 2074 6865 2053          of the S
+000013d0: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
+000013e0: 7320 666f 7220 7370 6563 6966 6963 2053  s for specific S
+000013f0: 6c75 726d 206a 6f62 206d 6f64 656c 732e  lurm job models.
+00001400: 0a20 2020 2020 2020 2020 2020 2057 696c  .            Wil
+00001410: 6c20 6669 6c6c 2061 7574 6f6d 6174 6963  l fill automatic
+00001420: 616c 6c79 2066 726f 6d20 7468 6520 6461  ally from the da
+00001430: 7461 2069 6e20 7468 6520 6769 7420 7265  ta in the git re
+00001440: 706f 7369 746f 7279 2c0a 2020 2020 2020  pository,.      
+00001450: 2020 2020 2020 6966 2079 6f75 2073 6574        if you set
+00001460: 2069 6e69 745f 736c 7572 6d2e 0a20 2020   init_slurm..   
+00001470: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00001480: 745f 7061 7468 2028 7374 7229 3a20 5468  t_path (str): Th
+00001490: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
+000014a0: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
+000014b0: 6e67 0a20 2020 2020 2020 2020 2020 2074  ng.            t
+000014c0: 6865 2053 6c75 726d 206a 6f62 2073 7562  he Slurm job sub
+000014d0: 6d69 7373 696f 6e20 7363 7269 7074 7320  mission scripts 
+000014e0: 6f6e 2053 6c75 726d 2e0a 2020 2020 2020  on Slurm..      
+000014f0: 2020 736c 7572 6d5f 7363 7269 7074 5f72    slurm_script_r
+00001500: 6570 6f20 2873 7472 293a 2054 6865 2067  epo (str): The g
+00001510: 6974 2068 7474 7073 2055 524c 2066 6f72  it https URL for
+00001520: 2063 6c6f 6e69 6e67 2074 6865 2072 6570   cloning the rep
+00001530: 6f0a 2020 2020 2020 2020 2020 2020 636f  o.            co
+00001540: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
+00001550: 726d 206a 6f62 2073 7562 6d69 7373 696f  rm job submissio
+00001560: 6e20 7363 7269 7074 732e 204f 7074 696f  n scripts. Optio
+00001570: 6e61 6c2e 0a0a 2020 2020 4578 616d 706c  nal...    Exampl
+00001580: 653a 0a20 2020 2020 2020 2023 2043 7265  e:.        # Cre
+00001590: 6174 6520 6120 536c 7572 6d43 6c69 656e  ate a SlurmClien
+000015a0: 7420 6f62 6a65 6374 2061 7320 636f 6e74  t object as cont
+000015b0: 6578 746d 616e 6167 6572 0a0a 2020 2020  extmanager..    
+000015c0: 2020 2020 7769 7468 2053 6c75 726d 436c      with SlurmCl
+000015d0: 6965 6e74 2e66 726f 6d5f 636f 6e66 6967  ient.from_config
+000015e0: 2829 2061 7320 636c 6965 6e74 3a0a 0a20  () as client:.. 
+000015f0: 2020 2020 2020 2020 2020 2023 2052 756e             # Run
+00001600: 2061 2063 6f6d 6d61 6e64 206f 6e20 7468   a command on th
+00001610: 6520 7265 6d6f 7465 2068 6f73 740a 0a20  e remote host.. 
+00001620: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00001630: 7420 3d20 636c 6965 6e74 2e72 756e 2827  t = client.run('
+00001640: 7362 6174 6368 206d 796a 6f62 2e73 6827  sbatch myjob.sh'
+00001650: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00001660: 2043 6865 636b 2077 6865 7468 6572 2074   Check whether t
+00001670: 6865 2063 6f6d 6d61 6e64 2073 7563 6365  he command succe
+00001680: 6564 6564 0a0a 2020 2020 2020 2020 2020  eded..          
+00001690: 2020 6966 2072 6573 756c 742e 6f6b 3a0a    if result.ok:.
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 7072 696e 7428 274a 6f62 2073 7562 6d69  print('Job submi
+000016c0: 7474 6564 2073 7563 6365 7373 6675 6c6c  tted successfull
+000016d0: 7921 2729 0a0a 2020 2020 2020 2020 2020  y!')..          
+000016e0: 2020 2320 5072 696e 7420 7468 6520 6f75    # Print the ou
+000016f0: 7470 7574 206f 6620 7468 6520 636f 6d6d  tput of the comm
+00001700: 616e 640a 0a20 2020 2020 2020 2020 2020  and..           
+00001710: 2070 7269 6e74 2872 6573 756c 742e 7374   print(result.st
+00001720: 646f 7574 290a 0a20 2020 2045 7861 6d70  dout)..    Examp
+00001730: 6c65 2032 3a0a 2020 2020 2020 2020 2320  le 2:.        # 
+00001740: 4372 6561 7465 2061 2053 6c75 726d 436c  Create a SlurmCl
+00001750: 6965 6e74 2061 6e64 2073 6574 7570 2053  ient and setup S
+00001760: 6c75 726d 2028 646f 776e 6c6f 6164 2063  lurm (download c
+00001770: 6f6e 7461 696e 6572 7320 6574 632e 290a  ontainers etc.).
+00001780: 0a20 2020 2020 2020 2077 6974 6820 536c  .        with Sl
+00001790: 7572 6d43 6c69 656e 742e 6672 6f6d 5f63  urmClient.from_c
+000017a0: 6f6e 6669 6728 696e 6974 5f73 6c75 726d  onfig(init_slurm
+000017b0: 3d54 7275 6529 2061 7320 636c 6965 6e74  =True) as client
+000017c0: 3a0a 0a20 2020 2020 2020 2020 2020 2063  :..            c
+000017d0: 6c69 656e 742e 7275 6e5f 776f 726b 666c  lient.run_workfl
+000017e0: 6f77 282e 2e2e 290a 0a20 2020 2022 2222  ow(...)..    """
+000017f0: 0a20 2020 205f 4445 4641 554c 545f 434f  .    _DEFAULT_CO
+00001800: 4e46 4947 5f50 4154 485f 3120 3d20 222f  NFIG_PATH_1 = "/
+00001810: 6574 632f 736c 7572 6d2d 636f 6e66 6967  etc/slurm-config
+00001820: 2e69 6e69 220a 2020 2020 5f44 4546 4155  .ini".    _DEFAU
+00001830: 4c54 5f43 4f4e 4649 475f 5041 5448 5f32  LT_CONFIG_PATH_2
+00001840: 203d 2022 7e2f 736c 7572 6d2d 636f 6e66   = "~/slurm-conf
+00001850: 6967 2e69 6e69 220a 2020 2020 5f44 4546  ig.ini".    _DEF
+00001860: 4155 4c54 5f48 4f53 5420 3d20 2273 6c75  AULT_HOST = "slu
+00001870: 726d 220a 2020 2020 5f44 4546 4155 4c54  rm".    _DEFAULT
+00001880: 5f49 4e4c 494e 455f 5353 485f 454e 5620  _INLINE_SSH_ENV 
+00001890: 3d20 5472 7565 0a20 2020 205f 4445 4641  = True.    _DEFA
+000018a0: 554c 545f 534c 5552 4d5f 4441 5441 5f50  ULT_SLURM_DATA_P
+000018b0: 4154 4820 3d20 226d 792d 7363 7261 7463  ATH = "my-scratc
+000018c0: 682f 6461 7461 220a 2020 2020 5f44 4546  h/data".    _DEF
+000018d0: 4155 4c54 5f53 4c55 524d 5f49 4d41 4745  AULT_SLURM_IMAGE
+000018e0: 535f 5041 5448 203d 2022 6d79 2d73 6372  S_PATH = "my-scr
+000018f0: 6174 6368 2f73 696e 6775 6c61 7269 7479  atch/singularity
+00001900: 5f69 6d61 6765 732f 776f 726b 666c 6f77  _images/workflow
+00001910: 7322 0a20 2020 205f 4445 4641 554c 545f  s".    _DEFAULT_
+00001920: 534c 5552 4d5f 434f 4e56 4552 5445 5253  SLURM_CONVERTERS
+00001930: 5f50 4154 4820 3d20 226d 792d 7363 7261  _PATH = "my-scra
+00001940: 7463 682f 7369 6e67 756c 6172 6974 795f  tch/singularity_
+00001950: 696d 6167 6573 2f63 6f6e 7665 7274 6572  images/converter
+00001960: 7322 0a20 2020 205f 4445 4641 554c 545f  s".    _DEFAULT_
+00001970: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
+00001980: 5f50 4154 4820 3d20 2273 6c75 726d 2d73  _PATH = "slurm-s
+00001990: 6372 6970 7473 220a 2020 2020 5f4f 5554  cripts".    _OUT
+000019a0: 5f53 4550 203d 2022 2d2d 7370 6c69 742d  _SEP = "--split-
+000019b0: 2d22 0a20 2020 205f 5645 5253 494f 4e5f  -".    _VERSION_
+000019c0: 434d 4420 3d20 226c 7320 2d68 207b 736c  CMD = "ls -h {sl
+000019d0: 7572 6d5f 696d 6167 6573 5f70 6174 687d  urm_images_path}
+000019e0: 2f7b 696d 6167 655f 7061 7468 7d20 7c20  /{image_path} | 
+000019f0: 6772 6570 202d 6f50 2027 283f 3c3d 5c2d  grep -oP '(?<=\-
+00001a00: 7c5c 5f29 2876 2e2b 7c6c 6174 6573 7429  |\_)(v.+|latest)
+00001a10: 283f 3d2e 7369 6d67 7c2e 7369 6629 2722  (?=.simg|.sif)'"
+00001a20: 0a20 2020 2023 204e 6f74 652c 2067 7265  .    # Note, gre
+00001a30: 7020 7265 7475 726e 7320 6578 6974 636f  p returns exitco
+00001a40: 6465 2031 2069 6620 6e6f 206d 6174 6368  de 1 if no match
+00001a50: 2069 7320 666f 756e 6421 0a20 2020 2023   is found!.    #
+00001a60: 2054 6869 7320 7769 6c6c 2074 7261 6e73   This will trans
+00001a70: 6c61 7465 2069 6e74 6f20 6120 556e 6578  late into a Unex
+00001a80: 7065 6374 6564 4578 6974 2065 7272 6f72  pectedExit error
+00001a90: 2c20 736f 206d 7574 6520 7468 6174 2069  , so mute that i
+00001aa0: 6620 796f 750a 2020 2020 2320 646f 6e27  f you.    # don'
+00001ab0: 7420 6361 7265 2061 626f 7574 2065 6d70  t care about emp
+00001ac0: 7479 2e0a 2020 2020 2320 4c69 6b65 2062  ty..    # Like b
+00001ad0: 656c 6f77 2077 6974 6820 7468 6520 227c  elow with the "|
+00001ae0: 7c20 3a22 2e0a 2020 2020 2320 4461 7461  | :"..    # Data
+00001af0: 2063 6f75 6c64 206c 6567 6974 2062 6520   could legit be 
+00001b00: 656d 7074 792e 0a20 2020 205f 4441 5441  empty..    _DATA
+00001b10: 5f43 4d44 203d 2022 6c73 202d 6820 7b73  _CMD = "ls -h {s
+00001b20: 6c75 726d 5f64 6174 615f 7061 7468 7d20  lurm_data_path} 
+00001b30: 7c20 6772 6570 202d 6f50 2027 2e2b 283f  | grep -oP '.+(?
+00001b40: 3d2e 7a69 7029 2720 7c7c 203a 220a 2020  =.zip)' || :".  
+00001b50: 2020 5f41 4c4c 5f4a 4f42 535f 434d 4420    _ALL_JOBS_CMD 
+00001b60: 3d20 2273 6163 6374 202d 2d73 7461 7274  = "sacct --start
+00001b70: 7469 6d65 207b 7374 6172 745f 7469 6d65  time {start_time
+00001b80: 7d20 2d2d 656e 6474 696d 6520 7b65 6e64  } --endtime {end
+00001b90: 5f74 696d 657d 202d 2d73 7461 7465 207b  _time} --state {
+00001ba0: 7374 6174 6573 7d20 2d6f 207b 636f 6c75  states} -o {colu
+00001bb0: 6d6e 737d 202d 6e20 2d58 2022 0a20 2020  mns} -n -X ".   
+00001bc0: 205f 5a49 505f 434d 4420 3d20 2237 7a20   _ZIP_CMD = "7z 
+00001bd0: 6120 2d79 207b 6669 6c65 6e61 6d65 7d20  a -y {filename} 
+00001be0: 2d74 7a69 7020 7b64 6174 615f 6c6f 6361  -tzip {data_loca
+00001bf0: 7469 6f6e 7d2f 6461 7461 2f6f 7574 220a  tion}/data/out".
+00001c00: 2020 2020 5f41 4354 4956 455f 4a4f 4253      _ACTIVE_JOBS
+00001c10: 5f43 4d44 203d 2022 7371 7565 7565 202d  _CMD = "squeue -
+00001c20: 7520 2455 5345 5220 2d2d 6e6f 6865 6164  u $USER --nohead
+00001c30: 202d 2d66 6f72 6d61 7420 2546 220a 2020   --format %F".  
+00001c40: 2020 5f4a 4f42 5f53 5441 5455 535f 434d    _JOB_STATUS_CM
+00001c50: 4420 3d20 2273 6163 6374 202d 6e20 2d6f  D = "sacct -n -o
+00001c60: 204a 6f62 4964 2c53 7461 7465 2c45 6e64   JobId,State,End
+00001c70: 202d 5820 2d6a 207b 736c 7572 6d5f 6a6f   -X -j {slurm_jo
+00001c80: 625f 6964 7d22 0a20 2020 2023 2054 4f44  b_id}".    # TOD
+00001c90: 4f20 6d6f 7665 2061 6c6c 2063 6f6d 6d61  O move all comma
+00001ca0: 6e64 7320 746f 2061 2073 696d 696c 6172  nds to a similar
+00001cb0: 2066 6f72 6d61 742e 0a20 2020 2023 2054   format..    # T
+00001cc0: 6865 6e20 6d61 7962 6520 616c 6c6f 7720  hen maybe allow 
+00001cd0: 6f76 6572 7772 6974 6520 6672 6f6d 2073  overwrite from s
+00001ce0: 6c75 726d 2d63 6f6e 6669 672e 696e 690a  lurm-config.ini.
+00001cf0: 2020 2020 5f4c 4f47 4649 4c45 203d 2022      _LOGFILE = "
+00001d00: 6f6d 6572 6f2d 7b73 6c75 726d 5f6a 6f62  omero-{slurm_job
+00001d10: 5f69 647d 2e6c 6f67 220a 2020 2020 5f43  _id}.log".    _C
+00001d20: 4f4e 5645 5254 4552 5f4c 4f47 4649 4c45  ONVERTER_LOGFILE
+00001d30: 203d 2022 736c 7572 6d2d 7b73 6c75 726d   = "slurm-{slurm
+00001d40: 5f6a 6f62 5f69 647d 5f2a 2e6f 7574 220a  _job_id}_*.out".
+00001d50: 2020 2020 5f54 4149 4c5f 4c4f 475f 434d      _TAIL_LOG_CM
+00001d60: 4420 3d20 2274 6169 6c20 2d6e 207b 6e7d  D = "tail -n {n}
+00001d70: 207b 6c6f 675f 6669 6c65 7d20 7c20 7374   {log_file} | st
+00001d80: 7269 6e67 7322 0a20 2020 205f 4c4f 4746  rings".    _LOGF
+00001d90: 494c 455f 4441 5441 5f43 4d44 203d 2022  ILE_DATA_CMD = "
+00001da0: 6361 7420 7b6c 6f67 5f66 696c 657d 207c  cat {log_file} |
+00001db0: 2070 6572 6c20 2d77 6e65 2027 2f52 756e   perl -wne '/Run
+00001dc0: 6e69 6e67 205b 5c77 2d5d 2b3f 204a 6f62  ning [\w-]+? Job
+00001dd0: 2077 5c2f 202e 2b3f 205c 7c20 2e2b 3f20   w\/ .+? \| .+? 
+00001de0: 5c7c 2028 2e2b 3f29 205c 7c2e 2a2f 6920  \| (.+?) \|.*/i 
+00001df0: 616e 6420 7072 696e 7424 3127 220a 0a20  and print$1'".. 
+00001e00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001e10: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00001e20: 2020 2020 2020 2068 6f73 743d 5f44 4546         host=_DEF
+00001e30: 4155 4c54 5f48 4f53 542c 0a20 2020 2020  AULT_HOST,.     
+00001e40: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00001e50: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00001e60: 2020 2020 2020 2020 706f 7274 3d4e 6f6e          port=Non
+00001e70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001e80: 2020 2020 636f 6e66 6967 3d4e 6f6e 652c      config=None,
+00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ea0: 2020 6761 7465 7761 793d 4e6f 6e65 2c0a    gateway=None,.
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2066 6f72 7761 7264 5f61 6765 6e74 3d4e   forward_agent=N
+00001ed0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001ee0: 2020 2020 2020 636f 6e6e 6563 745f 7469        connect_ti
+00001ef0: 6d65 6f75 743d 4e6f 6e65 2c0a 2020 2020  meout=None,.    
+00001f00: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00001f10: 6e65 6374 5f6b 7761 7267 733d 4e6f 6e65  nect_kwargs=None
+00001f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001f30: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
+00001f40: 763d 5f44 4546 4155 4c54 5f49 4e4c 494e  v=_DEFAULT_INLIN
+00001f50: 455f 5353 485f 454e 562c 0a20 2020 2020  E_SSH_ENV,.     
+00001f60: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00001f70: 6d5f 6461 7461 5f70 6174 683a 2073 7472  m_data_path: str
+00001f80: 203d 205f 4445 4641 554c 545f 534c 5552   = _DEFAULT_SLUR
+00001f90: 4d5f 4441 5441 5f50 4154 482c 0a20 2020  M_DATA_PATH,.   
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00001fb0: 7572 6d5f 696d 6167 6573 5f70 6174 683a  urm_images_path:
+00001fc0: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
+00001fd0: 534c 5552 4d5f 494d 4147 4553 5f50 4154  SLURM_IMAGES_PAT
+00001fe0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+00001ff0: 2020 2020 736c 7572 6d5f 636f 6e76 6572      slurm_conver
+00002000: 7465 7273 5f70 6174 683a 2073 7472 203d  ters_path: str =
+00002010: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
+00002020: 434f 4e56 4552 5445 5253 5f50 4154 482c  CONVERTERS_PATH,
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
+00002050: 7468 733a 2064 6963 7420 3d20 4e6f 6e65  ths: dict = None
+00002060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002070: 2020 2073 6c75 726d 5f6d 6f64 656c 5f72     slurm_model_r
+00002080: 6570 6f73 3a20 6469 6374 203d 204e 6f6e  epos: dict = Non
+00002090: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000020a0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+000020b0: 696d 6167 6573 3a20 6469 6374 203d 204e  images: dict = N
+000020c0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000020d0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+000020e0: 6c5f 6a6f 6273 3a20 6469 6374 203d 204e  l_jobs: dict = N
+000020f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00002100: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00002110: 6c5f 6a6f 6273 5f70 6172 616d 733a 2064  l_jobs_params: d
+00002120: 6963 7420 3d20 4e6f 6e65 2c0a 2020 2020  ict = None,.    
+00002130: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00002140: 726d 5f73 6372 6970 745f 7061 7468 3a20  rm_script_path: 
+00002150: 7374 7220 3d20 5f44 4546 4155 4c54 5f53  str = _DEFAULT_S
+00002160: 4c55 524d 5f47 4954 5f53 4352 4950 545f  LURM_GIT_SCRIPT_
+00002170: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00002180: 2020 2020 2020 2073 6c75 726d 5f73 6372         slurm_scr
+00002190: 6970 745f 7265 706f 3a20 7374 7220 3d20  ipt_repo: str = 
+000021a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+000021b0: 2020 2020 2020 2069 6e69 745f 736c 7572         init_slur
+000021c0: 6d3a 2062 6f6f 6c20 3d20 4661 6c73 652c  m: bool = False,
+000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021e0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+000021f0: 496e 6974 6961 6c69 7a65 7320 6120 6e65  Initializes a ne
+00002200: 7720 696e 7374 616e 6365 206f 6620 7468  w instance of th
+00002210: 6520 536c 7572 6d43 6c69 656e 7420 636c  e SlurmClient cl
+00002220: 6173 732e 0a0a 2020 2020 2020 2020 4974  ass...        It
+00002230: 2069 7320 7072 6566 6572 6162 6c65 2074   is preferable t
+00002240: 6f20 7573 6520 2366 726f 6d5f 636f 6e66  o use #from_conf
+00002250: 6967 282e 2e2e 2920 6d65 7468 6f64 2074  ig(...) method t
+00002260: 6f20 696e 6974 6961 6c69 7a65 0a20 2020  o initialize.   
+00002270: 2020 2020 2070 6172 616d 6574 6572 7320       parameters 
+00002280: 6672 6f6d 2061 2063 6f6e 6669 6720 6669  from a config fi
+00002290: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
+000022a0: 733a 0a20 2020 2020 2020 2020 2020 2068  s:.            h
+000022b0: 6f73 7420 2873 7472 2c20 6f70 7469 6f6e  ost (str, option
+000022c0: 616c 293a 2054 6865 2068 6f73 746e 616d  al): The hostnam
+000022d0: 6520 6f72 2049 5020 6164 6472 6573 7320  e or IP address 
+000022e0: 6f66 2074 6865 2072 656d 6f74 650a 2020  of the remote.  
+000022f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002300: 7276 6572 2e20 4465 6661 756c 7473 2074  rver. Defaults t
+00002310: 6f20 5f44 4546 4155 4c54 5f48 4f53 542e  o _DEFAULT_HOST.
+00002320: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00002330: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
+00002340: 293a 2054 6865 2075 7365 726e 616d 6520  ): The username 
+00002350: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
+00002360: 6563 7469 6e67 2074 6f20 0a20 2020 2020  ecting to .     
+00002370: 2020 2020 2020 2020 2020 2074 6865 2072             the r
+00002380: 656d 6f74 6520 7365 7276 6572 2e20 4465  emote server. De
+00002390: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
+000023a0: 7768 6963 6820 6465 6661 756c 7473 200a  which defaults .
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 746f 2063 6f6e 6669 672e 7573 6572 2e0a  to config.user..
+000023d0: 2020 2020 2020 2020 2020 2020 706f 7274              port
+000023e0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+000023f0: 3a20 5468 6520 5353 4820 706f 7274 2074  : The SSH port t
+00002400: 6f20 7573 6520 7768 656e 2063 6f6e 6e65  o use when conne
+00002410: 6374 696e 672e 0a20 2020 2020 2020 2020  cting..         
+00002420: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00002430: 746f 204e 6f6e 652c 2077 6869 6368 2064  to None, which d
+00002440: 6566 6175 6c74 7320 746f 2063 6f6e 6669  efaults to confi
+00002450: 672e 706f 7274 2e0a 2020 2020 2020 2020  g.port..        
+00002460: 2020 2020 636f 6e66 6967 2028 7374 722c      config (str,
+00002470: 206f 7074 696f 6e61 6c29 3a20 5061 7468   optional): Path
+00002480: 2074 6f20 7468 6520 5353 4820 636f 6e66   to the SSH conf
+00002490: 6967 2066 696c 652e 0a20 2020 2020 2020  ig file..       
+000024a0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+000024b0: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
+000024c0: 2064 6566 6175 6c74 7320 746f 2079 6f75   defaults to you
+000024d0: 7220 5353 4820 636f 6e66 6967 2066 696c  r SSH config fil
+000024e0: 652e 0a20 2020 2020 2020 2020 2020 2067  e..            g
+000024f0: 6174 6577 6179 2028 436f 6e6e 6563 7469  ateway (Connecti
+00002500: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2041  on, optional): A
+00002510: 6e20 6f70 7469 6f6e 616c 2067 6174 6577  n optional gatew
+00002520: 6179 2066 6f72 2063 6f6e 6e65 6374 696e  ay for connectin
+00002530: 6720 0a20 2020 2020 2020 2020 2020 2020  g .             
+00002540: 2020 2074 6872 6f75 6768 2061 206a 756d     through a jum
+00002550: 7020 686f 7374 2e20 4465 6661 756c 7473  p host. Defaults
+00002560: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
+00002570: 2020 2020 2020 666f 7277 6172 645f 6167        forward_ag
+00002580: 656e 7420 2862 6f6f 6c2c 206f 7074 696f  ent (bool, optio
+00002590: 6e61 6c29 3a20 5768 6574 6865 7220 746f  nal): Whether to
+000025a0: 2066 6f72 7761 7264 2074 6865 206c 6f63   forward the loc
+000025b0: 616c 2053 5348 200a 2020 2020 2020 2020  al SSH .        
+000025c0: 2020 2020 2020 2020 6167 656e 7420 746f          agent to
+000025d0: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
+000025e0: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
+000025f0: 4e6f 6e65 2c20 7768 6963 6820 0a20 2020  None, which .   
+00002600: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00002610: 6175 6c74 7320 746f 2063 6f6e 6669 672e  aults to config.
+00002620: 666f 7277 6172 645f 6167 656e 742e 0a20  forward_agent.. 
+00002630: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+00002640: 6374 5f74 696d 656f 7574 2028 696e 742c  ct_timeout (int,
+00002650: 206f 7074 696f 6e61 6c29 3a20 5469 6d65   optional): Time
+00002660: 6f75 7420 666f 7220 6573 7461 626c 6973  out for establis
+00002670: 6869 6e67 2074 6865 2053 5348 200a 2020  hing the SSH .  
+00002680: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002690: 6e6e 6563 7469 6f6e 2e20 4465 6661 756c  nnection. Defaul
+000026a0: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
+000026b0: 6820 6465 6661 756c 7473 200a 2020 2020  h defaults .    
+000026c0: 2020 2020 2020 2020 2020 2020 746f 2063              to c
+000026d0: 6f6e 6669 672e 7469 6d65 6f75 7473 2e63  onfig.timeouts.c
+000026e0: 6f6e 6e65 6374 2e0a 2020 2020 2020 2020  onnect..        
+000026f0: 2020 2020 636f 6e6e 6563 745f 6b77 6172      connect_kwar
+00002700: 6773 2028 6469 6374 2c20 6f70 7469 6f6e  gs (dict, option
+00002710: 616c 293a 2041 6464 6974 696f 6e61 6c20  al): Additional 
+00002720: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00002730: 7320 666f 7220 0a20 2020 2020 2020 2020  s for .         
+00002740: 2020 2020 2020 2074 6865 2075 6e64 6572         the under
+00002750: 6c79 696e 6720 5353 4820 636f 6e6e 6563  lying SSH connec
+00002760: 7469 6f6e 2e20 4861 6e64 6564 2076 6572  tion. Handed ver
+00002770: 6261 7469 6d20 746f 200a 2020 2020 2020  batim to .      
+00002780: 2020 2020 2020 2020 2020 6053 5348 436c            `SSHCl
+00002790: 6965 6e74 2e63 6f6e 6e65 6374 203c 7061  ient.connect <pa
+000027a0: 7261 6d69 6b6f 2e63 6c69 656e 742e 5353  ramiko.client.SS
+000027b0: 4843 6c69 656e 742e 636f 6e6e 6563 743e  HClient.connect>
+000027c0: 602e 200a 2020 2020 2020 2020 2020 2020  `. .            
+000027d0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+000027e0: 4e6f 6e65 2e20 0a20 2020 2020 2020 2020  None. .         
+000027f0: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
+00002800: 7620 2862 6f6f 6c2c 206f 7074 696f 6e61  v (bool, optiona
+00002810: 6c29 3a20 5768 6574 6865 7220 746f 2075  l): Whether to u
+00002820: 7365 2069 6e6c 696e 6520 5353 480a 2020  se inline SSH.  
+00002830: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00002840: 7669 726f 6e6d 656e 742e 2054 6869 7320  vironment. This 
+00002850: 6973 206e 6563 6573 7361 7279 2069 6620  is necessary if 
+00002860: 7468 6520 7265 6d6f 7465 2073 6572 7665  the remote serve
+00002870: 7220 6861 7320 0a20 2020 2020 2020 2020  r has .         
+00002880: 2020 2020 2020 2061 2072 6573 7472 6963         a restric
+00002890: 7465 6420 6060 4163 6365 7074 456e 7660  ted ``AcceptEnv`
+000028a0: 6020 7365 7474 696e 6720 2877 6869 6368  ` setting (which
+000028b0: 2069 7320 7468 6520 636f 6d6d 6f6e 200a   is the common .
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 6465 6661 756c 7429 2e20 4465 6661 756c  default). Defaul
+000028e0: 7473 2074 6f20 5f44 4546 4155 4c54 5f49  ts to _DEFAULT_I
+000028f0: 4e4c 494e 455f 5353 485f 454e 562e 0a20  NLINE_SSH_ENV.. 
+00002900: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00002910: 5f64 6174 615f 7061 7468 2028 7374 722c  _data_path (str,
+00002920: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00002930: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
+00002940: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
+00002950: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
+00002960: 2074 6865 2064 6174 6120 6669 6c65 7320   the data files 
+00002970: 666f 7220 536c 7572 6d20 6a6f 6273 2e0a  for Slurm jobs..
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 4465 6661 756c 7473 2074 6f20 5f44 4546  Defaults to _DEF
+000029a0: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
+000029b0: 5041 5448 2e0a 2020 2020 2020 2020 2020  PATH..          
+000029c0: 2020 736c 7572 6d5f 696d 6167 6573 5f70    slurm_images_p
+000029d0: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
+000029e0: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
+000029f0: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002a10: 6f6e 7461 696e 696e 6720 7468 6520 5369  ontaining the Si
+00002a20: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
+00002a30: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
+00002a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a50: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
+00002a60: 4641 554c 545f 534c 5552 4d5f 494d 4147  FAULT_SLURM_IMAG
+00002a70: 4553 5f50 4154 482e 0a20 2020 2020 2020  ES_PATH..       
+00002a80: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
+00002a90: 7274 6572 735f 7061 7468 2028 7374 722c  rters_path (str,
+00002aa0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00002ab0: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
+00002ac0: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
+00002ad0: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
+00002ae0: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
+00002af0: 2069 6d61 6765 7320 666f 7220 6669 6c65   images for file
+00002b00: 2063 6f6e 7665 7274 6572 732e 0a20 2020   converters..   
+00002b10: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00002b20: 6175 6c74 7320 746f 205f 4445 4641 554c  aults to _DEFAUL
+00002b30: 545f 534c 5552 4d5f 434f 4e56 4552 5445  T_SLURM_CONVERTE
+00002b40: 5253 5f50 4154 482e 0a20 2020 2020 2020  RS_PATH..       
+00002b50: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+00002b60: 5f70 6174 6873 2028 6469 6374 2c20 6f70  _paths (dict, op
+00002b70: 7469 6f6e 616c 293a 2041 2064 6963 7469  tional): A dicti
+00002b80: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00002b90: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+00002ba0: 2020 2020 2020 7061 7468 7320 746f 2074        paths to t
+00002bb0: 6865 2053 696e 6775 6c61 7269 7479 2069  he Singularity i
+00002bc0: 6d61 6765 7320 666f 7220 7370 6563 6966  mages for specif
+00002bd0: 6963 2053 6c75 726d 206a 6f62 206d 6f64  ic Slurm job mod
+00002be0: 656c 732e 0a20 2020 2020 2020 2020 2020  els..           
+00002bf0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00002c00: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
+00002c10: 2020 2073 6c75 726d 5f6d 6f64 656c 5f72     slurm_model_r
+00002c20: 6570 6f73 2028 6469 6374 2c20 6f70 7469  epos (dict, opti
+00002c30: 6f6e 616c 293a 2041 2064 6963 7469 6f6e  onal): A diction
+00002c40: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+00002c50: 6865 200a 2020 2020 2020 2020 2020 2020  he .            
+00002c60: 2020 2020 6769 7420 7265 706f 7369 746f      git reposito
+00002c70: 7269 6573 206f 6620 5369 6e67 756c 6172  ries of Singular
+00002c80: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
+00002c90: 7065 6369 6669 6320 536c 7572 6d20 0a20  pecific Slurm . 
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+00002cb0: 6f62 206d 6f64 656c 732e 0a20 2020 2020  ob models..     
+00002cc0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00002cd0: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+00002ce0: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
+00002cf0: 6f64 656c 5f69 6d61 6765 7320 2864 6963  odel_images (dic
+00002d00: 742c 206f 7074 696f 6e61 6c29 3a20 4120  t, optional): A 
+00002d10: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+00002d20: 696e 696e 6720 7468 6520 0a20 2020 2020  ining the .     
+00002d30: 2020 2020 2020 2020 2020 2064 6f63 6b65             docke
+00002d40: 7268 7562 206f 6620 7468 6520 5369 6e67  rhub of the Sing
+00002d50: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
+00002d60: 6f72 2073 7065 6369 6669 6320 536c 7572  or specific Slur
+00002d70: 6d20 0a20 2020 2020 2020 2020 2020 2020  m .             
+00002d80: 2020 206a 6f62 206d 6f64 656c 732e 2057     job models. W
+00002d90: 696c 6c20 6669 6c6c 2061 7574 6f6d 6174  ill fill automat
+00002da0: 6963 616c 6c79 2066 726f 6d20 7468 6520  ically from the 
+00002db0: 6461 7461 2069 6e20 7468 6520 6769 7420  data in the git 
+00002dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002dd0: 2072 6570 6f73 6974 6f72 7920 6966 2079   repository if y
+00002de0: 6f75 2073 6574 2069 6e69 745f 736c 7572  ou set init_slur
+00002df0: 6d2e 0a20 2020 2020 2020 2020 2020 2020  m..             
+00002e00: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
+00002e10: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+00002e20: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+00002e30: 7320 2864 6963 742c 206f 7074 696f 6e61  s (dict, optiona
+00002e40: 6c29 3a20 4120 6469 6374 696f 6e61 7279  l): A dictionary
+00002e50: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
+00002e60: 2020 2020 2020 2020 2020 2020 696e 666f              info
+00002e70: 726d 6174 696f 6e20 6162 6f75 7420 7370  rmation about sp
+00002e80: 6563 6966 6963 2053 6c75 726d 206a 6f62  ecific Slurm job
+00002e90: 206d 6f64 656c 732e 0a20 2020 2020 2020   models..       
+00002ea0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00002eb0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+00002ec0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00002ed0: 656c 5f6a 6f62 735f 7061 7261 6d73 2028  el_jobs_params (
+00002ee0: 6469 6374 2c20 6f70 7469 6f6e 616c 293a  dict, optional):
+00002ef0: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00002f00: 6e74 6169 6e69 6e67 0a20 2020 2020 2020  ntaining.       
+00002f10: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+00002f20: 6572 7320 666f 7220 7370 6563 6966 6963  ers for specific
+00002f30: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
+00002f40: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00002f50: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
+00002f60: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+00002f70: 2073 6c75 726d 5f73 6372 6970 745f 7061   slurm_script_pa
+00002f80: 7468 2028 7374 722c 206f 7074 696f 6e61  th (str, optiona
+00002f90: 6c29 3a20 5468 6520 7061 7468 2074 6f20  l): The path to 
+00002fa0: 7468 6520 6469 7265 6374 6f72 790a 2020  the directory.  
+00002fb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002fc0: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
+00002fd0: 726d 206a 6f62 2073 7562 6d69 7373 696f  rm job submissio
+00002fe0: 6e20 7363 7269 7074 7320 6f6e 2053 6c75  n scripts on Slu
+00002ff0: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
+00003000: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00003010: 5f44 4546 4155 4c54 5f53 4c55 524d 5f47  _DEFAULT_SLURM_G
+00003020: 4954 5f53 4352 4950 545f 5041 5448 2e0a  IT_SCRIPT_PATH..
+00003030: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00003040: 6d5f 7363 7269 7074 5f72 6570 6f20 2873  m_script_repo (s
+00003050: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
+00003060: 6865 2067 6974 2068 7474 7073 2055 524c  he git https URL
+00003070: 2066 6f72 2063 6c6f 6e69 6e67 0a20 2020   for cloning.   
+00003080: 2020 2020 2020 2020 2020 2020 2074 6865               the
+00003090: 2072 6570 6f20 636f 6e74 6169 6e69 6e67   repo containing
+000030a0: 2074 6865 2053 6c75 726d 206a 6f62 2073   the Slurm job s
+000030b0: 7562 6d69 7373 696f 6e20 7363 7269 7074  ubmission script
+000030c0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+000030d0: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
+000030e0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+000030f0: 2069 6e69 745f 736c 7572 6d20 2862 6f6f   init_slurm (boo
+00003100: 6c29 3a20 5768 6574 6865 7220 746f 2073  l): Whether to s
+00003110: 6574 2075 7020 7468 6520 7265 7175 6972  et up the requir
+00003120: 6564 2073 7472 7563 7475 7265 7320 0a20  ed structures . 
+00003130: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00003140: 6e20 536c 7572 6d20 6166 7465 7220 696e  n Slurm after in
+00003150: 6974 6961 7469 6e67 2074 6869 7320 636c  itiating this cl
+00003160: 6965 6e74 2e20 5468 6973 2069 6e63 6c75  ient. This inclu
+00003170: 6465 7320 6372 6561 7469 6e67 200a 2020  des creating .  
+00003180: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00003190: 7373 696e 6720 666f 6c64 6572 732c 2064  ssing folders, d
+000031a0: 6f77 6e6c 6f61 6469 6e67 2063 6f6e 7461  ownloading conta
+000031b0: 696e 6572 2069 6d61 6765 732c 2063 6c6f  iner images, clo
+000031c0: 6e69 6e67 2067 6974 2c65 7463 2e0a 2020  ning git,etc..  
+000031d0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+000031e0: 6973 2077 696c 6c20 7461 6b65 2061 2077  is will take a w
+000031f0: 6869 6c65 2061 7420 6669 7273 7420 6275  hile at first bu
+00003200: 7420 7769 6c6c 2076 616c 6964 6174 6520  t will validate 
+00003210: 796f 7572 2073 6574 7570 2e0a 2020 2020  your setup..    
+00003220: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00003230: 756c 7473 2074 6f20 4661 6c73 6520 746f  ults to False to
+00003240: 2073 6176 6520 7469 6d65 2e0a 2020 2020   save time..    
+00003250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00003260: 7375 7065 7228 536c 7572 6d43 6c69 656e  super(SlurmClien
+00003270: 742c 2073 656c 6629 2e5f 5f69 6e69 745f  t, self).__init_
+00003280: 5f28 686f 7374 2c0a 2020 2020 2020 2020  _(host,.        
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-000032c0: 6563 745f 6b77 6172 6773 2c0a 2020 2020  ect_kwargs,.    
+000032b0: 2020 7573 6572 2c0a 2020 2020 2020 2020    user,.        
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
-00003300: 5f65 6e76 290a 2020 2020 2020 2020 7365  _env).        se
-00003310: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
-00003320: 7468 203d 2073 6c75 726d 5f64 6174 615f  th = slurm_data_
-00003330: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
-00003340: 662e 736c 7572 6d5f 696d 6167 6573 5f70  f.slurm_images_p
-00003350: 6174 6820 3d20 736c 7572 6d5f 696d 6167  ath = slurm_imag
-00003360: 6573 5f70 6174 680a 2020 2020 2020 2020  es_path.        
-00003370: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
-00003380: 7274 6572 735f 7061 7468 203d 2073 6c75  rters_path = slu
-00003390: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
-000033a0: 7468 0a20 2020 2020 2020 2073 656c 662e  th.        self.
-000033b0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-000033c0: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
-000033d0: 7061 7468 730a 2020 2020 2020 2020 7365  paths.        se
-000033e0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-000033f0: 7061 7468 203d 2073 6c75 726d 5f73 6372  path = slurm_scr
-00003400: 6970 745f 7061 7468 0a20 2020 2020 2020  ipt_path.       
-00003410: 2073 656c 662e 736c 7572 6d5f 7363 7269   self.slurm_scri
-00003420: 7074 5f72 6570 6f20 3d20 736c 7572 6d5f  pt_repo = slurm_
-00003430: 7363 7269 7074 5f72 6570 6f0a 2020 2020  script_repo.    
-00003440: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
-00003450: 6f64 656c 5f72 6570 6f73 203d 2073 6c75  odel_repos = slu
-00003460: 726d 5f6d 6f64 656c 5f72 6570 6f73 0a20  rm_model_repos. 
-00003470: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
-00003480: 6d5f 6d6f 6465 6c5f 696d 6167 6573 203d  m_model_images =
-00003490: 2073 6c75 726d 5f6d 6f64 656c 5f69 6d61   slurm_model_ima
-000034a0: 6765 730a 2020 2020 2020 2020 7365 6c66  ges.        self
-000034b0: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
-000034c0: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
-000034d0: 6a6f 6273 0a20 2020 2020 2020 2073 656c  jobs.        sel
-000034e0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
-000034f0: 6273 5f70 6172 616d 7320 3d20 736c 7572  bs_params = slur
-00003500: 6d5f 6d6f 6465 6c5f 6a6f 6273 5f70 6172  m_model_jobs_par
-00003510: 616d 730a 0a20 2020 2020 2020 2023 2049  ams..        # I
-00003520: 6e69 7420 6361 6368 652e 204b 6565 7020  nit cache. Keep 
-00003530: 7265 7370 6f6e 7365 7320 666f 7220 3336  responses for 36
-00003540: 3020 7365 636f 6e64 730a 2020 2020 2020  0 seconds.      
-00003550: 2020 7365 6c66 2e63 6163 6865 203d 2072    self.cache = r
-00003560: 6571 7565 7374 735f 6361 6368 652e 6261  equests_cache.ba
-00003570: 636b 656e 6473 2e73 716c 6974 652e 5351  ckends.sqlite.SQ
-00003580: 4c69 7465 4361 6368 6528 0a20 2020 2020  LiteCache(.     
-00003590: 2020 2020 2020 2064 625f 7061 7468 3d22         db_path="
-000035a0: 6769 7468 7562 5f63 6163 6865 222c 2075  github_cache", u
-000035b0: 7365 5f74 656d 703d 5472 7565 290a 2020  se_temp=True).  
-000035c0: 2020 2020 2020 7365 6c66 2e67 6574 5f6f        self.get_o
-000035d0: 725f 6372 6561 7465 5f67 6974 6875 625f  r_create_github_
-000035e0: 7365 7373 696f 6e28 290a 0a20 2020 2020  session()..     
-000035f0: 2020 2073 656c 662e 696e 6974 5f77 6f72     self.init_wor
-00003600: 6b66 6c6f 7773 2829 0a20 2020 2020 2020  kflows().       
-00003610: 2073 656c 662e 7661 6c69 6461 7465 2876   self.validate(v
-00003620: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
-00003630: 7475 703d 696e 6974 5f73 6c75 726d 290a  tup=init_slurm).
-00003640: 0a20 2020 2064 6566 2069 6e69 745f 776f  .    def init_wo
-00003650: 726b 666c 6f77 7328 7365 6c66 2c20 666f  rkflows(self, fo
-00003660: 7263 655f 7570 6461 7465 3a20 626f 6f6c  rce_update: bool
-00003670: 203d 2046 616c 7365 293a 0a20 2020 2020   = False):.     
-00003680: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00003690: 6574 7269 6576 6573 2074 6865 2072 6571  etrieves the req
-000036a0: 7569 7265 6420 696e 666f 2066 6f72 2074  uired info for t
-000036b0: 6865 2063 6f6e 6669 6775 7265 6420 776f  he configured wo
-000036c0: 726b 666c 6f77 7320 6672 6f6d 2067 6974  rkflows from git
-000036d0: 6875 622e 0a20 2020 2020 2020 2049 7420  hub..        It 
-000036e0: 7769 6c6c 2066 696c 6c20 6073 6c75 726d  will fill `slurm
-000036f0: 5f6d 6f64 656c 5f69 6d61 6765 7360 2077  _model_images` w
-00003700: 6974 6820 646f 636b 6572 6875 6220 6c69  ith dockerhub li
-00003710: 6e6b 732e 0a0a 2020 2020 2020 2020 4172  nks...        Ar
-00003720: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00003730: 666f 7263 655f 7570 6461 7465 2028 626f  force_update (bo
-00003740: 6f6c 293a 2057 696c 6c20 6f76 6572 7772  ol): Will overwr
-00003750: 6974 6520 616c 7265 6164 7920 6769 7665  ite already give
-00003760: 6e20 7061 7468 730a 2020 2020 2020 2020  n paths.        
-00003770: 2020 2020 2020 2020 696e 2060 736c 7572          in `slur
-00003780: 6d5f 6d6f 6465 6c5f 696d 6167 6573 600a  m_model_images`.
-00003790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000037a0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-000037b0: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
-000037c0: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-000037d0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-000037e0: 6c5f 696d 6167 6573 203d 207b 7d0a 2020  l_images = {}.  
-000037f0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00003800: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7265  f.slurm_model_re
-00003810: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
-00003820: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-00003830: 224e 6f20 776f 726b 666c 6f77 7320 636f  "No workflows co
-00003840: 6e66 6967 7572 6564 2122 290a 2020 2020  nfigured!").    
-00003850: 2020 2020 2020 2020 7365 6c66 2e73 6c75          self.slu
-00003860: 726d 5f6d 6f64 656c 5f72 6570 6f73 203d  rm_model_repos =
-00003870: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00003880: 2320 736b 6970 7320 7468 6520 7365 7475  # skips the setu
-00003890: 700a 2020 2020 2020 2020 666f 7220 776f  p.        for wo
-000038a0: 726b 666c 6f77 2069 6e20 7365 6c66 2e73  rkflow in self.s
-000038b0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-000038c0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
-000038d0: 2020 2020 2069 6620 776f 726b 666c 6f77       if workflow
-000038e0: 206e 6f74 2069 6e20 7365 6c66 2e73 6c75   not in self.slu
-000038f0: 726d 5f6d 6f64 656c 5f69 6d61 6765 7320  rm_model_images 
-00003900: 6f72 2066 6f72 6365 5f75 7064 6174 653a  or force_update:
-00003910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003920: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
-00003930: 203d 2073 656c 662e 7075 6c6c 5f64 6573   = self.pull_des
-00003940: 6372 6970 746f 725f 6672 6f6d 5f67 6974  criptor_from_git
-00003950: 6875 6228 776f 726b 666c 6f77 290a 2020  hub(workflow).  
-00003960: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00003970: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
-00003980: 2573 272c 2077 6f72 6b66 6c6f 772c 206a  %s', workflow, j
-00003990: 736f 6e5f 6465 7363 7269 7074 6f72 290a  son_descriptor).
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 696d 6167 6520 3d20 6a73 6f6e 5f64 6573  image = json_des
-000039c0: 6372 6970 746f 725b 2763 6f6e 7461 696e  criptor['contain
-000039d0: 6572 2d69 6d61 6765 275d 5b27 696d 6167  er-image']['imag
-000039e0: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
-000039f0: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
-00003a00: 6f64 656c 5f69 6d61 6765 735b 776f 726b  odel_images[work
-00003a10: 666c 6f77 5d20 3d20 696d 6167 650a 0a20  flow] = image.. 
-00003a20: 2020 2064 6566 2073 6574 7570 5f73 6c75     def setup_slu
-00003a30: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
-00003a40: 2020 2222 220a 2020 2020 2020 2020 5661    """.        Va
-00003a50: 6c69 6461 7465 7320 6f72 2063 7265 6174  lidates or creat
-00003a60: 6573 2074 6865 2072 6571 7569 7265 6420  es the required 
-00003a70: 7365 7475 7020 6f6e 2074 6865 2053 6c75  setup on the Slu
-00003a80: 726d 2063 6c75 7374 6572 2e0a 0a20 2020  rm cluster...   
-00003a90: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-00003aa0: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
-00003ab0: 7074 696f 6e3a 2069 6620 6974 2063 616e  ption: if it can
-00003ac0: 6e6f 7420 636f 6e6e 6563 7420 746f 2053  not connect to S
-00003ad0: 6c75 726d 2c20 6f72 2072 756e 7320 696e  lurm, or runs in
-00003ae0: 746f 2061 6e20 6572 726f 720a 2020 2020  to an error.    
-00003af0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003b00: 6966 2073 656c 662e 7661 6c69 6461 7465  if self.validate
-00003b10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00003b20: 2320 312e 2043 7265 6174 6520 6469 7265  # 1. Create dire
-00003b30: 6374 6f72 6965 730a 2020 2020 2020 2020  ctories.        
-00003b40: 2020 2020 7365 6c66 2e73 6574 7570 5f64      self.setup_d
-00003b50: 6972 6563 746f 7269 6573 2829 0a0a 2020  irectories()..  
-00003b60: 2020 2020 2020 2020 2020 2320 322e 2043            # 2. C
-00003b70: 6c6f 6e65 2067 6974 0a20 2020 2020 2020  lone git.       
-00003b80: 2020 2020 2073 656c 662e 7365 7475 705f       self.setup_
-00003b90: 6a6f 625f 7363 7269 7074 7328 290a 0a20  job_scripts().. 
-00003ba0: 2020 2020 2020 2020 2020 2023 2033 2e20             # 3. 
-00003bb0: 5365 7475 7020 636f 6e76 6572 7465 7273  Setup converters
-00003bc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003bd0: 662e 7365 7475 705f 636f 6e76 6572 7465  f.setup_converte
-00003be0: 7273 2829 0a0a 2020 2020 2020 2020 2020  rs()..          
-00003bf0: 2020 2320 342e 2044 6f77 6e6c 6f61 6420    # 4. Download 
-00003c00: 776f 726b 666c 6f77 2069 6d61 6765 730a  workflow images.
-00003c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003c20: 2e73 6574 7570 5f63 6f6e 7461 696e 6572  .setup_container
-00003c30: 5f69 6d61 6765 7328 290a 0a20 2020 2020  _images()..     
-00003c40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003c50: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00003c60: 6365 7074 696f 6e28 2246 6169 6c75 7265  ception("Failure
-00003c70: 2069 6e20 636f 6e6e 6563 7469 6e67 2074   in connecting t
-00003c80: 6f20 536c 7572 6d20 636c 7573 7465 7222  o Slurm cluster"
-00003c90: 290a 0a20 2020 2064 6566 2073 6574 7570  )..    def setup
-00003ca0: 5f63 6f6e 7461 696e 6572 5f69 6d61 6765  _container_image
-00003cb0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00003cc0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
-00003cd0: 7320 7570 2063 6f6e 7461 696e 6572 2069  s up container i
-00003ce0: 6d61 6765 7320 666f 7220 536c 7572 6d20  mages for Slurm 
-00003cf0: 6f70 6572 6174 696f 6e73 2e0a 0a20 2020  operations...   
-00003d00: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-00003d10: 6f6e 2063 7265 6174 6573 2073 7065 6369  on creates speci
-00003d20: 6669 6320 6469 7265 6374 6f72 6965 7320  fic directories 
-00003d30: 666f 7220 636f 6e74 6169 6e65 7220 696d  for container im
-00003d40: 6167 6573 2061 6e64 2070 756c 6c73 0a20  ages and pulls. 
-00003d50: 2020 2020 2020 206e 6563 6573 7361 7279         necessary
-00003d60: 2069 6d61 6765 7320 6672 6f6d 2044 6f63   images from Doc
-00003d70: 6b65 7220 7265 706f 7369 746f 7269 6573  ker repositories
-00003d80: 2e20 4974 2067 656e 6572 6174 6573 2061  . It generates a
-00003d90: 6e64 2065 7865 6375 7465 730a 2020 2020  nd executes.    
-00003da0: 2020 2020 6120 7363 7269 7074 2074 6f20      a script to 
-00003db0: 7075 6c6c 2069 6d61 6765 7320 616e 6420  pull images and 
-00003dc0: 636f 7069 6573 2069 7420 746f 2074 6865  copies it to the
-00003dd0: 2072 656d 6f74 6520 6c6f 6361 7469 6f6e   remote location
-00003de0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00003df0: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
-00003e00: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
-00003e10: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
-00003e20: 6520 6578 6563 7574 696e 6720 636f 6d6d  e executing comm
-00003e30: 616e 6473 206f 7220 636f 7079 696e 6720  ands or copying 
-00003e40: 6669 6c65 732e 0a20 2020 2020 2020 2022  files..        "
-00003e50: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
-00003e60: 6174 6520 7370 6563 6966 6963 2077 6f72  ate specific wor
-00003e70: 6b66 6c6f 7720 6469 7273 0a20 2020 2020  kflow dirs.     
-00003e80: 2020 2077 6974 6820 7365 6c66 2e63 6428     with self.cd(
-00003e90: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
-00003ea0: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00003eb0: 2020 2020 2069 6620 7365 6c66 2e73 6c75       if self.slu
-00003ec0: 726d 5f6d 6f64 656c 5f70 6174 6873 3a0a  rm_model_paths:.
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 6d6f 6465 6c70 6174 6873 203d 2022 2022  modelpaths = " "
-00003ef0: 2e6a 6f69 6e28 7365 6c66 2e73 6c75 726d  .join(self.slurm
-00003f00: 5f6d 6f64 656c 5f70 6174 6873 2e76 616c  _model_paths.val
-00003f10: 7565 7328 2929 0a20 2020 2020 2020 2020  ues()).         
-00003f20: 2020 2020 2020 2023 206d 6b64 6972 2063         # mkdir c
-00003f30: 656c 6c70 726f 6669 6c65 7220 696d 6167  ellprofiler imag
-00003f40: 656a 202e 2e2e 0a20 2020 2020 2020 2020  ej ....         
-00003f50: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
-00003f60: 7275 6e5f 636f 6d6d 616e 6473 285b 6622  run_commands([f"
-00003f70: 6d6b 6469 7220 2d70 207b 6d6f 6465 6c70  mkdir -p {modelp
-00003f80: 6174 6873 7d22 5d29 0a20 2020 2020 2020  aths}"]).       
-00003f90: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00003fa0: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
-00003fb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00003fc0: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
-00003fd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003fe0: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00003ff0: 5f69 6d61 6765 733a 0a20 2020 2020 2020  _images:.       
-00004000: 2020 2020 2020 2020 2070 756c 6c5f 636f           pull_co
-00004010: 6d6d 616e 6473 203d 205b 5d0a 2020 2020  mmands = [].    
-00004020: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00004030: 7766 2c20 696d 6167 6520 696e 2073 656c  wf, image in sel
-00004040: 662e 736c 7572 6d5f 6d6f 6465 6c5f 696d  f.slurm_model_im
-00004050: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
-00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004070: 2020 7265 706f 203d 2073 656c 662e 736c    repo = self.sl
-00004080: 7572 6d5f 6d6f 6465 6c5f 7265 706f 735b  urm_model_repos[
-00004090: 7766 5d0a 2020 2020 2020 2020 2020 2020  wf].            
-000040a0: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
-000040b0: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-000040c0: 7061 7468 735b 7766 5d0a 2020 2020 2020  paths[wf].      
-000040d0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
-000040e0: 2076 6572 7369 6f6e 203d 2073 656c 662e   version = self.
-000040f0: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
-00004100: 6f6d 5f75 726c 2872 6570 6f29 0a20 2020  om_url(repo).   
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2069 6620 7665 7273 696f 6e20 3d3d 2022   if version == "
-00004130: 6d61 7374 6572 223a 0a20 2020 2020 2020  master":.       
-00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004150: 2076 6572 7369 6f6e 203d 2022 6c61 7465   version = "late
-00004160: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
-00004170: 2020 2020 2020 2020 7075 6c6c 5f74 656d          pull_tem
-00004180: 706c 6174 6520 3d20 2265 6368 6f20 2773  plate = "echo 's
-00004190: 7461 7274 696e 6720 2470 6174 6820 2476  tarting $path $v
-000041a0: 6572 7369 6f6e 2720 3e3e 2073 696e 672e  ersion' >> sing.
-000041b0: 6c6f 675c 6e6e 6f68 7570 2073 6820 2d63  log\nnohup sh -c
-000041c0: 205c 2273 696e 6775 6c61 7269 7479 2070   \"singularity p
-000041d0: 756c 6c20 2d2d 6469 7361 626c 652d 6361  ull --disable-ca
-000041e0: 6368 6520 2d2d 6469 7220 2470 6174 6820  che --dir $path 
-000041f0: 646f 636b 6572 3a2f 2f24 696d 6167 653a  docker://$image:
-00004200: 2476 6572 7369 6f6e 3b20 6563 686f 2027  $version; echo '
-00004210: 6669 6e69 7368 6564 2024 7061 7468 2024  finished $path $
-00004220: 7665 7273 696f 6e27 5c22 203e 3e20 7369  version'\" >> si
-00004230: 6e67 2e6c 6f67 2032 3e26 3120 2620 6469  ng.log 2>&1 & di
-00004240: 736f 776e 220a 2020 2020 2020 2020 2020  sown".          
-00004250: 2020 2020 2020 2020 2020 7420 3d20 5465            t = Te
-00004260: 6d70 6c61 7465 2870 756c 6c5f 7465 6d70  mplate(pull_temp
-00004270: 6c61 7465 290a 2020 2020 2020 2020 2020  late).          
-00004280: 2020 2020 2020 2020 2020 7375 6273 7469            substi
-00004290: 7475 7465 7320 3d20 7b7d 0a20 2020 2020  tutes = {}.     
-000042a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000042b0: 7562 7374 6974 7574 6573 5b27 7061 7468  ubstitutes['path
-000042c0: 275d 203d 2070 6174 680a 2020 2020 2020  '] = path.      
-000042d0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000042e0: 6273 7469 7475 7465 735b 2769 6d61 6765  bstitutes['image
-000042f0: 275d 203d 2069 6d61 6765 0a20 2020 2020  '] = image.     
-00004300: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004310: 7562 7374 6974 7574 6573 5b27 7665 7273  ubstitutes['vers
-00004320: 696f 6e27 5d20 3d20 7665 7273 696f 6e0a  ion'] = version.
-00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004340: 2020 2020 636d 6420 3d20 742e 7361 6665      cmd = t.safe
-00004350: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
-00004360: 7469 7475 7465 7329 0a20 2020 2020 2020  titutes).       
-00004370: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00004380: 6765 722e 6465 6275 6728 6622 7375 6273  ger.debug(f"subs
-00004390: 7469 7475 7465 643a 207b 636d 647d 2229  tituted: {cmd}")
-000043a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000043b0: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
-000043c0: 6473 2e61 7070 656e 6428 636d 6429 0a20  ds.append(cmd). 
-000043d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000043e0: 6372 6970 745f 6e61 6d65 203d 2022 7075  cript_name = "pu
-000043f0: 6c6c 5f69 6d61 6765 732e 7368 220a 2020  ll_images.sh".  
-00004400: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00004410: 6d70 6c61 7465 5f73 6372 6970 7420 3d20  mplate_script = 
-00004420: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
-00004430: 2229 2e6a 6f69 6e70 6174 6828 7363 7269  ").joinpath(scri
-00004440: 7074 5f6e 616d 6529 0a20 2020 2020 2020  pt_name).       
-00004450: 2020 2020 2020 2020 2077 6974 6820 7465           with te
-00004460: 6d70 6c61 7465 5f73 6372 6970 742e 6f70  mplate_script.op
-00004470: 656e 2827 7227 2920 6173 2066 3a0a 2020  en('r') as f:.  
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 7372 6320 3d20 5465 6d70 6c61 7465    src = Template
-000044a0: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000044c0: 7562 7374 6974 7574 6520 3d20 7b27 7075  ubstitute = {'pu
-000044d0: 6c6c 636f 6d6d 616e 6473 273a 2022 5c6e  llcommands': "\n
-000044e0: 222e 6a6f 696e 2870 756c 6c5f 636f 6d6d  ".join(pull_comm
-000044f0: 616e 6473 297d 0a20 2020 2020 2020 2020  ands)}.         
-00004500: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
-00004510: 6372 6970 7420 3d20 7372 632e 7361 6665  cript = src.safe
-00004520: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
-00004530: 7469 7475 7465 290a 2020 2020 2020 2020  titute).        
-00004540: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00004550: 6562 7567 2866 2273 7562 7374 6974 7574  ebug(f"substitut
-00004560: 6564 3a5c 6e20 7b6a 6f62 5f73 6372 6970  ed:\n {job_scrip
-00004570: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
-00004580: 2020 2020 2023 2063 6f70 7920 746f 2072       # copy to r
-00004590: 656d 6f74 6520 6669 6c65 0a20 2020 2020  emote file.     
-000045a0: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-000045b0: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
-000045c0: 6d5f 696d 6167 6573 5f70 6174 682b 222f  m_images_path+"/
-000045d0: 222b 7363 7269 7074 5f6e 616d 650a 2020  "+script_name.  
-000045e0: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
-000045f0: 3d20 7365 6c66 2e70 7574 286c 6f63 616c  = self.put(local
-00004600: 3d69 6f2e 5374 7269 6e67 494f 286a 6f62  =io.StringIO(job
-00004610: 5f73 6372 6970 7429 2c0a 2020 2020 2020  _script),.      
-00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 2020 2020 2072 656d 6f74 653d 6675         remote=fu
-00004640: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
-00004650: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
-00004660: 2274 696d 6520 7368 207b 7363 7269 7074  "time sh {script
-00004670: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
-00004680: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
-00004690: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
-000046a0: 6d64 5d29 0a20 2020 2020 2020 2020 2020  md]).           
-000046b0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
-000046c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000046d0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-000046e0: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
-000046f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00004700: 6572 2e69 6e66 6f28 722e 7374 646f 7574  er.info(r.stdout
-00004710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004720: 2020 6c6f 6767 6572 2e69 6e66 6f28 2249    logger.info("I
-00004730: 6e69 7469 6174 6564 2064 6f77 6e6c 6f61  nitiated downloa
-00004740: 6469 6e67 2061 6e64 2062 7569 6c64 696e  ding and buildin
-00004750: 6722 202b 0a20 2020 2020 2020 2020 2020  g" +.           
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2022 2063 6f6e 7461 696e 6572 2069 6d61   " container ima
-00004780: 6765 7320 6f6e 2053 6c75 726d 2e22 202b  ges on Slurm." +
-00004790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000047a0: 2020 2020 2020 2020 2020 2020 2022 2054               " T
-000047b0: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
-000047c0: 7768 696c 6520 696e 2074 6865 2062 6163  while in the bac
-000047d0: 6b67 726f 756e 642e 2220 2b20 0a20 2020  kground." + .   
-000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047f0: 2020 2020 2020 2020 2022 2043 6865 636b           " Check
-00004800: 2027 7369 6e67 2e6c 6f67 2720 6f6e 2053   'sing.log' on S
-00004810: 6c75 726d 2066 6f72 2070 726f 6772 6573  lurm for progres
-00004820: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
-00004830: 2020 2020 2023 2023 2063 6c65 616e 7570       # # cleanup
-00004840: 2067 6961 6e74 2073 696e 6775 6c61 7269   giant singulari
-00004850: 7479 2063 6163 6865 210a 2020 2020 2020  ty cache!.      
-00004860: 2020 2020 2020 2020 2020 2320 7573 696e            # usin
-00004870: 6720 2d2d 6469 7361 626c 652d 6361 6368  g --disable-cach
-00004880: 6520 6265 6361 7573 6520 7765 2072 756e  e because we run
-00004890: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
-000048a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-000048b0: 2020 2023 2063 6d64 203d 2022 7369 6e67     # cmd = "sing
-000048c0: 756c 6172 6974 7920 6361 6368 6520 636c  ularity cache cl
-000048d0: 6561 6e20 2d66 220a 2020 2020 2020 2020  ean -f".        
-000048e0: 2020 2020 2020 2020 2320 7220 3d20 7365          # r = se
-000048f0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00004900: 5b63 6d64 5d29 0a0a 2020 2020 6465 6620  [cmd])..    def 
-00004910: 7365 7475 705f 636f 6e76 6572 7465 7273  setup_converters
-00004920: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004930: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
-00004940: 2075 7020 636f 6e76 6572 7465 7273 2066   up converters f
-00004950: 6f72 2053 6c75 726d 206f 7065 7261 7469  or Slurm operati
-00004960: 6f6e 732e 0a0a 2020 2020 2020 2020 5468  ons...        Th
-00004970: 6973 2066 756e 6374 696f 6e20 6372 6561  is function crea
-00004980: 7465 7320 6e65 6365 7373 6172 7920 6469  tes necessary di
-00004990: 7265 6374 6f72 6965 7320 666f 7220 636f  rectories for co
-000049a0: 6e76 6572 7465 7273 2061 6e64 2063 6f70  nverters and cop
-000049b0: 6965 730a 2020 2020 2020 2020 636f 6e76  ies.        conv
-000049c0: 6572 7465 7220 7363 7269 7074 7320 616e  erter scripts an
-000049d0: 6420 6465 6669 6e69 7469 6f6e 7320 746f  d definitions to
-000049e0: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
-000049f0: 206c 6f63 6174 696f 6e73 2e20 4974 2061   locations. It a
-00004a00: 6c73 6f0a 2020 2020 2020 2020 6275 696c  lso.        buil
-00004a10: 6473 2053 696e 6775 6c61 7269 7479 2063  ds Singularity c
-00004a20: 6f6e 7461 696e 6572 7320 6672 6f6d 2074  ontainers from t
-00004a30: 6865 2070 726f 7669 6465 6420 6465 6669  he provided defi
-00004a40: 6e69 7469 6f6e 732e 0a0a 2020 2020 2020  nitions...      
-00004a50: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00004a60: 2020 2020 2020 5353 4845 7863 6570 7469        SSHExcepti
-00004a70: 6f6e 3a20 4966 2074 6865 7265 2069 7320  on: If there is 
-00004a80: 616e 2069 7373 7565 2065 7865 6375 7469  an issue executi
-00004a90: 6e67 2063 6f6d 6d61 6e64 7320 6f72 2063  ng commands or c
-00004aa0: 6f70 7969 6e67 2066 696c 6573 2e0a 2020  opying files..  
-00004ab0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00004ac0: 2020 636f 6e76 6572 745f 636d 6473 203d    convert_cmds =
-00004ad0: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-00004ae0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
-00004af0: 7465 7273 5f70 6174 683a 0a20 2020 2020  ters_path:.     
-00004b00: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
-00004b10: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-00004b20: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-00004b30: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
-00004b40: 687d 2229 0a20 2020 2020 2020 2072 203d  h}").        r =
-00004b50: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00004b60: 6473 2863 6f6e 7665 7274 5f63 6d64 7329  ds(convert_cmds)
-00004b70: 0a20 2020 2020 2020 2023 2063 6f70 7920  .        # copy 
-00004b80: 6765 6e65 7269 6320 6a6f 6220 6172 7261  generic job arra
-00004b90: 7920 7363 7269 7074 206f 7665 7220 746f  y script over to
-00004ba0: 2073 6c75 726d 0a20 2020 2020 2020 2063   slurm.        c
-00004bb0: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
-00004bc0: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
-00004bd0: 6365 7322 292e 6a6f 696e 7061 7468 280a  ces").joinpath(.
-00004be0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00004bf0: 7665 7274 5f6a 6f62 5f61 7272 6179 2e73  vert_job_array.s
-00004c00: 6822 290a 2020 2020 2020 2020 5f20 3d20  h").        _ = 
-00004c10: 7365 6c66 2e70 7574 286c 6f63 616c 3d63  self.put(local=c
-00004c20: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
-00004c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004c40: 2020 2020 2020 2072 656d 6f74 653d 7365         remote=se
-00004c50: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-00004c60: 7061 7468 290a 2020 2020 2020 2020 2320  path).        # 
-00004c70: 6375 7272 656e 746c 7920 6b6e 6f77 6e20  currently known 
-00004c80: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
-00004c90: 2020 2023 2033 612e 205a 4152 5220 746f     # 3a. ZARR to
-00004ca0: 2054 4946 460a 2020 2020 2020 2020 2320   TIFF.        # 
-00004cb0: 544f 444f 2065 7874 7261 6374 2074 6865  TODO extract the
-00004cc0: 7365 2076 616c 7565 7320 746f 2065 2e67  se values to e.g
-00004cd0: 2e20 636f 6e66 6967 2069 6620 7765 2068  . config if we h
-00004ce0: 6176 6520 6d6f 7265 0a20 2020 2020 2020  ave more.       
-00004cf0: 2063 6f6e 7665 7274 5f6e 616d 6520 3d20   convert_name = 
-00004d00: 2263 6f6e 7665 7274 5f7a 6172 725f 746f  "convert_zarr_to
-00004d10: 5f74 6966 6622 0a20 2020 2020 2020 2063  _tiff".        c
-00004d20: 6f6e 7665 7274 5f70 7920 3d20 6622 7b63  onvert_py = f"{c
-00004d30: 6f6e 7665 7274 5f6e 616d 657d 2e70 7922  onvert_name}.py"
-00004d40: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
-00004d50: 5f73 6372 6970 745f 6c6f 6361 6c20 3d20  _script_local = 
-00004d60: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
-00004d70: 2229 2e6a 6f69 6e70 6174 6828 0a20 2020  ").joinpath(.   
-00004d80: 2020 2020 2020 2020 2063 6f6e 7665 7274           convert
-00004d90: 5f70 7929 0a20 2020 2020 2020 2063 6f6e  _py).        con
-00004da0: 7665 7274 5f64 6566 203d 2066 227b 636f  vert_def = f"{co
-00004db0: 6e76 6572 745f 6e61 6d65 7d2e 6465 6622  nvert_name}.def"
-00004dc0: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
-00004dd0: 5f64 6566 5f6c 6f63 616c 203d 2066 696c  _def_local = fil
-00004de0: 6573 2822 7265 736f 7572 6365 7322 292e  es("resources").
-00004df0: 6a6f 696e 7061 7468 280a 2020 2020 2020  joinpath(.      
-00004e00: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
-00004e10: 6629 0a20 2020 2020 2020 205f 203d 2073  f).        _ = s
-00004e20: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
-00004e30: 6e76 6572 745f 7363 7269 7074 5f6c 6f63  nvert_script_loc
-00004e40: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00004e50: 2020 2020 2020 2020 2072 656d 6f74 653d           remote=
-00004e60: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
-00004e70: 7274 6572 735f 7061 7468 290a 2020 2020  rters_path).    
-00004e80: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
-00004e90: 286c 6f63 616c 3d63 6f6e 7665 7274 5f64  (local=convert_d
-00004ea0: 6566 5f6c 6f63 616c 2c0a 2020 2020 2020  ef_local,.      
-00004eb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004ec0: 656d 6f74 653d 7365 6c66 2e73 6c75 726d  emote=self.slurm
-00004ed0: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
-00004ee0: 290a 2020 2020 2020 2020 2320 4275 696c  ).        # Buil
-00004ef0: 6420 7369 6e67 756c 6172 6974 7920 636f  d singularity co
-00004f00: 6e74 6169 6e65 7220 6672 6f6d 2064 6566  ntainer from def
-00004f10: 696e 6974 696f 6e0a 2020 2020 2020 2020  inition.        
-00004f20: 7769 7468 2073 656c 662e 6364 2873 656c  with self.cd(sel
-00004f30: 662e 736c 7572 6d5f 636f 6e76 6572 7465  f.slurm_converte
-00004f40: 7273 5f70 6174 6829 3a0a 2020 2020 2020  rs_path):.      
-00004f50: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
-00004f60: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
-00004f70: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00004f80: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004fa0: 2054 4f44 4f20 4368 616e 6765 2074 6865   TODO Change the
-00004fb0: 2074 6d70 2064 6972 3f0a 2020 2020 2020   tmp dir?.      
-00004fc0: 2020 2020 2020 2020 2020 2320 6578 706f            # expo
-00004fd0: 7274 2053 494e 4755 4c41 5249 5459 5f54  rt SINGULARITY_T
-00004fe0: 4d50 4449 523d 7e2f 6d79 2d73 6372 6174  MPDIR=~/my-scrat
-00004ff0: 6368 2f74 6d70 3b0a 2020 2020 2020 2020  ch/tmp;.        
-00005000: 2020 2020 2020 2020 2320 6f6e 6c79 2069          # only i
-00005010: 6620 6669 6c65 2064 6f65 7320 6e6f 7420  f file does not 
-00005020: 6578 6973 7420 7965 740a 2020 2020 2020  exist yet.      
-00005030: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
-00005040: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
-00005050: 6622 5b20 2120 2d66 207b 636f 6e76 6572  f"[ ! -f {conver
-00005060: 745f 6e61 6d65 7d2e 7369 6620 5d22 290a  t_name}.sif ]").
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2320 4544 4954 202d 2d20 4e4f 2c20 7468  # EDIT -- NO, th
-00005090: 656e 2077 6520 6361 6e27 7420 7570 6461  en we can't upda
-000050a0: 7465 2120 466f 7263 6520 7265 6275 696c  te! Force rebuil
-000050b0: 6421 0a20 2020 2020 2020 2020 2020 2020  d!.             
-000050c0: 2020 2023 2064 6f77 6e6c 6f61 6420 2f62     # download /b
-000050d0: 7569 6c64 206e 6577 2063 6f6e 7461 696e  uild new contain
-000050e0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-000050f0: 2020 2063 6f6e 7665 7274 5f63 6d64 732e     convert_cmds.
-00005100: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-00005110: 2020 2020 2020 2020 2020 2020 6622 7369              f"si
-00005120: 6e67 756c 6172 6974 7920 6275 696c 6420  ngularity build 
-00005130: 2d46 207b 636f 6e76 6572 745f 6e61 6d65  -F {convert_name
-00005140: 7d2e 7369 6620 7b63 6f6e 7665 7274 5f64  }.sif {convert_d
-00005150: 6566 7d20 3e3e 2073 696e 672e 6c6f 6720  ef} >> sing.log 
-00005160: 323e 2631 203b 2065 6368 6f20 2766 696e  2>&1 ; echo 'fin
-00005170: 6973 6865 6420 7b63 6f6e 7665 7274 5f6e  ished {convert_n
-00005180: 616d 657d 2e73 6966 2720 2622 290a 2020  ame}.sif' &").  
-00005190: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
-000051a0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-000051b0: 636f 6e76 6572 745f 636d 6473 290a 0a20  convert_cmds).. 
-000051c0: 2020 2064 6566 2073 6574 7570 5f6a 6f62     def setup_job
-000051d0: 5f73 6372 6970 7473 2873 656c 6629 3a0a  _scripts(self):.
-000051e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000051f0: 2020 2020 5365 7473 2075 7020 6a6f 6220      Sets up job 
-00005200: 7363 7269 7074 7320 666f 7220 536c 7572  scripts for Slur
-00005210: 6d20 6f70 6572 6174 696f 6e73 2e0a 0a20  m operations... 
-00005220: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
-00005230: 7469 6f6e 2065 6974 6865 7220 636c 6f6e  tion either clon
-00005240: 6573 2061 2047 6974 2072 6570 6f73 6974  es a Git reposit
-00005250: 6f72 7920 636f 6e74 6169 6e69 6e67 206a  ory containing j
-00005260: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
-00005270: 2020 2069 6e74 6f20 7468 6520 7370 6563     into the spec
-00005280: 6966 6965 6420 7363 7269 7074 2070 6174  ified script pat
-00005290: 6820 6f72 2067 656e 6572 6174 6573 2073  h or generates s
-000052a0: 6372 6970 7473 206c 6f63 616c 6c79 2069  cripts locally i
-000052b0: 6620 6e6f 2072 6570 6f73 6974 6f72 790a  f no repository.
-000052c0: 2020 2020 2020 2020 6973 2070 726f 7669          is provi
-000052d0: 6465 642e 0a0a 2020 2020 2020 2020 5261  ded...        Ra
-000052e0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-000052f0: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
-00005300: 4966 2074 6865 7265 2069 7320 616e 2069  If there is an i
-00005310: 7373 7565 2065 7865 6375 7469 6e67 2047  ssue executing G
-00005320: 6974 2063 6f6d 6d61 6e64 7320 6f72 2067  it commands or g
-00005330: 656e 6572 6174 696e 6720 7363 7269 7074  enerating script
-00005340: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00005350: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00005360: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-00005370: 2061 6e64 2073 656c 662e 736c 7572 6d5f   and self.slurm_
-00005380: 7363 7269 7074 5f70 6174 683a 0a20 2020  script_path:.   
-00005390: 2020 2020 2020 2020 2023 2067 6974 2063           # git c
-000053a0: 6c6f 6e65 2069 6e74 6f20 7363 7269 7074  lone into script
-000053b0: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
-000053c0: 2020 656e 7620 3d20 7b0a 2020 2020 2020    env = {.      
-000053d0: 2020 2020 2020 2020 2020 2252 4550 4f53            "REPOS
-000053e0: 5243 223a 2073 656c 662e 736c 7572 6d5f  RC": self.slurm_
-000053f0: 7363 7269 7074 5f72 6570 6f2c 0a20 2020  script_repo,.   
-00005400: 2020 2020 2020 2020 2020 2020 2022 4c4f               "LO
-00005410: 4341 4c52 4550 4f22 3a20 7365 6c66 2e73  CALREPO": self.s
-00005420: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
-00005430: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00005440: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00005450: 2027 6769 7420 636c 6f6e 6520 2224 5245   'git clone "$RE
-00005460: 504f 5352 4322 2022 244c 4f43 414c 5245  POSRC" "$LOCALRE
-00005470: 504f 2220 323e 202f 6465 762f 6e75 6c6c  PO" 2> /dev/null
-00005480: 207c 7c20 6769 7420 2d43 2022 244c 4f43   || git -C "$LOC
-00005490: 414c 5245 504f 2220 7075 6c6c 270a 2020  ALREPO" pull'.  
-000054a0: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
-000054b0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-000054c0: 5b63 6d64 5d2c 2065 6e76 290a 2020 2020  [cmd], env).    
-000054d0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-000054e0: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
-000054f0: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00005500: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
-00005510: 2020 2065 6c69 6620 7365 6c66 2e73 6c75     elif self.slu
-00005520: 726d 5f73 6372 6970 745f 7061 7468 3a0a  rm_script_path:.
-00005530: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00005540: 6e65 7261 7465 2073 6372 6970 7473 0a20  nerate scripts. 
-00005550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005560: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
-00005570: 6970 7473 2867 656e 6572 6174 655f 6a6f  ipts(generate_jo
-00005580: 6273 3d54 7275 6529 0a0a 2020 2020 6465  bs=True)..    de
-00005590: 6620 7365 7475 705f 6469 7265 6374 6f72  f setup_director
-000055a0: 6965 7328 7365 6c66 293a 0a20 2020 2020  ies(self):.     
-000055b0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-000055c0: 7265 6174 6573 206e 6563 6573 7361 7279  reates necessary
-000055d0: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
-000055e0: 2053 6c75 726d 206f 7065 7261 7469 6f6e   Slurm operation
-000055f0: 732e 0a0a 2020 2020 2020 2020 5468 6973  s...        This
-00005600: 2066 756e 6374 696f 6e20 6372 6561 7465   function create
-00005610: 7320 6469 7265 6374 6f72 6965 7320 666f  s directories fo
-00005620: 7220 6461 7461 2073 746f 7261 6765 2c20  r data storage, 
-00005630: 7363 7269 7074 732c 2061 6e64 2077 6f72  scripts, and wor
-00005640: 6b66 6c6f 7773 0a20 2020 2020 2020 2061  kflows.        a
-00005650: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-00005660: 6865 2053 6c75 726d 436c 6965 6e74 206f  he SlurmClient o
-00005670: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
-00005680: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00005690: 2020 2020 5353 4845 7863 6570 7469 6f6e      SSHException
-000056a0: 3a20 4966 2074 6865 7265 2069 7320 616e  : If there is an
-000056b0: 2069 7373 7565 2065 7865 6375 7469 6e67   issue executing
-000056c0: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
-000056d0: 696f 6e20 636f 6d6d 616e 6473 2e0a 2020  ion commands..  
-000056e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000056f0: 2020 6469 725f 636d 6473 203d 205b 5d0a    dir_cmds = [].
-00005700: 2020 2020 2020 2020 2320 612e 2064 6174          # a. dat
-00005710: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
-00005720: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-00005730: 683a 0a20 2020 2020 2020 2020 2020 2064  h:.            d
-00005740: 6972 5f63 6d64 732e 6170 7065 6e64 2866  ir_cmds.append(f
-00005750: 226d 6b64 6972 202d 7020 7b73 656c 662e  "mkdir -p {self.
-00005760: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-00005770: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
-00005780: 2062 2e20 7363 7269 7074 730a 2020 2020   b. scripts.    
-00005790: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-000057a0: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
-000057b0: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
-000057c0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-000057d0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-000057e0: 6d5f 7363 7269 7074 5f70 6174 687d 2229  m_script_path}")
-000057f0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00005800: 2e20 776f 726b 666c 6f77 730a 2020 2020  . workflows.    
-00005810: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00005820: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
-00005830: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
-00005840: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-00005850: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-00005860: 6d5f 696d 6167 6573 5f70 6174 687d 2229  m_images_path}")
-00005870: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
-00005880: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
-00005890: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
-000058a0: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
-000058b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000058c0: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
-000058d0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-000058e0: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
-000058f0: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
-00005900: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
-00005910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005920: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
-00005930: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-00005940: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
-00005950: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-00005960: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
-00005970: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
-00005980: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
-00005990: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
-000059a0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-000059b0: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
-000059c0: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
-000059d0: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
-000059e0: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
-000059f0: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
-00005a00: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
-00005a10: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
-00005a20: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
-00005a30: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
-00005a40: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
-00005a50: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
-00005a60: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
-00005a70: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
-00005a80: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
-00005a90: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
-00005aa0: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
-00005ab0: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
-00005ac0: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
-00005ad0: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
-00005ae0: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
-00005af0: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
-00005b00: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
-00005b10: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
-00005b20: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
-00005b30: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
-00005b40: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00005b50: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
-00005b60: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
-00005b70: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
-00005b80: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
-00005b90: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
-00005ba0: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00005bb0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00005bc0: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
-00005bd0: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
-00005be0: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
-00005bf0: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
-00005c00: 2020 2020 2020 2020 2020 2020 696e 6974              init
-00005c10: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
-00005c20: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
-00005c30: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
-00005c40: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
-00005c50: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
-00005c60: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
-00005c70: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
-00005c80: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
-00005c90: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
-00005ca0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00005cb0: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
-00005cc0: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
-00005cd0: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00005ce0: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
-00005cf0: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
-00005d00: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
-00005d10: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
-00005d20: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
-00005d30: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
-00005d40: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
-00005d50: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
-00005d60: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
-00005d70: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
-00005d80: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
-00005d90: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
-00005da0: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
-00005db0: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
-00005dc0: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
-00005df0: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
-00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e10: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
-00005e20: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
-00005e30: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
-00005e40: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
-00005e50: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00005e60: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
-00005e70: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
-00005e80: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
-00005e90: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
-00005ea0: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
-00005eb0: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
-00005ec0: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
-00005ed0: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
-00005ee0: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
-00005ef0: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
-00005f00: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
-00005f10: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
-00005f20: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
-00005f30: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
-00005f40: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
-00005f50: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
-00005f60: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
-00005f70: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
-00005f80: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
-00005f90: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
-00005fa0: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
-00005fb0: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00005fc0: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-00005fd0: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
-00005fe0: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
-00005ff0: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
-00006000: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
-00006010: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-00006020: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-00006030: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
-00006040: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
-00006050: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
-00006060: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
-00006070: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
-00006080: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
-00006090: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
-000060a0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-000060b0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-000060c0: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
-000060d0: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
-000060e0: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
-000060f0: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
-00006100: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
-00006110: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
-00006120: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
-00006130: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
-00006140: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00006150: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
-00006160: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006170: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
-00006180: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00006190: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
-000061a0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-000061b0: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
-000061c0: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
-000061d0: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
-000061e0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-000061f0: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
-00006200: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
-00006210: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
-00006220: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
-00006230: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00006240: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
-00006250: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
-00006260: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00006270: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
-00006280: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
-00006290: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
-000062a0: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
-000062b0: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
-000062c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062d0: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
-000062e0: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
-000062f0: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
-00006300: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-00006310: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
-00006320: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
-00006330: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006340: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
-00006350: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
-00006360: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
-00006370: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00006380: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
-00006390: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
-000063a0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-000063b0: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
-000063c0: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
-000063d0: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
-000063e0: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
-000063f0: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
-00006400: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006410: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00006420: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
-00006430: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
-00006440: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
-00006470: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
-00006480: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
-00006490: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
-000064a0: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
-000064b0: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
-000064c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000064d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000064e0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-000064f0: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
-00006500: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00006510: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
-00006520: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-00006530: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
-00006540: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
-00006550: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
-00006560: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
-00006570: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
-00006580: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
-00006590: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
-000065a0: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
-000065b0: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
-000065c0: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
-000065d0: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
-000065e0: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
-000065f0: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
-00006600: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-00006610: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
-00006620: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-00006630: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
-00006640: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
-00006650: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
-00006660: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00006670: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
-000066a0: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
-000066b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066c0: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
-000066d0: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
-000066e0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-000066f0: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
-00006700: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
-00006710: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
-00006720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006730: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
-00006740: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
-00006750: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
-00006760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006770: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
-00006780: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
-00006790: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-000067a0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-000067b0: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
-000067c0: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000067e0: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
-000067f0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00006800: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-00006810: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
-00006820: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-00006850: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
-00006860: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
-00006870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006880: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00006890: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
-000068a0: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
-000068b0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-000068c0: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
-000068d0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-000068e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000068f0: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
-00006900: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
-00006910: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
-00006920: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-00006950: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+000032e0: 2020 706f 7274 2c0a 2020 2020 2020 2020    port,.        
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003310: 2020 636f 6e66 6967 2c0a 2020 2020 2020    config,.      
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003340: 2020 2020 6761 7465 7761 792c 0a20 2020      gateway,.   
+00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
+00003380: 6765 6e74 2c0a 2020 2020 2020 2020 2020  gent,.          
+00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 636f 6e6e 6563 745f 7469 6d65 6f75 742c  connect_timeout,
+000033c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033e0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+000033f0: 6374 5f6b 7761 7267 732c 0a20 2020 2020  ct_kwargs,.     
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003420: 2020 2020 2069 6e6c 696e 655f 7373 685f       inline_ssh_
+00003430: 656e 7629 0a20 2020 2020 2020 2073 656c  env).        sel
+00003440: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
+00003450: 6820 3d20 736c 7572 6d5f 6461 7461 5f70  h = slurm_data_p
+00003460: 6174 680a 2020 2020 2020 2020 7365 6c66  ath.        self
+00003470: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
+00003480: 7468 203d 2073 6c75 726d 5f69 6d61 6765  th = slurm_image
+00003490: 735f 7061 7468 0a20 2020 2020 2020 2073  s_path.        s
+000034a0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
+000034b0: 7465 7273 5f70 6174 6820 3d20 736c 7572  ters_path = slur
+000034c0: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
+000034d0: 680a 2020 2020 2020 2020 7365 6c66 2e73  h.        self.s
+000034e0: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+000034f0: 203d 2073 6c75 726d 5f6d 6f64 656c 5f70   = slurm_model_p
+00003500: 6174 6873 0a20 2020 2020 2020 2073 656c  aths.        sel
+00003510: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
+00003520: 6174 6820 3d20 736c 7572 6d5f 7363 7269  ath = slurm_scri
+00003530: 7074 5f70 6174 680a 2020 2020 2020 2020  pt_path.        
+00003540: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
+00003550: 745f 7265 706f 203d 2073 6c75 726d 5f73  t_repo = slurm_s
+00003560: 6372 6970 745f 7265 706f 0a20 2020 2020  cript_repo.     
+00003570: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
+00003580: 6465 6c5f 7265 706f 7320 3d20 736c 7572  del_repos = slur
+00003590: 6d5f 6d6f 6465 6c5f 7265 706f 730a 2020  m_model_repos.  
+000035a0: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
+000035b0: 5f6d 6f64 656c 5f69 6d61 6765 7320 3d20  _model_images = 
+000035c0: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
+000035d0: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+000035e0: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
+000035f0: 203d 2073 6c75 726d 5f6d 6f64 656c 5f6a   = slurm_model_j
+00003600: 6f62 730a 2020 2020 2020 2020 7365 6c66  obs.        self
+00003610: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
+00003620: 735f 7061 7261 6d73 203d 2073 6c75 726d  s_params = slurm
+00003630: 5f6d 6f64 656c 5f6a 6f62 735f 7061 7261  _model_jobs_para
+00003640: 6d73 0a0a 2020 2020 2020 2020 2320 496e  ms..        # In
+00003650: 6974 2063 6163 6865 2e20 4b65 6570 2072  it cache. Keep r
+00003660: 6573 706f 6e73 6573 2066 6f72 2033 3630  esponses for 360
+00003670: 2073 6563 6f6e 6473 0a20 2020 2020 2020   seconds.       
+00003680: 2073 656c 662e 6361 6368 6520 3d20 7265   self.cache = re
+00003690: 7175 6573 7473 5f63 6163 6865 2e62 6163  quests_cache.bac
+000036a0: 6b65 6e64 732e 7371 6c69 7465 2e53 514c  kends.sqlite.SQL
+000036b0: 6974 6543 6163 6865 280a 2020 2020 2020  iteCache(.      
+000036c0: 2020 2020 2020 6462 5f70 6174 683d 2267        db_path="g
+000036d0: 6974 6875 625f 6361 6368 6522 2c20 7573  ithub_cache", us
+000036e0: 655f 7465 6d70 3d54 7275 6529 0a20 2020  e_temp=True).   
+000036f0: 2020 2020 2073 656c 662e 6765 745f 6f72       self.get_or
+00003700: 5f63 7265 6174 655f 6769 7468 7562 5f73  _create_github_s
+00003710: 6573 7369 6f6e 2829 0a0a 2020 2020 2020  ession()..      
+00003720: 2020 7365 6c66 2e69 6e69 745f 776f 726b    self.init_work
+00003730: 666c 6f77 7328 290a 2020 2020 2020 2020  flows().        
+00003740: 7365 6c66 2e76 616c 6964 6174 6528 7661  self.validate(va
+00003750: 6c69 6461 7465 5f73 6c75 726d 5f73 6574  lidate_slurm_set
+00003760: 7570 3d69 6e69 745f 736c 7572 6d29 0a0a  up=init_slurm)..
+00003770: 2020 2020 6465 6620 696e 6974 5f77 6f72      def init_wor
+00003780: 6b66 6c6f 7773 2873 656c 662c 2066 6f72  kflows(self, for
+00003790: 6365 5f75 7064 6174 653a 2062 6f6f 6c20  ce_update: bool 
+000037a0: 3d20 4661 6c73 6529 3a0a 2020 2020 2020  = False):.      
+000037b0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+000037c0: 7472 6965 7665 7320 7468 6520 7265 7175  trieves the requ
+000037d0: 6972 6564 2069 6e66 6f20 666f 7220 7468  ired info for th
+000037e0: 6520 636f 6e66 6967 7572 6564 2077 6f72  e configured wor
+000037f0: 6b66 6c6f 7773 2066 726f 6d20 6769 7468  kflows from gith
+00003800: 7562 2e0a 2020 2020 2020 2020 4974 2077  ub..        It w
+00003810: 696c 6c20 6669 6c6c 2060 736c 7572 6d5f  ill fill `slurm_
+00003820: 6d6f 6465 6c5f 696d 6167 6573 6020 7769  model_images` wi
+00003830: 7468 2064 6f63 6b65 7268 7562 206c 696e  th dockerhub lin
+00003840: 6b73 2e0a 0a20 2020 2020 2020 2041 7267  ks...        Arg
+00003850: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00003860: 6f72 6365 5f75 7064 6174 6520 2862 6f6f  orce_update (boo
+00003870: 6c29 3a20 5769 6c6c 206f 7665 7277 7269  l): Will overwri
+00003880: 7465 2061 6c72 6561 6479 2067 6976 656e  te already given
+00003890: 2070 6174 6873 0a20 2020 2020 2020 2020   paths.         
+000038a0: 2020 2020 2020 2069 6e20 6073 6c75 726d         in `slurm
+000038b0: 5f6d 6f64 656c 5f69 6d61 6765 7360 0a0a  _model_images`..
+000038c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000038d0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+000038e0: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
+000038f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00003900: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00003910: 5f69 6d61 6765 7320 3d20 7b7d 0a20 2020  _images = {}.   
+00003920: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00003930: 2e73 6c75 726d 5f6d 6f64 656c 5f72 6570  .slurm_model_rep
+00003940: 6f73 3a0a 2020 2020 2020 2020 2020 2020  os:.            
+00003950: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00003960: 4e6f 2077 6f72 6b66 6c6f 7773 2063 6f6e  No workflows con
+00003970: 6669 6775 7265 6421 2229 0a20 2020 2020  figured!").     
+00003980: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
+00003990: 6d5f 6d6f 6465 6c5f 7265 706f 7320 3d20  m_model_repos = 
+000039a0: 7b7d 0a20 2020 2020 2020 2020 2020 2023  {}.            #
+000039b0: 2073 6b69 7073 2074 6865 2073 6574 7570   skips the setup
+000039c0: 0a20 2020 2020 2020 2066 6f72 2077 6f72  .        for wor
+000039d0: 6b66 6c6f 7720 696e 2073 656c 662e 736c  kflow in self.sl
+000039e0: 7572 6d5f 6d6f 6465 6c5f 7265 706f 732e  urm_model_repos.
+000039f0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+00003a00: 2020 2020 6966 2077 6f72 6b66 6c6f 7720      if workflow 
+00003a10: 6e6f 7420 696e 2073 656c 662e 736c 7572  not in self.slur
+00003a20: 6d5f 6d6f 6465 6c5f 696d 6167 6573 206f  m_model_images o
+00003a30: 7220 666f 7263 655f 7570 6461 7465 3a0a  r force_update:.
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
+00003a60: 3d20 7365 6c66 2e70 756c 6c5f 6465 7363  = self.pull_desc
+00003a70: 7269 7074 6f72 5f66 726f 6d5f 6769 7468  riptor_from_gith
+00003a80: 7562 2877 6f72 6b66 6c6f 7729 0a20 2020  ub(workflow).   
+00003a90: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00003aa0: 6765 722e 6465 6275 6728 2725 733a 2025  ger.debug('%s: %
+00003ab0: 7327 2c20 776f 726b 666c 6f77 2c20 6a73  s', workflow, js
+00003ac0: 6f6e 5f64 6573 6372 6970 746f 7229 0a20  on_descriptor). 
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003ae0: 6d61 6765 203d 206a 736f 6e5f 6465 7363  mage = json_desc
+00003af0: 7269 7074 6f72 5b27 636f 6e74 6169 6e65  riptor['containe
+00003b00: 722d 696d 6167 6527 5d5b 2769 6d61 6765  r-image']['image
+00003b10: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+00003b20: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
+00003b30: 6465 6c5f 696d 6167 6573 5b77 6f72 6b66  del_images[workf
+00003b40: 6c6f 775d 203d 2069 6d61 6765 0a0a 2020  low] = image..  
+00003b50: 2020 6465 6620 7365 7475 705f 736c 7572    def setup_slur
+00003b60: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
+00003b70: 2022 2222 0a20 2020 2020 2020 2056 616c   """.        Val
+00003b80: 6964 6174 6573 206f 7220 6372 6561 7465  idates or create
+00003b90: 7320 7468 6520 7265 7175 6972 6564 2073  s the required s
+00003ba0: 6574 7570 206f 6e20 7468 6520 536c 7572  etup on the Slur
+00003bb0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
+00003bc0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00003bd0: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
+00003be0: 7469 6f6e 3a20 6966 2069 7420 6361 6e6e  tion: if it cann
+00003bf0: 6f74 2063 6f6e 6e65 6374 2074 6f20 536c  ot connect to Sl
+00003c00: 7572 6d2c 206f 7220 7275 6e73 2069 6e74  urm, or runs int
+00003c10: 6f20 616e 2065 7272 6f72 0a20 2020 2020  o an error.     
+00003c20: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00003c30: 6620 7365 6c66 2e76 616c 6964 6174 6528  f self.validate(
+00003c40: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+00003c50: 2031 2e20 4372 6561 7465 2064 6972 6563   1. Create direc
+00003c60: 746f 7269 6573 0a20 2020 2020 2020 2020  tories.         
+00003c70: 2020 2073 656c 662e 7365 7475 705f 6469     self.setup_di
+00003c80: 7265 6374 6f72 6965 7328 290a 0a20 2020  rectories()..   
+00003c90: 2020 2020 2020 2020 2023 2032 2e20 436c           # 2. Cl
+00003ca0: 6f6e 6520 6769 740a 2020 2020 2020 2020  one git.        
+00003cb0: 2020 2020 7365 6c66 2e73 6574 7570 5f6a      self.setup_j
+00003cc0: 6f62 5f73 6372 6970 7473 2829 0a0a 2020  ob_scripts()..  
+00003cd0: 2020 2020 2020 2020 2020 2320 332e 2053            # 3. S
+00003ce0: 6574 7570 2063 6f6e 7665 7274 6572 730a  etup converters.
+00003cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003d00: 2e73 6574 7570 5f63 6f6e 7665 7274 6572  .setup_converter
+00003d10: 7328 290a 0a20 2020 2020 2020 2020 2020  s()..           
+00003d20: 2023 2034 2e20 446f 776e 6c6f 6164 2077   # 4. Download w
+00003d30: 6f72 6b66 6c6f 7720 696d 6167 6573 0a20  orkflow images. 
+00003d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003d50: 7365 7475 705f 636f 6e74 6169 6e65 725f  setup_container_
+00003d60: 696d 6167 6573 2829 0a0a 2020 2020 2020  images()..      
+00003d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003d80: 2020 2020 7261 6973 6520 5353 4845 7863      raise SSHExc
+00003d90: 6570 7469 6f6e 2822 4661 696c 7572 6520  eption("Failure 
+00003da0: 696e 2063 6f6e 6e65 6374 696e 6720 746f  in connecting to
+00003db0: 2053 6c75 726d 2063 6c75 7374 6572 2229   Slurm cluster")
+00003dc0: 0a0a 2020 2020 6465 6620 7365 7475 705f  ..    def setup_
+00003dd0: 636f 6e74 6169 6e65 725f 696d 6167 6573  container_images
+00003de0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003df0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
+00003e00: 2075 7020 636f 6e74 6169 6e65 7220 696d   up container im
+00003e10: 6167 6573 2066 6f72 2053 6c75 726d 206f  ages for Slurm o
+00003e20: 7065 7261 7469 6f6e 732e 0a0a 2020 2020  perations...    
+00003e30: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00003e40: 6e20 6372 6561 7465 7320 7370 6563 6966  n creates specif
+00003e50: 6963 2064 6972 6563 746f 7269 6573 2066  ic directories f
+00003e60: 6f72 2063 6f6e 7461 696e 6572 2069 6d61  or container ima
+00003e70: 6765 7320 616e 6420 7075 6c6c 730a 2020  ges and pulls.  
+00003e80: 2020 2020 2020 6e65 6365 7373 6172 7920        necessary 
+00003e90: 696d 6167 6573 2066 726f 6d20 446f 636b  images from Dock
+00003ea0: 6572 2072 6570 6f73 6974 6f72 6965 732e  er repositories.
+00003eb0: 2049 7420 6765 6e65 7261 7465 7320 616e   It generates an
+00003ec0: 6420 6578 6563 7574 6573 0a20 2020 2020  d executes.     
+00003ed0: 2020 2061 2073 6372 6970 7420 746f 2070     a script to p
+00003ee0: 756c 6c20 696d 6167 6573 2061 6e64 2063  ull images and c
+00003ef0: 6f70 6965 7320 6974 2074 6f20 7468 6520  opies it to the 
+00003f00: 7265 6d6f 7465 206c 6f63 6174 696f 6e2e  remote location.
+00003f10: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00003f20: 3a0a 2020 2020 2020 2020 2020 2020 5353  :.            SS
+00003f30: 4845 7863 6570 7469 6f6e 3a20 4966 2074  HException: If t
+00003f40: 6865 7265 2069 7320 616e 2069 7373 7565  here is an issue
+00003f50: 2065 7865 6375 7469 6e67 2063 6f6d 6d61   executing comma
+00003f60: 6e64 7320 6f72 2063 6f70 7969 6e67 2066  nds or copying f
+00003f70: 696c 6573 2e0a 2020 2020 2020 2020 2222  iles..        ""
+00003f80: 220a 2020 2020 2020 2020 2320 4372 6561  ".        # Crea
+00003f90: 7465 2073 7065 6369 6669 6320 776f 726b  te specific work
+00003fa0: 666c 6f77 2064 6972 730a 2020 2020 2020  flow dirs.      
+00003fb0: 2020 7769 7468 2073 656c 662e 6364 2873    with self.cd(s
+00003fc0: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
+00003fd0: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
+00003fe0: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00003ff0: 6d5f 6d6f 6465 6c5f 7061 7468 733a 0a20  m_model_paths:. 
+00004000: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00004010: 6f64 656c 7061 7468 7320 3d20 2220 222e  odelpaths = " ".
+00004020: 6a6f 696e 2873 656c 662e 736c 7572 6d5f  join(self.slurm_
+00004030: 6d6f 6465 6c5f 7061 7468 732e 7661 6c75  model_paths.valu
+00004040: 6573 2829 290a 2020 2020 2020 2020 2020  es()).          
+00004050: 2020 2020 2020 2320 6d6b 6469 7220 6365        # mkdir ce
+00004060: 6c6c 7072 6f66 696c 6572 2069 6d61 6765  llprofiler image
+00004070: 6a20 2e2e 2e0a 2020 2020 2020 2020 2020  j ....          
+00004080: 2020 2020 2020 7220 3d20 7365 6c66 2e72        r = self.r
+00004090: 756e 5f63 6f6d 6d61 6e64 7328 5b66 226d  un_commands([f"m
+000040a0: 6b64 6972 202d 7020 7b6d 6f64 656c 7061  kdir -p {modelpa
+000040b0: 7468 737d 225d 290a 2020 2020 2020 2020  ths}"]).        
+000040c0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+000040d0: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
+000040e0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+000040f0: 5348 4578 6365 7074 696f 6e28 7229 0a0a  SHException(r)..
+00004100: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004110: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+00004120: 696d 6167 6573 3a0a 2020 2020 2020 2020  images:.        
+00004130: 2020 2020 2020 2020 7075 6c6c 5f63 6f6d          pull_com
+00004140: 6d61 6e64 7320 3d20 5b5d 0a20 2020 2020  mands = [].     
+00004150: 2020 2020 2020 2020 2020 2066 6f72 2077             for w
+00004160: 662c 2069 6d61 6765 2069 6e20 7365 6c66  f, image in self
+00004170: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
+00004180: 6765 732e 6974 656d 7328 293a 0a20 2020  ges.items():.   
+00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041a0: 2072 6570 6f20 3d20 7365 6c66 2e73 6c75   repo = self.slu
+000041b0: 726d 5f6d 6f64 656c 5f72 6570 6f73 5b77  rm_model_repos[w
+000041c0: 665d 0a20 2020 2020 2020 2020 2020 2020  f].             
+000041d0: 2020 2020 2020 2070 6174 6820 3d20 7365         path = se
+000041e0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
+000041f0: 6174 6873 5b77 665d 0a20 2020 2020 2020  aths[wf].       
+00004200: 2020 2020 2020 2020 2020 2020 205f 2c20               _, 
+00004210: 7665 7273 696f 6e20 3d20 7365 6c66 2e65  version = self.e
+00004220: 7874 7261 6374 5f70 6172 7473 5f66 726f  xtract_parts_fro
+00004230: 6d5f 7572 6c28 7265 706f 290a 2020 2020  m_url(repo).    
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 6966 2076 6572 7369 6f6e 203d 3d20 226d  if version == "m
+00004260: 6173 7465 7222 3a0a 2020 2020 2020 2020  aster":.        
+00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004280: 7665 7273 696f 6e20 3d20 226c 6174 6573  version = "lates
+00004290: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
+000042a0: 2020 2020 2020 2070 756c 6c5f 7465 6d70         pull_temp
+000042b0: 6c61 7465 203d 2022 6563 686f 2027 7374  late = "echo 'st
+000042c0: 6172 7469 6e67 2024 7061 7468 2024 7665  arting $path $ve
+000042d0: 7273 696f 6e27 203e 3e20 7369 6e67 2e6c  rsion' >> sing.l
+000042e0: 6f67 5c6e 6e6f 6875 7020 7368 202d 6320  og\nnohup sh -c 
+000042f0: 5c22 7369 6e67 756c 6172 6974 7920 7075  \"singularity pu
+00004300: 6c6c 202d 2d64 6973 6162 6c65 2d63 6163  ll --disable-cac
+00004310: 6865 202d 2d64 6972 2024 7061 7468 2064  he --dir $path d
+00004320: 6f63 6b65 723a 2f2f 2469 6d61 6765 3a24  ocker://$image:$
+00004330: 7665 7273 696f 6e3b 2065 6368 6f20 2766  version; echo 'f
+00004340: 696e 6973 6865 6420 2470 6174 6820 2476  inished $path $v
+00004350: 6572 7369 6f6e 275c 2220 3e3e 2073 696e  ersion'\" >> sin
+00004360: 672e 6c6f 6720 323e 2631 2026 2064 6973  g.log 2>&1 & dis
+00004370: 6f77 6e22 0a20 2020 2020 2020 2020 2020  own".           
+00004380: 2020 2020 2020 2020 2074 203d 2054 656d           t = Tem
+00004390: 706c 6174 6528 7075 6c6c 5f74 656d 706c  plate(pull_templ
+000043a0: 6174 6529 0a20 2020 2020 2020 2020 2020  ate).           
+000043b0: 2020 2020 2020 2020 2073 7562 7374 6974           substit
+000043c0: 7574 6573 203d 207b 7d0a 2020 2020 2020  utes = {}.      
+000043d0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+000043e0: 6273 7469 7475 7465 735b 2770 6174 6827  bstitutes['path'
+000043f0: 5d20 3d20 7061 7468 0a20 2020 2020 2020  ] = path.       
+00004400: 2020 2020 2020 2020 2020 2020 2073 7562               sub
+00004410: 7374 6974 7574 6573 5b27 696d 6167 6527  stitutes['image'
+00004420: 5d20 3d20 696d 6167 650a 2020 2020 2020  ] = image.      
+00004430: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00004440: 6273 7469 7475 7465 735b 2776 6572 7369  bstitutes['versi
+00004450: 6f6e 275d 203d 2076 6572 7369 6f6e 0a20  on'] = version. 
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2063 6d64 203d 2074 2e73 6166 655f     cmd = t.safe_
+00004480: 7375 6273 7469 7475 7465 2873 7562 7374  substitute(subst
+00004490: 6974 7574 6573 290a 2020 2020 2020 2020  itutes).        
+000044a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000044b0: 6572 2e64 6562 7567 2866 2273 7562 7374  er.debug(f"subst
+000044c0: 6974 7574 6564 3a20 7b63 6d64 7d22 290a  ituted: {cmd}").
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 2020 2020 7075 6c6c 5f63 6f6d 6d61 6e64      pull_command
+000044f0: 732e 6170 7065 6e64 2863 6d64 290a 2020  s.append(cmd).  
+00004500: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00004510: 7269 7074 5f6e 616d 6520 3d20 2270 756c  ript_name = "pul
+00004520: 6c5f 696d 6167 6573 2e73 6822 0a20 2020  l_images.sh".   
+00004530: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+00004540: 706c 6174 655f 7363 7269 7074 203d 2066  plate_script = f
+00004550: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
+00004560: 292e 6a6f 696e 7061 7468 2873 6372 6970  ).joinpath(scrip
+00004570: 745f 6e61 6d65 290a 2020 2020 2020 2020  t_name).        
+00004580: 2020 2020 2020 2020 7769 7468 2074 656d          with tem
+00004590: 706c 6174 655f 7363 7269 7074 2e6f 7065  plate_script.ope
+000045a0: 6e28 2772 2729 2061 7320 663a 0a20 2020  n('r') as f:.   
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 2073 7263 203d 2054 656d 706c 6174 6528   src = Template(
+000045d0: 662e 7265 6164 2829 290a 2020 2020 2020  f.read()).      
+000045e0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+000045f0: 6273 7469 7475 7465 203d 207b 2770 756c  bstitute = {'pul
+00004600: 6c63 6f6d 6d61 6e64 7327 3a20 225c 6e22  lcommands': "\n"
+00004610: 2e6a 6f69 6e28 7075 6c6c 5f63 6f6d 6d61  .join(pull_comma
+00004620: 6e64 7329 7d0a 2020 2020 2020 2020 2020  nds)}.          
+00004630: 2020 2020 2020 2020 2020 6a6f 625f 7363            job_sc
+00004640: 7269 7074 203d 2073 7263 2e73 6166 655f  ript = src.safe_
+00004650: 7375 6273 7469 7475 7465 2873 7562 7374  substitute(subst
+00004660: 6974 7574 6529 0a20 2020 2020 2020 2020  itute).         
+00004670: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00004680: 6275 6728 6622 7375 6273 7469 7475 7465  bug(f"substitute
+00004690: 643a 5c6e 207b 6a6f 625f 7363 7269 7074  d:\n {job_script
+000046a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000046b0: 2020 2020 2320 636f 7079 2074 6f20 7265      # copy to re
+000046c0: 6d6f 7465 2066 696c 650a 2020 2020 2020  mote file.      
+000046d0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
+000046e0: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
+000046f0: 5f69 6d61 6765 735f 7061 7468 2b22 2f22  _images_path+"/"
+00004700: 2b73 6372 6970 745f 6e61 6d65 0a20 2020  +script_name.   
+00004710: 2020 2020 2020 2020 2020 2020 205f 203d               _ =
+00004720: 2073 656c 662e 7075 7428 6c6f 6361 6c3d   self.put(local=
+00004730: 696f 2e53 7472 696e 6749 4f28 6a6f 625f  io.StringIO(job_
+00004740: 7363 7269 7074 292c 0a20 2020 2020 2020  script),.       
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 2020 2020 7265 6d6f 7465 3d66 756c        remote=ful
+00004770: 6c5f 7061 7468 290a 2020 2020 2020 2020  l_path).        
+00004780: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
+00004790: 7469 6d65 2073 6820 7b73 6372 6970 745f  time sh {script_
+000047a0: 6e61 6d65 7d22 0a20 2020 2020 2020 2020  name}".         
+000047b0: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
+000047c0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+000047d0: 645d 290a 2020 2020 2020 2020 2020 2020  d]).            
+000047e0: 2020 2020 6966 206e 6f74 2072 2e6f 6b3a      if not r.ok:
+000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004800: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00004810: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
+00004820: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00004830: 722e 696e 666f 2872 2e73 7464 6f75 7429  r.info(r.stdout)
+00004840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004850: 206c 6f67 6765 722e 696e 666f 2822 496e   logger.info("In
+00004860: 6974 6961 7465 6420 646f 776e 6c6f 6164  itiated download
+00004870: 696e 6720 616e 6420 6275 696c 6469 6e67  ing and building
+00004880: 2220 2b0a 2020 2020 2020 2020 2020 2020  " +.            
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2220 636f 6e74 6169 6e65 7220 696d 6167  " container imag
+000048b0: 6573 206f 6e20 536c 7572 6d2e 2220 2b0a  es on Slurm." +.
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 2020 2020 2020 2020 2220 5468              " Th
+000048e0: 6973 2077 696c 6c20 7461 6b65 2061 2077  is will take a w
+000048f0: 6869 6c65 2069 6e20 7468 6520 6261 636b  hile in the back
+00004900: 6772 6f75 6e64 2e22 202b 200a 2020 2020  ground." + .    
+00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 2020 2020 2020 2020 2220 4368 6563 6b20          " Check 
+00004930: 2773 696e 672e 6c6f 6727 206f 6e20 536c  'sing.log' on Sl
+00004940: 7572 6d20 666f 7220 7072 6f67 7265 7373  urm for progress
+00004950: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00004960: 2020 2020 2320 2320 636c 6561 6e75 7020      # # cleanup 
+00004970: 6769 616e 7420 7369 6e67 756c 6172 6974  giant singularit
+00004980: 7920 6361 6368 6521 0a20 2020 2020 2020  y cache!.       
+00004990: 2020 2020 2020 2020 2023 2075 7369 6e67           # using
+000049a0: 202d 2d64 6973 6162 6c65 2d63 6163 6865   --disable-cache
+000049b0: 2062 6563 6175 7365 2077 6520 7275 6e20   because we run 
+000049c0: 696e 2074 6865 2062 6163 6b67 726f 756e  in the backgroun
+000049d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000049e0: 2020 2320 636d 6420 3d20 2273 696e 6775    # cmd = "singu
+000049f0: 6c61 7269 7479 2063 6163 6865 2063 6c65  larity cache cle
+00004a00: 616e 202d 6622 0a20 2020 2020 2020 2020  an -f".         
+00004a10: 2020 2020 2020 2023 2072 203d 2073 656c         # r = sel
+00004a20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
+00004a30: 636d 645d 290a 0a20 2020 2064 6566 2073  cmd])..    def s
+00004a40: 6574 7570 5f63 6f6e 7665 7274 6572 7328  etup_converters(
+00004a50: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00004a60: 2222 0a20 2020 2020 2020 2053 6574 7320  "".        Sets 
+00004a70: 7570 2063 6f6e 7665 7274 6572 7320 666f  up converters fo
+00004a80: 7220 536c 7572 6d20 6f70 6572 6174 696f  r Slurm operatio
+00004a90: 6e73 2e0a 0a20 2020 2020 2020 2054 6869  ns...        Thi
+00004aa0: 7320 6675 6e63 7469 6f6e 2063 7265 6174  s function creat
+00004ab0: 6573 206e 6563 6573 7361 7279 2064 6972  es necessary dir
+00004ac0: 6563 746f 7269 6573 2066 6f72 2063 6f6e  ectories for con
+00004ad0: 7665 7274 6572 7320 616e 6420 636f 7069  verters and copi
+00004ae0: 6573 0a20 2020 2020 2020 2063 6f6e 7665  es.        conve
+00004af0: 7274 6572 2073 6372 6970 7473 2061 6e64  rter scripts and
+00004b00: 2064 6566 696e 6974 696f 6e73 2074 6f20   definitions to 
+00004b10: 7468 6520 6170 7072 6f70 7269 6174 6520  the appropriate 
+00004b20: 6c6f 6361 7469 6f6e 732e 2049 7420 616c  locations. It al
+00004b30: 736f 0a20 2020 2020 2020 2062 7569 6c64  so.        build
+00004b40: 7320 5369 6e67 756c 6172 6974 7920 636f  s Singularity co
+00004b50: 6e74 6169 6e65 7273 2066 726f 6d20 7468  ntainers from th
+00004b60: 6520 7072 6f76 6964 6564 2064 6566 696e  e provided defin
+00004b70: 6974 696f 6e73 2e0a 0a20 2020 2020 2020  itions...       
+00004b80: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00004b90: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
+00004ba0: 6e3a 2049 6620 7468 6572 6520 6973 2061  n: If there is a
+00004bb0: 6e20 6973 7375 6520 6578 6563 7574 696e  n issue executin
+00004bc0: 6720 636f 6d6d 616e 6473 206f 7220 636f  g commands or co
+00004bd0: 7079 696e 6720 6669 6c65 732e 0a20 2020  pying files..   
+00004be0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004bf0: 2063 6f6e 7665 7274 5f63 6d64 7320 3d20   convert_cmds = 
+00004c00: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
+00004c10: 6c66 2e73 6c75 726d 5f63 6f6e 7665 7274  lf.slurm_convert
+00004c20: 6572 735f 7061 7468 3a0a 2020 2020 2020  ers_path:.      
+00004c30: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
+00004c40: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
+00004c50: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
+00004c60: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
+00004c70: 7d22 290a 2020 2020 2020 2020 7220 3d20  }").        r = 
+00004c80: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+00004c90: 7328 636f 6e76 6572 745f 636d 6473 290a  s(convert_cmds).
+00004ca0: 2020 2020 2020 2020 2320 636f 7079 2067          # copy g
+00004cb0: 656e 6572 6963 206a 6f62 2061 7272 6179  eneric job array
+00004cc0: 2073 6372 6970 7420 6f76 6572 2074 6f20   script over to 
+00004cd0: 736c 7572 6d0a 2020 2020 2020 2020 636f  slurm.        co
+00004ce0: 6e76 6572 745f 6a6f 625f 6c6f 6361 6c20  nvert_job_local 
+00004cf0: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
+00004d00: 6573 2229 2e6a 6f69 6e70 6174 6828 0a20  es").joinpath(. 
+00004d10: 2020 2020 2020 2020 2020 2022 636f 6e76             "conv
+00004d20: 6572 745f 6a6f 625f 6172 7261 792e 7368  ert_job_array.sh
+00004d30: 2229 0a20 2020 2020 2020 205f 203d 2073  ").        _ = s
+00004d40: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
+00004d50: 6e76 6572 745f 6a6f 625f 6c6f 6361 6c2c  nvert_job_local,
+00004d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d70: 2020 2020 2020 7265 6d6f 7465 3d73 656c        remote=sel
+00004d80: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
+00004d90: 6174 6829 0a20 2020 2020 2020 2023 2063  ath).        # c
+00004da0: 7572 7265 6e74 6c79 206b 6e6f 776e 2063  urrently known c
+00004db0: 6f6e 7665 7274 6572 730a 2020 2020 2020  onverters.      
+00004dc0: 2020 2320 3361 2e20 5a41 5252 2074 6f20    # 3a. ZARR to 
+00004dd0: 5449 4646 0a20 2020 2020 2020 2023 2054  TIFF.        # T
+00004de0: 4f44 4f20 6578 7472 6163 7420 7468 6573  ODO extract thes
+00004df0: 6520 7661 6c75 6573 2074 6f20 652e 672e  e values to e.g.
+00004e00: 2063 6f6e 6669 6720 6966 2077 6520 6861   config if we ha
+00004e10: 7665 206d 6f72 650a 2020 2020 2020 2020  ve more.        
+00004e20: 636f 6e76 6572 745f 6e61 6d65 203d 2022  convert_name = "
+00004e30: 636f 6e76 6572 745f 7a61 7272 5f74 6f5f  convert_zarr_to_
+00004e40: 7469 6666 220a 2020 2020 2020 2020 636f  tiff".        co
+00004e50: 6e76 6572 745f 7079 203d 2066 227b 636f  nvert_py = f"{co
+00004e60: 6e76 6572 745f 6e61 6d65 7d2e 7079 220a  nvert_name}.py".
+00004e70: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+00004e80: 7363 7269 7074 5f6c 6f63 616c 203d 2066  script_local = f
+00004e90: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
+00004ea0: 292e 6a6f 696e 7061 7468 280a 2020 2020  ).joinpath(.    
+00004eb0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+00004ec0: 7079 290a 2020 2020 2020 2020 636f 6e76  py).        conv
+00004ed0: 6572 745f 6465 6620 3d20 6622 7b63 6f6e  ert_def = f"{con
+00004ee0: 7665 7274 5f6e 616d 657d 2e64 6566 220a  vert_name}.def".
+00004ef0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+00004f00: 6465 665f 6c6f 6361 6c20 3d20 6669 6c65  def_local = file
+00004f10: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
+00004f20: 6f69 6e70 6174 6828 0a20 2020 2020 2020  oinpath(.       
+00004f30: 2020 2020 2063 6f6e 7665 7274 5f64 6566       convert_def
+00004f40: 290a 2020 2020 2020 2020 5f20 3d20 7365  ).        _ = se
+00004f50: 6c66 2e70 7574 286c 6f63 616c 3d63 6f6e  lf.put(local=con
+00004f60: 7665 7274 5f73 6372 6970 745f 6c6f 6361  vert_script_loca
+00004f70: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00004f80: 2020 2020 2020 2020 7265 6d6f 7465 3d73          remote=s
+00004f90: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
+00004fa0: 7465 7273 5f70 6174 6829 0a20 2020 2020  ters_path).     
+00004fb0: 2020 205f 203d 2073 656c 662e 7075 7428     _ = self.put(
+00004fc0: 6c6f 6361 6c3d 636f 6e76 6572 745f 6465  local=convert_de
+00004fd0: 665f 6c6f 6361 6c2c 0a20 2020 2020 2020  f_local,.       
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004ff0: 6d6f 7465 3d73 656c 662e 736c 7572 6d5f  mote=self.slurm_
+00005000: 636f 6e76 6572 7465 7273 5f70 6174 6829  converters_path)
+00005010: 0a20 2020 2020 2020 2023 2042 7569 6c64  .        # Build
+00005020: 2073 696e 6775 6c61 7269 7479 2063 6f6e   singularity con
+00005030: 7461 696e 6572 2066 726f 6d20 6465 6669  tainer from defi
+00005040: 6e69 7469 6f6e 0a20 2020 2020 2020 2077  nition.        w
+00005050: 6974 6820 7365 6c66 2e63 6428 7365 6c66  ith self.cd(self
+00005060: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
+00005070: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
+00005080: 2020 2020 2063 6f6e 7665 7274 5f63 6d64       convert_cmd
+00005090: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
+000050a0: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
+000050b0: 5f69 6d61 6765 735f 7061 7468 3a0a 2020  _images_path:.  
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000050d0: 544f 444f 2043 6861 6e67 6520 7468 6520  TODO Change the 
+000050e0: 746d 7020 6469 723f 0a20 2020 2020 2020  tmp dir?.       
+000050f0: 2020 2020 2020 2020 2023 2065 7870 6f72           # expor
+00005100: 7420 5349 4e47 554c 4152 4954 595f 544d  t SINGULARITY_TM
+00005110: 5044 4952 3d7e 2f6d 792d 7363 7261 7463  PDIR=~/my-scratc
+00005120: 682f 746d 703b 0a20 2020 2020 2020 2020  h/tmp;.         
+00005130: 2020 2020 2020 2023 206f 6e6c 7920 6966         # only if
+00005140: 2066 696c 6520 646f 6573 206e 6f74 2065   file does not e
+00005150: 7869 7374 2079 6574 0a20 2020 2020 2020  xist yet.       
+00005160: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
+00005170: 7274 5f63 6d64 732e 6170 7065 6e64 2866  rt_cmds.append(f
+00005180: 225b 2021 202d 6620 7b63 6f6e 7665 7274  "[ ! -f {convert
+00005190: 5f6e 616d 657d 2e73 6966 205d 2229 0a20  _name}.sif ]"). 
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000051b0: 2045 4449 5420 2d2d 204e 4f2c 2074 6865   EDIT -- NO, the
+000051c0: 6e20 7765 2063 616e 2774 2075 7064 6174  n we can't updat
+000051d0: 6521 2046 6f72 6365 2072 6562 7569 6c64  e! Force rebuild
+000051e0: 210a 2020 2020 2020 2020 2020 2020 2020  !.              
+000051f0: 2020 2320 646f 776e 6c6f 6164 202f 6275    # download /bu
+00005200: 696c 6420 6e65 7720 636f 6e74 6169 6e65  ild new containe
+00005210: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00005220: 2020 636f 6e76 6572 745f 636d 6473 2e61    convert_cmds.a
+00005230: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+00005240: 2020 2020 2020 2020 2020 2066 2273 696e             f"sin
+00005250: 6775 6c61 7269 7479 2062 7569 6c64 202d  gularity build -
+00005260: 4620 7b63 6f6e 7665 7274 5f6e 616d 657d  F {convert_name}
+00005270: 2e73 6966 207b 636f 6e76 6572 745f 6465  .sif {convert_de
+00005280: 667d 203e 3e20 7369 6e67 2e6c 6f67 2032  f} >> sing.log 2
+00005290: 3e26 3120 3b20 6563 686f 2027 6669 6e69  >&1 ; echo 'fini
+000052a0: 7368 6564 207b 636f 6e76 6572 745f 6e61  shed {convert_na
+000052b0: 6d65 7d2e 7369 6627 2026 2229 0a20 2020  me}.sif' &").   
+000052c0: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
+000052d0: 662e 7275 6e5f 636f 6d6d 616e 6473 2863  f.run_commands(c
+000052e0: 6f6e 7665 7274 5f63 6d64 7329 0a0a 2020  onvert_cmds)..  
+000052f0: 2020 6465 6620 7365 7475 705f 6a6f 625f    def setup_job_
+00005300: 7363 7269 7074 7328 7365 6c66 293a 0a20  scripts(self):. 
+00005310: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005320: 2020 2053 6574 7320 7570 206a 6f62 2073     Sets up job s
+00005330: 6372 6970 7473 2066 6f72 2053 6c75 726d  cripts for Slurm
+00005340: 206f 7065 7261 7469 6f6e 732e 0a0a 2020   operations...  
+00005350: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+00005360: 696f 6e20 6569 7468 6572 2063 6c6f 6e65  ion either clone
+00005370: 7320 6120 4769 7420 7265 706f 7369 746f  s a Git reposito
+00005380: 7279 2063 6f6e 7461 696e 696e 6720 6a6f  ry containing jo
+00005390: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
+000053a0: 2020 696e 746f 2074 6865 2073 7065 6369    into the speci
+000053b0: 6669 6564 2073 6372 6970 7420 7061 7468  fied script path
+000053c0: 206f 7220 6765 6e65 7261 7465 7320 7363   or generates sc
+000053d0: 7269 7074 7320 6c6f 6361 6c6c 7920 6966  ripts locally if
+000053e0: 206e 6f20 7265 706f 7369 746f 7279 0a20   no repository. 
+000053f0: 2020 2020 2020 2069 7320 7072 6f76 6964         is provid
+00005400: 6564 2e0a 0a20 2020 2020 2020 2052 6169  ed...        Rai
+00005410: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00005420: 2053 5348 4578 6365 7074 696f 6e3a 2049   SSHException: I
+00005430: 6620 7468 6572 6520 6973 2061 6e20 6973  f there is an is
+00005440: 7375 6520 6578 6563 7574 696e 6720 4769  sue executing Gi
+00005450: 7420 636f 6d6d 616e 6473 206f 7220 6765  t commands or ge
+00005460: 6e65 7261 7469 6e67 2073 6372 6970 7473  nerating scripts
+00005470: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00005480: 2020 2020 2020 6966 2073 656c 662e 736c        if self.sl
+00005490: 7572 6d5f 7363 7269 7074 5f72 6570 6f20  urm_script_repo 
+000054a0: 616e 6420 7365 6c66 2e73 6c75 726d 5f73  and self.slurm_s
+000054b0: 6372 6970 745f 7061 7468 3a0a 2020 2020  cript_path:.    
+000054c0: 2020 2020 2020 2020 2320 6769 7420 636c          # git cl
+000054d0: 6f6e 6520 696e 746f 2073 6372 6970 7420  one into script 
+000054e0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+000054f0: 2065 6e76 203d 207b 0a20 2020 2020 2020   env = {.       
+00005500: 2020 2020 2020 2020 2022 5245 504f 5352           "REPOSR
+00005510: 4322 3a20 7365 6c66 2e73 6c75 726d 5f73  C": self.slurm_s
+00005520: 6372 6970 745f 7265 706f 2c0a 2020 2020  cript_repo,.    
+00005530: 2020 2020 2020 2020 2020 2020 224c 4f43              "LOC
+00005540: 414c 5245 504f 223a 2073 656c 662e 736c  ALREPO": self.sl
+00005550: 7572 6d5f 7363 7269 7074 5f70 6174 680a  urm_script_path.
+00005560: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00005570: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+00005580: 2767 6974 2063 6c6f 6e65 2022 2452 4550  'git clone "$REP
+00005590: 4f53 5243 2220 2224 4c4f 4341 4c52 4550  OSRC" "$LOCALREP
+000055a0: 4f22 2032 3e20 2f64 6576 2f6e 756c 6c20  O" 2> /dev/null 
+000055b0: 7c7c 2067 6974 202d 4320 2224 4c4f 4341  || git -C "$LOCA
+000055c0: 4c52 4550 4f22 2070 756c 6c27 0a20 2020  LREPO" pull'.   
+000055d0: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
+000055e0: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
+000055f0: 636d 645d 2c20 656e 7629 0a20 2020 2020  cmd], env).     
+00005600: 2020 2020 2020 2069 6620 6e6f 7420 722e         if not r.
+00005610: 6f6b 3a0a 2020 2020 2020 2020 2020 2020  ok:.            
+00005620: 2020 2020 7261 6973 6520 5353 4845 7863      raise SSHExc
+00005630: 6570 7469 6f6e 2872 290a 2020 2020 2020  eption(r).      
+00005640: 2020 656c 6966 2073 656c 662e 736c 7572    elif self.slur
+00005650: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
+00005660: 2020 2020 2020 2020 2020 2023 2067 656e             # gen
+00005670: 6572 6174 6520 7363 7269 7074 730a 2020  erate scripts.  
+00005680: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00005690: 7064 6174 655f 736c 7572 6d5f 7363 7269  pdate_slurm_scri
+000056a0: 7074 7328 6765 6e65 7261 7465 5f6a 6f62  pts(generate_job
+000056b0: 733d 5472 7565 290a 0a20 2020 2064 6566  s=True)..    def
+000056c0: 2073 6574 7570 5f64 6972 6563 746f 7269   setup_directori
+000056d0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+000056e0: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
+000056f0: 6561 7465 7320 6e65 6365 7373 6172 7920  eates necessary 
+00005700: 6469 7265 6374 6f72 6965 7320 666f 7220  directories for 
+00005710: 536c 7572 6d20 6f70 6572 6174 696f 6e73  Slurm operations
+00005720: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+00005730: 6675 6e63 7469 6f6e 2063 7265 6174 6573  function creates
+00005740: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
+00005750: 2064 6174 6120 7374 6f72 6167 652c 2073   data storage, s
+00005760: 6372 6970 7473 2c20 616e 6420 776f 726b  cripts, and work
+00005770: 666c 6f77 730a 2020 2020 2020 2020 6173  flows.        as
+00005780: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
+00005790: 6520 536c 7572 6d43 6c69 656e 7420 6f62  e SlurmClient ob
+000057a0: 6a65 6374 2e0a 0a20 2020 2020 2020 2052  ject...        R
+000057b0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+000057c0: 2020 2053 5348 4578 6365 7074 696f 6e3a     SSHException:
+000057d0: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
+000057e0: 6973 7375 6520 6578 6563 7574 696e 6720  issue executing 
+000057f0: 6469 7265 6374 6f72 7920 6372 6561 7469  directory creati
+00005800: 6f6e 2063 6f6d 6d61 6e64 732e 0a20 2020  on commands..   
+00005810: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005820: 2064 6972 5f63 6d64 7320 3d20 5b5d 0a20   dir_cmds = []. 
+00005830: 2020 2020 2020 2023 2061 2e20 6461 7461         # a. data
+00005840: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005850: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+00005860: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+00005870: 725f 636d 6473 2e61 7070 656e 6428 6622  r_cmds.append(f"
+00005880: 6d6b 6469 7220 2d70 207b 7365 6c66 2e73  mkdir -p {self.s
+00005890: 6c75 726d 5f64 6174 615f 7061 7468 7d22  lurm_data_path}"
+000058a0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+000058b0: 622e 2073 6372 6970 7473 0a20 2020 2020  b. scripts.     
+000058c0: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
+000058d0: 5f73 6372 6970 745f 7061 7468 3a0a 2020  _script_path:.  
+000058e0: 2020 2020 2020 2020 2020 6469 725f 636d            dir_cm
+000058f0: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
+00005900: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
+00005910: 5f73 6372 6970 745f 7061 7468 7d22 290a  _script_path}").
+00005920: 2020 2020 2020 2020 2020 2020 2320 632e              # c.
+00005930: 2077 6f72 6b66 6c6f 7773 0a20 2020 2020   workflows.     
+00005940: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
+00005950: 5f69 6d61 6765 735f 7061 7468 3a0a 2020  _images_path:.  
+00005960: 2020 2020 2020 2020 2020 6469 725f 636d            dir_cm
+00005970: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
+00005980: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
+00005990: 5f69 6d61 6765 735f 7061 7468 7d22 290a  _images_path}").
+000059a0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+000059b0: 2e72 756e 5f63 6f6d 6d61 6e64 7328 6469  .run_commands(di
+000059c0: 725f 636d 6473 290a 2020 2020 2020 2020  r_cmds).        
+000059d0: 6966 206e 6f74 2072 2e6f 6b3a 0a20 2020  if not r.ok:.   
+000059e0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+000059f0: 5348 4578 6365 7074 696f 6e28 7229 0a0a  SHException(r)..
+00005a00: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00005a10: 0a20 2020 2064 6566 2066 726f 6d5f 636f  .    def from_co
+00005a20: 6e66 6967 2863 6c73 2c20 636f 6e66 6967  nfig(cls, config
+00005a30: 6669 6c65 3a20 7374 7220 3d20 2727 2c0a  file: str = '',.
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2020 2020 696e 6974 5f73 6c75 726d 3a20      init_slurm: 
+00005a60: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+00005a70: 2027 536c 7572 6d43 6c69 656e 7427 3a0a   'SlurmClient':.
+00005a80: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
+00005a90: 6573 2061 206e 6577 2053 6c75 726d 436c  es a new SlurmCl
+00005aa0: 6965 6e74 206f 626a 6563 7420 7573 696e  ient object usin
+00005ab0: 6720 7468 6520 7061 7261 6d65 7465 7273  g the parameters
+00005ac0: 2072 6561 6420 6672 6f6d 2061 0a20 2020   read from a.   
+00005ad0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+00005ae0: 6f6e 2066 696c 6520 282e 696e 6929 2e0a  on file (.ini)..
+00005af0: 0a20 2020 2020 2020 2044 6566 6175 6c74  .        Default
+00005b00: 7320 7061 7468 7320 746f 206c 6f6f 6b20  s paths to look 
+00005b10: 666f 7220 636f 6e66 6967 2066 696c 6573  for config files
+00005b20: 2061 7265 3a0a 2020 2020 2020 2020 2020   are:.          
+00005b30: 2020 2d20 2f65 7463 2f73 6c75 726d 2d63    - /etc/slurm-c
+00005b40: 6f6e 6669 672e 696e 690a 2020 2020 2020  onfig.ini.      
+00005b50: 2020 2020 2020 2d20 7e2f 736c 7572 6d2d        - ~/slurm-
+00005b60: 636f 6e66 6967 2e69 6e69 0a0a 2020 2020  config.ini..    
+00005b70: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
+00005b80: 6973 2069 7320 6f6e 6c79 2066 6f72 2074  is is only for t
+00005b90: 6865 2053 4c55 524d 2073 7065 6369 6669  he SLURM specifi
+00005ba0: 6320 7661 6c75 6573 2074 6861 7420 7765  c values that we
+00005bb0: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
+00005bc0: 4d6f 7374 2063 6f6e 6669 6775 7261 7469  Most configurati
+00005bd0: 6f6e 2076 616c 7565 7320 6172 6520 7365  on values are se
+00005be0: 7420 7669 6120 636f 6e66 6967 7572 6174  t via configurat
+00005bf0: 696f 6e20 6d65 6368 616e 6973 6d73 2066  ion mechanisms f
+00005c00: 726f 6d0a 2020 2020 2020 2020 4661 6272  rom.        Fabr
+00005c10: 6963 206c 6962 7261 7279 2c0a 2020 2020  ic library,.    
+00005c20: 2020 2020 6c69 6b65 2053 5348 2073 6574      like SSH set
+00005c30: 7469 6e67 7320 6265 696e 6720 6c6f 6164  tings being load
+00005c40: 6564 2066 726f 6d20 5353 4820 636f 6e66  ed from SSH conf
+00005c50: 6967 2c20 2f65 7463 2f66 6162 7269 632e  ig, /etc/fabric.
+00005c60: 796d 6c20 6f72 0a20 2020 2020 2020 2065  yml or.        e
+00005c70: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00005c80: 626c 6573 2e0a 2020 2020 2020 2020 5365  bles..        Se
+00005c90: 6520 4661 6272 6963 2773 2064 6f63 756d  e Fabric's docum
+00005ca0: 656e 7461 7469 6f6e 2066 6f72 206d 6f72  entation for mor
+00005cb0: 6520 696e 666f 206f 6e20 636f 6e66 6967  e info on config
+00005cc0: 7572 6174 696f 6e20 6966 206e 6565 6465  uration if neede
+00005cd0: 642e 0a0a 2020 2020 2020 2020 4172 6773  d...        Args
+00005ce0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00005cf0: 6e66 6967 6669 6c65 2028 7374 7229 3a20  nfigfile (str): 
+00005d00: 5468 6520 7061 7468 2074 6f20 796f 7572  The path to your
+00005d10: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00005d20: 696c 652e 204f 7074 696f 6e61 6c2e 0a20  ile. Optional.. 
+00005d30: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
+00005d40: 736c 7572 6d20 2862 6f6f 6c29 3a20 496e  slurm (bool): In
+00005d50: 6974 6961 7465 202f 2076 616c 6964 6174  itiate / validat
+00005d60: 6520 736c 7572 6d20 7365 7475 702e 204f  e slurm setup. O
+00005d70: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00005d80: 2020 2020 2020 2020 4d69 6768 7420 7461          Might ta
+00005d90: 6b65 2073 6f6d 6520 7469 6d65 2074 6865  ke some time the
+00005da0: 2066 6972 7374 2074 696d 6520 7769 7468   first time with
+00005db0: 2064 6f77 6e6c 6f61 6469 6e67 2065 7463   downloading etc
+00005dc0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005dd0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00005de0: 536c 7572 6d43 6c69 656e 743a 2041 206e  SlurmClient: A n
+00005df0: 6577 2053 6c75 726d 436c 6965 6e74 206f  ew SlurmClient o
+00005e00: 626a 6563 742e 0a20 2020 2020 2020 2022  bject..        "
+00005e10: 2222 0a20 2020 2020 2020 2023 204c 6f61  "".        # Loa
+00005e20: 6420 7468 6520 636f 6e66 6967 7572 6174  d the configurat
+00005e30: 696f 6e20 6669 6c65 0a20 2020 2020 2020  ion file.       
+00005e40: 2063 6f6e 6669 6773 203d 2063 6f6e 6669   configs = confi
+00005e50: 6770 6172 7365 722e 436f 6e66 6967 5061  gparser.ConfigPa
+00005e60: 7273 6572 2861 6c6c 6f77 5f6e 6f5f 7661  rser(allow_no_va
+00005e70: 6c75 653d 5472 7565 290a 2020 2020 2020  lue=True).      
+00005e80: 2020 2320 4c6f 6164 7320 6672 6f6d 2064    # Loads from d
+00005e90: 6566 6175 6c74 206c 6f63 6174 696f 6e73  efault locations
+00005ea0: 2061 6e64 2067 6976 656e 206c 6f63 6174   and given locat
+00005eb0: 696f 6e2c 206d 6973 7369 6e67 2066 696c  ion, missing fil
+00005ec0: 6573 2061 7265 206f 6b0a 2020 2020 2020  es are ok.      
+00005ed0: 2020 636f 6e66 6967 732e 7265 6164 285b    configs.read([
+00005ee0: 636c 732e 5f44 4546 4155 4c54 5f43 4f4e  cls._DEFAULT_CON
+00005ef0: 4649 475f 5041 5448 5f31 2c0a 2020 2020  FIG_PATH_1,.    
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 2063 6c73 2e5f 4445 4641 554c 545f 434f   cls._DEFAULT_CO
+00005f20: 4e46 4947 5f50 4154 485f 322c 0a20 2020  NFIG_PATH_2,.   
+00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f40: 2020 636f 6e66 6967 6669 6c65 5d29 0a20    configfile]). 
+00005f50: 2020 2020 2020 2023 2052 6561 6420 7468         # Read th
+00005f60: 6520 7265 7175 6972 6564 2070 6172 616d  e required param
+00005f70: 6574 6572 7320 6672 6f6d 2074 6865 2063  eters from the c
+00005f80: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+00005f90: 652c 0a20 2020 2020 2020 2023 2066 616c  e,.        # fal
+00005fa0: 6c62 6163 6b20 746f 2064 6566 6175 6c74  lback to default
+00005fb0: 730a 2020 2020 2020 2020 686f 7374 203d  s.        host =
+00005fc0: 2063 6f6e 6669 6773 2e67 6574 2822 5353   configs.get("SS
+00005fd0: 4822 2c20 2268 6f73 7422 2c20 6661 6c6c  H", "host", fall
+00005fe0: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
+00005ff0: 545f 484f 5354 290a 2020 2020 2020 2020  T_HOST).        
+00006000: 696e 6c69 6e65 5f73 7368 5f65 6e76 203d  inline_ssh_env =
+00006010: 2063 6f6e 6669 6773 2e67 6574 626f 6f6c   configs.getbool
+00006020: 6561 6e28 0a20 2020 2020 2020 2020 2020  ean(.           
+00006030: 2022 5353 4822 2c20 2269 6e6c 696e 655f   "SSH", "inline_
+00006040: 7373 685f 656e 7622 2c20 6661 6c6c 6261  ssh_env", fallba
+00006050: 636b 3d63 6c73 2e5f 4445 4641 554c 545f  ck=cls._DEFAULT_
+00006060: 494e 4c49 4e45 5f53 5348 5f45 4e56 290a  INLINE_SSH_ENV).
+00006070: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
+00006080: 7461 5f70 6174 6820 3d20 636f 6e66 6967  ta_path = config
+00006090: 732e 6765 7428 0a20 2020 2020 2020 2020  s.get(.         
+000060a0: 2020 2022 534c 5552 4d22 2c20 2273 6c75     "SLURM", "slu
+000060b0: 726d 5f64 6174 615f 7061 7468 222c 2066  rm_data_path", f
+000060c0: 616c 6c62 6163 6b3d 636c 732e 5f44 4546  allback=cls._DEF
+000060d0: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
+000060e0: 5041 5448 290a 2020 2020 2020 2020 736c  PATH).        sl
+000060f0: 7572 6d5f 696d 6167 6573 5f70 6174 6820  urm_images_path 
+00006100: 3d20 636f 6e66 6967 732e 6765 7428 0a20  = configs.get(. 
+00006110: 2020 2020 2020 2020 2020 2022 534c 5552             "SLUR
+00006120: 4d22 2c20 2273 6c75 726d 5f69 6d61 6765  M", "slurm_image
+00006130: 735f 7061 7468 222c 0a20 2020 2020 2020  s_path",.       
+00006140: 2020 2020 2066 616c 6c62 6163 6b3d 636c       fallback=cl
+00006150: 732e 5f44 4546 4155 4c54 5f53 4c55 524d  s._DEFAULT_SLURM
+00006160: 5f49 4d41 4745 535f 5041 5448 290a 2020  _IMAGES_PATH).  
+00006170: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
+00006180: 6572 7465 7273 5f70 6174 6820 3d20 636f  erters_path = co
+00006190: 6e66 6967 732e 6765 7428 0a20 2020 2020  nfigs.get(.     
+000061a0: 2020 2020 2020 2022 534c 5552 4d22 2c20         "SLURM", 
+000061b0: 2273 6c75 726d 5f63 6f6e 7665 7274 6572  "slurm_converter
+000061c0: 735f 7061 7468 222c 0a20 2020 2020 2020  s_path",.       
+000061d0: 2020 2020 2066 616c 6c62 6163 6b3d 636c       fallback=cl
+000061e0: 732e 5f44 4546 4155 4c54 5f53 4c55 524d  s._DEFAULT_SLURM
+000061f0: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
+00006200: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
+00006210: 6974 2074 6865 204d 4f44 454c 5320 696e  it the MODELS in
+00006220: 746f 2070 6174 6873 2c20 7265 706f 7320  to paths, repos 
+00006230: 616e 6420 696d 6167 6573 0a20 2020 2020  and images.     
+00006240: 2020 206d 6f64 656c 735f 6469 6374 203d     models_dict =
+00006250: 2064 6963 7428 636f 6e66 6967 732e 6974   dict(configs.it
+00006260: 656d 7328 224d 4f44 454c 5322 2929 0a20  ems("MODELS")). 
+00006270: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006280: 656c 5f70 6174 6873 203d 207b 7d0a 2020  el_paths = {}.  
+00006290: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+000062a0: 6c5f 7265 706f 7320 3d20 7b7d 0a20 2020  l_repos = {}.   
+000062b0: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+000062c0: 5f6a 6f62 7320 3d20 7b7d 0a20 2020 2020  _jobs = {}.     
+000062d0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f6a     slurm_model_j
+000062e0: 6f62 735f 7061 7261 6d73 203d 207b 7d0a  obs_params = {}.
+000062f0: 2020 2020 2020 2020 666f 7220 6b2c 2076          for k, v
+00006300: 2069 6e20 6d6f 6465 6c73 5f64 6963 742e   in models_dict.
+00006310: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00006320: 2020 2020 2073 7566 6669 785f 7265 706f       suffix_repo
+00006330: 203d 2027 5f72 6570 6f27 0a20 2020 2020   = '_repo'.     
+00006340: 2020 2020 2020 2073 7566 6669 785f 6a6f         suffix_jo
+00006350: 6220 3d20 275f 6a6f 6227 0a20 2020 2020  b = '_job'.     
+00006360: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
+00006370: 5f70 6174 7465 726e 203d 2022 282e 2b29  _pattern = "(.+)
+00006380: 5f6a 6f62 5f28 2e2b 2922 0a20 2020 2020  _job_(.+)".     
+00006390: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
+000063a0: 5f6d 6174 6368 203d 2072 652e 6d61 7463  _match = re.matc
+000063b0: 6828 6a6f 625f 7061 7261 6d5f 7061 7474  h(job_param_patt
+000063c0: 6572 6e2c 206b 290a 2020 2020 2020 2020  ern, k).        
+000063d0: 2020 2020 6966 206b 2e65 6e64 7377 6974      if k.endswit
+000063e0: 6828 7375 6666 6978 5f72 6570 6f29 3a0a  h(suffix_repo):.
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 736c 7572 6d5f 6d6f 6465 6c5f 7265 706f  slurm_model_repo
+00006410: 735b 6b5b 3a2d 6c65 6e28 7375 6666 6978  s[k[:-len(suffix
+00006420: 5f72 6570 6f29 5d5d 203d 2076 0a20 2020  _repo)]] = v.   
+00006430: 2020 2020 2020 2020 2065 6c69 6620 6b2e           elif k.
+00006440: 656e 6473 7769 7468 2873 7566 6669 785f  endswith(suffix_
+00006450: 6a6f 6229 3a0a 2020 2020 2020 2020 2020  job):.          
+00006460: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006470: 6c5f 6a6f 6273 5b6b 5b3a 2d6c 656e 2873  l_jobs[k[:-len(s
+00006480: 7566 6669 785f 6a6f 6229 5d5d 203d 2076  uffix_job)]] = v
+00006490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064a0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+000064b0: 735f 7061 7261 6d73 5b6b 5b3a 2d6c 656e  s_params[k[:-len
+000064c0: 2873 7566 6669 785f 6a6f 6229 5d5d 203d  (suffix_job)]] =
+000064d0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+000064e0: 656c 6966 206a 6f62 5f70 6172 616d 5f6d  elif job_param_m
+000064f0: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00006500: 2020 2020 2020 7072 696e 7428 6622 4d61        print(f"Ma
+00006510: 7463 683a 207b 736c 7572 6d5f 6d6f 6465  tch: {slurm_mode
+00006520: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
+00006530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006540: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+00006550: 735f 7061 7261 6d73 5b6a 6f62 5f70 6172  s_params[job_par
+00006560: 616d 5f6d 6174 6368 2e67 726f 7570 2831  am_match.group(1
+00006570: 295d 2e61 7070 656e 6428 0a20 2020 2020  )].append(.     
+00006580: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006590: 2220 2d2d 7b6a 6f62 5f70 6172 616d 5f6d  " --{job_param_m
+000065a0: 6174 6368 2e67 726f 7570 2832 297d 3d7b  atch.group(2)}={
+000065b0: 767d 2229 0a20 2020 2020 2020 2020 2020  v}").           
+000065c0: 2020 2020 2070 7269 6e74 2866 2241 6464       print(f"Add
+000065d0: 6564 3a20 7b73 6c75 726d 5f6d 6f64 656c  ed: {slurm_model
+000065e0: 5f6a 6f62 735f 7061 7261 6d73 7d22 290a  _jobs_params}").
+000065f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00006600: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006610: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
+00006620: 7468 735b 6b5d 203d 2076 0a0a 2020 2020  ths[k] = v..    
+00006630: 2020 2020 736c 7572 6d5f 7363 7269 7074      slurm_script
+00006640: 5f70 6174 6820 3d20 636f 6e66 6967 732e  _path = configs.
+00006650: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
+00006660: 2022 534c 5552 4d22 2c20 2273 6c75 726d   "SLURM", "slurm
+00006670: 5f73 6372 6970 745f 7061 7468 222c 0a20  _script_path",. 
+00006680: 2020 2020 2020 2020 2020 2066 616c 6c62             fallb
+00006690: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
+000066a0: 5f53 4c55 524d 5f47 4954 5f53 4352 4950  _SLURM_GIT_SCRIP
+000066b0: 545f 5041 5448 290a 2020 2020 2020 2020  T_PATH).        
+000066c0: 736c 7572 6d5f 7363 7269 7074 5f72 6570  slurm_script_rep
+000066d0: 6f20 3d20 636f 6e66 6967 732e 6765 7428  o = configs.get(
+000066e0: 0a20 2020 2020 2020 2020 2020 2022 534c  .            "SL
+000066f0: 5552 4d22 2c20 2273 6c75 726d 5f73 6372  URM", "slurm_scr
+00006700: 6970 745f 7265 706f 222c 0a20 2020 2020  ipt_repo",.     
+00006710: 2020 2020 2020 2066 616c 6c62 6163 6b3d         fallback=
+00006720: 4e6f 6e65 0a20 2020 2020 2020 2029 0a20  None.        ). 
+00006730: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00006740: 7468 6520 536c 7572 6d43 6c69 656e 7420  the SlurmClient 
+00006750: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
+00006760: 7061 7261 6d65 7465 7273 2072 6561 6420  parameters read 
+00006770: 6672 6f6d 0a20 2020 2020 2020 2023 2074  from.        # t
+00006780: 6865 2063 6f6e 6669 6720 6669 6c65 0a20  he config file. 
+00006790: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+000067a0: 7328 686f 7374 3d68 6f73 742c 0a20 2020  s(host=host,.   
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067c0: 696e 6c69 6e65 5f73 7368 5f65 6e76 3d69  inline_ssh_env=i
+000067d0: 6e6c 696e 655f 7373 685f 656e 762c 0a20  nline_ssh_env,. 
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 736c 7572 6d5f 6461 7461 5f70 6174    slurm_data_pat
+00006800: 683d 736c 7572 6d5f 6461 7461 5f70 6174  h=slurm_data_pat
+00006810: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+00006820: 2020 2020 2020 736c 7572 6d5f 696d 6167        slurm_imag
+00006830: 6573 5f70 6174 683d 736c 7572 6d5f 696d  es_path=slurm_im
+00006840: 6167 6573 5f70 6174 682c 0a20 2020 2020  ages_path,.     
+00006850: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00006860: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
+00006870: 6174 683d 736c 7572 6d5f 636f 6e76 6572  ath=slurm_conver
+00006880: 7465 7273 5f70 6174 682c 0a20 2020 2020  ters_path,.     
+00006890: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+000068a0: 7572 6d5f 6d6f 6465 6c5f 7061 7468 733d  urm_model_paths=
+000068b0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
+000068c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000068d0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+000068e0: 6c5f 7265 706f 733d 736c 7572 6d5f 6d6f  l_repos=slurm_mo
+000068f0: 6465 6c5f 7265 706f 732c 0a20 2020 2020  del_repos,.     
+00006900: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00006910: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
+00006920: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00006930: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+00006940: 6d6f 6465 6c5f 6a6f 6273 3d73 6c75 726d  model_jobs=slurm
+00006950: 5f6d 6f64 656c 5f6a 6f62 732c 0a20 2020  _model_jobs,.   
 00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
-00006980: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00006990: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-000069a0: 615f 6c6f 6361 7469 6f6e 3a20 7374 7220  a_location: str 
-000069b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
-000069e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2029 202d 3e20 5265 7375 6c74 3a0a 2020   ) -> Result:.  
-00006a10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006a20: 2020 436c 6561 6e75 7020 7a69 7020 616e    Cleanup zip an
-00006a30: 6420 756e 7a69 7070 6564 2066 696c 6573  d unzipped files
-00006a40: 2f66 6f6c 6465 7273 2061 7373 6f63 6961  /folders associa
-00006a50: 7465 6420 7769 7468 2061 2053 6c75 726d  ted with a Slurm
-00006a60: 206a 6f62 2e0a 0a20 2020 2020 2020 2041   job...        A
-00006a70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00006a80: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
-00006a90: 7472 293a 2054 6865 206a 6f62 2049 4420  tr): The job ID 
-00006aa0: 6f66 2074 6865 2053 6c75 726d 2073 6372  of the Slurm scr
-00006ab0: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
-00006ac0: 2066 696c 656e 616d 6520 2873 7472 293a   filename (str):
-00006ad0: 2054 6865 207a 6970 2066 696c 656e 616d   The zip filenam
-00006ae0: 6520 6f6e 2053 6c75 726d 2e0a 2020 2020  e on Slurm..    
-00006af0: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
-00006b00: 6174 696f 6e20 2873 7472 2c20 6f70 7469  ation (str, opti
-00006b10: 6f6e 616c 293a 2054 6865 206c 6f63 6174  onal): The locat
-00006b20: 696f 6e20 6f66 2064 6174 6120 6669 6c65  ion of data file
-00006b30: 7320 6f6e 2053 6c75 726d 2e0a 2020 2020  s on Slurm..    
-00006b40: 2020 2020 2020 2020 2020 2020 4966 206e              If n
-00006b50: 6f74 2070 726f 7669 6465 642c 2069 7420  ot provided, it 
-00006b60: 7769 6c6c 2062 6520 6578 7472 6163 7465  will be extracte
-00006b70: 6420 6672 6f6d 2074 6865 206c 6f67 2066  d from the log f
-00006b80: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
-00006b90: 206c 6f67 6669 6c65 2028 7374 722c 206f   logfile (str, o
-00006ba0: 7074 696f 6e61 6c29 3a20 5468 6520 6c6f  ptional): The lo
-00006bb0: 6720 6669 6c65 206f 6620 7468 6520 536c  g file of the Sl
-00006bc0: 7572 6d20 6a6f 622e 200a 2020 2020 2020  urm job. .      
-00006bd0: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
-00006be0: 2070 726f 7669 6465 642c 2061 2064 6566   provided, a def
-00006bf0: 6175 6c74 206c 6f67 2066 696c 6520 7769  ault log file wi
-00006c00: 6c6c 2062 6520 7573 6564 2e0a 0a20 2020  ll be used...   
-00006c10: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00006c20: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
-00006c30: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
-00006c40: 7468 6520 636c 6561 6e75 7020 6f70 6572  the cleanup oper
-00006c50: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00006c60: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
-00006c70: 2020 5468 6520 636c 6561 6e75 7020 7072    The cleanup pr
-00006c80: 6f63 6573 7320 696e 766f 6c76 6573 2072  ocess involves r
-00006c90: 656d 6f76 696e 6720 7468 6520 7370 6563  emoving the spec
-00006ca0: 6966 6965 6420 7a69 7020 6669 6c65 2c20  ified zip file, 
-00006cb0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-00006cc0: 206c 6f67 2066 696c 652c 2061 6e64 2061   log file, and a
-00006cd0: 7373 6f63 6961 7465 6420 6461 7461 2066  ssociated data f
-00006ce0: 696c 6573 2061 6e64 2066 6f6c 6465 7273  iles and folders
-00006cf0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00006d00: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00006d10: 2320 436c 6561 6e75 7020 7465 6d70 6f72  # Cleanup tempor
-00006d20: 6172 7920 6669 6c65 7320 666f 7220 6120  ary files for a 
-00006d30: 536c 7572 6d20 6a6f 620a 2020 2020 2020  Slurm job.      
-00006d40: 2020 2020 2020 636c 6965 6e74 2e63 6c65        client.cle
-00006d50: 616e 7570 5f74 6d70 5f66 696c 6573 2822  anup_tmp_files("
-00006d60: 3132 3334 3522 2c20 226f 7574 7075 742e  12345", "output.
-00006d70: 7a69 7022 290a 2020 2020 2020 2020 2222  zip").        ""
-00006d80: 220a 2020 2020 2020 2020 636d 6473 203d  ".        cmds =
-00006d90: 205b 5d0a 2020 2020 2020 2020 2320 7a69   [].        # zi
-00006da0: 700a 2020 2020 2020 2020 726d 7a69 7020  p.        rmzip 
-00006db0: 3d20 6622 726d 207b 6669 6c65 6e61 6d65  = f"rm {filename
-00006dc0: 7d2e 2a22 0a20 2020 2020 2020 2063 6d64  }.*".        cmd
-00006dd0: 732e 6170 7065 6e64 2872 6d7a 6970 290a  s.append(rmzip).
-00006de0: 2020 2020 2020 2020 2320 6c6f 670a 2020          # log.  
-00006df0: 2020 2020 2020 6966 206c 6f67 6669 6c65        if logfile
-00006e00: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006e10: 2020 2020 2020 6c6f 6766 696c 6520 3d20        logfile = 
-00006e20: 7365 6c66 2e5f 4c4f 4746 494c 450a 2020  self._LOGFILE.  
-00006e30: 2020 2020 2020 2020 2020 6c6f 6766 696c            logfil
-00006e40: 6520 3d20 6c6f 6766 696c 652e 666f 726d  e = logfile.form
-00006e50: 6174 2873 6c75 726d 5f6a 6f62 5f69 643d  at(slurm_job_id=
-00006e60: 736c 7572 6d5f 6a6f 625f 6964 290a 2020  slurm_job_id).  
-00006e70: 2020 2020 2020 726d 6c6f 6720 3d20 6622        rmlog = f"
-00006e80: 726d 207b 6c6f 6766 696c 657d 220a 2020  rm {logfile}".  
-00006e90: 2020 2020 2020 636d 6473 2e61 7070 656e        cmds.appen
-00006ea0: 6428 726d 6c6f 6729 0a20 2020 2020 2020  d(rmlog).       
-00006eb0: 2023 2063 6f6e 7665 7274 6572 206c 6f67   # converter log
-00006ec0: 730a 2020 2020 2020 2020 636c 6f67 203d  s.        clog =
-00006ed0: 2073 656c 662e 5f43 4f4e 5645 5254 4552   self._CONVERTER
-00006ee0: 5f4c 4f47 4649 4c45 0a20 2020 2020 2020  _LOGFILE.       
-00006ef0: 2063 6c6f 6720 3d20 636c 6f67 2e66 6f72   clog = clog.for
-00006f00: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
-00006f10: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
-00006f20: 2020 2020 2020 2072 6d63 6c6f 6720 3d20         rmclog = 
-00006f30: 6622 726d 207b 636c 6f67 7d22 0a20 2020  f"rm {clog}".   
-00006f40: 2020 2020 2063 6d64 732e 6170 7065 6e64       cmds.append
-00006f50: 2872 6d63 6c6f 6729 0a20 2020 2020 2020  (rmclog).       
-00006f60: 2023 2064 6174 610a 2020 2020 2020 2020   # data.        
-00006f70: 6966 2064 6174 615f 6c6f 6361 7469 6f6e  if data_location
-00006f80: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006f90: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
-00006fa0: 696f 6e20 3d20 7365 6c66 2e65 7874 7261  ion = self.extra
-00006fb0: 6374 5f64 6174 615f 6c6f 6361 7469 6f6e  ct_data_location
-00006fc0: 5f66 726f 6d5f 6c6f 6728 6c6f 6766 696c  _from_log(logfil
-00006fd0: 6529 0a20 2020 2020 2020 2072 6d64 6174  e).        rmdat
-00006fe0: 6120 3d20 6622 726d 202d 7266 207b 6461  a = f"rm -rf {da
-00006ff0: 7461 5f6c 6f63 6174 696f 6e7d 207b 6461  ta_location} {da
-00007000: 7461 5f6c 6f63 6174 696f 6e7d 2e2a 220a  ta_location}.*".
-00007010: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
-00007020: 656e 6428 726d 6461 7461 290a 0a20 2020  end(rmdata)..   
-00007030: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00007040: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-00007050: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-00007060: 2863 6d64 7329 0a20 2020 2020 2020 2065  (cmds).        e
-00007070: 7863 6570 7420 556e 6578 7065 6374 6564  xcept Unexpected
-00007080: 4578 6974 2061 7320 653a 0a20 2020 2020  Exit as e:.     
-00007090: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-000070a0: 726e 696e 6728 6529 0a20 2020 2020 2020  rning(e).       
-000070b0: 2020 2020 2072 6573 756c 7420 3d20 652e       result = e.
-000070c0: 7265 7375 6c74 0a20 2020 2020 2020 2072  result.        r
-000070d0: 6574 7572 6e20 7265 7375 6c74 206f 7220  eturn result or 
-000070e0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7661  None..    def va
-000070f0: 6c69 6461 7465 2873 656c 662c 2076 616c  lidate(self, val
-00007100: 6964 6174 655f 736c 7572 6d5f 7365 7475  idate_slurm_setu
-00007110: 703a 2062 6f6f 6c20 3d20 4661 6c73 6529  p: bool = False)
-00007120: 3a0a 2020 2020 2020 2020 2222 2256 616c  :.        """Val
-00007130: 6964 6174 6520 7468 6520 636f 6e6e 6563  idate the connec
-00007140: 7469 6f6e 2074 6f20 7468 6520 536c 7572  tion to the Slur
-00007150: 6d20 636c 7573 7465 7220 6279 2072 756e  m cluster by run
-00007160: 6e69 6e67 0a20 2020 2020 2020 2061 2073  ning.        a s
-00007170: 696d 706c 6520 636f 6d6d 616e 642e 0a0a  imple command...
-00007180: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00007190: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-000071a0: 7465 5f73 6c75 726d 5f73 6574 7570 2028  te_slurm_setup (
-000071b0: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
-000071c0: 6f20 616c 736f 2063 6865 636b 0a20 2020  o also check.   
-000071d0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-000071e0: 2066 6978 2074 6865 2053 6c75 726d 2073   fix the Slurm s
-000071f0: 6574 7570 2028 666f 6c64 6572 732c 2069  etup (folders, i
-00007200: 6d61 6765 732c 2065 7463 2e29 0a0a 2020  mages, etc.)..  
-00007210: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00007220: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
-00007230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007240: 2054 7275 6520 6966 2074 6865 2076 616c   True if the val
-00007250: 6964 6174 696f 6e20 6973 2073 7563 6365  idation is succe
-00007260: 7373 6675 6c2c 0a20 2020 2020 2020 2020  ssful,.         
-00007270: 2020 2020 2020 2046 616c 7365 206f 7468         False oth
-00007280: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00007290: 2222 220a 2020 2020 2020 2020 636f 6e6e  """.        conn
-000072a0: 6563 7465 6420 3d20 7365 6c66 2e72 756e  ected = self.run
-000072b0: 2827 6563 686f 2022 2022 2729 2e6f 6b0a  ('echo " "').ok.
-000072c0: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
-000072d0: 6374 6564 2061 6e64 2076 616c 6964 6174  cted and validat
-000072e0: 655f 736c 7572 6d5f 7365 7475 703a 0a20  e_slurm_setup:. 
-000072f0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 7365 6c66 2e73 6574 7570 5f73 6c75 726d  self.setup_slurm
-00007320: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-00007330: 7863 6570 7420 5353 4845 7863 6570 7469  xcept SSHExcepti
-00007340: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00007350: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007360: 6572 726f 7228 6529 0a20 2020 2020 2020  error(e).       
-00007370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007380: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
-00007390: 7475 726e 2063 6f6e 6e65 6374 6564 0a0a  turn connected..
-000073a0: 2020 2020 6465 6620 6765 745f 7265 6365      def get_rece
-000073b0: 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64 2873  nt_log_command(s
-000073c0: 656c 662c 206c 6f67 5f66 696c 653a 2073  elf, log_file: s
-000073d0: 7472 2c20 6e3a 2069 6e74 203d 2031 3029  tr, n: int = 10)
-000073e0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-000073f0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-00007400: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
-00007410: 7265 7472 6965 7665 2074 6865 2072 6563  retrieve the rec
-00007420: 656e 7420 6c6f 6720 656e 7472 6965 7320  ent log entries 
-00007430: 6672 6f6d 2061 0a20 2020 2020 2020 2073  from a.        s
-00007440: 7065 6369 6669 6564 206c 6f67 2066 696c  pecified log fil
-00007450: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-00007460: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00007470: 675f 6669 6c65 2028 7374 7229 3a20 5468  g_file (str): Th
-00007480: 6520 7061 7468 2074 6f20 7468 6520 6c6f  e path to the lo
-00007490: 6720 6669 6c65 2e0a 2020 2020 2020 2020  g file..        
-000074a0: 2020 2020 6e20 2869 6e74 2c20 6f70 7469      n (int, opti
-000074b0: 6f6e 616c 293a 2054 6865 206e 756d 6265  onal): The numbe
-000074c0: 7220 6f66 2072 6563 656e 7420 6c6f 6720  r of recent log 
-000074d0: 656e 7472 6965 7320 746f 2072 6574 7269  entries to retri
-000074e0: 6576 652e 0a20 2020 2020 2020 2020 2020  eve..           
-000074f0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00007500: 2031 302e 0a0a 2020 2020 2020 2020 5265   10...        Re
-00007510: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00007520: 2020 2073 7472 3a20 5468 6520 636f 6d6d     str: The comm
-00007530: 616e 6420 746f 2072 6574 7269 6576 6520  and to retrieve 
-00007540: 7468 6520 7265 6365 6e74 206c 6f67 2065  the recent log e
-00007550: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
-00007560: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00007570: 726e 2073 656c 662e 5f54 4149 4c5f 4c4f  rn self._TAIL_LO
-00007580: 475f 434d 442e 666f 726d 6174 286e 3d6e  G_CMD.format(n=n
-00007590: 2c20 6c6f 675f 6669 6c65 3d6c 6f67 5f66  , log_file=log_f
-000075a0: 696c 6529 0a0a 2020 2020 6465 6620 6765  ile)..    def ge
-000075b0: 745f 6163 7469 7665 5f6a 6f62 5f70 726f  t_active_job_pro
-000075c0: 6772 6573 7328 7365 6c66 2c0a 2020 2020  gress(self,.    
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-000075f0: 6d5f 6a6f 625f 6964 3a20 7374 722c 0a20  m_job_id: str,. 
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007620: 6174 7465 726e 3a20 7374 7220 3d20 7222  attern: str = r"
-00007630: 5c64 2b25 222c 0a20 2020 2020 2020 2020  \d+%",.         
-00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007650: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00007660: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00007670: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-00007680: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-00007690: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
-000076a0: 2070 726f 6772 6573 7320 6f66 2061 6e20   progress of an 
-000076b0: 6163 7469 7665 2053 6c75 726d 206a 6f62  active Slurm job
-000076c0: 2066 726f 6d20 6974 7320 6c6f 6766 696c   from its logfil
-000076d0: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
-000076e0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-000076f0: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
-00007700: 293a 2054 6865 2049 4420 6f66 2074 6865  ): The ID of the
-00007710: 2053 6c75 726d 206a 6f62 2e0a 2020 2020   Slurm job..    
-00007720: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
-00007730: 2873 7472 293a 2054 6865 2070 6174 7465  (str): The patte
-00007740: 726e 2074 6f20 6d61 7463 6820 696e 2074  rn to match in t
-00007750: 6865 206a 6f62 206c 6f67 2074 6f20 6578  he job log to ex
-00007760: 7472 6163 740a 2020 2020 2020 2020 2020  tract.          
-00007770: 2020 2020 2020 7468 6520 7072 6f67 7265        the progre
-00007780: 7373 2028 6465 6661 756c 743a 2072 225c  ss (default: r"\
-00007790: 642b 2522 292e 0a0a 2020 2020 2020 2020  d+%")...        
-000077a0: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
-000077b0: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-000077c0: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
-000077d0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-000077e0: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
-000077f0: 2020 2020 746f 2073 6574 2077 6865 6e20      to set when 
-00007800: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00007810: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-00007820: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00007830: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00007840: 2020 2020 2073 7472 3a20 5468 6520 7072       str: The pr
-00007850: 6f67 7265 7373 206f 6620 7468 6520 536c  ogress of the Sl
-00007860: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
-00007870: 2022 2222 0a20 2020 2020 2020 2063 6d64   """.        cmd
-00007880: 6c69 7374 203d 205b 5d0a 2020 2020 2020  list = [].      
-00007890: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
-000078a0: 5f72 6563 656e 745f 6c6f 675f 636f 6d6d  _recent_log_comm
-000078b0: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
-000078c0: 206c 6f67 5f66 696c 653d 7365 6c66 2e5f   log_file=self._
-000078d0: 4c4f 4746 494c 452e 666f 726d 6174 2873  LOGFILE.format(s
-000078e0: 6c75 726d 5f6a 6f62 5f69 643d 736c 7572  lurm_job_id=slur
-000078f0: 6d5f 6a6f 625f 6964 2929 0a20 2020 2020  m_job_id)).     
-00007900: 2020 2063 6d64 6c69 7374 2e61 7070 656e     cmdlist.appen
-00007910: 6428 636d 6429 0a20 2020 2020 2020 2069  d(cmd).        i
-00007920: 6620 656e 7620 6973 204e 6f6e 653a 0a20  f env is None:. 
-00007930: 2020 2020 2020 2020 2020 2065 6e76 203d             env =
-00007940: 207b 7d0a 2020 2020 2020 2020 7472 793a   {}.        try:
-00007950: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007960: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-00007970: 6f6d 6d61 6e64 7328 636d 646c 6973 742c  ommands(cmdlist,
-00007980: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
-00007990: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000079a0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-000079b0: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
-000079c0: 7228 6622 4973 7375 6520 7769 7468 2072  r(f"Issue with r
-000079d0: 756e 2063 6f6d 6d61 6e64 3a20 7b65 7d22  un command: {e}"
-000079e0: 290a 2020 2020 2020 2020 2320 4d61 7463  ).        # Matc
-000079f0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-00007a00: 7061 7474 6572 6e20 696e 2074 6865 2072  pattern in the r
-00007a10: 6573 756c 7427 7320 7374 646f 7574 0a20  esult's stdout. 
-00007a20: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00007a30: 2020 2020 2020 2020 6c61 7465 7374 5f70          latest_p
-00007a40: 726f 6772 6573 7320 3d20 7265 2e66 696e  rogress = re.fin
-00007a50: 6461 6c6c 280a 2020 2020 2020 2020 2020  dall(.          
-00007a60: 2020 2020 2020 7061 7474 6572 6e2c 2072        pattern, r
-00007a70: 6573 756c 742e 7374 646f 7574 295b 2d31  esult.stdout)[-1
-00007a80: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
-00007a90: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00007aa0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00007ab0: 6765 722e 6572 726f 7228 6622 4973 7375  ger.error(f"Issu
-00007ac0: 6520 7769 7468 2065 7874 7261 6374 696e  e with extractin
-00007ad0: 6720 7072 6f67 7265 7373 3a20 7b65 7d22  g progress: {e}"
-00007ae0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00007af0: 6e20 6622 5072 6f67 7265 7373 3a20 7b6c  n f"Progress: {l
-00007b00: 6174 6573 745f 7072 6f67 7265 7373 7d5c  atest_progress}\
-00007b10: 6e22 0a0a 2020 2020 6465 6620 7275 6e5f  n"..    def run_
-00007b20: 636f 6d6d 616e 6473 2873 656c 662c 2063  commands(self, c
-00007b30: 6d64 6c69 7374 3a20 4c69 7374 5b73 7472  mdlist: List[str
-00007b40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00007b50: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
-00007b60: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00007b70: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 2073 6570 3a20 7374 7220 3d20 2720     sep: str = ' 
-00007ba0: 2626 2027 2c0a 2020 2020 2020 2020 2020  && ',.          
-00007bb0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00007bc0: 7267 7329 202d 3e20 5265 7375 6c74 3a0a  rgs) -> Result:.
-00007bd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007be0: 2020 2020 5275 6e20 6120 6c69 7374 206f      Run a list o
-00007bf0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
-00007c00: 2063 6f6e 7365 6375 7469 7665 6c79 206f   consecutively o
-00007c10: 6e20 7468 6520 536c 7572 6d20 636c 7573  n the Slurm clus
-00007c20: 7465 722c 0a20 2020 2020 2020 2065 6e73  ter,.        ens
-00007c30: 7572 696e 6720 7468 6520 7375 6363 6573  uring the succes
-00007c40: 7320 6f66 2065 6163 6820 6265 666f 7265  s of each before
-00007c50: 2070 726f 6365 6564 696e 6720 746f 2074   proceeding to t
-00007c60: 6865 206e 6578 742e 0a0a 2020 2020 2020  he next...      
-00007c70: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
-00007c80: 7420 7661 7269 6162 6c65 7320 6361 6e20  t variables can 
-00007c90: 6265 2073 6574 2075 7369 6e67 2074 6865  be set using the
-00007ca0: 2060 656e 7660 2061 7267 756d 656e 742e   `env` argument.
-00007cb0: 0a20 2020 2020 2020 2054 6865 7365 2063  .        These c
-00007cc0: 6f6d 6d61 6e64 7320 7265 7461 696e 2074  ommands retain t
-00007cd0: 6865 2073 616d 6520 7365 7373 696f 6e20  he same session 
-00007ce0: 2865 6e76 6972 6f6e 6d65 6e74 2076 6172  (environment var
-00007cf0: 6961 626c 6573 0a20 2020 2020 2020 2065  iables.        e
-00007d00: 7463 2e29 2c20 756e 6c69 6b65 2072 756e  tc.), unlike run
-00007d10: 6e69 6e67 2074 6865 6d20 7365 7061 7261  ning them separa
-00007d20: 7465 6c79 2e0a 0a20 2020 2020 2020 2041  tely...        A
-00007d30: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00007d40: 2063 6d64 6c69 7374 2028 4c69 7374 5b73   cmdlist (List[s
-00007d50: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
-00007d60: 7368 656c 6c20 636f 6d6d 616e 6473 2074  shell commands t
-00007d70: 6f20 7275 6e20 6f6e 2053 6c75 726d 2e0a  o run on Slurm..
-00007d80: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00007d90: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
-00007da0: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
-00007db0: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
-00007dc0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007de0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-00007df0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-00007e00: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00007e10: 2020 2020 2020 2020 2020 7365 7020 2873            sep (s
-00007e20: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-00007e30: 6865 2073 6570 6172 6174 6f72 2075 7365  he separator use
-00007e40: 6420 746f 2063 6f6e 6361 7465 6e61 7465  d to concatenate
-00007e50: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
-00007e60: 2020 2020 2020 636f 6d6d 616e 6473 2e20        commands. 
-00007e70: 4465 6661 756c 7473 2074 6f20 2720 2626  Defaults to ' &&
-00007e80: 2027 2e0a 2020 2020 2020 2020 2020 2020   '..            
-00007e90: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
-00007ea0: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
-00007eb0: 756d 656e 7473 2e0a 0a20 2020 2020 2020  uments...       
-00007ec0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00007ed0: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
-00007ee0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
-00007ef0: 6c61 7374 2063 6f6d 6d61 6e64 2069 6e20  last command in 
-00007f00: 7468 6520 6c69 7374 2e0a 2020 2020 2020  the list..      
-00007f10: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00007f20: 2065 6e76 2069 7320 4e6f 6e65 3a0a 2020   env is None:.  
-00007f30: 2020 2020 2020 2020 2020 656e 7620 3d20            env = 
-00007f40: 7b7d 0a20 2020 2020 2020 2063 6d64 203d  {}.        cmd =
-00007f50: 2073 6570 2e6a 6f69 6e28 636d 646c 6973   sep.join(cmdlis
-00007f60: 7429 0a20 2020 2020 2020 206c 6f67 6765  t).        logge
-00007f70: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-00007f80: 2020 2020 6622 5275 6e6e 696e 6720 636f      f"Running co
-00007f90: 6d6d 616e 6473 2c20 7769 7468 2065 6e76  mmands, with env
-00007fa0: 207b 656e 767d 2061 6e64 2073 6570 207b   {env} and sep {
-00007fb0: 7365 707d 205c 0a20 2020 2020 2020 2020  sep} \.         
-00007fc0: 2020 2020 2020 2061 6e64 207b 6b77 6172         and {kwar
-00007fd0: 6773 7d3a 207b 636d 647d 2229 0a20 2020  gs}: {cmd}").   
-00007fe0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00007ff0: 6c66 2e72 756e 2863 6d64 2c20 656e 763d  lf.run(cmd, env=
-00008000: 656e 762c 202a 2a6b 7761 7267 7329 2020  env, **kwargs)  
-00008010: 2320 6f75 745f 7374 7265 616d 3d6f 7574  # out_stream=out
-00008020: 5f73 7472 6561 6d2c 0a0a 2020 2020 2020  _stream,..      
-00008030: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00008040: 2020 2023 2057 6174 6368 206f 7574 2066     # Watch out f
-00008050: 6f72 2055 6e69 636f 6465 456e 636f 6465  or UnicodeEncode
-00008060: 4572 726f 7220 7768 656e 2079 6f75 2073  Error when you s
-00008070: 7472 2829 2074 6869 732e 0a20 2020 2020  tr() this..     
-00008080: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00008090: 666f 2866 227b 7265 7375 6c74 2e73 7464  fo(f"{result.std
-000080a0: 6f75 747d 2229 0a20 2020 2020 2020 2065  out}").        e
-000080b0: 7863 6570 7420 556e 6963 6f64 6545 6e63  xcept UnicodeEnc
-000080c0: 6f64 6545 7272 6f72 2061 7320 653a 0a20  odeError as e:. 
-000080d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000080e0: 722e 6572 726f 7228 6622 556e 6963 6f64  r.error(f"Unicod
-000080f0: 6520 6572 726f 723a 207b 657d 2229 0a20  e error: {e}"). 
-00008100: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00008110: 4f3a 204f 4e4c 5920 7374 646f 7574 2052  O: ONLY stdout R
-00008120: 4543 4f44 4520 4e45 4544 4544 3f3f 206f  ECODE NEEDED?? o
-00008130: 7220 616c 736f 2065 7272 6f72 3f0a 2020  r also error?.  
-00008140: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008150: 2e73 7464 6f75 7420 3d20 7265 7375 6c74  .stdout = result
-00008160: 2e73 7464 6f75 742e 656e 636f 6465 280a  .stdout.encode(.
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2775 7466 2d38 272c 2027 6967 6e6f 7265  'utf-8', 'ignore
-00008190: 2729 2e64 6563 6f64 6528 2775 7466 2d38  ').decode('utf-8
-000081a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000081b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000081c0: 6620 7374 725f 746f 5f63 6c61 7373 2873  f str_to_class(s
-000081d0: 656c 662c 206d 6f64 756c 655f 6e61 6d65  elf, module_name
-000081e0: 3a20 7374 722c 2063 6c61 7373 5f6e 616d  : str, class_nam
-000081f0: 653a 2073 7472 2c20 2a61 7267 732c 202a  e: str, *args, *
-00008200: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00008210: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00008220: 7475 726e 2061 2063 6c61 7373 2069 6e73  turn a class ins
-00008230: 7461 6e63 6520 6672 6f6d 2061 2073 7472  tance from a str
-00008240: 696e 6720 7265 6665 7265 6e63 652e 0a0a  ing reference...
-00008250: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00008260: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
-00008270: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
-00008280: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-00008290: 756c 652e 0a20 2020 2020 2020 2020 2020  ule..           
-000082a0: 2063 6c61 7373 5f6e 616d 6520 2873 7472   class_name (str
-000082b0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
-000082c0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
-000082d0: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
-000082e0: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
-000082f0: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
-00008300: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
-00008310: 7275 6374 6f72 2e0a 2020 2020 2020 2020  ructor..        
-00008320: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
-00008330: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
-00008340: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-00008350: 6865 2063 6c61 7373 2063 6f6e 7374 7275  he class constru
-00008360: 6374 6f72 2e0a 0a20 2020 2020 2020 2052  ctor...        R
-00008370: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00008380: 2020 2020 6f62 6a65 6374 3a20 416e 2069      object: An i
-00008390: 6e73 7461 6e63 6520 6f66 2074 6865 2073  nstance of the s
-000083a0: 7065 6369 6669 6564 2063 6c61 7373 2c20  pecified class, 
-000083b0: 6f72 204e 6f6e 6520 6966 2074 6865 2063  or None if the c
-000083c0: 6c61 7373 206f 720a 2020 2020 2020 2020  lass or.        
-000083d0: 2020 2020 2020 2020 6d6f 6475 6c65 2064          module d
-000083e0: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
-000083f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008400: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00008410: 2020 2020 6d6f 6475 6c65 5f20 3d20 696d      module_ = im
-00008420: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
-00008430: 6f64 756c 6528 6d6f 6475 6c65 5f6e 616d  odule(module_nam
-00008440: 6529 0a20 2020 2020 2020 2020 2020 2074  e).            t
-00008450: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00008460: 2020 2020 636c 6173 735f 203d 2067 6574      class_ = get
-00008470: 6174 7472 286d 6f64 756c 655f 2c20 636c  attr(module_, cl
-00008480: 6173 735f 6e61 6d65 2928 2a61 7267 732c  ass_name)(*args,
-00008490: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-000084a0: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-000084b0: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
-000084c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000084d0: 6767 6572 2e65 7272 6f72 2827 436c 6173  gger.error('Clas
-000084e0: 7320 646f 6573 206e 6f74 2065 7869 7374  s does not exist
-000084f0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
-00008500: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-00008510: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00008520: 722e 6572 726f 7228 274d 6f64 756c 6520  r.error('Module 
-00008530: 646f 6573 206e 6f74 2065 7869 7374 2729  does not exist')
-00008540: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008550: 636c 6173 735f 206f 7220 4e6f 6e65 0a0a  class_ or None..
-00008560: 2020 2020 6465 6620 7275 6e5f 636f 6d6d      def run_comm
-00008570: 616e 6473 5f73 706c 6974 5f6f 7574 2873  ands_split_out(s
-00008580: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 636d 646c 6973 743a 204c 6973      cmdlist: Lis
-000085b0: 745b 7374 725d 2c0a 2020 2020 2020 2020  t[str],.        
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-000085e0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-000085f0: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00008620: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-00008630: 2020 2022 2222 5275 6e20 6120 6c69 7374     """Run a list
-00008640: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
-00008650: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
-00008660: 2061 6e64 2073 706c 6974 2074 6865 206f   and split the o
-00008670: 7574 7075 740a 2020 2020 2020 2020 6f66  utput.        of
-00008680: 2065 6163 6820 636f 6d6d 616e 642e 0a0a   each command...
-00008690: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
-000086a0: 6d61 6e64 2069 6e20 7468 6520 6c69 7374  mand in the list
-000086b0: 2069 7320 6578 6563 7574 6564 2077 6974   is executed wit
-000086c0: 6820 6120 7365 7061 7261 746f 7220 696e  h a separator in
-000086d0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
-000086e0: 2074 6861 7420 6973 2075 6e69 7175 6520   that is unique 
-000086f0: 616e 6420 6361 6e20 6265 2075 7365 6420  and can be used 
-00008700: 746f 2073 706c 6974 0a20 2020 2020 2020  to split.       
-00008710: 2074 6865 206f 7574 7075 7420 6f66 2065   the output of e
-00008720: 6163 6820 636f 6d6d 616e 6420 6c61 7465  ach command late
-00008730: 722e 2054 6865 2073 6570 6172 6174 6f72  r. The separator
-00008740: 2075 7365 6420 6973 2073 7065 6369 6669   used is specifi
-00008750: 6564 0a20 2020 2020 2020 2062 7920 7468  ed.        by th
-00008760: 6520 605f 4f55 545f 5345 5060 2061 7474  e `_OUT_SEP` att
-00008770: 7269 6275 7465 206f 6620 7468 650a 2020  ribute of the.  
-00008780: 2020 2020 2020 536c 7572 6d43 6c69 656e        SlurmClien
-00008790: 7420 696e 7374 616e 6365 2e0a 0a20 2020  t instance...   
-000087a0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000087b0: 2020 2020 2020 2063 6d64 6c69 7374 2028         cmdlist (
-000087c0: 4c69 7374 5b73 7472 5d29 3a20 4120 6c69  List[str]): A li
-000087d0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
-000087e0: 616e 6473 2074 6f20 7275 6e2e 0a20 2020  ands to run..   
-000087f0: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-00008800: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-00008810: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-00008820: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-00008830: 7269 6162 6c65 7320 0a20 2020 2020 2020  riables .       
-00008840: 2020 2020 2020 2020 2074 6f20 7365 7420           to set 
-00008850: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
-00008860: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
-00008870: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
-00008880: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00008890: 2020 2020 2020 2020 2020 4c69 7374 5b73            List[s
-000088a0: 7472 5d3a 0a20 2020 2020 2020 2020 2020  tr]:.           
-000088b0: 2020 2020 2041 206c 6973 7420 6f66 2073       A list of s
-000088c0: 7472 696e 6773 2c20 7768 6572 6520 6561  trings, where ea
-000088d0: 6368 2073 7472 696e 6720 636f 7272 6573  ch string corres
-000088e0: 706f 6e64 7320 746f 0a20 2020 2020 2020  ponds to.       
-000088f0: 2020 2020 2020 2020 2074 6865 206f 7574           the out
-00008900: 7075 7420 6f66 2061 2073 696e 676c 6520  put of a single 
-00008910: 636f 6d6d 616e 6420 696e 2060 636d 646c  command in `cmdl
-00008920: 6973 7460 2073 706c 6974 0a20 2020 2020  ist` split.     
-00008930: 2020 2020 2020 2020 2020 2062 7920 7468             by th
-00008940: 6520 7365 7061 7261 746f 7220 605f 4f55  e separator `_OU
-00008950: 545f 5345 5060 2e0a 0a20 2020 2020 2020  T_SEP`...       
-00008960: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00008970: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
-00008980: 6e3a 2049 6620 616e 7920 6f66 2074 6865  n: If any of the
-00008990: 2063 6f6d 6d61 6e64 7320 6661 696c 2074   commands fail t
-000089a0: 6f20 6578 6563 7574 6520 7375 6363 6573  o execute succes
-000089b0: 7366 756c 6c79 2e0a 2020 2020 2020 2020  sfully..        
-000089c0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
-000089d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000089e0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-000089f0: 6f6d 6d61 6e64 7328 636d 646c 6973 743d  ommands(cmdlist=
-00008a00: 636d 646c 6973 742c 0a20 2020 2020 2020  cmdlist,.       
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 656e 763d 656e 762c 0a20 2020 2020 2020  env=env,.       
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a60: 7365 703d 6622 203b 2065 6368 6f20 7b73  sep=f" ; echo {s
-00008a70: 656c 662e 5f4f 5554 5f53 4550 7d20 3b20  elf._OUT_SEP} ; 
-00008a80: 2229 0a20 2020 2020 2020 2065 7863 6570  ").        excep
-00008a90: 7420 556e 6578 7065 6374 6564 4578 6974  t UnexpectedExit
-00008aa0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00008ab0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00008ac0: 6728 6529 0a20 2020 2020 2020 2020 2020  g(e).           
-00008ad0: 2072 6573 756c 7420 3d20 652e 7265 7375   result = e.resu
-00008ae0: 6c74 0a20 2020 2020 2020 2069 6620 7265  lt.        if re
-00008af0: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
-00008b00: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-00008b10: 7265 7375 6c74 2e73 7464 6f75 740a 2020  result.stdout.  
-00008b20: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
-00008b30: 7265 7370 6f6e 7365 7320 3d20 7265 7370  responses = resp
-00008b40: 6f6e 7365 2e73 706c 6974 2873 656c 662e  onse.split(self.
-00008b50: 5f4f 5554 5f53 4550 290a 2020 2020 2020  _OUT_SEP).      
-00008b60: 2020 2020 2020 7265 7475 726e 2073 706c        return spl
-00008b70: 6974 5f72 6573 706f 6e73 6573 0a20 2020  it_responses.   
-00008b80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008b90: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
-00008ba0: 7265 7375 6c74 2069 7320 6e6f 7420 6f6b  result is not ok
-00008bb0: 2c20 6c6f 6720 7468 6520 6572 726f 7220  , log the error 
-00008bc0: 616e 6420 7261 6973 6520 616e 2053 5348  and raise an SSH
-00008bd0: 4578 6365 7074 696f 6e0a 2020 2020 2020  Exception.      
-00008be0: 2020 2020 2020 6572 726f 7220 3d20 6622        error = f"
-00008bf0: 5265 7375 6c74 2069 7320 6e6f 7420 6f6b  Result is not ok
-00008c00: 3a20 7b72 6573 756c 747d 220a 2020 2020  : {result}".    
-00008c10: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00008c20: 7272 6f72 2865 7272 6f72 290a 2020 2020  rror(error).    
-00008c30: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
-00008c40: 4845 7863 6570 7469 6f6e 2865 7272 6f72  HException(error
-00008c50: 290a 0a20 2020 2064 6566 206c 6973 745f  )..    def list_
-00008c60: 6163 7469 7665 5f6a 6f62 7328 7365 6c66  active_jobs(self
-00008c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008c80: 2020 2020 2020 2020 2020 2065 6e76 3a20             env: 
-00008c90: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00008ca0: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
-00008cb0: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-00008cc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008cd0: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
-00008ce0: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
-00008cf0: 6d20 534c 5552 4d2e 0a0a 2020 2020 2020  m SLURM...      
-00008d00: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00008d10: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
-00008d20: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-00008d30: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
-00008d40: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00008d50: 6573 2074 6f20 0a20 2020 2020 2020 2020  es to .         
-00008d60: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
-00008d70: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00008d80: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-00008d90: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00008da0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00008db0: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
-00008dc0: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
-00008dd0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00008de0: 2020 2020 2020 2023 2063 6d64 203d 2073         # cmd = s
-00008df0: 656c 662e 5f41 4354 4956 455f 4a4f 4253  elf._ACTIVE_JOBS
-00008e00: 5f43 4d44 0a20 2020 2020 2020 2063 6d64  _CMD.        cmd
-00008e10: 203d 2073 656c 662e 6765 745f 6a6f 6273   = self.get_jobs
-00008e20: 5f69 6e66 6f5f 636f 6d6d 616e 6428 7374  _info_command(st
-00008e30: 6172 745f 7469 6d65 3d22 6e6f 7722 2c20  art_time="now", 
-00008e40: 7374 6174 6573 3d22 7222 290a 2020 2020  states="r").    
-00008e50: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00008e60: 2252 6574 7269 6576 696e 6720 6c69 7374  "Retrieving list
-00008e70: 206f 6620 6163 7469 7665 206a 6f62 7320   of active jobs 
-00008e80: 6672 6f6d 2053 6c75 726d 2229 0a20 2020  from Slurm").   
-00008e90: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00008ea0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00008eb0: 5b63 6d64 5d2c 2065 6e76 3d65 6e76 290a  [cmd], env=env).
-00008ec0: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
-00008ed0: 203d 2072 6573 756c 742e 7374 646f 7574   = result.stdout
-00008ee0: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
-00008ef0: 5c6e 2729 0a20 2020 2020 2020 206a 6f62  \n').        job
-00008f00: 5f6c 6973 742e 7265 7665 7273 6528 290a  _list.reverse().
-00008f10: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-00008f20: 6f62 5f6c 6973 740a 0a20 2020 2064 6566  ob_list..    def
-00008f30: 206c 6973 745f 636f 6d70 6c65 7465 645f   list_completed_
-00008f40: 6a6f 6273 2873 656c 662c 0a20 2020 2020  jobs(self,.     
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f60: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00008f70: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00008f80: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-00008f90: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-00008fa0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00008fb0: 6574 2061 206c 6973 7420 6f66 2063 6f6d  et a list of com
-00008fc0: 706c 6574 6564 206a 6f62 7320 6672 6f6d  pleted jobs from
-00008fd0: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
-00008fe0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00008ff0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-00009000: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-00009010: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-00009020: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00009030: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
-00009040: 2020 2020 2073 6574 2077 6865 6e20 7275       set when ru
-00009050: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-00009060: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
-00009070: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
-00009080: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00009090: 2020 204c 6973 745b 7374 725d 3a20 4120     List[str]: A 
-000090a0: 6c69 7374 206f 6620 6a6f 6220 4944 732e  list of job IDs.
-000090b0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-000090c0: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-000090d0: 2e67 6574 5f6a 6f62 735f 696e 666f 5f63  .get_jobs_info_c
-000090e0: 6f6d 6d61 6e64 2873 7461 7465 733d 2263  ommand(states="c
-000090f0: 6422 290a 2020 2020 2020 2020 6c6f 6767  d").        logg
-00009100: 6572 2e69 6e66 6f28 2252 6574 7269 6576  er.info("Retriev
-00009110: 696e 6720 6120 6c69 7374 206f 6620 636f  ing a list of co
-00009120: 6d70 6c65 7465 6420 6a6f 6273 2066 726f  mpleted jobs fro
-00009130: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
-00009140: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00009150: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-00009160: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-00009170: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
-00009180: 5b6a 6f62 2e73 7472 6970 2829 2066 6f72  [job.strip() for
-00009190: 206a 6f62 2069 6e20 7265 7375 6c74 2e73   job in result.s
-000091a0: 7464 6f75 742e 7374 7269 7028 292e 7370  tdout.strip().sp
-000091b0: 6c69 7428 275c 6e27 295d 0a20 2020 2020  lit('\n')].     
-000091c0: 2020 206a 6f62 5f6c 6973 742e 7265 7665     job_list.reve
-000091d0: 7273 6528 290a 2020 2020 2020 2020 7265  rse().        re
-000091e0: 7475 726e 206a 6f62 5f6c 6973 740a 0a20  turn job_list.. 
-000091f0: 2020 2064 6566 206c 6973 745f 616c 6c5f     def list_all_
-00009200: 6a6f 6273 2873 656c 662c 2065 6e76 3a20  jobs(self, env: 
-00009210: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00009220: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
-00009230: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-00009240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009250: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
-00009260: 2061 6c6c 206a 6f62 7320 6672 6f6d 2053   all jobs from S
-00009270: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
-00009280: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00009290: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
-000092a0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-000092b0: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
-000092c0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092e0: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
-000092f0: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
-00009300: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00009310: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
-00009320: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00009330: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
-00009340: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
-00009350: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00009360: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
-00009370: 6765 745f 6a6f 6273 5f69 6e66 6f5f 636f  get_jobs_info_co
-00009380: 6d6d 616e 6428 290a 2020 2020 2020 2020  mmand().        
-00009390: 6c6f 6767 6572 2e69 6e66 6f28 2252 6574  logger.info("Ret
-000093a0: 7269 6576 696e 6720 6120 6c69 7374 206f  rieving a list o
-000093b0: 6620 616c 6c20 6a6f 6273 2066 726f 6d20  f all jobs from 
-000093c0: 536c 7572 6d22 290a 2020 2020 2020 2020  Slurm").        
-000093d0: 7265 7375 6c74 203d 2073 656c 662e 7275  result = self.ru
-000093e0: 6e5f 636f 6d6d 616e 6473 285b 636d 645d  n_commands([cmd]
-000093f0: 2c20 656e 763d 656e 7629 0a20 2020 2020  , env=env).     
-00009400: 2020 206a 6f62 5f6c 6973 7420 3d20 7265     job_list = re
-00009410: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
-00009420: 7028 292e 7370 6c69 7428 275c 6e27 290a  p().split('\n').
-00009430: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
-00009440: 2e72 6576 6572 7365 2829 0a20 2020 2020  .reverse().     
-00009450: 2020 2072 6574 7572 6e20 6a6f 625f 6c69     return job_li
-00009460: 7374 0a0a 2020 2020 6465 6620 6765 745f  st..    def get_
-00009470: 6a6f 6273 5f69 6e66 6f5f 636f 6d6d 616e  jobs_info_comman
-00009480: 6428 7365 6c66 2c20 7374 6172 745f 7469  d(self, start_ti
-00009490: 6d65 3a20 7374 7220 3d20 2232 3032 332d  me: str = "2023-
-000094a0: 3031 2d30 3122 2c0a 2020 2020 2020 2020  01-01",.        
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 656e 645f 7469 6d65 3a20        end_time: 
-000094d0: 7374 7220 3d20 226e 6f77 222c 0a20 2020  str = "now",.   
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00009500: 6e73 3a20 7374 7220 3d20 224a 6f62 4964  ns: str = "JobId
-00009510: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009530: 2073 7461 7465 733a 2073 7472 203d 2022   states: str = "
-00009540: 722c 6364 2c66 2c74 6f2c 7273 2c64 6c2c  r,cd,f,to,rs,dl,
-00009550: 6e66 2229 202d 3e20 7374 723a 0a20 2020  nf") -> str:.   
-00009560: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00009570: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
-00009580: 2074 6f20 7265 7472 6965 7665 2069 6e66   to retrieve inf
-00009590: 6f72 6d61 7469 6f6e 2061 626f 7574 206f  ormation about o
-000095a0: 6c64 206a 6f62 732e 0a0a 2020 2020 2020  ld jobs...      
-000095b0: 2020 5468 6520 636f 6d6d 616e 6420 7769    The command wi
-000095c0: 6c6c 2062 6520 666f 726d 6174 7465 6420  ll be formatted 
-000095d0: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
-000095e0: 6564 2073 7461 7274 2074 696d 652c 2077  ed start time, w
-000095f0: 6869 6368 2069 730a 2020 2020 2020 2020  hich is.        
-00009600: 6578 7065 6374 6564 2074 6f20 6265 2069  expected to be i
-00009610: 6e20 7468 6520 4953 4f20 666f 726d 6174  n the ISO format
-00009620: 2022 5959 5959 2d4d 4d2d 4444 222e 0a20   "YYYY-MM-DD".. 
-00009630: 2020 2020 2020 2054 6865 2063 6f6d 6d61         The comma
-00009640: 6e64 2077 696c 6c20 7573 6520 7468 6520  nd will use the 
-00009650: 2273 6163 6374 2220 746f 6f6c 2074 6f20  "sacct" tool to 
-00009660: 7175 6572 7920 7468 650a 2020 2020 2020  query the.      
-00009670: 2020 536c 7572 6d20 6163 636f 756e 7469    Slurm accounti
-00009680: 6e67 2064 6174 6162 6173 6520 666f 7220  ng database for 
-00009690: 6a6f 6273 2074 6861 7420 7374 6172 7465  jobs that starte
-000096a0: 6420 6f6e 206f 7220 6166 7465 7220 7468  d on or after th
-000096b0: 650a 2020 2020 2020 2020 7370 6563 6966  e.        specif
-000096c0: 6965 6420 7374 6172 7420 7469 6d65 2c20  ied start time, 
-000096d0: 616e 6420 7769 6c6c 206f 7574 7075 7420  and will output 
-000096e0: 6f6e 6c79 2074 6865 206a 6f62 2049 4473  only the job IDs
-000096f0: 2028 2d6f 204a 6f62 4964 290a 2020 2020   (-o JobId).    
-00009700: 2020 2020 7769 7468 6f75 7420 6865 6164      without head
-00009710: 6572 206f 7220 7472 6169 6c65 7220 6c69  er or trailer li
-00009720: 6e65 7320 282d 6e20 2d58 292e 0a0a 2020  nes (-n -X)...  
-00009730: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009740: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
-00009750: 6d65 2028 7374 7229 3a20 5468 6520 7374  me (str): The st
-00009760: 6172 7420 7469 6d65 2066 726f 6d20 7768  art time from wh
-00009770: 6963 6820 746f 2072 6574 7269 6576 6520  ich to retrieve 
-00009780: 6a6f 620a 2020 2020 2020 2020 2020 2020  job.            
-00009790: 2020 2020 696e 666f 726d 6174 696f 6e2e      information.
-000097a0: 2044 6566 6175 6c74 7320 746f 2022 3230   Defaults to "20
-000097b0: 3233 2d30 312d 3031 222e 0a20 2020 2020  23-01-01"..     
-000097c0: 2020 2020 2020 2065 6e64 5f74 696d 6520         end_time 
-000097d0: 2873 7472 293a 2054 6865 2065 6e64 2074  (str): The end t
-000097e0: 696d 6520 756e 7469 6c20 7768 6963 6820  ime until which 
-000097f0: 746f 2072 6574 7269 6576 6520 6a6f 620a  to retrieve job.
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 696e 666f 726d 6174 696f 6e2e 2044 6566  information. Def
-00009820: 6175 6c74 7320 746f 2022 6e6f 7722 2e0a  aults to "now"..
-00009830: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00009840: 6d6e 7320 2873 7472 293a 2054 6865 2063  mns (str): The c
-00009850: 6f6c 756d 6e73 2074 6f20 7265 7472 6965  olumns to retrie
-00009860: 7665 2066 726f 6d20 7468 6520 6a6f 6220  ve from the job 
-00009870: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-00009880: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00009890: 6175 6c74 7320 746f 2022 4a6f 6249 6422  aults to "JobId"
-000098a0: 2e20 4974 2069 7320 636f 6d6d 6120 7365  . It is comma se
-000098b0: 7061 7261 7465 642c 2065 2e67 2e20 224a  parated, e.g. "J
-000098c0: 6f62 4964 2c53 7461 7465 222e 0a20 2020  obId,State"..   
-000098d0: 2020 2020 2020 2020 2073 7461 7465 7320           states 
-000098e0: 2873 7472 293a 2054 6865 206a 6f62 2073  (str): The job s
-000098f0: 7461 7465 7320 746f 2069 6e63 6c75 6465  tates to include
-00009900: 2069 6e20 7468 6520 7175 6572 792e 0a20   in the query.. 
-00009910: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00009920: 6566 6175 6c74 7320 746f 2022 722c 6364  efaults to "r,cd
-00009930: 2c66 2c74 6f2c 7273 2c64 6c2c 6e66 222e  ,f,to,rs,dl,nf".
-00009940: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00009950: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00009960: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
-00009970: 2020 2020 4120 7374 7269 6e67 2072 6570      A string rep
-00009980: 7265 7365 6e74 696e 6720 7468 6520 536c  resenting the Sl
-00009990: 7572 6d20 636f 6d6d 616e 6420 746f 2072  urm command to r
-000099a0: 6574 7269 6576 650a 2020 2020 2020 2020  etrieve.        
-000099b0: 2020 2020 2020 2020 696e 666f 726d 6174          informat
-000099c0: 696f 6e20 6162 6f75 7420 6f6c 6420 6a6f  ion about old jo
-000099d0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
-000099e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000099f0: 656c 662e 5f41 4c4c 5f4a 4f42 535f 434d  elf._ALL_JOBS_CM
-00009a00: 442e 666f 726d 6174 2873 7461 7274 5f74  D.format(start_t
-00009a10: 696d 653d 7374 6172 745f 7469 6d65 2c0a  ime=start_time,.
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
-00009a50: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2073 7461 7465 733d 7374 6174       states=stat
-00009a90: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00009ac0: 756d 6e73 3d63 6f6c 756d 6e73 290a 0a20  umns=columns).. 
-00009ad0: 2020 2064 6566 2074 7261 6e73 6665 725f     def transfer_
-00009ae0: 6461 7461 2873 656c 662c 206c 6f63 616c  data(self, local
-00009af0: 5f70 6174 683a 2073 7472 2920 2d3e 2052  _path: str) -> R
-00009b00: 6573 756c 743a 0a20 2020 2020 2020 2022  esult:.        "
-00009b10: 2222 0a20 2020 2020 2020 2054 7261 6e73  "".        Trans
-00009b20: 6665 7273 2061 2066 696c 6520 6f72 2064  fers a file or d
-00009b30: 6972 6563 746f 7279 2066 726f 6d20 7468  irectory from th
-00009b40: 6520 6c6f 6361 6c20 6d61 6368 696e 6520  e local machine 
-00009b50: 746f 2074 6865 2072 656d 6f74 650a 2020  to the remote.  
-00009b60: 2020 2020 2020 536c 7572 6d20 636c 7573        Slurm clus
-00009b70: 7465 722e 0a0a 2020 2020 2020 2020 4172  ter...        Ar
-00009b80: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00009b90: 6c6f 6361 6c5f 7061 7468 2028 7374 7229  local_path (str)
-00009ba0: 3a20 5468 6520 6c6f 6361 6c20 7061 7468  : The local path
-00009bb0: 2074 6f20 7468 6520 6669 6c65 206f 7220   to the file or 
-00009bc0: 6469 7265 6374 6f72 7920 746f 0a20 2020  directory to.   
-00009bd0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00009be0: 6e73 6665 722e 0a0a 2020 2020 2020 2020  nsfer...        
-00009bf0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00009c00: 2020 2020 2052 6573 756c 743a 2054 6865       Result: The
-00009c10: 2072 6573 756c 7420 6f66 2074 6865 2066   result of the f
-00009c20: 696c 6520 7472 616e 7366 6572 206f 7065  ile transfer ope
-00009c30: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00009c40: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00009c50: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
-00009c60: 2020 2020 2066 2254 7261 6e73 6665 7269       f"Transferi
-00009c70: 6e67 2066 696c 6520 7b6c 6f63 616c 5f70  ng file {local_p
-00009c80: 6174 687d 2074 6f20 7b73 656c 662e 736c  ath} to {self.sl
-00009c90: 7572 6d5f 6461 7461 5f70 6174 687d 2229  urm_data_path}")
-00009ca0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009cb0: 7365 6c66 2e70 7574 286c 6f63 616c 3d6c  self.put(local=l
-00009cc0: 6f63 616c 5f70 6174 682c 2072 656d 6f74  ocal_path, remot
-00009cd0: 653d 7365 6c66 2e73 6c75 726d 5f64 6174  e=self.slurm_dat
-00009ce0: 615f 7061 7468 290a 0a20 2020 2064 6566  a_path)..    def
-00009cf0: 2075 6e70 6163 6b5f 6461 7461 2873 656c   unpack_data(sel
-00009d00: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
-00009d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d20: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
-00009d30: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
-00009d40: 5d5d 203d 204e 6f6e 6529 202d 3e20 5265  ]] = None) -> Re
-00009d50: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
-00009d60: 220a 2020 2020 2020 2020 556e 7061 636b  ".        Unpack
-00009d70: 7320 6120 7a69 7070 6564 2066 696c 6520  s a zipped file 
-00009d80: 6f6e 2074 6865 2072 656d 6f74 6520 536c  on the remote Sl
-00009d90: 7572 6d20 636c 7573 7465 722e 0a0a 2020  urm cluster...  
-00009da0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009db0: 2020 2020 2020 2020 7a69 7066 696c 6520          zipfile 
-00009dc0: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
-00009dd0: 6f66 2074 6865 207a 6970 7065 6420 6669  of the zipped fi
-00009de0: 6c65 2074 6f20 6265 2075 6e70 6163 6b65  le to be unpacke
-00009df0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00009e00: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
-00009e10: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-00009e20: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
-00009e30: 6d65 6e74 2076 6172 6961 626c 6573 200a  ment variables .
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 746f 2073 6574 2077 6865 6e20 7275 6e6e  to set when runn
-00009e60: 696e 6720 7468 6520 636f 6d6d 616e 642e  ing the command.
-00009e70: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00009e80: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00009e90: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00009ea0: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
-00009eb0: 756c 7420 6f66 2074 6865 2063 6f6d 6d61  ult of the comma
-00009ec0: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
-00009ed0: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00009ee0: 6c66 2e67 6574 5f75 6e7a 6970 5f63 6f6d  lf.get_unzip_com
-00009ef0: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
-00009f00: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00009f10: 6f28 6622 556e 7061 636b 696e 6720 7b7a  o(f"Unpacking {z
-00009f20: 6970 6669 6c65 7d20 6f6e 2053 6c75 726d  ipfile} on Slurm
-00009f30: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00009f40: 6e20 7365 6c66 2e72 756e 5f63 6f6d 6d61  n self.run_comma
-00009f50: 6e64 7328 5b63 6d64 5d2c 2065 6e76 3d65  nds([cmd], env=e
-00009f60: 6e76 290a 0a20 2020 2064 6566 2063 6f6e  nv)..    def con
-00009f70: 7665 7274 5f64 6174 6128 7365 6c66 2c20  vert_data(self, 
-00009f80: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 2020 2065 6e76 3a20 4f70 7469 6f6e 616c     env: Optional
-00009fb0: 5b44 6963 745b 7374 722c 2073 7472 5d5d  [Dict[str, str]]
-00009fc0: 203d 204e 6f6e 6529 202d 3e20 5265 7375   = None) -> Resu
-00009fd0: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
-00009fe0: 2020 2020 2020 2020 556e 7061 636b 7320          Unpacks 
-00009ff0: 6120 7a69 7070 6564 2066 696c 6520 6f6e  a zipped file on
-0000a000: 2074 6865 2072 656d 6f74 6520 536c 7572   the remote Slur
-0000a010: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
-0000a020: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000a030: 2020 2020 2020 7a69 7066 696c 6520 2873        zipfile (s
-0000a040: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-0000a050: 2074 6865 207a 6970 7065 6420 6669 6c65   the zipped file
-0000a060: 2074 6f20 6265 2075 6e70 6163 6b65 642e   to be unpacked.
-0000a070: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-0000a080: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
-0000a090: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
-0000a0a0: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
-0000a0b0: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000a0d0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
-0000a0e0: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
-0000a0f0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-0000a100: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000a110: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-0000a120: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
-0000a130: 7420 6f66 2074 6865 2063 6f6d 6d61 6e64  t of the command
-0000a140: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000a150: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-0000a160: 2e67 6574 5f63 6f6e 7665 7274 5f63 6f6d  .get_convert_com
-0000a170: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
-0000a180: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-0000a190: 6f28 6622 436f 6e76 6572 7469 6e67 207b  o(f"Converting {
-0000a1a0: 7a69 7066 696c 657d 206f 6e20 536c 7572  zipfile} on Slur
-0000a1b0: 6d22 290a 2020 2020 2020 2020 7265 7475  m").        retu
-0000a1c0: 726e 2073 656c 662e 7275 6e5f 636f 6d6d  rn self.run_comm
-0000a1d0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
-0000a1e0: 656e 7629 0a0a 2020 2020 6465 6620 6765  env)..    def ge
-0000a1f0: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
-0000a200: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7365  _for_workflow(se
-0000a210: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000a240: 666c 6f77 3a20 7374 722c 0a20 2020 2020  flow: str,.     
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2073 7562 7374 6974 7574 6573 3a20     substitutes: 
-0000a280: 4469 6374 5b73 7472 2c20 7374 725d 2c0a  Dict[str, str],.
-0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
+00006980: 5f70 6172 616d 733d 736c 7572 6d5f 6d6f  _params=slurm_mo
+00006990: 6465 6c5f 6a6f 6273 5f70 6172 616d 732c  del_jobs_params,
+000069a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069b0: 2020 2020 736c 7572 6d5f 7363 7269 7074      slurm_script
+000069c0: 5f70 6174 683d 736c 7572 6d5f 7363 7269  _path=slurm_scri
+000069d0: 7074 5f70 6174 682c 0a20 2020 2020 2020  pt_path,.       
+000069e0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+000069f0: 6d5f 7363 7269 7074 5f72 6570 6f3d 736c  m_script_repo=sl
+00006a00: 7572 6d5f 7363 7269 7074 5f72 6570 6f2c  urm_script_repo,
+00006a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a20: 2020 2020 696e 6974 5f73 6c75 726d 3d69      init_slurm=i
+00006a30: 6e69 745f 736c 7572 6d29 0a0a 2020 2020  nit_slurm)..    
+00006a40: 6465 6620 636c 6561 6e75 705f 746d 705f  def cleanup_tmp_
+00006a50: 6669 6c65 7328 7365 6c66 2c0a 2020 2020  files(self,.    
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
+00006a80: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
+00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006aa0: 2020 2066 696c 656e 616d 653a 2073 7472     filename: str
+00006ab0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ad0: 2020 2064 6174 615f 6c6f 6361 7469 6f6e     data_location
+00006ae0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 2020 2020 2020 2020 6c6f 6766 696c 653a          logfile:
+00006b10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b30: 2020 2020 2020 2029 202d 3e20 5265 7375         ) -> Resu
+00006b40: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
+00006b50: 2020 2020 2020 2020 436c 6561 6e75 7020          Cleanup 
+00006b60: 7a69 7020 616e 6420 756e 7a69 7070 6564  zip and unzipped
+00006b70: 2066 696c 6573 2f66 6f6c 6465 7273 2061   files/folders a
+00006b80: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
+00006b90: 2053 6c75 726d 206a 6f62 2e0a 0a20 2020   Slurm job...   
+00006ba0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00006bb0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
+00006bc0: 5f69 6420 2873 7472 293a 2054 6865 206a  _id (str): The j
+00006bd0: 6f62 2049 4420 6f66 2074 6865 2053 6c75  ob ID of the Slu
+00006be0: 726d 2073 6372 6970 742e 0a20 2020 2020  rm script..     
+00006bf0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+00006c00: 2873 7472 293a 2054 6865 207a 6970 2066  (str): The zip f
+00006c10: 696c 656e 616d 6520 6f6e 2053 6c75 726d  ilename on Slurm
+00006c20: 2e0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00006c30: 7461 5f6c 6f63 6174 696f 6e20 2873 7472  ta_location (str
+00006c40: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00006c50: 206c 6f63 6174 696f 6e20 6f66 2064 6174   location of dat
+00006c60: 6120 6669 6c65 7320 6f6e 2053 6c75 726d  a files on Slurm
+00006c70: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006c80: 2020 4966 206e 6f74 2070 726f 7669 6465    If not provide
+00006c90: 642c 2069 7420 7769 6c6c 2062 6520 6578  d, it will be ex
+00006ca0: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
+00006cb0: 206c 6f67 2066 696c 652e 0a20 2020 2020   log file..     
+00006cc0: 2020 2020 2020 206c 6f67 6669 6c65 2028         logfile (
+00006cd0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00006ce0: 5468 6520 6c6f 6720 6669 6c65 206f 6620  The log file of 
+00006cf0: 7468 6520 536c 7572 6d20 6a6f 622e 200a  the Slurm job. .
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 4966 206e 6f74 2070 726f 7669 6465 642c  If not provided,
+00006d20: 2061 2064 6566 6175 6c74 206c 6f67 2066   a default log f
+00006d30: 696c 6520 7769 6c6c 2062 6520 7573 6564  ile will be used
+00006d40: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00006d50: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00006d60: 5265 7375 6c74 3a20 5468 6520 7265 7375  Result: The resu
+00006d70: 6c74 206f 6620 7468 6520 636c 6561 6e75  lt of the cleanu
+00006d80: 7020 6f70 6572 6174 696f 6e2e 0a0a 2020  p operation...  
+00006d90: 2020 2020 2020 4e6f 7465 3a0a 2020 2020        Note:.    
+00006da0: 2020 2020 2020 2020 5468 6520 636c 6561          The clea
+00006db0: 6e75 7020 7072 6f63 6573 7320 696e 766f  nup process invo
+00006dc0: 6c76 6573 2072 656d 6f76 696e 6720 7468  lves removing th
+00006dd0: 6520 7370 6563 6966 6965 6420 7a69 7020  e specified zip 
+00006de0: 6669 6c65 2c20 0a20 2020 2020 2020 2020  file, .         
+00006df0: 2020 2074 6865 206c 6f67 2066 696c 652c     the log file,
+00006e00: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+00006e10: 6461 7461 2066 696c 6573 2061 6e64 2066  data files and f
+00006e20: 6f6c 6465 7273 2e0a 0a20 2020 2020 2020  olders...       
+00006e30: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00006e40: 2020 2020 2020 2320 436c 6561 6e75 7020        # Cleanup 
+00006e50: 7465 6d70 6f72 6172 7920 6669 6c65 7320  temporary files 
+00006e60: 666f 7220 6120 536c 7572 6d20 6a6f 620a  for a Slurm job.
+00006e70: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00006e80: 6e74 2e63 6c65 616e 7570 5f74 6d70 5f66  nt.cleanup_tmp_f
+00006e90: 696c 6573 2822 3132 3334 3522 2c20 226f  iles("12345", "o
+00006ea0: 7574 7075 742e 7a69 7022 290a 2020 2020  utput.zip").    
+00006eb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006ec0: 636d 6473 203d 205b 5d0a 2020 2020 2020  cmds = [].      
+00006ed0: 2020 2320 7a69 700a 2020 2020 2020 2020    # zip.        
+00006ee0: 6966 2066 696c 656e 616d 653a 0a20 2020  if filename:.   
+00006ef0: 2020 2020 2020 2020 2072 6d7a 6970 203d           rmzip =
+00006f00: 2066 2272 6d20 7b66 696c 656e 616d 657d   f"rm {filename}
+00006f10: 2e2a 220a 2020 2020 2020 2020 2020 2020  .*".            
+00006f20: 636d 6473 2e61 7070 656e 6428 726d 7a69  cmds.append(rmzi
+00006f30: 7029 0a20 2020 2020 2020 2023 206c 6f67  p).        # log
+00006f40: 0a20 2020 2020 2020 2069 6620 6c6f 6766  .        if logf
+00006f50: 696c 6520 6973 204e 6f6e 653a 0a20 2020  ile is None:.   
+00006f60: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00006f70: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
+00006f80: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00006f90: 6669 6c65 203d 206c 6f67 6669 6c65 2e66  file = logfile.f
+00006fa0: 6f72 6d61 7428 736c 7572 6d5f 6a6f 625f  ormat(slurm_job_
+00006fb0: 6964 3d73 6c75 726d 5f6a 6f62 5f69 6429  id=slurm_job_id)
+00006fc0: 0a20 2020 2020 2020 2072 6d6c 6f67 203d  .        rmlog =
+00006fd0: 2066 2272 6d20 7b6c 6f67 6669 6c65 7d22   f"rm {logfile}"
+00006fe0: 0a20 2020 2020 2020 2063 6d64 732e 6170  .        cmds.ap
+00006ff0: 7065 6e64 2872 6d6c 6f67 290a 2020 2020  pend(rmlog).    
+00007000: 2020 2020 2320 636f 6e76 6572 7465 7220      # converter 
+00007010: 6c6f 6773 0a20 2020 2020 2020 2063 6c6f  logs.        clo
+00007020: 6720 3d20 7365 6c66 2e5f 434f 4e56 4552  g = self._CONVER
+00007030: 5445 525f 4c4f 4746 494c 450a 2020 2020  TER_LOGFILE.    
+00007040: 2020 2020 636c 6f67 203d 2063 6c6f 672e      clog = clog.
+00007050: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
+00007060: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
+00007070: 290a 2020 2020 2020 2020 726d 636c 6f67  ).        rmclog
+00007080: 203d 2066 2272 6d20 7b63 6c6f 677d 220a   = f"rm {clog}".
+00007090: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
+000070a0: 656e 6428 726d 636c 6f67 290a 2020 2020  end(rmclog).    
+000070b0: 2020 2020 0a20 2020 2020 2020 2023 2064      .        # d
+000070c0: 6174 610a 2020 2020 2020 2020 6966 2064  ata.        if d
+000070d0: 6174 615f 6c6f 6361 7469 6f6e 2069 7320  ata_location is 
+000070e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000070f0: 2020 6461 7461 5f6c 6f63 6174 696f 6e20    data_location 
+00007100: 3d20 7365 6c66 2e65 7874 7261 6374 5f64  = self.extract_d
+00007110: 6174 615f 6c6f 6361 7469 6f6e 5f66 726f  ata_location_fro
+00007120: 6d5f 6c6f 6728 6c6f 6766 696c 6529 0a20  m_log(logfile). 
+00007130: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00007140: 2020 2020 6966 2064 6174 615f 6c6f 6361      if data_loca
+00007150: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00007160: 2020 726d 6461 7461 203d 2066 2272 6d20    rmdata = f"rm 
+00007170: 2d72 6620 7b64 6174 615f 6c6f 6361 7469  -rf {data_locati
+00007180: 6f6e 7d20 7b64 6174 615f 6c6f 6361 7469  on} {data_locati
+00007190: 6f6e 7d2e 2a22 0a20 2020 2020 2020 2020  on}.*".         
+000071a0: 2020 2063 6d64 732e 6170 7065 6e64 2872     cmds.append(r
+000071b0: 6d64 6174 6129 0a20 2020 2020 2020 2020  mdata).         
+000071c0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+000071d0: 2320 636f 6e76 6572 7420 636f 6e66 6967  # convert config
+000071e0: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+000071f0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
+00007200: 6622 636f 6e66 6967 5f7b 6f73 2e70 6174  f"config_{os.pat
+00007210: 682e 6261 7365 6e61 6d65 2864 6174 615f  h.basename(data_
+00007220: 6c6f 6361 7469 6f6e 297d 2e74 7874 220a  location)}.txt".
+00007230: 2020 2020 2020 2020 2020 2020 726d 636f              rmco
+00007240: 6e66 6967 203d 2066 2272 6d20 7b63 6f6e  nfig = f"rm {con
+00007250: 6669 675f 6669 6c65 7d22 0a20 2020 2020  fig_file}".     
+00007260: 2020 2020 2020 2063 6d64 732e 6170 7065         cmds.appe
+00007270: 6e64 2872 6d63 6f6e 6669 6729 0a20 2020  nd(rmconfig).   
+00007280: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00007290: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+000072a0: 726e 696e 6728 6622 436f 756c 6420 6e6f  rning(f"Could no
+000072b0: 7420 6578 7472 6163 7420 6461 7461 206c  t extract data l
+000072c0: 6f63 6174 696f 6e20 6672 6f6d 206c 6f67  ocation from log
+000072d0: 207b 6c6f 6766 696c 657d 2e20 536b 6970   {logfile}. Skip
+000072e0: 7069 6e67 2063 6c65 616e 7570 2e22 290a  ping cleanup.").
+000072f0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00007300: 2020 2020 2020 2020 2020 2320 646f 2061            # do a
+00007310: 7320 6d75 6368 2061 7320 706f 7373 6962  s much as possib
+00007320: 6c65 2c20 6e6f 7420 636f 6e64 6974 696f  le, not conditio
+00007330: 6e61 6c20 7265 6d6f 7661 6c0a 2020 2020  nal removal.    
+00007340: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00007350: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00007360: 6473 2863 6d64 732c 2073 6570 3d27 203b  ds(cmds, sep=' ;
+00007370: 2027 290a 2020 2020 2020 2020 6578 6365   ').        exce
+00007380: 7074 2055 6e65 7870 6563 7465 6445 7869  pt UnexpectedExi
+00007390: 7420 6173 2065 3a0a 2020 2020 2020 2020  t as e:.        
+000073a0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+000073b0: 6e67 2865 290a 2020 2020 2020 2020 2020  ng(e).          
+000073c0: 2020 7265 7375 6c74 203d 2065 2e72 6573    result = e.res
+000073d0: 756c 740a 2020 2020 2020 2020 7265 7475  ult.        retu
+000073e0: 726e 2072 6573 756c 7420 6f72 204e 6f6e  rn result or Non
+000073f0: 650a 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
+00007400: 6174 6528 7365 6c66 2c20 7661 6c69 6461  ate(self, valida
+00007410: 7465 5f73 6c75 726d 5f73 6574 7570 3a20  te_slurm_setup: 
+00007420: 626f 6f6c 203d 2046 616c 7365 293a 0a20  bool = False):. 
+00007430: 2020 2020 2020 2022 2222 5661 6c69 6461         """Valida
+00007440: 7465 2074 6865 2063 6f6e 6e65 6374 696f  te the connectio
+00007450: 6e20 746f 2074 6865 2053 6c75 726d 2063  n to the Slurm c
+00007460: 6c75 7374 6572 2062 7920 7275 6e6e 696e  luster by runnin
+00007470: 670a 2020 2020 2020 2020 6120 7369 6d70  g.        a simp
+00007480: 6c65 2063 6f6d 6d61 6e64 2e0a 0a20 2020  le command...   
+00007490: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000074a0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
+000074b0: 736c 7572 6d5f 7365 7475 7020 2862 6f6f  slurm_setup (boo
+000074c0: 6c29 3a20 5768 6574 6865 7220 746f 2061  l): Whether to a
+000074d0: 6c73 6f20 6368 6563 6b0a 2020 2020 2020  lso check.      
+000074e0: 2020 2020 2020 2020 2020 616e 6420 6669            and fi
+000074f0: 7820 7468 6520 536c 7572 6d20 7365 7475  x the Slurm setu
+00007500: 7020 2866 6f6c 6465 7273 2c20 696d 6167  p (folders, imag
+00007510: 6573 2c20 6574 632e 290a 0a20 2020 2020  es, etc.)..     
+00007520: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00007530: 2020 2020 2020 2020 626f 6f6c 3a0a 2020          bool:.  
+00007540: 2020 2020 2020 2020 2020 2020 2020 5472                Tr
+00007550: 7565 2069 6620 7468 6520 7661 6c69 6461  ue if the valida
+00007560: 7469 6f6e 2069 7320 7375 6363 6573 7366  tion is successf
+00007570: 756c 2c0a 2020 2020 2020 2020 2020 2020  ul,.            
+00007580: 2020 2020 4661 6c73 6520 6f74 6865 7277      False otherw
+00007590: 6973 652e 0a20 2020 2020 2020 2022 2222  ise..        """
+000075a0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+000075b0: 6564 203d 2073 656c 662e 7275 6e28 2765  ed = self.run('e
+000075c0: 6368 6f20 2220 2227 292e 6f6b 0a20 2020  cho " "').ok.   
+000075d0: 2020 2020 2069 6620 636f 6e6e 6563 7465       if connecte
+000075e0: 6420 616e 6420 7661 6c69 6461 7465 5f73  d and validate_s
+000075f0: 6c75 726d 5f73 6574 7570 3a0a 2020 2020  lurm_setup:.    
+00007600: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00007610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007620: 662e 7365 7475 705f 736c 7572 6d28 290a  f.setup_slurm().
+00007630: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00007640: 7074 2053 5348 4578 6365 7074 696f 6e20  pt SSHException 
+00007650: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00007660: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+00007670: 6f72 2865 290a 2020 2020 2020 2020 2020  or(e).          
+00007680: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00007690: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
+000076a0: 6e20 636f 6e6e 6563 7465 640a 0a20 2020  n connected..   
+000076b0: 2064 6566 2067 6574 5f72 6563 656e 745f   def get_recent_
+000076c0: 6c6f 675f 636f 6d6d 616e 6428 7365 6c66  log_command(self
+000076d0: 2c20 6c6f 675f 6669 6c65 3a20 7374 722c  , log_file: str,
+000076e0: 206e 3a20 696e 7420 3d20 3130 2920 2d3e   n: int = 10) ->
+000076f0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+00007700: 220a 2020 2020 2020 2020 4765 7420 7468  ".        Get th
+00007710: 6520 636f 6d6d 616e 6420 746f 2072 6574  e command to ret
+00007720: 7269 6576 6520 7468 6520 7265 6365 6e74  rieve the recent
+00007730: 206c 6f67 2065 6e74 7269 6573 2066 726f   log entries fro
+00007740: 6d20 610a 2020 2020 2020 2020 7370 6563  m a.        spec
+00007750: 6966 6965 6420 6c6f 6720 6669 6c65 2e0a  ified log file..
+00007760: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00007770: 2020 2020 2020 2020 2020 206c 6f67 5f66             log_f
+00007780: 696c 6520 2873 7472 293a 2054 6865 2070  ile (str): The p
+00007790: 6174 6820 746f 2074 6865 206c 6f67 2066  ath to the log f
+000077a0: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
+000077b0: 206e 2028 696e 742c 206f 7074 696f 6e61   n (int, optiona
+000077c0: 6c29 3a20 5468 6520 6e75 6d62 6572 206f  l): The number o
+000077d0: 6620 7265 6365 6e74 206c 6f67 2065 6e74  f recent log ent
+000077e0: 7269 6573 2074 6f20 7265 7472 6965 7665  ries to retrieve
+000077f0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007800: 2020 4465 6661 756c 7473 2074 6f20 3130    Defaults to 10
+00007810: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00007820: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00007830: 7374 723a 2054 6865 2063 6f6d 6d61 6e64  str: The command
+00007840: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
+00007850: 2072 6563 656e 7420 6c6f 6720 656e 7472   recent log entr
+00007860: 6965 732e 0a20 2020 2020 2020 2022 2222  ies..        """
+00007870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007880: 7365 6c66 2e5f 5441 494c 5f4c 4f47 5f43  self._TAIL_LOG_C
+00007890: 4d44 2e66 6f72 6d61 7428 6e3d 6e2c 206c  MD.format(n=n, l
+000078a0: 6f67 5f66 696c 653d 6c6f 675f 6669 6c65  og_file=log_file
+000078b0: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
+000078c0: 6374 6976 655f 6a6f 625f 7072 6f67 7265  ctive_job_progre
+000078d0: 7373 2873 656c 662c 0a20 2020 2020 2020  ss(self,.       
+000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078f0: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
+00007900: 6f62 5f69 643a 2073 7472 2c0a 2020 2020  ob_id: str,.    
+00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2020 2020 2020 2020 2020 7061 7474              patt
+00007930: 6572 6e3a 2073 7472 203d 2072 225c 642b  ern: str = r"\d+
+00007940: 2522 2c0a 2020 2020 2020 2020 2020 2020  %",.            
+00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007960: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
+00007970: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
+00007980: 5d20 3d20 4e6f 6e65 2920 2d3e 2073 7472  ] = None) -> str
+00007990: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000079a0: 2020 2020 2020 4765 7420 7468 6520 7072        Get the pr
+000079b0: 6f67 7265 7373 206f 6620 616e 2061 6374  ogress of an act
+000079c0: 6976 6520 536c 7572 6d20 6a6f 6220 6672  ive Slurm job fr
+000079d0: 6f6d 2069 7473 206c 6f67 6669 6c65 732e  om its logfiles.
+000079e0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000079f0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00007a00: 6d5f 6a6f 625f 6964 2028 7374 7229 3a20  m_job_id (str): 
+00007a10: 5468 6520 4944 206f 6620 7468 6520 536c  The ID of the Sl
+00007a20: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
+00007a30: 2020 2020 2070 6174 7465 726e 2028 7374       pattern (st
+00007a40: 7229 3a20 5468 6520 7061 7474 6572 6e20  r): The pattern 
+00007a50: 746f 206d 6174 6368 2069 6e20 7468 6520  to match in the 
+00007a60: 6a6f 6220 6c6f 6720 746f 2065 7874 7261  job log to extra
+00007a70: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+00007a80: 2020 2074 6865 2070 726f 6772 6573 7320     the progress 
+00007a90: 2864 6566 6175 6c74 3a20 7222 5c64 2b25  (default: r"\d+%
+00007aa0: 2229 2e0a 0a20 2020 2020 2020 2020 2020  ")...           
+00007ab0: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
+00007ac0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
+00007ad0: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
+00007ae0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00007af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b00: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
+00007b10: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
+00007b20: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00007b30: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
+00007b40: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00007b50: 2020 7374 723a 2054 6865 2070 726f 6772    str: The progr
+00007b60: 6573 7320 6f66 2074 6865 2053 6c75 726d  ess of the Slurm
+00007b70: 206a 6f62 2e0a 2020 2020 2020 2020 2222   job..        ""
+00007b80: 220a 2020 2020 2020 2020 636d 646c 6973  ".        cmdlis
+00007b90: 7420 3d20 5b5d 0a20 2020 2020 2020 2063  t = [].        c
+00007ba0: 6d64 203d 2073 656c 662e 6765 745f 7265  md = self.get_re
+00007bb0: 6365 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64  cent_log_command
+00007bc0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
+00007bd0: 675f 6669 6c65 3d73 656c 662e 5f4c 4f47  g_file=self._LOG
+00007be0: 4649 4c45 2e66 6f72 6d61 7428 736c 7572  FILE.format(slur
+00007bf0: 6d5f 6a6f 625f 6964 3d73 6c75 726d 5f6a  m_job_id=slurm_j
+00007c00: 6f62 5f69 6429 290a 2020 2020 2020 2020  ob_id)).        
+00007c10: 636d 646c 6973 742e 6170 7065 6e64 2863  cmdlist.append(c
+00007c20: 6d64 290a 2020 2020 2020 2020 6966 2065  md).        if e
+00007c30: 6e76 2069 7320 4e6f 6e65 3a0a 2020 2020  nv is None:.    
+00007c40: 2020 2020 2020 2020 656e 7620 3d20 7b7d          env = {}
+00007c50: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00007c60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00007c70: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00007c80: 616e 6473 2863 6d64 6c69 7374 2c20 656e  ands(cmdlist, en
+00007c90: 763d 656e 7629 0a20 2020 2020 2020 2065  v=env).        e
+00007ca0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00007cb0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00007cc0: 2020 6c6f 6767 6572 2e65 7272 6f72 2866    logger.error(f
+00007cd0: 2249 7373 7565 2077 6974 6820 7275 6e20  "Issue with run 
+00007ce0: 636f 6d6d 616e 643a 207b 657d 2229 0a20  command: {e}"). 
+00007cf0: 2020 2020 2020 2023 204d 6174 6368 2074         # Match t
+00007d00: 6865 2073 7065 6369 6669 6564 2070 6174  he specified pat
+00007d10: 7465 726e 2069 6e20 7468 6520 7265 7375  tern in the resu
+00007d20: 6c74 2773 2073 7464 6f75 740a 2020 2020  lt's stdout.    
+00007d30: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00007d40: 2020 2020 206c 6174 6573 745f 7072 6f67       latest_prog
+00007d50: 7265 7373 203d 2072 652e 6669 6e64 616c  ress = re.findal
+00007d60: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00007d70: 2020 2070 6174 7465 726e 2c20 7265 7375     pattern, resu
+00007d80: 6c74 2e73 7464 6f75 7429 5b2d 315d 0a20  lt.stdout)[-1]. 
+00007d90: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00007da0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00007db0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00007dc0: 2e65 7272 6f72 2866 2249 7373 7565 2077  .error(f"Issue w
+00007dd0: 6974 6820 6578 7472 6163 7469 6e67 2070  ith extracting p
+00007de0: 726f 6772 6573 733a 207b 657d 2229 0a0a  rogress: {e}")..
+00007df0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00007e00: 2250 726f 6772 6573 733a 207b 6c61 7465  "Progress: {late
+00007e10: 7374 5f70 726f 6772 6573 737d 5c6e 220a  st_progress}\n".
+00007e20: 0a20 2020 2064 6566 2072 756e 5f63 6f6d  .    def run_com
+00007e30: 6d61 6e64 7328 7365 6c66 2c20 636d 646c  mands(self, cmdl
+00007e40: 6973 743a 204c 6973 745b 7374 725d 2c0a  ist: List[str],.
+00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
+00007e70: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
+00007e80: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ea0: 7365 703a 2073 7472 203d 2027 2026 2620  sep: str = ' && 
+00007eb0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00007ec0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00007ed0: 2920 2d3e 2052 6573 756c 743a 0a20 2020  ) -> Result:.   
+00007ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007ef0: 2052 756e 2061 206c 6973 7420 6f66 2073   Run a list of s
+00007f00: 6865 6c6c 2063 6f6d 6d61 6e64 7320 636f  hell commands co
+00007f10: 6e73 6563 7574 6976 656c 7920 6f6e 2074  nsecutively on t
+00007f20: 6865 2053 6c75 726d 2063 6c75 7374 6572  he Slurm cluster
+00007f30: 2c0a 2020 2020 2020 2020 656e 7375 7269  ,.        ensuri
+00007f40: 6e67 2074 6865 2073 7563 6365 7373 206f  ng the success o
+00007f50: 6620 6561 6368 2062 6566 6f72 6520 7072  f each before pr
+00007f60: 6f63 6565 6469 6e67 2074 6f20 7468 6520  oceeding to the 
+00007f70: 6e65 7874 2e0a 0a20 2020 2020 2020 2054  next...        T
+00007f80: 6865 2065 6e76 6972 6f6e 6d65 6e74 2076  he environment v
+00007f90: 6172 6961 626c 6573 2063 616e 2062 6520  ariables can be 
+00007fa0: 7365 7420 7573 696e 6720 7468 6520 6065  set using the `e
+00007fb0: 6e76 6020 6172 6775 6d65 6e74 2e0a 2020  nv` argument..  
+00007fc0: 2020 2020 2020 5468 6573 6520 636f 6d6d        These comm
+00007fd0: 616e 6473 2072 6574 6169 6e20 7468 6520  ands retain the 
+00007fe0: 7361 6d65 2073 6573 7369 6f6e 2028 656e  same session (en
+00007ff0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00008000: 6c65 730a 2020 2020 2020 2020 6574 632e  les.        etc.
+00008010: 292c 2075 6e6c 696b 6520 7275 6e6e 696e  ), unlike runnin
+00008020: 6720 7468 656d 2073 6570 6172 6174 656c  g them separatel
+00008030: 792e 0a0a 2020 2020 2020 2020 4172 6773  y...        Args
+00008040: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00008050: 646c 6973 7420 284c 6973 745b 7374 725d  dlist (List[str]
+00008060: 293a 2041 206c 6973 7420 6f66 2073 6865  ): A list of she
+00008070: 6c6c 2063 6f6d 6d61 6e64 7320 746f 2072  ll commands to r
+00008080: 756e 206f 6e20 536c 7572 6d2e 0a20 2020  un on Slurm..   
+00008090: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+000080a0: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+000080b0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+000080c0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+000080d0: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
+000080e0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
+000080f0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
+00008100: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
+00008110: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+00008120: 2020 2020 2020 2073 6570 2028 7374 722c         sep (str,
+00008130: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00008140: 7365 7061 7261 746f 7220 7573 6564 2074  separator used t
+00008150: 6f20 636f 6e63 6174 656e 6174 6520 7468  o concatenate th
+00008160: 6520 0a20 2020 2020 2020 2020 2020 2020  e .             
+00008170: 2020 2063 6f6d 6d61 6e64 732e 2044 6566     commands. Def
+00008180: 6175 6c74 7320 746f 2027 2026 2620 272e  aults to ' && '.
+00008190: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+000081a0: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
+000081b0: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+000081c0: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
+000081d0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000081e0: 2020 2052 6573 756c 743a 2054 6865 2072     Result: The r
+000081f0: 6573 756c 7420 6f66 2074 6865 206c 6173  esult of the las
+00008200: 7420 636f 6d6d 616e 6420 696e 2074 6865  t command in the
+00008210: 206c 6973 742e 0a20 2020 2020 2020 2022   list..        "
+00008220: 2222 0a20 2020 2020 2020 2069 6620 656e  "".        if en
+00008230: 7620 6973 204e 6f6e 653a 0a20 2020 2020  v is None:.     
+00008240: 2020 2020 2020 2065 6e76 203d 207b 7d0a         env = {}.
+00008250: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+00008260: 702e 6a6f 696e 2863 6d64 6c69 7374 290a  p.join(cmdlist).
+00008270: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00008280: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00008290: 2066 2252 756e 6e69 6e67 2063 6f6d 6d61   f"Running comma
+000082a0: 6e64 732c 2077 6974 6820 656e 7620 7b65  nds, with env {e
+000082b0: 6e76 7d20 616e 6420 7365 7020 7b73 6570  nv} and sep {sep
+000082c0: 7d20 5c0a 2020 2020 2020 2020 2020 2020  } \.            
+000082d0: 2020 2020 616e 6420 7b6b 7761 7267 737d      and {kwargs}
+000082e0: 3a20 7b63 6d64 7d22 290a 2020 2020 2020  : {cmd}").      
+000082f0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00008300: 7275 6e28 636d 642c 2065 6e76 3d65 6e76  run(cmd, env=env
+00008310: 2c20 2a2a 6b77 6172 6773 2920 2023 206f  , **kwargs)  # o
+00008320: 7574 5f73 7472 6561 6d3d 6f75 745f 7374  ut_stream=out_st
+00008330: 7265 616d 2c0a 0a20 2020 2020 2020 2074  ream,..        t
+00008340: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00008350: 2320 5761 7463 6820 6f75 7420 666f 7220  # Watch out for 
+00008360: 556e 6963 6f64 6545 6e63 6f64 6545 7272  UnicodeEncodeErr
+00008370: 6f72 2077 6865 6e20 796f 7520 7374 7228  or when you str(
+00008380: 2920 7468 6973 2e0a 2020 2020 2020 2020  ) this..        
+00008390: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000083a0: 6622 7b72 6573 756c 742e 7374 646f 7574  f"{result.stdout
+000083b0: 7d22 290a 2020 2020 2020 2020 6578 6365  }").        exce
+000083c0: 7074 2055 6e69 636f 6465 456e 636f 6465  pt UnicodeEncode
+000083d0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+000083e0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+000083f0: 7272 6f72 2866 2255 6e69 636f 6465 2065  rror(f"Unicode e
+00008400: 7272 6f72 3a20 7b65 7d22 290a 2020 2020  rror: {e}").    
+00008410: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+00008420: 4f4e 4c59 2073 7464 6f75 7420 5245 434f  ONLY stdout RECO
+00008430: 4445 204e 4545 4445 443f 3f20 6f72 2061  DE NEEDED?? or a
+00008440: 6c73 6f20 6572 726f 723f 0a20 2020 2020  lso error?.     
+00008450: 2020 2020 2020 2072 6573 756c 742e 7374         result.st
+00008460: 646f 7574 203d 2072 6573 756c 742e 7374  dout = result.st
+00008470: 646f 7574 2e65 6e63 6f64 6528 0a20 2020  dout.encode(.   
+00008480: 2020 2020 2020 2020 2020 2020 2027 7574               'ut
+00008490: 662d 3827 2c20 2769 676e 6f72 6527 292e  f-8', 'ignore').
+000084a0: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
+000084b0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000084c0: 6573 756c 740a 0a20 2020 2064 6566 2073  esult..    def s
+000084d0: 7472 5f74 6f5f 636c 6173 7328 7365 6c66  tr_to_class(self
+000084e0: 2c20 6d6f 6475 6c65 5f6e 616d 653a 2073  , module_name: s
+000084f0: 7472 2c20 636c 6173 735f 6e61 6d65 3a20  tr, class_name: 
+00008500: 7374 722c 202a 6172 6773 2c20 2a2a 6b77  str, *args, **kw
+00008510: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+00008520: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+00008530: 6e20 6120 636c 6173 7320 696e 7374 616e  n a class instan
+00008540: 6365 2066 726f 6d20 6120 7374 7269 6e67  ce from a string
+00008550: 2072 6566 6572 656e 6365 2e0a 0a20 2020   reference...   
+00008560: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00008570: 2020 2020 2020 206d 6f64 756c 655f 6e61         module_na
+00008580: 6d65 2028 7374 7229 3a20 5468 6520 6e61  me (str): The na
+00008590: 6d65 206f 6620 7468 6520 6d6f 6475 6c65  me of the module
+000085a0: 2e0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
+000085b0: 6173 735f 6e61 6d65 2028 7374 7229 3a20  ass_name (str): 
+000085c0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+000085d0: 636c 6173 732e 0a20 2020 2020 2020 2020  class..         
+000085e0: 2020 202a 6172 6773 3a20 4164 6469 7469     *args: Additi
+000085f0: 6f6e 616c 2070 6f73 6974 696f 6e61 6c20  onal positional 
+00008600: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
+00008610: 6520 636c 6173 7320 636f 6e73 7472 7563  e class construc
+00008620: 746f 722e 0a20 2020 2020 2020 2020 2020  tor..           
+00008630: 202a 2a6b 7761 7267 733a 2041 6464 6974   **kwargs: Addit
+00008640: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
+00008650: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
+00008660: 636c 6173 7320 636f 6e73 7472 7563 746f  class constructo
+00008670: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
+00008680: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00008690: 206f 626a 6563 743a 2041 6e20 696e 7374   object: An inst
+000086a0: 616e 6365 206f 6620 7468 6520 7370 6563  ance of the spec
+000086b0: 6966 6965 6420 636c 6173 732c 206f 7220  ified class, or 
+000086c0: 4e6f 6e65 2069 6620 7468 6520 636c 6173  None if the clas
+000086d0: 7320 6f72 0a20 2020 2020 2020 2020 2020  s or.           
+000086e0: 2020 2020 206d 6f64 756c 6520 646f 6573       module does
+000086f0: 206e 6f74 2065 7869 7374 2e0a 2020 2020   not exist..    
+00008700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008710: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00008720: 206d 6f64 756c 655f 203d 2069 6d70 6f72   module_ = impor
+00008730: 746c 6962 2e69 6d70 6f72 745f 6d6f 6475  tlib.import_modu
+00008740: 6c65 286d 6f64 756c 655f 6e61 6d65 290a  le(module_name).
+00008750: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00008760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008770: 2063 6c61 7373 5f20 3d20 6765 7461 7474   class_ = getatt
+00008780: 7228 6d6f 6475 6c65 5f2c 2063 6c61 7373  r(module_, class
+00008790: 5f6e 616d 6529 282a 6172 6773 2c20 2a2a  _name)(*args, **
+000087a0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+000087b0: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
+000087c0: 6275 7465 4572 726f 723a 0a20 2020 2020  buteError:.     
+000087d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000087e0: 722e 6572 726f 7228 2743 6c61 7373 2064  r.error('Class d
+000087f0: 6f65 7320 6e6f 7420 6578 6973 7427 290a  oes not exist').
+00008800: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+00008810: 6d70 6f72 7445 7272 6f72 3a0a 2020 2020  mportError:.    
+00008820: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00008830: 7272 6f72 2827 4d6f 6475 6c65 2064 6f65  rror('Module doe
+00008840: 7320 6e6f 7420 6578 6973 7427 290a 2020  s not exist').  
+00008850: 2020 2020 2020 7265 7475 726e 2063 6c61        return cla
+00008860: 7373 5f20 6f72 204e 6f6e 650a 0a20 2020  ss_ or None..   
+00008870: 2064 6566 2072 756e 5f63 6f6d 6d61 6e64   def run_command
+00008880: 735f 7370 6c69 745f 6f75 7428 7365 6c66  s_split_out(self
+00008890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088b0: 2063 6d64 6c69 7374 3a20 4c69 7374 5b73   cmdlist: List[s
+000088c0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
+000088f0: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
+00008900: 5d20 3d20 4e6f 6e65 0a20 2020 2020 2020  ] = None.       
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 2020 2020 2020 2920 2d3e 204c 6973          ) -> Lis
+00008930: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
+00008940: 2222 2252 756e 2061 206c 6973 7420 6f66  """Run a list of
+00008950: 2073 6865 6c6c 2063 6f6d 6d61 6e64 7320   shell commands 
+00008960: 636f 6e73 6563 7574 6976 656c 7920 616e  consecutively an
+00008970: 6420 7370 6c69 7420 7468 6520 6f75 7470  d split the outp
+00008980: 7574 0a20 2020 2020 2020 206f 6620 6561  ut.        of ea
+00008990: 6368 2063 6f6d 6d61 6e64 2e0a 0a20 2020  ch command...   
+000089a0: 2020 2020 2045 6163 6820 636f 6d6d 616e       Each comman
+000089b0: 6420 696e 2074 6865 206c 6973 7420 6973  d in the list is
+000089c0: 2065 7865 6375 7465 6420 7769 7468 2061   executed with a
+000089d0: 2073 6570 6172 6174 6f72 2069 6e20 6265   separator in be
+000089e0: 7477 6565 6e0a 2020 2020 2020 2020 7468  tween.        th
+000089f0: 6174 2069 7320 756e 6971 7565 2061 6e64  at is unique and
+00008a00: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00008a10: 7370 6c69 740a 2020 2020 2020 2020 7468  split.        th
+00008a20: 6520 6f75 7470 7574 206f 6620 6561 6368  e output of each
+00008a30: 2063 6f6d 6d61 6e64 206c 6174 6572 2e20   command later. 
+00008a40: 5468 6520 7365 7061 7261 746f 7220 7573  The separator us
+00008a50: 6564 2069 7320 7370 6563 6966 6965 640a  ed is specified.
+00008a60: 2020 2020 2020 2020 6279 2074 6865 2060          by the `
+00008a70: 5f4f 5554 5f53 4550 6020 6174 7472 6962  _OUT_SEP` attrib
+00008a80: 7574 6520 6f66 2074 6865 0a20 2020 2020  ute of the.     
+00008a90: 2020 2053 6c75 726d 436c 6965 6e74 2069     SlurmClient i
+00008aa0: 6e73 7461 6e63 652e 0a0a 2020 2020 2020  nstance...      
+00008ab0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008ac0: 2020 2020 636d 646c 6973 7420 284c 6973      cmdlist (Lis
+00008ad0: 745b 7374 725d 293a 2041 206c 6973 7420  t[str]): A list 
+00008ae0: 6f66 2073 6865 6c6c 2063 6f6d 6d61 6e64  of shell command
+00008af0: 7320 746f 2072 756e 2e0a 2020 2020 2020  s to run..      
+00008b00: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+00008b10: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+00008b20: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+00008b30: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00008b40: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
+00008b50: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
+00008b60: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+00008b70: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+00008b80: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+00008b90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00008ba0: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
+00008bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008bc0: 2020 4120 6c69 7374 206f 6620 7374 7269    A list of stri
+00008bd0: 6e67 732c 2077 6865 7265 2065 6163 6820  ngs, where each 
+00008be0: 7374 7269 6e67 2063 6f72 7265 7370 6f6e  string correspon
+00008bf0: 6473 2074 6f0a 2020 2020 2020 2020 2020  ds to.          
+00008c00: 2020 2020 2020 7468 6520 6f75 7470 7574        the output
+00008c10: 206f 6620 6120 7369 6e67 6c65 2063 6f6d   of a single com
+00008c20: 6d61 6e64 2069 6e20 6063 6d64 6c69 7374  mand in `cmdlist
+00008c30: 6020 7370 6c69 740a 2020 2020 2020 2020  ` split.        
+00008c40: 2020 2020 2020 2020 6279 2074 6865 2073          by the s
+00008c50: 6570 6172 6174 6f72 2060 5f4f 5554 5f53  eparator `_OUT_S
+00008c60: 4550 602e 0a0a 2020 2020 2020 2020 5261  EP`...        Ra
+00008c70: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00008c80: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
+00008c90: 4966 2061 6e79 206f 6620 7468 6520 636f  If any of the co
+00008ca0: 6d6d 616e 6473 2066 6169 6c20 746f 2065  mmands fail to e
+00008cb0: 7865 6375 7465 2073 7563 6365 7373 6675  xecute successfu
+00008cc0: 6c6c 792e 0a20 2020 2020 2020 2022 2222  lly..        """
+00008cd0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00008ce0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00008cf0: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00008d00: 616e 6473 2863 6d64 6c69 7374 3d63 6d64  ands(cmdlist=cmd
+00008d10: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
+00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d30: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+00008d40: 3d65 6e76 2c0a 2020 2020 2020 2020 2020  =env,.          
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 2020 2020 2020 2020 2020 2020 2073 6570               sep
+00008d70: 3d66 2220 3b20 6563 686f 207b 7365 6c66  =f" ; echo {self
+00008d80: 2e5f 4f55 545f 5345 507d 203b 2022 290a  ._OUT_SEP} ; ").
+00008d90: 2020 2020 2020 2020 6578 6365 7074 2055          except U
+00008da0: 6e65 7870 6563 7465 6445 7869 7420 6173  nexpectedExit as
+00008db0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00008dc0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2865  logger.warning(e
+00008dd0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00008de0: 7375 6c74 203d 2065 2e72 6573 756c 740a  sult = e.result.
+00008df0: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00008e00: 742e 6f6b 3a0a 2020 2020 2020 2020 2020  t.ok:.          
+00008e10: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
+00008e20: 756c 742e 7374 646f 7574 0a20 2020 2020  ult.stdout.     
+00008e30: 2020 2020 2020 2073 706c 6974 5f72 6573         split_res
+00008e40: 706f 6e73 6573 203d 2072 6573 706f 6e73  ponses = respons
+00008e50: 652e 7370 6c69 7428 7365 6c66 2e5f 4f55  e.split(self._OU
+00008e60: 545f 5345 5029 0a20 2020 2020 2020 2020  T_SEP).         
+00008e70: 2020 2072 6574 7572 6e20 7370 6c69 745f     return split_
+00008e80: 7265 7370 6f6e 7365 730a 2020 2020 2020  responses.      
+00008e90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008ea0: 2020 2020 2320 4966 2074 6865 2072 6573      # If the res
+00008eb0: 756c 7420 6973 206e 6f74 206f 6b2c 206c  ult is not ok, l
+00008ec0: 6f67 2074 6865 2065 7272 6f72 2061 6e64  og the error and
+00008ed0: 2072 6169 7365 2061 6e20 5353 4845 7863   raise an SSHExc
+00008ee0: 6570 7469 6f6e 0a20 2020 2020 2020 2020  eption.         
+00008ef0: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
+00008f00: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
+00008f10: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
+00008f20: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
+00008f30: 7228 6572 726f 7229 0a20 2020 2020 2020  r(error).       
+00008f40: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00008f50: 6365 7074 696f 6e28 6572 726f 7229 0a0a  ception(error)..
+00008f60: 2020 2020 6465 6620 6c69 7374 5f61 6374      def list_act
+00008f70: 6976 655f 6a6f 6273 2873 656c 662c 0a20  ive_jobs(self,. 
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
+00008fa0: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00008fb0: 7374 725d 5d20 3d20 4e6f 6e65 2920 2d3e  str]] = None) ->
+00008fc0: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00008fd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008fe0: 4765 7420 6120 6c69 7374 206f 6620 6163  Get a list of ac
+00008ff0: 7469 7665 206a 6f62 7320 6672 6f6d 2053  tive jobs from S
+00009000: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
+00009010: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00009020: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
+00009030: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
+00009040: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
+00009050: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00009060: 746f 200a 2020 2020 2020 2020 2020 2020  to .            
+00009070: 2020 2020 7365 7420 7768 656e 2072 756e      set when run
+00009080: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
+00009090: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+000090a0: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
+000090b0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000090c0: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
+000090d0: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
+000090e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000090f0: 2020 2020 2320 636d 6420 3d20 7365 6c66      # cmd = self
+00009100: 2e5f 4143 5449 5645 5f4a 4f42 535f 434d  ._ACTIVE_JOBS_CM
+00009110: 440a 2020 2020 2020 2020 636d 6420 3d20  D.        cmd = 
+00009120: 7365 6c66 2e67 6574 5f6a 6f62 735f 696e  self.get_jobs_in
+00009130: 666f 5f63 6f6d 6d61 6e64 2873 7461 7274  fo_command(start
+00009140: 5f74 696d 653d 226e 6f77 222c 2073 7461  _time="now", sta
+00009150: 7465 733d 2272 2229 0a20 2020 2020 2020  tes="r").       
+00009160: 206c 6f67 6765 722e 696e 666f 2822 5265   logger.info("Re
+00009170: 7472 6965 7669 6e67 206c 6973 7420 6f66  trieving list of
+00009180: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
+00009190: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
+000091a0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+000091b0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+000091c0: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
+000091d0: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
+000091e0: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
+000091f0: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
+00009200: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
+00009210: 7374 2e72 6576 6572 7365 2829 0a20 2020  st.reverse().   
+00009220: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
+00009230: 6c69 7374 0a0a 2020 2020 6465 6620 6c69  list..    def li
+00009240: 7374 5f63 6f6d 706c 6574 6564 5f6a 6f62  st_completed_job
+00009250: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
+00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009270: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
+00009280: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
+00009290: 5d20 3d20 4e6f 6e65 2920 2d3e 204c 6973  ] = None) -> Lis
+000092a0: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
+000092b0: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
+000092c0: 6120 6c69 7374 206f 6620 636f 6d70 6c65  a list of comple
+000092d0: 7465 6420 6a6f 6273 2066 726f 6d20 534c  ted jobs from SL
+000092e0: 5552 4d2e 0a0a 2020 2020 2020 2020 4172  URM...        Ar
+000092f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00009300: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
+00009310: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+00009320: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
+00009330: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
+00009340: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+00009350: 2020 7365 7420 7768 656e 2072 756e 6e69    set when runni
+00009360: 6e67 2074 6865 2063 6f6d 6d61 6e64 2e20  ng the command. 
+00009370: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00009380: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00009390: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000093a0: 4c69 7374 5b73 7472 5d3a 2041 206c 6973  List[str]: A lis
+000093b0: 7420 6f66 206a 6f62 2049 4473 2e0a 2020  t of job IDs..  
+000093c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000093d0: 2020 2063 6d64 203d 2073 656c 662e 6765     cmd = self.ge
+000093e0: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
+000093f0: 616e 6428 7374 6174 6573 3d22 6364 2229  and(states="cd")
+00009400: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00009410: 696e 666f 2822 5265 7472 6965 7669 6e67  info("Retrieving
+00009420: 2061 206c 6973 7420 6f66 2063 6f6d 706c   a list of compl
+00009430: 6574 6564 206a 6f62 7320 6672 6f6d 2053  eted jobs from S
+00009440: 6c75 726d 2229 0a20 2020 2020 2020 2072  lurm").        r
+00009450: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
+00009460: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d2c  _commands([cmd],
+00009470: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
+00009480: 2020 6a6f 625f 6c69 7374 203d 205b 6a6f    job_list = [jo
+00009490: 622e 7374 7269 7028 2920 666f 7220 6a6f  b.strip() for jo
+000094a0: 6220 696e 2072 6573 756c 742e 7374 646f  b in result.stdo
+000094b0: 7574 2e73 7472 6970 2829 2e73 706c 6974  ut.strip().split
+000094c0: 2827 5c6e 2729 5d0a 2020 2020 2020 2020  ('\n')].        
+000094d0: 6a6f 625f 6c69 7374 2e72 6576 6572 7365  job_list.reverse
+000094e0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000094f0: 6e20 6a6f 625f 6c69 7374 0a0a 2020 2020  n job_list..    
+00009500: 6465 6620 6c69 7374 5f61 6c6c 5f6a 6f62  def list_all_job
+00009510: 7328 7365 6c66 2c20 656e 763a 204f 7074  s(self, env: Opt
+00009520: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00009530: 7374 725d 5d20 3d20 4e6f 6e65 2920 2d3e  str]] = None) ->
+00009540: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00009550: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009560: 4765 7420 6120 6c69 7374 206f 6620 616c  Get a list of al
+00009570: 6c20 6a6f 6273 2066 726f 6d20 534c 5552  l jobs from SLUR
+00009580: 4d2e 0a0a 2020 2020 2020 2020 4172 6773  M...        Args
+00009590: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
+000095a0: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
+000095b0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
+000095c0: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
+000095d0: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
+000095e0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+000095f0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
+00009600: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
+00009610: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00009620: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009630: 733a 0a20 2020 2020 2020 2020 2020 204c  s:.            L
+00009640: 6973 745b 7374 725d 3a20 4120 6c69 7374  ist[str]: A list
+00009650: 206f 6620 6a6f 6220 4944 732e 0a20 2020   of job IDs..   
+00009660: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00009670: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
+00009680: 5f6a 6f62 735f 696e 666f 5f63 6f6d 6d61  _jobs_info_comma
+00009690: 6e64 2829 0a20 2020 2020 2020 206c 6f67  nd().        log
+000096a0: 6765 722e 696e 666f 2822 5265 7472 6965  ger.info("Retrie
+000096b0: 7669 6e67 2061 206c 6973 7420 6f66 2061  ving a list of a
+000096c0: 6c6c 206a 6f62 7320 6672 6f6d 2053 6c75  ll jobs from Slu
+000096d0: 726d 2229 0a20 2020 2020 2020 2072 6573  rm").        res
+000096e0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+000096f0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
+00009700: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
+00009710: 6a6f 625f 6c69 7374 203d 2072 6573 756c  job_list = resul
+00009720: 742e 7374 646f 7574 2e73 7472 6970 2829  t.stdout.strip()
+00009730: 2e73 706c 6974 2827 5c6e 2729 0a20 2020  .split('\n').   
+00009740: 2020 2020 206a 6f62 5f6c 6973 742e 7265       job_list.re
+00009750: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
+00009760: 7265 7475 726e 206a 6f62 5f6c 6973 740a  return job_list.
+00009770: 0a20 2020 2064 6566 2067 6574 5f6a 6f62  .    def get_job
+00009780: 735f 696e 666f 5f63 6f6d 6d61 6e64 2873  s_info_command(s
+00009790: 656c 662c 2073 7461 7274 5f74 696d 653a  elf, start_time:
+000097a0: 2073 7472 203d 2022 3230 3233 2d30 312d   str = "2023-01-
+000097b0: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097d0: 2020 2065 6e64 5f74 696d 653a 2073 7472     end_time: str
+000097e0: 203d 2022 6e6f 7722 2c0a 2020 2020 2020   = "now",.      
+000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009800: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00009810: 2073 7472 203d 2022 4a6f 6249 6422 2c0a   str = "JobId",.
+00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00009840: 6174 6573 3a20 7374 7220 3d20 2272 2c63  ates: str = "r,c
+00009850: 642c 662c 746f 2c72 732c 646c 2c6e 6622  d,f,to,rs,dl,nf"
+00009860: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00009870: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
+00009880: 536c 7572 6d20 636f 6d6d 616e 6420 746f  Slurm command to
+00009890: 2072 6574 7269 6576 6520 696e 666f 726d   retrieve inform
+000098a0: 6174 696f 6e20 6162 6f75 7420 6f6c 6420  ation about old 
+000098b0: 6a6f 6273 2e0a 0a20 2020 2020 2020 2054  jobs...        T
+000098c0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
+000098d0: 6265 2066 6f72 6d61 7474 6564 2077 6974  be formatted wit
+000098e0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
+000098f0: 7374 6172 7420 7469 6d65 2c20 7768 6963  start time, whic
+00009900: 6820 6973 0a20 2020 2020 2020 2065 7870  h is.        exp
+00009910: 6563 7465 6420 746f 2062 6520 696e 2074  ected to be in t
+00009920: 6865 2049 534f 2066 6f72 6d61 7420 2259  he ISO format "Y
+00009930: 5959 592d 4d4d 2d44 4422 2e0a 2020 2020  YYY-MM-DD"..    
+00009940: 2020 2020 5468 6520 636f 6d6d 616e 6420      The command 
+00009950: 7769 6c6c 2075 7365 2074 6865 2022 7361  will use the "sa
+00009960: 6363 7422 2074 6f6f 6c20 746f 2071 7565  cct" tool to que
+00009970: 7279 2074 6865 0a20 2020 2020 2020 2053  ry the.        S
+00009980: 6c75 726d 2061 6363 6f75 6e74 696e 6720  lurm accounting 
+00009990: 6461 7461 6261 7365 2066 6f72 206a 6f62  database for job
+000099a0: 7320 7468 6174 2073 7461 7274 6564 206f  s that started o
+000099b0: 6e20 6f72 2061 6674 6572 2074 6865 0a20  n or after the. 
+000099c0: 2020 2020 2020 2073 7065 6369 6669 6564         specified
+000099d0: 2073 7461 7274 2074 696d 652c 2061 6e64   start time, and
+000099e0: 2077 696c 6c20 6f75 7470 7574 206f 6e6c   will output onl
+000099f0: 7920 7468 6520 6a6f 6220 4944 7320 282d  y the job IDs (-
+00009a00: 6f20 4a6f 6249 6429 0a20 2020 2020 2020  o JobId).       
+00009a10: 2077 6974 686f 7574 2068 6561 6465 7220   without header 
+00009a20: 6f72 2074 7261 696c 6572 206c 696e 6573  or trailer lines
+00009a30: 2028 2d6e 202d 5829 2e0a 0a20 2020 2020   (-n -X)...     
+00009a40: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00009a50: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
+00009a60: 2873 7472 293a 2054 6865 2073 7461 7274  (str): The start
+00009a70: 2074 696d 6520 6672 6f6d 2077 6869 6368   time from which
+00009a80: 2074 6f20 7265 7472 6965 7665 206a 6f62   to retrieve job
+00009a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009aa0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 4465   information. De
+00009ab0: 6661 756c 7473 2074 6f20 2232 3032 332d  faults to "2023-
+00009ac0: 3031 2d30 3122 2e0a 2020 2020 2020 2020  01-01"..        
+00009ad0: 2020 2020 656e 645f 7469 6d65 2028 7374      end_time (st
+00009ae0: 7229 3a20 5468 6520 656e 6420 7469 6d65  r): The end time
+00009af0: 2075 6e74 696c 2077 6869 6368 2074 6f20   until which to 
+00009b00: 7265 7472 6965 7665 206a 6f62 0a20 2020  retrieve job.   
+00009b10: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00009b20: 6f72 6d61 7469 6f6e 2e20 4465 6661 756c  ormation. Defaul
+00009b30: 7473 2074 6f20 226e 6f77 222e 0a20 2020  ts to "now"..   
+00009b40: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00009b50: 2028 7374 7229 3a20 5468 6520 636f 6c75   (str): The colu
+00009b60: 6d6e 7320 746f 2072 6574 7269 6576 6520  mns to retrieve 
+00009b70: 6672 6f6d 2074 6865 206a 6f62 2069 6e66  from the job inf
+00009b80: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
+00009b90: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00009ba0: 7473 2074 6f20 224a 6f62 4964 222e 2049  ts to "JobId". I
+00009bb0: 7420 6973 2063 6f6d 6d61 2073 6570 6172  t is comma separ
+00009bc0: 6174 6564 2c20 652e 672e 2022 4a6f 6249  ated, e.g. "JobI
+00009bd0: 642c 5374 6174 6522 2e0a 2020 2020 2020  d,State"..      
+00009be0: 2020 2020 2020 7374 6174 6573 2028 7374        states (st
+00009bf0: 7229 3a20 5468 6520 6a6f 6220 7374 6174  r): The job stat
+00009c00: 6573 2074 6f20 696e 636c 7564 6520 696e  es to include in
+00009c10: 2074 6865 2071 7565 7279 2e0a 2020 2020   the query..    
+00009c20: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00009c30: 756c 7473 2074 6f20 2272 2c63 642c 662c  ults to "r,cd,f,
+00009c40: 746f 2c72 732c 646c 2c6e 6622 2e0a 0a20  to,rs,dl,nf"... 
+00009c50: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00009c60: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00009c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c80: 2041 2073 7472 696e 6720 7265 7072 6573   A string repres
+00009c90: 656e 7469 6e67 2074 6865 2053 6c75 726d  enting the Slurm
+00009ca0: 2063 6f6d 6d61 6e64 2074 6f20 7265 7472   command to retr
+00009cb0: 6965 7665 0a20 2020 2020 2020 2020 2020  ieve.           
+00009cc0: 2020 2020 2069 6e66 6f72 6d61 7469 6f6e       information
+00009cd0: 2061 626f 7574 206f 6c64 206a 6f62 732e   about old jobs.
+00009ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009cf0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009d00: 2e5f 414c 4c5f 4a4f 4253 5f43 4d44 2e66  ._ALL_JOBS_CMD.f
+00009d10: 6f72 6d61 7428 7374 6172 745f 7469 6d65  ormat(start_time
+00009d20: 3d73 7461 7274 5f74 696d 652c 0a20 2020  =start_time,.   
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d50: 2020 2020 2020 656e 645f 7469 6d65 3d65        end_time=e
+00009d60: 6e64 5f74 696d 652c 0a20 2020 2020 2020  nd_time,.       
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d90: 2020 7374 6174 6573 3d73 7461 7465 732c    states=states,
+00009da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00009dd0: 733d 636f 6c75 6d6e 7329 0a0a 2020 2020  s=columns)..    
+00009de0: 6465 6620 7472 616e 7366 6572 5f64 6174  def transfer_dat
+00009df0: 6128 7365 6c66 2c20 6c6f 6361 6c5f 7061  a(self, local_pa
+00009e00: 7468 3a20 7374 7229 202d 3e20 5265 7375  th: str) -> Resu
+00009e10: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
+00009e20: 2020 2020 2020 2020 5472 616e 7366 6572          Transfer
+00009e30: 7320 6120 6669 6c65 206f 7220 6469 7265  s a file or dire
+00009e40: 6374 6f72 7920 6672 6f6d 2074 6865 206c  ctory from the l
+00009e50: 6f63 616c 206d 6163 6869 6e65 2074 6f20  ocal machine to 
+00009e60: 7468 6520 7265 6d6f 7465 0a20 2020 2020  the remote.     
+00009e70: 2020 2053 6c75 726d 2063 6c75 7374 6572     Slurm cluster
+00009e80: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00009e90: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+00009ea0: 616c 5f70 6174 6820 2873 7472 293a 2054  al_path (str): T
+00009eb0: 6865 206c 6f63 616c 2070 6174 6820 746f  he local path to
+00009ec0: 2074 6865 2066 696c 6520 6f72 2064 6972   the file or dir
+00009ed0: 6563 746f 7279 2074 6f0a 2020 2020 2020  ectory to.      
+00009ee0: 2020 2020 2020 2020 2020 7472 616e 7366            transf
+00009ef0: 6572 2e0a 0a20 2020 2020 2020 2052 6574  er...        Ret
+00009f00: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00009f10: 2020 5265 7375 6c74 3a20 5468 6520 7265    Result: The re
+00009f20: 7375 6c74 206f 6620 7468 6520 6669 6c65  sult of the file
+00009f30: 2074 7261 6e73 6665 7220 6f70 6572 6174   transfer operat
+00009f40: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
+00009f50: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00009f60: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
+00009f70: 2020 6622 5472 616e 7366 6572 696e 6720    f"Transfering 
+00009f80: 6669 6c65 207b 6c6f 6361 6c5f 7061 7468  file {local_path
+00009f90: 7d20 746f 207b 7365 6c66 2e73 6c75 726d  } to {self.slurm
+00009fa0: 5f64 6174 615f 7061 7468 7d22 290a 2020  _data_path}").  
+00009fb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00009fc0: 662e 7075 7428 6c6f 6361 6c3d 6c6f 6361  f.put(local=loca
+00009fd0: 6c5f 7061 7468 2c20 7265 6d6f 7465 3d73  l_path, remote=s
+00009fe0: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
+00009ff0: 6174 6829 0a0a 2020 2020 6465 6620 756e  ath)..    def un
+0000a000: 7061 636b 5f64 6174 6128 7365 6c66 2c20  pack_data(self, 
+0000a010: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
+0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 2020 656e 763a 204f 7074 696f 6e61 6c5b    env: Optional[
+0000a040: 4469 6374 5b73 7472 2c20 7374 725d 5d20  Dict[str, str]] 
+0000a050: 3d20 4e6f 6e65 2920 2d3e 2052 6573 756c  = None) -> Resul
+0000a060: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+0000a070: 2020 2020 2020 2055 6e70 6163 6b73 2061         Unpacks a
+0000a080: 207a 6970 7065 6420 6669 6c65 206f 6e20   zipped file on 
+0000a090: 7468 6520 7265 6d6f 7465 2053 6c75 726d  the remote Slurm
+0000a0a0: 2063 6c75 7374 6572 2e0a 0a20 2020 2020   cluster...     
+0000a0b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000a0c0: 2020 2020 207a 6970 6669 6c65 2028 7374       zipfile (st
+0000a0d0: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
+0000a0e0: 7468 6520 7a69 7070 6564 2066 696c 6520  the zipped file 
+0000a0f0: 746f 2062 6520 756e 7061 636b 6564 2e0a  to be unpacked..
+0000a100: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
+0000a110: 2028 4469 6374 5b73 7472 2c20 7374 725d   (Dict[str, str]
+0000a120: 2c20 6f70 7469 6f6e 616c 293a 204f 7074  , optional): Opt
+0000a130: 696f 6e61 6c20 656e 7669 726f 6e6d 656e  ional environmen
+0000a140: 7420 7661 7269 6162 6c65 7320 0a20 2020  t variables .   
+0000a150: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
+0000a160: 7365 7420 7768 656e 2072 756e 6e69 6e67  set when running
+0000a170: 2074 6865 2063 6f6d 6d61 6e64 2e20 4465   the command. De
+0000a180: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+0000a190: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000a1a0: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+0000a1b0: 7375 6c74 3a20 5468 6520 7265 7375 6c74  sult: The result
+0000a1c0: 206f 6620 7468 6520 636f 6d6d 616e 642e   of the command.
+0000a1d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000a1e0: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
+0000a1f0: 6765 745f 756e 7a69 705f 636f 6d6d 616e  get_unzip_comman
+0000a200: 6428 7a69 7066 696c 6529 0a20 2020 2020  d(zipfile).     
+0000a210: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+0000a220: 2255 6e70 6163 6b69 6e67 207b 7a69 7066  "Unpacking {zipf
+0000a230: 696c 657d 206f 6e20 536c 7572 6d22 290a  ile} on Slurm").
+0000a240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000a250: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+0000a260: 285b 636d 645d 2c20 656e 763d 656e 7629  ([cmd], env=env)
+0000a270: 0a0a 2020 2020 6465 6620 636f 6e76 6572  ..    def conver
+0000a280: 745f 6461 7461 2873 656c 662c 207a 6970  t_data(self, zip
+0000a290: 6669 6c65 3a20 7374 722c 0a20 2020 2020  file: str,.     
 0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
-0000a2c0: 3a20 7374 7220 3d20 226a 6f62 5f74 656d  : str = "job_tem
-0000a2d0: 706c 6174 652e 7368 220a 2020 2020 2020  plate.sh".      
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
-0000a310: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a320: 4765 6e65 7261 7465 2061 2053 6c75 726d  Generate a Slurm
-0000a330: 206a 6f62 2073 6372 6970 7420 666f 7220   job script for 
-0000a340: 6120 7370 6563 6966 6963 2077 6f72 6b66  a specific workf
-0000a350: 6c6f 772e 0a0a 2020 2020 2020 2020 4172  low...        Ar
-0000a360: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000a370: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
-0000a380: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000a390: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
-0000a3a0: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
-0000a3b0: 7320 2844 6963 745b 7374 722c 2073 7472  s (Dict[str, str
-0000a3c0: 5d29 3a20 4120 6469 6374 696f 6e61 7279  ]): A dictionary
-0000a3d0: 2063 6f6e 7461 696e 696e 6720 6b65 792d   containing key-
-0000a3e0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
-0000a3f0: 2020 2020 2020 7061 6972 7320 666f 7220        pairs for 
-0000a400: 7375 6273 7469 7475 7469 6e67 2070 6c61  substituting pla
-0000a410: 6365 686f 6c64 6572 7320 696e 2074 6865  ceholders in the
-0000a420: 206a 6f62 2074 656d 706c 6174 652e 0a20   job template.. 
-0000a430: 2020 2020 2020 2020 2020 2074 656d 706c             templ
-0000a440: 6174 6520 2873 7472 2c20 6f70 7469 6f6e  ate (str, option
-0000a450: 616c 293a 2054 6865 2066 696c 656e 616d  al): The filenam
-0000a460: 6520 6f66 2074 6865 206a 6f62 2074 656d  e of the job tem
-0000a470: 706c 6174 652e 0a20 2020 2020 2020 2020  plate..         
-0000a480: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-0000a490: 746f 2022 6a6f 625f 7465 6d70 6c61 7465  to "job_template
-0000a4a0: 2e73 6822 2e0a 0a20 2020 2020 2020 2052  .sh"...        R
-0000a4b0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000a4c0: 2020 2020 7374 723a 2054 6865 2067 656e      str: The gen
-0000a4d0: 6572 6174 6564 2053 6c75 726d 206a 6f62  erated Slurm job
-0000a4e0: 2073 6372 6970 7420 6173 2061 2073 7472   script as a str
-0000a4f0: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
-0000a500: 0a20 2020 2020 2020 2023 2061 6464 2077  .        # add w
-0000a510: 6f72 6b66 6c6f 7720 746f 2073 7562 7374  orkflow to subst
-0000a520: 6974 7574 6573 0a20 2020 2020 2020 2073  itutes.        s
-0000a530: 7562 7374 6974 7574 6573 5b27 6a6f 626e  ubstitutes['jobn
-0000a540: 616d 6527 5d20 3d20 776f 726b 666c 6f77  ame'] = workflow
-0000a550: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
-0000a560: 6a6f 6220 7465 6d70 6c61 7465 0a20 2020  job template.   
-0000a570: 2020 2020 2074 656d 706c 6174 655f 6620       template_f 
-0000a580: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
-0000a590: 6573 2229 2e6a 6f69 6e70 6174 6828 7465  es").joinpath(te
-0000a5a0: 6d70 6c61 7465 290a 2020 2020 2020 2020  mplate).        
-0000a5b0: 7769 7468 2074 656d 706c 6174 655f 662e  with template_f.
-0000a5c0: 6f70 656e 2827 7227 2920 6173 2066 3a0a  open('r') as f:.
-0000a5d0: 2020 2020 2020 2020 2020 2020 7372 6320              src 
-0000a5e0: 3d20 5465 6d70 6c61 7465 2866 2e72 6561  = Template(f.rea
-0000a5f0: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
-0000a600: 206a 6f62 5f73 6372 6970 7420 3d20 7372   job_script = sr
-0000a610: 632e 7361 6665 5f73 7562 7374 6974 7574  c.safe_substitut
-0000a620: 6528 7375 6273 7469 7475 7465 7329 0a20  e(substitutes). 
-0000a630: 2020 2020 2020 2072 6574 7572 6e20 6a6f         return jo
-0000a640: 625f 7363 7269 7074 0a0a 2020 2020 6465  b_script..    de
-0000a650: 6620 776f 726b 666c 6f77 5f70 6172 616d  f workflow_param
-0000a660: 735f 746f 5f73 7562 7328 7365 6c66 2c20  s_to_subs(self, 
-0000a670: 7061 7261 6d73 2920 2d3e 2044 6963 745b  params) -> Dict[
-0000a680: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-0000a690: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000a6a0: 6f6e 7665 7274 2077 6f72 6b66 6c6f 7720  onvert workflow 
-0000a6b0: 7061 7261 6d65 7465 7273 2074 6f20 7375  parameters to su
-0000a6c0: 6273 7469 7475 7469 6f6e 2064 6963 7469  bstitution dicti
-0000a6d0: 6f6e 6172 7920 666f 7220 6a6f 6220 7363  onary for job sc
-0000a6e0: 7269 7074 2e0a 0a20 2020 2020 2020 2041  ript...        A
-0000a6f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000a700: 2070 6172 616d 733a 2041 2064 6963 7469   params: A dicti
-0000a710: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-0000a720: 2077 6f72 6b66 6c6f 7720 7061 7261 6d65   workflow parame
-0000a730: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
-0000a740: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000a750: 2020 2020 4469 6374 5b73 7472 2c20 7374      Dict[str, st
-0000a760: 725d 3a20 4120 6469 6374 696f 6e61 7279  r]: A dictionary
-0000a770: 2077 6974 6820 7061 7261 6d65 7465 7220   with parameter 
-0000a780: 6e61 6d65 7320 6173 206b 6579 7320 616e  names as keys an
-0000a790: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000a7a0: 2020 636f 7272 6573 706f 6e64 696e 6720    corresponding 
-0000a7b0: 666c 6167 7320 7769 7468 2070 6c61 6365  flags with place
-0000a7c0: 686f 6c64 6572 7320 6173 2076 616c 7565  holders as value
-0000a7d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0000a7e0: 2020 2020 2020 2073 7562 7320 3d20 7b7d         subs = {}
-0000a7f0: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
-0000a800: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0000a810: 5f2c 2070 6172 616d 2069 6e20 7061 7261  _, param in para
-0000a820: 6d73 2e69 7465 6d73 2829 3a0a 2020 2020  ms.items():.    
-0000a830: 2020 2020 2020 2020 666c 6167 203d 2070          flag = p
-0000a840: 6172 616d 5b27 636d 645f 666c 6167 275d  aram['cmd_flag']
-0000a850: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
-0000a860: 6720 3d20 666c 6167 202b 2022 2024 2220  g = flag + " $" 
-0000a870: 2b20 7061 7261 6d5b 276e 616d 6527 5d2e  + param['name'].
-0000a880: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-0000a890: 2020 2020 666c 6167 732e 6170 7065 6e64      flags.append
-0000a8a0: 2866 6c61 6729 0a20 2020 2020 2020 2073  (flag).        s
-0000a8b0: 7562 735b 2750 4152 414d 5327 5d20 3d20  ubs['PARAMS'] = 
-0000a8c0: 2220 222e 6a6f 696e 2866 6c61 6773 290a  " ".join(flags).
-0000a8d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000a8e0: 7562 730a 0a20 2020 2064 6566 2075 7064  ubs..    def upd
-0000a8f0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
-0000a900: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 2020 2067 656e 6572 6174 655f 6a6f       generate_jo
-0000a930: 6273 3a20 626f 6f6c 203d 2046 616c 7365  bs: bool = False
-0000a940: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a960: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
-0000a970: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
-0000a980: 6f6e 6529 202d 3e20 5265 7375 6c74 3a0a  one) -> Result:.
-0000a990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000a9a0: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
-0000a9b0: 6c6f 6361 6c20 636f 7079 206f 6620 7468  local copy of th
-0000a9c0: 6520 536c 7572 6d20 6a6f 6220 7375 626d  e Slurm job subm
-0000a9d0: 6973 7369 6f6e 2073 6372 6970 7473 2e0a  ission scripts..
-0000a9e0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
-0000a9f0: 6e63 7469 6f6e 2070 756c 6c73 2074 6865  nction pulls the
-0000aa00: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
-0000aa10: 6f66 2074 6865 2073 6372 6970 7473 2066  of the scripts f
-0000aa20: 726f 6d20 7468 6520 4769 740a 2020 2020  rom the Git.    
-0000aa30: 2020 2020 7265 706f 7369 746f 7279 2061      repository a
-0000aa40: 6e64 2063 6f70 6965 7320 7468 656d 2074  nd copies them t
-0000aa50: 6f20 7468 6520 736c 7572 6d5f 7363 7269  o the slurm_scri
-0000aa60: 7074 5f70 6174 6820 6469 7265 6374 6f72  pt_path director
-0000aa70: 792e 0a20 2020 2020 2020 2041 6c74 6572  y..        Alter
-0000aa80: 6e61 7469 7665 6c79 2c20 6974 2063 616e  natively, it can
-0000aa90: 2067 656e 6572 6174 6520 7363 7269 7074   generate script
-0000aaa0: 7320 6672 6f6d 2061 2074 656d 706c 6174  s from a templat
-0000aab0: 652e 2054 6869 7320 6973 2074 6865 0a20  e. This is the. 
-0000aac0: 2020 2020 2020 2064 6566 6175 6c74 2062         default b
-0000aad0: 6568 6176 696f 7220 6966 206e 6f20 4769  ehavior if no Gi
-0000aae0: 7420 7265 706f 2069 7320 7072 6f76 6964  t repo is provid
-0000aaf0: 6564 206f 7220 6361 6e20 6265 2066 6f72  ed or can be for
-0000ab00: 6365 6420 7669 6120 7468 650a 2020 2020  ced via the.    
-0000ab10: 2020 2020 6067 656e 6572 6174 655f 6a6f      `generate_jo
-0000ab20: 6273 6020 7061 7261 6d65 7465 722e 0a0a  bs` parameter...
-0000ab30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000ab40: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
-0000ab50: 7465 5f6a 6f62 7320 2862 6f6f 6c29 3a20  te_jobs (bool): 
-0000ab60: 5768 6574 6865 7220 746f 2067 656e 6572  Whether to gener
-0000ab70: 6174 6520 6e65 7720 736c 7572 6d20 6a6f  ate new slurm jo
-0000ab80: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
-0000ab90: 2020 2020 2020 2020 2020 494e 5354 4541            INSTEA
-0000aba0: 4420 286f 6620 7075 6c6c 696e 6720 6672  D (of pulling fr
-0000abb0: 6f6d 2067 6974 292e 2044 6566 6175 6c74  om git). Default
-0000abc0: 7320 746f 2046 616c 7365 2c20 6578 6365  s to False, exce
-0000abd0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
-0000abe0: 2020 2069 6620 6e6f 2073 6c75 726d 5f73     if no slurm_s
-0000abf0: 6372 6970 745f 7265 706f 2069 7320 636f  cript_repo is co
-0000ac00: 6e66 6967 7572 6564 2e0a 2020 2020 2020  nfigured..      
-0000ac10: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-0000ac20: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-0000ac30: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-0000ac40: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-0000ac50: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
-0000ac60: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
-0000ac70: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-0000ac80: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-0000ac90: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-0000aca0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000acb0: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
-0000acc0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-0000acd0: 2063 6f6d 6d61 6e64 2e0a 2020 2020 2020   command..      
-0000ace0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000acf0: 206e 6f74 2073 656c 662e 736c 7572 6d5f   not self.slurm_
-0000ad00: 7363 7269 7074 5f72 6570 6f3a 0a20 2020  script_repo:.   
-0000ad10: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-0000ad20: 655f 6a6f 6273 203d 2054 7275 650a 0a20  e_jobs = True.. 
-0000ad30: 2020 2020 2020 2069 6620 6765 6e65 7261         if genera
-0000ad40: 7465 5f6a 6f62 733a 0a20 2020 2020 2020  te_jobs:.       
-0000ad50: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000ad60: 2822 4765 6e65 7261 7469 6e67 2053 6c75  ("Generating Slu
-0000ad70: 726d 206a 6f62 2073 6372 6970 7473 2229  rm job scripts")
-0000ad80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000ad90: 2077 662c 206a 6f62 5f70 6174 6820 696e   wf, job_path in
-0000ada0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-0000adb0: 6c5f 6a6f 6273 2e69 7465 6d73 2829 3a0a  l_jobs.items():.
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 2320 6765 6e65 7261 7465 206a 6f62 2073  # generate job s
-0000ade0: 6372 6970 740a 2020 2020 2020 2020 2020  cript.          
-0000adf0: 2020 2020 2020 7061 7261 6d73 203d 2073        params = s
-0000ae00: 656c 662e 6765 745f 776f 726b 666c 6f77  elf.get_workflow
-0000ae10: 5f70 6172 616d 6574 6572 7328 7766 290a  _parameters(wf).
-0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae30: 7375 6273 203d 2073 656c 662e 776f 726b  subs = self.work
-0000ae40: 666c 6f77 5f70 6172 616d 735f 746f 5f73  flow_params_to_s
-0000ae50: 7562 7328 7061 7261 6d73 290a 2020 2020  ubs(params).    
-0000ae60: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000ae70: 7363 7269 7074 203d 2073 656c 662e 6765  script = self.ge
-0000ae80: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
-0000ae90: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7766  _for_workflow(wf
-0000aea0: 2c20 7375 6273 290a 2020 2020 2020 2020  , subs).        
-0000aeb0: 2020 2020 2020 2020 2320 656e 7375 7265          # ensure
-0000aec0: 2061 6c6c 2064 6972 7320 6578 6973 7420   all dirs exist 
-0000aed0: 7265 6d6f 7465 6c79 0a20 2020 2020 2020  remotely.       
-0000aee0: 2020 2020 2020 2020 2066 756c 6c5f 7061           full_pa
-0000aef0: 7468 203d 2073 656c 662e 736c 7572 6d5f  th = self.slurm_
-0000af00: 7363 7269 7074 5f70 6174 682b 222f 222b  script_path+"/"+
-0000af10: 6a6f 625f 7061 7468 0a20 2020 2020 2020  job_path.       
-0000af20: 2020 2020 2020 2020 206a 6f62 5f64 6972           job_dir
-0000af30: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
-0000af40: 6c69 7428 6675 6c6c 5f70 6174 6829 0a20  lit(full_path). 
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000af60: 656c 662e 7275 6e28 6622 6d6b 6469 7220  elf.run(f"mkdir 
-0000af70: 2d70 207b 6a6f 625f 6469 727d 2229 0a20  -p {job_dir}"). 
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000af90: 2063 6f70 7920 746f 2072 656d 6f74 6520   copy to remote 
-0000afa0: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-0000afb0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-0000afc0: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
-0000afd0: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
-0000afe0: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 2020 2020 2020 2020 7265 6d6f 7465 3d66          remote=f
-0000b010: 756c 6c5f 7061 7468 290a 2020 2020 2020  ull_path).      
-0000b020: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b030: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
-0000b040: 6574 5f75 7064 6174 655f 736c 7572 6d5f  et_update_slurm_
-0000b050: 7363 7269 7074 735f 636f 6d6d 616e 6428  scripts_command(
-0000b060: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-0000b070: 6767 6572 2e69 6e66 6f28 2255 7064 6174  gger.info("Updat
-0000b080: 696e 6720 536c 7572 6d20 6a6f 6220 7363  ing Slurm job sc
-0000b090: 7269 7074 7320 6f6e 2053 6c75 726d 2229  ripts on Slurm")
-0000b0a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000b0b0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-0000b0c0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
-0000b0d0: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
-0000b0e0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0000b0f0: 2020 2064 6566 2072 756e 5f77 6f72 6b66     def run_workf
-0000b100: 6c6f 7728 7365 6c66 2c0a 2020 2020 2020  low(self,.      
-0000b110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000b120: 6f72 6b66 6c6f 775f 6e61 6d65 3a20 7374  orkflow_name: st
-0000b130: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000b140: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000b150: 5f76 6572 7369 6f6e 3a20 7374 722c 0a20  _version: str,. 
-0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2020 2020 696e 7075 745f 6461 7461 3a20      input_data: 
-0000b180: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000b190: 2020 2020 2020 2020 2020 656d 6169 6c3a            email:
-0000b1a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000b1b0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0000b1c0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000b1d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000b1e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b1f0: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-0000b200: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
-0000b210: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-0000b220: 5475 706c 655b 5265 7375 6c74 2c20 696e  Tuple[Result, in
-0000b230: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-0000b240: 2020 2020 2020 2020 5275 6e20 6120 7370          Run a sp
-0000b250: 6563 6966 6965 6420 776f 726b 666c 6f77  ecified workflow
-0000b260: 206f 6e20 536c 7572 6d20 7573 696e 6720   on Slurm using 
-0000b270: 7468 6520 6769 7665 6e20 7061 7261 6d65  the given parame
-0000b280: 7465 7273 2e0a 0a20 2020 2020 2020 2041  ters...        A
-0000b290: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000b2a0: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
-0000b2b0: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
-0000b2c0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
-0000b2d0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
-0000b2e0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
-0000b2f0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
-0000b300: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
-0000b310: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
-0000b320: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
-0000b330: 2020 206f 6e20 536c 7572 6d29 2e0a 2020     on Slurm)..  
-0000b340: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000b350: 6461 7461 2028 7374 7229 3a20 4e61 6d65  data (str): Name
-0000b360: 206f 6620 7468 6520 696e 7075 7420 6461   of the input da
-0000b370: 7461 2066 6f6c 6465 7220 636f 6e74 6169  ta folder contai
-0000b380: 6e69 6e67 2069 6e70 7574 0a20 2020 2020  ning input.     
-0000b390: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0000b3a0: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
-0000b3b0: 2020 2020 656d 6169 6c20 2873 7472 2c20      email (str, 
-0000b3c0: 6f70 7469 6f6e 616c 293a 2045 6d61 696c  optional): Email
-0000b3d0: 2061 6464 7265 7373 2066 6f72 2053 6c75   address for Slu
-0000b3e0: 726d 206a 6f62 206e 6f74 6966 6963 6174  rm job notificat
-0000b3f0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000b400: 2020 7469 6d65 2028 7374 722c 206f 7074    time (str, opt
-0000b410: 696f 6e61 6c29 3a20 5469 6d65 206c 696d  ional): Time lim
-0000b420: 6974 2066 6f72 2074 6865 2053 6c75 726d  it for the Slurm
-0000b430: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
-0000b440: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000b450: 6d61 7420 4848 3a4d 4d3a 5353 2e0a 2020  mat HH:MM:SS..  
-0000b460: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000b470: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
-0000b480: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000b490: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
-0000b4a0: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
-0000b4b0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000b4c0: 2054 7570 6c65 5b52 6573 756c 742c 2069   Tuple[Result, i
-0000b4d0: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
-0000b4e0: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
-0000b4f0: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
-0000b500: 6c74 206f 6620 7374 6172 7469 6e67 2074  lt of starting t
-0000b510: 6865 2077 6f72 6b66 6c6f 7720 6a6f 6220  he workflow job 
-0000b520: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-0000b530: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
-0000b540: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
-0000b550: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
-0000b560: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
-0000b570: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
-0000b580: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0000b590: 2053 6c75 726d 206a 6f62 2049 4420 6973   Slurm job ID is
-0000b5a0: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
-0000b5b0: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
-0000b5c0: 6520 0a20 2020 2020 2020 2020 2020 2060  e .            `
-0000b5d0: 7275 6e5f 636f 6d6d 616e 6473 6020 6d65  run_commands` me
-0000b5e0: 7468 6f64 2e0a 2020 2020 2020 2020 2222  thod..        ""
-0000b5f0: 220a 2020 2020 2020 2020 7362 6174 6368  ".        sbatch
-0000b600: 5f63 6d64 2c20 7362 6174 6368 5f65 6e76  _cmd, sbatch_env
-0000b610: 203d 2073 656c 662e 6765 745f 776f 726b   = self.get_work
-0000b620: 666c 6f77 5f63 6f6d 6d61 6e64 280a 2020  flow_command(.  
-0000b630: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000b640: 6f77 5f6e 616d 652c 2077 6f72 6b66 6c6f  ow_name, workflo
-0000b650: 775f 7665 7273 696f 6e2c 2069 6e70 7574  w_version, input
-0000b660: 5f64 6174 612c 2065 6d61 696c 2c20 7469  _data, email, ti
-0000b670: 6d65 2c20 2a2a 6b77 6172 6773 290a 2020  me, **kwargs).  
-0000b680: 2020 2020 2020 7072 696e 7428 6622 5275        print(f"Ru
-0000b690: 6e6e 696e 6720 7b77 6f72 6b66 6c6f 775f  nning {workflow_
-0000b6a0: 6e61 6d65 7d20 6a6f 6220 6f6e 207b 696e  name} job on {in
-0000b6b0: 7075 745f 6461 7461 7d20 6f6e 2053 6c75  put_data} on Slu
-0000b6c0: 726d 3a5c 0a20 2020 2020 2020 2020 2020  rm:\.           
-0000b6d0: 207b 7362 6174 6368 5f63 6d64 7d20 772f   {sbatch_cmd} w/
-0000b6e0: 207b 7362 6174 6368 5f65 6e76 7d22 290a   {sbatch_env}").
-0000b6f0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-0000b700: 6e66 6f28 6622 5275 6e6e 696e 6720 7b77  nfo(f"Running {w
-0000b710: 6f72 6b66 6c6f 775f 6e61 6d65 7d20 6a6f  orkflow_name} jo
-0000b720: 6220 6f6e 207b 696e 7075 745f 6461 7461  b on {input_data
-0000b730: 7d20 6f6e 2053 6c75 726d 2229 0a20 2020  } on Slurm").   
-0000b740: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-0000b750: 7275 6e5f 636f 6d6d 616e 6473 285b 7362  run_commands([sb
-0000b760: 6174 6368 5f63 6d64 5d2c 2073 6261 7463  atch_cmd], sbatc
-0000b770: 685f 656e 7629 0a20 2020 2020 2020 2072  h_env).        r
-0000b780: 6574 7572 6e20 7265 732c 2073 656c 662e  eturn res, self.
-0000b790: 6578 7472 6163 745f 6a6f 625f 6964 2872  extract_job_id(r
-0000b7a0: 6573 290a 0a20 2020 2064 6566 2072 756e  es)..    def run
-0000b7b0: 5f77 6f72 6b66 6c6f 775f 6a6f 6228 7365  _workflow_job(se
-0000b7c0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000b7d0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000b7e0: 6b66 6c6f 775f 6e61 6d65 3a20 7374 722c  kflow_name: str,
-0000b7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b800: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000b810: 6f77 5f76 6572 7369 6f6e 3a20 7374 722c  ow_version: str,
-0000b820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b830: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000b840: 6461 7461 3a20 7374 722c 0a20 2020 2020  data: str,.     
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 656d 6169 6c3a 204f 7074 696f      email: Optio
-0000b870: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000b880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b890: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
-0000b8a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000b8b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000b8d0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
-0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8f0: 2029 202d 3e20 536c 7572 6d4a 6f62 3a0a   ) -> SlurmJob:.
-0000b900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b910: 2020 2020 5275 6e20 6120 7370 6563 6966      Run a specif
-0000b920: 6965 6420 776f 726b 666c 6f77 206f 6e20  ied workflow on 
-0000b930: 536c 7572 6d20 7573 696e 6720 7468 6520  Slurm using the 
-0000b940: 6769 7665 6e20 7061 7261 6d65 7465 7273  given parameters
-0000b950: 2061 6e64 2072 6574 7572 6e20 6120 536c   and return a Sl
-0000b960: 7572 6d4a 6f62 2069 6e73 7461 6e63 652e  urmJob instance.
-0000b970: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000b980: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000b990: 666c 6f77 5f6e 616d 6520 2873 7472 293a  flow_name (str):
-0000b9a0: 204e 616d 6520 6f66 2074 6865 2077 6f72   Name of the wor
-0000b9b0: 6b66 6c6f 7720 746f 2065 7865 6375 7465  kflow to execute
-0000b9c0: 2e0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
-0000b9d0: 726b 666c 6f77 5f76 6572 7369 6f6e 2028  rkflow_version (
-0000b9e0: 7374 7229 3a20 5665 7273 696f 6e20 6f66  str): Version of
-0000b9f0: 2074 6865 2077 6f72 6b66 6c6f 7720 2869   the workflow (i
-0000ba00: 6d61 6765 2076 6572 7369 6f6e 206f 6e20  mage version on 
-0000ba10: 536c 7572 6d29 2e0a 2020 2020 2020 2020  Slurm)..        
-0000ba20: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
-0000ba30: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
-0000ba40: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
-0000ba50: 6465 7220 636f 6e74 6169 6e69 6e67 2069  der containing i
-0000ba60: 6e70 7574 2069 6d61 6765 2066 696c 6573  nput image files
-0000ba70: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
-0000ba80: 6169 6c20 2873 7472 2c20 6f70 7469 6f6e  ail (str, option
-0000ba90: 616c 293a 2045 6d61 696c 2061 6464 7265  al): Email addre
-0000baa0: 7373 2066 6f72 2053 6c75 726d 206a 6f62  ss for Slurm job
-0000bab0: 206e 6f74 6966 6963 6174 696f 6e73 2e0a   notifications..
-0000bac0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000bad0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0000bae0: 3a20 5469 6d65 206c 696d 6974 2066 6f72  : Time limit for
-0000baf0: 2074 6865 2053 6c75 726d 206a 6f62 2069   the Slurm job i
-0000bb00: 6e20 7468 6520 666f 726d 6174 2048 483a  n the format HH:
-0000bb10: 4d4d 3a53 532e 0a20 2020 2020 2020 2020  MM:SS..         
-0000bb20: 2020 202a 2a6b 7761 7267 733a 2041 6464     **kwargs: Add
-0000bb30: 6974 696f 6e61 6c20 6b65 7977 6f72 6420  itional keyword 
-0000bb40: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
-0000bb50: 6520 776f 726b 666c 6f77 2e0a 0a20 2020  e workflow...   
-0000bb60: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000bb70: 2020 2020 2020 2020 2020 536c 7572 6d4a            SlurmJ
-0000bb80: 6f62 3a20 4120 536c 7572 6d4a 6f62 2069  ob: A SlurmJob i
-0000bb90: 6e73 7461 6e63 6520 7265 7072 6573 656e  nstance represen
-0000bba0: 7469 6e67 2074 6865 2073 7461 7274 6564  ting the started
-0000bbb0: 2077 6f72 6b66 6c6f 7720 6a6f 622e 0a20   workflow job.. 
-0000bbc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000bbd0: 2020 2072 6573 756c 742c 206a 6f62 5f69     result, job_i
-0000bbe0: 6420 3d20 7365 6c66 2e72 756e 5f77 6f72  d = self.run_wor
-0000bbf0: 6b66 6c6f 7728 0a20 2020 2020 2020 2020  kflow(.         
-0000bc00: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
-0000bc10: 2c20 776f 726b 666c 6f77 5f76 6572 7369  , workflow_versi
-0000bc20: 6f6e 2c20 696e 7075 745f 6461 7461 2c20  on, input_data, 
-0000bc30: 656d 6169 6c2c 2074 696d 652c 202a 2a6b  email, time, **k
-0000bc40: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
-0000bc50: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
-0000bc60: 6573 756c 742c 206a 6f62 5f69 6429 0a0a  esult, job_id)..
-0000bc70: 2020 2020 6465 6620 7275 6e5f 636f 6e76      def run_conv
-0000bc80: 6572 7369 6f6e 5f77 6f72 6b66 6c6f 775f  ersion_workflow_
-0000bc90: 6a6f 6228 7365 6c66 2c20 666f 6c64 6572  job(self, folder
-0000bca0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 736f 7572 6365 5f66 6f72 6d61 743a 2073  source_format: s
-0000bce0: 7472 203d 2027 7a61 7272 272c 0a20 2020  tr = 'zarr',.   
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
-0000bd20: 7374 7220 3d20 2774 6966 6627 0a20 2020  str = 'tiff'.   
-0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 2029 202d 3e20 5475 706c 655b 5265 7375   ) -> Tuple[Resu
-0000bd60: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
-0000bd70: 2020 2222 220a 2020 2020 2020 2020 5275    """.        Ru
-0000bd80: 6e20 7468 6520 6461 7461 2063 6f6e 7665  n the data conve
-0000bd90: 7273 696f 6e20 776f 726b 666c 6f77 206f  rsion workflow o
-0000bda0: 6e20 536c 7572 6d20 7573 696e 6720 7468  n Slurm using th
-0000bdb0: 6520 6769 7665 6e20 6461 7461 2066 6f6c  e given data fol
-0000bdc0: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
-0000bdd0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000bde0: 666f 6c64 6572 5f6e 616d 6520 2873 7472  folder_name (str
-0000bdf0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
-0000be00: 6865 2064 6174 6120 666f 6c64 6572 2063  he data folder c
-0000be10: 6f6e 7461 696e 696e 6720 736f 7572 6365  ontaining source
-0000be20: 2066 6f72 6d61 7420 6669 6c65 732e 0a20   format files.. 
-0000be30: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0000be40: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
-0000be50: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
-0000be60: 6174 2066 6f72 2063 6f6e 7665 7273 696f  at for conversio
-0000be70: 6e20 2864 6566 6175 6c74 2069 7320 277a  n (default is 'z
-0000be80: 6172 7227 292e 0a20 2020 2020 2020 2020  arr')..         
-0000be90: 2020 2074 6172 6765 745f 666f 726d 6174     target_format
-0000bea0: 2028 7374 7229 3a20 5461 7267 6574 2064   (str): Target d
-0000beb0: 6174 6120 666f 726d 6174 2061 6674 6572  ata format after
-0000bec0: 2063 6f6e 7665 7273 696f 6e20 2864 6566   conversion (def
-0000bed0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
-0000bee0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000bef0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0000bf00: 7570 6c65 5b52 6573 756c 742c 2069 6e74  uple[Result, int
-0000bf10: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000bf20: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-0000bf30: 696e 696e 6720 7468 6520 7265 7375 6c74  ining the result
-0000bf40: 206f 6620 7374 6172 7469 6e67 2074 6865   of starting the
-0000bf50: 2063 6f6e 7665 7273 696f 6e20 6a6f 6220   conversion job 
-0000bf60: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-0000bf70: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
-0000bf80: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
-0000bf90: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
-0000bfa0: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
-0000bfb0: 2e0a 0a20 2020 2020 2020 2057 6172 6e69  ...        Warni
-0000bfc0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-0000bfd0: 5468 6520 6465 6661 756c 7420 696d 706c  The default impl
-0000bfe0: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
-0000bff0: 7375 7070 6f72 7473 2063 6f6e 7665 7273  supports convers
-0000c000: 696f 6e20 6672 6f6d 2027 7a61 7272 2720  ion from 'zarr' 
-0000c010: 746f 2027 7469 6666 272e 0a20 2020 2020  to 'tiff'..     
-0000c020: 2020 2020 2020 2049 6620 7573 696e 6720         If using 
-0000c030: 6f74 6865 7220 736f 7572 6365 206f 7220  other source or 
-0000c040: 7461 7267 6574 2066 6f72 6d61 7473 2c20  target formats, 
-0000c050: 7573 6572 7320 6d75 7374 2069 6d70 6c65  users must imple
-0000c060: 6d65 6e74 2061 6e64 2063 6f6e 6669 6775  ment and configu
-0000c070: 7265 0a20 2020 2020 2020 2020 2020 2061  re.            a
-0000c080: 6464 6974 696f 6e61 6c20 636f 6e76 6572  dditional conver
-0000c090: 7465 7273 2074 6865 6d73 656c 7665 732e  ters themselves.
-0000c0a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c0b0: 2020 2020 2023 2047 656e 6572 6174 6520       # Generate 
-0000c0c0: 6120 756e 6971 7565 2063 6f6e 6669 6720  a unique config 
-0000c0d0: 6669 6c65 206e 616d 650a 2020 2020 2020  file name.      
-0000c0e0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
-0000c0f0: 6622 636f 6e66 6967 5f7b 666f 6c64 6572  f"config_{folder
-0000c100: 5f6e 616d 657d 2e74 7874 220a 0a20 2020  _name}.txt"..   
-0000c110: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
-0000c120: 2061 6c6c 2063 6f6d 6d61 6e64 7320 746f   all commands to
-0000c130: 2072 756e 2063 6f6e 7365 6375 7469 7665   run consecutive
-0000c140: 6c79 0a20 2020 2020 2020 2064 6174 615f  ly.        data_
-0000c150: 7061 7468 203d 2066 227b 7365 6c66 2e73  path = f"{self.s
-0000c160: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
-0000c170: 7b66 6f6c 6465 725f 6e61 6d65 7d22 0a20  {folder_name}". 
-0000c180: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
-0000c190: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
-0000c1a0: 7620 3d20 7365 6c66 2e67 6574 5f63 6f6e  v = self.get_con
-0000c1b0: 7665 7273 696f 6e5f 636f 6d6d 616e 6428  version_command(
-0000c1c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000c1d0: 615f 7061 7468 2c20 636f 6e66 6967 5f66  a_path, config_f
-0000c1e0: 696c 652c 2073 6f75 7263 655f 666f 726d  ile, source_form
-0000c1f0: 6174 2c20 7461 7267 6574 5f66 6f72 6d61  at, target_forma
-0000c200: 7429 0a20 2020 2020 2020 2063 6f6d 6d61  t).        comma
-0000c210: 6e64 7320 3d20 5b0a 2020 2020 2020 2020  nds = [.        
-0000c220: 2020 2020 6622 6669 6e64 207b 6461 7461      f"find {data
-0000c230: 5f70 6174 687d 2f64 6174 612f 696e 202d  _path}/data/in -
-0000c240: 6e61 6d65 2027 2a2e 7b73 6f75 7263 655f  name '*.{source_
-0000c250: 666f 726d 6174 7d27 207c 2061 776b 2027  format}' | awk '
-0000c260: 7b7b 7072 696e 7420 4e52 2c20 2430 7d7d  {{print NR, $0}}
-0000c270: 2720 3e20 7b63 6f6e 6669 675f 6669 6c65  ' > {config_file
-0000c280: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-0000c290: 6622 4e3d 2428 7763 202d 6c20 3c20 5c22  f"N=$(wc -l < \"
-0000c2a0: 7b63 6f6e 6669 675f 6669 6c65 7d5c 2229  {config_file}\")
-0000c2b0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
-0000c2c0: 2265 6368 6f20 5c22 4e75 6d62 6572 206f  "echo \"Number o
-0000c2d0: 6620 2e7b 736f 7572 6365 5f66 6f72 6d61  f .{source_forma
-0000c2e0: 747d 2066 696c 6573 3a20 244e 5c22 222c  t} files: $N\"",
-0000c2f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000c300: 7665 7273 696f 6e5f 636d 640a 2020 2020  version_cmd.    
-0000c310: 2020 2020 5d0a 0a20 2020 2020 2020 2023      ]..        #
-0000c320: 2052 756e 2061 6c6c 2063 6f6d 6d61 6e64   Run all command
-0000c330: 7320 636f 6e73 6563 7574 6976 656c 790a  s consecutively.
-0000c340: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-0000c350: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-0000c360: 636f 6d6d 616e 6473 2c20 7362 6174 6368  commands, sbatch
-0000c370: 5f65 6e76 290a 0a20 2020 2020 2020 2072  _env)..        r
-0000c380: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
-0000c390: 6573 2c20 7365 6c66 2e65 7874 7261 6374  es, self.extract
-0000c3a0: 5f6a 6f62 5f69 6428 7265 7329 290a 0a20  _job_id(res)).. 
-0000c3b0: 2020 2064 6566 2065 7874 7261 6374 5f6a     def extract_j
-0000c3c0: 6f62 5f69 6428 7365 6c66 2c20 7265 7375  ob_id(self, resu
-0000c3d0: 6c74 3a20 5265 7375 6c74 2920 2d3e 2069  lt: Result) -> i
-0000c3e0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-0000c3f0: 2020 2020 2020 2020 4578 7472 6163 7420          Extract 
-0000c400: 7468 6520 536c 7572 6d20 6a6f 6220 4944  the Slurm job ID
-0000c410: 2066 726f 6d20 7468 6520 7265 7375 6c74   from the result
-0000c420: 206f 6620 6120 636f 6d6d 616e 642e 0a0a   of a command...
-0000c430: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c440: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000c450: 2028 5265 7375 6c74 293a 2054 6865 2072   (Result): The r
-0000c460: 6573 756c 7420 6f66 2061 2063 6f6d 6d61  esult of a comma
-0000c470: 6e64 2065 7865 6375 7469 6f6e 2e0a 0a20  nd execution... 
-0000c480: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000c490: 2020 2020 2020 2020 2020 2020 696e 743a              int:
-0000c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4b0: 2054 6865 2053 6c75 726d 206a 6f62 2049   The Slurm job I
-0000c4c0: 4420 6578 7472 6163 7465 6420 6672 6f6d  D extracted from
-0000c4d0: 2074 6865 2072 6573 756c 742c 0a20 2020   the result,.   
-0000c4e0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000c4f0: 2d31 2069 6620 6e6f 7420 666f 756e 642e  -1 if not found.
-0000c500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c510: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-0000c520: 6420 3d20 6e65 7874 2828 696e 7428 732e  d = next((int(s.
-0000c530: 7374 7269 7028 2929 2066 6f72 2073 2069  strip()) for s i
-0000c540: 6e20 7265 7375 6c74 2e73 7464 6f75 742e  n result.stdout.
-0000c550: 7370 6c69 7428 0a20 2020 2020 2020 2020  split(.         
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2020 2022 5375 626d 6974 7465 6420 6261     "Submitted ba
-0000c580: 7463 6820 6a6f 6222 2920 6966 2073 2e73  tch job") if s.s
-0000c590: 7472 6970 2829 2e69 7364 6967 6974 2829  trip().isdigit()
-0000c5a0: 292c 202d 3129 0a20 2020 2020 2020 2072  ), -1).        r
-0000c5b0: 6574 7572 6e20 736c 7572 6d5f 6a6f 625f  eturn slurm_job_
-0000c5c0: 6964 0a0a 2020 2020 6465 6620 6765 745f  id..    def get_
-0000c5d0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
-0000c5e0: 6970 7473 5f63 6f6d 6d61 6e64 2873 656c  ipts_command(sel
-0000c5f0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-0000c600: 2020 2022 2222 4765 6e65 7261 7465 2074     """Generate t
-0000c610: 6865 2063 6f6d 6d61 6e64 2074 6f20 7570  he command to up
-0000c620: 6461 7465 2074 6865 2047 6974 2072 6570  date the Git rep
-0000c630: 6f73 6974 6f72 7920 636f 6e74 6169 6e69  ository containi
-0000c640: 6e67 0a20 2020 2020 2020 2074 6865 2053  ng.        the S
-0000c650: 6c75 726d 2073 6372 6970 7473 2c20 6966  lurm scripts, if
-0000c660: 206e 6563 6573 7361 7279 2e0a 0a20 2020   necessary...   
-0000c670: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000c680: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0000c6a0: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
-0000c6b0: 6e67 2074 6865 2047 6974 2063 6f6d 6d61  ng the Git comma
-0000c6c0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-0000c6d0: 2020 2074 6f20 7570 6461 7465 2074 6865     to update the
-0000c6e0: 2053 6c75 726d 2073 6372 6970 7473 2e0a   Slurm scripts..
-0000c6f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c700: 2020 2020 7570 6461 7465 5f63 6d64 203d      update_cmd =
-0000c710: 2066 2267 6974 202d 4320 7b73 656c 662e   f"git -C {self.
-0000c720: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
-0000c730: 687d 2070 756c 6c22 0a20 2020 2020 2020  h} pull".       
-0000c740: 2072 6574 7572 6e20 7570 6461 7465 5f63   return update_c
-0000c750: 6d64 0a0a 2020 2020 6465 6620 6368 6563  md..    def chec
-0000c760: 6b5f 6a6f 625f 7374 6174 7573 2873 656c  k_job_status(sel
-0000c770: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-0000c780: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-0000c790: 6d5f 6a6f 625f 6964 733a 204c 6973 745b  m_job_ids: List[
-0000c7a0: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c7c0: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
-0000c7d0: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
-0000c7e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000c7f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-0000c800: 3e20 5475 706c 655b 4469 6374 5b69 6e74  > Tuple[Dict[int
-0000c810: 2c20 7374 725d 2c20 5265 7375 6c74 5d3a  , str], Result]:
-0000c820: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c830: 2020 2020 2043 6865 636b 2074 6865 2073       Check the s
-0000c840: 7461 7475 7320 6f66 2053 6c75 726d 206a  tatus of Slurm j
-0000c850: 6f62 7320 7769 7468 2074 6865 2067 6976  obs with the giv
-0000c860: 656e 206a 6f62 2049 4473 2e0a 0a20 2020  en job IDs...   
-0000c870: 2020 2020 204e 6f74 653a 2054 6869 7320       Note: This 
-0000c880: 646f 6573 6e27 7420 7265 7475 726e 206a  doesn't return j
-0000c890: 6f62 2061 7272 6179 7320 696e 6469 7669  ob arrays indivi
-0000c8a0: 6475 616c 6c79 2e0a 2020 2020 2020 2020  dually..        
-0000c8b0: 4974 2074 616b 6573 2074 6865 206c 6173  It takes the las
-0000c8c0: 7420 7661 6c75 6520 7265 7475 726e 6564  t value returned
-0000c8d0: 2066 6f72 2074 686f 7365 2073 7562 2069   for those sub i
-0000c8e0: 6473 200a 2020 2020 2020 2020 2867 656e  ds .        (gen
-0000c8f0: 6572 616c 6c79 2074 6865 206f 6e65 2073  erally the one s
-0000c900: 7469 6c6c 2050 454e 4449 4e47 292e 0a0a  till PENDING)...
-0000c910: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c920: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-0000c930: 6a6f 625f 6964 7320 284c 6973 745b 696e  job_ids (List[in
-0000c940: 745d 293a 2054 6865 206a 6f62 2049 4473  t]): The job IDs
-0000c950: 206f 6620 7468 6520 536c 7572 6d20 6a6f   of the Slurm jo
-0000c960: 6273 2074 6f20 6368 6563 6b2e 0a20 2020  bs to check..   
-0000c970: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-0000c980: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-0000c990: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-0000c9a0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-0000c9b0: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
-0000c9c0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
-0000c9d0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
-0000c9e0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
-0000c9f0: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
-0000ca00: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000ca10: 2020 2020 2020 2020 2054 7570 6c65 5b44           Tuple[D
-0000ca20: 6963 745b 696e 742c 2073 7472 5d2c 2052  ict[int, str], R
-0000ca30: 6573 756c 745d 3a0a 2020 2020 2020 2020  esult]:.        
-0000ca40: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
-0000ca50: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
-0000ca60: 7461 7475 7320 7065 7220 696e 7075 7420  tatus per input 
-0000ca70: 4944 2061 6e64 2074 6865 2072 6573 756c  ID and the resul
-0000ca80: 7420 6f66 200a 2020 2020 2020 2020 2020  t of .          
-0000ca90: 2020 2020 2020 7468 6520 636f 6d6d 616e        the comman
-0000caa0: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
-0000cab0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-0000cac0: 2020 2020 2020 2020 2020 5353 4845 7863            SSHExc
-0000cad0: 6570 7469 6f6e 3a20 4966 2074 6865 2063  eption: If the c
-0000cae0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
-0000caf0: 2066 6169 6c73 206f 7220 6e6f 2072 6573   fails or no res
-0000cb00: 706f 6e73 6520 6973 0a20 2020 2020 2020  ponse is.       
-0000cb10: 2020 2020 2020 2020 2072 6563 6569 7665           receive
-0000cb20: 6420 6166 7465 7220 6d75 6c74 6970 6c65  d after multiple
-0000cb30: 2072 6574 7269 6573 2e0a 2020 2020 2020   retries..      
-0000cb40: 2020 2222 220a 2020 2020 2020 2020 636d    """.        cm
-0000cb50: 6420 3d20 7365 6c66 2e67 6574 5f6a 6f62  d = self.get_job
-0000cb60: 5f73 7461 7475 735f 636f 6d6d 616e 6428  _status_command(
-0000cb70: 736c 7572 6d5f 6a6f 625f 6964 7329 0a20  slurm_job_ids). 
-0000cb80: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000cb90: 666f 2866 2247 6574 7469 6e67 2073 7461  fo(f"Getting sta
-0000cba0: 7475 7320 6f66 207b 736c 7572 6d5f 6a6f  tus of {slurm_jo
-0000cbb0: 625f 6964 737d 206f 6e20 536c 7572 6d22  b_ids} on Slurm"
-0000cbc0: 290a 2020 2020 2020 2020 7265 7472 795f  ).        retry_
-0000cbd0: 7374 6174 7573 203d 2030 0a20 2020 2020  status = 0.     
-0000cbe0: 2020 2077 6869 6c65 2072 6574 7279 5f73     while retry_s
-0000cbf0: 7461 7475 7320 3c20 333a 0a20 2020 2020  tatus < 3:.     
-0000cc00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000cc10: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000cc20: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
-0000cc30: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-0000cc40: 6767 6572 2e69 6e66 6f28 7265 7375 6c74  gger.info(result
-0000cc50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000cc60: 2072 6573 756c 742e 6f6b 3a0a 2020 2020   result.ok:.    
-0000cc70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000cc80: 6f74 2072 6573 756c 742e 7374 646f 7574  ot result.stdout
-0000cc90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cca0: 2020 2020 2020 2320 7761 6974 2066 6f72        # wait for
-0000ccb0: 2033 2073 6563 6f6e 6473 2062 6566 6f72   3 seconds befor
-0000ccc0: 6520 6368 6563 6b69 6e67 2061 6761 696e  e checking again
-0000ccd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cce0: 2020 2020 2074 696d 6573 6c65 6570 2e73       timesleep.s
-0000ccf0: 6c65 6570 2833 290a 2020 2020 2020 2020  leep(3).        
-0000cd00: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-0000cd10: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
-0000cd20: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
-0000cd30: 6174 7573 202b 3d20 310a 2020 2020 2020  atus += 1.      
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000cd50: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 6622 5265 7472 7920 7b72 6574      f"Retry {ret
-0000cd80: 7279 5f73 7461 7475 737d 2067 6574 7469  ry_status} getti
-0000cd90: 6e67 2073 7461 7475 7320 5c0a 2020 2020  ng status \.    
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2020 2020 2020 2020 6f66 207b 736c 7572          of {slur
-0000cdc0: 6d5f 6a6f 625f 6964 737d 2122 290a 2020  m_job_ids}!").  
-0000cdd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000cde0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cdf0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000ce10: 625f 7374 6174 7573 5f64 6963 7420 3d20  b_status_dict = 
-0000ce20: 7b69 6e74 286c 696e 652e 7370 6c69 7428  {int(line.split(
-0000ce30: 295b 305d 2e73 706c 6974 2827 5f27 295b  )[0].split('_')[
-0000ce40: 305d 293a 206c 696e 652e 7370 6c69 7428  0]): line.split(
-0000ce50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ce60: 2020 2020 2029 5b31 5d20 666f 7220 6c69       )[1] for li
-0000ce70: 6e65 2069 6e20 7265 7375 6c74 2e73 7464  ne in result.std
-0000ce80: 6f75 742e 7370 6c69 7428 225c 6e22 2920  out.split("\n") 
-0000ce90: 6966 206c 696e 657d 0a20 2020 2020 2020  if line}.       
-0000cea0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000ceb0: 6765 722e 6465 6275 6728 6622 4a6f 6220  ger.debug(f"Job 
-0000cec0: 7374 6174 7573 6573 3a20 7b6a 6f62 5f73  statuses: {job_s
-0000ced0: 7461 7475 735f 6469 6374 7d22 290a 2020  tatus_dict}").  
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cef0: 2020 7265 7475 726e 206a 6f62 5f73 7461    return job_sta
-0000cf00: 7475 735f 6469 6374 2c20 7265 7375 6c74  tus_dict, result
-0000cf10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000cf20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000cf30: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
-0000cf40: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
-0000cf50: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
-0000cf60: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000cf70: 6572 726f 7228 6572 726f 7229 0a20 2020  error(error).   
-0000cf80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000cf90: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
-0000cfa0: 6572 726f 7229 0a20 2020 2020 2020 2065  error).        e
-0000cfb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cfc0: 2065 7272 6f72 203d 2066 2245 7272 6f72   error = f"Error
-0000cfd0: 3a20 5265 7472 6965 6420 7b72 6574 7279  : Retried {retry
-0000cfe0: 5f73 7461 7475 737d 2074 696d 6573 2074  _status} times t
-0000cff0: 6f20 6765 7420 5c0a 2020 2020 2020 2020  o get \.        
-0000d000: 2020 2020 2020 2020 7374 6174 7573 206f          status o
-0000d010: 6620 7b73 6c75 726d 5f6a 6f62 5f69 6473  f {slurm_job_ids
-0000d020: 7d2c 2062 7574 206e 6f20 7265 7370 6f6e  }, but no respon
-0000d030: 7365 2e22 0a20 2020 2020 2020 2020 2020  se.".           
-0000d040: 206c 6f67 6765 722e 6572 726f 7228 6572   logger.error(er
-0000d050: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
-0000d060: 2072 6169 7365 2053 5348 4578 6365 7074   raise SSHExcept
-0000d070: 696f 6e28 6572 726f 7229 0a0a 2020 2020  ion(error)..    
-0000d080: 6465 6620 6765 745f 6a6f 625f 7374 6174  def get_job_stat
-0000d090: 7573 5f63 6f6d 6d61 6e64 2873 656c 662c  us_command(self,
-0000d0a0: 2073 6c75 726d 5f6a 6f62 5f69 6473 3a20   slurm_job_ids: 
-0000d0b0: 4c69 7374 5b69 6e74 5d29 202d 3e20 7374  List[int]) -> st
-0000d0c0: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
-0000d0d0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0000d0e0: 6520 536c 7572 6d20 636f 6d6d 616e 6420  e Slurm command 
-0000d0f0: 746f 2067 6574 2074 6865 2073 7461 7475  to get the statu
-0000d100: 7320 6f66 206a 6f62 7320 7769 7468 2074  s of jobs with t
-0000d110: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
-0000d120: 206a 6f62 2049 4473 2e0a 0a20 2020 2020   job IDs...     
-0000d130: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000d140: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-0000d150: 6473 2028 4c69 7374 5b69 6e74 5d29 3a20  ds (List[int]): 
-0000d160: 5468 6520 6a6f 6220 4944 7320 6f66 2074  The job IDs of t
-0000d170: 6865 206a 6f62 7320 746f 2063 6865 636b  he jobs to check
-0000d180: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000d190: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000d1a0: 7374 723a 200a 2020 2020 2020 2020 2020  str: .          
-0000d1b0: 2020 2020 2020 5468 6520 536c 7572 6d20        The Slurm 
-0000d1c0: 636f 6d6d 616e 6420 746f 2067 6574 2074  command to get t
-0000d1d0: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
-0000d1e0: 206a 6f62 732e 0a20 2020 2020 2020 2022   jobs..        "
-0000d1f0: 2222 0a20 2020 2020 2020 2023 2063 6f6e  "".        # con
-0000d200: 6361 7420 6d75 6c74 6970 6c65 206a 6f62  cat multiple job
-0000d210: 7320 6966 206e 6565 6465 640a 2020 2020  s if needed.    
-0000d220: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
-0000d230: 203d 2022 202d 6a20 222e 6a6f 696e 285b   = " -j ".join([
-0000d240: 7374 7228 6964 2920 666f 7220 6964 2069  str(id) for id i
-0000d250: 6e20 736c 7572 6d5f 6a6f 625f 6964 735d  n slurm_job_ids]
-0000d260: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d270: 2073 656c 662e 5f4a 4f42 5f53 5441 5455   self._JOB_STATU
-0000d280: 535f 434d 442e 666f 726d 6174 2873 6c75  S_CMD.format(slu
-0000d290: 726d 5f6a 6f62 5f69 643d 736c 7572 6d5f  rm_job_id=slurm_
-0000d2a0: 6a6f 625f 6964 290a 0a20 2020 2064 6566  job_id)..    def
-0000d2b0: 2065 7874 7261 6374 5f64 6174 615f 6c6f   extract_data_lo
-0000d2c0: 6361 7469 6f6e 5f66 726f 6d5f 6c6f 6728  cation_from_log(
-0000d2d0: 7365 6c66 2c20 736c 7572 6d5f 6a6f 625f  self, slurm_job_
-0000d2e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2020 2020 2020 206c 6f67 6669 6c65 3a20         logfile: 
-0000d320: 7374 7220 3d20 4e6f 6e65 2920 2d3e 2073  str = None) -> s
-0000d330: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
-0000d340: 6561 6420 534c 5552 4d20 6a6f 6220 6c6f  ead SLURM job lo
-0000d350: 6766 696c 6520 746f 2066 696e 6420 6c6f  gfile to find lo
-0000d360: 6361 7469 6f6e 206f 6620 7468 6520 6461  cation of the da
-0000d370: 7461 2e0a 0a20 2020 2020 2020 204f 6e65  ta...        One
-0000d380: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
-0000d390: 7273 2069 7320 7265 7175 6972 6564 2c20  rs is required, 
-0000d3a0: 6569 7468 6572 2069 6420 6f72 2066 696c  either id or fil
-0000d3b0: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-0000d3c0: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
-0000d3d0: 7572 6d5f 6a6f 625f 6964 2028 7374 7229  urm_job_id (str)
-0000d3e0: 3a20 4964 206f 6620 7468 6520 736c 7572  : Id of the slur
-0000d3f0: 6d20 6a6f 620a 2020 2020 2020 2020 2020  m job.          
-0000d400: 2020 6c6f 6766 696c 6520 2873 7472 293a    logfile (str):
-0000d410: 2050 6174 6820 746f 2074 6865 206c 6f67   Path to the log
-0000d420: 6669 6c65 0a0a 2020 2020 2020 2020 5265  file..        Re
-0000d430: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000d440: 2020 2073 7472 3a20 4461 7461 206c 6f63     str: Data loc
-0000d450: 6174 696f 6e20 6163 636f 7264 696e 6720  ation according 
-0000d460: 746f 2074 6865 206c 6f67 0a0a 2020 2020  to the log..    
-0000d470: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-0000d480: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
-0000d490: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
-0000d4a0: 7320 616e 2069 7373 7565 2077 6974 6820  s an issue with 
-0000d4b0: 7468 6520 636f 6d6d 616e 6420 6578 6563  the command exec
-0000d4c0: 7574 696f 6e2e 0a20 2020 2020 2020 2022  ution..        "
-0000d4d0: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
-0000d4e0: 6766 696c 6520 6973 204e 6f6e 6520 616e  gfile is None an
-0000d4f0: 6420 736c 7572 6d5f 6a6f 625f 6964 2069  d slurm_job_id i
-0000d500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000d510: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
-0000d520: 3d20 7365 6c66 2e5f 4c4f 4746 494c 450a  = self._LOGFILE.
-0000d530: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
-0000d540: 696c 6520 3d20 6c6f 6766 696c 652e 666f  ile = logfile.fo
-0000d550: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
-0000d560: 643d 736c 7572 6d5f 6a6f 625f 6964 290a  d=slurm_job_id).
-0000d570: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-0000d580: 6c66 2e5f 4c4f 4746 494c 455f 4441 5441  lf._LOGFILE_DATA
-0000d590: 5f43 4d44 2e66 6f72 6d61 7428 6c6f 675f  _CMD.format(log_
-0000d5a0: 6669 6c65 3d6c 6f67 6669 6c65 290a 2020  file=logfile).  
-0000d5b0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-0000d5c0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-0000d5d0: 285b 636d 645d 290a 2020 2020 2020 2020  ([cmd]).        
-0000d5e0: 6966 2072 6573 756c 742e 6f6b 3a0a 2020  if result.ok:.  
-0000d5f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d600: 2072 6573 756c 742e 7374 646f 7574 0a20   result.stdout. 
-0000d610: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000d620: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000d630: 5348 4578 6365 7074 696f 6e28 7265 7375  SHException(resu
-0000d640: 6c74 290a 0a20 2020 2064 6566 2067 6574  lt)..    def get
-0000d650: 5f77 6f72 6b66 6c6f 775f 7061 7261 6d65  _workflow_parame
-0000d660: 7465 7273 2873 656c 662c 0a20 2020 2020  ters(self,.     
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000d690: 6c6f 773a 2073 7472 2920 2d3e 2044 6963  low: str) -> Dic
-0000d6a0: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
-0000d6b0: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
-0000d6c0: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
-0000d6d0: 6965 7665 2074 6865 2070 6172 616d 6574  ieve the paramet
-0000d6e0: 6572 7320 6f66 2061 2077 6f72 6b66 6c6f  ers of a workflo
-0000d6f0: 772e 0a0a 2020 2020 2020 2020 4172 6773  w...        Args
-0000d700: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
-0000d710: 726b 666c 6f77 2028 7374 7229 3a20 5468  rkflow (str): Th
-0000d720: 6520 776f 726b 666c 6f77 2066 6f72 2077  e workflow for w
-0000d730: 6869 6368 2074 6f20 7265 7472 6965 7665  hich to retrieve
-0000d740: 2074 6865 2070 6172 616d 6574 6572 732e   the parameters.
-0000d750: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000d760: 733a 0a20 2020 2020 2020 2020 2020 2044  s:.            D
-0000d770: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
-0000d780: 722c 2041 6e79 5d5d 3a0a 2020 2020 2020  r, Any]]:.      
-0000d790: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
-0000d7a0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-0000d7b0: 6720 7468 6520 776f 726b 666c 6f77 2070  g the workflow p
-0000d7c0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-0000d7d0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-0000d7e0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-0000d7f0: 6f72 3a20 4966 2061 6e20 6572 726f 7220  or: If an error 
-0000d800: 6f63 6375 7273 2077 6869 6c65 2072 6574  occurs while ret
-0000d810: 7269 6576 696e 6720 7468 6520 776f 726b  rieving the work
-0000d820: 666c 6f77 0a20 2020 2020 2020 2020 2020  flow.           
-0000d830: 2020 2020 2070 6172 616d 6574 6572 732e       parameters.
-0000d840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d850: 2020 2020 206a 736f 6e5f 6465 7363 7269       json_descri
-0000d860: 7074 6f72 203d 2073 656c 662e 7075 6c6c  ptor = self.pull
-0000d870: 5f64 6573 6372 6970 746f 725f 6672 6f6d  _descriptor_from
-0000d880: 5f67 6974 6875 6228 776f 726b 666c 6f77  _github(workflow
-0000d890: 290a 2020 2020 2020 2020 2320 636f 6e76  ).        # conv
-0000d8a0: 6572 7420 746f 206f 6d65 726f 2074 7970  ert to omero typ
-0000d8b0: 6573 0a20 2020 2020 2020 206c 6f67 6765  es.        logge
-0000d8c0: 722e 6465 6275 6728 6a73 6f6e 5f64 6573  r.debug(json_des
-0000d8d0: 6372 6970 746f 7229 0a20 2020 2020 2020  criptor).       
-0000d8e0: 2077 6f72 6b66 6c6f 775f 6469 6374 203d   workflow_dict =
-0000d8f0: 207b 7d0a 2020 2020 2020 2020 666f 7220   {}.        for 
-0000d900: 696e 7075 7420 696e 206a 736f 6e5f 6465  input in json_de
-0000d910: 7363 7269 7074 6f72 5b27 696e 7075 7473  scriptor['inputs
-0000d920: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0000d930: 2320 6669 6c74 6572 2063 7974 6f6d 696e  # filter cytomin
-0000d940: 6520 7061 7261 6d65 7465 7273 0a20 2020  e parameters.   
-0000d950: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000d960: 696e 7075 745b 2769 6427 5d2e 7374 6172  input['id'].star
-0000d970: 7473 7769 7468 2827 6379 746f 6d69 6e65  tswith('cytomine
-0000d980: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0000d990: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
-0000d9a0: 616d 7320 3d20 7b7d 0a20 2020 2020 2020  ams = {}.       
-0000d9b0: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000d9c0: 775f 7061 7261 6d73 5b27 6e61 6d65 275d  w_params['name']
-0000d9d0: 203d 2069 6e70 7574 5b27 6964 275d 0a20   = input['id']. 
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000d9f0: 6f72 6b66 6c6f 775f 7061 7261 6d73 5b27  orkflow_params['
-0000da00: 6465 6661 756c 7427 5d20 3d20 696e 7075  default'] = inpu
-0000da10: 745b 2764 6566 6175 6c74 2d76 616c 7565  t['default-value
-0000da20: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0000da30: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
-0000da40: 6d73 5b27 6379 7479 7065 275d 203d 2069  ms['cytype'] = i
-0000da50: 6e70 7574 5b27 7479 7065 275d 0a20 2020  nput['type'].   
-0000da60: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000da70: 6b66 6c6f 775f 7061 7261 6d73 5b27 6f70  kflow_params['op
-0000da80: 7469 6f6e 616c 275d 203d 2069 6e70 7574  tional'] = input
-0000da90: 5b27 6f70 7469 6f6e 616c 275d 0a20 2020  ['optional'].   
-0000daa0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000dab0: 5f66 6c61 6720 3d20 696e 7075 745b 2763  _flag = input['c
-0000dac0: 6f6d 6d61 6e64 2d6c 696e 652d 666c 6167  ommand-line-flag
-0000dad0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0000dae0: 2020 2063 6d64 5f66 6c61 6720 3d20 636d     cmd_flag = cm
-0000daf0: 645f 666c 6167 2e72 6570 6c61 6365 2822  d_flag.replace("
-0000db00: 4069 6422 2c20 696e 7075 745b 2769 6427  @id", input['id'
-0000db10: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000db20: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
-0000db30: 6d73 5b27 636d 645f 666c 6167 275d 203d  ms['cmd_flag'] =
-0000db40: 2063 6d64 5f66 6c61 670a 2020 2020 2020   cmd_flag.      
-0000db50: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000db60: 6f77 5f70 6172 616d 735b 2764 6573 6372  ow_params['descr
-0000db70: 6970 7469 6f6e 275d 203d 2069 6e70 7574  iption'] = input
-0000db80: 5b27 6465 7363 7269 7074 696f 6e27 5d0a  ['description'].
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 776f 726b 666c 6f77 5f64 6963 745b 696e  workflow_dict[in
-0000dbb0: 7075 745b 2769 6427 5d5d 203d 2077 6f72  put['id']] = wor
-0000dbc0: 6b66 6c6f 775f 7061 7261 6d73 0a20 2020  kflow_params.   
-0000dbd0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
-0000dbe0: 666c 6f77 5f64 6963 740a 0a20 2020 2064  flow_dict..    d
-0000dbf0: 6566 2063 6f6e 7665 7274 5f63 7974 7970  ef convert_cytyp
-0000dc00: 655f 746f 5f6f 6d74 7970 6528 7365 6c66  e_to_omtype(self
-0000dc10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc30: 2020 2063 7974 7970 653a 2073 7472 2c20     cytype: str, 
-0000dc40: 5f64 6566 6175 6c74 2c20 2a61 7267 732c  _default, *args,
-0000dc50: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-0000dc80: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
-0000dc90: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-0000dca0: 2061 2043 7974 6f6d 696e 6520 7479 7065   a Cytomine type
-0000dcb0: 2074 6f20 616e 204f 4d45 524f 2074 7970   to an OMERO typ
-0000dcc0: 6520 616e 6420 696e 7374 616e 7469 6174  e and instantiat
-0000dcd0: 6573 2069 740a 2020 2020 2020 2020 7769  es it.        wi
-0000dce0: 7468 2061 7267 732f 6b77 6172 6773 2e0a  th args/kwargs..
-0000dcf0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-0000dd00: 6174 2043 7974 6f6d 696e 6520 6861 7320  at Cytomine has 
-0000dd10: 6120 5079 7468 6f6e 2043 6c69 656e 742c  a Python Client,
-0000dd20: 2061 6e64 2073 6f6d 6520 636f 6e76 6572   and some conver
-0000dd30: 7369 6f6e 206d 6574 686f 6473 0a20 2020  sion methods.   
-0000dd40: 2020 2020 2074 6f20 7079 7468 6f6e 2074       to python t
-0000dd50: 7970 6573 2c20 6275 7420 6e6f 7468 696e  ypes, but nothin
-0000dd60: 6720 7061 7274 6963 756c 6172 6c79 2077  g particularly w
-0000dd70: 6f72 7468 2064 6570 656e 6469 6e67 206f  orth depending o
-0000dd80: 6e20 7468 6174 0a20 2020 2020 2020 206c  n that.        l
-0000dd90: 6962 7261 7279 2066 6f72 2079 6574 2e20  ibrary for yet. 
-0000dda0: 4d69 6768 7420 6265 2075 7365 6675 6c20  Might be useful 
-0000ddb0: 696e 2074 6865 2066 7574 7572 6520 7065  in the future pe
-0000ddc0: 7268 6170 732e 0a20 2020 2020 2020 2028  rhaps..        (
-0000ddd0: 652e 672e 2068 7474 7073 3a2f 2f67 6974  e.g. https://git
-0000dde0: 6875 622e 636f 6d2f 4379 746f 6d69 6e65  hub.com/Cytomine
-0000ddf0: 2d55 4c69 6567 652f 4379 746f 6d69 6e65  -ULiege/Cytomine
-0000de00: 2d70 7974 686f 6e2d 636c 6965 6e74 2f0a  -python-client/.
-0000de10: 2020 2020 2020 2020 626c 6f62 2f6d 6173          blob/mas
-0000de20: 7465 722f 6379 746f 6d69 6e65 2f63 7974  ter/cytomine/cyt
-0000de30: 6f6d 696e 655f 6a6f 622e 7079 290a 0a20  omine_job.py).. 
-0000de40: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000de50: 2020 2020 2020 2020 2063 7974 7970 6520           cytype 
-0000de60: 2873 7472 293a 2054 6865 2043 7974 6f6d  (str): The Cytom
-0000de70: 696e 6520 7479 7065 2074 6f20 636f 6e76  ine type to conv
-0000de80: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
-0000de90: 205f 6465 6661 756c 743a 2054 6865 2064   _default: The d
-0000dea0: 6566 6175 6c74 2076 616c 7565 2e20 5265  efault value. Re
-0000deb0: 7175 6972 6564 2074 6f20 6469 7374 696e  quired to distin
-0000dec0: 6775 6973 6820 6265 7477 6565 6e20 666c  guish between fl
-0000ded0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-0000dee0: 2020 2020 616e 6420 696e 742e 0a20 2020      and int..   
-0000def0: 2020 2020 2020 2020 202a 6172 6773 3a20           *args: 
-0000df00: 4164 6469 7469 6f6e 616c 2070 6f73 6974  Additional posit
-0000df10: 696f 6e61 6c20 6172 6775 6d65 6e74 732e  ional arguments.
-0000df20: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-0000df30: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-0000df40: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-0000df50: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
-0000df60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000df70: 2020 2041 6e79 3a0a 2020 2020 2020 2020     Any:.        
-0000df80: 2020 2020 2020 2020 5468 6520 636f 6e76          The conv
-0000df90: 6572 7465 6420 4f4d 4552 4f20 7479 7065  erted OMERO type
-0000dfa0: 2063 6c61 7373 2069 6e73 7461 6e63 650a   class instance.
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfc0: 6f72 204e 6f6e 6520 6966 2065 7272 6f72  or None if error
-0000dfd0: 7320 6f63 6375 7265 642e 0a0a 2020 2020  s occured...    
-0000dfe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000dff0: 2320 544f 444f 206d 616b 6520 456e 756d  # TODO make Enum
-0000e000: 203f 0a20 2020 2020 2020 2069 6620 6379   ?.        if cy
-0000e010: 7479 7065 203d 3d20 274e 756d 6265 7227  type == 'Number'
-0000e020: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000e030: 2069 7369 6e73 7461 6e63 6528 5f64 6566   isinstance(_def
-0000e040: 6175 6c74 2c20 666c 6f61 7429 3a0a 2020  ault, float):.  
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000e060: 666c 6f61 7420 696e 7374 6561 640a 2020  float instead.  
-0000e070: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e080: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
-0000e090: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
-0000e0a0: 7269 7074 7322 2c20 2246 6c6f 6174 222c  ripts", "Float",
-0000e0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0d0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
-0000e0e0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000e0f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000e100: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000e110: 7572 6e20 7365 6c66 2e73 7472 5f74 6f5f  urn self.str_to_
-0000e120: 636c 6173 7328 226f 6d65 726f 2e73 6372  class("omero.scr
-0000e130: 6970 7473 222c 2022 496e 7422 2c0a 2020  ipts", "Int",.  
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
-0000e170: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000e180: 656c 6966 2063 7974 7970 6520 3d3d 2027  elif cytype == '
-0000e190: 426f 6f6c 6561 6e27 3a0a 2020 2020 2020  Boolean':.      
-0000e1a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e1b0: 662e 7374 725f 746f 5f63 6c61 7373 2822  f.str_to_class("
-0000e1c0: 6f6d 6572 6f2e 7363 7269 7074 7322 2c20  omero.scripts", 
-0000e1d0: 2242 6f6f 6c22 2c0a 2020 2020 2020 2020  "Bool",.        
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 2020 2020 2020 2020 2020 202a 6172               *ar
-0000e200: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-0000e210: 2020 2020 2020 656c 6966 2063 7974 7970        elif cytyp
-0000e220: 6520 3d3d 2027 5374 7269 6e67 273a 0a20  e == 'String':. 
-0000e230: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e240: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
-0000e250: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
-0000e260: 7473 222c 2022 5374 7269 6e67 222c 0a20  ts", "String",. 
-0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
-0000e2a0: 7267 7329 0a0a 2020 2020 6465 6620 6578  rgs)..    def ex
-0000e2b0: 7472 6163 745f 7061 7274 735f 6672 6f6d  tract_parts_from
-0000e2c0: 5f75 726c 2873 656c 662c 2069 6e70 7574  _url(self, input
-0000e2d0: 5f75 726c 3a20 7374 7229 202d 3e20 5475  _url: str) -> Tu
-0000e2e0: 706c 655b 4c69 7374 5b73 7472 5d2c 2073  ple[List[str], s
-0000e2f0: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
-0000e300: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
-0000e310: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-0000e320: 616e 6420 6272 616e 6368 2069 6e66 6f72  and branch infor
-0000e330: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
-0000e340: 696e 7075 7420 5552 4c2e 0a0a 2020 2020  input URL...    
-0000e350: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000e360: 2020 2020 2020 696e 7075 745f 7572 6c20        input_url 
-0000e370: 2873 7472 293a 2054 6865 2069 6e70 7574  (str): The input
-0000e380: 2047 6974 4875 6220 5552 4c2e 0a0a 2020   GitHub URL...  
-0000e390: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000e3a0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-0000e3b0: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
-0000e3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e3d0: 2020 5468 6520 6c69 7374 206f 6620 7572    The list of ur
-0000e3e0: 6c20 7061 7274 7320 616e 6420 7468 6520  l parts and the 
-0000e3f0: 6272 616e 6368 2f76 6572 7369 6f6e 2e0a  branch/version..
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 4966 206e 6f20 6272 616e 6368 2069 7320  If no branch is 
-0000e420: 666f 756e 642c 2069 7420 7769 6c6c 2072  found, it will r
-0000e430: 6574 7572 6e20 226d 6173 7465 7222 0a0a  eturn "master"..
-0000e440: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-0000e450: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-0000e460: 6545 7272 6f72 3a20 4966 2074 6865 2069  eError: If the i
-0000e470: 6e70 7574 2055 524c 2069 7320 6e6f 7420  nput URL is not 
-0000e480: 6120 7661 6c69 6420 4769 7448 7562 2055  a valid GitHub U
-0000e490: 524c 2e0a 2020 2020 2020 2020 2222 220a  RL..        """.
-0000e4a0: 2020 2020 2020 2020 7572 6c5f 7061 7274          url_part
-0000e4b0: 7320 3d20 696e 7075 745f 7572 6c2e 7370  s = input_url.sp
-0000e4c0: 6c69 7428 222f 2229 0a20 2020 2020 2020  lit("/").       
-0000e4d0: 2069 6620 6c65 6e28 7572 6c5f 7061 7274   if len(url_part
-0000e4e0: 7329 203c 2035 206f 7220 7572 6c5f 7061  s) < 5 or url_pa
-0000e4f0: 7274 735b 325d 2021 3d20 2267 6974 6875  rts[2] != "githu
-0000e500: 622e 636f 6d22 3a0a 2020 2020 2020 2020  b.com":.        
-0000e510: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000e520: 7272 6f72 2822 496e 7661 6c69 6420 4769  rror("Invalid Gi
-0000e530: 7448 7562 2055 524c 2229 0a0a 2020 2020  tHub URL")..    
-0000e540: 2020 2020 6966 2022 7472 6565 2220 696e      if "tree" in
-0000e550: 2075 726c 5f70 6172 7473 3a0a 2020 2020   url_parts:.    
-0000e560: 2020 2020 2020 2020 2320 4361 7365 3a20          # Case: 
-0000e570: 5552 4c20 636f 6e74 6169 6e73 2061 2062  URL contains a b
-0000e580: 7261 6e63 680a 2020 2020 2020 2020 2020  ranch.          
-0000e590: 2020 6272 616e 6368 5f69 6e64 6578 203d    branch_index =
-0000e5a0: 2075 726c 5f70 6172 7473 2e69 6e64 6578   url_parts.index
-0000e5b0: 2822 7472 6565 2229 202b 2031 0a20 2020  ("tree") + 1.   
-0000e5c0: 2020 2020 2020 2020 2062 7261 6e63 6820           branch 
-0000e5d0: 3d20 7572 6c5f 7061 7274 735b 6272 616e  = url_parts[bran
-0000e5e0: 6368 5f69 6e64 6578 5d0a 2020 2020 2020  ch_index].      
-0000e5f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e600: 2020 2020 2320 4361 7365 3a20 5552 4c20      # Case: URL 
-0000e610: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
-0000e620: 2061 2062 7261 6e63 680a 2020 2020 2020   a branch.      
-0000e630: 2020 2020 2020 6272 616e 6368 203d 2022        branch = "
-0000e640: 6d61 7374 6572 220a 0a20 2020 2020 2020  master"..       
-0000e650: 2072 6574 7572 6e20 7572 6c5f 7061 7274   return url_part
-0000e660: 732c 2062 7261 6e63 680a 0a20 2020 2064  s, branch..    d
-0000e670: 6566 2063 6f6e 7665 7274 5f75 726c 2873  ef convert_url(s
-0000e680: 656c 662c 2069 6e70 7574 5f75 726c 3a20  elf, input_url: 
-0000e690: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
-0000e6a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000e6b0: 2043 6f6e 7665 7274 2074 6865 2069 6e70   Convert the inp
-0000e6c0: 7574 2047 6974 4875 6220 5552 4c20 746f  ut GitHub URL to
-0000e6d0: 2061 6e20 6f75 7470 7574 2055 524c 2074   an output URL t
-0000e6e0: 6861 7420 7265 7472 6965 7665 730a 2020  hat retrieves.  
-0000e6f0: 2020 2020 2020 7468 6520 2764 6573 6372        the 'descr
-0000e700: 6970 746f 722e 6a73 6f6e 2720 6669 6c65  iptor.json' file
-0000e710: 2069 6e20 7261 7720 666f 726d 6174 2e0a   in raw format..
-0000e720: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000e730: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-0000e740: 5f75 726c 2028 7374 7229 3a20 5468 6520  _url (str): The 
-0000e750: 696e 7075 7420 4769 7448 7562 2055 524c  input GitHub URL
-0000e760: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000e770: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000e780: 7374 723a 2054 6865 206f 7574 7075 7420  str: The output 
-0000e790: 5552 4c20 746f 2074 6865 2027 6465 7363  URL to the 'desc
-0000e7a0: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
-0000e7b0: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
-0000e7c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000e7d0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
-0000e7e0: 6865 2069 6e70 7574 2055 524c 2069 7320  he input URL is 
-0000e7f0: 6e6f 7420 6120 7661 6c69 6420 4769 7448  not a valid GitH
-0000e800: 7562 2055 524c 2e0a 2020 2020 2020 2020  ub URL..        
-0000e810: 2222 220a 2020 2020 2020 2020 7572 6c5f  """.        url_
-0000e820: 7061 7274 732c 2062 7261 6e63 6820 3d20  parts, branch = 
-0000e830: 7365 6c66 2e65 7874 7261 6374 5f70 6172  self.extract_par
-0000e840: 7473 5f66 726f 6d5f 7572 6c28 696e 7075  ts_from_url(inpu
-0000e850: 745f 7572 6c29 0a0a 2020 2020 2020 2020  t_url)..        
-0000e860: 2320 436f 6e73 7472 7563 7420 7468 6520  # Construct the 
-0000e870: 6f75 7470 7574 2055 524c 2062 7920 636f  output URL by co
-0000e880: 6d62 696e 696e 6720 7468 6520 6578 7472  mbining the extr
-0000e890: 6163 7465 6420 696e 666f 726d 6174 696f  acted informatio
-0000e8a0: 6e0a 2020 2020 2020 2020 2320 7769 7468  n.        # with
-0000e8b0: 2074 6865 2064 6573 6972 6564 2066 696c   the desired fil
-0000e8c0: 6520 7061 7468 0a20 2020 2020 2020 206f  e path.        o
-0000e8d0: 7574 7075 745f 7572 6c20 3d20 6622 6874  utput_url = f"ht
-0000e8e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000e8f0: 2f7b 7572 6c5f 7061 7274 735b 335d 7d2f  /{url_parts[3]}/
-0000e900: 7b75 726c 5f70 6172 7473 5b34 5d7d 2f72  {url_parts[4]}/r
-0000e910: 6177 2f7b 6272 616e 6368 7d2f 6465 7363  aw/{branch}/desc
-0000e920: 7269 7074 6f72 2e6a 736f 6e22 0a0a 2020  riptor.json"..  
-0000e930: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-0000e940: 7075 745f 7572 6c0a 0a20 2020 2064 6566  put_url..    def
-0000e950: 2070 756c 6c5f 6465 7363 7269 7074 6f72   pull_descriptor
-0000e960: 5f66 726f 6d5f 6769 7468 7562 2873 656c  _from_github(sel
-0000e970: 662c 2077 6f72 6b66 6c6f 773a 2073 7472  f, workflow: str
-0000e980: 2920 2d3e 2044 6963 743a 0a20 2020 2020  ) -> Dict:.     
-0000e990: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-0000e9a0: 756c 6c20 7468 6520 776f 726b 666c 6f77  ull the workflow
-0000e9b0: 2064 6573 6372 6970 746f 7220 6672 6f6d   descriptor from
-0000e9c0: 2047 6974 4875 622e 0a0a 2020 2020 2020   GitHub...      
-0000e9d0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000e9e0: 2020 2020 776f 726b 666c 6f77 2028 7374      workflow (st
-0000e9f0: 7229 3a20 5468 6520 776f 726b 666c 6f77  r): The workflow
-0000ea00: 2066 6f72 2077 6869 6368 2074 6f20 7075   for which to pu
-0000ea10: 6c6c 2074 6865 2064 6573 6372 6970 746f  ll the descripto
-0000ea20: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
-0000ea30: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000ea40: 2044 6963 743a 2054 6865 204a 534f 4e20   Dict: The JSON 
-0000ea50: 6465 7363 7269 7074 6f72 2e0a 0a20 2020  descriptor...   
-0000ea60: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-0000ea70: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-0000ea80: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
-0000ea90: 206f 6363 7572 7320 7768 696c 6520 7075   occurs while pu
-0000eaa0: 6c6c 696e 6720 7468 6520 6465 7363 7269  lling the descri
-0000eab0: 7074 6f72 2066 696c 652e 0a20 2020 2020  ptor file..     
-0000eac0: 2020 2022 2222 0a20 2020 2020 2020 2067     """.        g
-0000ead0: 6974 5f72 6570 6f20 3d20 7365 6c66 2e73  it_repo = self.s
-0000eae0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-0000eaf0: 5b77 6f72 6b66 6c6f 775d 0a20 2020 2020  [workflow].     
-0000eb00: 2020 2023 2063 6f6e 7665 7274 2067 6974     # convert git
-0000eb10: 2072 6570 6f20 746f 206a 736f 6e20 6669   repo to json fi
-0000eb20: 6c65 0a20 2020 2020 2020 2072 6177 5f75  le.        raw_u
-0000eb30: 726c 203d 2073 656c 662e 636f 6e76 6572  rl = self.conver
-0000eb40: 745f 7572 6c28 6769 745f 7265 706f 290a  t_url(git_repo).
-0000eb50: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000eb60: 6562 7567 2866 2250 756c 6c20 776f 726b  ebug(f"Pull work
-0000eb70: 666c 6f77 3a20 7b77 6f72 6b66 6c6f 777d  flow: {workflow}
-0000eb80: 3a20 7b67 6974 5f72 6570 6f7d 203e 3e20  : {git_repo} >> 
-0000eb90: 7b72 6177 5f75 726c 7d22 290a 2020 2020  {raw_url}").    
-0000eba0: 2020 2020 2320 7075 6c6c 2077 6f72 6b66      # pull workf
-0000ebb0: 6c6f 7720 7061 7261 6d73 0a20 2020 2020  low params.     
-0000ebc0: 2020 2067 6974 6875 625f 7365 7373 696f     github_sessio
-0000ebd0: 6e20 3d20 7365 6c66 2e67 6574 5f6f 725f  n = self.get_or_
-0000ebe0: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
-0000ebf0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
-0000ec00: 6768 6669 6c65 203d 2067 6974 6875 625f  ghfile = github_
-0000ec10: 7365 7373 696f 6e2e 6765 7428 7261 775f  session.get(raw_
-0000ec20: 7572 6c29 0a20 2020 2020 2020 2069 6620  url).        if 
-0000ec30: 6768 6669 6c65 2e6f 6b3a 0a20 2020 2020  ghfile.ok:.     
-0000ec40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000ec50: 6275 6728 6622 4361 6368 6564 3f20 7b67  bug(f"Cached? {g
-0000ec60: 6866 696c 652e 6672 6f6d 5f63 6163 6865  hfile.from_cache
-0000ec70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-0000ec80: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
-0000ec90: 3d20 6768 6669 6c65 2e6a 736f 6e28 290a  = ghfile.json().
-0000eca0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ecb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000ecc0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000ecd0: 2020 2020 2020 2020 2020 2020 6627 4572              f'Er
-0000ece0: 726f 7220 7768 696c 6520 7075 6c6c 696e  ror while pullin
-0000ecf0: 6720 6465 7363 7269 7074 6f72 2066 696c  g descriptor fil
-0000ed00: 6520 666f 7220 776f 726b 666c 6f77 207b  e for workflow {
-0000ed10: 776f 726b 666c 6f77 7d2c 5c0a 2020 2020  workflow},\.    
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 6672 6f6d 207b 7261 775f 7572 6c7d 3a20  from {raw_url}: 
-0000ed40: 7b67 6866 696c 652e 5f5f 6469 6374 5f5f  {ghfile.__dict__
-0000ed50: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
-0000ed60: 726e 206a 736f 6e5f 6465 7363 7269 7074  rn json_descript
-0000ed70: 6f72 0a0a 2020 2020 6465 6620 6765 745f  or..    def get_
-0000ed80: 6f72 5f63 7265 6174 655f 6769 7468 7562  or_create_github
-0000ed90: 5f73 6573 7369 6f6e 2873 656c 6629 3a0a  _session(self):.
-0000eda0: 2020 2020 2020 2020 2320 4e6f 7465 2c20          # Note, 
-0000edb0: 7573 696e 6720 7265 7175 6573 7473 5f63  using requests_c
-0000edc0: 6163 6865 2031 2e31 2e31 2c20 636f 6e64  ache 1.1.1, cond
-0000edd0: 6974 696f 6e61 6c20 7175 6572 6965 7320  itional queries 
-0000ede0: 6172 6520 6465 6661 756c 743a 0a20 2020  are default:.   
-0000edf0: 2020 2020 2023 2054 6865 2063 6163 6865       # The cache
-0000ee00: 6420 7265 7370 6f6e 7365 2077 696c 6c20  d response will 
-0000ee10: 7374 696c 6c20 6265 2075 7365 6420 756e  still be used un
-0000ee20: 7469 6c20 7468 6520 7265 6d6f 7465 2063  til the remote c
-0000ee30: 6f6e 7465 6e74 2061 6374 7561 6c6c 7920  ontent actually 
-0000ee40: 6368 616e 6765 730a 2020 2020 2020 2020  changes.        
-0000ee50: 2320 4576 656e 2069 6620 7468 6520 2765  # Even if the 'e
-0000ee60: 7870 6972 655f 6166 7465 7227 2069 7320  xpire_after' is 
-0000ee70: 7472 6967 6765 7265 642e 2054 6869 7320  triggered. This 
-0000ee80: 6973 2062 7569 6c74 2069 6e74 6f20 4769  is built into Gi
-0000ee90: 7448 7562 2c20 7768 6963 6820 7265 7475  tHub, which retu
-0000eea0: 726e 730a 2020 2020 2020 2020 2320 6120  rns.        # a 
-0000eeb0: 4574 6167 2069 6e20 7468 6520 6865 6164  Etag in the head
-0000eec0: 6572 2074 6861 7420 6f6e 6c79 2063 6861  er that only cha
-0000eed0: 6e67 6573 2077 6865 6e20 7468 6520 636f  nges when the co
-0000eee0: 6e74 656e 7420 2865 2e67 2e20 7468 6520  ntent (e.g. the 
-0000eef0: 6465 7363 7269 7074 6f72 2920 6368 616e  descriptor) chan
-0000ef00: 6765 732e 0a20 2020 2020 2020 2023 2049  ges..        # I
-0000ef10: 6620 796f 7520 7072 6f76 6964 6520 7468  f you provide th
-0000ef20: 6973 2045 7461 6720 7768 656e 2071 7565  is Etag when que
-0000ef30: 7279 696e 672c 2079 6f75 2077 696c 6c20  rying, you will 
-0000ef40: 6765 7420 6120 3330 3420 2827 6e6f 2063  get a 304 ('no c
-0000ef50: 6861 6e67 6527 2920 616e 6420 6974 2077  hange') and it w
-0000ef60: 696c 6c0a 2020 2020 2020 2020 2320 4e4f  ill.        # NO
-0000ef70: 5420 636f 756e 7420 746f 7761 7264 7320  T count towards 
-0000ef80: 796f 7572 2047 6974 6875 6220 6c69 6d69  your Github limi
-0000ef90: 7473 2e20 416e 6420 7265 7175 6573 7473  ts. And requests
-0000efa0: 5f63 6163 6865 2064 6f65 7320 7468 6174  _cache does that
-0000efb0: 2066 6f72 2075 7320 6e6f 772e 0a20 2020   for us now..   
-0000efc0: 2020 2020 2023 204e 6f74 2061 7661 696c       # Not avail
-0000efd0: 6162 6c65 2069 6e20 5079 7468 6f6e 332e  able in Python3.
-0000efe0: 3620 7468 6f75 6768 2e0a 2020 2020 2020  6 though..      
-0000eff0: 2020 7320 3d20 7265 7175 6573 7473 5f63    s = requests_c
-0000f000: 6163 6865 2e43 6163 6865 6453 6573 7369  ache.CachedSessi
-0000f010: 6f6e 2827 6769 7468 7562 5f63 6163 6865  on('github_cache
-0000f020: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f040: 2020 2020 2020 2020 2020 2020 6261 636b              back
-0000f050: 656e 643d 7365 6c66 2e63 6163 6865 2c0a  end=self.cache,.
-0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 2020 2020 2020 2020 2065 7870 6972 655f           expire_
-0000f090: 6166 7465 723d 312c 0a20 2020 2020 2020  after=1,.       
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0c0: 2020 6361 6368 655f 636f 6e74 726f 6c3d    cache_control=
-0000f0d0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000f100: 2020 2020 2020 2020 2320 4d69 6768 7420          # Might 
-0000f110: 6861 7665 2062 6967 6765 7220 6973 7375  have bigger issu
-0000f120: 6573 2c20 7468 6973 2069 7320 7265 6c61  es, this is rela
-0000f130: 7465 6420 746f 2072 6174 6520 6c69 6d69  ted to rate limi
-0000f140: 7473 206f 6e20 4769 7448 7562 0a20 2020  ts on GitHub.   
-0000f150: 2020 2020 2023 2068 7474 7073 3a2f 2f64       # https://d
-0000f160: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
-0000f170: 6e2f 7265 7374 2f75 7369 6e67 2d74 6865  n/rest/using-the
-0000f180: 2d72 6573 742d 6170 692f 7261 7465 2d6c  -rest-api/rate-l
-0000f190: 696d 6974 732d 666f 722d 7468 652d 7265  imits-for-the-re
-0000f1a0: 7374 2d61 7069 0a20 2020 2020 2020 2023  st-api.        #
-0000f1b0: 2049 6620 6974 2073 7461 7973 2061 2070   If it stays a p
-0000f1c0: 726f 626c 656d 2c20 7765 2068 6176 6520  roblem, we have 
-0000f1d0: 746f 2061 6464 2061 6e20 6f70 7469 6f6e  to add an option
-0000f1e0: 2074 6f20 6164 6420 6120 4748 206b 6579   to add a GH key
-0000f1f0: 2074 6f20 7468 6520 636f 6e66 6967 0a20   to the config. 
-0000f200: 2020 2020 2020 2023 2045 2e67 2e20 7365         # E.g. se
-0000f210: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-0000f220: 2e63 6f6d 2f72 6571 7565 7374 732d 6361  .com/requests-ca
-0000f230: 6368 652f 7265 7175 6573 7473 2d63 6163  che/requests-cac
-0000f240: 6865 2f62 6c6f 622f 3533 3133 3465 6630  he/blob/53134ef0
-0000f250: 6539 3964 3731 3366 6564 3632 3531 3564  e99d713fed62515d
-0000f260: 6662 3762 6366 6161 6335 6636 3366 3964  fb7bcfaac5f63f9d
-0000f270: 2f65 7861 6d70 6c65 732f 7079 6769 7468  /examples/pygith
-0000f280: 7562 2e70 790a 2020 2020 2020 2020 2320  ub.py.        # 
-0000f290: 4865 7265 2079 6f75 2063 6f75 6c64 2068  Here you could h
-0000f2a0: 6176 6520 616e 2041 4343 4553 535f 544f  ave an ACCESS_TO
-0000f2b0: 4b45 4e2e 0a20 2020 2020 2020 2023 2041  KEN..        # A
-0000f2c0: 6e20 4143 4345 5353 5f54 4f4b 454e 2063  n ACCESS_TOKEN c
-0000f2d0: 6f75 6c64 2069 6d70 726f 7665 2061 7069  ould improve api
-0000f2e0: 206c 696d 6974 7320 746f 2035 3030 302f   limits to 5000/
-0000f2f0: 6820 2866 726f 6d20 3630 2f68 292e 0a20  h (from 60/h).. 
-0000f300: 2020 2020 2020 2072 6574 7279 5f73 7472         retry_str
-0000f310: 6174 6567 7920 3d20 5265 7472 7928 0a20  ategy = Retry(. 
-0000f320: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-0000f330: 3d35 2c20 2020 2020 2020 2020 2020 2020  =5,             
-0000f340: 2020 2320 4d61 7869 6d75 6d20 6e75 6d62    # Maximum numb
-0000f350: 6572 206f 6620 7265 7472 6965 730a 2020  er of retries.  
-0000f360: 2020 2020 2020 2020 2020 2320 4578 706f            # Expo
-0000f370: 6e65 6e74 6961 6c20 6261 636b 6f66 6620  nential backoff 
-0000f380: 6661 6374 6f72 2028 6465 6c61 7920 6265  factor (delay be
-0000f390: 7477 6565 6e20 7265 7472 6965 7329 0a20  tween retries). 
-0000f3a0: 2020 2020 2020 2020 2020 2062 6163 6b6f             backo
-0000f3b0: 6666 5f66 6163 746f 723d 352c 0a20 2020  ff_factor=5,.   
-0000f3c0: 2020 2020 2020 2020 2023 2052 6574 7279           # Retry
-0000f3d0: 206f 6e20 7468 6573 6520 4854 5450 2073   on these HTTP s
-0000f3e0: 7461 7475 7320 636f 6465 730a 2020 2020  tatus codes.    
-0000f3f0: 2020 2020 2020 2020 7374 6174 7573 5f66          status_f
-0000f400: 6f72 6365 6c69 7374 3d5b 3530 302c 2035  orcelist=[500, 5
-0000f410: 3032 2c20 3530 332c 2035 3034 2c20 3430  02, 503, 504, 40
-0000f420: 332c 2034 3239 5d2c 0a20 2020 2020 2020  3, 429],.       
-0000f430: 2020 2020 2061 6c6c 6f77 6564 5f6d 6574       allowed_met
-0000f440: 686f 6473 3d66 726f 7a65 6e73 6574 285b  hods=frozenset([
-0000f450: 2747 4554 275d 2920 2023 204f 6e6c 7920  'GET'])  # Only 
-0000f460: 7265 7472 7920 666f 7220 4745 5420 7265  retry for GET re
-0000f470: 7175 6573 7473 0a20 2020 2020 2020 2029  quests.        )
-0000f480: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
-0000f490: 2827 6874 7470 733a 2f2f 6769 7468 7562  ('https://github
-0000f4a0: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
-0000f4b0: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
-0000f4c0: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
-0000f4d0: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
-0000f4e0: 2827 6874 7470 3a2f 2f67 6974 6875 622e  ('http://github.
-0000f4f0: 636f 6d2f 272c 2048 5454 5041 6461 7074  com/', HTTPAdapt
-0000f500: 6572 286d 6178 5f72 6574 7269 6573 3d72  er(max_retries=r
-0000f510: 6574 7279 5f73 7472 6174 6567 7929 290a  etry_strategy)).
-0000f520: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000f530: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
-0000f540: 726b 666c 6f77 5f63 6f6d 6d61 6e64 2873  rkflow_command(s
-0000f550: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f570: 2020 776f 726b 666c 6f77 3a20 7374 722c    workflow: str,
-0000f580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f590: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0000f5a0: 726b 666c 6f77 5f76 6572 7369 6f6e 3a20  rkflow_version: 
-0000f5b0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5d0: 2020 696e 7075 745f 6461 7461 3a20 7374    input_data: st
-0000f5e0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f600: 656d 6169 6c3a 204f 7074 696f 6e61 6c5b  email: Optional[
-0000f610: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
-0000f640: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000f650: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 2020 202a 2a6b 7761 7267 7329 202d 3e20     **kwargs) -> 
-0000f680: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
-0000f690: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f6a0: 2020 2020 2020 4765 6e65 7261 7465 2074        Generate t
-0000f6b0: 6865 2053 6c75 726d 2077 6f72 6b66 6c6f  he Slurm workflo
-0000f6c0: 7720 636f 6d6d 616e 6420 616e 6420 656e  w command and en
-0000f6d0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-0000f6e0: 6c65 732e 0a0a 2020 2020 2020 2020 4172  les...        Ar
-0000f6f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000f700: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
-0000f710: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000f720: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
-0000f730: 2020 2020 2020 776f 726b 666c 6f77 5f76        workflow_v
-0000f740: 6572 7369 6f6e 2028 7374 7229 3a20 5468  ersion (str): Th
-0000f750: 6520 7665 7273 696f 6e20 6f66 2074 6865  e version of the
-0000f760: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-0000f770: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-0000f780: 6120 2873 7472 293a 2054 6865 206e 616d  a (str): The nam
-0000f790: 6520 6f66 2074 6865 2069 6e70 7574 2064  e of the input d
-0000f7a0: 6174 6120 666f 6c64 6572 2063 6f6e 7461  ata folder conta
-0000f7b0: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
-0000f7c0: 2020 2020 2020 7468 6520 696e 7075 7420        the input 
-0000f7d0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
-0000f7e0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
-0000f7f0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-0000f800: 5468 6520 656d 6169 6c20 6164 6472 6573  The email addres
-0000f810: 7320 666f 7220 6a6f 6220 6e6f 7469 6669  s for job notifi
-0000f820: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
-0000f830: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0000f840: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
-0000f850: 2064 6566 6175 6c74 7320 746f 2077 6861   defaults to wha
-0000f860: 7420 6973 2069 6e20 7468 6520 6a6f 6220  t is in the job 
-0000f870: 7363 7269 7074 2e0a 2020 2020 2020 2020  script..        
-0000f880: 2020 2020 7469 6d65 2028 7374 722c 206f      time (str, o
-0000f890: 7074 696f 6e61 6c29 3a20 5468 6520 7469  ptional): The ti
-0000f8a0: 6d65 206c 696d 6974 2066 6f72 2074 6865  me limit for the
-0000f8b0: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
-0000f8c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f8d0: 6d61 7420 4848 3a4d 4d3a 5353 2e20 4465  mat HH:MM:SS. De
-0000f8e0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
-0000f8f0: 7768 6963 6820 6465 6661 756c 7473 2074  which defaults t
-0000f900: 6f20 7768 6174 200a 2020 2020 2020 2020  o what .        
-0000f910: 2020 2020 2020 2020 6973 2069 6e20 7468          is in th
-0000f920: 6520 6a6f 6220 7363 7269 7074 2e0a 2020  e job script..  
-0000f930: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000f940: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
-0000f950: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000f960: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
-0000f970: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
-0000f980: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000f990: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
-0000f9a0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000f9b0: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-0000f9c0: 696e 696e 6720 7468 6520 536c 7572 6d20  ining the Slurm 
-0000f9d0: 776f 726b 666c 6f77 2063 6f6d 6d61 6e64  workflow command
-0000f9e0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000f9f0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
-0000fa00: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-0000fa10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000fa20: 2020 2020 206d 6f64 656c 5f70 6174 6820       model_path 
-0000fa30: 3d20 7365 6c66 2e73 6c75 726d 5f6d 6f64  = self.slurm_mod
-0000fa40: 656c 5f70 6174 6873 5b77 6f72 6b66 6c6f  el_paths[workflo
-0000fa50: 772e 6c6f 7765 7228 295d 0a20 2020 2020  w.lower()].     
-0000fa60: 2020 206a 6f62 5f73 6372 6970 7420 3d20     job_script = 
-0000fa70: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-0000fa80: 5f6a 6f62 735b 776f 726b 666c 6f77 2e6c  _jobs[workflow.l
-0000fa90: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
-0000faa0: 6a6f 625f 7061 7261 6d73 203d 2073 656c  job_params = sel
-0000fab0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
-0000fac0: 6273 5f70 6172 616d 735b 776f 726b 666c  bs_params[workfl
-0000fad0: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
-0000fae0: 2020 2020 2320 6772 6162 206f 6e6c 7920      # grab only 
-0000faf0: 7468 6520 696d 6167 6520 6e61 6d65 2c20  the image name, 
-0000fb00: 6e6f 7420 7468 6520 6772 6f75 702f 6372  not the group/cr
-0000fb10: 6561 746f 720a 2020 2020 2020 2020 696d  eator.        im
-0000fb20: 6167 6520 3d20 7365 6c66 2e73 6c75 726d  age = self.slurm
-0000fb30: 5f6d 6f64 656c 5f69 6d61 6765 735b 776f  _model_images[wo
-0000fb40: 726b 666c 6f77 2e6c 6f77 6572 2829 5d2e  rkflow.lower()].
-0000fb50: 7370 6c69 7428 222f 2229 5b31 5d0a 0a20  split("/")[1].. 
-0000fb60: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
-0000fb70: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
-0000fb80: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
-0000fb90: 227b 7365 6c66 2e73 6c75 726d 5f64 6174  "{self.slurm_dat
-0000fba0: 615f 7061 7468 7d2f 7b69 6e70 7574 5f64  a_path}/{input_d
-0000fbb0: 6174 617d 222c 0a20 2020 2020 2020 2020  ata}",.         
-0000fbc0: 2020 2022 494d 4147 455f 5041 5448 223a     "IMAGE_PATH":
-0000fbd0: 2066 227b 7365 6c66 2e73 6c75 726d 5f69   f"{self.slurm_i
-0000fbe0: 6d61 6765 735f 7061 7468 7d2f 7b6d 6f64  mages_path}/{mod
-0000fbf0: 656c 5f70 6174 687d 222c 0a20 2020 2020  el_path}",.     
-0000fc00: 2020 2020 2020 2022 494d 4147 455f 5645         "IMAGE_VE
-0000fc10: 5253 494f 4e22 3a20 6622 7b77 6f72 6b66  RSION": f"{workf
-0000fc20: 6c6f 775f 7665 7273 696f 6e7d 222c 0a20  low_version}",. 
-0000fc30: 2020 2020 2020 2020 2020 2022 5349 4e47             "SING
-0000fc40: 554c 4152 4954 595f 494d 4147 4522 3a20  ULARITY_IMAGE": 
-0000fc50: 6622 7b69 6d61 6765 7d5f 7b77 6f72 6b66  f"{image}_{workf
-0000fc60: 6c6f 775f 7665 7273 696f 6e7d 2e73 6966  low_version}.sif
-0000fc70: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0000fc80: 5343 5249 5054 5f50 4154 4822 3a20 6622  SCRIPT_PATH": f"
-0000fc90: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
-0000fca0: 7074 5f70 6174 687d 220a 2020 2020 2020  pt_path}".      
-0000fcb0: 2020 7d0a 2020 2020 2020 2020 776f 726b    }.        work
-0000fcc0: 666c 6f77 5f65 6e76 203d 2073 656c 662e  flow_env = self.
-0000fcd0: 776f 726b 666c 6f77 5f70 6172 616d 735f  workflow_params_
-0000fce0: 746f 5f65 6e76 7661 7273 282a 2a6b 7761  to_envvars(**kwa
-0000fcf0: 7267 7329 0a20 2020 2020 2020 2065 6e76  rgs).        env
-0000fd00: 203d 207b 2a2a 7362 6174 6368 5f65 6e76   = {**sbatch_env
-0000fd10: 2c20 2a2a 776f 726b 666c 6f77 5f65 6e76  , **workflow_env
-0000fd20: 7d0a 0a20 2020 2020 2020 2065 6d61 696c  }..        email
-0000fd30: 5f70 6172 616d 203d 2022 2220 6966 2065  _param = "" if e
-0000fd40: 6d61 696c 2069 7320 4e6f 6e65 2065 6c73  mail is None els
-0000fd50: 6520 6622 202d 2d6d 6169 6c2d 7573 6572  e f" --mail-user
-0000fd60: 3d7b 656d 6169 6c7d 220a 2020 2020 2020  ={email}".      
-0000fd70: 2020 7469 6d65 5f70 6172 616d 203d 2022    time_param = "
-0000fd80: 2220 6966 2074 696d 6520 6973 204e 6f6e  " if time is Non
-0000fd90: 6520 656c 7365 2066 2220 2d2d 7469 6d65  e else f" --time
-0000fda0: 3d7b 7469 6d65 7d22 0a20 2020 2020 2020  ={time}".       
-0000fdb0: 206a 6f62 5f70 6172 616d 732e 6170 7065   job_params.appe
-0000fdc0: 6e64 2874 696d 655f 7061 7261 6d29 0a20  nd(time_param). 
-0000fdd0: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
-0000fde0: 732e 6170 7065 6e64 2865 6d61 696c 5f70  s.append(email_p
-0000fdf0: 6172 616d 290a 2020 2020 2020 2020 6a6f  aram).        jo
-0000fe00: 625f 7061 7261 6d20 3d20 2222 2e6a 6f69  b_param = "".joi
-0000fe10: 6e28 6a6f 625f 7061 7261 6d73 290a 2020  n(job_params).  
-0000fe20: 2020 2020 2020 7362 6174 6368 5f63 6d64        sbatch_cmd
-0000fe30: 203d 2066 2273 6261 7463 687b 6a6f 625f   = f"sbatch{job_
-0000fe40: 7061 7261 6d7d 202d 2d6f 7574 7075 743d  param} --output=
-0000fe50: 6f6d 6572 6f2d 256a 2e6c 6f67 205c 0a20  omero-%j.log \. 
-0000fe60: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-0000fe70: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
-0000fe80: 7468 7d2f 7b6a 6f62 5f73 6372 6970 747d  th}/{job_script}
-0000fe90: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000fea0: 6e20 7362 6174 6368 5f63 6d64 2c20 656e  n sbatch_cmd, en
-0000feb0: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
-0000fec0: 6f6e 7665 7273 696f 6e5f 636f 6d6d 616e  onversion_comman
-0000fed0: 6428 7365 6c66 2c20 6461 7461 5f70 6174  d(self, data_pat
-0000fee0: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff00: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
-0000ff10: 6c65 3a20 7374 722c 0a20 2020 2020 2020  le: str,.       
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
-0000ff40: 6f72 6d61 743a 2073 7472 203d 2027 7a61  ormat: str = 'za
-0000ff50: 7272 272c 0a20 2020 2020 2020 2020 2020  rr',.           
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff70: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
-0000ff80: 743a 2073 7472 203d 2027 7469 6666 2729  t: str = 'tiff')
-0000ff90: 202d 3e20 5475 706c 655b 7374 722c 2044   -> Tuple[str, D
-0000ffa0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
-0000ffb0: 220a 2020 2020 2020 2020 4765 6e65 7261  ".        Genera
-0000ffc0: 7465 2053 6c75 726d 2063 6f6e 7665 7273  te Slurm convers
-0000ffd0: 696f 6e20 636f 6d6d 616e 6420 616e 6420  ion command and 
-0000ffe0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-0000fff0: 6162 6c65 7320 666f 7220 6461 7461 2063  ables for data c
-00010000: 6f6e 7665 7273 696f 6e2e 0a0a 2020 2020  onversion...    
-00010010: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00010020: 2020 2020 2020 6461 7461 5f70 6174 6820        data_path 
-00010030: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
-00010040: 6865 2064 6174 6120 666f 6c64 6572 2e0a  he data folder..
-00010050: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00010060: 6967 5f66 696c 6520 2873 7472 293a 2050  ig_file (str): P
-00010070: 6174 6820 746f 2074 6865 2063 6f6e 6669  ath to the confi
-00010080: 6775 7261 7469 6f6e 2066 696c 652e 0a20  guration file.. 
-00010090: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-000100a0: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
-000100b0: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
-000100c0: 6174 2028 6465 6661 756c 7420 6973 2027  at (default is '
-000100d0: 7a61 7272 2729 2e0a 2020 2020 2020 2020  zarr')..        
-000100e0: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
-000100f0: 7420 2873 7472 293a 2054 6172 6765 7420  t (str): Target 
-00010100: 6461 7461 2066 6f72 6d61 7420 2864 6566  data format (def
-00010110: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
-00010120: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00010130: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00010140: 7570 6c65 5b73 7472 2c20 4469 6374 5d3a  uple[str, Dict]:
-00010150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010160: 2041 2074 7570 6c65 2063 6f6e 7461 696e   A tuple contain
-00010170: 696e 6720 7468 6520 536c 7572 6d20 636f  ing the Slurm co
-00010180: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
-00010190: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-000101a0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
-000101b0: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-000101c0: 0a20 2020 2020 2020 2057 6172 6e69 6e67  .        Warning
-000101d0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-000101e0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
-000101f0: 656e 7461 7469 6f6e 206f 6e6c 7920 7375  entation only su
-00010200: 7070 6f72 7473 2063 6f6e 7665 7273 696f  pports conversio
-00010210: 6e20 6672 6f6d 2027 7a61 7272 2720 746f  n from 'zarr' to
-00010220: 2027 7469 6666 272e 0a20 2020 2020 2020   'tiff'..       
-00010230: 2020 2020 2049 6620 7573 696e 6720 6f74       If using ot
-00010240: 6865 7220 736f 7572 6365 206f 7220 7461  her source or ta
-00010250: 7267 6574 2066 6f72 6d61 7473 2c20 7573  rget formats, us
-00010260: 6572 7320 6d75 7374 2069 6d70 6c65 6d65  ers must impleme
-00010270: 6e74 2061 6e64 2063 6f6e 6669 6775 7265  nt and configure
-00010280: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00010290: 6974 696f 6e61 6c20 636f 6e76 6572 7465  itional converte
-000102a0: 7273 2074 6865 6d73 656c 7665 732e 0a20  rs themselves.. 
-000102b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000102c0: 2020 2069 6620 736f 7572 6365 5f66 6f72     if source_for
-000102d0: 6d61 7420 213d 2022 7a61 7272 2220 6f72  mat != "zarr" or
-000102e0: 2074 6172 6765 745f 666f 726d 6174 2021   target_format !
-000102f0: 3d20 2274 6966 6622 3a0a 2020 2020 2020  = "tiff":.      
-00010300: 2020 2020 2020 2320 5761 726e 2061 626f        # Warn abo
-00010310: 7574 2075 6e73 7570 706f 7274 6564 2063  ut unsupported c
-00010320: 6f6e 7665 7273 696f 6e3b 2061 6464 6974  onversion; addit
-00010330: 696f 6e61 6c20 636f 6e76 6572 7465 7273  ional converters
-00010340: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
-00010350: 2020 2020 2320 6164 6465 6420 6f75 7473      # added outs
-00010360: 6964 6520 6f75 7220 6b6e 6f77 6c65 6467  ide our knowledg
-00010370: 652e 0a20 2020 2020 2020 2020 2020 2023  e..            #
-00010380: 2043 6865 636b 696e 6720 536c 7572 6d27   Checking Slurm'
-00010390: 7320 6073 6c75 726d 5f63 6f6e 7665 7274  s `slurm_convert
-000103a0: 6572 735f 7061 7468 6020 6973 2073 6b69  ers_path` is ski
-000103b0: 7070 6564 2066 6f72 0a20 2020 2020 2020  pped for.       
-000103c0: 2020 2020 2023 2070 6572 666f 726d 616e       # performan
-000103d0: 6365 2072 6561 736f 6e73 2e0a 2020 2020  ce reasons..    
-000103e0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-000103f0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-00010400: 2020 2020 2020 2020 6622 436f 6e76 6572          f"Conver
-00010410: 7369 6f6e 2066 726f 6d20 7b73 6f75 7263  sion from {sourc
-00010420: 655f 666f 726d 6174 7d20 746f 207b 7461  e_format} to {ta
-00010430: 7267 6574 5f66 6f72 6d61 747d 2069 7320  rget_format} is 
-00010440: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00010450: 2064 6566 6175 6c74 2122 290a 0a20 2020   default!")..   
-00010460: 2020 2020 2063 686f 7365 6e5f 636f 6e76       chosen_conv
-00010470: 6572 7465 7220 3d20 6622 636f 6e76 6572  erter = f"conver
-00010480: 745f 7b73 6f75 7263 655f 666f 726d 6174  t_{source_format
-00010490: 7d5f 746f 5f7b 7461 7267 6574 5f66 6f72  }_to_{target_for
-000104a0: 6d61 747d 2e73 6966 220a 2020 2020 2020  mat}.sif".      
-000104b0: 2020 7362 6174 6368 5f65 6e76 203d 207b    sbatch_env = {
-000104c0: 0a20 2020 2020 2020 2020 2020 2022 4441  .            "DA
-000104d0: 5441 5f50 4154 4822 3a20 6622 7b64 6174  TA_PATH": f"{dat
-000104e0: 615f 7061 7468 7d22 2c0a 2020 2020 2020  a_path}",.      
-000104f0: 2020 2020 2020 2243 4f4e 5645 5253 494f        "CONVERSIO
-00010500: 4e5f 5041 5448 223a 2066 227b 7365 6c66  N_PATH": f"{self
-00010510: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
-00010520: 735f 7061 7468 7d22 2c0a 2020 2020 2020  s_path}",.      
-00010530: 2020 2020 2020 2243 4f4e 5645 5254 4552        "CONVERTER
-00010540: 5f49 4d41 4745 223a 2063 686f 7365 6e5f  _IMAGE": chosen_
-00010550: 636f 6e76 6572 7465 722c 0a20 2020 2020  converter,.     
-00010560: 2020 2020 2020 2022 5343 5249 5054 5f50         "SCRIPT_P
-00010570: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
-00010580: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
-00010590: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000105a0: 434f 4e46 4947 5f46 494c 4522 3a20 6622  CONFIG_FILE": f"
-000105b0: 7b63 6f6e 6669 675f 6669 6c65 7d22 0a20  {config_file}". 
-000105c0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000105d0: 2020 636f 6e76 6572 7369 6f6e 5f63 6d64    conversion_cmd
-000105e0: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
-000105f0: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
-00010600: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
-00010610: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
-00010620: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
-00010630: 2d2d 6172 7261 793d 312d 244e 2024 5343  --array=1-$N $SC
-00010640: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
-00010650: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
-00010660: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-00010670: 7369 6f6e 5f63 6d64 5f77 6169 7469 6e67  sion_cmd_waiting
-00010680: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
-00010690: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
-000106a0: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
-000106b0: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
-000106c0: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
-000106d0: 2d2d 6172 7261 793d 312d 244e 202d 2d77  --array=1-$N --w
-000106e0: 6169 7420 2453 4352 4950 545f 5041 5448  ait $SCRIPT_PATH
-000106f0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
-00010700: 6179 2e73 6822 0a0a 2020 2020 2020 2020  ay.sh"..        
-00010710: 7265 7475 726e 2063 6f6e 7665 7273 696f  return conversio
-00010720: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
-00010730: 760a 0a20 2020 2064 6566 2077 6f72 6b66  v..    def workf
-00010740: 6c6f 775f 7061 7261 6d73 5f74 6f5f 656e  low_params_to_en
-00010750: 7676 6172 7328 7365 6c66 2c20 2a2a 6b77  vvars(self, **kw
-00010760: 6172 6773 2920 2d3e 2044 6963 743a 0a20  args) -> Dict:. 
-00010770: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010780: 2020 2043 6f6e 7665 7274 2077 6f72 6b66     Convert workf
-00010790: 6c6f 7720 7061 7261 6d65 7465 7273 2074  low parameters t
-000107a0: 6f20 656e 7669 726f 6e6d 656e 7420 7661  o environment va
-000107b0: 7269 6162 6c65 732e 0a0a 2020 2020 2020  riables...      
-000107c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000107d0: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
-000107e0: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
-000107f0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-00010800: 6865 2077 6f72 6b66 6c6f 772e 0a0a 2020  he workflow...  
-00010810: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00010820: 2020 2020 2020 2020 2020 2044 6963 743a             Dict:
-00010830: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
-00010840: 6e74 6169 6e69 6e67 2074 6865 2065 6e76  ntaining the env
-00010850: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00010860: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00010870: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-00010880: 5f65 6e76 203d 207b 6b65 792e 7570 7065  _env = {key.uppe
-00010890: 7228 293a 2066 227b 7661 6c75 657d 2220  r(): f"{value}" 
-000108a0: 666f 7220 6b65 792c 0a20 2020 2020 2020  for key,.       
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2076 616c 7565 2069 6e20 6b77 6172 6773   value in kwargs
-000108d0: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
-000108e0: 2020 6c6f 6767 6572 2e64 6562 7567 2877    logger.debug(w
-000108f0: 6f72 6b66 6c6f 775f 656e 7629 0a20 2020  orkflow_env).   
-00010900: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
-00010910: 666c 6f77 5f65 6e76 0a0a 2020 2020 6465  flow_env..    de
-00010920: 6620 6765 745f 6365 6c6c 706f 7365 5f63  f get_cellpose_c
-00010930: 6f6d 6d61 6e64 2873 656c 662c 2069 6d61  ommand(self, ima
-00010940: 6765 5f76 6572 7369 6f6e 3a20 7374 722c  ge_version: str,
-00010950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010960: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00010970: 7075 745f 6461 7461 3a20 7374 722c 0a20  put_data: str,. 
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 6370 5f6d              cp_m
-000109a0: 6f64 656c 3a20 7374 722c 0a20 2020 2020  odel: str,.     
-000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109c0: 2020 2020 2020 2020 6e75 635f 6368 616e          nuc_chan
-000109d0: 6e65 6c3a 2069 6e74 2c0a 2020 2020 2020  nel: int,.      
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 2070 726f 625f 7468 7265         prob_thre
-00010a00: 7368 6f6c 643a 2066 6c6f 6174 2c0a 2020  shold: float,.  
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-00010a30: 6469 616d 6574 6572 3a20 666c 6f61 742c  diameter: float,
-00010a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a50: 2020 2020 2020 2020 2020 2020 2020 656d                em
-00010a60: 6169 6c3a 204f 7074 696f 6e61 6c5b 7374  ail: Optional[st
-00010a70: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2020 2020 2020 2020 7469 6d65 3a20 4f70          time: Op
-00010aa0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00010ab0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ad0: 2075 7365 5f67 7075 3a20 626f 6f6c 203d   use_gpu: bool =
-00010ae0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 6d6f 6465 6c3a 2073 7472 203d      model: str =
-00010b10: 2022 6365 6c6c 706f 7365 2229 202d 3e20   "cellpose") -> 
-00010b20: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
-00010b30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010b40: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
-00010b50: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
-00010b60: 6972 6f6e 6d65 6e74 2064 6963 7469 6f6e  ironment diction
-00010b70: 6172 7920 746f 2072 756e 2061 2043 656c  ary to run a Cel
-00010b80: 6c50 6f73 6520 6a6f 620a 2020 2020 2020  lPose job.      
-00010b90: 2020 6f6e 2074 6865 2053 6c75 726d 2077    on the Slurm w
-00010ba0: 6f72 6b6c 6f61 6420 6d61 6e61 6765 722e  orkload manager.
-00010bb0: 0a20 2020 2020 2020 2041 2073 7065 6369  .        A speci
-00010bc0: 6669 6320 6578 616d 706c 6520 6f66 2075  fic example of u
-00010bd0: 7369 6e67 2074 6865 2067 656e 6572 6963  sing the generic
-00010be0: 2027 6765 745f 776f 726b 666c 6f77 5f63   'get_workflow_c
-00010bf0: 6f6d 6d61 6e64 272e 0a0a 2020 2020 2020  ommand'...      
-00010c00: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00010c10: 2020 2020 696d 6167 655f 7665 7273 696f      image_versio
-00010c20: 6e20 2873 7472 293a 2054 6865 2076 6572  n (str): The ver
-00010c30: 7369 6f6e 206f 6620 7468 6520 5369 6e67  sion of the Sing
-00010c40: 756c 6172 6974 7920 696d 6167 6520 746f  ularity image to
-00010c50: 2075 7365 2e0a 2020 2020 2020 2020 2020   use..          
-00010c60: 2020 696e 7075 745f 6461 7461 2028 7374    input_data (st
-00010c70: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
-00010c80: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
-00010c90: 6f6c 6465 7220 6f6e 2074 6865 2073 6861  older on the sha
-00010ca0: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
-00010cb0: 2020 2020 6669 6c65 2073 7973 7465 6d2e      file system.
-00010cc0: 0a20 2020 2020 2020 2020 2020 2063 705f  .            cp_
-00010cd0: 6d6f 6465 6c20 2873 7472 293a 2054 6865  model (str): The
-00010ce0: 206e 616d 6520 6f66 2074 6865 2043 656c   name of the Cel
-00010cf0: 6c50 6f73 6520 6d6f 6465 6c20 746f 2075  lPose model to u
-00010d00: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
-00010d10: 6e75 635f 6368 616e 6e65 6c20 2869 6e74  nuc_channel (int
-00010d20: 293a 2054 6865 2069 6e64 6578 206f 6620  ): The index of 
-00010d30: 7468 6520 6e75 636c 6561 7220 6368 616e  the nuclear chan
-00010d40: 6e65 6c2e 0a20 2020 2020 2020 2020 2020  nel..           
-00010d50: 2070 726f 625f 7468 7265 7368 6f6c 6420   prob_threshold 
-00010d60: 2866 6c6f 6174 293a 2054 6865 2070 726f  (float): The pro
-00010d70: 6261 6269 6c69 7479 2074 6872 6573 686f  bability thresho
-00010d80: 6c64 2066 6f72 0a20 2020 2020 2020 2020  ld for.         
-00010d90: 2020 2020 2020 206e 7563 6c65 6920 6465         nuclei de
-00010da0: 7465 6374 696f 6e2e 0a20 2020 2020 2020  tection..       
-00010db0: 2020 2020 2063 656c 6c5f 6469 616d 6574       cell_diamet
-00010dc0: 6572 2028 666c 6f61 7429 3a20 5468 6520  er (float): The 
-00010dd0: 6578 7065 6374 6564 2063 656c 6c20 6469  expected cell di
-00010de0: 616d 6574 6572 2069 6e20 7069 7865 6c73  ameter in pixels
-00010df0: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
-00010e00: 6169 6c20 284f 7074 696f 6e61 6c5b 7374  ail (Optional[st
-00010e10: 725d 293a 2054 6865 2065 6d61 696c 2061  r]): The email a
-00010e20: 6464 7265 7373 2074 6f20 7365 6e64 206e  ddress to send n
-00010e30: 6f74 6966 6963 6174 696f 6e73 2074 6f2e  otifications to.
-00010e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010e50: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00010e60: 652e 0a20 2020 2020 2020 2020 2020 2074  e..            t
-00010e70: 696d 6520 284f 7074 696f 6e61 6c5b 7374  ime (Optional[st
-00010e80: 725d 293a 2054 6865 206d 6178 696d 756d  r]): The maximum
-00010e90: 2074 696d 6520 666f 7220 7468 6520 6a6f   time for the jo
-00010ea0: 6220 746f 2072 756e 2e0a 2020 2020 2020  b to run..      
-00010eb0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00010ec0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00010ed0: 2020 2020 2020 2020 7573 655f 6770 7520          use_gpu 
-00010ee0: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
-00010ef0: 746f 2075 7365 2047 5055 2066 6f72 2074  to use GPU for t
-00010f00: 6865 2043 656c 6c50 6f73 6520 6a6f 622e  he CellPose job.
-00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f20: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00010f30: 652e 0a20 2020 2020 2020 2020 2020 206d  e..            m
-00010f40: 6f64 656c 2028 7374 7229 3a20 5468 6520  odel (str): The 
-00010f50: 6e61 6d65 206f 6620 7468 6520 666f 6c64  name of the fold
-00010f60: 6572 206f 6620 7468 6520 446f 636b 6572  er of the Docker
-00010f70: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00010f90: 6566 6175 6c74 7320 746f 2022 6365 6c6c  efaults to "cell
-00010fa0: 706f 7365 222e 0a0a 2020 2020 2020 2020  pose"...        
-00010fb0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00010fc0: 2020 2020 2054 7570 6c65 5b73 7472 2c20       Tuple[str, 
-00010fd0: 6469 6374 5d3a 0a20 2020 2020 2020 2020  dict]:.         
-00010fe0: 2020 2020 2020 2041 2074 7570 6c65 2063         A tuple c
-00010ff0: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
-00011000: 7572 6d20 7362 6174 6368 2063 6f6d 6d61  urm sbatch comma
-00011010: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00011020: 2020 2061 6e64 2074 6865 2065 6e76 6972     and the envir
-00011030: 6f6e 6d65 6e74 2064 6963 7469 6f6e 6172  onment dictionar
-00011040: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-00011050: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011060: 6c66 2e67 6574 5f77 6f72 6b66 6c6f 775f  lf.get_workflow_
-00011070: 636f 6d6d 616e 6428 776f 726b 666c 6f77  command(workflow
-00011080: 3d6d 6f64 656c 2c0a 2020 2020 2020 2020  =model,.        
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
-000110c0: 6e3d 696d 6167 655f 7665 7273 696f 6e2c  n=image_version,
-000110d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-00011100: 6461 7461 3d69 6e70 7574 5f64 6174 612c  data=input_data,
-00011110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 656d 6169 6c3d            email=
-00011140: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 7469 6d65 3d74 696d 652c 0a20 2020 2020  time=time,.     
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 6370 5f6d 6f64 656c 3d63 705f      cp_model=cp_
-000111b0: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 6e75 635f 6368 616e 6e65 6c3d 6e75 635f  nuc_channel=nuc_
-000111f0: 6368 616e 6e65 6c2c 0a20 2020 2020 2020  channel,.       
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 7072 6f62 5f74 6872 6573 686f 6c64    prob_threshold
-00011230: 3d70 726f 625f 7468 7265 7368 6f6c 642c  =prob_threshold,
-00011240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011260: 2020 2020 2020 2020 2020 6365 6c6c 5f64            cell_d
-00011270: 6961 6d65 7465 723d 6365 6c6c 5f64 6961  iameter=cell_dia
-00011280: 6d65 7465 722c 0a20 2020 2020 2020 2020  meter,.         
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 7573 655f 6770 753d 7573 655f 6770 7529  use_gpu=use_gpu)
-000112c0: 0a0a 2020 2020 6465 6620 636f 7079 5f7a  ..    def copy_z
-000112d0: 6970 5f6c 6f63 616c 6c79 2873 656c 662c  ip_locally(self,
-000112e0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
-000112f0: 6765 3a20 7374 722c 2066 696c 656e 616d  ge: str, filenam
-00011300: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2920 2d3e 2054 7261 6e73 6665 7252 6573  ) -> TransferRes
-00011330: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
-00011340: 2043 6f70 7920 6120 7a69 7020 6669 6c65   Copy a zip file
-00011350: 2066 726f 6d20 536c 7572 6d20 746f 2074   from Slurm to t
-00011360: 6865 206c 6f63 616c 2073 6572 7665 722e  he local server.
-00011370: 0a0a 2020 2020 2020 2020 4e6f 7465 2061  ..        Note a
-00011380: 626f 7574 2028 5472 616e 7366 6572 2952  bout (Transfer)R
-00011390: 6573 756c 743a 0a0a 2020 2020 2020 2020  esult:..        
-000113a0: 556e 6c69 6b65 2073 696d 696c 6172 2063  Unlike similar c
-000113b0: 6c61 7373 6573 2073 7563 6820 6173 2069  lasses such as i
-000113c0: 6e76 6f6b 652e 7275 6e6e 6572 732e 5265  nvoke.runners.Re
-000113d0: 7375 6c74 206f 720a 2020 2020 2020 2020  sult or.        
-000113e0: 6661 6272 6963 2e72 756e 6e65 7273 2e52  fabric.runners.R
-000113f0: 6573 756c 740a 2020 2020 2020 2020 2877  esult.        (w
-00011400: 6869 6368 2068 6176 6520 6120 636f 6e63  hich have a conc
-00011410: 6570 7420 6f66 20e2 809c 7761 726e 2061  ept of ...warn a
-00011420: 6e64 2072 6574 7572 6e20 616e 7977 6179  nd return anyway
-00011430: 7320 6f6e 2066 6169 6c75 7265 e280 9d29  s on failure...)
-00011440: 0a20 2020 2020 2020 2074 6869 7320 636c  .        this cl
-00011450: 6173 7320 6861 7320 6e6f 2075 7365 6675  ass has no usefu
-00011460: 6c20 7472 7574 6869 6e65 7373 2062 6568  l truthiness beh
-00011470: 6176 696f 722e 0a20 2020 2020 2020 2049  avior..        I
-00011480: 6620 6120 6669 6c65 2074 7261 6e73 6665  f a file transfe
-00011490: 7220 6661 696c 732c 2073 6f6d 6520 6578  r fails, some ex
-000114a0: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
-000114b0: 7261 6973 6564 2c0a 2020 2020 2020 2020  raised,.        
-000114c0: 6569 7468 6572 2061 6e20 4f53 4572 726f  either an OSErro
-000114d0: 7220 6f72 2061 6e20 6572 726f 7220 6672  r or an error fr
-000114e0: 6f6d 2077 6974 6869 6e20 5061 7261 6d69  om within Parami
-000114f0: 6b6f 2e0a 0a20 2020 2020 2020 2041 7267  ko...        Arg
-00011500: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-00011510: 6f63 616c 5f74 6d70 5f73 746f 7261 6765  ocal_tmp_storage
-00011520: 2028 5374 7269 6e67 293a 2050 6174 6820   (String): Path 
-00011530: 746f 2073 746f 7265 2074 6865 207a 6970  to store the zip
-00011540: 2066 696c 6520 6c6f 6361 6c6c 792e 0a20   file locally.. 
-00011550: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-00011560: 616d 6520 2853 7472 696e 6729 3a20 5a69  ame (String): Zi
-00011570: 7020 6669 6c65 6e61 6d65 206f 6e20 536c  p filename on Sl
-00011580: 7572 6d2e 0a0a 2020 2020 2020 2020 5265  urm...        Re
-00011590: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000115a0: 2020 2054 7261 6e73 6665 7252 6573 756c     TransferResul
-000115b0: 743a 2054 6865 2072 6573 756c 7420 6f66  t: The result of
-000115c0: 2074 6865 2073 6370 2061 7474 656d 7074   the scp attempt
-000115d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000115e0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000115f0: 6f28 6622 436f 7079 696e 6720 7a69 7020  o(f"Copying zip 
-00011600: 7b66 696c 656e 616d 657d 2066 726f 6d5c  {filename} from\
-00011610: 0a20 2020 2020 2020 2020 2020 2053 6c75  .            Slu
-00011620: 726d 2074 6f20 7b6c 6f63 616c 5f74 6d70  rm to {local_tmp
-00011630: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
-00011640: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011650: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00011660: 2072 656d 6f74 653d 6622 7b66 696c 656e   remote=f"{filen
-00011670: 616d 657d 2e7a 6970 222c 0a20 2020 2020  ame}.zip",.     
-00011680: 2020 2020 2020 206c 6f63 616c 3d6c 6f63         local=loc
-00011690: 616c 5f74 6d70 5f73 746f 7261 6765 290a  al_tmp_storage).
-000116a0: 0a20 2020 2064 6566 207a 6970 5f64 6174  .    def zip_dat
-000116b0: 615f 6f6e 5f73 6c75 726d 5f73 6572 7665  a_on_slurm_serve
-000116c0: 7228 7365 6c66 2c20 6461 7461 5f6c 6f63  r(self, data_loc
-000116d0: 6174 696f 6e3a 2073 7472 2c20 6669 6c65  ation: str, file
-000116e0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 2020 2020 2020 2020 656e 763a              env:
-00011710: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-00011720: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
-00011730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 2020 2920 2d3e 2052 6573 756c 743a 0a20    ) -> Result:. 
-00011760: 2020 2020 2020 2022 2222 5a69 7020 7468         """Zip th
-00011770: 6520 6f75 7470 7574 2066 6f6c 6465 7220  e output folder 
-00011780: 6f66 2061 206a 6f62 206f 6e20 536c 7572  of a job on Slur
-00011790: 6d0a 0a20 2020 2020 2020 2041 7267 733a  m..        Args:
-000117a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000117b0: 615f 6c6f 6361 7469 6f6e 2028 5374 7269  a_location (Stri
-000117c0: 6e67 293a 2046 6f6c 6465 7220 6f6e 2053  ng): Folder on S
-000117d0: 4c55 524d 2077 6974 6820 7468 6520 2264  LURM with the "d
-000117e0: 6174 612f 6f75 7422 0a20 2020 2020 2020  ata/out".       
-000117f0: 2020 2020 2020 2020 2073 7562 666f 6c64           subfold
-00011800: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-00011810: 6669 6c65 6e61 6d65 2028 5374 7269 6e67  filename (String
-00011820: 293a 204e 616d 6520 746f 2067 6976 6520  ): Name to give 
-00011830: 746f 2074 6865 207a 6970 6669 6c65 2e0a  to the zipfile..
-00011840: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00011850: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
-00011860: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
-00011870: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
-00011880: 2076 6172 6961 626c 6573 2074 6f20 0a20   variables to . 
-00011890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000118a0: 6574 2077 6865 6e20 7275 6e6e 696e 6720  et when running 
-000118b0: 7468 6520 636f 6d6d 616e 642e 2044 6566  the command. Def
-000118c0: 6175 6c74 7320 746f 204e 6f6e 652e 0a0a  aults to None...
-000118d0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000118e0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
-000118f0: 756c 743a 2054 6865 2072 6573 756c 7420  ult: The result 
-00011900: 6f66 2074 6865 207a 6970 2061 7474 656d  of the zip attem
-00011910: 7074 2e0a 2020 2020 2020 2020 2222 220a  pt..        """.
-00011920: 2020 2020 2020 2020 2320 7a69 700a 2020          # zip.  
-00011930: 2020 2020 2020 7a69 705f 636d 6420 3d20        zip_cmd = 
-00011940: 7365 6c66 2e67 6574 5f7a 6970 5f63 6f6d  self.get_zip_com
-00011950: 6d61 6e64 2864 6174 615f 6c6f 6361 7469  mand(data_locati
-00011960: 6f6e 2c20 6669 6c65 6e61 6d65 290a 2020  on, filename).  
-00011970: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00011980: 6f28 6622 5a69 7070 696e 6720 7b64 6174  o(f"Zipping {dat
-00011990: 615f 6c6f 6361 7469 6f6e 7d20 6173 207b  a_location} as {
-000119a0: 6669 6c65 6e61 6d65 7d20 6f6e 2053 6c75  filename} on Slu
-000119b0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
-000119c0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
-000119d0: 6d61 6e64 7328 5b7a 6970 5f63 6d64 5d2c  mands([zip_cmd],
-000119e0: 2065 6e76 3d65 6e76 290a 0a20 2020 2064   env=env)..    d
-000119f0: 6566 2067 6574 5f7a 6970 5f63 6f6d 6d61  ef get_zip_comma
-00011a00: 6e64 2873 656c 662c 2064 6174 615f 6c6f  nd(self, data_lo
-00011a10: 6361 7469 6f6e 3a20 7374 722c 2066 696c  cation: str, fil
-00011a20: 656e 616d 653a 2073 7472 2920 2d3e 2073  ename: str) -> s
-00011a30: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
-00011a40: 2020 2020 2020 2020 4765 6e65 7261 7465          Generate
-00011a50: 2061 2063 6f6d 6d61 6e64 2073 7472 696e   a command strin
-00011a60: 6720 666f 7220 7a69 7070 696e 6720 7468  g for zipping th
-00011a70: 6520 6461 7461 206f 6e20 536c 7572 6d2e  e data on Slurm.
-00011a80: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00011a90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00011aa0: 5f6c 6f63 6174 696f 6e20 2873 7472 293a  _location (str):
-00011ab0: 2054 6865 2066 6f6c 6465 7220 746f 2062   The folder to b
-00011ac0: 6520 7a69 7070 6564 2e0a 2020 2020 2020  e zipped..      
-00011ad0: 2020 2020 2020 6669 6c65 6e61 6d65 2028        filename (
-00011ae0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-00011af0: 6620 7468 6520 7a69 7020 6172 6368 6976  f the zip archiv
-00011b00: 6520 6669 6c65 2074 6f20 6578 7472 6163  e file to extrac
-00011b10: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
-00011b20: 2020 2057 6974 686f 7574 2065 7874 656e     Without exten
-00011b30: 7369 6f6e 2e0a 0a20 2020 2020 2020 2052  sion...        R
-00011b40: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00011b50: 2020 2020 7374 723a 2054 6865 2063 6f6d      str: The com
-00011b60: 6d61 6e64 2074 6f20 6372 6561 7465 2074  mand to create t
-00011b70: 6865 207a 6970 2066 696c 652e 0a20 2020  he zip file..   
-00011b80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011b90: 2072 6574 7572 6e20 7365 6c66 2e5f 5a49   return self._ZI
-00011ba0: 505f 434d 442e 666f 726d 6174 2866 696c  P_CMD.format(fil
-00011bb0: 656e 616d 653d 6669 6c65 6e61 6d65 2c0a  ename=filename,.
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
-00011bf0: 6e3d 6461 7461 5f6c 6f63 6174 696f 6e29  n=data_location)
-00011c00: 0a0a 2020 2020 6465 6620 6765 745f 6c6f  ..    def get_lo
-00011c10: 6766 696c 655f 6672 6f6d 5f73 6c75 726d  gfile_from_slurm
-00011c20: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c40: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
-00011c50: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
-00011c80: 705f 7374 6f72 6167 653a 2073 7472 203d  p_storage: str =
-00011c90: 2022 2f74 6d70 2f22 2c0a 2020 2020 2020   "/tmp/",.      
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00011cc0: 3a20 7374 7220 3d20 4e6f 6e65 0a20 2020  : str = None.   
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-00011cf0: 2054 7570 6c65 5b73 7472 2c20 7374 722c   Tuple[str, str,
-00011d00: 2054 7261 6e73 6665 7252 6573 756c 745d   TransferResult]
-00011d10: 3a0a 2020 2020 2020 2020 2222 2243 6f70  :.        """Cop
-00011d20: 7920 7468 6520 6c6f 6766 696c 6520 6f66  y the logfile of
-00011d30: 2074 6865 2067 6976 656e 2053 4c55 524d   the given SLURM
-00011d40: 206a 6f62 2074 6f20 7468 6520 6c6f 6361   job to the loca
-00011d50: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
-00011d60: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
-00011d70: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
-00011d80: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
-00011d90: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
-00011da0: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
-00011db0: 756e 6e65 7273 2e52 6573 756c 740a 2020  unners.Result.  
-00011dc0: 2020 2020 2020 6f72 2066 6162 7269 632e        or fabric.
-00011dd0: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
-00011de0: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
-00011df0: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
-00011e00: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
-00011e10: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
-00011e20: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
-00011e30: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
-00011e40: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
-00011e50: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
-00011e60: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
-00011e70: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
-00011e80: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
-00011e90: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
-00011ea0: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
-00011eb0: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
-00011ec0: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
-00011ed0: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
-00011ee0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00011ef0: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
-00011f00: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
-00011f10: 4944 206f 6620 7468 6520 534c 5552 4d20  ID of the SLURM 
-00011f20: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
-00011f30: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
-00011f40: 6765 2028 7374 722c 206f 7074 696f 6e61  ge (str, optiona
-00011f50: 6c29 3a20 5061 7468 2074 6f20 7374 6f72  l): Path to stor
-00011f60: 6520 7468 6520 6c6f 6766 696c 6520 0a20  e the logfile . 
-00011f70: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011f80: 6f63 616c 6c79 2e20 4465 6661 756c 7473  ocally. Defaults
-00011f90: 2074 6f20 222f 746d 702f 222e 0a20 2020   to "/tmp/"..   
-00011fa0: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00011fb0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00011fc0: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
-00011fd0: 6766 696c 6520 6f6e 2074 6865 2053 4c55  gfile on the SLU
-00011fe0: 524d 2073 6572 7665 722e 0a20 2020 2020  RM server..     
-00011ff0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00012000: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
-00012010: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00012020: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00012030: 3a20 6469 7265 6374 6f72 792c 2066 756c  : directory, ful
-00012040: 6c20 7061 7468 206f 6620 7468 6520 6c6f  l path of the lo
-00012050: 6766 696c 652c 2061 6e64 2054 7261 6e73  gfile, and Trans
-00012060: 6665 7252 6573 756c 740a 2020 2020 2020  ferResult.      
-00012070: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00012080: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
-00012090: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-000120a0: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
-000120b0: 4746 494c 450a 2020 2020 2020 2020 6c6f  GFILE.        lo
-000120c0: 6766 696c 6520 3d20 6c6f 6766 696c 652e  gfile = logfile.
-000120d0: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
-000120e0: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
-000120f0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-00012100: 2e69 6e66 6f28 6622 436f 7079 696e 6720  .info(f"Copying 
-00012110: 6c6f 6766 696c 6520 7b6c 6f67 6669 6c65  logfile {logfile
-00012120: 7d20 6672 6f6d 2053 6c75 726d 5c0a 2020  } from Slurm\.  
-00012130: 2020 2020 2020 2020 2020 746f 207b 6c6f            to {lo
-00012140: 6361 6c5f 746d 705f 7374 6f72 6167 657d  cal_tmp_storage}
-00012150: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
-00012160: 7420 3d20 7365 6c66 2e67 6574 280a 2020  t = self.get(.  
-00012170: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-00012180: 3d6c 6f67 6669 6c65 2c0a 2020 2020 2020  =logfile,.      
-00012190: 2020 2020 2020 6c6f 6361 6c3d 6c6f 6361        local=loca
-000121a0: 6c5f 746d 705f 7374 6f72 6167 6529 0a20  l_tmp_storage). 
-000121b0: 2020 2020 2020 2065 7870 6f72 745f 6669         export_fi
-000121c0: 6c65 203d 206c 6f63 616c 5f74 6d70 5f73  le = local_tmp_s
-000121d0: 746f 7261 6765 2b6c 6f67 6669 6c65 0a20  torage+logfile. 
-000121e0: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
-000121f0: 6361 6c5f 746d 705f 7374 6f72 6167 652c  cal_tmp_storage,
-00012200: 2065 7870 6f72 745f 6669 6c65 2c20 7265   export_file, re
-00012210: 7375 6c74 0a0a 2020 2020 6465 6620 6765  sult..    def ge
-00012220: 745f 756e 7a69 705f 636f 6d6d 616e 6428  t_unzip_command(
-00012230: 7365 6c66 2c20 7a69 7066 696c 653a 2073  self, zipfile: s
-00012240: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-00012250: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00012260: 6c74 6572 5f66 696c 6574 7970 6573 3a20  lter_filetypes: 
-00012270: 7374 7220 3d20 222a 2e7a 6172 7220 2a2e  str = "*.zarr *.
-00012280: 7469 6666 202a 2e74 6966 220a 2020 2020  tiff *.tif".    
-00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 2020 2020 2020 2920 2d3e 2073 7472 3a0a        ) -> str:.
-000122b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000122c0: 2020 2020 4765 6e65 7261 7465 2061 2063      Generate a c
-000122d0: 6f6d 6d61 6e64 2073 7472 696e 6720 666f  ommand string fo
-000122e0: 7220 756e 7a69 7070 696e 6720 6120 6461  r unzipping a da
-000122f0: 7461 2061 7263 6869 7665 2061 6e64 2063  ta archive and c
-00012300: 7265 6174 696e 670a 2020 2020 2020 2020  reating.        
-00012310: 7265 7175 6972 6564 2064 6972 6563 746f  required directo
-00012320: 7269 6573 2066 6f72 2053 6c75 726d 206a  ries for Slurm j
-00012330: 6f62 732e 0a0a 2020 2020 2020 2020 4172  obs...        Ar
-00012340: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00012350: 7a69 7066 696c 6520 2873 7472 293a 2054  zipfile (str): T
-00012360: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
-00012370: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
-00012380: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
-00012390: 2020 2020 2020 2020 2020 2020 5769 7468              With
-000123a0: 6f75 7420 6578 7465 6e73 696f 6e2e 0a20  out extension.. 
-000123b0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-000123c0: 725f 6669 6c65 7479 7065 7320 2873 7472  r_filetypes (str
-000123d0: 2c20 6f70 7469 6f6e 616c 293a 2041 2073  , optional): A s
-000123e0: 7061 6365 2d73 6570 6172 6174 6564 2073  pace-separated s
-000123f0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00012400: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
-00012410: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
-00012420: 696f 6e73 2074 6f20 6578 7472 6163 7420  ions to extract 
-00012430: 6672 6f6d 2074 6865 207a 6970 2066 696c  from the zip fil
-00012440: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-00012450: 2020 2045 2e67 2e20 6465 6661 756c 7473     E.g. defaults
-00012460: 2074 6f20 222a 2e7a 6172 7220 2a2e 7469   to "*.zarr *.ti
-00012470: 6666 202a 2e74 6966 222e 0a20 2020 2020  ff *.tif"..     
-00012480: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
-00012490: 6e67 2074 6869 7320 6172 6775 6d65 6e74  ng this argument
-000124a0: 2074 6f20 604e 6f6e 6560 2077 696c 6c20   to `None` will 
-000124b0: 6f6d 6974 2074 6865 2066 696c 650a 2020  omit the file.  
-000124c0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-000124d0: 6c74 6572 2061 6e64 2065 7874 7261 6374  lter and extract
-000124e0: 2061 6c6c 2066 696c 6573 2e0a 0a20 2020   all files...   
-000124f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00012500: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
-00012510: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00012520: 6865 2063 6f6d 6d61 6e64 2074 6f20 6578  he command to ex
-00012530: 7472 6163 7420 7468 6520 7370 6563 6966  tract the specif
-00012540: 6965 640a 2020 2020 2020 2020 2020 2020  ied.            
-00012550: 2020 2020 6669 6c65 7479 7065 7320 6672      filetypes fr
-00012560: 6f6d 2074 6865 207a 6970 2066 696c 652e  om the zip file.
-00012570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012580: 2020 2020 2075 6e7a 6970 5f63 6d64 203d       unzip_cmd =
-00012590: 2066 226d 6b64 6972 207b 7365 6c66 2e73   f"mkdir {self.s
-000125a0: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
-000125b0: 7b7a 6970 6669 6c65 7d20 5c0a 2020 2020  {zipfile} \.    
-000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125d0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
-000125e0: 5f70 6174 687d 2f7b 7a69 7066 696c 657d  _path}/{zipfile}
-000125f0: 2f64 6174 6120 5c0a 2020 2020 2020 2020  /data \.        
-00012600: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
-00012610: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-00012620: 687d 2f7b 7a69 7066 696c 657d 2f64 6174  h}/{zipfile}/dat
-00012630: 612f 696e 205c 0a20 2020 2020 2020 2020  a/in \.         
-00012640: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00012650: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-00012660: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
-00012670: 2f6f 7574 205c 0a20 2020 2020 2020 2020  /out \.         
-00012680: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00012690: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-000126a0: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
-000126b0: 2f67 743b 205c 0a20 2020 2020 2020 2020  /gt; \.         
-000126c0: 2020 2020 2020 2020 2020 2037 7a20 7820             7z x 
-000126d0: 2d79 202d 6f7b 7365 6c66 2e73 6c75 726d  -y -o{self.slurm
-000126e0: 5f64 6174 615f 7061 7468 7d2f 7b7a 6970  _data_path}/{zip
-000126f0: 6669 6c65 7d2f 6461 7461 2f69 6e20 5c0a  file}/data/in \.
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2020 7b73 656c 662e 736c 7572 6d5f      {self.slurm_
-00012720: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
-00012730: 696c 657d 2e7a 6970 207b 6669 6c74 6572  ile}.zip {filter
-00012740: 5f66 696c 6574 7970 6573 7d22 0a0a 2020  _filetypes}"..  
-00012750: 2020 2020 2020 7265 7475 726e 2075 6e7a        return unz
-00012760: 6970 5f63 6d64 0a0a 2020 2020 6465 6620  ip_cmd..    def 
-00012770: 6765 745f 696d 6167 655f 7665 7273 696f  get_image_versio
-00012780: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
-00012790: 7328 7365 6c66 2c20 6d6f 6465 6c3a 2073  s(self, model: s
-000127a0: 7472 0a20 2020 2020 2020 2020 2020 2020  tr.             
-000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127c0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-000127d0: 3e20 5475 706c 655b 4c69 7374 5b73 7472  > Tuple[List[str
-000127e0: 5d2c 204c 6973 745b 7374 725d 5d3a 0a20  ], List[str]]:. 
-000127f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012800: 2020 2052 6574 7269 6576 6520 7468 6520     Retrieve the 
-00012810: 6176 6169 6c61 626c 6520 696d 6167 6520  available image 
-00012820: 7665 7273 696f 6e73 2061 6e64 2069 6e70  versions and inp
-00012830: 7574 2064 6174 6120 6669 6c65 7320 666f  ut data files fo
-00012840: 7220 610a 2020 2020 2020 2020 6769 7665  r a.        give
-00012850: 6e20 6d6f 6465 6c2e 0a0a 2020 2020 2020  n model...      
-00012860: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00012870: 2020 2020 6d6f 6465 6c20 2873 7472 293a      model (str):
-00012880: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00012890: 206d 6f64 656c 2074 6f20 7175 6572 7920   model to query 
-000128a0: 666f 722e 0a0a 2020 2020 2020 2020 5265  for...        Re
-000128b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000128c0: 2020 2054 7570 6c65 5b4c 6973 745b 7374     Tuple[List[st
-000128d0: 725d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  r], List[str]]:.
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128f0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-00012900: 6e67 2074 776f 206c 6973 7473 3a0a 2020  ng two lists:.  
-00012910: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00012920: 5468 6520 6669 7273 7420 6c69 7374 2069  The first list i
-00012930: 6e63 6c75 6465 7320 7468 6520 6176 6169  ncludes the avai
-00012940: 6c61 626c 6520 696d 6167 6520 7665 7273  lable image vers
-00012950: 696f 6e73 2c20 0a20 2020 2020 2020 2020  ions, .         
-00012960: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00012970: 6420 696e 2064 6573 6365 6e64 696e 6720  d in descending 
-00012980: 6f72 6465 722e 0a20 2020 2020 2020 2020  order..         
-00012990: 2020 2020 2020 202d 2054 6865 2073 6563         - The sec
-000129a0: 6f6e 6420 6c69 7374 2069 6e63 6c75 6465  ond list include
-000129b0: 7320 7468 6520 6176 6169 6c61 626c 6520  s the available 
-000129c0: 6461 7461 2066 696c 6573 2e0a 0a20 2020  data files...   
-000129d0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-000129e0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-000129f0: 726f 723a 2049 6620 7468 6520 7072 6f76  ror: If the prov
-00012a00: 6964 6564 206d 6f64 656c 2069 7320 6e6f  ided model is no
-00012a10: 7420 666f 756e 6420 696e 2074 6865 0a20  t found in the. 
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00012a30: 6c75 726d 436c 6965 6e74 2773 206b 6e6f  lurmClient's kno
-00012a40: 776e 206d 6f64 656c 2070 6174 6873 2e0a  wn model paths..
-00012a50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012a60: 2020 2020 696d 6167 655f 7061 7468 203d      image_path =
-00012a70: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-00012a80: 6c5f 7061 7468 732e 6765 7428 6d6f 6465  l_paths.get(mode
-00012a90: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
-00012aa0: 7420 696d 6167 655f 7061 7468 3a0a 2020  t image_path:.  
-00012ab0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00012ac0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00012ad0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
-00012ae0: 2070 6174 6820 6b6e 6f77 6e20 666f 7220   path known for 
-00012af0: 7072 6f76 6964 6564 206d 6f64 656c 207b  provided model {
-00012b00: 6d6f 6465 6c7d 2c20 5c0a 2020 2020 2020  model}, \.      
-00012b10: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00012b20: 207b 7365 6c66 2e73 6c75 726d 5f6d 6f64   {self.slurm_mod
-00012b30: 656c 5f70 6174 6873 7d22 290a 2020 2020  el_paths}").    
-00012b40: 2020 2020 636d 646c 6973 7420 3d20 5b0a      cmdlist = [.
-00012b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012b60: 2e5f 5645 5253 494f 4e5f 434d 442e 666f  ._VERSION_CMD.fo
-00012b70: 726d 6174 2873 6c75 726d 5f69 6d61 6765  rmat(slurm_image
-00012b80: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
-00012b90: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 696d 6167 655f 7061 7468 3d69      image_path=i
-00012bd0: 6d61 6765 5f70 6174 6829 2c0a 2020 2020  mage_path),.    
-00012be0: 2020 2020 2020 2020 7365 6c66 2e5f 4441          self._DA
-00012bf0: 5441 5f43 4d44 2e66 6f72 6d61 7428 736c  TA_CMD.format(sl
-00012c00: 7572 6d5f 6461 7461 5f70 6174 683d 7365  urm_data_path=se
-00012c10: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
-00012c20: 7468 295d 0a20 2020 2020 2020 2023 2073  th)].        # s
-00012c30: 706c 6974 2072 6573 706f 6e73 6573 2070  plit responses p
-00012c40: 6572 2063 6f6d 6d61 6e64 0a20 2020 2020  er command.     
-00012c50: 2020 2072 6573 706f 6e73 655f 6c69 7374     response_list
-00012c60: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00012c70: 616e 6473 5f73 706c 6974 5f6f 7574 2863  ands_split_out(c
-00012c80: 6d64 6c69 7374 290a 2020 2020 2020 2020  mdlist).        
-00012c90: 2320 7370 6c69 7420 6c69 6e65 7320 6675  # split lines fu
-00012ca0: 7274 6865 7220 696e 746f 2073 7562 6c69  rther into subli
-00012cb0: 7374 730a 2020 2020 2020 2020 7265 7370  sts.        resp
-00012cc0: 6f6e 7365 5f6c 6973 7420 3d20 5b72 6573  onse_list = [res
-00012cd0: 706f 6e73 652e 7374 7269 7028 292e 7370  ponse.strip().sp
-00012ce0: 6c69 7428 275c 6e27 290a 2020 2020 2020  lit('\n').      
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2066 6f72 2072 6573 706f 6e73 6520     for response 
-00012d10: 696e 2072 6573 706f 6e73 655f 6c69 7374  in response_list
-00012d20: 5d0a 2020 2020 2020 2020 7265 7370 6f6e  ].        respon
-00012d30: 7365 5f6c 6973 745b 305d 203d 2073 6f72  se_list[0] = sor
-00012d40: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
-00012d50: 745b 305d 2c20 7265 7665 7273 653d 5472  t[0], reverse=Tr
-00012d60: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
-00012d70: 726e 2072 6573 706f 6e73 655f 6c69 7374  rn response_list
-00012d80: 5b30 5d2c 2072 6573 706f 6e73 655f 6c69  [0], response_li
-00012d90: 7374 5b31 5d0a 0a20 2020 2064 6566 2067  st[1]..    def g
-00012da0: 6574 5f61 6c6c 5f69 6d61 6765 5f76 6572  et_all_image_ver
-00012db0: 7369 6f6e 735f 616e 645f 6461 7461 5f66  sions_and_data_f
-00012dc0: 696c 6573 2873 656c 660a 2020 2020 2020  iles(self.      
-00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
-00012e00: 6c65 5b44 6963 745b 7374 722c 204c 6973  le[Dict[str, Lis
-00012e10: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 4c69 7374 5b73 7472 5d5d 3a0a 2020    List[str]]:.  
-00012e60: 2020 2020 2020 2222 2252 6574 7269 6576        """Retriev
-00012e70: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
-00012e80: 696d 6167 6520 7665 7273 696f 6e73 2061  image versions a
-00012e90: 6e64 2064 6174 6120 6669 6c65 7320 6672  nd data files fr
-00012ea0: 6f6d 0a20 2020 2020 2020 2074 6865 2053  om.        the S
-00012eb0: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
-00012ec0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00012ed0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00012ee0: 5b44 6963 745b 7374 722c 204c 6973 745b  [Dict[str, List[
-00012ef0: 7374 725d 5d2c 204c 6973 745b 7374 725d  str]], List[str]
-00012f00: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012f10: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-00012f20: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
-00012f30: 2020 2020 2020 202d 2041 2064 6963 7469         - A dicti
-00012f40: 6f6e 6172 7920 6d61 7070 696e 6720 6d6f  onary mapping mo
-00012f50: 6465 6c73 2074 6f20 6176 6169 6c61 626c  dels to availabl
-00012f60: 6520 7665 7273 696f 6e73 2e0a 2020 2020  e versions..    
-00012f70: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
-00012f80: 6c69 7374 206f 6620 6176 6169 6c61 626c  list of availabl
-00012f90: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
-00012fa0: 6465 7273 2e0a 2020 2020 2020 2020 2222  ders..        ""
-00012fb0: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
-00012fc0: 6469 6374 203d 207b 7d0a 2020 2020 2020  dict = {}.      
-00012fd0: 2020 636d 646c 6973 7420 3d20 5b5d 0a0a    cmdlist = []..
-00012fe0: 2020 2020 2020 2020 666f 7220 7061 7468          for path
-00012ff0: 2069 6e20 7365 6c66 2e73 6c75 726d 5f6d   in self.slurm_m
-00013000: 6f64 656c 5f70 6174 6873 2e76 616c 7565  odel_paths.value
-00013010: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00013020: 2070 6174 6863 6d64 203d 2073 656c 662e   pathcmd = self.
-00013030: 5f56 4552 5349 4f4e 5f43 4d44 2e66 6f72  _VERSION_CMD.for
-00013040: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00013050: 2020 2020 2073 6c75 726d 5f69 6d61 6765       slurm_image
-00013060: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
-00013070: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
-00013080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013090: 6d61 6765 5f70 6174 683d 7061 7468 290a  mage_path=path).
-000130a0: 2020 2020 2020 2020 2020 2020 636d 646c              cmdl
-000130b0: 6973 742e 6170 7065 6e64 2870 6174 6863  ist.append(pathc
-000130c0: 6d64 290a 0a20 2020 2020 2020 2023 2041  md)..        # A
-000130d0: 6464 2064 6174 6120 7061 7468 2074 6f6f  dd data path too
-000130e0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
-000130f0: 2e61 7070 656e 6428 7365 6c66 2e5f 4441  .append(self._DA
-00013100: 5441 5f43 4d44 2e66 6f72 6d61 7428 0a20  TA_CMD.format(. 
-00013110: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-00013120: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
-00013130: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
-00013140: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
-00013150: 6974 2072 6573 706f 6e73 6573 2070 6572  it responses per
-00013160: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
-00013170: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
-00013180: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00013190: 6473 5f73 706c 6974 5f6f 7574 2863 6d64  ds_split_out(cmd
-000131a0: 6c69 7374 290a 0a20 2020 2020 2020 2023  list)..        #
-000131b0: 2053 706c 6974 206c 696e 6573 2066 7572   Split lines fur
-000131c0: 7468 6572 2069 6e74 6f20 7375 626c 6973  ther into sublis
-000131d0: 7473 0a20 2020 2020 2020 2072 6573 706f  ts.        respo
-000131e0: 6e73 655f 6c69 7374 203d 205b 7265 7370  nse_list = [resp
-000131f0: 6f6e 7365 2e73 7472 6970 2829 2e73 706c  onse.strip().spl
-00013200: 6974 2827 5c6e 2729 0a20 2020 2020 2020  it('\n').       
+0000a2b0: 656e 763a 204f 7074 696f 6e61 6c5b 4469  env: Optional[Di
+0000a2c0: 6374 5b73 7472 2c20 7374 725d 5d20 3d20  ct[str, str]] = 
+0000a2d0: 4e6f 6e65 2920 2d3e 2052 6573 756c 743a  None) -> Result:
+0000a2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000a2f0: 2020 2020 2055 6e70 6163 6b73 2061 207a       Unpacks a z
+0000a300: 6970 7065 6420 6669 6c65 206f 6e20 7468  ipped file on th
+0000a310: 6520 7265 6d6f 7465 2053 6c75 726d 2063  e remote Slurm c
+0000a320: 6c75 7374 6572 2e0a 0a20 2020 2020 2020  luster...       
+0000a330: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000a340: 2020 207a 6970 6669 6c65 2028 7374 7229     zipfile (str)
+0000a350: 3a20 5468 6520 6e61 6d65 206f 6620 7468  : The name of th
+0000a360: 6520 7a69 7070 6564 2066 696c 6520 746f  e zipped file to
+0000a370: 2062 6520 756e 7061 636b 6564 2e0a 0a20   be unpacked... 
+0000a380: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
+0000a390: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
+0000a3a0: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
+0000a3b0: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
+0000a3c0: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
+0000a3d0: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
+0000a3e0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+0000a3f0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+0000a400: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
+0000a410: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000a420: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
+0000a430: 6c74 3a20 5468 6520 7265 7375 6c74 206f  lt: The result o
+0000a440: 6620 7468 6520 636f 6d6d 616e 642e 0a20  f the command.. 
+0000a450: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000a460: 2020 2063 6d64 203d 2073 656c 662e 6765     cmd = self.ge
+0000a470: 745f 636f 6e76 6572 745f 636f 6d6d 616e  t_convert_comman
+0000a480: 6428 7a69 7066 696c 6529 0a20 2020 2020  d(zipfile).     
+0000a490: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+0000a4a0: 2243 6f6e 7665 7274 696e 6720 7b7a 6970  "Converting {zip
+0000a4b0: 6669 6c65 7d20 6f6e 2053 6c75 726d 2229  file} on Slurm")
+0000a4c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a4d0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+0000a4e0: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
+0000a4f0: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
+0000a500: 6174 655f 736c 7572 6d5f 6a6f 625f 666f  ate_slurm_job_fo
+0000a510: 725f 776f 726b 666c 6f77 2873 656c 662c  r_workflow(self,
+0000a520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000a550: 773a 2073 7472 2c0a 2020 2020 2020 2020  w: str,.        
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 7375 6273 7469 7475 7465 733a 2044 6963  substitutes: Dic
+0000a590: 745b 7374 722c 2073 7472 5d2c 0a20 2020  t[str, str],.   
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2020 2074 656d 706c 6174 653a 2073       template: s
+0000a5d0: 7472 203d 2022 6a6f 625f 7465 6d70 6c61  tr = "job_templa
+0000a5e0: 7465 2e73 6822 0a20 2020 2020 2020 2020  te.sh".         
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000a610: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000a620: 2022 2222 0a20 2020 2020 2020 2047 656e   """.        Gen
+0000a630: 6572 6174 6520 6120 536c 7572 6d20 6a6f  erate a Slurm jo
+0000a640: 6220 7363 7269 7074 2066 6f72 2061 2073  b script for a s
+0000a650: 7065 6369 6669 6320 776f 726b 666c 6f77  pecific workflow
+0000a660: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000a670: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+0000a680: 6b66 6c6f 7720 2873 7472 293a 2054 6865  kflow (str): The
+0000a690: 206e 616d 6520 6f66 2074 6865 2077 6f72   name of the wor
+0000a6a0: 6b66 6c6f 772e 0a20 2020 2020 2020 2020  kflow..         
+0000a6b0: 2020 2073 7562 7374 6974 7574 6573 2028     substitutes (
+0000a6c0: 4469 6374 5b73 7472 2c20 7374 725d 293a  Dict[str, str]):
+0000a6d0: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+0000a6e0: 6e74 6169 6e69 6e67 206b 6579 2d76 616c  ntaining key-val
+0000a6f0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+0000a700: 2020 2070 6169 7273 2066 6f72 2073 7562     pairs for sub
+0000a710: 7374 6974 7574 696e 6720 706c 6163 6568  stituting placeh
+0000a720: 6f6c 6465 7273 2069 6e20 7468 6520 6a6f  olders in the jo
+0000a730: 6220 7465 6d70 6c61 7465 2e0a 2020 2020  b template..    
+0000a740: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
+0000a750: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+0000a760: 3a20 5468 6520 6669 6c65 6e61 6d65 206f  : The filename o
+0000a770: 6620 7468 6520 6a6f 6220 7465 6d70 6c61  f the job templa
+0000a780: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
+0000a790: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+0000a7a0: 226a 6f62 5f74 656d 706c 6174 652e 7368  "job_template.sh
+0000a7b0: 222e 0a0a 2020 2020 2020 2020 5265 7475  "...        Retu
+0000a7c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000a7d0: 2073 7472 3a20 5468 6520 6765 6e65 7261   str: The genera
+0000a7e0: 7465 6420 536c 7572 6d20 6a6f 6220 7363  ted Slurm job sc
+0000a7f0: 7269 7074 2061 7320 6120 7374 7269 6e67  ript as a string
+0000a800: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000a810: 2020 2020 2020 2320 6164 6420 776f 726b        # add work
+0000a820: 666c 6f77 2074 6f20 7375 6273 7469 7475  flow to substitu
+0000a830: 7465 730a 2020 2020 2020 2020 7375 6273  tes.        subs
+0000a840: 7469 7475 7465 735b 276a 6f62 6e61 6d65  titutes['jobname
+0000a850: 275d 203d 2077 6f72 6b66 6c6f 770a 2020  '] = workflow.  
+0000a860: 2020 2020 2020 2320 6772 6162 206a 6f62        # grab job
+0000a870: 2074 656d 706c 6174 650a 2020 2020 2020   template.      
+0000a880: 2020 7465 6d70 6c61 7465 5f66 203d 2066    template_f = f
+0000a890: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
+0000a8a0: 292e 6a6f 696e 7061 7468 2874 656d 706c  ).joinpath(templ
+0000a8b0: 6174 6529 0a20 2020 2020 2020 2077 6974  ate).        wit
+0000a8c0: 6820 7465 6d70 6c61 7465 5f66 2e6f 7065  h template_f.ope
+0000a8d0: 6e28 2772 2729 2061 7320 663a 0a20 2020  n('r') as f:.   
+0000a8e0: 2020 2020 2020 2020 2073 7263 203d 2054           src = T
+0000a8f0: 656d 706c 6174 6528 662e 7265 6164 2829  emplate(f.read()
+0000a900: 290a 2020 2020 2020 2020 2020 2020 6a6f  ).            jo
+0000a910: 625f 7363 7269 7074 203d 2073 7263 2e73  b_script = src.s
+0000a920: 6166 655f 7375 6273 7469 7475 7465 2873  afe_substitute(s
+0000a930: 7562 7374 6974 7574 6573 290a 2020 2020  ubstitutes).    
+0000a940: 2020 2020 7265 7475 726e 206a 6f62 5f73      return job_s
+0000a950: 6372 6970 740a 0a20 2020 2064 6566 2077  cript..    def w
+0000a960: 6f72 6b66 6c6f 775f 7061 7261 6d73 5f74  orkflow_params_t
+0000a970: 6f5f 7375 6273 2873 656c 662c 2070 6172  o_subs(self, par
+0000a980: 616d 7329 202d 3e20 4469 6374 5b73 7472  ams) -> Dict[str
+0000a990: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
+0000a9a0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
+0000a9b0: 6572 7420 776f 726b 666c 6f77 2070 6172  ert workflow par
+0000a9c0: 616d 6574 6572 7320 746f 2073 7562 7374  ameters to subst
+0000a9d0: 6974 7574 696f 6e20 6469 6374 696f 6e61  itution dictiona
+0000a9e0: 7279 2066 6f72 206a 6f62 2073 6372 6970  ry for job scrip
+0000a9f0: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
+0000aa00: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000aa10: 7261 6d73 3a20 4120 6469 6374 696f 6e61  rams: A dictiona
+0000aa20: 7279 2063 6f6e 7461 696e 696e 6720 776f  ry containing wo
+0000aa30: 726b 666c 6f77 2070 6172 616d 6574 6572  rkflow parameter
+0000aa40: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
+0000aa50: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000aa60: 2044 6963 745b 7374 722c 2073 7472 5d3a   Dict[str, str]:
+0000aa70: 2041 2064 6963 7469 6f6e 6172 7920 7769   A dictionary wi
+0000aa80: 7468 2070 6172 616d 6574 6572 206e 616d  th parameter nam
+0000aa90: 6573 2061 7320 6b65 7973 2061 6e64 0a20  es as keys and. 
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000aab0: 6f72 7265 7370 6f6e 6469 6e67 2066 6c61  orresponding fla
+0000aac0: 6773 2077 6974 6820 706c 6163 6568 6f6c  gs with placehol
+0000aad0: 6465 7273 2061 7320 7661 6c75 6573 2e0a  ders as values..
+0000aae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000aaf0: 2020 2020 7375 6273 203d 207b 7d0a 2020      subs = {}.  
+0000ab00: 2020 2020 2020 666c 6167 7320 3d20 5b5d        flags = []
+0000ab10: 0a20 2020 2020 2020 2066 6f72 205f 2c20  .        for _, 
+0000ab20: 7061 7261 6d20 696e 2070 6172 616d 732e  param in params.
+0000ab30: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0000ab40: 2020 2020 2066 6c61 6720 3d20 7061 7261       flag = para
+0000ab50: 6d5b 2763 6d64 5f66 6c61 6727 5d0a 2020  m['cmd_flag'].  
+0000ab60: 2020 2020 2020 2020 2020 666c 6167 203d            flag =
+0000ab70: 2066 6c61 6720 2b20 2220 2422 202b 2070   flag + " $" + p
+0000ab80: 6172 616d 5b27 6e61 6d65 275d 2e75 7070  aram['name'].upp
+0000ab90: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+0000aba0: 2066 6c61 6773 2e61 7070 656e 6428 666c   flags.append(fl
+0000abb0: 6167 290a 2020 2020 2020 2020 7375 6273  ag).        subs
+0000abc0: 5b27 5041 5241 4d53 275d 203d 2022 2022  ['PARAMS'] = " "
+0000abd0: 2e6a 6f69 6e28 666c 6167 7329 0a20 2020  .join(flags).   
+0000abe0: 2020 2020 2072 6574 7572 6e20 7375 6273       return subs
+0000abf0: 0a0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
+0000ac00: 5f73 6c75 726d 5f73 6372 6970 7473 2873  _slurm_scripts(s
+0000ac10: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac30: 2020 6765 6e65 7261 7465 5f6a 6f62 733a    generate_jobs:
+0000ac40: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 2020 2020 656e 763a              env:
+0000ac70: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+0000ac80: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
+0000ac90: 2920 2d3e 2052 6573 756c 743a 0a20 2020  ) -> Result:.   
+0000aca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000acb0: 2055 7064 6174 6573 2074 6865 206c 6f63   Updates the loc
+0000acc0: 616c 2063 6f70 7920 6f66 2074 6865 2053  al copy of the S
+0000acd0: 6c75 726d 206a 6f62 2073 7562 6d69 7373  lurm job submiss
+0000ace0: 696f 6e20 7363 7269 7074 732e 0a0a 2020  ion scripts...  
+0000acf0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+0000ad00: 696f 6e20 7075 6c6c 7320 7468 6520 6c61  ion pulls the la
+0000ad10: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+0000ad20: 7468 6520 7363 7269 7074 7320 6672 6f6d  the scripts from
+0000ad30: 2074 6865 2047 6974 0a20 2020 2020 2020   the Git.       
+0000ad40: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
+0000ad50: 636f 7069 6573 2074 6865 6d20 746f 2074  copies them to t
+0000ad60: 6865 2073 6c75 726d 5f73 6372 6970 745f  he slurm_script_
+0000ad70: 7061 7468 2064 6972 6563 746f 7279 2e0a  path directory..
+0000ad80: 2020 2020 2020 2020 416c 7465 726e 6174          Alternat
+0000ad90: 6976 656c 792c 2069 7420 6361 6e20 6765  ively, it can ge
+0000ada0: 6e65 7261 7465 2073 6372 6970 7473 2066  nerate scripts f
+0000adb0: 726f 6d20 6120 7465 6d70 6c61 7465 2e20  rom a template. 
+0000adc0: 5468 6973 2069 7320 7468 650a 2020 2020  This is the.    
+0000add0: 2020 2020 6465 6661 756c 7420 6265 6861      default beha
+0000ade0: 7669 6f72 2069 6620 6e6f 2047 6974 2072  vior if no Git r
+0000adf0: 6570 6f20 6973 2070 726f 7669 6465 6420  epo is provided 
+0000ae00: 6f72 2063 616e 2062 6520 666f 7263 6564  or can be forced
+0000ae10: 2076 6961 2074 6865 0a20 2020 2020 2020   via the.       
+0000ae20: 2060 6765 6e65 7261 7465 5f6a 6f62 7360   `generate_jobs`
+0000ae30: 2070 6172 616d 6574 6572 2e0a 0a20 2020   parameter...   
+0000ae40: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000ae50: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
+0000ae60: 6a6f 6273 2028 626f 6f6c 293a 2057 6865  jobs (bool): Whe
+0000ae70: 7468 6572 2074 6f20 6765 6e65 7261 7465  ther to generate
+0000ae80: 206e 6577 2073 6c75 726d 206a 6f62 2073   new slurm job s
+0000ae90: 6372 6970 7473 0a20 2020 2020 2020 2020  cripts.         
+0000aea0: 2020 2020 2020 2049 4e53 5445 4144 2028         INSTEAD (
+0000aeb0: 6f66 2070 756c 6c69 6e67 2066 726f 6d20  of pulling from 
+0000aec0: 6769 7429 2e20 4465 6661 756c 7473 2074  git). Defaults t
+0000aed0: 6f20 4661 6c73 652c 2065 7863 6570 740a  o False, except.
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aef0: 6966 206e 6f20 736c 7572 6d5f 7363 7269  if no slurm_scri
+0000af00: 7074 5f72 6570 6f20 6973 2063 6f6e 6669  pt_repo is confi
+0000af10: 6775 7265 642e 0a20 2020 2020 2020 2020  gured..         
+0000af20: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
+0000af30: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
+0000af40: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
+0000af50: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+0000af60: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
+0000af70: 2020 2074 6f20 7365 7420 7768 656e 2072     to set when r
+0000af80: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
+0000af90: 6e64 2e20 4465 6661 756c 7473 2074 6f20  nd. Defaults to 
+0000afa0: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
+0000afb0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000afc0: 2020 2020 5265 7375 6c74 3a20 5468 6520      Result: The 
+0000afd0: 7265 7375 6c74 206f 6620 7468 6520 636f  result of the co
+0000afe0: 6d6d 616e 642e 0a20 2020 2020 2020 2022  mmand..        "
+0000aff0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+0000b000: 7420 7365 6c66 2e73 6c75 726d 5f73 6372  t self.slurm_scr
+0000b010: 6970 745f 7265 706f 3a0a 2020 2020 2020  ipt_repo:.      
+0000b020: 2020 2020 2020 6765 6e65 7261 7465 5f6a        generate_j
+0000b030: 6f62 7320 3d20 5472 7565 0a0a 2020 2020  obs = True..    
+0000b040: 2020 2020 6966 2067 656e 6572 6174 655f      if generate_
+0000b050: 6a6f 6273 3a0a 2020 2020 2020 2020 2020  jobs:.          
+0000b060: 2020 6c6f 6767 6572 2e69 6e66 6f28 2247    logger.info("G
+0000b070: 656e 6572 6174 696e 6720 536c 7572 6d20  enerating Slurm 
+0000b080: 6a6f 6220 7363 7269 7074 7322 290a 2020  job scripts").  
+0000b090: 2020 2020 2020 2020 2020 666f 7220 7766            for wf
+0000b0a0: 2c20 6a6f 625f 7061 7468 2069 6e20 7365  , job_path in se
+0000b0b0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f6a  lf.slurm_model_j
+0000b0c0: 6f62 732e 6974 656d 7328 293a 0a20 2020  obs.items():.   
+0000b0d0: 2020 2020 2020 2020 2020 2020 2023 2067               # g
+0000b0e0: 656e 6572 6174 6520 6a6f 6220 7363 7269  enerate job scri
+0000b0f0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
+0000b100: 2020 2070 6172 616d 7320 3d20 7365 6c66     params = self
+0000b110: 2e67 6574 5f77 6f72 6b66 6c6f 775f 7061  .get_workflow_pa
+0000b120: 7261 6d65 7465 7273 2877 6629 0a20 2020  rameters(wf).   
+0000b130: 2020 2020 2020 2020 2020 2020 2073 7562               sub
+0000b140: 7320 3d20 7365 6c66 2e77 6f72 6b66 6c6f  s = self.workflo
+0000b150: 775f 7061 7261 6d73 5f74 6f5f 7375 6273  w_params_to_subs
+0000b160: 2870 6172 616d 7329 0a20 2020 2020 2020  (params).       
+0000b170: 2020 2020 2020 2020 206a 6f62 5f73 6372           job_scr
+0000b180: 6970 7420 3d20 7365 6c66 2e67 656e 6572  ipt = self.gener
+0000b190: 6174 655f 736c 7572 6d5f 6a6f 625f 666f  ate_slurm_job_fo
+0000b1a0: 725f 776f 726b 666c 6f77 2877 662c 2073  r_workflow(wf, s
+0000b1b0: 7562 7329 0a20 2020 2020 2020 2020 2020  ubs).           
+0000b1c0: 2020 2020 2023 2065 6e73 7572 6520 616c       # ensure al
+0000b1d0: 6c20 6469 7273 2065 7869 7374 2072 656d  l dirs exist rem
+0000b1e0: 6f74 656c 790a 2020 2020 2020 2020 2020  otely.          
+0000b1f0: 2020 2020 2020 6675 6c6c 5f70 6174 6820        full_path 
+0000b200: 3d20 7365 6c66 2e73 6c75 726d 5f73 6372  = self.slurm_scr
+0000b210: 6970 745f 7061 7468 2b22 2f22 2b6a 6f62  ipt_path+"/"+job
+0000b220: 5f70 6174 680a 2020 2020 2020 2020 2020  _path.          
+0000b230: 2020 2020 2020 6a6f 625f 6469 722c 205f        job_dir, _
+0000b240: 203d 206f 732e 7061 7468 2e73 706c 6974   = os.path.split
+0000b250: 2866 756c 6c5f 7061 7468 290a 2020 2020  (full_path).    
+0000b260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b270: 2e72 756e 2866 226d 6b64 6972 202d 7020  .run(f"mkdir -p 
+0000b280: 7b6a 6f62 5f64 6972 7d22 290a 2020 2020  {job_dir}").    
+0000b290: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+0000b2a0: 7079 2074 6f20 7265 6d6f 7465 2066 696c  py to remote fil
+0000b2b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000b2c0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+0000b2d0: 7075 7428 6c6f 6361 6c3d 696f 2e53 7472  put(local=io.Str
+0000b2e0: 696e 6749 4f28 6a6f 625f 7363 7269 7074  ingIO(job_script
+0000b2f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2020 2072 656d 6f74 653d 6675 6c6c       remote=full
+0000b320: 5f70 6174 6829 0a20 2020 2020 2020 2065  _path).        e
+0000b330: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000b340: 2063 6d64 203d 2073 656c 662e 6765 745f   cmd = self.get_
+0000b350: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
+0000b360: 6970 7473 5f63 6f6d 6d61 6e64 2829 0a20  ipts_command(). 
+0000b370: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000b380: 722e 696e 666f 2822 5570 6461 7469 6e67  r.info("Updating
+0000b390: 2053 6c75 726d 206a 6f62 2073 6372 6970   Slurm job scrip
+0000b3a0: 7473 206f 6e20 536c 7572 6d22 290a 2020  ts on Slurm").  
+0000b3b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000b3c0: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+0000b3d0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
+0000b3e0: 656e 7629 0a20 2020 2020 2020 2072 6574  env).        ret
+0000b3f0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0000b400: 6465 6620 7275 6e5f 776f 726b 666c 6f77  def run_workflow
+0000b410: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+0000b420: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000b430: 666c 6f77 5f6e 616d 653a 2073 7472 2c0a  flow_name: str,.
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2077 6f72 6b66 6c6f 775f 7665       workflow_ve
+0000b460: 7273 696f 6e3a 2073 7472 2c0a 2020 2020  rsion: str,.    
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2069 6e70 7574 5f64 6174 613a 2073 7472   input_data: str
+0000b490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b4a0: 2020 2020 2020 2065 6d61 696c 3a20 4f70         email: Op
+0000b4b0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000b4c0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000b4d0: 2020 2020 2020 2020 2074 696d 653a 204f           time: O
+0000b4e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000b4f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000b500: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000b510: 6773 0a20 2020 2020 2020 2020 2020 2020  gs.             
+0000b520: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
+0000b530: 6c65 5b52 6573 756c 742c 2069 6e74 5d3a  le[Result, int]:
+0000b540: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000b550: 2020 2020 2052 756e 2061 2073 7065 6369       Run a speci
+0000b560: 6669 6564 2077 6f72 6b66 6c6f 7720 6f6e  fied workflow on
+0000b570: 2053 6c75 726d 2075 7369 6e67 2074 6865   Slurm using the
+0000b580: 2067 6976 656e 2070 6172 616d 6574 6572   given parameter
+0000b590: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+0000b5a0: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
+0000b5b0: 726b 666c 6f77 5f6e 616d 6520 2873 7472  rkflow_name (str
+0000b5c0: 293a 204e 616d 6520 6f66 2074 6865 2077  ): Name of the w
+0000b5d0: 6f72 6b66 6c6f 7720 746f 2065 7865 6375  orkflow to execu
+0000b5e0: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
+0000b5f0: 776f 726b 666c 6f77 5f76 6572 7369 6f6e  workflow_version
+0000b600: 2028 7374 7229 3a20 5665 7273 696f 6e20   (str): Version 
+0000b610: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
+0000b620: 2869 6d61 6765 2076 6572 7369 6f6e 200a  (image version .
+0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b640: 6f6e 2053 6c75 726d 292e 0a20 2020 2020  on Slurm)..     
+0000b650: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+0000b660: 6120 2873 7472 293a 204e 616d 6520 6f66  a (str): Name of
+0000b670: 2074 6865 2069 6e70 7574 2064 6174 6120   the input data 
+0000b680: 666f 6c64 6572 2063 6f6e 7461 696e 696e  folder containin
+0000b690: 6720 696e 7075 740a 2020 2020 2020 2020  g input.        
+0000b6a0: 2020 2020 2020 2020 696d 6167 6520 6669          image fi
+0000b6b0: 6c65 732e 0a20 2020 2020 2020 2020 2020  les..           
+0000b6c0: 2065 6d61 696c 2028 7374 722c 206f 7074   email (str, opt
+0000b6d0: 696f 6e61 6c29 3a20 456d 6169 6c20 6164  ional): Email ad
+0000b6e0: 6472 6573 7320 666f 7220 536c 7572 6d20  dress for Slurm 
+0000b6f0: 6a6f 6220 6e6f 7469 6669 6361 7469 6f6e  job notification
+0000b700: 732e 0a20 2020 2020 2020 2020 2020 2074  s..            t
+0000b710: 696d 6520 2873 7472 2c20 6f70 7469 6f6e  ime (str, option
+0000b720: 616c 293a 2054 696d 6520 6c69 6d69 7420  al): Time limit 
+0000b730: 666f 7220 7468 6520 536c 7572 6d20 6a6f  for the Slurm jo
+0000b740: 6220 696e 2074 6865 200a 2020 2020 2020  b in the .      
+0000b750: 2020 2020 2020 2020 2020 666f 726d 6174            format
+0000b760: 2048 483a 4d4d 3a53 532e 0a20 2020 2020   HH:MM:SS..     
+0000b770: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+0000b780: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+0000b790: 6f72 6420 6172 6775 6d65 6e74 7320 666f  ord arguments fo
+0000b7a0: 7220 7468 6520 776f 726b 666c 6f77 2e0a  r the workflow..
+0000b7b0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000b7c0: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
+0000b7d0: 706c 655b 5265 7375 6c74 2c20 696e 745d  ple[Result, int]
+0000b7e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b7f0: 2020 4120 7475 706c 6520 636f 6e74 6169    A tuple contai
+0000b800: 6e69 6e67 2074 6865 2072 6573 756c 7420  ning the result 
+0000b810: 6f66 2073 7461 7274 696e 6720 7468 6520  of starting the 
+0000b820: 776f 726b 666c 6f77 206a 6f62 2061 6e64  workflow job and
+0000b830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b840: 2074 6865 2053 6c75 726d 206a 6f62 2049   the Slurm job I
+0000b850: 442c 206f 7220 2d31 2069 6620 7468 6520  D, or -1 if the 
+0000b860: 6a6f 6220 4944 2063 6f75 6c64 206e 6f74  job ID could not
+0000b870: 2062 6520 6578 7472 6163 7465 642e 0a0a   be extracted...
+0000b880: 2020 2020 2020 2020 4e6f 7465 3a0a 2020          Note:.  
+0000b890: 2020 2020 2020 2020 2020 5468 6520 536c            The Sl
+0000b8a0: 7572 6d20 6a6f 6220 4944 2069 7320 6578  urm job ID is ex
+0000b8b0: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
+0000b8c0: 2072 6573 756c 7420 6f66 2074 6865 200a   result of the .
+0000b8d0: 2020 2020 2020 2020 2020 2020 6072 756e              `run
+0000b8e0: 5f63 6f6d 6d61 6e64 7360 206d 6574 686f  _commands` metho
+0000b8f0: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
+0000b900: 2020 2020 2020 2073 6261 7463 685f 636d         sbatch_cm
+0000b910: 642c 2073 6261 7463 685f 656e 7620 3d20  d, sbatch_env = 
+0000b920: 7365 6c66 2e67 6574 5f77 6f72 6b66 6c6f  self.get_workflo
+0000b930: 775f 636f 6d6d 616e 6428 0a20 2020 2020  w_command(.     
+0000b940: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
+0000b950: 6e61 6d65 2c20 776f 726b 666c 6f77 5f76  name, workflow_v
+0000b960: 6572 7369 6f6e 2c20 696e 7075 745f 6461  ersion, input_da
+0000b970: 7461 2c20 656d 6169 6c2c 2074 696d 652c  ta, email, time,
+0000b980: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000b990: 2020 2070 7269 6e74 2866 2252 756e 6e69     print(f"Runni
+0000b9a0: 6e67 207b 776f 726b 666c 6f77 5f6e 616d  ng {workflow_nam
+0000b9b0: 657d 206a 6f62 206f 6e20 7b69 6e70 7574  e} job on {input
+0000b9c0: 5f64 6174 617d 206f 6e20 536c 7572 6d3a  _data} on Slurm:
+0000b9d0: 5c0a 2020 2020 2020 2020 2020 2020 7b73  \.            {s
+0000b9e0: 6261 7463 685f 636d 647d 2077 2f20 7b73  batch_cmd} w/ {s
+0000b9f0: 6261 7463 685f 656e 767d 2229 0a20 2020  batch_env}").   
+0000ba00: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000ba10: 2866 2252 756e 6e69 6e67 207b 776f 726b  (f"Running {work
+0000ba20: 666c 6f77 5f6e 616d 657d 206a 6f62 206f  flow_name} job o
+0000ba30: 6e20 7b69 6e70 7574 5f64 6174 617d 206f  n {input_data} o
+0000ba40: 6e20 536c 7572 6d22 290a 2020 2020 2020  n Slurm").      
+0000ba50: 2020 7265 7320 3d20 7365 6c66 2e72 756e    res = self.run
+0000ba60: 5f63 6f6d 6d61 6e64 7328 5b73 6261 7463  _commands([sbatc
+0000ba70: 685f 636d 645d 2c20 7362 6174 6368 5f65  h_cmd], sbatch_e
+0000ba80: 6e76 290a 2020 2020 2020 2020 7265 7475  nv).        retu
+0000ba90: 726e 2072 6573 2c20 7365 6c66 2e65 7874  rn res, self.ext
+0000baa0: 7261 6374 5f6a 6f62 5f69 6428 7265 7329  ract_job_id(res)
+0000bab0: 0a0a 2020 2020 6465 6620 7275 6e5f 776f  ..    def run_wo
+0000bac0: 726b 666c 6f77 5f6a 6f62 2873 656c 662c  rkflow_job(self,
+0000bad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bae0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000baf0: 6f77 5f6e 616d 653a 2073 7472 2c0a 2020  ow_name: str,.  
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
+0000bb20: 7665 7273 696f 6e3a 2073 7472 2c0a 2020  version: str,.  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+0000bb50: 613a 2073 7472 2c0a 2020 2020 2020 2020  a: str,.        
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2065 6d61 696c 3a20 4f70 7469 6f6e 616c   email: Optional
+0000bb80: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bba0: 2020 2020 2020 2074 696d 653a 204f 7074         time: Opt
+0000bbb0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000bbc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000bbd0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+0000bbe0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000bc00: 2d3e 2053 6c75 726d 4a6f 623a 0a20 2020  -> SlurmJob:.   
+0000bc10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000bc20: 2052 756e 2061 2073 7065 6369 6669 6564   Run a specified
+0000bc30: 2077 6f72 6b66 6c6f 7720 6f6e 2053 6c75   workflow on Slu
+0000bc40: 726d 2075 7369 6e67 2074 6865 2067 6976  rm using the giv
+0000bc50: 656e 2070 6172 616d 6574 6572 7320 616e  en parameters an
+0000bc60: 6420 7265 7475 726e 2061 2053 6c75 726d  d return a Slurm
+0000bc70: 4a6f 6220 696e 7374 616e 6365 2e0a 0a20  Job instance... 
+0000bc80: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000bc90: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000bca0: 775f 6e61 6d65 2028 7374 7229 3a20 4e61  w_name (str): Na
+0000bcb0: 6d65 206f 6620 7468 6520 776f 726b 666c  me of the workfl
+0000bcc0: 6f77 2074 6f20 6578 6563 7574 652e 0a20  ow to execute.. 
+0000bcd0: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000bce0: 6c6f 775f 7665 7273 696f 6e20 2873 7472  low_version (str
+0000bcf0: 293a 2056 6572 7369 6f6e 206f 6620 7468  ): Version of th
+0000bd00: 6520 776f 726b 666c 6f77 2028 696d 6167  e workflow (imag
+0000bd10: 6520 7665 7273 696f 6e20 6f6e 2053 6c75  e version on Slu
+0000bd20: 726d 292e 0a20 2020 2020 2020 2020 2020  rm)..           
+0000bd30: 2069 6e70 7574 5f64 6174 6120 2873 7472   input_data (str
+0000bd40: 293a 204e 616d 6520 6f66 2074 6865 2069  ): Name of the i
+0000bd50: 6e70 7574 2064 6174 6120 666f 6c64 6572  nput data folder
+0000bd60: 2063 6f6e 7461 696e 696e 6720 696e 7075   containing inpu
+0000bd70: 7420 696d 6167 6520 6669 6c65 732e 0a20  t image files.. 
+0000bd80: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+0000bd90: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+0000bda0: 3a20 456d 6169 6c20 6164 6472 6573 7320  : Email address 
+0000bdb0: 666f 7220 536c 7572 6d20 6a6f 6220 6e6f  for Slurm job no
+0000bdc0: 7469 6669 6361 7469 6f6e 732e 0a20 2020  tifications..   
+0000bdd0: 2020 2020 2020 2020 2074 696d 6520 2873           time (s
+0000bde0: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
+0000bdf0: 696d 6520 6c69 6d69 7420 666f 7220 7468  ime limit for th
+0000be00: 6520 536c 7572 6d20 6a6f 6220 696e 2074  e Slurm job in t
+0000be10: 6865 2066 6f72 6d61 7420 4848 3a4d 4d3a  he format HH:MM:
+0000be20: 5353 2e0a 2020 2020 2020 2020 2020 2020  SS..            
+0000be30: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
+0000be40: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+0000be50: 756d 656e 7473 2066 6f72 2074 6865 2077  uments for the w
+0000be60: 6f72 6b66 6c6f 772e 0a0a 2020 2020 2020  orkflow...      
+0000be70: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000be80: 2020 2020 2020 2053 6c75 726d 4a6f 623a         SlurmJob:
+0000be90: 2041 2053 6c75 726d 4a6f 6220 696e 7374   A SlurmJob inst
+0000bea0: 616e 6365 2072 6570 7265 7365 6e74 696e  ance representin
+0000beb0: 6720 7468 6520 7374 6172 7465 6420 776f  g the started wo
+0000bec0: 726b 666c 6f77 206a 6f62 2e0a 2020 2020  rkflow job..    
+0000bed0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000bee0: 7265 7375 6c74 2c20 6a6f 625f 6964 203d  result, job_id =
+0000bef0: 2073 656c 662e 7275 6e5f 776f 726b 666c   self.run_workfl
+0000bf00: 6f77 280a 2020 2020 2020 2020 2020 2020  ow(.            
+0000bf10: 776f 726b 666c 6f77 5f6e 616d 652c 2077  workflow_name, w
+0000bf20: 6f72 6b66 6c6f 775f 7665 7273 696f 6e2c  orkflow_version,
+0000bf30: 2069 6e70 7574 5f64 6174 612c 2065 6d61   input_data, ema
+0000bf40: 696c 2c20 7469 6d65 2c20 2a2a 6b77 6172  il, time, **kwar
+0000bf50: 6773 290a 2020 2020 2020 2020 7265 7475  gs).        retu
+0000bf60: 726e 2053 6c75 726d 4a6f 6228 7265 7375  rn SlurmJob(resu
+0000bf70: 6c74 2c20 6a6f 625f 6964 290a 0a20 2020  lt, job_id)..   
+0000bf80: 2064 6566 2072 756e 5f63 6f6e 7665 7273   def run_convers
+0000bf90: 696f 6e5f 776f 726b 666c 6f77 5f6a 6f62  ion_workflow_job
+0000bfa0: 2873 656c 662c 2066 6f6c 6465 725f 6e61  (self, folder_na
+0000bfb0: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+0000bfe0: 7263 655f 666f 726d 6174 3a20 7374 7220  rce_format: str 
+0000bff0: 3d20 277a 6172 7227 2c0a 2020 2020 2020  = 'zarr',.      
+0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c010: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0000c020: 7267 6574 5f66 6f72 6d61 743a 2073 7472  rget_format: str
+0000c030: 203d 2027 7469 6666 270a 2020 2020 2020   = 'tiff'.      
+0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000c060: 2d3e 2054 7570 6c65 5b52 6573 756c 742c  -> Tuple[Result,
+0000c070: 2069 6e74 5d3a 0a20 2020 2020 2020 2022   int]:.        "
+0000c080: 2222 0a20 2020 2020 2020 2052 756e 2074  "".        Run t
+0000c090: 6865 2064 6174 6120 636f 6e76 6572 7369  he data conversi
+0000c0a0: 6f6e 2077 6f72 6b66 6c6f 7720 6f6e 2053  on workflow on S
+0000c0b0: 6c75 726d 2075 7369 6e67 2074 6865 2067  lurm using the g
+0000c0c0: 6976 656e 2064 6174 6120 666f 6c64 6572  iven data folder
+0000c0d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000c0e0: 0a20 2020 2020 2020 2020 2020 2066 6f6c  .            fol
+0000c0f0: 6465 725f 6e61 6d65 2028 7374 7229 3a20  der_name (str): 
+0000c100: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0000c110: 6461 7461 2066 6f6c 6465 7220 636f 6e74  data folder cont
+0000c120: 6169 6e69 6e67 2073 6f75 7263 6520 666f  aining source fo
+0000c130: 726d 6174 2066 696c 6573 2e0a 2020 2020  rmat files..    
+0000c140: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
+0000c150: 6f72 6d61 7420 2873 7472 293a 2053 6f75  ormat (str): Sou
+0000c160: 7263 6520 6461 7461 2066 6f72 6d61 7420  rce data format 
+0000c170: 666f 7220 636f 6e76 6572 7369 6f6e 2028  for conversion (
+0000c180: 6465 6661 756c 7420 6973 2027 7a61 7272  default is 'zarr
+0000c190: 2729 2e0a 2020 2020 2020 2020 2020 2020  ')..            
+0000c1a0: 7461 7267 6574 5f66 6f72 6d61 7420 2873  target_format (s
+0000c1b0: 7472 293a 2054 6172 6765 7420 6461 7461  tr): Target data
+0000c1c0: 2066 6f72 6d61 7420 6166 7465 7220 636f   format after co
+0000c1d0: 6e76 6572 7369 6f6e 2028 6465 6661 756c  nversion (defaul
+0000c1e0: 7420 6973 2027 7469 6666 2729 2e0a 0a20  t is 'tiff')... 
+0000c1f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000c200: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+0000c210: 655b 5265 7375 6c74 2c20 696e 745d 3a0a  e[Result, int]:.
+0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c230: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+0000c240: 6e67 2074 6865 2072 6573 756c 7420 6f66  ng the result of
+0000c250: 2073 7461 7274 696e 6720 7468 6520 636f   starting the co
+0000c260: 6e76 6572 7369 6f6e 206a 6f62 2061 6e64  nversion job and
+0000c270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c280: 2074 6865 2053 6c75 726d 206a 6f62 2049   the Slurm job I
+0000c290: 442c 206f 7220 2d31 2069 6620 7468 6520  D, or -1 if the 
+0000c2a0: 6a6f 6220 4944 2063 6f75 6c64 206e 6f74  job ID could not
+0000c2b0: 2062 6520 6578 7472 6163 7465 642e 0a0a   be extracted...
+0000c2c0: 2020 2020 2020 2020 5761 726e 696e 673a          Warning:
+0000c2d0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000c2e0: 2064 6566 6175 6c74 2069 6d70 6c65 6d65   default impleme
+0000c2f0: 6e74 6174 696f 6e20 6f6e 6c79 2073 7570  ntation only sup
+0000c300: 706f 7274 7320 636f 6e76 6572 7369 6f6e  ports conversion
+0000c310: 2066 726f 6d20 277a 6172 7227 2074 6f20   from 'zarr' to 
+0000c320: 2774 6966 6627 2e0a 2020 2020 2020 2020  'tiff'..        
+0000c330: 2020 2020 4966 2075 7369 6e67 206f 7468      If using oth
+0000c340: 6572 2073 6f75 7263 6520 6f72 2074 6172  er source or tar
+0000c350: 6765 7420 666f 726d 6174 732c 2075 7365  get formats, use
+0000c360: 7273 206d 7573 7420 696d 706c 656d 656e  rs must implemen
+0000c370: 7420 616e 6420 636f 6e66 6967 7572 650a  t and configure.
+0000c380: 2020 2020 2020 2020 2020 2020 6164 6469              addi
+0000c390: 7469 6f6e 616c 2063 6f6e 7665 7274 6572  tional converter
+0000c3a0: 7320 7468 656d 7365 6c76 6573 2e0a 2020  s themselves..  
+0000c3b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c3c0: 2020 2320 4765 6e65 7261 7465 2061 2075    # Generate a u
+0000c3d0: 6e69 7175 6520 636f 6e66 6967 2066 696c  nique config fil
+0000c3e0: 6520 6e61 6d65 0a20 2020 2020 2020 2063  e name.        c
+0000c3f0: 6f6e 6669 675f 6669 6c65 203d 2066 2263  onfig_file = f"c
+0000c400: 6f6e 6669 675f 7b66 6f6c 6465 725f 6e61  onfig_{folder_na
+0000c410: 6d65 7d2e 7478 7422 0a0a 2020 2020 2020  me}.txt"..      
+0000c420: 2020 2320 436f 6e73 7472 7563 7420 616c    # Construct al
+0000c430: 6c20 636f 6d6d 616e 6473 2074 6f20 7275  l commands to ru
+0000c440: 6e20 636f 6e73 6563 7574 6976 656c 790a  n consecutively.
+0000c450: 2020 2020 2020 2020 6461 7461 5f70 6174          data_pat
+0000c460: 6820 3d20 6622 7b73 656c 662e 736c 7572  h = f"{self.slur
+0000c470: 6d5f 6461 7461 5f70 6174 687d 2f7b 666f  m_data_path}/{fo
+0000c480: 6c64 6572 5f6e 616d 657d 220a 2020 2020  lder_name}".    
+0000c490: 2020 2020 636f 6e76 6572 7369 6f6e 5f63      conversion_c
+0000c4a0: 6d64 2c20 7362 6174 6368 5f65 6e76 203d  md, sbatch_env =
+0000c4b0: 2073 656c 662e 6765 745f 636f 6e76 6572   self.get_conver
+0000c4c0: 7369 6f6e 5f63 6f6d 6d61 6e64 280a 2020  sion_command(.  
+0000c4d0: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
+0000c4e0: 6174 682c 2063 6f6e 6669 675f 6669 6c65  ath, config_file
+0000c4f0: 2c20 736f 7572 6365 5f66 6f72 6d61 742c  , source_format,
+0000c500: 2074 6172 6765 745f 666f 726d 6174 290a   target_format).
+0000c510: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
+0000c520: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+0000c530: 2066 2266 696e 6420 7b64 6174 615f 7061   f"find {data_pa
+0000c540: 7468 7d2f 6461 7461 2f69 6e20 2d6e 616d  th}/data/in -nam
+0000c550: 6520 272a 2e7b 736f 7572 6365 5f66 6f72  e '*.{source_for
+0000c560: 6d61 747d 2720 7c20 6177 6b20 277b 7b70  mat}' | awk '{{p
+0000c570: 7269 6e74 204e 522c 2024 307d 7d27 203e  rint NR, $0}}' >
+0000c580: 207b 636f 6e66 6967 5f66 696c 657d 222c   {config_file}",
+0000c590: 0a20 2020 2020 2020 2020 2020 2066 224e  .            f"N
+0000c5a0: 3d24 2877 6320 2d6c 203c 205c 227b 636f  =$(wc -l < \"{co
+0000c5b0: 6e66 6967 5f66 696c 657d 5c22 2922 2c0a  nfig_file}\")",.
+0000c5c0: 2020 2020 2020 2020 2020 2020 6622 6563              f"ec
+0000c5d0: 686f 205c 224e 756d 6265 7220 6f66 202e  ho \"Number of .
+0000c5e0: 7b73 6f75 7263 655f 666f 726d 6174 7d20  {source_format} 
+0000c5f0: 6669 6c65 733a 2024 4e5c 2222 2c0a 2020  files: $N\"",.  
+0000c600: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
+0000c610: 7369 6f6e 5f63 6d64 0a20 2020 2020 2020  sion_cmd.       
+0000c620: 205d 0a0a 2020 2020 2020 2020 2320 5275   ]..        # Ru
+0000c630: 6e20 616c 6c20 636f 6d6d 616e 6473 2063  n all commands c
+0000c640: 6f6e 7365 6375 7469 7665 6c79 0a20 2020  onsecutively.   
+0000c650: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+0000c660: 7275 6e5f 636f 6d6d 616e 6473 2863 6f6d  run_commands(com
+0000c670: 6d61 6e64 732c 2073 6261 7463 685f 656e  mands, sbatch_en
+0000c680: 7629 0a0a 2020 2020 2020 2020 7265 7475  v)..        retu
+0000c690: 726e 2053 6c75 726d 4a6f 6228 7265 732c  rn SlurmJob(res,
+0000c6a0: 2073 656c 662e 6578 7472 6163 745f 6a6f   self.extract_jo
+0000c6b0: 625f 6964 2872 6573 2929 0a0a 2020 2020  b_id(res))..    
+0000c6c0: 6465 6620 6578 7472 6163 745f 6a6f 625f  def extract_job_
+0000c6d0: 6964 2873 656c 662c 2072 6573 756c 743a  id(self, result:
+0000c6e0: 2052 6573 756c 7429 202d 3e20 696e 743a   Result) -> int:
+0000c6f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c700: 2020 2020 2045 7874 7261 6374 2074 6865       Extract the
+0000c710: 2053 6c75 726d 206a 6f62 2049 4420 6672   Slurm job ID fr
+0000c720: 6f6d 2074 6865 2072 6573 756c 7420 6f66  om the result of
+0000c730: 2061 2063 6f6d 6d61 6e64 2e0a 0a20 2020   a command...   
+0000c740: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000c750: 2020 2020 2020 2072 6573 756c 7420 2852         result (R
+0000c760: 6573 756c 7429 3a20 5468 6520 7265 7375  esult): The resu
+0000c770: 6c74 206f 6620 6120 636f 6d6d 616e 6420  lt of a command 
+0000c780: 6578 6563 7574 696f 6e2e 0a0a 2020 2020  execution...    
+0000c790: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000c7a0: 2020 2020 2020 2020 2069 6e74 3a0a 2020           int:.  
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+0000c7c0: 6520 536c 7572 6d20 6a6f 6220 4944 2065  e Slurm job ID e
+0000c7d0: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
+0000c7e0: 6520 7265 7375 6c74 2c0a 2020 2020 2020  e result,.      
+0000c7f0: 2020 2020 2020 2020 2020 6f72 202d 3120            or -1 
+0000c800: 6966 206e 6f74 2066 6f75 6e64 2e0a 2020  if not found..  
+0000c810: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c820: 2020 736c 7572 6d5f 6a6f 625f 6964 203d    slurm_job_id =
+0000c830: 206e 6578 7428 2869 6e74 2873 2e73 7472   next((int(s.str
+0000c840: 6970 2829 2920 666f 7220 7320 696e 2072  ip()) for s in r
+0000c850: 6573 756c 742e 7374 646f 7574 2e73 706c  esult.stdout.spl
+0000c860: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
+0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c880: 2253 7562 6d69 7474 6564 2062 6174 6368  "Submitted batch
+0000c890: 206a 6f62 2229 2069 6620 732e 7374 7269   job") if s.stri
+0000c8a0: 7028 292e 6973 6469 6769 7428 2929 2c20  p().isdigit()), 
+0000c8b0: 2d31 290a 2020 2020 2020 2020 7265 7475  -1).        retu
+0000c8c0: 726e 2073 6c75 726d 5f6a 6f62 5f69 640a  rn slurm_job_id.
+0000c8d0: 0a20 2020 2064 6566 2067 6574 5f75 7064  .    def get_upd
+0000c8e0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
+0000c8f0: 735f 636f 6d6d 616e 6428 7365 6c66 2920  s_command(self) 
+0000c900: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0000c910: 2222 2247 656e 6572 6174 6520 7468 6520  """Generate the 
+0000c920: 636f 6d6d 616e 6420 746f 2075 7064 6174  command to updat
+0000c930: 6520 7468 6520 4769 7420 7265 706f 7369  e the Git reposi
+0000c940: 746f 7279 2063 6f6e 7461 696e 696e 670a  tory containing.
+0000c950: 2020 2020 2020 2020 7468 6520 536c 7572          the Slur
+0000c960: 6d20 7363 7269 7074 732c 2069 6620 6e65  m scripts, if ne
+0000c970: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
+0000c980: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000c990: 2020 2020 2020 2073 7472 3a0a 2020 2020         str:.    
+0000c9a0: 2020 2020 2020 2020 2020 2020 4120 7374              A st
+0000c9b0: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
+0000c9c0: 7468 6520 4769 7420 636f 6d6d 616e 640a  the Git command.
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9e0: 746f 2075 7064 6174 6520 7468 6520 536c  to update the Sl
+0000c9f0: 7572 6d20 7363 7269 7074 732e 0a20 2020  urm scripts..   
+0000ca00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ca10: 2075 7064 6174 655f 636d 6420 3d20 6622   update_cmd = f"
+0000ca20: 6769 7420 2d43 207b 7365 6c66 2e73 6c75  git -C {self.slu
+0000ca30: 726d 5f73 6372 6970 745f 7061 7468 7d20  rm_script_path} 
+0000ca40: 7075 6c6c 220a 2020 2020 2020 2020 7265  pull".        re
+0000ca50: 7475 726e 2075 7064 6174 655f 636d 640a  turn update_cmd.
+0000ca60: 0a20 2020 2064 6566 2063 6865 636b 5f6a  .    def check_j
+0000ca70: 6f62 5f73 7461 7475 7328 7365 6c66 2c0a  ob_status(self,.
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
+0000caa0: 6f62 5f69 6473 3a20 4c69 7374 5b69 6e74  ob_ids: List[int
+0000cab0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000cac0: 2020 2020 2020 2020 2020 2020 656e 763a              env:
+0000cad0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+0000cae0: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
+0000caf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb00: 2020 2020 2020 2020 2020 2920 2d3e 2054            ) -> T
+0000cb10: 7570 6c65 5b44 6963 745b 696e 742c 2073  uple[Dict[int, s
+0000cb20: 7472 5d2c 2052 6573 756c 745d 3a0a 2020  tr], Result]:.  
+0000cb30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000cb40: 2020 4368 6563 6b20 7468 6520 7374 6174    Check the stat
+0000cb50: 7573 206f 6620 536c 7572 6d20 6a6f 6273  us of Slurm jobs
+0000cb60: 2077 6974 6820 7468 6520 6769 7665 6e20   with the given 
+0000cb70: 6a6f 6220 4944 732e 0a0a 2020 2020 2020  job IDs...      
+0000cb80: 2020 4e6f 7465 3a20 5468 6973 2064 6f65    Note: This doe
+0000cb90: 736e 2774 2072 6574 7572 6e20 6a6f 6220  sn't return job 
+0000cba0: 6172 7261 7973 2069 6e64 6976 6964 7561  arrays individua
+0000cbb0: 6c6c 792e 0a20 2020 2020 2020 2049 7420  lly..        It 
+0000cbc0: 7461 6b65 7320 7468 6520 6c61 7374 2076  takes the last v
+0000cbd0: 616c 7565 2072 6574 7572 6e65 6420 666f  alue returned fo
+0000cbe0: 7220 7468 6f73 6520 7375 6220 6964 7320  r those sub ids 
+0000cbf0: 0a20 2020 2020 2020 2028 6765 6e65 7261  .        (genera
+0000cc00: 6c6c 7920 7468 6520 6f6e 6520 7374 696c  lly the one stil
+0000cc10: 6c20 5045 4e44 494e 4729 2e0a 0a20 2020  l PENDING)...   
+0000cc20: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000cc30: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
+0000cc40: 5f69 6473 2028 4c69 7374 5b69 6e74 5d29  _ids (List[int])
+0000cc50: 3a20 5468 6520 6a6f 6220 4944 7320 6f66  : The job IDs of
+0000cc60: 2074 6865 2053 6c75 726d 206a 6f62 7320   the Slurm jobs 
+0000cc70: 746f 2063 6865 636b 2e0a 2020 2020 2020  to check..      
+0000cc80: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+0000cc90: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+0000cca0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+0000ccb0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+0000ccc0: 626c 6573 2074 6f0a 2020 2020 2020 2020  bles to.        
+0000ccd0: 2020 2020 2020 2020 7365 7420 7768 656e          set when
+0000cce0: 2072 756e 6e69 6e67 2074 6865 2063 6f6d   running the com
+0000ccf0: 6d61 6e64 2e20 4465 6661 756c 7473 2074  mand. Defaults t
+0000cd00: 6f20 4e6f 6e65 2e0a 0a20 2020 2020 2020  o None...       
+0000cd10: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000cd20: 2020 2020 2020 5475 706c 655b 4469 6374        Tuple[Dict
+0000cd30: 5b69 6e74 2c20 7374 725d 2c20 5265 7375  [int, str], Resu
+0000cd40: 6c74 5d3a 0a20 2020 2020 2020 2020 2020  lt]:.           
+0000cd50: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
+0000cd60: 7461 696e 696e 6720 7468 6520 7374 6174  taining the stat
+0000cd70: 7573 2070 6572 2069 6e70 7574 2049 4420  us per input ID 
+0000cd80: 616e 6420 7468 6520 7265 7375 6c74 206f  and the result o
+0000cd90: 6620 0a20 2020 2020 2020 2020 2020 2020  f .             
+0000cda0: 2020 2074 6865 2063 6f6d 6d61 6e64 2065     the command e
+0000cdb0: 7865 6375 7469 6f6e 2e0a 0a20 2020 2020  xecution...     
+0000cdc0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+0000cdd0: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
+0000cde0: 696f 6e3a 2049 6620 7468 6520 636f 6d6d  ion: If the comm
+0000cdf0: 616e 6420 6578 6563 7574 696f 6e20 6661  and execution fa
+0000ce00: 696c 7320 6f72 206e 6f20 7265 7370 6f6e  ils or no respon
+0000ce10: 7365 2069 730a 2020 2020 2020 2020 2020  se is.          
+0000ce20: 2020 2020 2020 7265 6365 6976 6564 2061        received a
+0000ce30: 6674 6572 206d 756c 7469 706c 6520 7265  fter multiple re
+0000ce40: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
+0000ce50: 2222 0a20 2020 2020 2020 2063 6d64 203d  "".        cmd =
+0000ce60: 2073 656c 662e 6765 745f 6a6f 625f 7374   self.get_job_st
+0000ce70: 6174 7573 5f63 6f6d 6d61 6e64 2873 6c75  atus_command(slu
+0000ce80: 726d 5f6a 6f62 5f69 6473 290a 2020 2020  rm_job_ids).    
+0000ce90: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0000cea0: 6622 4765 7474 696e 6720 7374 6174 7573  f"Getting status
+0000ceb0: 206f 6620 7b73 6c75 726d 5f6a 6f62 5f69   of {slurm_job_i
+0000cec0: 6473 7d20 6f6e 2053 6c75 726d 2229 0a20  ds} on Slurm"). 
+0000ced0: 2020 2020 2020 2072 6574 7279 5f73 7461         retry_sta
+0000cee0: 7475 7320 3d20 300a 2020 2020 2020 2020  tus = 0.        
+0000cef0: 7768 696c 6520 7265 7472 795f 7374 6174  while retry_stat
+0000cf00: 7573 203c 2033 3a0a 2020 2020 2020 2020  us < 3:.        
+0000cf10: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+0000cf20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
+0000cf30: 636d 645d 2c20 656e 763d 656e 7629 0a20  cmd], env=env). 
+0000cf40: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000cf50: 722e 696e 666f 2872 6573 756c 7429 0a20  r.info(result). 
+0000cf60: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0000cf70: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
+0000cf80: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000cf90: 7265 7375 6c74 2e73 7464 6f75 743a 0a20  result.stdout:. 
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2023 2077 6169 7420 666f 7220 3320     # wait for 3 
+0000cfc0: 7365 636f 6e64 7320 6265 666f 7265 2063  seconds before c
+0000cfd0: 6865 636b 696e 6720 6167 6169 6e0a 2020  hecking again.  
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 7469 6d65 736c 6565 702e 736c 6565    timesleep.slee
+0000d000: 7028 3329 0a20 2020 2020 2020 2020 2020  p(3).           
+0000d010: 2020 2020 2020 2020 2023 2072 6574 7279           # retry
+0000d020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d030: 2020 2020 2072 6574 7279 5f73 7461 7475       retry_statu
+0000d040: 7320 2b3d 2031 0a20 2020 2020 2020 2020  s += 1.         
+0000d050: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000d060: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2066 2252 6574 7279 207b 7265 7472 795f   f"Retry {retry_
+0000d090: 7374 6174 7573 7d20 6765 7474 696e 6720  status} getting 
+0000d0a0: 7374 6174 7573 205c 0a20 2020 2020 2020  status \.       
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 206f 6620 7b73 6c75 726d 5f6a       of {slurm_j
+0000d0d0: 6f62 5f69 6473 7d21 2229 0a20 2020 2020  ob_ids}!").     
+0000d0e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000d0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d100: 2020 2020 2023 0a20 2020 2020 2020 2020       #.         
+0000d110: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
+0000d120: 7461 7475 735f 6469 6374 203d 207b 696e  tatus_dict = {in
+0000d130: 7428 6c69 6e65 2e73 706c 6974 2829 5b30  t(line.split()[0
+0000d140: 5d2e 7370 6c69 7428 275f 2729 5b30 5d29  ].split('_')[0])
+0000d150: 3a20 6c69 6e65 2e73 706c 6974 280a 2020  : line.split(.  
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2020 295b 315d 2066 6f72 206c 696e 6520    )[1] for line 
+0000d180: 696e 2072 6573 756c 742e 7374 646f 7574  in result.stdout
+0000d190: 2e73 706c 6974 2822 5c6e 2229 2069 6620  .split("\n") if 
+0000d1a0: 6c69 6e65 7d0a 2020 2020 2020 2020 2020  line}.          
+0000d1b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000d1c0: 2e64 6562 7567 2866 224a 6f62 2073 7461  .debug(f"Job sta
+0000d1d0: 7475 7365 733a 207b 6a6f 625f 7374 6174  tuses: {job_stat
+0000d1e0: 7573 5f64 6963 747d 2229 0a20 2020 2020  us_dict}").     
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d200: 6574 7572 6e20 6a6f 625f 7374 6174 7573  eturn job_status
+0000d210: 5f64 6963 742c 2072 6573 756c 740a 2020  _dict, result.  
+0000d220: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 6572 726f 7220 3d20 6622 5265 7375 6c74  error = f"Result
+0000d250: 2069 7320 6e6f 7420 6f6b 3a20 7b72 6573   is not ok: {res
+0000d260: 756c 747d 220a 2020 2020 2020 2020 2020  ult}".          
+0000d270: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+0000d280: 6f72 2865 7272 6f72 290a 2020 2020 2020  or(error).      
+0000d290: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d2a0: 5353 4845 7863 6570 7469 6f6e 2865 7272  SSHException(err
+0000d2b0: 6f72 290a 2020 2020 2020 2020 656c 7365  or).        else
+0000d2c0: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
+0000d2d0: 726f 7220 3d20 6622 4572 726f 723a 2052  ror = f"Error: R
+0000d2e0: 6574 7269 6564 207b 7265 7472 795f 7374  etried {retry_st
+0000d2f0: 6174 7573 7d20 7469 6d65 7320 746f 2067  atus} times to g
+0000d300: 6574 205c 0a20 2020 2020 2020 2020 2020  et \.           
+0000d310: 2020 2020 2073 7461 7475 7320 6f66 207b       status of {
+0000d320: 736c 7572 6d5f 6a6f 625f 6964 737d 2c20  slurm_job_ids}, 
+0000d330: 6275 7420 6e6f 2072 6573 706f 6e73 652e  but no response.
+0000d340: 220a 2020 2020 2020 2020 2020 2020 6c6f  ".            lo
+0000d350: 6767 6572 2e65 7272 6f72 2865 7272 6f72  gger.error(error
+0000d360: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+0000d370: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
+0000d380: 2865 7272 6f72 290a 0a20 2020 2064 6566  (error)..    def
+0000d390: 2067 6574 5f6a 6f62 5f73 7461 7475 735f   get_job_status_
+0000d3a0: 636f 6d6d 616e 6428 7365 6c66 2c20 736c  command(self, sl
+0000d3b0: 7572 6d5f 6a6f 625f 6964 733a 204c 6973  urm_job_ids: Lis
+0000d3c0: 745b 696e 745d 2920 2d3e 2073 7472 3a0a  t[int]) -> str:.
+0000d3d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d3e0: 2020 2020 5265 7475 726e 2074 6865 2053      Return the S
+0000d3f0: 6c75 726d 2063 6f6d 6d61 6e64 2074 6f20  lurm command to 
+0000d400: 6765 7420 7468 6520 7374 6174 7573 206f  get the status o
+0000d410: 6620 6a6f 6273 2077 6974 6820 7468 6520  f jobs with the 
+0000d420: 6769 7665 6e0a 2020 2020 2020 2020 6a6f  given.        jo
+0000d430: 6220 4944 732e 0a0a 2020 2020 2020 2020  b IDs...        
+0000d440: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000d450: 2020 736c 7572 6d5f 6a6f 625f 6964 7320    slurm_job_ids 
+0000d460: 284c 6973 745b 696e 745d 293a 2054 6865  (List[int]): The
+0000d470: 206a 6f62 2049 4473 206f 6620 7468 6520   job IDs of the 
+0000d480: 6a6f 6273 2074 6f20 6368 6563 6b2e 0a0a  jobs to check...
+0000d490: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000d4a0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000d4b0: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
+0000d4c0: 2020 2054 6865 2053 6c75 726d 2063 6f6d     The Slurm com
+0000d4d0: 6d61 6e64 2074 6f20 6765 7420 7468 6520  mand to get the 
+0000d4e0: 7374 6174 7573 206f 6620 7468 6520 6a6f  status of the jo
+0000d4f0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
+0000d500: 2020 2020 2020 2020 2320 636f 6e63 6174          # concat
+0000d510: 206d 756c 7469 706c 6520 6a6f 6273 2069   multiple jobs i
+0000d520: 6620 6e65 6564 6564 0a20 2020 2020 2020  f needed.       
+0000d530: 2073 6c75 726d 5f6a 6f62 5f69 6420 3d20   slurm_job_id = 
+0000d540: 2220 2d6a 2022 2e6a 6f69 6e28 5b73 7472  " -j ".join([str
+0000d550: 2869 6429 2066 6f72 2069 6420 696e 2073  (id) for id in s
+0000d560: 6c75 726d 5f6a 6f62 5f69 6473 5d29 0a20  lurm_job_ids]). 
+0000d570: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000d580: 6c66 2e5f 4a4f 425f 5354 4154 5553 5f43  lf._JOB_STATUS_C
+0000d590: 4d44 2e66 6f72 6d61 7428 736c 7572 6d5f  MD.format(slurm_
+0000d5a0: 6a6f 625f 6964 3d73 6c75 726d 5f6a 6f62  job_id=slurm_job
+0000d5b0: 5f69 6429 0a0a 2020 2020 6465 6620 6578  _id)..    def ex
+0000d5c0: 7472 6163 745f 6461 7461 5f6c 6f63 6174  tract_data_locat
+0000d5d0: 696f 6e5f 6672 6f6d 5f6c 6f67 2873 656c  ion_from_log(sel
+0000d5e0: 662c 2073 6c75 726d 5f6a 6f62 5f69 643a  f, slurm_job_id:
+0000d5f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d620: 2020 2020 6c6f 6766 696c 653a 2073 7472      logfile: str
+0000d630: 203d 204e 6f6e 6529 202d 3e20 7374 723a   = None) -> str:
+0000d640: 0a20 2020 2020 2020 2022 2222 5265 6164  .        """Read
+0000d650: 2053 4c55 524d 206a 6f62 206c 6f67 6669   SLURM job logfi
+0000d660: 6c65 2074 6f20 6669 6e64 206c 6f63 6174  le to find locat
+0000d670: 696f 6e20 6f66 2074 6865 2064 6174 612e  ion of the data.
+0000d680: 0a0a 2020 2020 2020 2020 4f6e 6520 6f66  ..        One of
+0000d690: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+0000d6a0: 6973 2072 6571 7569 7265 642c 2065 6974  is required, eit
+0000d6b0: 6865 7220 6964 206f 7220 6669 6c65 2e0a  her id or file..
+0000d6c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000d6d0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+0000d6e0: 5f6a 6f62 5f69 6420 2873 7472 293a 2049  _job_id (str): I
+0000d6f0: 6420 6f66 2074 6865 2073 6c75 726d 206a  d of the slurm j
+0000d700: 6f62 0a20 2020 2020 2020 2020 2020 206c  ob.            l
+0000d710: 6f67 6669 6c65 2028 7374 7229 3a20 5061  ogfile (str): Pa
+0000d720: 7468 2074 6f20 7468 6520 6c6f 6766 696c  th to the logfil
+0000d730: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+0000d740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000d750: 7374 723a 2044 6174 6120 6c6f 6361 7469  str: Data locati
+0000d760: 6f6e 2061 6363 6f72 6469 6e67 2074 6f20  on according to 
+0000d770: 7468 6520 6c6f 670a 0a20 2020 2020 2020  the log..       
+0000d780: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+0000d790: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
+0000d7a0: 6e3a 2049 6620 7468 6572 6520 6973 2061  n: If there is a
+0000d7b0: 6e20 6973 7375 6520 7769 7468 2074 6865  n issue with the
+0000d7c0: 2063 6f6d 6d61 6e64 2065 7865 6375 7469   command executi
+0000d7d0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+0000d7e0: 2020 2020 2020 2020 6966 206c 6f67 6669          if logfi
+0000d7f0: 6c65 2069 7320 4e6f 6e65 2061 6e64 2073  le is None and s
+0000d800: 6c75 726d 5f6a 6f62 5f69 6420 6973 206e  lurm_job_id is n
+0000d810: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000d820: 2020 2020 206c 6f67 6669 6c65 203d 2073       logfile = s
+0000d830: 656c 662e 5f4c 4f47 4649 4c45 0a20 2020  elf._LOGFILE.   
+0000d840: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+0000d850: 203d 206c 6f67 6669 6c65 2e66 6f72 6d61   = logfile.forma
+0000d860: 7428 736c 7572 6d5f 6a6f 625f 6964 3d73  t(slurm_job_id=s
+0000d870: 6c75 726d 5f6a 6f62 5f69 6429 0a20 2020  lurm_job_id).   
+0000d880: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
+0000d890: 5f4c 4f47 4649 4c45 5f44 4154 415f 434d  _LOGFILE_DATA_CM
+0000d8a0: 442e 666f 726d 6174 286c 6f67 5f66 696c  D.format(log_fil
+0000d8b0: 653d 6c6f 6766 696c 6529 0a20 2020 2020  e=logfile).     
+0000d8c0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0000d8d0: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
+0000d8e0: 6d64 5d29 0a20 2020 2020 2020 2069 6620  md]).        if 
+0000d8f0: 7265 7375 6c74 2e6f 6b3a 0a20 2020 2020  result.ok:.     
+0000d900: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000d910: 7375 6c74 2e73 7464 6f75 740a 2020 2020  sult.stdout.    
+0000d920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d930: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+0000d940: 7863 6570 7469 6f6e 2872 6573 756c 7429  xception(result)
+0000d950: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
+0000d960: 726b 666c 6f77 5f70 6172 616d 6574 6572  rkflow_parameter
+0000d970: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d990: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000d9a0: 3a20 7374 7229 202d 3e20 4469 6374 5b73  : str) -> Dict[s
+0000d9b0: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
+0000d9c0: 795d 5d3a 0a20 2020 2020 2020 2022 2222  y]]:.        """
+0000d9d0: 0a20 2020 2020 2020 2052 6574 7269 6576  .        Retriev
+0000d9e0: 6520 7468 6520 7061 7261 6d65 7465 7273  e the parameters
+0000d9f0: 206f 6620 6120 776f 726b 666c 6f77 2e0a   of a workflow..
+0000da00: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000da10: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000da20: 6c6f 7720 2873 7472 293a 2054 6865 2077  low (str): The w
+0000da30: 6f72 6b66 6c6f 7720 666f 7220 7768 6963  orkflow for whic
+0000da40: 6820 746f 2072 6574 7269 6576 6520 7468  h to retrieve th
+0000da50: 6520 7061 7261 6d65 7465 7273 2e0a 0a20  e parameters... 
+0000da60: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000da70: 2020 2020 2020 2020 2020 2020 4469 6374              Dict
+0000da80: 5b73 7472 2c20 4469 6374 5b73 7472 2c20  [str, Dict[str, 
+0000da90: 416e 795d 5d3a 0a20 2020 2020 2020 2020  Any]]:.         
+0000daa0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
+0000dab0: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+0000dac0: 6865 2077 6f72 6b66 6c6f 7720 7061 7261  he workflow para
+0000dad0: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
+0000dae0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+0000daf0: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
+0000db00: 2049 6620 616e 2065 7272 6f72 206f 6363   If an error occ
+0000db10: 7572 7320 7768 696c 6520 7265 7472 6965  urs while retrie
+0000db20: 7669 6e67 2074 6865 2077 6f72 6b66 6c6f  ving the workflo
+0000db30: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+0000db40: 2020 7061 7261 6d65 7465 7273 2e0a 2020    parameters..  
+0000db50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000db60: 2020 6a73 6f6e 5f64 6573 6372 6970 746f    json_descripto
+0000db70: 7220 3d20 7365 6c66 2e70 756c 6c5f 6465  r = self.pull_de
+0000db80: 7363 7269 7074 6f72 5f66 726f 6d5f 6769  scriptor_from_gi
+0000db90: 7468 7562 2877 6f72 6b66 6c6f 7729 0a20  thub(workflow). 
+0000dba0: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
+0000dbb0: 2074 6f20 6f6d 6572 6f20 7479 7065 730a   to omero types.
+0000dbc0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000dbd0: 6562 7567 286a 736f 6e5f 6465 7363 7269  ebug(json_descri
+0000dbe0: 7074 6f72 290a 2020 2020 2020 2020 776f  ptor).        wo
+0000dbf0: 726b 666c 6f77 5f64 6963 7420 3d20 7b7d  rkflow_dict = {}
+0000dc00: 0a20 2020 2020 2020 2066 6f72 2069 6e70  .        for inp
+0000dc10: 7574 2069 6e20 6a73 6f6e 5f64 6573 6372  ut in json_descr
+0000dc20: 6970 746f 725b 2769 6e70 7574 7327 5d3a  iptor['inputs']:
+0000dc30: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
+0000dc40: 696c 7465 7220 6379 746f 6d69 6e65 2070  ilter cytomine p
+0000dc50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000dc60: 2020 2020 2020 6966 206e 6f74 2069 6e70        if not inp
+0000dc70: 7574 5b27 6964 275d 2e73 7461 7274 7377  ut['id'].startsw
+0000dc80: 6974 6828 2763 7974 6f6d 696e 6527 293a  ith('cytomine'):
+0000dc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dca0: 2077 6f72 6b66 6c6f 775f 7061 7261 6d73   workflow_params
+0000dcb0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+0000dcc0: 2020 2020 2020 776f 726b 666c 6f77 5f70        workflow_p
+0000dcd0: 6172 616d 735b 276e 616d 6527 5d20 3d20  arams['name'] = 
+0000dce0: 696e 7075 745b 2769 6427 5d0a 2020 2020  input['id'].    
+0000dcf0: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000dd00: 666c 6f77 5f70 6172 616d 735b 2764 6566  flow_params['def
+0000dd10: 6175 6c74 275d 203d 2069 6e70 7574 5b27  ault'] = input['
+0000dd20: 6465 6661 756c 742d 7661 6c75 6527 5d0a  default-value'].
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
+0000dd50: 2763 7974 7970 6527 5d20 3d20 696e 7075  'cytype'] = inpu
+0000dd60: 745b 2774 7970 6527 5d0a 2020 2020 2020  t['type'].      
+0000dd70: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000dd80: 6f77 5f70 6172 616d 735b 276f 7074 696f  ow_params['optio
+0000dd90: 6e61 6c27 5d20 3d20 696e 7075 745b 276f  nal'] = input['o
+0000dda0: 7074 696f 6e61 6c27 5d0a 2020 2020 2020  ptional'].      
+0000ddb0: 2020 2020 2020 2020 2020 636d 645f 666c            cmd_fl
+0000ddc0: 6167 203d 2069 6e70 7574 5b27 636f 6d6d  ag = input['comm
+0000ddd0: 616e 642d 6c69 6e65 2d66 6c61 6727 5d0a  and-line-flag'].
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddf0: 636d 645f 666c 6167 203d 2063 6d64 5f66  cmd_flag = cmd_f
+0000de00: 6c61 672e 7265 706c 6163 6528 2240 6964  lag.replace("@id
+0000de10: 222c 2069 6e70 7574 5b27 6964 275d 290a  ", input['id']).
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
+0000de40: 2763 6d64 5f66 6c61 6727 5d20 3d20 636d  'cmd_flag'] = cm
+0000de50: 645f 666c 6167 0a20 2020 2020 2020 2020  d_flag.         
+0000de60: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
+0000de70: 7061 7261 6d73 5b27 6465 7363 7269 7074  params['descript
+0000de80: 696f 6e27 5d20 3d20 696e 7075 745b 2764  ion'] = input['d
+0000de90: 6573 6372 6970 7469 6f6e 275d 0a20 2020  escription'].   
+0000dea0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000deb0: 6b66 6c6f 775f 6469 6374 5b69 6e70 7574  kflow_dict[input
+0000dec0: 5b27 6964 275d 5d20 3d20 776f 726b 666c  ['id']] = workfl
+0000ded0: 6f77 5f70 6172 616d 730a 2020 2020 2020  ow_params.      
+0000dee0: 2020 7265 7475 726e 2077 6f72 6b66 6c6f    return workflo
+0000def0: 775f 6469 6374 0a0a 2020 2020 6465 6620  w_dict..    def 
+0000df00: 636f 6e76 6572 745f 6379 7479 7065 5f74  convert_cytype_t
+0000df10: 6f5f 6f6d 7479 7065 2873 656c 662c 0a20  o_omtype(self,. 
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df40: 6379 7479 7065 3a20 7374 722c 205f 6465  cytype: str, _de
+0000df50: 6661 756c 742c 202a 6172 6773 2c20 2a2a  fault, *args, **
+0000df60: 6b77 6172 6773 0a20 2020 2020 2020 2020  kwargs.         
+0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df80: 2020 2020 2020 2020 2920 2d3e 2041 6e79          ) -> Any
+0000df90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000dfa0: 2020 2020 2020 436f 6e76 6572 7420 6120        Convert a 
+0000dfb0: 4379 746f 6d69 6e65 2074 7970 6520 746f  Cytomine type to
+0000dfc0: 2061 6e20 4f4d 4552 4f20 7479 7065 2061   an OMERO type a
+0000dfd0: 6e64 2069 6e73 7461 6e74 6961 7465 7320  nd instantiates 
+0000dfe0: 6974 0a20 2020 2020 2020 2077 6974 6820  it.        with 
+0000dff0: 6172 6773 2f6b 7761 7267 732e 0a0a 2020  args/kwargs...  
+0000e000: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
+0000e010: 4379 746f 6d69 6e65 2068 6173 2061 2050  Cytomine has a P
+0000e020: 7974 686f 6e20 436c 6965 6e74 2c20 616e  ython Client, an
+0000e030: 6420 736f 6d65 2063 6f6e 7665 7273 696f  d some conversio
+0000e040: 6e20 6d65 7468 6f64 730a 2020 2020 2020  n methods.      
+0000e050: 2020 746f 2070 7974 686f 6e20 7479 7065    to python type
+0000e060: 732c 2062 7574 206e 6f74 6869 6e67 2070  s, but nothing p
+0000e070: 6172 7469 6375 6c61 726c 7920 776f 7274  articularly wort
+0000e080: 6820 6465 7065 6e64 696e 6720 6f6e 2074  h depending on t
+0000e090: 6861 740a 2020 2020 2020 2020 6c69 6272  hat.        libr
+0000e0a0: 6172 7920 666f 7220 7965 742e 204d 6967  ary for yet. Mig
+0000e0b0: 6874 2062 6520 7573 6566 756c 2069 6e20  ht be useful in 
+0000e0c0: 7468 6520 6675 7475 7265 2070 6572 6861  the future perha
+0000e0d0: 7073 2e0a 2020 2020 2020 2020 2865 2e67  ps..        (e.g
+0000e0e0: 2e20 6874 7470 733a 2f2f 6769 7468 7562  . https://github
+0000e0f0: 2e63 6f6d 2f43 7974 6f6d 696e 652d 554c  .com/Cytomine-UL
+0000e100: 6965 6765 2f43 7974 6f6d 696e 652d 7079  iege/Cytomine-py
+0000e110: 7468 6f6e 2d63 6c69 656e 742f 0a20 2020  thon-client/.   
+0000e120: 2020 2020 2062 6c6f 622f 6d61 7374 6572       blob/master
+0000e130: 2f63 7974 6f6d 696e 652f 6379 746f 6d69  /cytomine/cytomi
+0000e140: 6e65 5f6a 6f62 2e70 7929 0a0a 2020 2020  ne_job.py)..    
+0000e150: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000e160: 2020 2020 2020 6379 7479 7065 2028 7374        cytype (st
+0000e170: 7229 3a20 5468 6520 4379 746f 6d69 6e65  r): The Cytomine
+0000e180: 2074 7970 6520 746f 2063 6f6e 7665 7274   type to convert
+0000e190: 2e0a 2020 2020 2020 2020 2020 2020 5f64  ..            _d
+0000e1a0: 6566 6175 6c74 3a20 5468 6520 6465 6661  efault: The defa
+0000e1b0: 756c 7420 7661 6c75 652e 2052 6571 7569  ult value. Requi
+0000e1c0: 7265 6420 746f 2064 6973 7469 6e67 7569  red to distingui
+0000e1d0: 7368 2062 6574 7765 656e 2066 6c6f 6174  sh between float
+0000e1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1f0: 2061 6e64 2069 6e74 2e0a 2020 2020 2020   and int..      
+0000e200: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
+0000e210: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
+0000e220: 616c 2061 7267 756d 656e 7473 2e0a 2020  al arguments..  
+0000e230: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000e240: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000e250: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000e260: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000e270: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000e280: 416e 793a 0a20 2020 2020 2020 2020 2020  Any:.           
+0000e290: 2020 2020 2054 6865 2063 6f6e 7665 7274       The convert
+0000e2a0: 6564 204f 4d45 524f 2074 7970 6520 636c  ed OMERO type cl
+0000e2b0: 6173 7320 696e 7374 616e 6365 0a20 2020  ass instance.   
+0000e2c0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000e2d0: 4e6f 6e65 2069 6620 6572 726f 7273 206f  None if errors o
+0000e2e0: 6363 7572 6564 2e0a 0a20 2020 2020 2020  ccured...       
+0000e2f0: 2022 2222 0a20 2020 2020 2020 2023 2054   """.        # T
+0000e300: 4f44 4f20 6d61 6b65 2045 6e75 6d20 3f0a  ODO make Enum ?.
+0000e310: 2020 2020 2020 2020 6966 2063 7974 7970          if cytyp
+0000e320: 6520 3d3d 2027 4e75 6d62 6572 273a 0a20  e == 'Number':. 
+0000e330: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000e340: 696e 7374 616e 6365 285f 6465 6661 756c  instance(_defaul
+0000e350: 742c 2066 6c6f 6174 293a 0a20 2020 2020  t, float):.     
+0000e360: 2020 2020 2020 2020 2020 2023 2066 6c6f             # flo
+0000e370: 6174 2069 6e73 7465 6164 0a20 2020 2020  at instead.     
+0000e380: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e390: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
+0000e3a0: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
+0000e3b0: 7473 222c 2022 466c 6f61 7422 2c0a 2020  ts", "Float",.  
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
+0000e3f0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+0000e400: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000e410: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e420: 2073 656c 662e 7374 725f 746f 5f63 6c61   self.str_to_cla
+0000e430: 7373 2822 6f6d 6572 6f2e 7363 7269 7074  ss("omero.script
+0000e440: 7322 2c20 2249 6e74 222c 0a20 2020 2020  s", "Int",.     
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
+0000e480: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
+0000e490: 6620 6379 7479 7065 203d 3d20 2742 6f6f  f cytype == 'Boo
+0000e4a0: 6c65 616e 273a 0a20 2020 2020 2020 2020  lean':.         
+0000e4b0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+0000e4c0: 7472 5f74 6f5f 636c 6173 7328 226f 6d65  tr_to_class("ome
+0000e4d0: 726f 2e73 6372 6970 7473 222c 2022 426f  ro.scripts", "Bo
+0000e4e0: 6f6c 222c 0a20 2020 2020 2020 2020 2020  ol",.           
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
+0000e510: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000e520: 2020 2065 6c69 6620 6379 7479 7065 203d     elif cytype =
+0000e530: 3d20 2753 7472 696e 6727 3a0a 2020 2020  = 'String':.    
+0000e540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000e550: 656c 662e 7374 725f 746f 5f63 6c61 7373  elf.str_to_class
+0000e560: 2822 6f6d 6572 6f2e 7363 7269 7074 7322  ("omero.scripts"
+0000e570: 2c20 2253 7472 696e 6722 2c0a 2020 2020  , "String",.    
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+0000e5b0: 290a 0a20 2020 2064 6566 2065 7874 7261  )..    def extra
+0000e5c0: 6374 5f70 6172 7473 5f66 726f 6d5f 7572  ct_parts_from_ur
+0000e5d0: 6c28 7365 6c66 2c20 696e 7075 745f 7572  l(self, input_ur
+0000e5e0: 6c3a 2073 7472 2920 2d3e 2054 7570 6c65  l: str) -> Tuple
+0000e5f0: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
+0000e600: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000e610: 2020 2020 2020 4578 7472 6163 7420 7468        Extract th
+0000e620: 6520 7265 706f 7369 746f 7279 2061 6e64  e repository and
+0000e630: 2062 7261 6e63 6820 696e 666f 726d 6174   branch informat
+0000e640: 696f 6e20 6672 6f6d 2074 6865 2069 6e70  ion from the inp
+0000e650: 7574 2055 524c 2e0a 0a20 2020 2020 2020  ut URL...       
+0000e660: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000e670: 2020 2069 6e70 7574 5f75 726c 2028 7374     input_url (st
+0000e680: 7229 3a20 5468 6520 696e 7075 7420 4769  r): The input Gi
+0000e690: 7448 7562 2055 524c 2e0a 0a20 2020 2020  tHub URL...     
+0000e6a0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000e6b0: 2020 2020 2020 2020 5475 706c 655b 4c69          Tuple[Li
+0000e6c0: 7374 5b73 7472 5d2c 2073 7472 5d3a 0a20  st[str], str]:. 
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000e6e0: 6865 206c 6973 7420 6f66 2075 726c 2070  he list of url p
+0000e6f0: 6172 7473 2061 6e64 2074 6865 2062 7261  arts and the bra
+0000e700: 6e63 682f 7665 7273 696f 6e2e 0a20 2020  nch/version..   
+0000e710: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+0000e720: 6e6f 2062 7261 6e63 6820 6973 2066 6f75  no branch is fou
+0000e730: 6e64 2c20 6974 2077 696c 6c20 7265 7475  nd, it will retu
+0000e740: 726e 2022 6d61 7374 6572 220a 0a20 2020  rn "master"..   
+0000e750: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0000e760: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+0000e770: 726f 723a 2049 6620 7468 6520 696e 7075  ror: If the inpu
+0000e780: 7420 5552 4c20 6973 206e 6f74 2061 2076  t URL is not a v
+0000e790: 616c 6964 2047 6974 4875 6220 5552 4c2e  alid GitHub URL.
+0000e7a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e7b0: 2020 2020 2075 726c 5f70 6172 7473 203d       url_parts =
+0000e7c0: 2069 6e70 7574 5f75 726c 2e73 706c 6974   input_url.split
+0000e7d0: 2822 2f22 290a 2020 2020 2020 2020 6966  ("/").        if
+0000e7e0: 206c 656e 2875 726c 5f70 6172 7473 2920   len(url_parts) 
+0000e7f0: 3c20 3520 6f72 2075 726c 5f70 6172 7473  < 5 or url_parts
+0000e800: 5b32 5d20 213d 2022 6769 7468 7562 2e63  [2] != "github.c
+0000e810: 6f6d 223a 0a20 2020 2020 2020 2020 2020  om":.           
+0000e820: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000e830: 7228 2249 6e76 616c 6964 2047 6974 4875  r("Invalid GitHu
+0000e840: 6220 5552 4c22 290a 0a20 2020 2020 2020  b URL")..       
+0000e850: 2069 6620 2274 7265 6522 2069 6e20 7572   if "tree" in ur
+0000e860: 6c5f 7061 7274 733a 0a20 2020 2020 2020  l_parts:.       
+0000e870: 2020 2020 2023 2043 6173 653a 2055 524c       # Case: URL
+0000e880: 2063 6f6e 7461 696e 7320 6120 6272 616e   contains a bran
+0000e890: 6368 0a20 2020 2020 2020 2020 2020 2062  ch.            b
+0000e8a0: 7261 6e63 685f 696e 6465 7820 3d20 7572  ranch_index = ur
+0000e8b0: 6c5f 7061 7274 732e 696e 6465 7828 2274  l_parts.index("t
+0000e8c0: 7265 6522 2920 2b20 310a 2020 2020 2020  ree") + 1.      
+0000e8d0: 2020 2020 2020 6272 616e 6368 203d 2075        branch = u
+0000e8e0: 726c 5f70 6172 7473 5b62 7261 6e63 685f  rl_parts[branch_
+0000e8f0: 696e 6465 785d 0a20 2020 2020 2020 2065  index].        e
+0000e900: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000e910: 2023 2043 6173 653a 2055 524c 2064 6f65   # Case: URL doe
+0000e920: 7320 6e6f 7420 7370 6563 6966 7920 6120  s not specify a 
+0000e930: 6272 616e 6368 0a20 2020 2020 2020 2020  branch.         
+0000e940: 2020 2062 7261 6e63 6820 3d20 226d 6173     branch = "mas
+0000e950: 7465 7222 0a0a 2020 2020 2020 2020 7265  ter"..        re
+0000e960: 7475 726e 2075 726c 5f70 6172 7473 2c20  turn url_parts, 
+0000e970: 6272 616e 6368 0a0a 2020 2020 6465 6620  branch..    def 
+0000e980: 636f 6e76 6572 745f 7572 6c28 7365 6c66  convert_url(self
+0000e990: 2c20 696e 7075 745f 7572 6c3a 2073 7472  , input_url: str
+0000e9a0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+0000e9b0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
+0000e9c0: 6e76 6572 7420 7468 6520 696e 7075 7420  nvert the input 
+0000e9d0: 4769 7448 7562 2055 524c 2074 6f20 616e  GitHub URL to an
+0000e9e0: 206f 7574 7075 7420 5552 4c20 7468 6174   output URL that
+0000e9f0: 2072 6574 7269 6576 6573 0a20 2020 2020   retrieves.     
+0000ea00: 2020 2074 6865 2027 6465 7363 7269 7074     the 'descript
+0000ea10: 6f72 2e6a 736f 6e27 2066 696c 6520 696e  or.json' file in
+0000ea20: 2072 6177 2066 6f72 6d61 742e 0a0a 2020   raw format...  
+0000ea30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0000ea40: 2020 2020 2020 2020 696e 7075 745f 7572          input_ur
+0000ea50: 6c20 2873 7472 293a 2054 6865 2069 6e70  l (str): The inp
+0000ea60: 7574 2047 6974 4875 6220 5552 4c2e 0a0a  ut GitHub URL...
+0000ea70: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000ea80: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000ea90: 3a20 5468 6520 6f75 7470 7574 2055 524c  : The output URL
+0000eaa0: 2074 6f20 7468 6520 2764 6573 6372 6970   to the 'descrip
+0000eab0: 746f 722e 6a73 6f6e 2720 6669 6c65 2e0a  tor.json' file..
+0000eac0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0000ead0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+0000eae0: 7565 4572 726f 723a 2049 6620 7468 6520  ueError: If the 
+0000eaf0: 696e 7075 7420 5552 4c20 6973 206e 6f74  input URL is not
+0000eb00: 2061 2076 616c 6964 2047 6974 4875 6220   a valid GitHub 
+0000eb10: 5552 4c2e 0a20 2020 2020 2020 2022 2222  URL..        """
+0000eb20: 0a20 2020 2020 2020 2075 726c 5f70 6172  .        url_par
+0000eb30: 7473 2c20 6272 616e 6368 203d 2073 656c  ts, branch = sel
+0000eb40: 662e 6578 7472 6163 745f 7061 7274 735f  f.extract_parts_
+0000eb50: 6672 6f6d 5f75 726c 2869 6e70 7574 5f75  from_url(input_u
+0000eb60: 726c 290a 0a20 2020 2020 2020 2023 2043  rl)..        # C
+0000eb70: 6f6e 7374 7275 6374 2074 6865 206f 7574  onstruct the out
+0000eb80: 7075 7420 5552 4c20 6279 2063 6f6d 6269  put URL by combi
+0000eb90: 6e69 6e67 2074 6865 2065 7874 7261 6374  ning the extract
+0000eba0: 6564 2069 6e66 6f72 6d61 7469 6f6e 0a20  ed information. 
+0000ebb0: 2020 2020 2020 2023 2077 6974 6820 7468         # with th
+0000ebc0: 6520 6465 7369 7265 6420 6669 6c65 2070  e desired file p
+0000ebd0: 6174 680a 2020 2020 2020 2020 6f75 7470  ath.        outp
+0000ebe0: 7574 5f75 726c 203d 2066 2268 7474 7073  ut_url = f"https
+0000ebf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7b75  ://github.com/{u
+0000ec00: 726c 5f70 6172 7473 5b33 5d7d 2f7b 7572  rl_parts[3]}/{ur
+0000ec10: 6c5f 7061 7274 735b 345d 7d2f 7261 772f  l_parts[4]}/raw/
+0000ec20: 7b62 7261 6e63 687d 2f64 6573 6372 6970  {branch}/descrip
+0000ec30: 746f 722e 6a73 6f6e 220a 0a20 2020 2020  tor.json"..     
+0000ec40: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
+0000ec50: 5f75 726c 0a0a 2020 2020 6465 6620 7075  _url..    def pu
+0000ec60: 6c6c 5f64 6573 6372 6970 746f 725f 6672  ll_descriptor_fr
+0000ec70: 6f6d 5f67 6974 6875 6228 7365 6c66 2c20  om_github(self, 
+0000ec80: 776f 726b 666c 6f77 3a20 7374 7229 202d  workflow: str) -
+0000ec90: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
+0000eca0: 2222 220a 2020 2020 2020 2020 5075 6c6c  """.        Pull
+0000ecb0: 2074 6865 2077 6f72 6b66 6c6f 7720 6465   the workflow de
+0000ecc0: 7363 7269 7074 6f72 2066 726f 6d20 4769  scriptor from Gi
+0000ecd0: 7448 7562 2e0a 0a20 2020 2020 2020 2041  tHub...        A
+0000ece0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000ecf0: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
+0000ed00: 2054 6865 2077 6f72 6b66 6c6f 7720 666f   The workflow fo
+0000ed10: 7220 7768 6963 6820 746f 2070 756c 6c20  r which to pull 
+0000ed20: 7468 6520 6465 7363 7269 7074 6f72 2e0a  the descriptor..
+0000ed30: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000ed40: 3a0a 2020 2020 2020 2020 2020 2020 4469  :.            Di
+0000ed50: 6374 3a20 5468 6520 4a53 4f4e 2064 6573  ct: The JSON des
+0000ed60: 6372 6970 746f 722e 0a0a 2020 2020 2020  criptor...      
+0000ed70: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+0000ed80: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+0000ed90: 3a20 4966 2061 6e20 6572 726f 7220 6f63  : If an error oc
+0000eda0: 6375 7273 2077 6869 6c65 2070 756c 6c69  curs while pulli
+0000edb0: 6e67 2074 6865 2064 6573 6372 6970 746f  ng the descripto
+0000edc0: 7220 6669 6c65 2e0a 2020 2020 2020 2020  r file..        
+0000edd0: 2222 220a 2020 2020 2020 2020 6769 745f  """.        git_
+0000ede0: 7265 706f 203d 2073 656c 662e 736c 7572  repo = self.slur
+0000edf0: 6d5f 6d6f 6465 6c5f 7265 706f 735b 776f  m_model_repos[wo
+0000ee00: 726b 666c 6f77 5d0a 2020 2020 2020 2020  rkflow].        
+0000ee10: 2320 636f 6e76 6572 7420 6769 7420 7265  # convert git re
+0000ee20: 706f 2074 6f20 6a73 6f6e 2066 696c 650a  po to json file.
+0000ee30: 2020 2020 2020 2020 7261 775f 7572 6c20          raw_url 
+0000ee40: 3d20 7365 6c66 2e63 6f6e 7665 7274 5f75  = self.convert_u
+0000ee50: 726c 2867 6974 5f72 6570 6f29 0a20 2020  rl(git_repo).   
+0000ee60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000ee70: 6728 6622 5075 6c6c 2077 6f72 6b66 6c6f  g(f"Pull workflo
+0000ee80: 773a 207b 776f 726b 666c 6f77 7d3a 207b  w: {workflow}: {
+0000ee90: 6769 745f 7265 706f 7d20 3e3e 207b 7261  git_repo} >> {ra
+0000eea0: 775f 7572 6c7d 2229 0a20 2020 2020 2020  w_url}").       
+0000eeb0: 2023 2070 756c 6c20 776f 726b 666c 6f77   # pull workflow
+0000eec0: 2070 6172 616d 730a 2020 2020 2020 2020   params.        
+0000eed0: 6769 7468 7562 5f73 6573 7369 6f6e 203d  github_session =
+0000eee0: 2073 656c 662e 6765 745f 6f72 5f63 7265   self.get_or_cre
+0000eef0: 6174 655f 6769 7468 7562 5f73 6573 7369  ate_github_sessi
+0000ef00: 6f6e 2829 0a20 2020 2020 2020 2067 6866  on().        ghf
+0000ef10: 696c 6520 3d20 6769 7468 7562 5f73 6573  ile = github_ses
+0000ef20: 7369 6f6e 2e67 6574 2872 6177 5f75 726c  sion.get(raw_url
+0000ef30: 290a 2020 2020 2020 2020 6966 2067 6866  ).        if ghf
+0000ef40: 696c 652e 6f6b 3a0a 2020 2020 2020 2020  ile.ok:.        
+0000ef50: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000ef60: 2866 2243 6163 6865 643f 207b 6768 6669  (f"Cached? {ghfi
+0000ef70: 6c65 2e66 726f 6d5f 6361 6368 657d 2229  le.from_cache}")
+0000ef80: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
+0000ef90: 6e5f 6465 7363 7269 7074 6f72 203d 2067  n_descriptor = g
+0000efa0: 6866 696c 652e 6a73 6f6e 2829 0a20 2020  hfile.json().   
+0000efb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000efc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000efd0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+0000efe0: 2020 2020 2020 2020 2066 2745 7272 6f72           f'Error
+0000eff0: 2077 6869 6c65 2070 756c 6c69 6e67 2064   while pulling d
+0000f000: 6573 6372 6970 746f 7220 6669 6c65 2066  escriptor file f
+0000f010: 6f72 2077 6f72 6b66 6c6f 7720 7b77 6f72  or workflow {wor
+0000f020: 6b66 6c6f 777d 2c5c 0a20 2020 2020 2020  kflow},\.       
+0000f030: 2020 2020 2020 2020 2020 2020 2066 726f               fro
+0000f040: 6d20 7b72 6177 5f75 726c 7d3a 207b 6768  m {raw_url}: {gh
+0000f050: 6669 6c65 2e5f 5f64 6963 745f 5f7d 2729  file.__dict__}')
+0000f060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f070: 6a73 6f6e 5f64 6573 6372 6970 746f 720a  json_descriptor.
+0000f080: 0a20 2020 2064 6566 2067 6574 5f6f 725f  .    def get_or_
+0000f090: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
+0000f0a0: 7373 696f 6e28 7365 6c66 293a 0a20 2020  ssion(self):.   
+0000f0b0: 2020 2020 2023 204e 6f74 652c 2075 7369       # Note, usi
+0000f0c0: 6e67 2072 6571 7565 7374 735f 6361 6368  ng requests_cach
+0000f0d0: 6520 312e 312e 312c 2063 6f6e 6469 7469  e 1.1.1, conditi
+0000f0e0: 6f6e 616c 2071 7565 7269 6573 2061 7265  onal queries are
+0000f0f0: 2064 6566 6175 6c74 3a0a 2020 2020 2020   default:.      
+0000f100: 2020 2320 5468 6520 6361 6368 6564 2072    # The cached r
+0000f110: 6573 706f 6e73 6520 7769 6c6c 2073 7469  esponse will sti
+0000f120: 6c6c 2062 6520 7573 6564 2075 6e74 696c  ll be used until
+0000f130: 2074 6865 2072 656d 6f74 6520 636f 6e74   the remote cont
+0000f140: 656e 7420 6163 7475 616c 6c79 2063 6861  ent actually cha
+0000f150: 6e67 6573 0a20 2020 2020 2020 2023 2045  nges.        # E
+0000f160: 7665 6e20 6966 2074 6865 2027 6578 7069  ven if the 'expi
+0000f170: 7265 5f61 6674 6572 2720 6973 2074 7269  re_after' is tri
+0000f180: 6767 6572 6564 2e20 5468 6973 2069 7320  ggered. This is 
+0000f190: 6275 696c 7420 696e 746f 2047 6974 4875  built into GitHu
+0000f1a0: 622c 2077 6869 6368 2072 6574 7572 6e73  b, which returns
+0000f1b0: 0a20 2020 2020 2020 2023 2061 2045 7461  .        # a Eta
+0000f1c0: 6720 696e 2074 6865 2068 6561 6465 7220  g in the header 
+0000f1d0: 7468 6174 206f 6e6c 7920 6368 616e 6765  that only change
+0000f1e0: 7320 7768 656e 2074 6865 2063 6f6e 7465  s when the conte
+0000f1f0: 6e74 2028 652e 672e 2074 6865 2064 6573  nt (e.g. the des
+0000f200: 6372 6970 746f 7229 2063 6861 6e67 6573  criptor) changes
+0000f210: 2e0a 2020 2020 2020 2020 2320 4966 2079  ..        # If y
+0000f220: 6f75 2070 726f 7669 6465 2074 6869 7320  ou provide this 
+0000f230: 4574 6167 2077 6865 6e20 7175 6572 7969  Etag when queryi
+0000f240: 6e67 2c20 796f 7520 7769 6c6c 2067 6574  ng, you will get
+0000f250: 2061 2033 3034 2028 276e 6f20 6368 616e   a 304 ('no chan
+0000f260: 6765 2729 2061 6e64 2069 7420 7769 6c6c  ge') and it will
+0000f270: 0a20 2020 2020 2020 2023 204e 4f54 2063  .        # NOT c
+0000f280: 6f75 6e74 2074 6f77 6172 6473 2079 6f75  ount towards you
+0000f290: 7220 4769 7468 7562 206c 696d 6974 732e  r Github limits.
+0000f2a0: 2041 6e64 2072 6571 7565 7374 735f 6361   And requests_ca
+0000f2b0: 6368 6520 646f 6573 2074 6861 7420 666f  che does that fo
+0000f2c0: 7220 7573 206e 6f77 2e0a 2020 2020 2020  r us now..      
+0000f2d0: 2020 2320 4e6f 7420 6176 6169 6c61 626c    # Not availabl
+0000f2e0: 6520 696e 2050 7974 686f 6e33 2e36 2074  e in Python3.6 t
+0000f2f0: 686f 7567 682e 0a20 2020 2020 2020 2073  hough..        s
+0000f300: 203d 2072 6571 7565 7374 735f 6361 6368   = requests_cach
+0000f310: 652e 4361 6368 6564 5365 7373 696f 6e28  e.CachedSession(
+0000f320: 2767 6974 6875 625f 6361 6368 6527 2c0a  'github_cache',.
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f350: 2020 2020 2020 2020 2062 6163 6b65 6e64           backend
+0000f360: 3d73 656c 662e 6361 6368 652c 0a20 2020  =self.cache,.   
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f390: 2020 2020 2020 6578 7069 7265 5f61 6674        expire_aft
+0000f3a0: 6572 3d31 2c0a 2020 2020 2020 2020 2020  er=1,.          
+0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f3d0: 6163 6865 5f63 6f6e 7472 6f6c 3d54 7275  ache_control=Tru
+0000f3e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f410: 2020 2020 2023 204d 6967 6874 2068 6176       # Might hav
+0000f420: 6520 6269 6767 6572 2069 7373 7565 732c  e bigger issues,
+0000f430: 2074 6869 7320 6973 2072 656c 6174 6564   this is related
+0000f440: 2074 6f20 7261 7465 206c 696d 6974 7320   to rate limits 
+0000f450: 6f6e 2047 6974 4875 620a 2020 2020 2020  on GitHub.      
+0000f460: 2020 2320 6874 7470 733a 2f2f 646f 6373    # https://docs
+0000f470: 2e67 6974 6875 622e 636f 6d2f 656e 2f72  .github.com/en/r
+0000f480: 6573 742f 7573 696e 672d 7468 652d 7265  est/using-the-re
+0000f490: 7374 2d61 7069 2f72 6174 652d 6c69 6d69  st-api/rate-limi
+0000f4a0: 7473 2d66 6f72 2d74 6865 2d72 6573 742d  ts-for-the-rest-
+0000f4b0: 6170 690a 2020 2020 2020 2020 2320 4966  api.        # If
+0000f4c0: 2069 7420 7374 6179 7320 6120 7072 6f62   it stays a prob
+0000f4d0: 6c65 6d2c 2077 6520 6861 7665 2074 6f20  lem, we have to 
+0000f4e0: 6164 6420 616e 206f 7074 696f 6e20 746f  add an option to
+0000f4f0: 2061 6464 2061 2047 4820 6b65 7920 746f   add a GH key to
+0000f500: 2074 6865 2063 6f6e 6669 670a 2020 2020   the config.    
+0000f510: 2020 2020 2320 452e 672e 2073 6565 2068      # E.g. see h
+0000f520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000f530: 6d2f 7265 7175 6573 7473 2d63 6163 6865  m/requests-cache
+0000f540: 2f72 6571 7565 7374 732d 6361 6368 652f  /requests-cache/
+0000f550: 626c 6f62 2f35 3331 3334 6566 3065 3939  blob/53134ef0e99
+0000f560: 6437 3133 6665 6436 3235 3135 6466 6237  d713fed62515dfb7
+0000f570: 6263 6661 6163 3566 3633 6639 642f 6578  bcfaac5f63f9d/ex
+0000f580: 616d 706c 6573 2f70 7967 6974 6875 622e  amples/pygithub.
+0000f590: 7079 0a20 2020 2020 2020 2023 2048 6572  py.        # Her
+0000f5a0: 6520 796f 7520 636f 756c 6420 6861 7665  e you could have
+0000f5b0: 2061 6e20 4143 4345 5353 5f54 4f4b 454e   an ACCESS_TOKEN
+0000f5c0: 2e0a 2020 2020 2020 2020 2320 416e 2041  ..        # An A
+0000f5d0: 4343 4553 535f 544f 4b45 4e20 636f 756c  CCESS_TOKEN coul
+0000f5e0: 6420 696d 7072 6f76 6520 6170 6920 6c69  d improve api li
+0000f5f0: 6d69 7473 2074 6f20 3530 3030 2f68 2028  mits to 5000/h (
+0000f600: 6672 6f6d 2036 302f 6829 2e0a 2020 2020  from 60/h)..    
+0000f610: 2020 2020 7265 7472 795f 7374 7261 7465      retry_strate
+0000f620: 6779 203d 2052 6574 7279 280a 2020 2020  gy = Retry(.    
+0000f630: 2020 2020 2020 2020 746f 7461 6c3d 352c          total=5,
+0000f640: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f650: 204d 6178 696d 756d 206e 756d 6265 7220   Maximum number 
+0000f660: 6f66 2072 6574 7269 6573 0a20 2020 2020  of retries.     
+0000f670: 2020 2020 2020 2023 2045 7870 6f6e 656e         # Exponen
+0000f680: 7469 616c 2062 6163 6b6f 6666 2066 6163  tial backoff fac
+0000f690: 746f 7220 2864 656c 6179 2062 6574 7765  tor (delay betwe
+0000f6a0: 656e 2072 6574 7269 6573 290a 2020 2020  en retries).    
+0000f6b0: 2020 2020 2020 2020 6261 636b 6f66 665f          backoff_
+0000f6c0: 6661 6374 6f72 3d35 2c0a 2020 2020 2020  factor=5,.      
+0000f6d0: 2020 2020 2020 2320 5265 7472 7920 6f6e        # Retry on
+0000f6e0: 2074 6865 7365 2048 5454 5020 7374 6174   these HTTP stat
+0000f6f0: 7573 2063 6f64 6573 0a20 2020 2020 2020  us codes.       
+0000f700: 2020 2020 2073 7461 7475 735f 666f 7263       status_forc
+0000f710: 656c 6973 743d 5b35 3030 2c20 3530 322c  elist=[500, 502,
+0000f720: 2035 3033 2c20 3530 342c 2034 3033 2c20   503, 504, 403, 
+0000f730: 3432 395d 2c0a 2020 2020 2020 2020 2020  429],.          
+0000f740: 2020 616c 6c6f 7765 645f 6d65 7468 6f64    allowed_method
+0000f750: 733d 6672 6f7a 656e 7365 7428 5b27 4745  s=frozenset(['GE
+0000f760: 5427 5d29 2020 2320 4f6e 6c79 2072 6574  T'])  # Only ret
+0000f770: 7279 2066 6f72 2047 4554 2072 6571 7565  ry for GET reque
+0000f780: 7374 730a 2020 2020 2020 2020 290a 2020  sts.        ).  
+0000f790: 2020 2020 2020 732e 6d6f 756e 7428 2768        s.mount('h
+0000f7a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000f7b0: 6d2f 272c 2048 5454 5041 6461 7074 6572  m/', HTTPAdapter
+0000f7c0: 286d 6178 5f72 6574 7269 6573 3d72 6574  (max_retries=ret
+0000f7d0: 7279 5f73 7472 6174 6567 7929 290a 2020  ry_strategy)).  
+0000f7e0: 2020 2020 2020 732e 6d6f 756e 7428 2768        s.mount('h
+0000f7f0: 7474 703a 2f2f 6769 7468 7562 2e63 6f6d  ttp://github.com
+0000f800: 2f27 2c20 4854 5450 4164 6170 7465 7228  /', HTTPAdapter(
+0000f810: 6d61 785f 7265 7472 6965 733d 7265 7472  max_retries=retr
+0000f820: 795f 7374 7261 7465 6779 2929 0a20 2020  y_strategy)).   
+0000f830: 2020 2020 2072 6574 7572 6e20 730a 0a20       return s.. 
+0000f840: 2020 2064 6566 2067 6574 5f77 6f72 6b66     def get_workf
+0000f850: 6c6f 775f 636f 6d6d 616e 6428 7365 6c66  low_command(self
+0000f860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000f880: 6f72 6b66 6c6f 773a 2073 7472 2c0a 2020  orkflow: str,.  
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000f8b0: 6c6f 775f 7665 7273 696f 6e3a 2073 7472  low_version: str
+0000f8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f8e0: 6e70 7574 5f64 6174 613a 2073 7472 2c0a  nput_data: str,.
+0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f900: 2020 2020 2020 2020 2020 2020 2065 6d61               ema
+0000f910: 696c 3a20 4f70 7469 6f6e 616c 5b73 7472  il: Optional[str
+0000f920: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f940: 2020 2020 2020 2074 696d 653a 204f 7074         time: Opt
+0000f950: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000f960: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2a2a 6b77 6172 6773 2920 2d3e 2054 7570  **kwargs) -> Tup
+0000f990: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
+0000f9a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f9b0: 2020 2047 656e 6572 6174 6520 7468 6520     Generate the 
+0000f9c0: 536c 7572 6d20 776f 726b 666c 6f77 2063  Slurm workflow c
+0000f9d0: 6f6d 6d61 6e64 2061 6e64 2065 6e76 6972  ommand and envir
+0000f9e0: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+0000f9f0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000fa00: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+0000fa10: 6b66 6c6f 7720 2873 7472 293a 2054 6865  kflow (str): The
+0000fa20: 206e 616d 6520 6f66 2074 6865 2077 6f72   name of the wor
+0000fa30: 6b66 6c6f 772e 0a20 2020 2020 2020 2020  kflow..         
+0000fa40: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+0000fa50: 696f 6e20 2873 7472 293a 2054 6865 2076  ion (str): The v
+0000fa60: 6572 7369 6f6e 206f 6620 7468 6520 776f  ersion of the wo
+0000fa70: 726b 666c 6f77 2e0a 2020 2020 2020 2020  rkflow..        
+0000fa80: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
+0000fa90: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+0000faa0: 6620 7468 6520 696e 7075 7420 6461 7461  f the input data
+0000fab0: 2066 6f6c 6465 7220 636f 6e74 6169 6e69   folder containi
+0000fac0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+0000fad0: 2020 2074 6865 2069 6e70 7574 2069 6d61     the input ima
+0000fae0: 6765 2066 696c 6573 2e0a 2020 2020 2020  ge files..      
+0000faf0: 2020 2020 2020 656d 6169 6c20 2873 7472        email (str
+0000fb00: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000fb10: 2065 6d61 696c 2061 6464 7265 7373 2066   email address f
+0000fb20: 6f72 206a 6f62 206e 6f74 6966 6963 6174  or job notificat
+0000fb30: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+0000fb40: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+0000fb50: 6f20 4e6f 6e65 2c20 7768 6963 6820 6465  o None, which de
+0000fb60: 6661 756c 7473 2074 6f20 7768 6174 2069  faults to what i
+0000fb70: 7320 696e 2074 6865 206a 6f62 2073 6372  s in the job scr
+0000fb80: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
+0000fb90: 2074 696d 6520 2873 7472 2c20 6f70 7469   time (str, opti
+0000fba0: 6f6e 616c 293a 2054 6865 2074 696d 6520  onal): The time 
+0000fbb0: 6c69 6d69 7420 666f 7220 7468 6520 6a6f  limit for the jo
+0000fbc0: 6220 696e 2074 6865 200a 2020 2020 2020  b in the .      
+0000fbd0: 2020 2020 2020 2020 2020 666f 726d 6174            format
+0000fbe0: 2048 483a 4d4d 3a53 532e 2044 6566 6175   HH:MM:SS. Defau
+0000fbf0: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
+0000fc00: 6368 2064 6566 6175 6c74 7320 746f 2077  ch defaults to w
+0000fc10: 6861 7420 0a20 2020 2020 2020 2020 2020  hat .           
+0000fc20: 2020 2020 2069 7320 696e 2074 6865 206a       is in the j
+0000fc30: 6f62 2073 6372 6970 742e 0a20 2020 2020  ob script..     
+0000fc40: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+0000fc50: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+0000fc60: 6f72 6420 6172 6775 6d65 6e74 7320 666f  ord arguments fo
+0000fc70: 7220 7468 6520 776f 726b 666c 6f77 2e0a  r the workflow..
+0000fc80: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000fc90: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
+0000fca0: 706c 655b 7374 722c 2044 6963 745d 3a0a  ple[str, Dict]:.
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcc0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+0000fcd0: 6e67 2074 6865 2053 6c75 726d 2077 6f72  ng the Slurm wor
+0000fce0: 6b66 6c6f 7720 636f 6d6d 616e 6420 616e  kflow command an
+0000fcf0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000fd00: 2020 7468 6520 656e 7669 726f 6e6d 656e    the environmen
+0000fd10: 7420 7661 7269 6162 6c65 732e 0a0a 2020  t variables...  
+0000fd20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000fd30: 2020 6d6f 6465 6c5f 7061 7468 203d 2073    model_path = s
+0000fd40: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+0000fd50: 7061 7468 735b 776f 726b 666c 6f77 2e6c  paths[workflow.l
+0000fd60: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
+0000fd70: 6a6f 625f 7363 7269 7074 203d 2073 656c  job_script = sel
+0000fd80: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
+0000fd90: 6273 5b77 6f72 6b66 6c6f 772e 6c6f 7765  bs[workflow.lowe
+0000fda0: 7228 295d 0a20 2020 2020 2020 206a 6f62  r()].        job
+0000fdb0: 5f70 6172 616d 7320 3d20 7365 6c66 2e73  _params = self.s
+0000fdc0: 6c75 726d 5f6d 6f64 656c 5f6a 6f62 735f  lurm_model_jobs_
+0000fdd0: 7061 7261 6d73 5b77 6f72 6b66 6c6f 772e  params[workflow.
+0000fde0: 6c6f 7765 7228 295d 0a20 2020 2020 2020  lower()].       
+0000fdf0: 2023 2067 7261 6220 6f6e 6c79 2074 6865   # grab only the
+0000fe00: 2069 6d61 6765 206e 616d 652c 206e 6f74   image name, not
+0000fe10: 2074 6865 2067 726f 7570 2f63 7265 6174   the group/creat
+0000fe20: 6f72 0a20 2020 2020 2020 2069 6d61 6765  or.        image
+0000fe30: 203d 2073 656c 662e 736c 7572 6d5f 6d6f   = self.slurm_mo
+0000fe40: 6465 6c5f 696d 6167 6573 5b77 6f72 6b66  del_images[workf
+0000fe50: 6c6f 772e 6c6f 7765 7228 295d 2e73 706c  low.lower()].spl
+0000fe60: 6974 2822 2f22 295b 315d 0a0a 2020 2020  it("/")[1]..    
+0000fe70: 2020 2020 7362 6174 6368 5f65 6e76 203d      sbatch_env =
+0000fe80: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+0000fe90: 4441 5441 5f50 4154 4822 3a20 6622 7b73  DATA_PATH": f"{s
+0000fea0: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
+0000feb0: 6174 687d 2f7b 696e 7075 745f 6461 7461  ath}/{input_data
+0000fec0: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+0000fed0: 2249 4d41 4745 5f50 4154 4822 3a20 6622  "IMAGE_PATH": f"
+0000fee0: 7b73 656c 662e 736c 7572 6d5f 696d 6167  {self.slurm_imag
+0000fef0: 6573 5f70 6174 687d 2f7b 6d6f 6465 6c5f  es_path}/{model_
+0000ff00: 7061 7468 7d22 2c0a 2020 2020 2020 2020  path}",.        
+0000ff10: 2020 2020 2249 4d41 4745 5f56 4552 5349      "IMAGE_VERSI
+0000ff20: 4f4e 223a 2066 227b 776f 726b 666c 6f77  ON": f"{workflow
+0000ff30: 5f76 6572 7369 6f6e 7d22 2c0a 2020 2020  _version}",.    
+0000ff40: 2020 2020 2020 2020 2253 494e 4755 4c41          "SINGULA
+0000ff50: 5249 5459 5f49 4d41 4745 223a 2066 227b  RITY_IMAGE": f"{
+0000ff60: 696d 6167 657d 5f7b 776f 726b 666c 6f77  image}_{workflow
+0000ff70: 5f76 6572 7369 6f6e 7d2e 7369 6622 2c0a  _version}.sif",.
+0000ff80: 2020 2020 2020 2020 2020 2020 2253 4352              "SCR
+0000ff90: 4950 545f 5041 5448 223a 2066 227b 7365  IPT_PATH": f"{se
+0000ffa0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
+0000ffb0: 7061 7468 7d22 0a20 2020 2020 2020 207d  path}".        }
+0000ffc0: 0a20 2020 2020 2020 2077 6f72 6b66 6c6f  .        workflo
+0000ffd0: 775f 656e 7620 3d20 7365 6c66 2e77 6f72  w_env = self.wor
+0000ffe0: 6b66 6c6f 775f 7061 7261 6d73 5f74 6f5f  kflow_params_to_
+0000fff0: 656e 7676 6172 7328 2a2a 6b77 6172 6773  envvars(**kwargs
+00010000: 290a 2020 2020 2020 2020 656e 7620 3d20  ).        env = 
+00010010: 7b2a 2a73 6261 7463 685f 656e 762c 202a  {**sbatch_env, *
+00010020: 2a77 6f72 6b66 6c6f 775f 656e 767d 0a0a  *workflow_env}..
+00010030: 2020 2020 2020 2020 656d 6169 6c5f 7061          email_pa
+00010040: 7261 6d20 3d20 2222 2069 6620 656d 6169  ram = "" if emai
+00010050: 6c20 6973 204e 6f6e 6520 656c 7365 2066  l is None else f
+00010060: 2220 2d2d 6d61 696c 2d75 7365 723d 7b65  " --mail-user={e
+00010070: 6d61 696c 7d22 0a20 2020 2020 2020 2074  mail}".        t
+00010080: 696d 655f 7061 7261 6d20 3d20 2222 2069  ime_param = "" i
+00010090: 6620 7469 6d65 2069 7320 4e6f 6e65 2065  f time is None e
+000100a0: 6c73 6520 6622 202d 2d74 696d 653d 7b74  lse f" --time={t
+000100b0: 696d 657d 220a 2020 2020 2020 2020 6a6f  ime}".        jo
+000100c0: 625f 7061 7261 6d73 2e61 7070 656e 6428  b_params.append(
+000100d0: 7469 6d65 5f70 6172 616d 290a 2020 2020  time_param).    
+000100e0: 2020 2020 6a6f 625f 7061 7261 6d73 2e61      job_params.a
+000100f0: 7070 656e 6428 656d 6169 6c5f 7061 7261  ppend(email_para
+00010100: 6d29 0a20 2020 2020 2020 206a 6f62 5f70  m).        job_p
+00010110: 6172 616d 203d 2022 222e 6a6f 696e 286a  aram = "".join(j
+00010120: 6f62 5f70 6172 616d 7329 0a20 2020 2020  ob_params).     
+00010130: 2020 2073 6261 7463 685f 636d 6420 3d20     sbatch_cmd = 
+00010140: 6622 7362 6174 6368 7b6a 6f62 5f70 6172  f"sbatch{job_par
+00010150: 616d 7d20 2d2d 6f75 7470 7574 3d6f 6d65  am} --output=ome
+00010160: 726f 2d25 6a2e 6c6f 6720 5c0a 2020 2020  ro-%j.log \.    
+00010170: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
+00010180: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
+00010190: 2f7b 6a6f 625f 7363 7269 7074 7d22 0a0a  /{job_script}"..
+000101a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000101b0: 6261 7463 685f 636d 642c 2065 6e76 0a0a  batch_cmd, env..
+000101c0: 2020 2020 6465 6620 6765 745f 636f 6e76      def get_conv
+000101d0: 6572 7369 6f6e 5f63 6f6d 6d61 6e64 2873  ersion_command(s
+000101e0: 656c 662c 2064 6174 615f 7061 7468 3a20  elf, data_path: 
+000101f0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010210: 2020 2020 636f 6e66 6967 5f66 696c 653a      config_file:
+00010220: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 2020 2020 2073 6f75 7263 655f 666f 726d       source_form
+00010250: 6174 3a20 7374 7220 3d20 277a 6172 7227  at: str = 'zarr'
+00010260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010280: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
+00010290: 7374 7220 3d20 2774 6966 6627 2920 2d3e  str = 'tiff') ->
+000102a0: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
+000102b0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+000102c0: 2020 2020 2020 2047 656e 6572 6174 6520         Generate 
+000102d0: 536c 7572 6d20 636f 6e76 6572 7369 6f6e  Slurm conversion
+000102e0: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
+000102f0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00010300: 6573 2066 6f72 2064 6174 6120 636f 6e76  es for data conv
+00010310: 6572 7369 6f6e 2e0a 0a20 2020 2020 2020  ersion...       
+00010320: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00010330: 2020 2064 6174 615f 7061 7468 2028 7374     data_path (st
+00010340: 7229 3a20 5061 7468 2074 6f20 7468 6520  r): Path to the 
+00010350: 6461 7461 2066 6f6c 6465 722e 0a20 2020  data folder..   
+00010360: 2020 2020 2020 2020 2063 6f6e 6669 675f           config_
+00010370: 6669 6c65 2028 7374 7229 3a20 5061 7468  file (str): Path
+00010380: 2074 6f20 7468 6520 636f 6e66 6967 7572   to the configur
+00010390: 6174 696f 6e20 6669 6c65 2e0a 2020 2020  ation file..    
+000103a0: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
+000103b0: 6f72 6d61 7420 2873 7472 293a 2053 6f75  ormat (str): Sou
+000103c0: 7263 6520 6461 7461 2066 6f72 6d61 7420  rce data format 
+000103d0: 2864 6566 6175 6c74 2069 7320 277a 6172  (default is 'zar
+000103e0: 7227 292e 0a20 2020 2020 2020 2020 2020  r')..           
+000103f0: 2074 6172 6765 745f 666f 726d 6174 2028   target_format (
+00010400: 7374 7229 3a20 5461 7267 6574 2064 6174  str): Target dat
+00010410: 6120 666f 726d 6174 2028 6465 6661 756c  a format (defaul
+00010420: 7420 6973 2027 7469 6666 2729 2e0a 0a20  t is 'tiff')... 
+00010430: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00010440: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+00010450: 655b 7374 722c 2044 6963 745d 3a0a 2020  e[str, Dict]:.  
+00010460: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+00010470: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+00010480: 2074 6865 2053 6c75 726d 2063 6f6e 7665   the Slurm conve
+00010490: 7273 696f 6e20 636f 6d6d 616e 6420 616e  rsion command an
+000104a0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000104b0: 2020 7468 6520 656e 7669 726f 6e6d 656e    the environmen
+000104c0: 7420 7661 7269 6162 6c65 732e 0a0a 2020  t variables...  
+000104d0: 2020 2020 2020 5761 726e 696e 673a 0a20        Warning:. 
+000104e0: 2020 2020 2020 2020 2020 2054 6865 2064             The d
+000104f0: 6566 6175 6c74 2069 6d70 6c65 6d65 6e74  efault implement
+00010500: 6174 696f 6e20 6f6e 6c79 2073 7570 706f  ation only suppo
+00010510: 7274 7320 636f 6e76 6572 7369 6f6e 2066  rts conversion f
+00010520: 726f 6d20 277a 6172 7227 2074 6f20 2774  rom 'zarr' to 't
+00010530: 6966 6627 2e0a 2020 2020 2020 2020 2020  iff'..          
+00010540: 2020 4966 2075 7369 6e67 206f 7468 6572    If using other
+00010550: 2073 6f75 7263 6520 6f72 2074 6172 6765   source or targe
+00010560: 7420 666f 726d 6174 732c 2075 7365 7273  t formats, users
+00010570: 206d 7573 7420 696d 706c 656d 656e 7420   must implement 
+00010580: 616e 6420 636f 6e66 6967 7572 650a 2020  and configure.  
+00010590: 2020 2020 2020 2020 2020 6164 6469 7469            additi
+000105a0: 6f6e 616c 2063 6f6e 7665 7274 6572 7320  onal converters 
+000105b0: 7468 656d 7365 6c76 6573 2e0a 2020 2020  themselves..    
+000105c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000105d0: 6966 2073 6f75 7263 655f 666f 726d 6174  if source_format
+000105e0: 2021 3d20 227a 6172 7222 206f 7220 7461   != "zarr" or ta
+000105f0: 7267 6574 5f66 6f72 6d61 7420 213d 2022  rget_format != "
+00010600: 7469 6666 223a 0a20 2020 2020 2020 2020  tiff":.         
+00010610: 2020 2023 2057 6172 6e20 6162 6f75 7420     # Warn about 
+00010620: 756e 7375 7070 6f72 7465 6420 636f 6e76  unsupported conv
+00010630: 6572 7369 6f6e 3b20 6164 6469 7469 6f6e  ersion; addition
+00010640: 616c 2063 6f6e 7665 7274 6572 7320 6361  al converters ca
+00010650: 6e20 6265 0a20 2020 2020 2020 2020 2020  n be.           
+00010660: 2023 2061 6464 6564 206f 7574 7369 6465   # added outside
+00010670: 206f 7572 206b 6e6f 776c 6564 6765 2e0a   our knowledge..
+00010680: 2020 2020 2020 2020 2020 2020 2320 4368              # Ch
+00010690: 6563 6b69 6e67 2053 6c75 726d 2773 2060  ecking Slurm's `
+000106a0: 736c 7572 6d5f 636f 6e76 6572 7465 7273  slurm_converters
+000106b0: 5f70 6174 6860 2069 7320 736b 6970 7065  _path` is skippe
+000106c0: 6420 666f 720a 2020 2020 2020 2020 2020  d for.          
+000106d0: 2020 2320 7065 7266 6f72 6d61 6e63 6520    # performance 
+000106e0: 7265 6173 6f6e 732e 0a20 2020 2020 2020  reasons..       
+000106f0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+00010700: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00010710: 2020 2020 2066 2243 6f6e 7665 7273 696f       f"Conversio
+00010720: 6e20 6672 6f6d 207b 736f 7572 6365 5f66  n from {source_f
+00010730: 6f72 6d61 747d 2074 6f20 7b74 6172 6765  ormat} to {targe
+00010740: 745f 666f 726d 6174 7d20 6973 206e 6f74  t_format} is not
+00010750: 2073 7570 706f 7274 6564 2062 7920 6465   supported by de
+00010760: 6661 756c 7421 2229 0a0a 2020 2020 2020  fault!")..      
+00010770: 2020 6368 6f73 656e 5f63 6f6e 7665 7274    chosen_convert
+00010780: 6572 203d 2066 2263 6f6e 7665 7274 5f7b  er = f"convert_{
+00010790: 736f 7572 6365 5f66 6f72 6d61 747d 5f74  source_format}_t
+000107a0: 6f5f 7b74 6172 6765 745f 666f 726d 6174  o_{target_format
+000107b0: 7d2e 7369 6622 0a20 2020 2020 2020 2073  }.sif".        s
+000107c0: 6261 7463 685f 656e 7620 3d20 7b0a 2020  batch_env = {.  
+000107d0: 2020 2020 2020 2020 2020 2244 4154 415f            "DATA_
+000107e0: 5041 5448 223a 2066 227b 6461 7461 5f70  PATH": f"{data_p
+000107f0: 6174 687d 222c 0a20 2020 2020 2020 2020  ath}",.         
+00010800: 2020 2022 434f 4e56 4552 5349 4f4e 5f50     "CONVERSION_P
+00010810: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
+00010820: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
+00010830: 6174 687d 222c 0a20 2020 2020 2020 2020  ath}",.         
+00010840: 2020 2022 434f 4e56 4552 5445 525f 494d     "CONVERTER_IM
+00010850: 4147 4522 3a20 6368 6f73 656e 5f63 6f6e  AGE": chosen_con
+00010860: 7665 7274 6572 2c0a 2020 2020 2020 2020  verter,.        
+00010870: 2020 2020 2253 4352 4950 545f 5041 5448      "SCRIPT_PATH
+00010880: 223a 2066 227b 7365 6c66 2e73 6c75 726d  ": f"{self.slurm
+00010890: 5f73 6372 6970 745f 7061 7468 7d22 2c0a  _script_path}",.
+000108a0: 2020 2020 2020 2020 2020 2020 2243 4f4e              "CON
+000108b0: 4649 475f 4649 4c45 223a 2066 227b 636f  FIG_FILE": f"{co
+000108c0: 6e66 6967 5f66 696c 657d 220a 2020 2020  nfig_file}".    
+000108d0: 2020 2020 7d0a 0a20 2020 2020 2020 2063      }..        c
+000108e0: 6f6e 7665 7273 696f 6e5f 636d 6420 3d20  onversion_cmd = 
+000108f0: 2273 6261 7463 6820 2d2d 6a6f 622d 6e61  "sbatch --job-na
+00010900: 6d65 3d63 6f6e 7665 7273 696f 6e20 2d2d  me=conversion --
+00010910: 6578 706f 7274 3d41 4c4c 2c43 4f4e 4649  export=ALL,CONFI
+00010920: 475f 5041 5448 3d5c 2224 5057 442f 2443  G_PATH=\"$PWD/$C
+00010930: 4f4e 4649 475f 4649 4c45 5c22 202d 2d61  ONFIG_FILE\" --a
+00010940: 7272 6179 3d31 2d24 4e20 2453 4352 4950  rray=1-$N $SCRIP
+00010950: 545f 5041 5448 2f63 6f6e 7665 7274 5f6a  T_PATH/convert_j
+00010960: 6f62 5f61 7272 6179 2e73 6822 0a20 2020  ob_array.sh".   
+00010970: 2020 2020 2023 2063 6f6e 7665 7273 696f       # conversio
+00010980: 6e5f 636d 645f 7761 6974 696e 6720 3d20  n_cmd_waiting = 
+00010990: 2273 6261 7463 6820 2d2d 6a6f 622d 6e61  "sbatch --job-na
+000109a0: 6d65 3d63 6f6e 7665 7273 696f 6e20 2d2d  me=conversion --
+000109b0: 6578 706f 7274 3d41 4c4c 2c43 4f4e 4649  export=ALL,CONFI
+000109c0: 475f 5041 5448 3d5c 2224 5057 442f 2443  G_PATH=\"$PWD/$C
+000109d0: 4f4e 4649 475f 4649 4c45 5c22 202d 2d61  ONFIG_FILE\" --a
+000109e0: 7272 6179 3d31 2d24 4e20 2d2d 7761 6974  rray=1-$N --wait
+000109f0: 2024 5343 5249 5054 5f50 4154 482f 636f   $SCRIPT_PATH/co
+00010a00: 6e76 6572 745f 6a6f 625f 6172 7261 792e  nvert_job_array.
+00010a10: 7368 220a 0a20 2020 2020 2020 2072 6574  sh"..        ret
+00010a20: 7572 6e20 636f 6e76 6572 7369 6f6e 5f63  urn conversion_c
+00010a30: 6d64 2c20 7362 6174 6368 5f65 6e76 0a0a  md, sbatch_env..
+00010a40: 2020 2020 6465 6620 776f 726b 666c 6f77      def workflow
+00010a50: 5f70 6172 616d 735f 746f 5f65 6e76 7661  _params_to_envva
+00010a60: 7273 2873 656c 662c 202a 2a6b 7761 7267  rs(self, **kwarg
+00010a70: 7329 202d 3e20 4469 6374 3a0a 2020 2020  s) -> Dict:.    
+00010a80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010a90: 436f 6e76 6572 7420 776f 726b 666c 6f77  Convert workflow
+00010aa0: 2070 6172 616d 6574 6572 7320 746f 2065   parameters to e
+00010ab0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00010ac0: 626c 6573 2e0a 0a20 2020 2020 2020 2041  bles...        A
+00010ad0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010ae0: 202a 2a6b 7761 7267 733a 2041 6464 6974   **kwargs: Addit
+00010af0: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
+00010b00: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
+00010b10: 776f 726b 666c 6f77 2e0a 0a20 2020 2020  workflow...     
+00010b20: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00010b30: 2020 2020 2020 2020 4469 6374 3a20 4120          Dict: A 
+00010b40: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+00010b50: 696e 696e 6720 7468 6520 656e 7669 726f  ining the enviro
+00010b60: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
+00010b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010b80: 2020 2020 2077 6f72 6b66 6c6f 775f 656e       workflow_en
+00010b90: 7620 3d20 7b6b 6579 2e75 7070 6572 2829  v = {key.upper()
+00010ba0: 3a20 6622 7b76 616c 7565 7d22 2066 6f72  : f"{value}" for
+00010bb0: 206b 6579 2c0a 2020 2020 2020 2020 2020   key,.          
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00010bd0: 6c75 6520 696e 206b 7761 7267 732e 6974  lue in kwargs.it
+00010be0: 656d 7328 297d 0a20 2020 2020 2020 206c  ems()}.        l
+00010bf0: 6f67 6765 722e 6465 6275 6728 776f 726b  ogger.debug(work
+00010c00: 666c 6f77 5f65 6e76 290a 2020 2020 2020  flow_env).      
+00010c10: 2020 7265 7475 726e 2077 6f72 6b66 6c6f    return workflo
+00010c20: 775f 656e 760a 0a20 2020 2064 6566 2067  w_env..    def g
+00010c30: 6574 5f63 656c 6c70 6f73 655f 636f 6d6d  et_cellpose_comm
+00010c40: 616e 6428 7365 6c66 2c20 696d 6167 655f  and(self, image_
+00010c50: 7665 7273 696f 6e3a 2073 7472 2c0a 2020  version: str,.  
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c70: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00010c80: 5f64 6174 613a 2073 7472 2c0a 2020 2020  _data: str,.    
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 2020 2063 705f 6d6f 6465           cp_mode
+00010cb0: 6c3a 2073 7472 2c0a 2020 2020 2020 2020  l: str,.        
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 2020 2020 206e 7563 5f63 6861 6e6e 656c       nuc_channel
+00010ce0: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d00: 2020 2020 7072 6f62 5f74 6872 6573 686f      prob_thresho
+00010d10: 6c64 3a20 666c 6f61 742c 0a20 2020 2020  ld: float,.     
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d30: 2020 2020 2020 2020 6365 6c6c 5f64 6961          cell_dia
+00010d40: 6d65 7465 723a 2066 6c6f 6174 2c0a 2020  meter: float,.  
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+00010d70: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00010d80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2074 696d 653a 204f 7074 696f       time: Optio
+00010db0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dd0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00010de0: 655f 6770 753a 2062 6f6f 6c20 3d20 5472  e_gpu: bool = Tr
+00010df0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e10: 206d 6f64 656c 3a20 7374 7220 3d20 2263   model: str = "c
+00010e20: 656c 6c70 6f73 6522 2920 2d3e 2054 7570  ellpose") -> Tup
+00010e30: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
+00010e40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010e50: 2020 2052 6574 7572 6e20 7468 6520 636f     Return the co
+00010e60: 6d6d 616e 6420 616e 6420 656e 7669 726f  mmand and enviro
+00010e70: 6e6d 656e 7420 6469 6374 696f 6e61 7279  nment dictionary
+00010e80: 2074 6f20 7275 6e20 6120 4365 6c6c 506f   to run a CellPo
+00010e90: 7365 206a 6f62 0a20 2020 2020 2020 206f  se job.        o
+00010ea0: 6e20 7468 6520 536c 7572 6d20 776f 726b  n the Slurm work
+00010eb0: 6c6f 6164 206d 616e 6167 6572 2e0a 2020  load manager..  
+00010ec0: 2020 2020 2020 4120 7370 6563 6966 6963        A specific
+00010ed0: 2065 7861 6d70 6c65 206f 6620 7573 696e   example of usin
+00010ee0: 6720 7468 6520 6765 6e65 7269 6320 2767  g the generic 'g
+00010ef0: 6574 5f77 6f72 6b66 6c6f 775f 636f 6d6d  et_workflow_comm
+00010f00: 616e 6427 2e0a 0a20 2020 2020 2020 2041  and'...        A
+00010f10: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010f20: 2069 6d61 6765 5f76 6572 7369 6f6e 2028   image_version (
+00010f30: 7374 7229 3a20 5468 6520 7665 7273 696f  str): The versio
+00010f40: 6e20 6f66 2074 6865 2053 696e 6775 6c61  n of the Singula
+00010f50: 7269 7479 2069 6d61 6765 2074 6f20 7573  rity image to us
+00010f60: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00010f70: 6e70 7574 5f64 6174 6120 2873 7472 293a  nput_data (str):
+00010f80: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00010f90: 2069 6e70 7574 2064 6174 6120 666f 6c64   input data fold
+00010fa0: 6572 206f 6e20 7468 6520 7368 6172 6564  er on the shared
+00010fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010fc0: 2066 696c 6520 7379 7374 656d 2e0a 2020   file system..  
+00010fd0: 2020 2020 2020 2020 2020 6370 5f6d 6f64            cp_mod
+00010fe0: 656c 2028 7374 7229 3a20 5468 6520 6e61  el (str): The na
+00010ff0: 6d65 206f 6620 7468 6520 4365 6c6c 506f  me of the CellPo
+00011000: 7365 206d 6f64 656c 2074 6f20 7573 652e  se model to use.
+00011010: 0a20 2020 2020 2020 2020 2020 206e 7563  .            nuc
+00011020: 5f63 6861 6e6e 656c 2028 696e 7429 3a20  _channel (int): 
+00011030: 5468 6520 696e 6465 7820 6f66 2074 6865  The index of the
+00011040: 206e 7563 6c65 6172 2063 6861 6e6e 656c   nuclear channel
+00011050: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00011060: 6f62 5f74 6872 6573 686f 6c64 2028 666c  ob_threshold (fl
+00011070: 6f61 7429 3a20 5468 6520 7072 6f62 6162  oat): The probab
+00011080: 696c 6974 7920 7468 7265 7368 6f6c 6420  ility threshold 
+00011090: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+000110a0: 2020 2020 6e75 636c 6569 2064 6574 6563      nuclei detec
+000110b0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+000110c0: 2020 6365 6c6c 5f64 6961 6d65 7465 7220    cell_diameter 
+000110d0: 2866 6c6f 6174 293a 2054 6865 2065 7870  (float): The exp
+000110e0: 6563 7465 6420 6365 6c6c 2064 6961 6d65  ected cell diame
+000110f0: 7465 7220 696e 2070 6978 656c 732e 0a20  ter in pixels.. 
+00011100: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+00011110: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
+00011120: 3a20 5468 6520 656d 6169 6c20 6164 6472  : The email addr
+00011130: 6573 7320 746f 2073 656e 6420 6e6f 7469  ess to send noti
+00011140: 6669 6361 7469 6f6e 7320 746f 2e0a 2020  fications to..  
+00011150: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00011160: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+00011170: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00011180: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
+00011190: 3a20 5468 6520 6d61 7869 6d75 6d20 7469  : The maximum ti
+000111a0: 6d65 2066 6f72 2074 6865 206a 6f62 2074  me for the job t
+000111b0: 6f20 7275 6e2e 0a20 2020 2020 2020 2020  o run..         
+000111c0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+000111d0: 746f 204e 6f6e 652e 0a20 2020 2020 2020  to None..       
+000111e0: 2020 2020 2075 7365 5f67 7075 2028 626f       use_gpu (bo
+000111f0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00011200: 7573 6520 4750 5520 666f 7220 7468 6520  use GPU for the 
+00011210: 4365 6c6c 506f 7365 206a 6f62 2e0a 2020  CellPose job..  
+00011220: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00011230: 6661 756c 7473 2074 6f20 5472 7565 2e0a  faults to True..
+00011240: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00011250: 6c20 2873 7472 293a 2054 6865 206e 616d  l (str): The nam
+00011260: 6520 6f66 2074 6865 2066 6f6c 6465 7220  e of the folder 
+00011270: 6f66 2074 6865 2044 6f63 6b65 7220 696d  of the Docker im
+00011280: 6167 6520 746f 2075 7365 2e0a 2020 2020  age to use..    
+00011290: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+000112a0: 756c 7473 2074 6f20 2263 656c 6c70 6f73  ults to "cellpos
+000112b0: 6522 2e0a 0a20 2020 2020 2020 2052 6574  e"...        Ret
+000112c0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000112d0: 2020 5475 706c 655b 7374 722c 2064 6963    Tuple[str, dic
+000112e0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+000112f0: 2020 2020 4120 7475 706c 6520 636f 6e74      A tuple cont
+00011300: 6169 6e69 6e67 2074 6865 2053 6c75 726d  aining the Slurm
+00011310: 2073 6261 7463 6820 636f 6d6d 616e 640a   sbatch command.
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 616e 6420 7468 6520 656e 7669 726f 6e6d  and the environm
+00011340: 656e 7420 6469 6374 696f 6e61 7279 2e0a  ent dictionary..
+00011350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011360: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00011370: 6765 745f 776f 726b 666c 6f77 5f63 6f6d  get_workflow_com
+00011380: 6d61 6e64 2877 6f72 6b66 6c6f 773d 6d6f  mand(workflow=mo
+00011390: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+000113c0: 726b 666c 6f77 5f76 6572 7369 6f6e 3d69  rkflow_version=i
+000113d0: 6d61 6765 5f76 6572 7369 6f6e 2c0a 2020  mage_version,.  
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+00011410: 613d 696e 7075 745f 6461 7461 2c0a 2020  a=input_data,.  
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2065 6d61 696c 3d65 6d61         email=ema
+00011450: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+00011480: 653d 7469 6d65 2c0a 2020 2020 2020 2020  e=time,.        
+00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2063 705f 6d6f 6465 6c3d 6370 5f6d 6f64   cp_model=cp_mod
+000114c0: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2020 2020 2020 2020 2020 206e 7563               nuc
+000114f0: 5f63 6861 6e6e 656c 3d6e 7563 5f63 6861  _channel=nuc_cha
+00011500: 6e6e 656c 2c0a 2020 2020 2020 2020 2020  nnel,.          
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00011530: 726f 625f 7468 7265 7368 6f6c 643d 7072  rob_threshold=pr
+00011540: 6f62 5f74 6872 6573 686f 6c64 2c0a 2020  ob_threshold,.  
+00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2063 656c 6c5f 6469 616d         cell_diam
+00011580: 6574 6572 3d63 656c 6c5f 6469 616d 6574  eter=cell_diamet
+00011590: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+000115c0: 5f67 7075 3d75 7365 5f67 7075 290a 0a20  _gpu=use_gpu).. 
+000115d0: 2020 2064 6566 2063 6f70 795f 7a69 705f     def copy_zip_
+000115e0: 6c6f 6361 6c6c 7928 7365 6c66 2c20 6c6f  locally(self, lo
+000115f0: 6361 6c5f 746d 705f 7374 6f72 6167 653a  cal_tmp_storage:
+00011600: 2073 7472 2c20 6669 6c65 6e61 6d65 3a20   str, filename: 
+00011610: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00011620: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00011630: 3e20 5472 616e 7366 6572 5265 7375 6c74  > TransferResult
+00011640: 3a0a 2020 2020 2020 2020 2222 2220 436f  :.        """ Co
+00011650: 7079 2061 207a 6970 2066 696c 6520 6672  py a zip file fr
+00011660: 6f6d 2053 6c75 726d 2074 6f20 7468 6520  om Slurm to the 
+00011670: 6c6f 6361 6c20 7365 7276 6572 2e0a 0a20  local server... 
+00011680: 2020 2020 2020 204e 6f74 6520 6162 6f75         Note abou
+00011690: 7420 2854 7261 6e73 6665 7229 5265 7375  t (Transfer)Resu
+000116a0: 6c74 3a0a 0a20 2020 2020 2020 2055 6e6c  lt:..        Unl
+000116b0: 696b 6520 7369 6d69 6c61 7220 636c 6173  ike similar clas
+000116c0: 7365 7320 7375 6368 2061 7320 696e 766f  ses such as invo
+000116d0: 6b65 2e72 756e 6e65 7273 2e52 6573 756c  ke.runners.Resul
+000116e0: 7420 6f72 0a20 2020 2020 2020 2066 6162  t or.        fab
+000116f0: 7269 632e 7275 6e6e 6572 732e 5265 7375  ric.runners.Resu
+00011700: 6c74 0a20 2020 2020 2020 2028 7768 6963  lt.        (whic
+00011710: 6820 6861 7665 2061 2063 6f6e 6365 7074  h have a concept
+00011720: 206f 6620 e280 9c77 6172 6e20 616e 6420   of ...warn and 
+00011730: 7265 7475 726e 2061 6e79 7761 7973 206f  return anyways o
+00011740: 6e20 6661 696c 7572 65e2 809d 290a 2020  n failure...).  
+00011750: 2020 2020 2020 7468 6973 2063 6c61 7373        this class
+00011760: 2068 6173 206e 6f20 7573 6566 756c 2074   has no useful t
+00011770: 7275 7468 696e 6573 7320 6265 6861 7669  ruthiness behavi
+00011780: 6f72 2e0a 2020 2020 2020 2020 4966 2061  or..        If a
+00011790: 2066 696c 6520 7472 616e 7366 6572 2066   file transfer f
+000117a0: 6169 6c73 2c20 736f 6d65 2065 7863 6570  ails, some excep
+000117b0: 7469 6f6e 2077 696c 6c20 6265 2072 6169  tion will be rai
+000117c0: 7365 642c 0a20 2020 2020 2020 2065 6974  sed,.        eit
+000117d0: 6865 7220 616e 204f 5345 7272 6f72 206f  her an OSError o
+000117e0: 7220 616e 2065 7272 6f72 2066 726f 6d20  r an error from 
+000117f0: 7769 7468 696e 2050 6172 616d 696b 6f2e  within Paramiko.
+00011800: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00011810: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00011820: 6c5f 746d 705f 7374 6f72 6167 6520 2853  l_tmp_storage (S
+00011830: 7472 696e 6729 3a20 5061 7468 2074 6f20  tring): Path to 
+00011840: 7374 6f72 6520 7468 6520 7a69 7020 6669  store the zip fi
+00011850: 6c65 206c 6f63 616c 6c79 2e0a 2020 2020  le locally..    
+00011860: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+00011870: 2028 5374 7269 6e67 293a 205a 6970 2066   (String): Zip f
+00011880: 696c 656e 616d 6520 6f6e 2053 6c75 726d  ilename on Slurm
+00011890: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000118a0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000118b0: 5472 616e 7366 6572 5265 7375 6c74 3a20  TransferResult: 
+000118c0: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
+000118d0: 6520 7363 7020 6174 7465 6d70 742e 0a20  e scp attempt.. 
+000118e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000118f0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00011900: 2243 6f70 7969 6e67 207a 6970 207b 6669  "Copying zip {fi
+00011910: 6c65 6e61 6d65 7d20 6672 6f6d 5c0a 2020  lename} from\.  
+00011920: 2020 2020 2020 2020 2020 536c 7572 6d20            Slurm 
+00011930: 746f 207b 6c6f 6361 6c5f 746d 705f 7374  to {local_tmp_st
+00011940: 6f72 6167 657d 2229 0a20 2020 2020 2020  orage}").       
+00011950: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+00011960: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00011970: 6d6f 7465 3d66 227b 6669 6c65 6e61 6d65  mote=f"{filename
+00011980: 7d2e 7a69 7022 2c0a 2020 2020 2020 2020  }.zip",.        
+00011990: 2020 2020 6c6f 6361 6c3d 6c6f 6361 6c5f      local=local_
+000119a0: 746d 705f 7374 6f72 6167 6529 0a0a 2020  tmp_storage)..  
+000119b0: 2020 6465 6620 7a69 705f 6461 7461 5f6f    def zip_data_o
+000119c0: 6e5f 736c 7572 6d5f 7365 7276 6572 2873  n_slurm_server(s
+000119d0: 656c 662c 2064 6174 615f 6c6f 6361 7469  elf, data_locati
+000119e0: 6f6e 3a20 7374 722c 2066 696c 656e 616d  on: str, filenam
+000119f0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
+00011a20: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00011a30: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00011a60: 202d 3e20 5265 7375 6c74 3a0a 2020 2020   -> Result:.    
+00011a70: 2020 2020 2222 225a 6970 2074 6865 206f      """Zip the o
+00011a80: 7574 7075 7420 666f 6c64 6572 206f 6620  utput folder of 
+00011a90: 6120 6a6f 6220 6f6e 2053 6c75 726d 0a0a  a job on Slurm..
+00011aa0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00011ab0: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
+00011ac0: 6f63 6174 696f 6e20 2853 7472 696e 6729  ocation (String)
+00011ad0: 3a20 466f 6c64 6572 206f 6e20 534c 5552  : Folder on SLUR
+00011ae0: 4d20 7769 7468 2074 6865 2022 6461 7461  M with the "data
+00011af0: 2f6f 7574 220a 2020 2020 2020 2020 2020  /out".          
+00011b00: 2020 2020 2020 7375 6266 6f6c 6465 722e        subfolder.
+00011b10: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00011b20: 656e 616d 6520 2853 7472 696e 6729 3a20  ename (String): 
+00011b30: 4e61 6d65 2074 6f20 6769 7665 2074 6f20  Name to give to 
+00011b40: 7468 6520 7a69 7066 696c 652e 0a20 2020  the zipfile..   
+00011b50: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+00011b60: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+00011b70: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+00011b80: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+00011b90: 7269 6162 6c65 7320 746f 200a 2020 2020  riables to .    
+00011ba0: 2020 2020 2020 2020 2020 2020 7365 7420              set 
+00011bb0: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
+00011bc0: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
+00011bd0: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
+00011be0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00011bf0: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
+00011c00: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
+00011c10: 7468 6520 7a69 7020 6174 7465 6d70 742e  the zip attempt.
+00011c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011c30: 2020 2020 2023 207a 6970 0a20 2020 2020       # zip.     
+00011c40: 2020 207a 6970 5f63 6d64 203d 2073 656c     zip_cmd = sel
+00011c50: 662e 6765 745f 7a69 705f 636f 6d6d 616e  f.get_zip_comman
+00011c60: 6428 6461 7461 5f6c 6f63 6174 696f 6e2c  d(data_location,
+00011c70: 2066 696c 656e 616d 6529 0a20 2020 2020   filename).     
+00011c80: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00011c90: 225a 6970 7069 6e67 207b 6461 7461 5f6c  "Zipping {data_l
+00011ca0: 6f63 6174 696f 6e7d 2061 7320 7b66 696c  ocation} as {fil
+00011cb0: 656e 616d 657d 206f 6e20 536c 7572 6d22  ename} on Slurm"
+00011cc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00011cd0: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00011ce0: 6473 285b 7a69 705f 636d 645d 2c20 656e  ds([zip_cmd], en
+00011cf0: 763d 656e 7629 0a0a 2020 2020 6465 6620  v=env)..    def 
+00011d00: 6765 745f 7a69 705f 636f 6d6d 616e 6428  get_zip_command(
+00011d10: 7365 6c66 2c20 6461 7461 5f6c 6f63 6174  self, data_locat
+00011d20: 696f 6e3a 2073 7472 2c20 6669 6c65 6e61  ion: str, filena
+00011d30: 6d65 3a20 7374 7229 202d 3e20 7374 723a  me: str) -> str:
+00011d40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011d50: 2020 2020 2047 656e 6572 6174 6520 6120       Generate a 
+00011d60: 636f 6d6d 616e 6420 7374 7269 6e67 2066  command string f
+00011d70: 6f72 207a 6970 7069 6e67 2074 6865 2064  or zipping the d
+00011d80: 6174 6120 6f6e 2053 6c75 726d 2e0a 0a20  ata on Slurm... 
+00011d90: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00011da0: 2020 2020 2020 2020 2064 6174 615f 6c6f           data_lo
+00011db0: 6361 7469 6f6e 2028 7374 7229 3a20 5468  cation (str): Th
+00011dc0: 6520 666f 6c64 6572 2074 6f20 6265 207a  e folder to be z
+00011dd0: 6970 7065 642e 0a20 2020 2020 2020 2020  ipped..         
+00011de0: 2020 2066 696c 656e 616d 6520 2873 7472     filename (str
+00011df0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+00011e00: 6865 207a 6970 2061 7263 6869 7665 2066  he zip archive f
+00011e10: 696c 6520 746f 2065 7874 7261 6374 2e0a  ile to extract..
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e30: 5769 7468 6f75 7420 6578 7465 6e73 696f  Without extensio
+00011e40: 6e2e 0a0a 2020 2020 2020 2020 5265 7475  n...        Retu
+00011e50: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00011e60: 2073 7472 3a20 5468 6520 636f 6d6d 616e   str: The comman
+00011e70: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
+00011e80: 7a69 7020 6669 6c65 2e0a 2020 2020 2020  zip file..      
+00011e90: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00011ea0: 7475 726e 2073 656c 662e 5f5a 4950 5f43  turn self._ZIP_C
+00011eb0: 4d44 2e66 6f72 6d61 7428 6669 6c65 6e61  MD.format(filena
+00011ec0: 6d65 3d66 696c 656e 616d 652c 0a20 2020  me=filename,.   
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ef0: 2064 6174 615f 6c6f 6361 7469 6f6e 3d64   data_location=d
+00011f00: 6174 615f 6c6f 6361 7469 6f6e 290a 0a20  ata_location).. 
+00011f10: 2020 2064 6566 2067 6574 5f6c 6f67 6669     def get_logfi
+00011f20: 6c65 5f66 726f 6d5f 736c 7572 6d28 7365  le_from_slurm(se
+00011f30: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2020 2073 6c75 726d 5f6a 6f62 5f69 643a     slurm_job_id:
+00011f60: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 2020 2020 206c 6f63 616c 5f74 6d70 5f73       local_tmp_s
+00011f90: 746f 7261 6765 3a20 7374 7220 3d20 222f  torage: str = "/
+00011fa0: 746d 702f 222c 0a20 2020 2020 2020 2020  tmp/",.         
+00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2020 6c6f 6766 696c 653a 2073        logfile: s
+00011fd0: 7472 203d 204e 6f6e 650a 2020 2020 2020  tr = None.      
+00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ff0: 2020 2020 2020 2020 2029 202d 3e20 5475           ) -> Tu
+00012000: 706c 655b 7374 722c 2073 7472 2c20 5472  ple[str, str, Tr
+00012010: 616e 7366 6572 5265 7375 6c74 5d3a 0a20  ansferResult]:. 
+00012020: 2020 2020 2020 2022 2222 436f 7079 2074         """Copy t
+00012030: 6865 206c 6f67 6669 6c65 206f 6620 7468  he logfile of th
+00012040: 6520 6769 7665 6e20 534c 5552 4d20 6a6f  e given SLURM jo
+00012050: 6220 746f 2074 6865 206c 6f63 616c 2073  b to the local s
+00012060: 6572 7665 722e 0a0a 2020 2020 2020 2020  erver...        
+00012070: 4e6f 7465 2061 626f 7574 2028 5472 616e  Note about (Tran
+00012080: 7366 6572 2952 6573 756c 743a 0a0a 2020  sfer)Result:..  
+00012090: 2020 2020 2020 556e 6c69 6b65 2073 696d        Unlike sim
+000120a0: 696c 6172 2063 6c61 7373 6573 2073 7563  ilar classes suc
+000120b0: 6820 6173 2069 6e76 6f6b 652e 7275 6e6e  h as invoke.runn
+000120c0: 6572 732e 5265 7375 6c74 0a20 2020 2020  ers.Result.     
+000120d0: 2020 206f 7220 6661 6272 6963 2e72 756e     or fabric.run
+000120e0: 6e65 7273 2e52 6573 756c 740a 2020 2020  ners.Result.    
+000120f0: 2020 2020 2877 6869 6368 2068 6176 6520      (which have 
+00012100: 6120 636f 6e63 6570 7420 6f66 20e2 809c  a concept of ...
+00012110: 7761 726e 2061 6e64 2072 6574 7572 6e20  warn and return 
+00012120: 616e 7977 6179 7320 6f6e 2066 6169 6c75  anyways on failu
+00012130: 7265 e280 9d29 0a20 2020 2020 2020 2074  re...).        t
+00012140: 6869 7320 636c 6173 7320 6861 7320 6e6f  his class has no
+00012150: 2075 7365 6675 6c20 7472 7574 6869 6e65   useful truthine
+00012160: 7373 2062 6568 6176 696f 722e 0a20 2020  ss behavior..   
+00012170: 2020 2020 2049 6620 6120 6669 6c65 2074       If a file t
+00012180: 7261 6e73 6665 7220 6661 696c 732c 2073  ransfer fails, s
+00012190: 6f6d 6520 6578 6365 7074 696f 6e20 7769  ome exception wi
+000121a0: 6c6c 2062 6520 7261 6973 6564 2c0a 2020  ll be raised,.  
+000121b0: 2020 2020 2020 6569 7468 6572 2061 6e20        either an 
+000121c0: 4f53 4572 726f 7220 6f72 2061 6e20 6572  OSError or an er
+000121d0: 726f 7220 6672 6f6d 2077 6974 6869 6e20  ror from within 
+000121e0: 5061 7261 6d69 6b6f 2e0a 0a20 2020 2020  Paramiko...     
+000121f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012200: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+00012210: 6420 2873 7472 293a 2054 6865 2049 4420  d (str): The ID 
+00012220: 6f66 2074 6865 2053 4c55 524d 206a 6f62  of the SLURM job
+00012230: 2e0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00012240: 6361 6c5f 746d 705f 7374 6f72 6167 6520  cal_tmp_storage 
+00012250: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00012260: 2050 6174 6820 746f 2073 746f 7265 2074   Path to store t
+00012270: 6865 206c 6f67 6669 6c65 200a 2020 2020  he logfile .    
+00012280: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00012290: 6c6c 792e 2044 6566 6175 6c74 7320 746f  lly. Defaults to
+000122a0: 2022 2f74 6d70 2f22 2e0a 2020 2020 2020   "/tmp/"..      
+000122b0: 2020 2020 2020 6c6f 6766 696c 6520 2873        logfile (s
+000122c0: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
+000122d0: 6174 6820 746f 2074 6865 206c 6f67 6669  ath to the logfi
+000122e0: 6c65 206f 6e20 7468 6520 534c 5552 4d20  le on the SLURM 
+000122f0: 7365 7276 6572 2e0a 2020 2020 2020 2020  server..        
+00012300: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00012310: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
+00012320: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00012330: 2020 2020 2020 2020 5475 706c 653a 2064          Tuple: d
+00012340: 6972 6563 746f 7279 2c20 6675 6c6c 2070  irectory, full p
+00012350: 6174 6820 6f66 2074 6865 206c 6f67 6669  ath of the logfi
+00012360: 6c65 2c20 616e 6420 5472 616e 7366 6572  le, and Transfer
+00012370: 5265 7375 6c74 0a20 2020 2020 2020 2022  Result.        "
+00012380: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
+00012390: 6766 696c 6520 6973 204e 6f6e 653a 0a20  gfile is None:. 
+000123a0: 2020 2020 2020 2020 2020 206c 6f67 6669             logfi
+000123b0: 6c65 203d 2073 656c 662e 5f4c 4f47 4649  le = self._LOGFI
+000123c0: 4c45 0a20 2020 2020 2020 206c 6f67 6669  LE.        logfi
+000123d0: 6c65 203d 206c 6f67 6669 6c65 2e66 6f72  le = logfile.for
+000123e0: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
+000123f0: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
+00012400: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00012410: 666f 2866 2243 6f70 7969 6e67 206c 6f67  fo(f"Copying log
+00012420: 6669 6c65 207b 6c6f 6766 696c 657d 2066  file {logfile} f
+00012430: 726f 6d20 536c 7572 6d5c 0a20 2020 2020  rom Slurm\.     
+00012440: 2020 2020 2020 2074 6f20 7b6c 6f63 616c         to {local
+00012450: 5f74 6d70 5f73 746f 7261 6765 7d22 290a  _tmp_storage}").
+00012460: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00012470: 2073 656c 662e 6765 7428 0a20 2020 2020   self.get(.     
+00012480: 2020 2020 2020 2072 656d 6f74 653d 6c6f         remote=lo
+00012490: 6766 696c 652c 0a20 2020 2020 2020 2020  gfile,.         
+000124a0: 2020 206c 6f63 616c 3d6c 6f63 616c 5f74     local=local_t
+000124b0: 6d70 5f73 746f 7261 6765 290a 2020 2020  mp_storage).    
+000124c0: 2020 2020 6578 706f 7274 5f66 696c 6520      export_file 
+000124d0: 3d20 6c6f 6361 6c5f 746d 705f 7374 6f72  = local_tmp_stor
+000124e0: 6167 652b 6c6f 6766 696c 650a 2020 2020  age+logfile.    
+000124f0: 2020 2020 7265 7475 726e 206c 6f63 616c      return local
+00012500: 5f74 6d70 5f73 746f 7261 6765 2c20 6578  _tmp_storage, ex
+00012510: 706f 7274 5f66 696c 652c 2072 6573 756c  port_file, resul
+00012520: 740a 0a20 2020 2064 6566 2067 6574 5f75  t..    def get_u
+00012530: 6e7a 6970 5f63 6f6d 6d61 6e64 2873 656c  nzip_command(sel
+00012540: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
+00012550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012560: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00012570: 725f 6669 6c65 7479 7065 733a 2073 7472  r_filetypes: str
+00012580: 203d 2022 2a2e 7a61 7272 202a 2e74 6966   = "*.zarr *.tif
+00012590: 6620 2a2e 7469 6622 0a20 2020 2020 2020  f *.tif".       
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125b0: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+000125c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000125d0: 2047 656e 6572 6174 6520 6120 636f 6d6d   Generate a comm
+000125e0: 616e 6420 7374 7269 6e67 2066 6f72 2075  and string for u
+000125f0: 6e7a 6970 7069 6e67 2061 2064 6174 6120  nzipping a data 
+00012600: 6172 6368 6976 6520 616e 6420 6372 6561  archive and crea
+00012610: 7469 6e67 0a20 2020 2020 2020 2072 6571  ting.        req
+00012620: 7569 7265 6420 6469 7265 6374 6f72 6965  uired directorie
+00012630: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
+00012640: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00012650: 0a20 2020 2020 2020 2020 2020 207a 6970  .            zip
+00012660: 6669 6c65 2028 7374 7229 3a20 5468 6520  file (str): The 
+00012670: 6e61 6d65 206f 6620 7468 6520 7a69 7020  name of the zip 
+00012680: 6172 6368 6976 6520 6669 6c65 2074 6f20  archive file to 
+00012690: 6578 7472 6163 742e 0a20 2020 2020 2020  extract..       
+000126a0: 2020 2020 2020 2020 2057 6974 686f 7574           Without
+000126b0: 2065 7874 656e 7369 6f6e 2e0a 2020 2020   extension..    
+000126c0: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
+000126d0: 696c 6574 7970 6573 2028 7374 722c 206f  iletypes (str, o
+000126e0: 7074 696f 6e61 6c29 3a20 4120 7370 6163  ptional): A spac
+000126f0: 652d 7365 7061 7261 7465 6420 7374 7269  e-separated stri
+00012700: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00012710: 2020 2063 6f6e 7461 696e 696e 6720 7468     containing th
+00012720: 6520 6669 6c65 2065 7874 656e 7369 6f6e  e file extension
+00012730: 7320 746f 2065 7874 7261 6374 2066 726f  s to extract fro
+00012740: 6d20 7468 6520 7a69 7020 6669 6c65 2e0a  m the zip file..
+00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012760: 452e 672e 2064 6566 6175 6c74 7320 746f  E.g. defaults to
+00012770: 2022 2a2e 7a61 7272 202a 2e74 6966 6620   "*.zarr *.tiff 
+00012780: 2a2e 7469 6622 2e0a 2020 2020 2020 2020  *.tif"..        
+00012790: 2020 2020 2020 2020 5365 7474 696e 6720          Setting 
+000127a0: 7468 6973 2061 7267 756d 656e 7420 746f  this argument to
+000127b0: 2060 4e6f 6e65 6020 7769 6c6c 206f 6d69   `None` will omi
+000127c0: 7420 7468 6520 6669 6c65 0a20 2020 2020  t the file.     
+000127d0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+000127e0: 7220 616e 6420 6578 7472 6163 7420 616c  r and extract al
+000127f0: 6c20 6669 6c65 732e 0a0a 2020 2020 2020  l files...      
+00012800: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00012810: 2020 2020 2020 2073 7472 3a0a 2020 2020         str:.    
+00012820: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00012830: 636f 6d6d 616e 6420 746f 2065 7874 7261  command to extra
+00012840: 6374 2074 6865 2073 7065 6369 6669 6564  ct the specified
+00012850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012860: 2066 696c 6574 7970 6573 2066 726f 6d20   filetypes from 
+00012870: 7468 6520 7a69 7020 6669 6c65 2e0a 2020  the zip file..  
+00012880: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012890: 2020 756e 7a69 705f 636d 6420 3d20 6622    unzip_cmd = f"
+000128a0: 6d6b 6469 7220 7b73 656c 662e 736c 7572  mkdir {self.slur
+000128b0: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
+000128c0: 7066 696c 657d 205c 0a20 2020 2020 2020  pfile} \.       
+000128d0: 2020 2020 2020 2020 2020 2020 207b 7365               {se
+000128e0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
+000128f0: 7468 7d2f 7b7a 6970 6669 6c65 7d2f 6461  th}/{zipfile}/da
+00012900: 7461 205c 0a20 2020 2020 2020 2020 2020  ta \.           
+00012910: 2020 2020 2020 2020 207b 7365 6c66 2e73           {self.s
+00012920: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
+00012930: 7b7a 6970 6669 6c65 7d2f 6461 7461 2f69  {zipfile}/data/i
+00012940: 6e20 5c0a 2020 2020 2020 2020 2020 2020  n \.            
+00012950: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
+00012960: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
+00012970: 7a69 7066 696c 657d 2f64 6174 612f 6f75  zipfile}/data/ou
+00012980: 7420 5c0a 2020 2020 2020 2020 2020 2020  t \.            
+00012990: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
+000129a0: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
+000129b0: 7a69 7066 696c 657d 2f64 6174 612f 6774  zipfile}/data/gt
+000129c0: 3b20 5c0a 2020 2020 2020 2020 2020 2020  ; \.            
+000129d0: 2020 2020 2020 2020 377a 2078 202d 7920          7z x -y 
+000129e0: 2d6f 7b73 656c 662e 736c 7572 6d5f 6461  -o{self.slurm_da
+000129f0: 7461 5f70 6174 687d 2f7b 7a69 7066 696c  ta_path}/{zipfil
+00012a00: 657d 2f64 6174 612f 696e 205c 0a20 2020  e}/data/in \.   
+00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a20: 207b 7365 6c66 2e73 6c75 726d 5f64 6174   {self.slurm_dat
+00012a30: 615f 7061 7468 7d2f 7b7a 6970 6669 6c65  a_path}/{zipfile
+00012a40: 7d2e 7a69 7020 7b66 696c 7465 725f 6669  }.zip {filter_fi
+00012a50: 6c65 7479 7065 737d 220a 0a20 2020 2020  letypes}"..     
+00012a60: 2020 2072 6574 7572 6e20 756e 7a69 705f     return unzip_
+00012a70: 636d 640a 0a20 2020 2064 6566 2067 6574  cmd..    def get
+00012a80: 5f69 6d61 6765 5f76 6572 7369 6f6e 735f  _image_versions_
+00012a90: 616e 645f 6461 7461 5f66 696c 6573 2873  and_data_files(s
+00012aa0: 656c 662c 206d 6f64 656c 3a20 7374 720a  elf, model: str.
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ad0: 2020 2020 2020 2020 2020 2920 2d3e 2054            ) -> T
+00012ae0: 7570 6c65 5b4c 6973 745b 7374 725d 2c20  uple[List[str], 
+00012af0: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
+00012b00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012b10: 5265 7472 6965 7665 2074 6865 2061 7661  Retrieve the ava
+00012b20: 696c 6162 6c65 2069 6d61 6765 2076 6572  ilable image ver
+00012b30: 7369 6f6e 7320 616e 6420 696e 7075 7420  sions and input 
+00012b40: 6461 7461 2066 696c 6573 2066 6f72 2061  data files for a
+00012b50: 0a20 2020 2020 2020 2067 6976 656e 206d  .        given m
+00012b60: 6f64 656c 2e0a 0a20 2020 2020 2020 2041  odel...        A
+00012b70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012b80: 206d 6f64 656c 2028 7374 7229 3a20 5468   model (str): Th
+00012b90: 6520 6e61 6d65 206f 6620 7468 6520 6d6f  e name of the mo
+00012ba0: 6465 6c20 746f 2071 7565 7279 2066 6f72  del to query for
+00012bb0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00012bc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00012bd0: 5475 706c 655b 4c69 7374 5b73 7472 5d2c  Tuple[List[str],
+00012be0: 204c 6973 745b 7374 725d 5d3a 0a20 2020   List[str]]:.   
+00012bf0: 2020 2020 2020 2020 2020 2020 2041 2074               A t
+00012c00: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
+00012c10: 7477 6f20 6c69 7374 733a 0a20 2020 2020  two lists:.     
+00012c20: 2020 2020 2020 2020 2020 202d 2054 6865             - The
+00012c30: 2066 6972 7374 206c 6973 7420 696e 636c   first list incl
+00012c40: 7564 6573 2074 6865 2061 7661 696c 6162  udes the availab
+00012c50: 6c65 2069 6d61 6765 2076 6572 7369 6f6e  le image version
+00012c60: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
+00012c70: 2020 2020 2020 2020 736f 7274 6564 2069          sorted i
+00012c80: 6e20 6465 7363 656e 6469 6e67 206f 7264  n descending ord
+00012c90: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+00012ca0: 2020 2020 2d20 5468 6520 7365 636f 6e64      - The second
+00012cb0: 206c 6973 7420 696e 636c 7564 6573 2074   list includes t
+00012cc0: 6865 2061 7661 696c 6162 6c65 2064 6174  he available dat
+00012cd0: 6120 6669 6c65 732e 0a0a 2020 2020 2020  a files...      
+00012ce0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00012cf0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+00012d00: 3a20 4966 2074 6865 2070 726f 7669 6465  : If the provide
+00012d10: 6420 6d6f 6465 6c20 6973 206e 6f74 2066  d model is not f
+00012d20: 6f75 6e64 2069 6e20 7468 650a 2020 2020  ound in the.    
+00012d30: 2020 2020 2020 2020 2020 2020 536c 7572              Slur
+00012d40: 6d43 6c69 656e 7427 7320 6b6e 6f77 6e20  mClient's known 
+00012d50: 6d6f 6465 6c20 7061 7468 732e 0a20 2020  model paths..   
+00012d60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012d70: 2069 6d61 6765 5f70 6174 6820 3d20 7365   image_path = se
+00012d80: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
+00012d90: 6174 6873 2e67 6574 286d 6f64 656c 290a  aths.get(model).
+00012da0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00012db0: 6d61 6765 5f70 6174 683a 0a20 2020 2020  mage_path:.     
+00012dc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00012dd0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+00012de0: 2020 2020 2020 2020 2066 224e 6f20 7061           f"No pa
+00012df0: 7468 206b 6e6f 776e 2066 6f72 2070 726f  th known for pro
+00012e00: 7669 6465 6420 6d6f 6465 6c20 7b6d 6f64  vided model {mod
+00012e10: 656c 7d2c 205c 0a20 2020 2020 2020 2020  el}, \.         
+00012e20: 2020 2020 2020 2020 2020 2069 6e20 7b73             in {s
+00012e30: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+00012e40: 7061 7468 737d 2229 0a20 2020 2020 2020  paths}").       
+00012e50: 2063 6d64 6c69 7374 203d 205b 0a20 2020   cmdlist = [.   
+00012e60: 2020 2020 2020 2020 2073 656c 662e 5f56           self._V
+00012e70: 4552 5349 4f4e 5f43 4d44 2e66 6f72 6d61  ERSION_CMD.forma
+00012e80: 7428 736c 7572 6d5f 696d 6167 6573 5f70  t(slurm_images_p
+00012e90: 6174 683d 7365 6c66 2e73 6c75 726d 5f69  ath=self.slurm_i
+00012ea0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2069 6d61 6765 5f70 6174 683d 696d 6167   image_path=imag
+00012ee0: 655f 7061 7468 292c 0a20 2020 2020 2020  e_path),.       
+00012ef0: 2020 2020 2073 656c 662e 5f44 4154 415f       self._DATA_
+00012f00: 434d 442e 666f 726d 6174 2873 6c75 726d  CMD.format(slurm
+00012f10: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
+00012f20: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
+00012f30: 5d0a 2020 2020 2020 2020 2320 7370 6c69  ].        # spli
+00012f40: 7420 7265 7370 6f6e 7365 7320 7065 7220  t responses per 
+00012f50: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+00012f60: 7265 7370 6f6e 7365 5f6c 6973 7420 3d20  response_list = 
+00012f70: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+00012f80: 735f 7370 6c69 745f 6f75 7428 636d 646c  s_split_out(cmdl
+00012f90: 6973 7429 0a20 2020 2020 2020 2023 2073  ist).        # s
+00012fa0: 706c 6974 206c 696e 6573 2066 7572 7468  plit lines furth
+00012fb0: 6572 2069 6e74 6f20 7375 626c 6973 7473  er into sublists
+00012fc0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00012fd0: 655f 6c69 7374 203d 205b 7265 7370 6f6e  e_list = [respon
+00012fe0: 7365 2e73 7472 6970 2829 2e73 706c 6974  se.strip().split
+00012ff0: 2827 5c6e 2729 0a20 2020 2020 2020 2020  ('\n').         
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 666f 7220 7265 7370 6f6e 7365 2069 6e20  for response in 
+00013020: 7265 7370 6f6e 7365 5f6c 6973 745d 0a20  response_list]. 
+00013030: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
+00013040: 6c69 7374 5b30 5d20 3d20 736f 7274 6564  list[0] = sorted
+00013050: 2872 6573 706f 6e73 655f 6c69 7374 5b30  (response_list[0
+00013060: 5d2c 2072 6576 6572 7365 3d54 7275 6529  ], reverse=True)
+00013070: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013080: 7265 7370 6f6e 7365 5f6c 6973 745b 305d  response_list[0]
+00013090: 2c20 7265 7370 6f6e 7365 5f6c 6973 745b  , response_list[
+000130a0: 315d 0a0a 2020 2020 6465 6620 6765 745f  1]..    def get_
+000130b0: 616c 6c5f 696d 6167 655f 7665 7273 696f  all_image_versio
+000130c0: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
+000130d0: 7328 7365 6c66 0a20 2020 2020 2020 2020  s(self.         
+000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013100: 2020 2020 2029 202d 3e20 5475 706c 655b       ) -> Tuple[
+00013110: 4469 6374 5b73 7472 2c20 4c69 7374 5b73  Dict[str, List[s
+00013120: 7472 5d5d 2c0a 2020 2020 2020 2020 2020  tr]],.          
+00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013150: 2020 2020 2020 2020 2020 2020 2020 204c                 L
+00013160: 6973 745b 7374 725d 5d3a 0a20 2020 2020  ist[str]]:.     
+00013170: 2020 2022 2222 5265 7472 6965 7665 2061     """Retrieve a
+00013180: 6c6c 2061 7661 696c 6162 6c65 2069 6d61  ll available ima
+00013190: 6765 2076 6572 7369 6f6e 7320 616e 6420  ge versions and 
+000131a0: 6461 7461 2066 696c 6573 2066 726f 6d0a  data files from.
+000131b0: 2020 2020 2020 2020 7468 6520 536c 7572          the Slur
+000131c0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
+000131d0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000131e0: 2020 2020 2020 2020 5475 706c 655b 4469          Tuple[Di
+000131f0: 6374 5b73 7472 2c20 4c69 7374 5b73 7472  ct[str, List[str
+00013200: 5d5d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  ]], List[str]]:.
 00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 666f 7220 7265 7370 6f6e 7365 2069    for response i
-00013230: 6e20 7265 7370 6f6e 7365 5f6c 6973 745d  n response_list]
-00013240: 0a0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-00013250: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
-00013260: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00013270: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
-00013280: 2020 2020 2023 2052 6574 7572 6e20 6869       # Return hi
-00013290: 6768 6573 7420 7665 7273 696f 6e20 6669  ghest version fi
-000132a0: 7273 740a 2020 2020 2020 2020 2020 2020  rst.            
-000132b0: 7265 7375 6c74 6469 6374 5b6b 5d20 3d20  resultdict[k] = 
-000132c0: 736f 7274 6564 2872 6573 706f 6e73 655f  sorted(response_
-000132d0: 6c69 7374 5b69 5d2c 2072 6576 6572 7365  list[i], reverse
-000132e0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-000132f0: 7265 7475 726e 2072 6573 756c 7464 6963  return resultdic
-00013300: 742c 2072 6573 706f 6e73 655f 6c69 7374  t, response_list
-00013310: 5b2d 315d 0a                             [-1].
+00013220: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+00013230: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00013240: 2020 2020 2d20 4120 6469 6374 696f 6e61      - A dictiona
+00013250: 7279 206d 6170 7069 6e67 206d 6f64 656c  ry mapping model
+00013260: 7320 746f 2061 7661 696c 6162 6c65 2076  s to available v
+00013270: 6572 7369 6f6e 732e 0a20 2020 2020 2020  ersions..       
+00013280: 2020 2020 2020 2020 202d 2041 206c 6973           - A lis
+00013290: 7420 6f66 2061 7661 696c 6162 6c65 2069  t of available i
+000132a0: 6e70 7574 2064 6174 6120 666f 6c64 6572  nput data folder
+000132b0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+000132c0: 2020 2020 2020 2072 6573 756c 7464 6963         resultdic
+000132d0: 7420 3d20 7b7d 0a20 2020 2020 2020 2063  t = {}.        c
+000132e0: 6d64 6c69 7374 203d 205b 5d0a 0a20 2020  mdlist = []..   
+000132f0: 2020 2020 2066 6f72 2070 6174 6820 696e       for path in
+00013300: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+00013310: 6c5f 7061 7468 732e 7661 6c75 6573 2829  l_paths.values()
+00013320: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00013330: 7468 636d 6420 3d20 7365 6c66 2e5f 5645  thcmd = self._VE
+00013340: 5253 494f 4e5f 434d 442e 666f 726d 6174  RSION_CMD.format
+00013350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013360: 2020 736c 7572 6d5f 696d 6167 6573 5f70    slurm_images_p
+00013370: 6174 683d 7365 6c66 2e73 6c75 726d 5f69  ath=self.slurm_i
+00013380: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
+00013390: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+000133a0: 655f 7061 7468 3d70 6174 6829 0a20 2020  e_path=path).   
+000133b0: 2020 2020 2020 2020 2063 6d64 6c69 7374           cmdlist
+000133c0: 2e61 7070 656e 6428 7061 7468 636d 6429  .append(pathcmd)
+000133d0: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
+000133e0: 6461 7461 2070 6174 6820 746f 6f0a 2020  data path too.  
+000133f0: 2020 2020 2020 636d 646c 6973 742e 6170        cmdlist.ap
+00013400: 7065 6e64 2873 656c 662e 5f44 4154 415f  pend(self._DATA_
+00013410: 434d 442e 666f 726d 6174 280a 2020 2020  CMD.format(.    
+00013420: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
+00013430: 7461 5f70 6174 683d 7365 6c66 2e73 6c75  ta_path=self.slu
+00013440: 726d 5f64 6174 615f 7061 7468 2929 0a0a  rm_data_path))..
+00013450: 2020 2020 2020 2020 2320 5370 6c69 7420          # Split 
+00013460: 7265 7370 6f6e 7365 7320 7065 7220 636f  responses per co
+00013470: 6d6d 616e 640a 2020 2020 2020 2020 7265  mmand.        re
+00013480: 7370 6f6e 7365 5f6c 6973 7420 3d20 7365  sponse_list = se
+00013490: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 735f  lf.run_commands_
+000134a0: 7370 6c69 745f 6f75 7428 636d 646c 6973  split_out(cmdlis
+000134b0: 7429 0a0a 2020 2020 2020 2020 2320 5370  t)..        # Sp
+000134c0: 6c69 7420 6c69 6e65 7320 6675 7274 6865  lit lines furthe
+000134d0: 7220 696e 746f 2073 7562 6c69 7374 730a  r into sublists.
+000134e0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000134f0: 5f6c 6973 7420 3d20 5b72 6573 706f 6e73  _list = [respons
+00013500: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
+00013510: 275c 6e27 290a 2020 2020 2020 2020 2020  '\n').          
+00013520: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013530: 6f72 2072 6573 706f 6e73 6520 696e 2072  or response in r
+00013540: 6573 706f 6e73 655f 6c69 7374 5d0a 0a20  esponse_list].. 
+00013550: 2020 2020 2020 2066 6f72 2069 2c20 6b20         for i, k 
+00013560: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
+00013570: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
+00013580: 7468 7329 3a0a 2020 2020 2020 2020 2020  ths):.          
+00013590: 2020 2320 5265 7475 726e 2068 6967 6865    # Return highe
+000135a0: 7374 2076 6572 7369 6f6e 2066 6972 7374  st version first
+000135b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000135c0: 756c 7464 6963 745b 6b5d 203d 2073 6f72  ultdict[k] = sor
+000135d0: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
+000135e0: 745b 695d 2c20 7265 7665 7273 653d 5472  t[i], reverse=Tr
+000135f0: 7565 290a 0a20 2020 2020 2020 2072 6574  ue)..        ret
+00013600: 7572 6e20 7265 7375 6c74 6469 6374 2c20  urn resultdict, 
+00013610: 7265 7370 6f6e 7365 5f6c 6973 745b 2d31  response_list[-1
+00013620: 5d0a                                     ].
```

### Comparing `biomero-1.7.1/biomero.egg-info/PKG-INFO` & `biomero-1.8.0/biomero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.7.1
+Version: 1.8.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.7.1/biomero.egg-info/SOURCES.txt` & `biomero-1.8.0/biomero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/docs/Makefile` & `biomero-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/docs/conf.py` & `biomero-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/docs/index.rst` & `biomero-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/docs/make.bat` & `biomero-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/pyproject.toml` & `biomero-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/convert_job_array.sh` & `biomero-1.8.0/resources/convert_job_array.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/convert_zarr_to_tiff.py` & `biomero-1.8.0/resources/convert_zarr_to_tiff.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/job_template.sh` & `biomero-1.8.0/resources/job_template.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/slurm-config.ini` & `biomero-1.8.0/resources/slurm-config.ini`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/Cells.tif` & `biomero-1.8.0/resources/tutorials/images/Cells.tif`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/cellexpansion.png` & `biomero-1.8.0/resources/tutorials/images/cellexpansion.png`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/gc_allow_ssh.PNG` & `biomero-1.8.0/resources/tutorials/images/gc_allow_ssh.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/nuclei_labels.png` & `biomero-1.8.0/resources/tutorials/images/nuclei_labels.png`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/webclient_init_env.PNG` & `biomero-1.8.0/resources/tutorials/images/webclient_init_env.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/webclient_init_env_done.PNG` & `biomero-1.8.0/resources/tutorials/images/webclient_init_env_done.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/webclient_run_cellpose.PNG` & `biomero-1.8.0/resources/tutorials/images/webclient_run_cellpose.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/images/webclient_run_workflow.PNG` & `biomero-1.8.0/resources/tutorials/images/webclient_run_workflow.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/tutorial_Azure_slurm.md` & `biomero-1.8.0/resources/tutorials/tutorial_Azure_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/tutorial_GoogleCloud_slurm.md` & `biomero-1.8.0/resources/tutorials/tutorial_GoogleCloud_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/tutorial_cellexpansion.md` & `biomero-1.8.0/resources/tutorials/tutorial_cellexpansion.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/tutorial_cellprofiler.md` & `biomero-1.8.0/resources/tutorials/tutorial_cellprofiler.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/resources/tutorials/tutorial_local_slurm.md` & `biomero-1.8.0/resources/tutorials/tutorial_local_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.1/tests/unit/test_slurm_client.py` & `biomero-1.8.0/tests/unit/test_slurm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,29 +840,29 @@
     """
     # GIVEN
     slurm_job_id = "12345"
     filename = "output.zip"
     data_location = "/path"
     logfile = "/path/to/logfile"
 
-    mock_extract_data_location.return_value = data_location
     mock_run_commands.return_value = mock.MagicMock(ok=True)
 
     # WHEN
     result = slurm_client.cleanup_tmp_files(
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_not_called()
     mock_run_commands.assert_called_once_with([
         f"rm {filename}.*",
         f"rm {logfile}",
         f"rm slurm-{slurm_job_id}_*.out",
-        f"rm -rf {data_location} {data_location}.*"
-    ])
+        f"rm -rf {data_location} {data_location}.*",
+        f"rm config_path.txt"
+    ], sep=' ; ')
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.SlurmClient.run_commands')
 @patch('biomero.slurm_client.SlurmClient.extract_data_location_from_log')
 def test_cleanup_tmp_files(mock_extract_data_location, mock_run_commands,
@@ -871,30 +871,32 @@
     Test the cleanup of temporary files associated with a Slurm job.
     """
     # GIVEN
     slurm_job_id = "12345"
     filename = "output.zip"
     data_location = None
     logfile = "/path/to/logfile"
+    found_location = '/path'
 
-    mock_extract_data_location.return_value = data_location
+    mock_extract_data_location.return_value = found_location
     mock_run_commands.return_value = mock.MagicMock(ok=True)
 
     # WHEN
     result = slurm_client.cleanup_tmp_files(
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_called_once_with(logfile)
     mock_run_commands.assert_called_once_with([
         f"rm {filename}.*",
         f"rm {logfile}",
         f"rm slurm-{slurm_job_id}_*.out",
-        f"rm -rf {data_location} {data_location}.*"
-    ])
+        f"rm -rf {found_location} {found_location}.*",
+        f"rm config_path.txt"
+    ], sep=' ; ')
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.Connection.create_session')
 @patch('biomero.slurm_client.Connection.open')
 @patch('biomero.slurm_client.Connection.put')
```


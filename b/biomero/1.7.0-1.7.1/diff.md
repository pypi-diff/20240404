# Comparing `tmp/biomero-1.7.0.tar.gz` & `tmp/biomero-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-sn_9sy7g/biomero-1.7.0.tar", last modified: Tue Apr  2 12:55:51 2024, max compression
+gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-axp787tl/biomero-1.7.1.tar", last modified: Thu Apr  4 13:16:45 2024, max compression
```

## Comparing `biomero-1.7.0.tar` & `biomero-1.7.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 12:55:35.000000 biomero-1.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 12:55:35.000000 biomero-1.7.0/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-02 12:55:35.000000 biomero-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-02 12:55:35.000000 biomero-1.7.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:55:35.000000 biomero-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 12:55:35.000000 biomero-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-02 12:55:51.000000 biomero-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-02 12:55:35.000000 biomero-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    78069 2024-04-02 12:55:35.000000 biomero-1.7.0/biomero/slurm_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 12:55:51.000000 biomero-1.7.0/biomero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/omero_slurm_client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-02 12:55:35.000000 biomero-1.7.0/docs/tutorial_link.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-02 12:55:35.000000 biomero-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_job_array.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_zarr_to_tiff.def
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/convert_zarr_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/example.config
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/job_template.sh
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/pull_images.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/slurm-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/resources/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/Cells.tif
--rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/cellexpansion.png
--rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/gc_allow_ssh.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/nuclei_labels.png
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_init_env.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_init_env_done.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_run_cellpose.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/images/webclient_run_workflow.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_Azure_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_cellexpansion.md
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_cellprofiler.md
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-02 12:55:35.000000 biomero-1.7.0/resources/tutorials/tutorial_local_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:55:51.000000 biomero-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:51.000000 biomero-1.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45067 2024-04-02 12:55:35.000000 biomero-1.7.0/tests/unit/test_slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 13:16:39.000000 biomero-1.7.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 13:16:39.000000 biomero-1.7.1/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 13:16:39.000000 biomero-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 13:16:39.000000 biomero-1.7.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 13:16:39.000000 biomero-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 13:16:39.000000 biomero-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 13:16:45.000000 biomero-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-04 13:16:39.000000 biomero-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78613 2024-04-04 13:16:39.000000 biomero-1.7.1/biomero/slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 13:16:45.000000 biomero-1.7.1/biomero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/omero_slurm_client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 13:16:39.000000 biomero-1.7.1/docs/tutorial_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 13:16:39.000000 biomero-1.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_job_array.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_zarr_to_tiff.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/convert_zarr_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/job_template.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/pull_images.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/slurm-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/resources/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/Cells.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/cellexpansion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/gc_allow_ssh.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/nuclei_labels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_init_env.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_init_env_done.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_run_cellpose.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/images/webclient_run_workflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_Azure_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_GoogleCloud_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_cellexpansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_cellprofiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-04 13:16:39.000000 biomero-1.7.1/resources/tutorials/tutorial_local_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:16:45.000000 biomero-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:45.000000 biomero-1.7.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45151 2024-04-04 13:16:39.000000 biomero-1.7.1/tests/unit/test_slurm_client.py
```

### Comparing `biomero-1.7.0/.github/workflows/python-package.yml` & `biomero-1.7.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/.github/workflows/python-publish.yml` & `biomero-1.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/.github/workflows/sphinx.yml` & `biomero-1.7.1/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/.gitignore` & `biomero-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/CITATION.cff` & `biomero-1.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/LICENSE` & `biomero-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/PKG-INFO` & `biomero-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.7.0/README.md` & `biomero-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/biomero/constants.py` & `biomero-1.7.1/biomero/constants.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/biomero/slurm_client.py` & `biomero-1.7.1/biomero/slurm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,4764 +117,4798 @@
 00000740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
 00000750: 7374 723a 2054 6865 2066 696e 616c 2073  str: The final s
 00000760: 7461 7465 206f 6620 7468 6520 536c 7572  tate of the Slur
 00000770: 6d20 6a6f 622e 0a20 2020 2020 2020 2022  m job..        "
 00000780: 2222 0a20 2020 2020 2020 2077 6869 6c65  "".        while
 00000790: 2073 656c 662e 6a6f 625f 7374 6174 6520   self.job_state 
 000007a0: 6e6f 7420 696e 2028 2246 4149 4c45 4422  not in ("FAILED"
-000007b0: 2c20 2243 4f4d 504c 4554 4544 222c 2022  , "COMPLETED", "
-000007c0: 4341 4e43 454c 4c45 4422 2c20 2254 494d  CANCELLED", "TIM
-000007d0: 454f 5554 2229 3a0a 2020 2020 2020 2020  EOUT"):.        
-000007e0: 2020 2020 6a6f 625f 7374 6174 7573 5f64      job_status_d
-000007f0: 6963 742c 2070 6f6c 6c5f 7265 7375 6c74  ict, poll_result
-00000800: 203d 2073 6c75 726d 436c 6965 6e74 2e63   = slurmClient.c
-00000810: 6865 636b 5f6a 6f62 5f73 7461 7475 7328  heck_job_status(
-00000820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000830: 205b 7365 6c66 2e6a 6f62 5f69 645d 290a   [self.job_id]).
-00000840: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00000850: 6f74 2070 6f6c 6c5f 7265 7375 6c74 2e6f  ot poll_result.o
-00000860: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-00000870: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00000880: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-00000890: 2020 2020 2020 2066 2245 7272 6f72 2063         f"Error c
-000008a0: 6865 636b 696e 6720 6a6f 6220 7374 6174  hecking job stat
-000008b0: 7573 3a7b 706f 6c6c 5f72 6573 756c 742e  us:{poll_result.
-000008c0: 7374 6465 7272 7d22 290a 2020 2020 2020  stderr}").      
-000008d0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
-000008e0: 6f62 5f73 7461 7465 203d 2022 4641 494c  ob_state = "FAIL
-000008f0: 4544 220a 2020 2020 2020 2020 2020 2020  ED".            
-00000900: 7365 6c66 2e6a 6f62 5f73 7461 7465 203d  self.job_state =
-00000910: 206a 6f62 5f73 7461 7475 735f 6469 6374   job_status_dict
-00000920: 5b73 656c 662e 6a6f 625f 6964 5d0a 2020  [self.job_id].  
-00000930: 2020 2020 2020 2020 2020 2320 7761 6974            # wait
-00000940: 2066 6f72 2031 3020 7365 636f 6e64 7320   for 10 seconds 
-00000950: 6265 666f 7265 2063 6865 636b 696e 6720  before checking 
-00000960: 6167 6169 6e0a 2020 2020 2020 2020 2020  again.          
-00000970: 2020 6f6d 6572 6f43 6f6e 6e2e 6b65 6570    omeroConn.keep
-00000980: 416c 6976 6528 2920 2023 206b 6565 7020  Alive()  # keep 
-00000990: 7468 6520 4f4d 4552 4f20 636f 6e6e 6563  the OMERO connec
-000009a0: 7469 6f6e 2061 6c69 7665 0a20 2020 2020  tion alive.     
-000009b0: 2020 2020 2020 2074 696d 6573 6c65 6570         timesleep
-000009c0: 2e73 6c65 6570 2831 3029 0a20 2020 2020  .sleep(10).     
-000009d0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-000009e0: 224a 6f62 207b 7365 6c66 2e6a 6f62 5f69  "Job {self.job_i
-000009f0: 647d 2066 696e 6973 6865 643a 207b 7365  d} finished: {se
-00000a00: 6c66 2e6a 6f62 5f73 7461 7465 7d22 290a  lf.job_state}").
-00000a10: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00000a20: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00000a30: 2066 2259 6f75 2063 616e 2067 6574 2074   f"You can get t
-00000a40: 6865 206c 6f67 6669 6c65 2075 7369 6e67  he logfile using
-00000a50: 2060 536c 7572 6d20 4765 7420 5570 6461   `Slurm Get Upda
-00000a60: 7465 6020 6f6e 206a 6f62 207b 7365 6c66  te` on job {self
-00000a70: 2e6a 6f62 5f69 647d 2229 0a20 2020 2020  .job_id}").     
-00000a80: 2020 2072 6574 7572 6e20 7365 6c66 2e6a     return self.j
-00000a90: 6f62 5f73 7461 7465 0a0a 2020 2020 6465  ob_state..    de
-00000aa0: 6620 636f 6d70 6c65 7465 6428 7365 6c66  f completed(self
-00000ab0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00000ac0: 2020 2020 2020 2043 6865 636b 2069 6620         Check if 
-00000ad0: 7468 6520 536c 7572 6d20 6a6f 6220 6861  the Slurm job ha
-00000ae0: 7320 636f 6d70 6c65 7465 6420 7375 6363  s completed succ
-00000af0: 6573 7366 756c 6c79 2e0a 0a20 2020 2020  essfully...     
-00000b00: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00000b10: 2020 2020 2020 2020 626f 6f6c 3a20 5472          bool: Tr
-00000b20: 7565 2069 6620 7468 6520 6a6f 6220 6861  ue if the job ha
-00000b30: 7320 636f 6d70 6c65 7465 643b 2046 616c  s completed; Fal
-00000b40: 7365 206f 7468 6572 7769 7365 2e0a 2020  se otherwise..  
-00000b50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00000b60: 2020 7265 7475 726e 2073 656c 662e 6a6f    return self.jo
-00000b70: 625f 7374 6174 6520 3d3d 2022 434f 4d50  b_state == "COMP
-00000b80: 4c45 5445 4422 0a0a 2020 2020 6465 6620  LETED"..    def 
-00000b90: 5f5f 7374 725f 5f28 7365 6c66 293a 0a20  __str__(self):. 
-00000ba0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000bb0: 2020 2052 6574 7572 6e20 6120 7374 7269     Return a stri
-00000bc0: 6e67 2072 6570 7265 7365 6e74 6174 696f  ng representatio
-00000bd0: 6e20 6f66 2074 6865 2053 6c75 726d 4a6f  n of the SlurmJo
-00000be0: 6220 696e 7374 616e 6365 2e0a 0a20 2020  b instance...   
-00000bf0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00000c00: 2020 2020 2020 2020 2020 7374 723a 2053            str: S
-00000c10: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
-00000c20: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
-00000c30: 220a 2020 2020 2020 2020 7072 6f70 6572  ".        proper
-00000c40: 7469 6573 203d 2027 2c20 272e 6a6f 696e  ties = ', '.join
-00000c50: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-00000c60: 7b6b 6579 7d3d 7b76 616c 7565 7d22 2066  {key}={value}" f
-00000c70: 6f72 206b 6579 2c20 7661 6c75 6520 696e  or key, value in
-00000c80: 2073 656c 662e 5f5f 6469 6374 5f5f 2e69   self.__dict__.i
-00000c90: 7465 6d73 2829 290a 2020 2020 2020 2020  tems()).        
-00000ca0: 7265 7475 726e 2066 2253 6c75 726d 4a6f  return f"SlurmJo
-00000cb0: 6228 7b70 726f 7065 7274 6965 737d 2922  b({properties})"
-00000cc0: 0a0a 0a63 6c61 7373 2053 6c75 726d 436c  ...class SlurmCl
-00000cd0: 6965 6e74 2843 6f6e 6e65 6374 696f 6e29  ient(Connection)
-00000ce0: 3a0a 2020 2020 2222 2241 2063 6c69 656e  :.    """A clien
-00000cf0: 7420 666f 7220 636f 6e6e 6563 7469 6e67  t for connecting
-00000d00: 2074 6f20 616e 6420 696e 7465 7261 6374   to and interact
-00000d10: 696e 6720 7769 7468 2061 2053 6c75 726d  ing with a Slurm
-00000d20: 2063 6c75 7374 6572 206f 7665 720a 2020   cluster over.  
-00000d30: 2020 5353 482e 0a0a 2020 2020 5468 6973    SSH...    This
-00000d40: 2063 6c61 7373 2065 7874 656e 6473 2074   class extends t
-00000d50: 6865 2043 6f6e 6e65 6374 696f 6e20 636c  he Connection cl
-00000d60: 6173 732c 2061 6464 696e 6720 6d65 7468  ass, adding meth
-00000d70: 6f64 7320 616e 640a 2020 2020 6174 7472  ods and.    attr
-00000d80: 6962 7574 6573 2073 7065 6369 6669 6320  ibutes specific 
-00000d90: 746f 2077 6f72 6b69 6e67 2077 6974 6820  to working with 
-00000da0: 536c 7572 6d2e 0a0a 2020 2020 536c 7572  Slurm...    Slur
-00000db0: 6d43 6c69 656e 7420 6163 6365 7074 7320  mClient accepts 
-00000dc0: 7468 6520 7361 6d65 2061 7267 756d 656e  the same argumen
-00000dd0: 7473 2061 7320 436f 6e6e 6563 7469 6f6e  ts as Connection
-00000de0: 2e20 4265 6c6f 7720 6f6e 6c79 0a20 2020  . Below only.   
-00000df0: 206d 656e 7469 6f6e 7320 7468 6520 6164   mentions the ad
-00000e00: 6465 6420 6f6e 6573 3a0a 0a20 2020 2054  ded ones:..    T
-00000e10: 6865 2065 6173 6965 7374 2077 6179 2074  he easiest way t
-00000e20: 6f20 7365 7420 7468 6973 2063 6c69 656e  o set this clien
-00000e30: 7420 7570 2069 7320 6279 2075 7369 6e67  t up is by using
-00000e40: 2061 2073 6c75 726d 2d63 6f6e 6669 672e   a slurm-config.
-00000e50: 696e 690a 2020 2020 616e 6420 7468 6520  ini.    and the 
-00000e60: 6672 6f6d 2d63 6f6e 6669 6728 2920 6d65  from-config() me
-00000e70: 7468 6f64 2e0a 0a20 2020 2041 7474 7269  thod...    Attri
-00000e80: 6275 7465 733a 0a20 2020 2020 2020 2073  butes:.        s
-00000e90: 6c75 726d 5f64 6174 615f 7061 7468 2028  lurm_data_path (
-00000ea0: 7374 7229 3a20 5468 6520 7061 7468 2074  str): The path t
-00000eb0: 6f20 7468 6520 6469 7265 6374 6f72 7920  o the directory 
-00000ec0: 636f 6e74 6169 6e69 6e67 2074 6865 0a20  containing the. 
-00000ed0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00000ee0: 6669 6c65 7320 666f 7220 536c 7572 6d20  files for Slurm 
-00000ef0: 6a6f 6273 2e0a 2020 2020 2020 2020 736c  jobs..        sl
-00000f00: 7572 6d5f 696d 6167 6573 5f70 6174 6820  urm_images_path 
-00000f10: 2873 7472 293a 2054 6865 2070 6174 6820  (str): The path 
-00000f20: 746f 2074 6865 2064 6972 6563 746f 7279  to the directory
-00000f30: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
-00000f40: 2020 2020 2020 2020 7468 6520 5369 6e67          the Sing
-00000f50: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
-00000f60: 6f72 2053 6c75 726d 206a 6f62 732e 0a20  or Slurm jobs.. 
-00000f70: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
-00000f80: 7665 7274 6572 735f 7061 7468 2028 7374  verters_path (st
-00000f90: 7229 3a20 5468 6520 7061 7468 2074 6f20  r): The path to 
-00000fa0: 7468 6520 6469 7265 6374 6f72 7920 636f  the directory co
-00000fb0: 6e74 6169 6e69 6e67 0a20 2020 2020 2020  ntaining.       
-00000fc0: 2020 2020 2074 6865 2053 696e 6775 6c61       the Singula
-00000fd0: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
-00000fe0: 6669 6c65 2063 6f6e 7665 7274 6572 732e  file converters.
-00000ff0: 0a20 2020 2020 2020 2073 6c75 726d 5f6d  .        slurm_m
-00001000: 6f64 656c 5f70 6174 6873 2028 6469 6374  odel_paths (dict
-00001010: 293a 2041 2064 6963 7469 6f6e 6172 7920  ): A dictionary 
-00001020: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-00001030: 6174 6873 2074 6f0a 2020 2020 2020 2020  aths to.        
-00001040: 2020 2020 7468 6520 5369 6e67 756c 6172      the Singular
-00001050: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
-00001060: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
-00001070: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
-00001080: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7265    slurm_model_re
-00001090: 706f 7320 2864 6963 7429 3a20 4120 6469  pos (dict): A di
-000010a0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-000010b0: 696e 6720 7468 6520 6769 740a 2020 2020  ing the git.    
-000010c0: 2020 2020 2020 2020 7265 706f 7369 746f          reposito
-000010d0: 7269 6573 206f 6620 5369 6e67 756c 6172  ries of Singular
-000010e0: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
-000010f0: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
-00001100: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
-00001110: 2020 736c 7572 6d5f 6d6f 6465 6c5f 696d    slurm_model_im
-00001120: 6167 6573 2028 6469 6374 293a 2041 2064  ages (dict): A d
-00001130: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00001140: 6e69 6e67 2074 6865 2064 6f63 6b65 7268  ning the dockerh
-00001150: 7562 0a20 2020 2020 2020 2020 2020 206f  ub.            o
-00001160: 6620 7468 6520 5369 6e67 756c 6172 6974  f the Singularit
-00001170: 7920 696d 6167 6573 2066 6f72 2073 7065  y images for spe
-00001180: 6369 6669 6320 536c 7572 6d20 6a6f 6220  cific Slurm job 
-00001190: 6d6f 6465 6c73 2e0a 2020 2020 2020 2020  models..        
-000011a0: 2020 2020 5769 6c6c 2066 696c 6c20 6175      Will fill au
-000011b0: 746f 6d61 7469 6361 6c6c 7920 6672 6f6d  tomatically from
-000011c0: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
-000011d0: 2067 6974 2072 6570 6f73 6974 6f72 792c   git repository,
-000011e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000011f0: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
-00001200: 726d 2e0a 2020 2020 2020 2020 736c 7572  rm..        slur
-00001210: 6d5f 7363 7269 7074 5f70 6174 6820 2873  m_script_path (s
-00001220: 7472 293a 2054 6865 2070 6174 6820 746f  tr): The path to
-00001230: 2074 6865 2064 6972 6563 746f 7279 2063   the directory c
-00001240: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
-00001250: 2020 2020 2020 7468 6520 536c 7572 6d20        the Slurm 
-00001260: 6a6f 6220 7375 626d 6973 7369 6f6e 2073  job submission s
-00001270: 6372 6970 7473 206f 6e20 536c 7572 6d2e  cripts on Slurm.
-00001280: 0a20 2020 2020 2020 2073 6c75 726d 5f73  .        slurm_s
-00001290: 6372 6970 745f 7265 706f 2028 7374 7229  cript_repo (str)
-000012a0: 3a20 5468 6520 6769 7420 6874 7470 7320  : The git https 
-000012b0: 5552 4c20 666f 7220 636c 6f6e 696e 6720  URL for cloning 
-000012c0: 7468 6520 7265 706f 0a20 2020 2020 2020  the repo.       
-000012d0: 2020 2020 2063 6f6e 7461 696e 696e 6720       containing 
-000012e0: 7468 6520 536c 7572 6d20 6a6f 6220 7375  the Slurm job su
-000012f0: 626d 6973 7369 6f6e 2073 6372 6970 7473  bmission scripts
-00001300: 2e20 4f70 7469 6f6e 616c 2e0a 0a20 2020  . Optional...   
-00001310: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
-00001320: 2020 2320 4372 6561 7465 2061 2053 6c75    # Create a Slu
-00001330: 726d 436c 6965 6e74 206f 626a 6563 7420  rmClient object 
-00001340: 6173 2063 6f6e 7465 7874 6d61 6e61 6765  as contextmanage
-00001350: 720a 0a20 2020 2020 2020 2077 6974 6820  r..        with 
-00001360: 536c 7572 6d43 6c69 656e 742e 6672 6f6d  SlurmClient.from
-00001370: 5f63 6f6e 6669 6728 2920 6173 2063 6c69  _config() as cli
-00001380: 656e 743a 0a0a 2020 2020 2020 2020 2020  ent:..          
-00001390: 2020 2320 5275 6e20 6120 636f 6d6d 616e    # Run a comman
-000013a0: 6420 6f6e 2074 6865 2072 656d 6f74 6520  d on the remote 
-000013b0: 686f 7374 0a0a 2020 2020 2020 2020 2020  host..          
-000013c0: 2020 7265 7375 6c74 203d 2063 6c69 656e    result = clien
-000013d0: 742e 7275 6e28 2773 6261 7463 6820 6d79  t.run('sbatch my
-000013e0: 6a6f 622e 7368 2729 0a0a 2020 2020 2020  job.sh')..      
-000013f0: 2020 2020 2020 2320 4368 6563 6b20 7768        # Check wh
-00001400: 6574 6865 7220 7468 6520 636f 6d6d 616e  ether the comman
-00001410: 6420 7375 6363 6565 6465 640a 0a20 2020  d succeeded..   
-00001420: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
-00001430: 6c74 2e6f 6b3a 0a20 2020 2020 2020 2020  lt.ok:.         
-00001440: 2020 2020 2020 2070 7269 6e74 2827 4a6f         print('Jo
-00001450: 6220 7375 626d 6974 7465 6420 7375 6363  b submitted succ
-00001460: 6573 7366 756c 6c79 2127 290a 0a20 2020  essfully!')..   
-00001470: 2020 2020 2020 2020 2023 2050 7269 6e74           # Print
-00001480: 2074 6865 206f 7574 7075 7420 6f66 2074   the output of t
-00001490: 6865 2063 6f6d 6d61 6e64 0a0a 2020 2020  he command..    
-000014a0: 2020 2020 2020 2020 7072 696e 7428 7265          print(re
-000014b0: 7375 6c74 2e73 7464 6f75 7429 0a0a 2020  sult.stdout)..  
-000014c0: 2020 4578 616d 706c 6520 323a 0a20 2020    Example 2:.   
-000014d0: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
-000014e0: 536c 7572 6d43 6c69 656e 7420 616e 6420  SlurmClient and 
-000014f0: 7365 7475 7020 536c 7572 6d20 2864 6f77  setup Slurm (dow
-00001500: 6e6c 6f61 6420 636f 6e74 6169 6e65 7273  nload containers
-00001510: 2065 7463 2e29 0a0a 2020 2020 2020 2020   etc.)..        
-00001520: 7769 7468 2053 6c75 726d 436c 6965 6e74  with SlurmClient
-00001530: 2e66 726f 6d5f 636f 6e66 6967 2869 6e69  .from_config(ini
-00001540: 745f 736c 7572 6d3d 5472 7565 2920 6173  t_slurm=True) as
-00001550: 2063 6c69 656e 743a 0a0a 2020 2020 2020   client:..      
-00001560: 2020 2020 2020 636c 6965 6e74 2e72 756e        client.run
-00001570: 5f77 6f72 6b66 6c6f 7728 2e2e 2e29 0a0a  _workflow(...)..
-00001580: 2020 2020 2222 220a 2020 2020 5f44 4546      """.    _DEF
-00001590: 4155 4c54 5f43 4f4e 4649 475f 5041 5448  AULT_CONFIG_PATH
-000015a0: 5f31 203d 2022 2f65 7463 2f73 6c75 726d  _1 = "/etc/slurm
-000015b0: 2d63 6f6e 6669 672e 696e 6922 0a20 2020  -config.ini".   
-000015c0: 205f 4445 4641 554c 545f 434f 4e46 4947   _DEFAULT_CONFIG
-000015d0: 5f50 4154 485f 3220 3d20 227e 2f73 6c75  _PATH_2 = "~/slu
-000015e0: 726d 2d63 6f6e 6669 672e 696e 6922 0a20  rm-config.ini". 
-000015f0: 2020 205f 4445 4641 554c 545f 484f 5354     _DEFAULT_HOST
-00001600: 203d 2022 736c 7572 6d22 0a20 2020 205f   = "slurm".    _
-00001610: 4445 4641 554c 545f 494e 4c49 4e45 5f53  DEFAULT_INLINE_S
-00001620: 5348 5f45 4e56 203d 2054 7275 650a 2020  SH_ENV = True.  
-00001630: 2020 5f44 4546 4155 4c54 5f53 4c55 524d    _DEFAULT_SLURM
-00001640: 5f44 4154 415f 5041 5448 203d 2022 6d79  _DATA_PATH = "my
-00001650: 2d73 6372 6174 6368 2f64 6174 6122 0a20  -scratch/data". 
-00001660: 2020 205f 4445 4641 554c 545f 534c 5552     _DEFAULT_SLUR
-00001670: 4d5f 494d 4147 4553 5f50 4154 4820 3d20  M_IMAGES_PATH = 
-00001680: 226d 792d 7363 7261 7463 682f 7369 6e67  "my-scratch/sing
-00001690: 756c 6172 6974 795f 696d 6167 6573 2f77  ularity_images/w
-000016a0: 6f72 6b66 6c6f 7773 220a 2020 2020 5f44  orkflows".    _D
-000016b0: 4546 4155 4c54 5f53 4c55 524d 5f43 4f4e  EFAULT_SLURM_CON
-000016c0: 5645 5254 4552 535f 5041 5448 203d 2022  VERTERS_PATH = "
-000016d0: 6d79 2d73 6372 6174 6368 2f73 696e 6775  my-scratch/singu
-000016e0: 6c61 7269 7479 5f69 6d61 6765 732f 636f  larity_images/co
-000016f0: 6e76 6572 7465 7273 220a 2020 2020 5f44  nverters".    _D
-00001700: 4546 4155 4c54 5f53 4c55 524d 5f47 4954  EFAULT_SLURM_GIT
-00001710: 5f53 4352 4950 545f 5041 5448 203d 2022  _SCRIPT_PATH = "
-00001720: 736c 7572 6d2d 7363 7269 7074 7322 0a20  slurm-scripts". 
-00001730: 2020 205f 4f55 545f 5345 5020 3d20 222d     _OUT_SEP = "-
-00001740: 2d73 706c 6974 2d2d 220a 2020 2020 5f56  -split--".    _V
-00001750: 4552 5349 4f4e 5f43 4d44 203d 2022 6c73  ERSION_CMD = "ls
-00001760: 202d 6820 7b73 6c75 726d 5f69 6d61 6765   -h {slurm_image
-00001770: 735f 7061 7468 7d2f 7b69 6d61 6765 5f70  s_path}/{image_p
-00001780: 6174 687d 207c 2067 7265 7020 2d6f 5020  ath} | grep -oP 
-00001790: 2728 3f3c 3d5c 2d7c 5c5f 2928 762e 2b7c  '(?<=\-|\_)(v.+|
-000017a0: 6c61 7465 7374 2928 3f3d 2e73 696d 677c  latest)(?=.simg|
-000017b0: 2e73 6966 2927 220a 2020 2020 2320 4e6f  .sif)'".    # No
-000017c0: 7465 2c20 6772 6570 2072 6574 7572 6e73  te, grep returns
-000017d0: 2065 7869 7463 6f64 6520 3120 6966 206e   exitcode 1 if n
-000017e0: 6f20 6d61 7463 6820 6973 2066 6f75 6e64  o match is found
-000017f0: 210a 2020 2020 2320 5468 6973 2077 696c  !.    # This wil
-00001800: 6c20 7472 616e 736c 6174 6520 696e 746f  l translate into
-00001810: 2061 2055 6e65 7870 6563 7465 6445 7869   a UnexpectedExi
-00001820: 7420 6572 726f 722c 2073 6f20 6d75 7465  t error, so mute
-00001830: 2074 6861 7420 6966 2079 6f75 0a20 2020   that if you.   
-00001840: 2023 2064 6f6e 2774 2063 6172 6520 6162   # don't care ab
-00001850: 6f75 7420 656d 7074 792e 0a20 2020 2023  out empty..    #
-00001860: 204c 696b 6520 6265 6c6f 7720 7769 7468   Like below with
-00001870: 2074 6865 2022 7c7c 203a 222e 0a20 2020   the "|| :"..   
-00001880: 2023 2044 6174 6120 636f 756c 6420 6c65   # Data could le
-00001890: 6769 7420 6265 2065 6d70 7479 2e0a 2020  git be empty..  
-000018a0: 2020 5f44 4154 415f 434d 4420 3d20 226c    _DATA_CMD = "l
-000018b0: 7320 2d68 207b 736c 7572 6d5f 6461 7461  s -h {slurm_data
-000018c0: 5f70 6174 687d 207c 2067 7265 7020 2d6f  _path} | grep -o
-000018d0: 5020 272e 2b28 3f3d 2e7a 6970 2927 207c  P '.+(?=.zip)' |
-000018e0: 7c20 3a22 0a20 2020 205f 414c 4c5f 4a4f  | :".    _ALL_JO
-000018f0: 4253 5f43 4d44 203d 2022 7361 6363 7420  BS_CMD = "sacct 
-00001900: 2d2d 7374 6172 7474 696d 6520 7b73 7461  --starttime {sta
-00001910: 7274 5f74 696d 657d 202d 2d65 6e64 7469  rt_time} --endti
-00001920: 6d65 207b 656e 645f 7469 6d65 7d20 2d2d  me {end_time} --
-00001930: 7374 6174 6520 7b73 7461 7465 737d 202d  state {states} -
-00001940: 6f20 7b63 6f6c 756d 6e73 7d20 2d6e 202d  o {columns} -n -
-00001950: 5820 220a 2020 2020 5f5a 4950 5f43 4d44  X ".    _ZIP_CMD
-00001960: 203d 2022 377a 2061 202d 7920 7b66 696c   = "7z a -y {fil
-00001970: 656e 616d 657d 202d 747a 6970 207b 6461  ename} -tzip {da
-00001980: 7461 5f6c 6f63 6174 696f 6e7d 2f64 6174  ta_location}/dat
-00001990: 612f 6f75 7422 0a20 2020 205f 4143 5449  a/out".    _ACTI
-000019a0: 5645 5f4a 4f42 535f 434d 4420 3d20 2273  VE_JOBS_CMD = "s
-000019b0: 7175 6575 6520 2d75 2024 5553 4552 202d  queue -u $USER -
-000019c0: 2d6e 6f68 6561 6420 2d2d 666f 726d 6174  -nohead --format
-000019d0: 2025 4622 0a20 2020 205f 4a4f 425f 5354   %F".    _JOB_ST
-000019e0: 4154 5553 5f43 4d44 203d 2022 7361 6363  ATUS_CMD = "sacc
-000019f0: 7420 2d6e 202d 6f20 4a6f 6249 642c 5374  t -n -o JobId,St
-00001a00: 6174 652c 456e 6420 2d58 202d 6a20 7b73  ate,End -X -j {s
-00001a10: 6c75 726d 5f6a 6f62 5f69 647d 220a 2020  lurm_job_id}".  
-00001a20: 2020 2320 544f 444f 206d 6f76 6520 616c    # TODO move al
-00001a30: 6c20 636f 6d6d 616e 6473 2074 6f20 6120  l commands to a 
-00001a40: 7369 6d69 6c61 7220 666f 726d 6174 2e0a  similar format..
-00001a50: 2020 2020 2320 5468 656e 206d 6179 6265      # Then maybe
-00001a60: 2061 6c6c 6f77 206f 7665 7277 7269 7465   allow overwrite
-00001a70: 2066 726f 6d20 736c 7572 6d2d 636f 6e66   from slurm-conf
-00001a80: 6967 2e69 6e69 0a20 2020 205f 4c4f 4746  ig.ini.    _LOGF
-00001a90: 494c 4520 3d20 226f 6d65 726f 2d7b 736c  ILE = "omero-{sl
-00001aa0: 7572 6d5f 6a6f 625f 6964 7d2e 6c6f 6722  urm_job_id}.log"
-00001ab0: 0a20 2020 205f 5441 494c 5f4c 4f47 5f43  .    _TAIL_LOG_C
-00001ac0: 4d44 203d 2022 7461 696c 202d 6e20 7b6e  MD = "tail -n {n
-00001ad0: 7d20 7b6c 6f67 5f66 696c 657d 207c 2073  } {log_file} | s
-00001ae0: 7472 696e 6773 220a 2020 2020 5f4c 4f47  trings".    _LOG
-00001af0: 4649 4c45 5f44 4154 415f 434d 4420 3d20  FILE_DATA_CMD = 
-00001b00: 2263 6174 207b 6c6f 675f 6669 6c65 7d20  "cat {log_file} 
-00001b10: 7c20 7065 726c 202d 776e 6520 272f 5275  | perl -wne '/Ru
-00001b20: 6e6e 696e 6720 5b5c 772d 5d2b 3f20 4a6f  nning [\w-]+? Jo
-00001b30: 6220 775c 2f20 2e2b 3f20 5c7c 202e 2b3f  b w\/ .+? \| .+?
-00001b40: 205c 7c20 282e 2b3f 2920 5c7c 2e2a 2f69   \| (.+?) \|.*/i
-00001b50: 2061 6e64 2070 7269 6e74 2431 2722 0a0a   and print$1'"..
-00001b60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001b70: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00001b80: 2020 2020 2020 2020 686f 7374 3d5f 4445          host=_DE
-00001b90: 4641 554c 545f 484f 5354 2c0a 2020 2020  FAULT_HOST,.    
-00001ba0: 2020 2020 2020 2020 2020 2020 2075 7365               use
-00001bb0: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
-00001bc0: 2020 2020 2020 2020 2070 6f72 743d 4e6f           port=No
-00001bd0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001be0: 2020 2020 2063 6f6e 6669 673d 4e6f 6e65       config=None
-00001bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001c00: 2020 2067 6174 6577 6179 3d4e 6f6e 652c     gateway=None,
-00001c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c20: 2020 666f 7277 6172 645f 6167 656e 743d    forward_agent=
-00001c30: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001c40: 2020 2020 2020 2063 6f6e 6e65 6374 5f74         connect_t
-00001c50: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
-00001c60: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001c70: 6e6e 6563 745f 6b77 6172 6773 3d4e 6f6e  nnect_kwargs=Non
-00001c80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001c90: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
-00001ca0: 6e76 3d5f 4445 4641 554c 545f 494e 4c49  nv=_DEFAULT_INLI
-00001cb0: 4e45 5f53 5348 5f45 4e56 2c0a 2020 2020  NE_SSH_ENV,.    
-00001cc0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00001cd0: 726d 5f64 6174 615f 7061 7468 3a20 7374  rm_data_path: st
-00001ce0: 7220 3d20 5f44 4546 4155 4c54 5f53 4c55  r = _DEFAULT_SLU
-00001cf0: 524d 5f44 4154 415f 5041 5448 2c0a 2020  RM_DATA_PATH,.  
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001d10: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-00001d20: 3a20 7374 7220 3d20 5f44 4546 4155 4c54  : str = _DEFAULT
-00001d30: 5f53 4c55 524d 5f49 4d41 4745 535f 5041  _SLURM_IMAGES_PA
-00001d40: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
-00001d50: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
-00001d60: 7274 6572 735f 7061 7468 3a20 7374 7220  rters_path: str 
-00001d70: 3d20 5f44 4546 4155 4c54 5f53 4c55 524d  = _DEFAULT_SLURM
-00001d80: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
-00001d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001da0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-00001db0: 6174 6873 3a20 6469 6374 203d 204e 6f6e  aths: dict = Non
-00001dc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001dd0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00001de0: 7265 706f 733a 2064 6963 7420 3d20 4e6f  repos: dict = No
-00001df0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001e00: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-00001e10: 5f69 6d61 6765 733a 2064 6963 7420 3d20  _images: dict = 
-00001e20: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001e30: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00001e40: 656c 5f6a 6f62 733a 2064 6963 7420 3d20  el_jobs: dict = 
-00001e50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001e60: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00001e70: 656c 5f6a 6f62 735f 7061 7261 6d73 3a20  el_jobs_params: 
-00001e80: 6469 6374 203d 204e 6f6e 652c 0a20 2020  dict = None,.   
-00001e90: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00001ea0: 7572 6d5f 7363 7269 7074 5f70 6174 683a  urm_script_path:
-00001eb0: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
-00001ec0: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
-00001ed0: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
-00001ee0: 2020 2020 2020 2020 736c 7572 6d5f 7363          slurm_sc
-00001ef0: 7269 7074 5f72 6570 6f3a 2073 7472 203d  ript_repo: str =
-00001f00: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00001f10: 2020 2020 2020 2020 696e 6974 5f73 6c75          init_slu
-00001f20: 726d 3a20 626f 6f6c 203d 2046 616c 7365  rm: bool = False
-00001f30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f40: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00001f50: 2249 6e69 7469 616c 697a 6573 2061 206e  "Initializes a n
-00001f60: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
-00001f70: 6865 2053 6c75 726d 436c 6965 6e74 2063  he SlurmClient c
-00001f80: 6c61 7373 2e0a 0a20 2020 2020 2020 2049  lass...        I
-00001f90: 7420 6973 2070 7265 6665 7261 626c 6520  t is preferable 
-00001fa0: 746f 2075 7365 2023 6672 6f6d 5f63 6f6e  to use #from_con
-00001fb0: 6669 6728 2e2e 2e29 206d 6574 686f 6420  fig(...) method 
-00001fc0: 746f 2069 6e69 7469 616c 697a 650a 2020  to initialize.  
-00001fd0: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
-00001fe0: 2066 726f 6d20 6120 636f 6e66 6967 2066   from a config f
-00001ff0: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
-00002000: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00002010: 686f 7374 2028 7374 722c 206f 7074 696f  host (str, optio
-00002020: 6e61 6c29 3a20 5468 6520 686f 7374 6e61  nal): The hostna
-00002030: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
-00002040: 206f 6620 7468 6520 7265 6d6f 7465 0a20   of the remote. 
-00002050: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002060: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
-00002070: 746f 205f 4445 4641 554c 545f 484f 5354  to _DEFAULT_HOST
-00002080: 2e0a 2020 2020 2020 2020 2020 2020 7573  ..            us
-00002090: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-000020a0: 6c29 3a20 5468 6520 7573 6572 6e61 6d65  l): The username
-000020b0: 2074 6f20 7573 6520 7768 656e 2063 6f6e   to use when con
-000020c0: 6e65 6374 696e 6720 746f 200a 2020 2020  necting to .    
-000020d0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-000020e0: 7265 6d6f 7465 2073 6572 7665 722e 2044  remote server. D
-000020f0: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
-00002100: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
-00002110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002120: 2074 6f20 636f 6e66 6967 2e75 7365 722e   to config.user.
-00002130: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
-00002140: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-00002150: 293a 2054 6865 2053 5348 2070 6f72 7420  ): The SSH port 
-00002160: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
-00002170: 6563 7469 6e67 2e0a 2020 2020 2020 2020  ecting..        
-00002180: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00002190: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
-000021a0: 6465 6661 756c 7473 2074 6f20 636f 6e66  defaults to conf
-000021b0: 6967 2e70 6f72 742e 0a20 2020 2020 2020  ig.port..       
-000021c0: 2020 2020 2063 6f6e 6669 6720 2873 7472       config (str
-000021d0: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
-000021e0: 6820 746f 2074 6865 2053 5348 2063 6f6e  h to the SSH con
-000021f0: 6669 6720 6669 6c65 2e0a 2020 2020 2020  fig file..      
-00002200: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00002210: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
-00002220: 6820 6465 6661 756c 7473 2074 6f20 796f  h defaults to yo
-00002230: 7572 2053 5348 2063 6f6e 6669 6720 6669  ur SSH config fi
-00002240: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-00002250: 6761 7465 7761 7920 2843 6f6e 6e65 6374  gateway (Connect
-00002260: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-00002270: 416e 206f 7074 696f 6e61 6c20 6761 7465  An optional gate
-00002280: 7761 7920 666f 7220 636f 6e6e 6563 7469  way for connecti
-00002290: 6e67 200a 2020 2020 2020 2020 2020 2020  ng .            
-000022a0: 2020 2020 7468 726f 7567 6820 6120 6a75      through a ju
-000022b0: 6d70 2068 6f73 742e 2044 6566 6175 6c74  mp host. Default
-000022c0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-000022d0: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
-000022e0: 6765 6e74 2028 626f 6f6c 2c20 6f70 7469  gent (bool, opti
-000022f0: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
-00002300: 6f20 666f 7277 6172 6420 7468 6520 6c6f  o forward the lo
-00002310: 6361 6c20 5353 4820 0a20 2020 2020 2020  cal SSH .       
-00002320: 2020 2020 2020 2020 2061 6765 6e74 2074           agent t
-00002330: 6f20 7468 6520 7265 6d6f 7465 2073 6572  o the remote ser
-00002340: 7665 722e 2044 6566 6175 6c74 7320 746f  ver. Defaults to
-00002350: 204e 6f6e 652c 2077 6869 6368 200a 2020   None, which .  
-00002360: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00002370: 6661 756c 7473 2074 6f20 636f 6e66 6967  faults to config
-00002380: 2e66 6f72 7761 7264 5f61 6765 6e74 2e0a  .forward_agent..
-00002390: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-000023a0: 6563 745f 7469 6d65 6f75 7420 2869 6e74  ect_timeout (int
-000023b0: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
-000023c0: 656f 7574 2066 6f72 2065 7374 6162 6c69  eout for establi
-000023d0: 7368 696e 6720 7468 6520 5353 4820 0a20  shing the SSH . 
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000023f0: 6f6e 6e65 6374 696f 6e2e 2044 6566 6175  onnection. Defau
-00002400: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
-00002410: 6368 2064 6566 6175 6c74 7320 0a20 2020  ch defaults .   
-00002420: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-00002430: 636f 6e66 6967 2e74 696d 656f 7574 732e  config.timeouts.
-00002440: 636f 6e6e 6563 742e 0a20 2020 2020 2020  connect..       
-00002450: 2020 2020 2063 6f6e 6e65 6374 5f6b 7761       connect_kwa
-00002460: 7267 7320 2864 6963 742c 206f 7074 696f  rgs (dict, optio
-00002470: 6e61 6c29 3a20 4164 6469 7469 6f6e 616c  nal): Additional
-00002480: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00002490: 7473 2066 6f72 200a 2020 2020 2020 2020  ts for .        
-000024a0: 2020 2020 2020 2020 7468 6520 756e 6465          the unde
-000024b0: 726c 7969 6e67 2053 5348 2063 6f6e 6e65  rlying SSH conne
-000024c0: 6374 696f 6e2e 2048 616e 6465 6420 7665  ction. Handed ve
-000024d0: 7262 6174 696d 2074 6f20 0a20 2020 2020  rbatim to .     
-000024e0: 2020 2020 2020 2020 2020 2060 5353 4843             `SSHC
-000024f0: 6c69 656e 742e 636f 6e6e 6563 7420 3c70  lient.connect <p
-00002500: 6172 616d 696b 6f2e 636c 6965 6e74 2e53  aramiko.client.S
-00002510: 5348 436c 6965 6e74 2e63 6f6e 6e65 6374  SHClient.connect
-00002520: 3e60 2e20 0a20 2020 2020 2020 2020 2020  >`. .           
-00002530: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00002540: 204e 6f6e 652e 200a 2020 2020 2020 2020   None. .        
-00002550: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
-00002560: 6e76 2028 626f 6f6c 2c20 6f70 7469 6f6e  nv (bool, option
-00002570: 616c 293a 2057 6865 7468 6572 2074 6f20  al): Whether to 
-00002580: 7573 6520 696e 6c69 6e65 2053 5348 0a20  use inline SSH. 
-00002590: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000025a0: 6e76 6972 6f6e 6d65 6e74 2e20 5468 6973  nvironment. This
-000025b0: 2069 7320 6e65 6365 7373 6172 7920 6966   is necessary if
-000025c0: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
-000025d0: 6572 2068 6173 200a 2020 2020 2020 2020  er has .        
-000025e0: 2020 2020 2020 2020 6120 7265 7374 7269          a restri
-000025f0: 6374 6564 2060 6041 6363 6570 7445 6e76  cted ``AcceptEnv
-00002600: 6060 2073 6574 7469 6e67 2028 7768 6963  `` setting (whic
-00002610: 6820 6973 2074 6865 2063 6f6d 6d6f 6e20  h is the common 
-00002620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002630: 2064 6566 6175 6c74 292e 2044 6566 6175   default). Defau
-00002640: 6c74 7320 746f 205f 4445 4641 554c 545f  lts to _DEFAULT_
-00002650: 494e 4c49 4e45 5f53 5348 5f45 4e56 2e0a  INLINE_SSH_ENV..
-00002660: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-00002670: 6d5f 6461 7461 5f70 6174 6820 2873 7472  m_data_path (str
-00002680: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00002690: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
-000026a0: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
-000026b0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-000026c0: 6720 7468 6520 6461 7461 2066 696c 6573  g the data files
-000026d0: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
-000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026f0: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
-00002700: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
-00002710: 5f50 4154 482e 0a20 2020 2020 2020 2020  _PATH..         
-00002720: 2020 2073 6c75 726d 5f69 6d61 6765 735f     slurm_images_
-00002730: 7061 7468 2028 7374 722c 206f 7074 696f  path (str, optio
-00002740: 6e61 6c29 3a20 5468 6520 7061 7468 2074  nal): The path t
-00002750: 6f20 7468 6520 6469 7265 6374 6f72 790a  o the directory.
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 636f 6e74 6169 6e69 6e67 2074 6865 2053  containing the S
-00002780: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
-00002790: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
-000027a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000027b0: 2020 4465 6661 756c 7473 2074 6f20 5f44    Defaults to _D
-000027c0: 4546 4155 4c54 5f53 4c55 524d 5f49 4d41  EFAULT_SLURM_IMA
-000027d0: 4745 535f 5041 5448 2e0a 2020 2020 2020  GES_PATH..      
-000027e0: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
-000027f0: 6572 7465 7273 5f70 6174 6820 2873 7472  erters_path (str
-00002800: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00002810: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
-00002820: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
-00002830: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-00002840: 6720 7468 6520 5369 6e67 756c 6172 6974  g the Singularit
-00002850: 7920 696d 6167 6573 2066 6f72 2066 696c  y images for fil
-00002860: 6520 636f 6e76 6572 7465 7273 2e0a 2020  e converters..  
-00002870: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00002880: 6661 756c 7473 2074 6f20 5f44 4546 4155  faults to _DEFAU
-00002890: 4c54 5f53 4c55 524d 5f43 4f4e 5645 5254  LT_SLURM_CONVERT
-000028a0: 4552 535f 5041 5448 2e0a 2020 2020 2020  ERS_PATH..      
-000028b0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-000028c0: 6c5f 7061 7468 7320 2864 6963 742c 206f  l_paths (dict, o
-000028d0: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
-000028e0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-000028f0: 6720 7468 6520 0a20 2020 2020 2020 2020  g the .         
-00002900: 2020 2020 2020 2070 6174 6873 2074 6f20         paths to 
-00002910: 7468 6520 5369 6e67 756c 6172 6974 7920  the Singularity 
-00002920: 696d 6167 6573 2066 6f72 2073 7065 6369  images for speci
-00002930: 6669 6320 536c 7572 6d20 6a6f 6220 6d6f  fic Slurm job mo
-00002940: 6465 6c73 2e0a 2020 2020 2020 2020 2020  dels..          
-00002950: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002960: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
-00002970: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00002980: 7265 706f 7320 2864 6963 742c 206f 7074  repos (dict, opt
-00002990: 696f 6e61 6c29 3a20 4120 6469 6374 696f  ional): A dictio
-000029a0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-000029b0: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
-000029c0: 2020 2020 2067 6974 2072 6570 6f73 6974       git reposit
-000029d0: 6f72 6965 7320 6f66 2053 696e 6775 6c61  ories of Singula
-000029e0: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
-000029f0: 7370 6563 6966 6963 2053 6c75 726d 200a  specific Slurm .
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
-00002a20: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00002a30: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00002a40: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-00002a50: 6d6f 6465 6c5f 696d 6167 6573 2028 6469  model_images (di
-00002a60: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
-00002a70: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-00002a80: 6169 6e69 6e67 2074 6865 200a 2020 2020  aining the .    
-00002a90: 2020 2020 2020 2020 2020 2020 646f 636b              dock
-00002aa0: 6572 6875 6220 6f66 2074 6865 2053 696e  erhub of the Sin
-00002ab0: 6775 6c61 7269 7479 2069 6d61 6765 7320  gularity images 
-00002ac0: 666f 7220 7370 6563 6966 6963 2053 6c75  for specific Slu
-00002ad0: 726d 200a 2020 2020 2020 2020 2020 2020  rm .            
-00002ae0: 2020 2020 6a6f 6220 6d6f 6465 6c73 2e20      job models. 
-00002af0: 5769 6c6c 2066 696c 6c20 6175 746f 6d61  Will fill automa
-00002b00: 7469 6361 6c6c 7920 6672 6f6d 2074 6865  tically from the
-00002b10: 2064 6174 6120 696e 2074 6865 2067 6974   data in the git
-00002b20: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002b30: 2020 7265 706f 7369 746f 7279 2069 6620    repository if 
-00002b40: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
-00002b50: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
-00002b60: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002b70: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002b80: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00002b90: 6273 2028 6469 6374 2c20 6f70 7469 6f6e  bs (dict, option
-00002ba0: 616c 293a 2041 2064 6963 7469 6f6e 6172  al): A dictionar
-00002bb0: 7920 636f 6e74 6169 6e69 6e67 0a20 2020  y containing.   
-00002bc0: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00002bd0: 6f72 6d61 7469 6f6e 2061 626f 7574 2073  ormation about s
-00002be0: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
-00002bf0: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
-00002c00: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00002c10: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00002c20: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00002c30: 6465 6c5f 6a6f 6273 5f70 6172 616d 7320  del_jobs_params 
-00002c40: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
-00002c50: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
-00002c60: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
-00002c70: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
-00002c80: 7465 7273 2066 6f72 2073 7065 6369 6669  ters for specifi
-00002c90: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
-00002ca0: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
-00002cb0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002cc0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002cd0: 2020 736c 7572 6d5f 7363 7269 7074 5f70    slurm_script_p
-00002ce0: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
-00002cf0: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
-00002d00: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002d20: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
-00002d30: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
-00002d40: 6f6e 2073 6372 6970 7473 206f 6e20 536c  on scripts on Sl
-00002d50: 7572 6d2e 0a20 2020 2020 2020 2020 2020  urm..           
-00002d60: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00002d70: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
-00002d80: 4749 545f 5343 5249 5054 5f50 4154 482e  GIT_SCRIPT_PATH.
-00002d90: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
-00002da0: 726d 5f73 6372 6970 745f 7265 706f 2028  rm_script_repo (
-00002db0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00002dc0: 5468 6520 6769 7420 6874 7470 7320 5552  The git https UR
-00002dd0: 4c20 666f 7220 636c 6f6e 696e 670a 2020  L for cloning.  
-00002de0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00002df0: 6520 7265 706f 2063 6f6e 7461 696e 696e  e repo containin
-00002e00: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
-00002e10: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
-00002e20: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00002e30: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00002e40: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
-00002e50: 2020 696e 6974 5f73 6c75 726d 2028 626f    init_slurm (bo
-00002e60: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
-00002e70: 7365 7420 7570 2074 6865 2072 6571 7569  set up the requi
-00002e80: 7265 6420 7374 7275 6374 7572 6573 200a  red structures .
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 6f6e 2053 6c75 726d 2061 6674 6572 2069  on Slurm after i
-00002eb0: 6e69 7469 6174 696e 6720 7468 6973 2063  nitiating this c
-00002ec0: 6c69 656e 742e 2054 6869 7320 696e 636c  lient. This incl
-00002ed0: 7564 6573 2063 7265 6174 696e 6720 0a20  udes creating . 
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00002ef0: 6973 7369 6e67 2066 6f6c 6465 7273 2c20  issing folders, 
-00002f00: 646f 776e 6c6f 6164 696e 6720 636f 6e74  downloading cont
-00002f10: 6169 6e65 7220 696d 6167 6573 2c20 636c  ainer images, cl
-00002f20: 6f6e 696e 6720 6769 742c 6574 632e 0a20  oning git,etc.. 
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00002f40: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
-00002f50: 7768 696c 6520 6174 2066 6972 7374 2062  while at first b
-00002f60: 7574 2077 696c 6c20 7661 6c69 6461 7465  ut will validate
-00002f70: 2079 6f75 7220 7365 7475 702e 0a20 2020   your setup..   
-00002f80: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00002f90: 6175 6c74 7320 746f 2046 616c 7365 2074  aults to False t
-00002fa0: 6f20 7361 7665 2074 696d 652e 0a20 2020  o save time..   
-00002fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002fc0: 2073 7570 6572 2853 6c75 726d 436c 6965   super(SlurmClie
-00002fd0: 6e74 2c20 7365 6c66 292e 5f5f 696e 6974  nt, self).__init
-00002fe0: 5f5f 2868 6f73 742c 0a20 2020 2020 2020  __(host,.       
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 2020 2020 2020 2020 2243 4f4d 504c 4554          "COMPLET
+000007e0: 4544 222c 200a 2020 2020 2020 2020 2020  ED", .          
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 2020 2022 4341 4e43             "CANC
+00000810: 454c 4c45 4422 2c0a 2020 2020 2020 2020  ELLED",.        
+00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000830: 2020 2020 2020 2020 2020 2020 2022 5449               "TI
+00000840: 4d45 4f55 5422 2c0a 2020 2020 2020 2020  MEOUT",.        
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 2020 2020 2020 2020 2020 2020 2022 4641               "FA
+00000870: 494c 4544 2b22 2c20 0a20 2020 2020 2020  ILED+", .       
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+000008a0: 4f4d 504c 4554 4544 2b22 2c20 0a20 2020  OMPLETED+", .   
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2243 414e 4345 4c4c 4544 2b22 2c0a    "CANCELLED+",.
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 2020 2022 5449 4d45 4f55 542b 2229       "TIMEOUT+")
+00000910: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+00000920: 625f 7374 6174 7573 5f64 6963 742c 2070  b_status_dict, p
+00000930: 6f6c 6c5f 7265 7375 6c74 203d 2073 6c75  oll_result = slu
+00000940: 726d 436c 6965 6e74 2e63 6865 636b 5f6a  rmClient.check_j
+00000950: 6f62 5f73 7461 7475 7328 0a20 2020 2020  ob_status(.     
+00000960: 2020 2020 2020 2020 2020 205b 7365 6c66             [self
+00000970: 2e6a 6f62 5f69 645d 290a 2020 2020 2020  .job_id]).      
+00000980: 2020 2020 2020 6966 206e 6f74 2070 6f6c        if not pol
+00000990: 6c5f 7265 7375 6c74 2e6f 6b3a 0a20 2020  l_result.ok:.   
+000009a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000009b0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2066 2245 7272 6f72 2063 6865 636b 696e   f"Error checkin
+000009e0: 6720 6a6f 6220 7374 6174 7573 3a7b 706f  g job status:{po
+000009f0: 6c6c 5f72 6573 756c 742e 7374 6465 7272  ll_result.stderr
+00000a00: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00000a10: 2020 2020 7365 6c66 2e6a 6f62 5f73 7461      self.job_sta
+00000a20: 7465 203d 2022 4641 494c 4544 220a 2020  te = "FAILED".  
+00000a30: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+00000a40: 6f62 5f73 7461 7465 203d 206a 6f62 5f73  ob_state = job_s
+00000a50: 7461 7475 735f 6469 6374 5b73 656c 662e  tatus_dict[self.
+00000a60: 6a6f 625f 6964 5d0a 2020 2020 2020 2020  job_id].        
+00000a70: 2020 2020 2320 7761 6974 2066 6f72 2031      # wait for 1
+00000a80: 3020 7365 636f 6e64 7320 6265 666f 7265  0 seconds before
+00000a90: 2063 6865 636b 696e 6720 6167 6169 6e0a   checking again.
+00000aa0: 2020 2020 2020 2020 2020 2020 6f6d 6572              omer
+00000ab0: 6f43 6f6e 6e2e 6b65 6570 416c 6976 6528  oConn.keepAlive(
+00000ac0: 2920 2023 206b 6565 7020 7468 6520 4f4d  )  # keep the OM
+00000ad0: 4552 4f20 636f 6e6e 6563 7469 6f6e 2061  ERO connection a
+00000ae0: 6c69 7665 0a20 2020 2020 2020 2020 2020  live.           
+00000af0: 2074 696d 6573 6c65 6570 2e73 6c65 6570   timesleep.sleep
+00000b00: 2831 3029 0a20 2020 2020 2020 206c 6f67  (10).        log
+00000b10: 6765 722e 696e 666f 2866 224a 6f62 207b  ger.info(f"Job {
+00000b20: 7365 6c66 2e6a 6f62 5f69 647d 2066 696e  self.job_id} fin
+00000b30: 6973 6865 643a 207b 7365 6c66 2e6a 6f62  ished: {self.job
+00000b40: 5f73 7461 7465 7d22 290a 2020 2020 2020  _state}").      
+00000b50: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
+00000b60: 2020 2020 2020 2020 2020 2066 2259 6f75             f"You
+00000b70: 2063 616e 2067 6574 2074 6865 206c 6f67   can get the log
+00000b80: 6669 6c65 2075 7369 6e67 2060 536c 7572  file using `Slur
+00000b90: 6d20 4765 7420 5570 6461 7465 6020 6f6e  m Get Update` on
+00000ba0: 206a 6f62 207b 7365 6c66 2e6a 6f62 5f69   job {self.job_i
+00000bb0: 647d 2229 0a20 2020 2020 2020 2072 6574  d}").        ret
+00000bc0: 7572 6e20 7365 6c66 2e6a 6f62 5f73 7461  urn self.job_sta
+00000bd0: 7465 0a0a 2020 2020 6465 6620 636f 6d70  te..    def comp
+00000be0: 6c65 7465 6428 7365 6c66 293a 0a20 2020  leted(self):.   
+00000bf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00000c00: 2043 6865 636b 2069 6620 7468 6520 536c   Check if the Sl
+00000c10: 7572 6d20 6a6f 6220 6861 7320 636f 6d70  urm job has comp
+00000c20: 6c65 7465 6420 7375 6363 6573 7366 756c  leted successful
+00000c30: 6c79 2e0a 0a20 2020 2020 2020 2052 6574  ly...        Ret
+00000c40: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00000c50: 2020 626f 6f6c 3a20 5472 7565 2069 6620    bool: True if 
+00000c60: 7468 6520 6a6f 6220 6861 7320 636f 6d70  the job has comp
+00000c70: 6c65 7465 643b 2046 616c 7365 206f 7468  leted; False oth
+00000c80: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
+00000c90: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00000ca0: 726e 2073 656c 662e 6a6f 625f 7374 6174  rn self.job_stat
+00000cb0: 6520 3d3d 2022 434f 4d50 4c45 5445 4422  e == "COMPLETED"
+00000cc0: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00000cd0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00000ce0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00000cf0: 7572 6e20 6120 7374 7269 6e67 2072 6570  urn a string rep
+00000d00: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+00000d10: 6865 2053 6c75 726d 4a6f 6220 696e 7374  he SlurmJob inst
+00000d20: 616e 6365 2e0a 0a20 2020 2020 2020 2052  ance...        R
+00000d30: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00000d40: 2020 2020 7374 723a 2053 7472 696e 6720      str: String 
+00000d50: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
+00000d60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000d70: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
+00000d80: 2027 2c20 272e 6a6f 696e 280a 2020 2020   ', '.join(.    
+00000d90: 2020 2020 2020 2020 6622 7b6b 6579 7d3d          f"{key}=
+00000da0: 7b76 616c 7565 7d22 2066 6f72 206b 6579  {value}" for key
+00000db0: 2c20 7661 6c75 6520 696e 2073 656c 662e  , value in self.
+00000dc0: 5f5f 6469 6374 5f5f 2e69 7465 6d73 2829  __dict__.items()
+00000dd0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00000de0: 2066 2253 6c75 726d 4a6f 6228 7b70 726f   f"SlurmJob({pro
+00000df0: 7065 7274 6965 737d 2922 0a0a 0a63 6c61  perties})"...cla
+00000e00: 7373 2053 6c75 726d 436c 6965 6e74 2843  ss SlurmClient(C
+00000e10: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+00000e20: 2222 2241 2063 6c69 656e 7420 666f 7220  """A client for 
+00000e30: 636f 6e6e 6563 7469 6e67 2074 6f20 616e  connecting to an
+00000e40: 6420 696e 7465 7261 6374 696e 6720 7769  d interacting wi
+00000e50: 7468 2061 2053 6c75 726d 2063 6c75 7374  th a Slurm clust
+00000e60: 6572 206f 7665 720a 2020 2020 5353 482e  er over.    SSH.
+00000e70: 0a0a 2020 2020 5468 6973 2063 6c61 7373  ..    This class
+00000e80: 2065 7874 656e 6473 2074 6865 2043 6f6e   extends the Con
+00000e90: 6e65 6374 696f 6e20 636c 6173 732c 2061  nection class, a
+00000ea0: 6464 696e 6720 6d65 7468 6f64 7320 616e  dding methods an
+00000eb0: 640a 2020 2020 6174 7472 6962 7574 6573  d.    attributes
+00000ec0: 2073 7065 6369 6669 6320 746f 2077 6f72   specific to wor
+00000ed0: 6b69 6e67 2077 6974 6820 536c 7572 6d2e  king with Slurm.
+00000ee0: 0a0a 2020 2020 536c 7572 6d43 6c69 656e  ..    SlurmClien
+00000ef0: 7420 6163 6365 7074 7320 7468 6520 7361  t accepts the sa
+00000f00: 6d65 2061 7267 756d 656e 7473 2061 7320  me arguments as 
+00000f10: 436f 6e6e 6563 7469 6f6e 2e20 4265 6c6f  Connection. Belo
+00000f20: 7720 6f6e 6c79 0a20 2020 206d 656e 7469  w only.    menti
+00000f30: 6f6e 7320 7468 6520 6164 6465 6420 6f6e  ons the added on
+00000f40: 6573 3a0a 0a20 2020 2054 6865 2065 6173  es:..    The eas
+00000f50: 6965 7374 2077 6179 2074 6f20 7365 7420  iest way to set 
+00000f60: 7468 6973 2063 6c69 656e 7420 7570 2069  this client up i
+00000f70: 7320 6279 2075 7369 6e67 2061 2073 6c75  s by using a slu
+00000f80: 726d 2d63 6f6e 6669 672e 696e 690a 2020  rm-config.ini.  
+00000f90: 2020 616e 6420 7468 6520 6672 6f6d 2d63    and the from-c
+00000fa0: 6f6e 6669 6728 2920 6d65 7468 6f64 2e0a  onfig() method..
+00000fb0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+00000fc0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
+00000fd0: 6174 615f 7061 7468 2028 7374 7229 3a20  ata_path (str): 
+00000fe0: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
+00000ff0: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
+00001000: 6e69 6e67 2074 6865 0a20 2020 2020 2020  ning the.       
+00001010: 2020 2020 2064 6174 6120 6669 6c65 7320       data files 
+00001020: 666f 7220 536c 7572 6d20 6a6f 6273 2e0a  for Slurm jobs..
+00001030: 2020 2020 2020 2020 736c 7572 6d5f 696d          slurm_im
+00001040: 6167 6573 5f70 6174 6820 2873 7472 293a  ages_path (str):
+00001050: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
+00001060: 2064 6972 6563 746f 7279 2063 6f6e 7461   directory conta
+00001070: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
+00001080: 2020 7468 6520 5369 6e67 756c 6172 6974    the Singularit
+00001090: 7920 696d 6167 6573 2066 6f72 2053 6c75  y images for Slu
+000010a0: 726d 206a 6f62 732e 0a20 2020 2020 2020  rm jobs..       
+000010b0: 2073 6c75 726d 5f63 6f6e 7665 7274 6572   slurm_converter
+000010c0: 735f 7061 7468 2028 7374 7229 3a20 5468  s_path (str): Th
+000010d0: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
+000010e0: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
+000010f0: 6e67 0a20 2020 2020 2020 2020 2020 2074  ng.            t
+00001100: 6865 2053 696e 6775 6c61 7269 7479 2069  he Singularity i
+00001110: 6d61 6765 7320 666f 7220 6669 6c65 2063  mages for file c
+00001120: 6f6e 7665 7274 6572 732e 0a20 2020 2020  onverters..     
+00001130: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00001140: 6174 6873 2028 6469 6374 293a 2041 2064  aths (dict): A d
+00001150: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+00001160: 6e69 6e67 2074 6865 2070 6174 6873 2074  ning the paths t
+00001170: 6f0a 2020 2020 2020 2020 2020 2020 7468  o.            th
+00001180: 6520 5369 6e67 756c 6172 6974 7920 696d  e Singularity im
+00001190: 6167 6573 2066 6f72 2073 7065 6369 6669  ages for specifi
+000011a0: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
+000011b0: 6c73 2e0a 2020 2020 2020 2020 736c 7572  ls..        slur
+000011c0: 6d5f 6d6f 6465 6c5f 7265 706f 7320 2864  m_model_repos (d
+000011d0: 6963 7429 3a20 4120 6469 6374 696f 6e61  ict): A dictiona
+000011e0: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
+000011f0: 6520 6769 740a 2020 2020 2020 2020 2020  e git.          
+00001200: 2020 7265 706f 7369 746f 7269 6573 206f    repositories o
+00001210: 6620 5369 6e67 756c 6172 6974 7920 696d  f Singularity im
+00001220: 6167 6573 2066 6f72 2073 7065 6369 6669  ages for specifi
+00001230: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
+00001240: 6c73 2e0a 2020 2020 2020 2020 736c 7572  ls..        slur
+00001250: 6d5f 6d6f 6465 6c5f 696d 6167 6573 2028  m_model_images (
+00001260: 6469 6374 293a 2041 2064 6963 7469 6f6e  dict): A diction
+00001270: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+00001280: 6865 2064 6f63 6b65 7268 7562 0a20 2020  he dockerhub.   
+00001290: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+000012a0: 5369 6e67 756c 6172 6974 7920 696d 6167  Singularity imag
+000012b0: 6573 2066 6f72 2073 7065 6369 6669 6320  es for specific 
+000012c0: 536c 7572 6d20 6a6f 6220 6d6f 6465 6c73  Slurm job models
+000012d0: 2e0a 2020 2020 2020 2020 2020 2020 5769  ..            Wi
+000012e0: 6c6c 2066 696c 6c20 6175 746f 6d61 7469  ll fill automati
+000012f0: 6361 6c6c 7920 6672 6f6d 2074 6865 2064  cally from the d
+00001300: 6174 6120 696e 2074 6865 2067 6974 2072  ata in the git r
+00001310: 6570 6f73 6974 6f72 792c 0a20 2020 2020  epository,.     
+00001320: 2020 2020 2020 2069 6620 796f 7520 7365         if you se
+00001330: 7420 696e 6974 5f73 6c75 726d 2e0a 2020  t init_slurm..  
+00001340: 2020 2020 2020 736c 7572 6d5f 7363 7269        slurm_scri
+00001350: 7074 5f70 6174 6820 2873 7472 293a 2054  pt_path (str): T
+00001360: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
+00001370: 6972 6563 746f 7279 2063 6f6e 7461 696e  irectory contain
+00001380: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00001390: 7468 6520 536c 7572 6d20 6a6f 6220 7375  the Slurm job su
+000013a0: 626d 6973 7369 6f6e 2073 6372 6970 7473  bmission scripts
+000013b0: 206f 6e20 536c 7572 6d2e 0a20 2020 2020   on Slurm..     
+000013c0: 2020 2073 6c75 726d 5f73 6372 6970 745f     slurm_script_
+000013d0: 7265 706f 2028 7374 7229 3a20 5468 6520  repo (str): The 
+000013e0: 6769 7420 6874 7470 7320 5552 4c20 666f  git https URL fo
+000013f0: 7220 636c 6f6e 696e 6720 7468 6520 7265  r cloning the re
+00001400: 706f 0a20 2020 2020 2020 2020 2020 2063  po.            c
+00001410: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00001420: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
+00001430: 6f6e 2073 6372 6970 7473 2e20 4f70 7469  on scripts. Opti
+00001440: 6f6e 616c 2e0a 0a20 2020 2045 7861 6d70  onal...    Examp
+00001450: 6c65 3a0a 2020 2020 2020 2020 2320 4372  le:.        # Cr
+00001460: 6561 7465 2061 2053 6c75 726d 436c 6965  eate a SlurmClie
+00001470: 6e74 206f 626a 6563 7420 6173 2063 6f6e  nt object as con
+00001480: 7465 7874 6d61 6e61 6765 720a 0a20 2020  textmanager..   
+00001490: 2020 2020 2077 6974 6820 536c 7572 6d43       with SlurmC
+000014a0: 6c69 656e 742e 6672 6f6d 5f63 6f6e 6669  lient.from_confi
+000014b0: 6728 2920 6173 2063 6c69 656e 743a 0a0a  g() as client:..
+000014c0: 2020 2020 2020 2020 2020 2020 2320 5275              # Ru
+000014d0: 6e20 6120 636f 6d6d 616e 6420 6f6e 2074  n a command on t
+000014e0: 6865 2072 656d 6f74 6520 686f 7374 0a0a  he remote host..
+000014f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00001500: 6c74 203d 2063 6c69 656e 742e 7275 6e28  lt = client.run(
+00001510: 2773 6261 7463 6820 6d79 6a6f 622e 7368  'sbatch myjob.sh
+00001520: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
+00001530: 2320 4368 6563 6b20 7768 6574 6865 7220  # Check whether 
+00001540: 7468 6520 636f 6d6d 616e 6420 7375 6363  the command succ
+00001550: 6565 6465 640a 0a20 2020 2020 2020 2020  eeded..         
+00001560: 2020 2069 6620 7265 7375 6c74 2e6f 6b3a     if result.ok:
+00001570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001580: 2070 7269 6e74 2827 4a6f 6220 7375 626d   print('Job subm
+00001590: 6974 7465 6420 7375 6363 6573 7366 756c  itted successful
+000015a0: 6c79 2127 290a 0a20 2020 2020 2020 2020  ly!')..         
+000015b0: 2020 2023 2050 7269 6e74 2074 6865 206f     # Print the o
+000015c0: 7574 7075 7420 6f66 2074 6865 2063 6f6d  utput of the com
+000015d0: 6d61 6e64 0a0a 2020 2020 2020 2020 2020  mand..          
+000015e0: 2020 7072 696e 7428 7265 7375 6c74 2e73    print(result.s
+000015f0: 7464 6f75 7429 0a0a 2020 2020 4578 616d  tdout)..    Exam
+00001600: 706c 6520 323a 0a20 2020 2020 2020 2023  ple 2:.        #
+00001610: 2043 7265 6174 6520 6120 536c 7572 6d43   Create a SlurmC
+00001620: 6c69 656e 7420 616e 6420 7365 7475 7020  lient and setup 
+00001630: 536c 7572 6d20 2864 6f77 6e6c 6f61 6420  Slurm (download 
+00001640: 636f 6e74 6169 6e65 7273 2065 7463 2e29  containers etc.)
+00001650: 0a0a 2020 2020 2020 2020 7769 7468 2053  ..        with S
+00001660: 6c75 726d 436c 6965 6e74 2e66 726f 6d5f  lurmClient.from_
+00001670: 636f 6e66 6967 2869 6e69 745f 736c 7572  config(init_slur
+00001680: 6d3d 5472 7565 2920 6173 2063 6c69 656e  m=True) as clien
+00001690: 743a 0a0a 2020 2020 2020 2020 2020 2020  t:..            
+000016a0: 636c 6965 6e74 2e72 756e 5f77 6f72 6b66  client.run_workf
+000016b0: 6c6f 7728 2e2e 2e29 0a0a 2020 2020 2222  low(...)..    ""
+000016c0: 220a 2020 2020 5f44 4546 4155 4c54 5f43  ".    _DEFAULT_C
+000016d0: 4f4e 4649 475f 5041 5448 5f31 203d 2022  ONFIG_PATH_1 = "
+000016e0: 2f65 7463 2f73 6c75 726d 2d63 6f6e 6669  /etc/slurm-confi
+000016f0: 672e 696e 6922 0a20 2020 205f 4445 4641  g.ini".    _DEFA
+00001700: 554c 545f 434f 4e46 4947 5f50 4154 485f  ULT_CONFIG_PATH_
+00001710: 3220 3d20 227e 2f73 6c75 726d 2d63 6f6e  2 = "~/slurm-con
+00001720: 6669 672e 696e 6922 0a20 2020 205f 4445  fig.ini".    _DE
+00001730: 4641 554c 545f 484f 5354 203d 2022 736c  FAULT_HOST = "sl
+00001740: 7572 6d22 0a20 2020 205f 4445 4641 554c  urm".    _DEFAUL
+00001750: 545f 494e 4c49 4e45 5f53 5348 5f45 4e56  T_INLINE_SSH_ENV
+00001760: 203d 2054 7275 650a 2020 2020 5f44 4546   = True.    _DEF
+00001770: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
+00001780: 5041 5448 203d 2022 6d79 2d73 6372 6174  PATH = "my-scrat
+00001790: 6368 2f64 6174 6122 0a20 2020 205f 4445  ch/data".    _DE
+000017a0: 4641 554c 545f 534c 5552 4d5f 494d 4147  FAULT_SLURM_IMAG
+000017b0: 4553 5f50 4154 4820 3d20 226d 792d 7363  ES_PATH = "my-sc
+000017c0: 7261 7463 682f 7369 6e67 756c 6172 6974  ratch/singularit
+000017d0: 795f 696d 6167 6573 2f77 6f72 6b66 6c6f  y_images/workflo
+000017e0: 7773 220a 2020 2020 5f44 4546 4155 4c54  ws".    _DEFAULT
+000017f0: 5f53 4c55 524d 5f43 4f4e 5645 5254 4552  _SLURM_CONVERTER
+00001800: 535f 5041 5448 203d 2022 6d79 2d73 6372  S_PATH = "my-scr
+00001810: 6174 6368 2f73 696e 6775 6c61 7269 7479  atch/singularity
+00001820: 5f69 6d61 6765 732f 636f 6e76 6572 7465  _images/converte
+00001830: 7273 220a 2020 2020 5f44 4546 4155 4c54  rs".    _DEFAULT
+00001840: 5f53 4c55 524d 5f47 4954 5f53 4352 4950  _SLURM_GIT_SCRIP
+00001850: 545f 5041 5448 203d 2022 736c 7572 6d2d  T_PATH = "slurm-
+00001860: 7363 7269 7074 7322 0a20 2020 205f 4f55  scripts".    _OU
+00001870: 545f 5345 5020 3d20 222d 2d73 706c 6974  T_SEP = "--split
+00001880: 2d2d 220a 2020 2020 5f56 4552 5349 4f4e  --".    _VERSION
+00001890: 5f43 4d44 203d 2022 6c73 202d 6820 7b73  _CMD = "ls -h {s
+000018a0: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+000018b0: 7d2f 7b69 6d61 6765 5f70 6174 687d 207c  }/{image_path} |
+000018c0: 2067 7265 7020 2d6f 5020 2728 3f3c 3d5c   grep -oP '(?<=\
+000018d0: 2d7c 5c5f 2928 762e 2b7c 6c61 7465 7374  -|\_)(v.+|latest
+000018e0: 2928 3f3d 2e73 696d 677c 2e73 6966 2927  )(?=.simg|.sif)'
+000018f0: 220a 2020 2020 2320 4e6f 7465 2c20 6772  ".    # Note, gr
+00001900: 6570 2072 6574 7572 6e73 2065 7869 7463  ep returns exitc
+00001910: 6f64 6520 3120 6966 206e 6f20 6d61 7463  ode 1 if no matc
+00001920: 6820 6973 2066 6f75 6e64 210a 2020 2020  h is found!.    
+00001930: 2320 5468 6973 2077 696c 6c20 7472 616e  # This will tran
+00001940: 736c 6174 6520 696e 746f 2061 2055 6e65  slate into a Une
+00001950: 7870 6563 7465 6445 7869 7420 6572 726f  xpectedExit erro
+00001960: 722c 2073 6f20 6d75 7465 2074 6861 7420  r, so mute that 
+00001970: 6966 2079 6f75 0a20 2020 2023 2064 6f6e  if you.    # don
+00001980: 2774 2063 6172 6520 6162 6f75 7420 656d  't care about em
+00001990: 7074 792e 0a20 2020 2023 204c 696b 6520  pty..    # Like 
+000019a0: 6265 6c6f 7720 7769 7468 2074 6865 2022  below with the "
+000019b0: 7c7c 203a 222e 0a20 2020 2023 2044 6174  || :"..    # Dat
+000019c0: 6120 636f 756c 6420 6c65 6769 7420 6265  a could legit be
+000019d0: 2065 6d70 7479 2e0a 2020 2020 5f44 4154   empty..    _DAT
+000019e0: 415f 434d 4420 3d20 226c 7320 2d68 207b  A_CMD = "ls -h {
+000019f0: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
+00001a00: 207c 2067 7265 7020 2d6f 5020 272e 2b28   | grep -oP '.+(
+00001a10: 3f3d 2e7a 6970 2927 207c 7c20 3a22 0a20  ?=.zip)' || :". 
+00001a20: 2020 205f 414c 4c5f 4a4f 4253 5f43 4d44     _ALL_JOBS_CMD
+00001a30: 203d 2022 7361 6363 7420 2d2d 7374 6172   = "sacct --star
+00001a40: 7474 696d 6520 7b73 7461 7274 5f74 696d  ttime {start_tim
+00001a50: 657d 202d 2d65 6e64 7469 6d65 207b 656e  e} --endtime {en
+00001a60: 645f 7469 6d65 7d20 2d2d 7374 6174 6520  d_time} --state 
+00001a70: 7b73 7461 7465 737d 202d 6f20 7b63 6f6c  {states} -o {col
+00001a80: 756d 6e73 7d20 2d6e 202d 5820 220a 2020  umns} -n -X ".  
+00001a90: 2020 5f5a 4950 5f43 4d44 203d 2022 377a    _ZIP_CMD = "7z
+00001aa0: 2061 202d 7920 7b66 696c 656e 616d 657d   a -y {filename}
+00001ab0: 202d 747a 6970 207b 6461 7461 5f6c 6f63   -tzip {data_loc
+00001ac0: 6174 696f 6e7d 2f64 6174 612f 6f75 7422  ation}/data/out"
+00001ad0: 0a20 2020 205f 4143 5449 5645 5f4a 4f42  .    _ACTIVE_JOB
+00001ae0: 535f 434d 4420 3d20 2273 7175 6575 6520  S_CMD = "squeue 
+00001af0: 2d75 2024 5553 4552 202d 2d6e 6f68 6561  -u $USER --nohea
+00001b00: 6420 2d2d 666f 726d 6174 2025 4622 0a20  d --format %F". 
+00001b10: 2020 205f 4a4f 425f 5354 4154 5553 5f43     _JOB_STATUS_C
+00001b20: 4d44 203d 2022 7361 6363 7420 2d6e 202d  MD = "sacct -n -
+00001b30: 6f20 4a6f 6249 642c 5374 6174 652c 456e  o JobId,State,En
+00001b40: 6420 2d58 202d 6a20 7b73 6c75 726d 5f6a  d -X -j {slurm_j
+00001b50: 6f62 5f69 647d 220a 2020 2020 2320 544f  ob_id}".    # TO
+00001b60: 444f 206d 6f76 6520 616c 6c20 636f 6d6d  DO move all comm
+00001b70: 616e 6473 2074 6f20 6120 7369 6d69 6c61  ands to a simila
+00001b80: 7220 666f 726d 6174 2e0a 2020 2020 2320  r format..    # 
+00001b90: 5468 656e 206d 6179 6265 2061 6c6c 6f77  Then maybe allow
+00001ba0: 206f 7665 7277 7269 7465 2066 726f 6d20   overwrite from 
+00001bb0: 736c 7572 6d2d 636f 6e66 6967 2e69 6e69  slurm-config.ini
+00001bc0: 0a20 2020 205f 4c4f 4746 494c 4520 3d20  .    _LOGFILE = 
+00001bd0: 226f 6d65 726f 2d7b 736c 7572 6d5f 6a6f  "omero-{slurm_jo
+00001be0: 625f 6964 7d2e 6c6f 6722 0a20 2020 205f  b_id}.log".    _
+00001bf0: 434f 4e56 4552 5445 525f 4c4f 4746 494c  CONVERTER_LOGFIL
+00001c00: 4520 3d20 2273 6c75 726d 2d7b 736c 7572  E = "slurm-{slur
+00001c10: 6d5f 6a6f 625f 6964 7d5f 2a2e 6f75 7422  m_job_id}_*.out"
+00001c20: 0a20 2020 205f 5441 494c 5f4c 4f47 5f43  .    _TAIL_LOG_C
+00001c30: 4d44 203d 2022 7461 696c 202d 6e20 7b6e  MD = "tail -n {n
+00001c40: 7d20 7b6c 6f67 5f66 696c 657d 207c 2073  } {log_file} | s
+00001c50: 7472 696e 6773 220a 2020 2020 5f4c 4f47  trings".    _LOG
+00001c60: 4649 4c45 5f44 4154 415f 434d 4420 3d20  FILE_DATA_CMD = 
+00001c70: 2263 6174 207b 6c6f 675f 6669 6c65 7d20  "cat {log_file} 
+00001c80: 7c20 7065 726c 202d 776e 6520 272f 5275  | perl -wne '/Ru
+00001c90: 6e6e 696e 6720 5b5c 772d 5d2b 3f20 4a6f  nning [\w-]+? Jo
+00001ca0: 6220 775c 2f20 2e2b 3f20 5c7c 202e 2b3f  b w\/ .+? \| .+?
+00001cb0: 205c 7c20 282e 2b3f 2920 5c7c 2e2a 2f69   \| (.+?) \|.*/i
+00001cc0: 2061 6e64 2070 7269 6e74 2431 2722 0a0a   and print$1'"..
+00001cd0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001ce0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+00001cf0: 2020 2020 2020 2020 686f 7374 3d5f 4445          host=_DE
+00001d00: 4641 554c 545f 484f 5354 2c0a 2020 2020  FAULT_HOST,.    
+00001d10: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00001d20: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
+00001d30: 2020 2020 2020 2020 2070 6f72 743d 4e6f           port=No
+00001d40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001d50: 2020 2020 2063 6f6e 6669 673d 4e6f 6e65       config=None
+00001d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001d70: 2020 2067 6174 6577 6179 3d4e 6f6e 652c     gateway=None,
+00001d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d90: 2020 666f 7277 6172 645f 6167 656e 743d    forward_agent=
+00001da0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001db0: 2020 2020 2020 2063 6f6e 6e65 6374 5f74         connect_t
+00001dc0: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001de0: 6e6e 6563 745f 6b77 6172 6773 3d4e 6f6e  nnect_kwargs=Non
+00001df0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001e00: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
+00001e10: 6e76 3d5f 4445 4641 554c 545f 494e 4c49  nv=_DEFAULT_INLI
+00001e20: 4e45 5f53 5348 5f45 4e56 2c0a 2020 2020  NE_SSH_ENV,.    
+00001e30: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00001e40: 726d 5f64 6174 615f 7061 7468 3a20 7374  rm_data_path: st
+00001e50: 7220 3d20 5f44 4546 4155 4c54 5f53 4c55  r = _DEFAULT_SLU
+00001e60: 524d 5f44 4154 415f 5041 5448 2c0a 2020  RM_DATA_PATH,.  
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001e80: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+00001e90: 3a20 7374 7220 3d20 5f44 4546 4155 4c54  : str = _DEFAULT
+00001ea0: 5f53 4c55 524d 5f49 4d41 4745 535f 5041  _SLURM_IMAGES_PA
+00001eb0: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
+00001ec0: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
+00001ed0: 7274 6572 735f 7061 7468 3a20 7374 7220  rters_path: str 
+00001ee0: 3d20 5f44 4546 4155 4c54 5f53 4c55 524d  = _DEFAULT_SLURM
+00001ef0: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
+00001f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001f10: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00001f20: 6174 6873 3a20 6469 6374 203d 204e 6f6e  aths: dict = Non
+00001f30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001f40: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00001f50: 7265 706f 733a 2064 6963 7420 3d20 4e6f  repos: dict = No
+00001f60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001f70: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+00001f80: 5f69 6d61 6765 733a 2064 6963 7420 3d20  _images: dict = 
+00001f90: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001fa0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00001fb0: 656c 5f6a 6f62 733a 2064 6963 7420 3d20  el_jobs: dict = 
+00001fc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001fd0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00001fe0: 656c 5f6a 6f62 735f 7061 7261 6d73 3a20  el_jobs_params: 
+00001ff0: 6469 6374 203d 204e 6f6e 652c 0a20 2020  dict = None,.   
+00002000: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00002010: 7572 6d5f 7363 7269 7074 5f70 6174 683a  urm_script_path:
+00002020: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
+00002030: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
+00002040: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
+00002050: 2020 2020 2020 2020 736c 7572 6d5f 7363          slurm_sc
+00002060: 7269 7074 5f72 6570 6f3a 2073 7472 203d  ript_repo: str =
+00002070: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00002080: 2020 2020 2020 2020 696e 6974 5f73 6c75          init_slu
+00002090: 726d 3a20 626f 6f6c 203d 2046 616c 7365  rm: bool = False
+000020a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000020b0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+000020c0: 2249 6e69 7469 616c 697a 6573 2061 206e  "Initializes a n
+000020d0: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
+000020e0: 6865 2053 6c75 726d 436c 6965 6e74 2063  he SlurmClient c
+000020f0: 6c61 7373 2e0a 0a20 2020 2020 2020 2049  lass...        I
+00002100: 7420 6973 2070 7265 6665 7261 626c 6520  t is preferable 
+00002110: 746f 2075 7365 2023 6672 6f6d 5f63 6f6e  to use #from_con
+00002120: 6669 6728 2e2e 2e29 206d 6574 686f 6420  fig(...) method 
+00002130: 746f 2069 6e69 7469 616c 697a 650a 2020  to initialize.  
+00002140: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
+00002150: 2066 726f 6d20 6120 636f 6e66 6967 2066   from a config f
+00002160: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
+00002170: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002180: 686f 7374 2028 7374 722c 206f 7074 696f  host (str, optio
+00002190: 6e61 6c29 3a20 5468 6520 686f 7374 6e61  nal): The hostna
+000021a0: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
+000021b0: 206f 6620 7468 6520 7265 6d6f 7465 0a20   of the remote. 
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000021d0: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
+000021e0: 746f 205f 4445 4641 554c 545f 484f 5354  to _DEFAULT_HOST
+000021f0: 2e0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+00002200: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
+00002210: 6c29 3a20 5468 6520 7573 6572 6e61 6d65  l): The username
+00002220: 2074 6f20 7573 6520 7768 656e 2063 6f6e   to use when con
+00002230: 6e65 6374 696e 6720 746f 200a 2020 2020  necting to .    
+00002240: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00002250: 7265 6d6f 7465 2073 6572 7665 722e 2044  remote server. D
+00002260: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
+00002270: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
+00002280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002290: 2074 6f20 636f 6e66 6967 2e75 7365 722e   to config.user.
+000022a0: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
+000022b0: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
+000022c0: 293a 2054 6865 2053 5348 2070 6f72 7420  ): The SSH port 
+000022d0: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
+000022e0: 6563 7469 6e67 2e0a 2020 2020 2020 2020  ecting..        
+000022f0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00002300: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
+00002310: 6465 6661 756c 7473 2074 6f20 636f 6e66  defaults to conf
+00002320: 6967 2e70 6f72 742e 0a20 2020 2020 2020  ig.port..       
+00002330: 2020 2020 2063 6f6e 6669 6720 2873 7472       config (str
+00002340: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
+00002350: 6820 746f 2074 6865 2053 5348 2063 6f6e  h to the SSH con
+00002360: 6669 6720 6669 6c65 2e0a 2020 2020 2020  fig file..      
+00002370: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00002380: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
+00002390: 6820 6465 6661 756c 7473 2074 6f20 796f  h defaults to yo
+000023a0: 7572 2053 5348 2063 6f6e 6669 6720 6669  ur SSH config fi
+000023b0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+000023c0: 6761 7465 7761 7920 2843 6f6e 6e65 6374  gateway (Connect
+000023d0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+000023e0: 416e 206f 7074 696f 6e61 6c20 6761 7465  An optional gate
+000023f0: 7761 7920 666f 7220 636f 6e6e 6563 7469  way for connecti
+00002400: 6e67 200a 2020 2020 2020 2020 2020 2020  ng .            
+00002410: 2020 2020 7468 726f 7567 6820 6120 6a75      through a ju
+00002420: 6d70 2068 6f73 742e 2044 6566 6175 6c74  mp host. Default
+00002430: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+00002440: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
+00002450: 6765 6e74 2028 626f 6f6c 2c20 6f70 7469  gent (bool, opti
+00002460: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
+00002470: 6f20 666f 7277 6172 6420 7468 6520 6c6f  o forward the lo
+00002480: 6361 6c20 5353 4820 0a20 2020 2020 2020  cal SSH .       
+00002490: 2020 2020 2020 2020 2061 6765 6e74 2074           agent t
+000024a0: 6f20 7468 6520 7265 6d6f 7465 2073 6572  o the remote ser
+000024b0: 7665 722e 2044 6566 6175 6c74 7320 746f  ver. Defaults to
+000024c0: 204e 6f6e 652c 2077 6869 6368 200a 2020   None, which .  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+000024e0: 6661 756c 7473 2074 6f20 636f 6e66 6967  faults to config
+000024f0: 2e66 6f72 7761 7264 5f61 6765 6e74 2e0a  .forward_agent..
+00002500: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00002510: 6563 745f 7469 6d65 6f75 7420 2869 6e74  ect_timeout (int
+00002520: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
+00002530: 656f 7574 2066 6f72 2065 7374 6162 6c69  eout for establi
+00002540: 7368 696e 6720 7468 6520 5353 4820 0a20  shing the SSH . 
+00002550: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002560: 6f6e 6e65 6374 696f 6e2e 2044 6566 6175  onnection. Defau
+00002570: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
+00002580: 6368 2064 6566 6175 6c74 7320 0a20 2020  ch defaults .   
+00002590: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
+000025a0: 636f 6e66 6967 2e74 696d 656f 7574 732e  config.timeouts.
+000025b0: 636f 6e6e 6563 742e 0a20 2020 2020 2020  connect..       
+000025c0: 2020 2020 2063 6f6e 6e65 6374 5f6b 7761       connect_kwa
+000025d0: 7267 7320 2864 6963 742c 206f 7074 696f  rgs (dict, optio
+000025e0: 6e61 6c29 3a20 4164 6469 7469 6f6e 616c  nal): Additional
+000025f0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00002600: 7473 2066 6f72 200a 2020 2020 2020 2020  ts for .        
+00002610: 2020 2020 2020 2020 7468 6520 756e 6465          the unde
+00002620: 726c 7969 6e67 2053 5348 2063 6f6e 6e65  rlying SSH conne
+00002630: 6374 696f 6e2e 2048 616e 6465 6420 7665  ction. Handed ve
+00002640: 7262 6174 696d 2074 6f20 0a20 2020 2020  rbatim to .     
+00002650: 2020 2020 2020 2020 2020 2060 5353 4843             `SSHC
+00002660: 6c69 656e 742e 636f 6e6e 6563 7420 3c70  lient.connect <p
+00002670: 6172 616d 696b 6f2e 636c 6965 6e74 2e53  aramiko.client.S
+00002680: 5348 436c 6965 6e74 2e63 6f6e 6e65 6374  SHClient.connect
+00002690: 3e60 2e20 0a20 2020 2020 2020 2020 2020  >`. .           
+000026a0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+000026b0: 204e 6f6e 652e 200a 2020 2020 2020 2020   None. .        
+000026c0: 2020 2020 696e 6c69 6e65 5f73 7368 5f65      inline_ssh_e
+000026d0: 6e76 2028 626f 6f6c 2c20 6f70 7469 6f6e  nv (bool, option
+000026e0: 616c 293a 2057 6865 7468 6572 2074 6f20  al): Whether to 
+000026f0: 7573 6520 696e 6c69 6e65 2053 5348 0a20  use inline SSH. 
+00002700: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002710: 6e76 6972 6f6e 6d65 6e74 2e20 5468 6973  nvironment. This
+00002720: 2069 7320 6e65 6365 7373 6172 7920 6966   is necessary if
+00002730: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
+00002740: 6572 2068 6173 200a 2020 2020 2020 2020  er has .        
+00002750: 2020 2020 2020 2020 6120 7265 7374 7269          a restri
+00002760: 6374 6564 2060 6041 6363 6570 7445 6e76  cted ``AcceptEnv
+00002770: 6060 2073 6574 7469 6e67 2028 7768 6963  `` setting (whic
+00002780: 6820 6973 2074 6865 2063 6f6d 6d6f 6e20  h is the common 
+00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027a0: 2064 6566 6175 6c74 292e 2044 6566 6175   default). Defau
+000027b0: 6c74 7320 746f 205f 4445 4641 554c 545f  lts to _DEFAULT_
+000027c0: 494e 4c49 4e45 5f53 5348 5f45 4e56 2e0a  INLINE_SSH_ENV..
+000027d0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+000027e0: 6d5f 6461 7461 5f70 6174 6820 2873 7472  m_data_path (str
+000027f0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00002800: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00002810: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+00002820: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+00002830: 6720 7468 6520 6461 7461 2066 696c 6573  g the data files
+00002840: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
+00002850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002860: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
+00002870: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
+00002880: 5f50 4154 482e 0a20 2020 2020 2020 2020  _PATH..         
+00002890: 2020 2073 6c75 726d 5f69 6d61 6765 735f     slurm_images_
+000028a0: 7061 7468 2028 7374 722c 206f 7074 696f  path (str, optio
+000028b0: 6e61 6c29 3a20 5468 6520 7061 7468 2074  nal): The path t
+000028c0: 6f20 7468 6520 6469 7265 6374 6f72 790a  o the directory.
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 636f 6e74 6169 6e69 6e67 2074 6865 2053  containing the S
+000028f0: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
+00002900: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
+00002910: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002920: 2020 4465 6661 756c 7473 2074 6f20 5f44    Defaults to _D
+00002930: 4546 4155 4c54 5f53 4c55 524d 5f49 4d41  EFAULT_SLURM_IMA
+00002940: 4745 535f 5041 5448 2e0a 2020 2020 2020  GES_PATH..      
+00002950: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
+00002960: 6572 7465 7273 5f70 6174 6820 2873 7472  erters_path (str
+00002970: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00002980: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00002990: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+000029a0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+000029b0: 6720 7468 6520 5369 6e67 756c 6172 6974  g the Singularit
+000029c0: 7920 696d 6167 6573 2066 6f72 2066 696c  y images for fil
+000029d0: 6520 636f 6e76 6572 7465 7273 2e0a 2020  e converters..  
+000029e0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+000029f0: 6661 756c 7473 2074 6f20 5f44 4546 4155  faults to _DEFAU
+00002a00: 4c54 5f53 4c55 524d 5f43 4f4e 5645 5254  LT_SLURM_CONVERT
+00002a10: 4552 535f 5041 5448 2e0a 2020 2020 2020  ERS_PATH..      
+00002a20: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00002a30: 6c5f 7061 7468 7320 2864 6963 742c 206f  l_paths (dict, o
+00002a40: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
+00002a50: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+00002a60: 6720 7468 6520 0a20 2020 2020 2020 2020  g the .         
+00002a70: 2020 2020 2020 2070 6174 6873 2074 6f20         paths to 
+00002a80: 7468 6520 5369 6e67 756c 6172 6974 7920  the Singularity 
+00002a90: 696d 6167 6573 2066 6f72 2073 7065 6369  images for speci
+00002aa0: 6669 6320 536c 7572 6d20 6a6f 6220 6d6f  fic Slurm job mo
+00002ab0: 6465 6c73 2e0a 2020 2020 2020 2020 2020  dels..          
+00002ac0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00002ad0: 6f20 4e6f 6e65 2e0a 2020 2020 2020 2020  o None..        
+00002ae0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00002af0: 7265 706f 7320 2864 6963 742c 206f 7074  repos (dict, opt
+00002b00: 696f 6e61 6c29 3a20 4120 6469 6374 696f  ional): A dictio
+00002b10: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00002b20: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
+00002b30: 2020 2020 2067 6974 2072 6570 6f73 6974       git reposit
+00002b40: 6f72 6965 7320 6f66 2053 696e 6775 6c61  ories of Singula
+00002b50: 7269 7479 2069 6d61 6765 7320 666f 7220  rity images for 
+00002b60: 7370 6563 6966 6963 2053 6c75 726d 200a  specific Slurm .
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b80: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
+00002b90: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00002ba0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00002bb0: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+00002bc0: 6d6f 6465 6c5f 696d 6167 6573 2028 6469  model_images (di
+00002bd0: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
+00002be0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
+00002bf0: 6169 6e69 6e67 2074 6865 200a 2020 2020  aining the .    
+00002c00: 2020 2020 2020 2020 2020 2020 646f 636b              dock
+00002c10: 6572 6875 6220 6f66 2074 6865 2053 696e  erhub of the Sin
+00002c20: 6775 6c61 7269 7479 2069 6d61 6765 7320  gularity images 
+00002c30: 666f 7220 7370 6563 6966 6963 2053 6c75  for specific Slu
+00002c40: 726d 200a 2020 2020 2020 2020 2020 2020  rm .            
+00002c50: 2020 2020 6a6f 6220 6d6f 6465 6c73 2e20      job models. 
+00002c60: 5769 6c6c 2066 696c 6c20 6175 746f 6d61  Will fill automa
+00002c70: 7469 6361 6c6c 7920 6672 6f6d 2074 6865  tically from the
+00002c80: 2064 6174 6120 696e 2074 6865 2067 6974   data in the git
+00002c90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002ca0: 2020 7265 706f 7369 746f 7279 2069 6620    repository if 
+00002cb0: 796f 7520 7365 7420 696e 6974 5f73 6c75  you set init_slu
+00002cc0: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
+00002cd0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002ce0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002cf0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00002d00: 6273 2028 6469 6374 2c20 6f70 7469 6f6e  bs (dict, option
+00002d10: 616c 293a 2041 2064 6963 7469 6f6e 6172  al): A dictionar
+00002d20: 7920 636f 6e74 6169 6e69 6e67 0a20 2020  y containing.   
+00002d30: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00002d40: 6f72 6d61 7469 6f6e 2061 626f 7574 2073  ormation about s
+00002d50: 7065 6369 6669 6320 536c 7572 6d20 6a6f  pecific Slurm jo
+00002d60: 6220 6d6f 6465 6c73 2e0a 2020 2020 2020  b models..      
+00002d70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00002d80: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00002d90: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00002da0: 6465 6c5f 6a6f 6273 5f70 6172 616d 7320  del_jobs_params 
+00002db0: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
+00002dc0: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
+00002dd0: 6f6e 7461 696e 696e 670a 2020 2020 2020  ontaining.      
+00002de0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00002df0: 7465 7273 2066 6f72 2073 7065 6369 6669  ters for specifi
+00002e00: 6320 536c 7572 6d20 6a6f 6220 6d6f 6465  c Slurm job mode
+00002e10: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+00002e20: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002e30: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002e40: 2020 736c 7572 6d5f 7363 7269 7074 5f70    slurm_script_p
+00002e50: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
+00002e60: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
+00002e70: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
+00002e80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002e90: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00002ea0: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
+00002eb0: 6f6e 2073 6372 6970 7473 206f 6e20 536c  on scripts on Sl
+00002ec0: 7572 6d2e 0a20 2020 2020 2020 2020 2020  urm..           
+00002ed0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00002ee0: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
+00002ef0: 4749 545f 5343 5249 5054 5f50 4154 482e  GIT_SCRIPT_PATH.
+00002f00: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
+00002f10: 726d 5f73 6372 6970 745f 7265 706f 2028  rm_script_repo (
+00002f20: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00002f30: 5468 6520 6769 7420 6874 7470 7320 5552  The git https UR
+00002f40: 4c20 666f 7220 636c 6f6e 696e 670a 2020  L for cloning.  
+00002f50: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00002f60: 6520 7265 706f 2063 6f6e 7461 696e 696e  e repo containin
+00002f70: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
+00002f80: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
+00002f90: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00002fa0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00002fb0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00002fc0: 2020 696e 6974 5f73 6c75 726d 2028 626f    init_slurm (bo
+00002fd0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00002fe0: 7365 7420 7570 2074 6865 2072 6571 7569  set up the requi
+00002ff0: 7265 6420 7374 7275 6374 7572 6573 200a  red structures .
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2075 7365 722c 0a20 2020 2020 2020     user,.       
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2070 6f72 742c 0a20 2020 2020 2020     port,.       
-00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2020 2063 6f6e 6669 672c 0a20 2020 2020     config,.     
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 2067 6174 6577 6179 2c0a 2020       gateway,.  
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 2020 2020 666f 7277 6172 645f          forward_
-000030e0: 6167 656e 742c 0a20 2020 2020 2020 2020  agent,.         
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2063 6f6e 6e65 6374 5f74 696d 656f 7574   connect_timeout
-00003120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-00003150: 6563 745f 6b77 6172 6773 2c0a 2020 2020  ect_kwargs,.    
+00003010: 6f6e 2053 6c75 726d 2061 6674 6572 2069  on Slurm after i
+00003020: 6e69 7469 6174 696e 6720 7468 6973 2063  nitiating this c
+00003030: 6c69 656e 742e 2054 6869 7320 696e 636c  lient. This incl
+00003040: 7564 6573 2063 7265 6174 696e 6720 0a20  udes creating . 
+00003050: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00003060: 6973 7369 6e67 2066 6f6c 6465 7273 2c20  issing folders, 
+00003070: 646f 776e 6c6f 6164 696e 6720 636f 6e74  downloading cont
+00003080: 6169 6e65 7220 696d 6167 6573 2c20 636c  ainer images, cl
+00003090: 6f6e 696e 6720 6769 742c 6574 632e 0a20  oning git,etc.. 
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000030b0: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
+000030c0: 7768 696c 6520 6174 2066 6972 7374 2062  while at first b
+000030d0: 7574 2077 696c 6c20 7661 6c69 6461 7465  ut will validate
+000030e0: 2079 6f75 7220 7365 7475 702e 0a20 2020   your setup..   
+000030f0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00003100: 6175 6c74 7320 746f 2046 616c 7365 2074  aults to False t
+00003110: 6f20 7361 7665 2074 696d 652e 0a20 2020  o save time..   
+00003120: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003130: 2073 7570 6572 2853 6c75 726d 436c 6965   super(SlurmClie
+00003140: 6e74 2c20 7365 6c66 292e 5f5f 696e 6974  nt, self).__init
+00003150: 5f5f 2868 6f73 742c 0a20 2020 2020 2020  __(host,.       
 00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
-00003190: 5f65 6e76 290a 2020 2020 2020 2020 7365  _env).        se
-000031a0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
-000031b0: 7468 203d 2073 6c75 726d 5f64 6174 615f  th = slurm_data_
-000031c0: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
-000031d0: 662e 736c 7572 6d5f 696d 6167 6573 5f70  f.slurm_images_p
-000031e0: 6174 6820 3d20 736c 7572 6d5f 696d 6167  ath = slurm_imag
-000031f0: 6573 5f70 6174 680a 2020 2020 2020 2020  es_path.        
-00003200: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
-00003210: 7274 6572 735f 7061 7468 203d 2073 6c75  rters_path = slu
-00003220: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
-00003230: 7468 0a20 2020 2020 2020 2073 656c 662e  th.        self.
-00003240: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-00003250: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
-00003260: 7061 7468 730a 2020 2020 2020 2020 7365  paths.        se
-00003270: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-00003280: 7061 7468 203d 2073 6c75 726d 5f73 6372  path = slurm_scr
-00003290: 6970 745f 7061 7468 0a20 2020 2020 2020  ipt_path.       
-000032a0: 2073 656c 662e 736c 7572 6d5f 7363 7269   self.slurm_scri
-000032b0: 7074 5f72 6570 6f20 3d20 736c 7572 6d5f  pt_repo = slurm_
-000032c0: 7363 7269 7074 5f72 6570 6f0a 2020 2020  script_repo.    
-000032d0: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
-000032e0: 6f64 656c 5f72 6570 6f73 203d 2073 6c75  odel_repos = slu
-000032f0: 726d 5f6d 6f64 656c 5f72 6570 6f73 0a20  rm_model_repos. 
-00003300: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
-00003310: 6d5f 6d6f 6465 6c5f 696d 6167 6573 203d  m_model_images =
-00003320: 2073 6c75 726d 5f6d 6f64 656c 5f69 6d61   slurm_model_ima
-00003330: 6765 730a 2020 2020 2020 2020 7365 6c66  ges.        self
-00003340: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
-00003350: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
-00003360: 6a6f 6273 0a20 2020 2020 2020 2073 656c  jobs.        sel
-00003370: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
-00003380: 6273 5f70 6172 616d 7320 3d20 736c 7572  bs_params = slur
-00003390: 6d5f 6d6f 6465 6c5f 6a6f 6273 5f70 6172  m_model_jobs_par
-000033a0: 616d 730a 0a20 2020 2020 2020 2023 2049  ams..        # I
-000033b0: 6e69 7420 6361 6368 652e 204b 6565 7020  nit cache. Keep 
-000033c0: 7265 7370 6f6e 7365 7320 666f 7220 3336  responses for 36
-000033d0: 3020 7365 636f 6e64 730a 2020 2020 2020  0 seconds.      
-000033e0: 2020 7365 6c66 2e63 6163 6865 203d 2072    self.cache = r
-000033f0: 6571 7565 7374 735f 6361 6368 652e 6261  equests_cache.ba
-00003400: 636b 656e 6473 2e73 716c 6974 652e 5351  ckends.sqlite.SQ
-00003410: 4c69 7465 4361 6368 6528 0a20 2020 2020  LiteCache(.     
-00003420: 2020 2020 2020 2064 625f 7061 7468 3d22         db_path="
-00003430: 6769 7468 7562 5f63 6163 6865 222c 2075  github_cache", u
-00003440: 7365 5f74 656d 703d 5472 7565 290a 2020  se_temp=True).  
-00003450: 2020 2020 2020 7365 6c66 2e67 6574 5f6f        self.get_o
-00003460: 725f 6372 6561 7465 5f67 6974 6875 625f  r_create_github_
-00003470: 7365 7373 696f 6e28 290a 0a20 2020 2020  session()..     
-00003480: 2020 2073 656c 662e 696e 6974 5f77 6f72     self.init_wor
-00003490: 6b66 6c6f 7773 2829 0a20 2020 2020 2020  kflows().       
-000034a0: 2073 656c 662e 7661 6c69 6461 7465 2876   self.validate(v
-000034b0: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
-000034c0: 7475 703d 696e 6974 5f73 6c75 726d 290a  tup=init_slurm).
-000034d0: 0a20 2020 2064 6566 2069 6e69 745f 776f  .    def init_wo
-000034e0: 726b 666c 6f77 7328 7365 6c66 2c20 666f  rkflows(self, fo
-000034f0: 7263 655f 7570 6461 7465 3a20 626f 6f6c  rce_update: bool
-00003500: 203d 2046 616c 7365 293a 0a20 2020 2020   = False):.     
-00003510: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00003520: 6574 7269 6576 6573 2074 6865 2072 6571  etrieves the req
-00003530: 7569 7265 6420 696e 666f 2066 6f72 2074  uired info for t
-00003540: 6865 2063 6f6e 6669 6775 7265 6420 776f  he configured wo
-00003550: 726b 666c 6f77 7320 6672 6f6d 2067 6974  rkflows from git
-00003560: 6875 622e 0a20 2020 2020 2020 2049 7420  hub..        It 
-00003570: 7769 6c6c 2066 696c 6c20 6073 6c75 726d  will fill `slurm
-00003580: 5f6d 6f64 656c 5f69 6d61 6765 7360 2077  _model_images` w
-00003590: 6974 6820 646f 636b 6572 6875 6220 6c69  ith dockerhub li
-000035a0: 6e6b 732e 0a0a 2020 2020 2020 2020 4172  nks...        Ar
-000035b0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000035c0: 666f 7263 655f 7570 6461 7465 2028 626f  force_update (bo
-000035d0: 6f6c 293a 2057 696c 6c20 6f76 6572 7772  ol): Will overwr
-000035e0: 6974 6520 616c 7265 6164 7920 6769 7665  ite already give
-000035f0: 6e20 7061 7468 730a 2020 2020 2020 2020  n paths.        
-00003600: 2020 2020 2020 2020 696e 2060 736c 7572          in `slur
-00003610: 6d5f 6d6f 6465 6c5f 696d 6167 6573 600a  m_model_images`.
-00003620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003630: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00003640: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
-00003650: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-00003660: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-00003670: 6c5f 696d 6167 6573 203d 207b 7d0a 2020  l_images = {}.  
-00003680: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00003690: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7265  f.slurm_model_re
-000036a0: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
-000036b0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-000036c0: 224e 6f20 776f 726b 666c 6f77 7320 636f  "No workflows co
-000036d0: 6e66 6967 7572 6564 2122 290a 2020 2020  nfigured!").    
-000036e0: 2020 2020 2020 2020 7365 6c66 2e73 6c75          self.slu
-000036f0: 726d 5f6d 6f64 656c 5f72 6570 6f73 203d  rm_model_repos =
-00003700: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00003710: 2320 736b 6970 7320 7468 6520 7365 7475  # skips the setu
-00003720: 700a 2020 2020 2020 2020 666f 7220 776f  p.        for wo
-00003730: 726b 666c 6f77 2069 6e20 7365 6c66 2e73  rkflow in self.s
-00003740: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-00003750: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
-00003760: 2020 2020 2069 6620 776f 726b 666c 6f77       if workflow
-00003770: 206e 6f74 2069 6e20 7365 6c66 2e73 6c75   not in self.slu
-00003780: 726d 5f6d 6f64 656c 5f69 6d61 6765 7320  rm_model_images 
-00003790: 6f72 2066 6f72 6365 5f75 7064 6174 653a  or force_update:
-000037a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037b0: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
-000037c0: 203d 2073 656c 662e 7075 6c6c 5f64 6573   = self.pull_des
-000037d0: 6372 6970 746f 725f 6672 6f6d 5f67 6974  criptor_from_git
-000037e0: 6875 6228 776f 726b 666c 6f77 290a 2020  hub(workflow).  
-000037f0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00003800: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
-00003810: 2573 272c 2077 6f72 6b66 6c6f 772c 206a  %s', workflow, j
-00003820: 736f 6e5f 6465 7363 7269 7074 6f72 290a  son_descriptor).
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 696d 6167 6520 3d20 6a73 6f6e 5f64 6573  image = json_des
-00003850: 6372 6970 746f 725b 2763 6f6e 7461 696e  criptor['contain
-00003860: 6572 2d69 6d61 6765 275d 5b27 696d 6167  er-image']['imag
-00003870: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
-00003880: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
-00003890: 6f64 656c 5f69 6d61 6765 735b 776f 726b  odel_images[work
-000038a0: 666c 6f77 5d20 3d20 696d 6167 650a 0a20  flow] = image.. 
-000038b0: 2020 2064 6566 2073 6574 7570 5f73 6c75     def setup_slu
-000038c0: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
-000038d0: 2020 2222 220a 2020 2020 2020 2020 5661    """.        Va
-000038e0: 6c69 6461 7465 7320 6f72 2063 7265 6174  lidates or creat
-000038f0: 6573 2074 6865 2072 6571 7569 7265 6420  es the required 
-00003900: 7365 7475 7020 6f6e 2074 6865 2053 6c75  setup on the Slu
-00003910: 726d 2063 6c75 7374 6572 2e0a 0a20 2020  rm cluster...   
-00003920: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-00003930: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
-00003940: 7074 696f 6e3a 2069 6620 6974 2063 616e  ption: if it can
-00003950: 6e6f 7420 636f 6e6e 6563 7420 746f 2053  not connect to S
-00003960: 6c75 726d 2c20 6f72 2072 756e 7320 696e  lurm, or runs in
-00003970: 746f 2061 6e20 6572 726f 720a 2020 2020  to an error.    
-00003980: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003990: 6966 2073 656c 662e 7661 6c69 6461 7465  if self.validate
-000039a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000039b0: 2320 312e 2043 7265 6174 6520 6469 7265  # 1. Create dire
-000039c0: 6374 6f72 6965 730a 2020 2020 2020 2020  ctories.        
-000039d0: 2020 2020 7365 6c66 2e73 6574 7570 5f64      self.setup_d
-000039e0: 6972 6563 746f 7269 6573 2829 0a0a 2020  irectories()..  
-000039f0: 2020 2020 2020 2020 2020 2320 322e 2043            # 2. C
-00003a00: 6c6f 6e65 2067 6974 0a20 2020 2020 2020  lone git.       
-00003a10: 2020 2020 2073 656c 662e 7365 7475 705f       self.setup_
-00003a20: 6a6f 625f 7363 7269 7074 7328 290a 0a20  job_scripts().. 
-00003a30: 2020 2020 2020 2020 2020 2023 2033 2e20             # 3. 
-00003a40: 5365 7475 7020 636f 6e76 6572 7465 7273  Setup converters
-00003a50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003a60: 662e 7365 7475 705f 636f 6e76 6572 7465  f.setup_converte
-00003a70: 7273 2829 0a0a 2020 2020 2020 2020 2020  rs()..          
-00003a80: 2020 2320 342e 2044 6f77 6e6c 6f61 6420    # 4. Download 
-00003a90: 776f 726b 666c 6f77 2069 6d61 6765 730a  workflow images.
-00003aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003ab0: 2e73 6574 7570 5f63 6f6e 7461 696e 6572  .setup_container
-00003ac0: 5f69 6d61 6765 7328 290a 0a20 2020 2020  _images()..     
-00003ad0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003ae0: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00003af0: 6365 7074 696f 6e28 2246 6169 6c75 7265  ception("Failure
-00003b00: 2069 6e20 636f 6e6e 6563 7469 6e67 2074   in connecting t
-00003b10: 6f20 536c 7572 6d20 636c 7573 7465 7222  o Slurm cluster"
-00003b20: 290a 0a20 2020 2064 6566 2073 6574 7570  )..    def setup
-00003b30: 5f63 6f6e 7461 696e 6572 5f69 6d61 6765  _container_image
-00003b40: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00003b50: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
-00003b60: 7320 7570 2063 6f6e 7461 696e 6572 2069  s up container i
-00003b70: 6d61 6765 7320 666f 7220 536c 7572 6d20  mages for Slurm 
-00003b80: 6f70 6572 6174 696f 6e73 2e0a 0a20 2020  operations...   
-00003b90: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-00003ba0: 6f6e 2063 7265 6174 6573 2073 7065 6369  on creates speci
-00003bb0: 6669 6320 6469 7265 6374 6f72 6965 7320  fic directories 
-00003bc0: 666f 7220 636f 6e74 6169 6e65 7220 696d  for container im
-00003bd0: 6167 6573 2061 6e64 2070 756c 6c73 0a20  ages and pulls. 
-00003be0: 2020 2020 2020 206e 6563 6573 7361 7279         necessary
-00003bf0: 2069 6d61 6765 7320 6672 6f6d 2044 6f63   images from Doc
-00003c00: 6b65 7220 7265 706f 7369 746f 7269 6573  ker repositories
-00003c10: 2e20 4974 2067 656e 6572 6174 6573 2061  . It generates a
-00003c20: 6e64 2065 7865 6375 7465 730a 2020 2020  nd executes.    
-00003c30: 2020 2020 6120 7363 7269 7074 2074 6f20      a script to 
-00003c40: 7075 6c6c 2069 6d61 6765 7320 616e 6420  pull images and 
-00003c50: 636f 7069 6573 2069 7420 746f 2074 6865  copies it to the
-00003c60: 2072 656d 6f74 6520 6c6f 6361 7469 6f6e   remote location
-00003c70: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00003c80: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
-00003c90: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
-00003ca0: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
-00003cb0: 6520 6578 6563 7574 696e 6720 636f 6d6d  e executing comm
-00003cc0: 616e 6473 206f 7220 636f 7079 696e 6720  ands or copying 
-00003cd0: 6669 6c65 732e 0a20 2020 2020 2020 2022  files..        "
-00003ce0: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
-00003cf0: 6174 6520 7370 6563 6966 6963 2077 6f72  ate specific wor
-00003d00: 6b66 6c6f 7720 6469 7273 0a20 2020 2020  kflow dirs.     
-00003d10: 2020 2077 6974 6820 7365 6c66 2e63 6428     with self.cd(
-00003d20: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
-00003d30: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00003d40: 2020 2020 2069 6620 7365 6c66 2e73 6c75       if self.slu
-00003d50: 726d 5f6d 6f64 656c 5f70 6174 6873 3a0a  rm_model_paths:.
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 6d6f 6465 6c70 6174 6873 203d 2022 2022  modelpaths = " "
-00003d80: 2e6a 6f69 6e28 7365 6c66 2e73 6c75 726d  .join(self.slurm
-00003d90: 5f6d 6f64 656c 5f70 6174 6873 2e76 616c  _model_paths.val
-00003da0: 7565 7328 2929 0a20 2020 2020 2020 2020  ues()).         
-00003db0: 2020 2020 2020 2023 206d 6b64 6972 2063         # mkdir c
-00003dc0: 656c 6c70 726f 6669 6c65 7220 696d 6167  ellprofiler imag
-00003dd0: 656a 202e 2e2e 0a20 2020 2020 2020 2020  ej ....         
-00003de0: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
-00003df0: 7275 6e5f 636f 6d6d 616e 6473 285b 6622  run_commands([f"
-00003e00: 6d6b 6469 7220 2d70 207b 6d6f 6465 6c70  mkdir -p {modelp
-00003e10: 6174 6873 7d22 5d29 0a20 2020 2020 2020  aths}"]).       
-00003e20: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00003e30: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
-00003e40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00003e50: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
-00003e60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003e70: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00003e80: 5f69 6d61 6765 733a 0a20 2020 2020 2020  _images:.       
-00003e90: 2020 2020 2020 2020 2070 756c 6c5f 636f           pull_co
-00003ea0: 6d6d 616e 6473 203d 205b 5d0a 2020 2020  mmands = [].    
-00003eb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003ec0: 7766 2c20 696d 6167 6520 696e 2073 656c  wf, image in sel
-00003ed0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 696d  f.slurm_model_im
-00003ee0: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
-00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f00: 2020 7265 706f 203d 2073 656c 662e 736c    repo = self.sl
-00003f10: 7572 6d5f 6d6f 6465 6c5f 7265 706f 735b  urm_model_repos[
-00003f20: 7766 5d0a 2020 2020 2020 2020 2020 2020  wf].            
-00003f30: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
-00003f40: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-00003f50: 7061 7468 735b 7766 5d0a 2020 2020 2020  paths[wf].      
-00003f60: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
-00003f70: 2076 6572 7369 6f6e 203d 2073 656c 662e   version = self.
-00003f80: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
-00003f90: 6f6d 5f75 726c 2872 6570 6f29 0a20 2020  om_url(repo).   
-00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fb0: 2069 6620 7665 7273 696f 6e20 3d3d 2022   if version == "
-00003fc0: 6d61 7374 6572 223a 0a20 2020 2020 2020  master":.       
-00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fe0: 2076 6572 7369 6f6e 203d 2022 6c61 7465   version = "late
-00003ff0: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
-00004000: 2020 2020 2020 2020 7075 6c6c 5f74 656d          pull_tem
-00004010: 706c 6174 6520 3d20 2265 6368 6f20 2773  plate = "echo 's
-00004020: 7461 7274 696e 6720 2470 6174 6820 2476  tarting $path $v
-00004030: 6572 7369 6f6e 2720 3e3e 2073 696e 672e  ersion' >> sing.
-00004040: 6c6f 675c 6e6e 6f68 7570 2073 6820 2d63  log\nnohup sh -c
-00004050: 205c 2273 696e 6775 6c61 7269 7479 2070   \"singularity p
-00004060: 756c 6c20 2d2d 6469 7361 626c 652d 6361  ull --disable-ca
-00004070: 6368 6520 2d2d 6469 7220 2470 6174 6820  che --dir $path 
-00004080: 646f 636b 6572 3a2f 2f24 696d 6167 653a  docker://$image:
-00004090: 2476 6572 7369 6f6e 3b20 6563 686f 2027  $version; echo '
-000040a0: 6669 6e69 7368 6564 2024 7061 7468 2024  finished $path $
-000040b0: 7665 7273 696f 6e27 5c22 203e 3e20 7369  version'\" >> si
-000040c0: 6e67 2e6c 6f67 2032 3e26 3120 2620 6469  ng.log 2>&1 & di
-000040d0: 736f 776e 220a 2020 2020 2020 2020 2020  sown".          
-000040e0: 2020 2020 2020 2020 2020 7420 3d20 5465            t = Te
-000040f0: 6d70 6c61 7465 2870 756c 6c5f 7465 6d70  mplate(pull_temp
-00004100: 6c61 7465 290a 2020 2020 2020 2020 2020  late).          
-00004110: 2020 2020 2020 2020 2020 7375 6273 7469            substi
-00004120: 7475 7465 7320 3d20 7b7d 0a20 2020 2020  tutes = {}.     
-00004130: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004140: 7562 7374 6974 7574 6573 5b27 7061 7468  ubstitutes['path
-00004150: 275d 203d 2070 6174 680a 2020 2020 2020  '] = path.      
-00004160: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00004170: 6273 7469 7475 7465 735b 2769 6d61 6765  bstitutes['image
-00004180: 275d 203d 2069 6d61 6765 0a20 2020 2020  '] = image.     
-00004190: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000041a0: 7562 7374 6974 7574 6573 5b27 7665 7273  ubstitutes['vers
-000041b0: 696f 6e27 5d20 3d20 7665 7273 696f 6e0a  ion'] = version.
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 636d 6420 3d20 742e 7361 6665      cmd = t.safe
-000041e0: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
-000041f0: 7469 7475 7465 7329 0a20 2020 2020 2020  titutes).       
-00004200: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00004210: 6765 722e 6465 6275 6728 6622 7375 6273  ger.debug(f"subs
-00004220: 7469 7475 7465 643a 207b 636d 647d 2229  tituted: {cmd}")
-00004230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004240: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
-00004250: 6473 2e61 7070 656e 6428 636d 6429 0a20  ds.append(cmd). 
-00004260: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004270: 6372 6970 745f 6e61 6d65 203d 2022 7075  cript_name = "pu
-00004280: 6c6c 5f69 6d61 6765 732e 7368 220a 2020  ll_images.sh".  
-00004290: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000042a0: 6d70 6c61 7465 5f73 6372 6970 7420 3d20  mplate_script = 
-000042b0: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
-000042c0: 2229 2e6a 6f69 6e70 6174 6828 7363 7269  ").joinpath(scri
-000042d0: 7074 5f6e 616d 6529 0a20 2020 2020 2020  pt_name).       
-000042e0: 2020 2020 2020 2020 2077 6974 6820 7465           with te
-000042f0: 6d70 6c61 7465 5f73 6372 6970 742e 6f70  mplate_script.op
-00004300: 656e 2827 7227 2920 6173 2066 3a0a 2020  en('r') as f:.  
-00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004320: 2020 7372 6320 3d20 5465 6d70 6c61 7465    src = Template
-00004330: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
-00004340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004350: 7562 7374 6974 7574 6520 3d20 7b27 7075  ubstitute = {'pu
-00004360: 6c6c 636f 6d6d 616e 6473 273a 2022 5c6e  llcommands': "\n
-00004370: 222e 6a6f 696e 2870 756c 6c5f 636f 6d6d  ".join(pull_comm
-00004380: 616e 6473 297d 0a20 2020 2020 2020 2020  ands)}.         
-00004390: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
-000043a0: 6372 6970 7420 3d20 7372 632e 7361 6665  cript = src.safe
-000043b0: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
-000043c0: 7469 7475 7465 290a 2020 2020 2020 2020  titute).        
-000043d0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-000043e0: 6562 7567 2866 2273 7562 7374 6974 7574  ebug(f"substitut
-000043f0: 6564 3a5c 6e20 7b6a 6f62 5f73 6372 6970  ed:\n {job_scrip
-00004400: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
-00004410: 2020 2020 2023 2063 6f70 7920 746f 2072       # copy to r
-00004420: 656d 6f74 6520 6669 6c65 0a20 2020 2020  emote file.     
-00004430: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-00004440: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
-00004450: 6d5f 696d 6167 6573 5f70 6174 682b 222f  m_images_path+"/
-00004460: 222b 7363 7269 7074 5f6e 616d 650a 2020  "+script_name.  
-00004470: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
-00004480: 3d20 7365 6c66 2e70 7574 286c 6f63 616c  = self.put(local
-00004490: 3d69 6f2e 5374 7269 6e67 494f 286a 6f62  =io.StringIO(job
-000044a0: 5f73 6372 6970 7429 2c0a 2020 2020 2020  _script),.      
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 2020 2020 2072 656d 6f74 653d 6675         remote=fu
-000044d0: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
-000044e0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
-000044f0: 2274 696d 6520 7368 207b 7363 7269 7074  "time sh {script
-00004500: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
-00004510: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
-00004520: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
-00004530: 6d64 5d29 0a20 2020 2020 2020 2020 2020  md]).           
-00004540: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
-00004550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004560: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-00004570: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
-00004580: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00004590: 6572 2e69 6e66 6f28 722e 7374 646f 7574  er.info(r.stdout
-000045a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000045b0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2249    logger.info("I
-000045c0: 6e69 7469 6174 6564 2064 6f77 6e6c 6f61  nitiated downloa
-000045d0: 6469 6e67 2061 6e64 2062 7569 6c64 696e  ding and buildin
-000045e0: 6722 202b 0a20 2020 2020 2020 2020 2020  g" +.           
-000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004600: 2022 2063 6f6e 7461 696e 6572 2069 6d61   " container ima
-00004610: 6765 7320 6f6e 2053 6c75 726d 2e22 202b  ges on Slurm." +
-00004620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004630: 2020 2020 2020 2020 2020 2020 2022 2054               " T
-00004640: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
-00004650: 7768 696c 6520 696e 2074 6865 2062 6163  while in the bac
-00004660: 6b67 726f 756e 642e 2220 2b20 0a20 2020  kground." + .   
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 2020 2020 2020 2022 2043 6865 636b           " Check
-00004690: 2027 7369 6e67 2e6c 6f67 2720 6f6e 2053   'sing.log' on S
-000046a0: 6c75 726d 2066 6f72 2070 726f 6772 6573  lurm for progres
-000046b0: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
-000046c0: 2020 2020 2023 2023 2063 6c65 616e 7570       # # cleanup
-000046d0: 2067 6961 6e74 2073 696e 6775 6c61 7269   giant singulari
-000046e0: 7479 2063 6163 6865 210a 2020 2020 2020  ty cache!.      
-000046f0: 2020 2020 2020 2020 2020 2320 7573 696e            # usin
-00004700: 6720 2d2d 6469 7361 626c 652d 6361 6368  g --disable-cach
-00004710: 6520 6265 6361 7573 6520 7765 2072 756e  e because we run
-00004720: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
-00004730: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00004740: 2020 2023 2063 6d64 203d 2022 7369 6e67     # cmd = "sing
-00004750: 756c 6172 6974 7920 6361 6368 6520 636c  ularity cache cl
-00004760: 6561 6e20 2d66 220a 2020 2020 2020 2020  ean -f".        
-00004770: 2020 2020 2020 2020 2320 7220 3d20 7365          # r = se
-00004780: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00004790: 5b63 6d64 5d29 0a0a 2020 2020 6465 6620  [cmd])..    def 
-000047a0: 7365 7475 705f 636f 6e76 6572 7465 7273  setup_converters
-000047b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000047c0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
-000047d0: 2075 7020 636f 6e76 6572 7465 7273 2066   up converters f
-000047e0: 6f72 2053 6c75 726d 206f 7065 7261 7469  or Slurm operati
-000047f0: 6f6e 732e 0a0a 2020 2020 2020 2020 5468  ons...        Th
-00004800: 6973 2066 756e 6374 696f 6e20 6372 6561  is function crea
-00004810: 7465 7320 6e65 6365 7373 6172 7920 6469  tes necessary di
-00004820: 7265 6374 6f72 6965 7320 666f 7220 636f  rectories for co
-00004830: 6e76 6572 7465 7273 2061 6e64 2063 6f70  nverters and cop
-00004840: 6965 730a 2020 2020 2020 2020 636f 6e76  ies.        conv
-00004850: 6572 7465 7220 7363 7269 7074 7320 616e  erter scripts an
-00004860: 6420 6465 6669 6e69 7469 6f6e 7320 746f  d definitions to
-00004870: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
-00004880: 206c 6f63 6174 696f 6e73 2e20 4974 2061   locations. It a
-00004890: 6c73 6f0a 2020 2020 2020 2020 6275 696c  lso.        buil
-000048a0: 6473 2053 696e 6775 6c61 7269 7479 2063  ds Singularity c
-000048b0: 6f6e 7461 696e 6572 7320 6672 6f6d 2074  ontainers from t
-000048c0: 6865 2070 726f 7669 6465 6420 6465 6669  he provided defi
-000048d0: 6e69 7469 6f6e 732e 0a0a 2020 2020 2020  nitions...      
-000048e0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-000048f0: 2020 2020 2020 5353 4845 7863 6570 7469        SSHExcepti
-00004900: 6f6e 3a20 4966 2074 6865 7265 2069 7320  on: If there is 
-00004910: 616e 2069 7373 7565 2065 7865 6375 7469  an issue executi
-00004920: 6e67 2063 6f6d 6d61 6e64 7320 6f72 2063  ng commands or c
-00004930: 6f70 7969 6e67 2066 696c 6573 2e0a 2020  opying files..  
-00004940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00004950: 2020 636f 6e76 6572 745f 636d 6473 203d    convert_cmds =
-00004960: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-00004970: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
-00004980: 7465 7273 5f70 6174 683a 0a20 2020 2020  ters_path:.     
-00004990: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
-000049a0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-000049b0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-000049c0: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
-000049d0: 687d 2229 0a20 2020 2020 2020 2072 203d  h}").        r =
-000049e0: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-000049f0: 6473 2863 6f6e 7665 7274 5f63 6d64 7329  ds(convert_cmds)
-00004a00: 0a20 2020 2020 2020 2023 2063 6f70 7920  .        # copy 
-00004a10: 6765 6e65 7269 6320 6a6f 6220 6172 7261  generic job arra
-00004a20: 7920 7363 7269 7074 206f 7665 7220 746f  y script over to
-00004a30: 2073 6c75 726d 0a20 2020 2020 2020 2063   slurm.        c
-00004a40: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
-00004a50: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
-00004a60: 6365 7322 292e 6a6f 696e 7061 7468 280a  ces").joinpath(.
-00004a70: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00004a80: 7665 7274 5f6a 6f62 5f61 7272 6179 2e73  vert_job_array.s
-00004a90: 6822 290a 2020 2020 2020 2020 5f20 3d20  h").        _ = 
-00004aa0: 7365 6c66 2e70 7574 286c 6f63 616c 3d63  self.put(local=c
-00004ab0: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
-00004ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004ad0: 2020 2020 2020 2072 656d 6f74 653d 7365         remote=se
-00004ae0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-00004af0: 7061 7468 290a 2020 2020 2020 2020 2320  path).        # 
-00004b00: 6375 7272 656e 746c 7920 6b6e 6f77 6e20  currently known 
-00004b10: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
-00004b20: 2020 2023 2033 612e 205a 4152 5220 746f     # 3a. ZARR to
-00004b30: 2054 4946 460a 2020 2020 2020 2020 2320   TIFF.        # 
-00004b40: 544f 444f 2065 7874 7261 6374 2074 6865  TODO extract the
-00004b50: 7365 2076 616c 7565 7320 746f 2065 2e67  se values to e.g
-00004b60: 2e20 636f 6e66 6967 2069 6620 7765 2068  . config if we h
-00004b70: 6176 6520 6d6f 7265 0a20 2020 2020 2020  ave more.       
-00004b80: 2063 6f6e 7665 7274 5f6e 616d 6520 3d20   convert_name = 
-00004b90: 2263 6f6e 7665 7274 5f7a 6172 725f 746f  "convert_zarr_to
-00004ba0: 5f74 6966 6622 0a20 2020 2020 2020 2063  _tiff".        c
-00004bb0: 6f6e 7665 7274 5f70 7920 3d20 6622 7b63  onvert_py = f"{c
-00004bc0: 6f6e 7665 7274 5f6e 616d 657d 2e70 7922  onvert_name}.py"
-00004bd0: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
-00004be0: 5f73 6372 6970 745f 6c6f 6361 6c20 3d20  _script_local = 
-00004bf0: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
-00004c00: 2229 2e6a 6f69 6e70 6174 6828 0a20 2020  ").joinpath(.   
-00004c10: 2020 2020 2020 2020 2063 6f6e 7665 7274           convert
-00004c20: 5f70 7929 0a20 2020 2020 2020 2063 6f6e  _py).        con
-00004c30: 7665 7274 5f64 6566 203d 2066 227b 636f  vert_def = f"{co
-00004c40: 6e76 6572 745f 6e61 6d65 7d2e 6465 6622  nvert_name}.def"
-00004c50: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
-00004c60: 5f64 6566 5f6c 6f63 616c 203d 2066 696c  _def_local = fil
-00004c70: 6573 2822 7265 736f 7572 6365 7322 292e  es("resources").
-00004c80: 6a6f 696e 7061 7468 280a 2020 2020 2020  joinpath(.      
-00004c90: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
-00004ca0: 6629 0a20 2020 2020 2020 205f 203d 2073  f).        _ = s
-00004cb0: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
-00004cc0: 6e76 6572 745f 7363 7269 7074 5f6c 6f63  nvert_script_loc
-00004cd0: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00004ce0: 2020 2020 2020 2020 2072 656d 6f74 653d           remote=
-00004cf0: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
-00004d00: 7274 6572 735f 7061 7468 290a 2020 2020  rters_path).    
-00004d10: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
-00004d20: 286c 6f63 616c 3d63 6f6e 7665 7274 5f64  (local=convert_d
-00004d30: 6566 5f6c 6f63 616c 2c0a 2020 2020 2020  ef_local,.      
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004d50: 656d 6f74 653d 7365 6c66 2e73 6c75 726d  emote=self.slurm
-00004d60: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
-00004d70: 290a 2020 2020 2020 2020 2320 4275 696c  ).        # Buil
-00004d80: 6420 7369 6e67 756c 6172 6974 7920 636f  d singularity co
-00004d90: 6e74 6169 6e65 7220 6672 6f6d 2064 6566  ntainer from def
-00004da0: 696e 6974 696f 6e0a 2020 2020 2020 2020  inition.        
-00004db0: 7769 7468 2073 656c 662e 6364 2873 656c  with self.cd(sel
-00004dc0: 662e 736c 7572 6d5f 636f 6e76 6572 7465  f.slurm_converte
-00004dd0: 7273 5f70 6174 6829 3a0a 2020 2020 2020  rs_path):.      
-00004de0: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
-00004df0: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
-00004e00: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00004e10: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
-00004e20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004e30: 2054 4f44 4f20 4368 616e 6765 2074 6865   TODO Change the
-00004e40: 2074 6d70 2064 6972 3f0a 2020 2020 2020   tmp dir?.      
-00004e50: 2020 2020 2020 2020 2020 2320 6578 706f            # expo
-00004e60: 7274 2053 494e 4755 4c41 5249 5459 5f54  rt SINGULARITY_T
-00004e70: 4d50 4449 523d 7e2f 6d79 2d73 6372 6174  MPDIR=~/my-scrat
-00004e80: 6368 2f74 6d70 3b0a 2020 2020 2020 2020  ch/tmp;.        
-00004e90: 2020 2020 2020 2020 2320 6f6e 6c79 2069          # only i
-00004ea0: 6620 6669 6c65 2064 6f65 7320 6e6f 7420  f file does not 
-00004eb0: 6578 6973 7420 7965 740a 2020 2020 2020  exist yet.      
-00004ec0: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
-00004ed0: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
-00004ee0: 6622 5b20 2120 2d66 207b 636f 6e76 6572  f"[ ! -f {conver
-00004ef0: 745f 6e61 6d65 7d2e 7369 6620 5d22 290a  t_name}.sif ]").
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2320 4544 4954 202d 2d20 4e4f 2c20 7468  # EDIT -- NO, th
-00004f20: 656e 2077 6520 6361 6e27 7420 7570 6461  en we can't upda
-00004f30: 7465 2120 466f 7263 6520 7265 6275 696c  te! Force rebuil
-00004f40: 6421 0a20 2020 2020 2020 2020 2020 2020  d!.             
-00004f50: 2020 2023 2064 6f77 6e6c 6f61 6420 2f62     # download /b
-00004f60: 7569 6c64 206e 6577 2063 6f6e 7461 696e  uild new contain
-00004f70: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-00004f80: 2020 2063 6f6e 7665 7274 5f63 6d64 732e     convert_cmds.
-00004f90: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-00004fa0: 2020 2020 2020 2020 2020 2020 6622 7369              f"si
-00004fb0: 6e67 756c 6172 6974 7920 6275 696c 6420  ngularity build 
-00004fc0: 2d46 207b 636f 6e76 6572 745f 6e61 6d65  -F {convert_name
-00004fd0: 7d2e 7369 6620 7b63 6f6e 7665 7274 5f64  }.sif {convert_d
-00004fe0: 6566 7d20 3e3e 2073 696e 672e 6c6f 6720  ef} >> sing.log 
-00004ff0: 323e 2631 203b 2065 6368 6f20 2766 696e  2>&1 ; echo 'fin
-00005000: 6973 6865 6420 7b63 6f6e 7665 7274 5f6e  ished {convert_n
-00005010: 616d 657d 2e73 6966 2720 2622 290a 2020  ame}.sif' &").  
-00005020: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
-00005030: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00005040: 636f 6e76 6572 745f 636d 6473 290a 0a20  convert_cmds).. 
-00005050: 2020 2064 6566 2073 6574 7570 5f6a 6f62     def setup_job
-00005060: 5f73 6372 6970 7473 2873 656c 6629 3a0a  _scripts(self):.
-00005070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005080: 2020 2020 5365 7473 2075 7020 6a6f 6220      Sets up job 
-00005090: 7363 7269 7074 7320 666f 7220 536c 7572  scripts for Slur
-000050a0: 6d20 6f70 6572 6174 696f 6e73 2e0a 0a20  m operations... 
-000050b0: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
-000050c0: 7469 6f6e 2065 6974 6865 7220 636c 6f6e  tion either clon
-000050d0: 6573 2061 2047 6974 2072 6570 6f73 6974  es a Git reposit
-000050e0: 6f72 7920 636f 6e74 6169 6e69 6e67 206a  ory containing j
-000050f0: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
-00005100: 2020 2069 6e74 6f20 7468 6520 7370 6563     into the spec
-00005110: 6966 6965 6420 7363 7269 7074 2070 6174  ified script pat
-00005120: 6820 6f72 2067 656e 6572 6174 6573 2073  h or generates s
-00005130: 6372 6970 7473 206c 6f63 616c 6c79 2069  cripts locally i
-00005140: 6620 6e6f 2072 6570 6f73 6974 6f72 790a  f no repository.
-00005150: 2020 2020 2020 2020 6973 2070 726f 7669          is provi
-00005160: 6465 642e 0a0a 2020 2020 2020 2020 5261  ded...        Ra
-00005170: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-00005180: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
-00005190: 4966 2074 6865 7265 2069 7320 616e 2069  If there is an i
-000051a0: 7373 7565 2065 7865 6375 7469 6e67 2047  ssue executing G
-000051b0: 6974 2063 6f6d 6d61 6e64 7320 6f72 2067  it commands or g
-000051c0: 656e 6572 6174 696e 6720 7363 7269 7074  enerating script
-000051d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-000051e0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000051f0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-00005200: 2061 6e64 2073 656c 662e 736c 7572 6d5f   and self.slurm_
-00005210: 7363 7269 7074 5f70 6174 683a 0a20 2020  script_path:.   
-00005220: 2020 2020 2020 2020 2023 2067 6974 2063           # git c
-00005230: 6c6f 6e65 2069 6e74 6f20 7363 7269 7074  lone into script
-00005240: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
-00005250: 2020 656e 7620 3d20 7b0a 2020 2020 2020    env = {.      
-00005260: 2020 2020 2020 2020 2020 2252 4550 4f53            "REPOS
-00005270: 5243 223a 2073 656c 662e 736c 7572 6d5f  RC": self.slurm_
-00005280: 7363 7269 7074 5f72 6570 6f2c 0a20 2020  script_repo,.   
-00005290: 2020 2020 2020 2020 2020 2020 2022 4c4f               "LO
-000052a0: 4341 4c52 4550 4f22 3a20 7365 6c66 2e73  CALREPO": self.s
-000052b0: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
-000052c0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000052d0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-000052e0: 2027 6769 7420 636c 6f6e 6520 2224 5245   'git clone "$RE
-000052f0: 504f 5352 4322 2022 244c 4f43 414c 5245  POSRC" "$LOCALRE
-00005300: 504f 2220 323e 202f 6465 762f 6e75 6c6c  PO" 2> /dev/null
-00005310: 207c 7c20 6769 7420 2d43 2022 244c 4f43   || git -C "$LOC
-00005320: 414c 5245 504f 2220 7075 6c6c 270a 2020  ALREPO" pull'.  
-00005330: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
-00005340: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00005350: 5b63 6d64 5d2c 2065 6e76 290a 2020 2020  [cmd], env).    
-00005360: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00005370: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
-00005380: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00005390: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
-000053a0: 2020 2065 6c69 6620 7365 6c66 2e73 6c75     elif self.slu
-000053b0: 726d 5f73 6372 6970 745f 7061 7468 3a0a  rm_script_path:.
-000053c0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-000053d0: 6e65 7261 7465 2073 6372 6970 7473 0a20  nerate scripts. 
-000053e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000053f0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
-00005400: 6970 7473 2867 656e 6572 6174 655f 6a6f  ipts(generate_jo
-00005410: 6273 3d54 7275 6529 0a0a 2020 2020 6465  bs=True)..    de
-00005420: 6620 7365 7475 705f 6469 7265 6374 6f72  f setup_director
-00005430: 6965 7328 7365 6c66 293a 0a20 2020 2020  ies(self):.     
-00005440: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00005450: 7265 6174 6573 206e 6563 6573 7361 7279  reates necessary
-00005460: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
-00005470: 2053 6c75 726d 206f 7065 7261 7469 6f6e   Slurm operation
-00005480: 732e 0a0a 2020 2020 2020 2020 5468 6973  s...        This
-00005490: 2066 756e 6374 696f 6e20 6372 6561 7465   function create
-000054a0: 7320 6469 7265 6374 6f72 6965 7320 666f  s directories fo
-000054b0: 7220 6461 7461 2073 746f 7261 6765 2c20  r data storage, 
-000054c0: 7363 7269 7074 732c 2061 6e64 2077 6f72  scripts, and wor
-000054d0: 6b66 6c6f 7773 0a20 2020 2020 2020 2061  kflows.        a
-000054e0: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-000054f0: 6865 2053 6c75 726d 436c 6965 6e74 206f  he SlurmClient o
-00005500: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
-00005510: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00005520: 2020 2020 5353 4845 7863 6570 7469 6f6e      SSHException
-00005530: 3a20 4966 2074 6865 7265 2069 7320 616e  : If there is an
-00005540: 2069 7373 7565 2065 7865 6375 7469 6e67   issue executing
-00005550: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
-00005560: 696f 6e20 636f 6d6d 616e 6473 2e0a 2020  ion commands..  
-00005570: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005580: 2020 6469 725f 636d 6473 203d 205b 5d0a    dir_cmds = [].
-00005590: 2020 2020 2020 2020 2320 612e 2064 6174          # a. dat
-000055a0: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
-000055b0: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-000055c0: 683a 0a20 2020 2020 2020 2020 2020 2064  h:.            d
-000055d0: 6972 5f63 6d64 732e 6170 7065 6e64 2866  ir_cmds.append(f
-000055e0: 226d 6b64 6972 202d 7020 7b73 656c 662e  "mkdir -p {self.
-000055f0: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-00005600: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
-00005610: 2062 2e20 7363 7269 7074 730a 2020 2020   b. scripts.    
-00005620: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00005630: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
-00005640: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
-00005650: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-00005660: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-00005670: 6d5f 7363 7269 7074 5f70 6174 687d 2229  m_script_path}")
-00005680: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00005690: 2e20 776f 726b 666c 6f77 730a 2020 2020  . workflows.    
-000056a0: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-000056b0: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
-000056c0: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
-000056d0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
-000056e0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
-000056f0: 6d5f 696d 6167 6573 5f70 6174 687d 2229  m_images_path}")
-00005700: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
-00005710: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
-00005720: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
-00005730: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
-00005740: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00005750: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
-00005760: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00005770: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
-00005780: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
-00005790: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
-000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057b0: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
-000057c0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-000057d0: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
-000057e0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-000057f0: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
-00005800: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
-00005810: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
-00005820: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
-00005830: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-00005840: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
-00005850: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
-00005860: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
-00005870: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
-00005880: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
-00005890: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
-000058a0: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
-000058b0: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
-000058c0: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
-000058d0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
-000058e0: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
-000058f0: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
-00005900: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
-00005910: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
-00005920: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
-00005930: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
-00005940: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
-00005950: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
-00005960: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
-00005970: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
-00005980: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
-00005990: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
-000059a0: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
-000059b0: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
-000059c0: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
-000059d0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-000059e0: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
-000059f0: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
-00005a00: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
-00005a10: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
-00005a20: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
-00005a30: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00005a40: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00005a50: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
-00005a60: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
-00005a70: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
-00005a80: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
-00005a90: 2020 2020 2020 2020 2020 2020 696e 6974              init
-00005aa0: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
-00005ab0: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
-00005ac0: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
-00005ad0: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
-00005ae0: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
-00005af0: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
-00005b00: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
-00005b10: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
-00005b20: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
-00005b30: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00005b40: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
-00005b50: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
-00005b60: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00005b70: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
-00005b80: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
-00005b90: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
-00005ba0: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
-00005bb0: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
-00005bc0: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
-00005bd0: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
-00005be0: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
-00005bf0: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
-00005c00: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
-00005c10: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
-00005c20: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
-00005c30: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
-00005c40: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
-00005c50: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
-00005c80: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
-00005cb0: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
-00005cc0: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
-00005cd0: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
-00005ce0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00005cf0: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
-00005d00: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
-00005d10: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
-00005d20: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
-00005d30: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
-00005d40: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
-00005d50: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
-00005d60: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
-00005d70: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
-00005d80: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
-00005d90: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
-00005da0: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
-00005db0: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
-00005dc0: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
-00005dd0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
-00005de0: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
-00005df0: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
-00005e00: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
-00005e10: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
-00005e20: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
-00005e30: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
-00005e40: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00005e50: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-00005e60: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
-00005e70: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
-00005e80: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
-00005e90: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
-00005ea0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-00005eb0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-00005ec0: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
-00005ed0: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
-00005ee0: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
-00005ef0: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
-00005f00: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
-00005f10: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
-00005f20: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
-00005f30: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-00005f40: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-00005f50: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
-00005f60: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
-00005f70: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
-00005f80: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
-00005f90: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
-00005fa0: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
-00005fb0: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
-00005fc0: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
-00005fd0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00005fe0: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
-00005ff0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006000: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
-00006010: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00006020: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
-00006030: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00006040: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
-00006050: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
-00006060: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
-00006070: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00006080: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
-00006090: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
-000060a0: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
-000060b0: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
-000060c0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-000060d0: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
-000060e0: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
-000060f0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00006100: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
-00006110: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
-00006120: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
-00006130: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
-00006140: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
-00006150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006160: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
-00006170: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
-00006180: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
-00006190: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-000061a0: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
-000061b0: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
-000061c0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-000061d0: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
-000061e0: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
-000061f0: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
-00006200: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00006210: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
-00006220: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
-00006230: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00006240: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
-00006250: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
-00006260: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
-00006270: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
-00006280: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
-00006290: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000062a0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-000062b0: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
-000062c0: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
-000062d0: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
-00006300: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
-00006310: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
-00006320: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
-00006330: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
-00006340: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
-00006350: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00006360: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006370: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-00006380: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
-00006390: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-000063a0: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
-000063b0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-000063c0: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
-000063d0: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
-000063e0: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
-000063f0: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
-00006400: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
-00006410: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
-00006420: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
-00006430: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
-00006440: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
-00006450: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
-00006460: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
-00006470: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
-00006480: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
-00006490: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-000064a0: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
-000064b0: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-000064c0: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
-000064d0: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
-000064e0: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
-000064f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00006500: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
-00006530: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
-00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
-00006560: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
-00006570: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00006580: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
-00006590: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
-000065a0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000065c0: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
-000065d0: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
-000065e0: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006600: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
-00006610: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
-00006620: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-00006630: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006640: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
-00006650: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
-00006660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006670: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
-00006680: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00006690: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-000066a0: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
-000066b0: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066d0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-000066e0: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
-000066f0: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
-00006700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006710: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00006720: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
-00006730: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
-00006740: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00006750: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
-00006760: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-00006770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006780: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
-00006790: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
-000067a0: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
-000067b0: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
-000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067d0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-000067e0: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
-00006810: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00006820: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00006830: 615f 6c6f 6361 7469 6f6e 3a20 7374 7220  a_location: str 
-00006840: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
-00006870: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2029 202d 3e20 5265 7375 6c74 3a0a 2020   ) -> Result:.  
-000068a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000068b0: 2020 436c 6561 6e75 7020 7a69 7020 616e    Cleanup zip an
-000068c0: 6420 756e 7a69 7070 6564 2066 696c 6573  d unzipped files
-000068d0: 2f66 6f6c 6465 7273 2061 7373 6f63 6961  /folders associa
-000068e0: 7465 6420 7769 7468 2061 2053 6c75 726d  ted with a Slurm
-000068f0: 206a 6f62 2e0a 0a20 2020 2020 2020 2041   job...        A
-00006900: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00006910: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
-00006920: 7472 293a 2054 6865 206a 6f62 2049 4420  tr): The job ID 
-00006930: 6f66 2074 6865 2053 6c75 726d 2073 6372  of the Slurm scr
-00006940: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
-00006950: 2066 696c 656e 616d 6520 2873 7472 293a   filename (str):
-00006960: 2054 6865 207a 6970 2066 696c 656e 616d   The zip filenam
-00006970: 6520 6f6e 2053 6c75 726d 2e0a 2020 2020  e on Slurm..    
-00006980: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
-00006990: 6174 696f 6e20 2873 7472 2c20 6f70 7469  ation (str, opti
-000069a0: 6f6e 616c 293a 2054 6865 206c 6f63 6174  onal): The locat
-000069b0: 696f 6e20 6f66 2064 6174 6120 6669 6c65  ion of data file
-000069c0: 7320 6f6e 2053 6c75 726d 2e0a 2020 2020  s on Slurm..    
-000069d0: 2020 2020 2020 2020 2020 2020 4966 206e              If n
-000069e0: 6f74 2070 726f 7669 6465 642c 2069 7420  ot provided, it 
-000069f0: 7769 6c6c 2062 6520 6578 7472 6163 7465  will be extracte
-00006a00: 6420 6672 6f6d 2074 6865 206c 6f67 2066  d from the log f
-00006a10: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
-00006a20: 206c 6f67 6669 6c65 2028 7374 722c 206f   logfile (str, o
-00006a30: 7074 696f 6e61 6c29 3a20 5468 6520 6c6f  ptional): The lo
-00006a40: 6720 6669 6c65 206f 6620 7468 6520 536c  g file of the Sl
-00006a50: 7572 6d20 6a6f 622e 200a 2020 2020 2020  urm job. .      
-00006a60: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
-00006a70: 2070 726f 7669 6465 642c 2061 2064 6566   provided, a def
-00006a80: 6175 6c74 206c 6f67 2066 696c 6520 7769  ault log file wi
-00006a90: 6c6c 2062 6520 7573 6564 2e0a 0a20 2020  ll be used...   
-00006aa0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00006ab0: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
-00006ac0: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
-00006ad0: 7468 6520 636c 6561 6e75 7020 6f70 6572  the cleanup oper
-00006ae0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00006af0: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
-00006b00: 2020 5468 6520 636c 6561 6e75 7020 7072    The cleanup pr
-00006b10: 6f63 6573 7320 696e 766f 6c76 6573 2072  ocess involves r
-00006b20: 656d 6f76 696e 6720 7468 6520 7370 6563  emoving the spec
-00006b30: 6966 6965 6420 7a69 7020 6669 6c65 2c20  ified zip file, 
-00006b40: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-00006b50: 206c 6f67 2066 696c 652c 2061 6e64 2061   log file, and a
-00006b60: 7373 6f63 6961 7465 6420 6461 7461 2066  ssociated data f
-00006b70: 696c 6573 2061 6e64 2066 6f6c 6465 7273  iles and folders
-00006b80: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00006b90: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00006ba0: 2320 436c 6561 6e75 7020 7465 6d70 6f72  # Cleanup tempor
-00006bb0: 6172 7920 6669 6c65 7320 666f 7220 6120  ary files for a 
-00006bc0: 536c 7572 6d20 6a6f 620a 2020 2020 2020  Slurm job.      
-00006bd0: 2020 2020 2020 636c 6965 6e74 2e63 6c65        client.cle
-00006be0: 616e 7570 5f74 6d70 5f66 696c 6573 2822  anup_tmp_files("
-00006bf0: 3132 3334 3522 2c20 226f 7574 7075 742e  12345", "output.
-00006c00: 7a69 7022 290a 2020 2020 2020 2020 2222  zip").        ""
-00006c10: 220a 2020 2020 2020 2020 636d 6473 203d  ".        cmds =
-00006c20: 205b 5d0a 2020 2020 2020 2020 2320 7a69   [].        # zi
-00006c30: 700a 2020 2020 2020 2020 726d 7a69 7020  p.        rmzip 
-00006c40: 3d20 6622 726d 207b 6669 6c65 6e61 6d65  = f"rm {filename
-00006c50: 7d2e 2a22 0a20 2020 2020 2020 2063 6d64  }.*".        cmd
-00006c60: 732e 6170 7065 6e64 2872 6d7a 6970 290a  s.append(rmzip).
-00006c70: 2020 2020 2020 2020 2320 6c6f 670a 2020          # log.  
-00006c80: 2020 2020 2020 6966 206c 6f67 6669 6c65        if logfile
-00006c90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006ca0: 2020 2020 2020 6c6f 6766 696c 6520 3d20        logfile = 
-00006cb0: 7365 6c66 2e5f 4c4f 4746 494c 450a 2020  self._LOGFILE.  
-00006cc0: 2020 2020 2020 2020 2020 6c6f 6766 696c            logfil
-00006cd0: 6520 3d20 6c6f 6766 696c 652e 666f 726d  e = logfile.form
-00006ce0: 6174 2873 6c75 726d 5f6a 6f62 5f69 643d  at(slurm_job_id=
-00006cf0: 736c 7572 6d5f 6a6f 625f 6964 290a 2020  slurm_job_id).  
-00006d00: 2020 2020 2020 726d 6c6f 6720 3d20 6622        rmlog = f"
-00006d10: 726d 207b 6c6f 6766 696c 657d 220a 2020  rm {logfile}".  
-00006d20: 2020 2020 2020 636d 6473 2e61 7070 656e        cmds.appen
-00006d30: 6428 726d 6c6f 6729 0a20 2020 2020 2020  d(rmlog).       
-00006d40: 2023 2064 6174 610a 2020 2020 2020 2020   # data.        
-00006d50: 6966 2064 6174 615f 6c6f 6361 7469 6f6e  if data_location
-00006d60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006d70: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
-00006d80: 696f 6e20 3d20 7365 6c66 2e65 7874 7261  ion = self.extra
-00006d90: 6374 5f64 6174 615f 6c6f 6361 7469 6f6e  ct_data_location
-00006da0: 5f66 726f 6d5f 6c6f 6728 6c6f 6766 696c  _from_log(logfil
-00006db0: 6529 0a20 2020 2020 2020 2072 6d64 6174  e).        rmdat
-00006dc0: 6120 3d20 6622 726d 202d 7266 207b 6461  a = f"rm -rf {da
-00006dd0: 7461 5f6c 6f63 6174 696f 6e7d 207b 6461  ta_location} {da
-00006de0: 7461 5f6c 6f63 6174 696f 6e7d 2e2a 220a  ta_location}.*".
-00006df0: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
-00006e00: 656e 6428 726d 6461 7461 290a 0a20 2020  end(rmdata)..   
-00006e10: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00006e20: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-00006e30: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-00006e40: 2863 6d64 7329 0a20 2020 2020 2020 2065  (cmds).        e
-00006e50: 7863 6570 7420 556e 6578 7065 6374 6564  xcept Unexpected
-00006e60: 4578 6974 2061 7320 653a 0a20 2020 2020  Exit as e:.     
-00006e70: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00006e80: 726e 696e 6728 6529 0a20 2020 2020 2020  rning(e).       
-00006e90: 2020 2020 2072 6573 756c 7420 3d20 652e       result = e.
-00006ea0: 7265 7375 6c74 0a20 2020 2020 2020 2072  result.        r
-00006eb0: 6574 7572 6e20 7265 7375 6c74 206f 7220  eturn result or 
-00006ec0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7661  None..    def va
-00006ed0: 6c69 6461 7465 2873 656c 662c 2076 616c  lidate(self, val
-00006ee0: 6964 6174 655f 736c 7572 6d5f 7365 7475  idate_slurm_setu
-00006ef0: 703a 2062 6f6f 6c20 3d20 4661 6c73 6529  p: bool = False)
-00006f00: 3a0a 2020 2020 2020 2020 2222 2256 616c  :.        """Val
-00006f10: 6964 6174 6520 7468 6520 636f 6e6e 6563  idate the connec
-00006f20: 7469 6f6e 2074 6f20 7468 6520 536c 7572  tion to the Slur
-00006f30: 6d20 636c 7573 7465 7220 6279 2072 756e  m cluster by run
-00006f40: 6e69 6e67 0a20 2020 2020 2020 2061 2073  ning.        a s
-00006f50: 696d 706c 6520 636f 6d6d 616e 642e 0a0a  imple command...
-00006f60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00006f70: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-00006f80: 7465 5f73 6c75 726d 5f73 6574 7570 2028  te_slurm_setup (
-00006f90: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
-00006fa0: 6f20 616c 736f 2063 6865 636b 0a20 2020  o also check.   
-00006fb0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00006fc0: 2066 6978 2074 6865 2053 6c75 726d 2073   fix the Slurm s
-00006fd0: 6574 7570 2028 666f 6c64 6572 732c 2069  etup (folders, i
-00006fe0: 6d61 6765 732c 2065 7463 2e29 0a0a 2020  mages, etc.)..  
-00006ff0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00007000: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
-00007010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007020: 2054 7275 6520 6966 2074 6865 2076 616c   True if the val
-00007030: 6964 6174 696f 6e20 6973 2073 7563 6365  idation is succe
-00007040: 7373 6675 6c2c 0a20 2020 2020 2020 2020  ssful,.         
-00007050: 2020 2020 2020 2046 616c 7365 206f 7468         False oth
-00007060: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00007070: 2222 220a 2020 2020 2020 2020 636f 6e6e  """.        conn
-00007080: 6563 7465 6420 3d20 7365 6c66 2e72 756e  ected = self.run
-00007090: 2827 6563 686f 2022 2022 2729 2e6f 6b0a  ('echo " "').ok.
-000070a0: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
-000070b0: 6374 6564 2061 6e64 2076 616c 6964 6174  cted and validat
-000070c0: 655f 736c 7572 6d5f 7365 7475 703a 0a20  e_slurm_setup:. 
-000070d0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 7365 6c66 2e73 6574 7570 5f73 6c75 726d  self.setup_slurm
-00007100: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-00007110: 7863 6570 7420 5353 4845 7863 6570 7469  xcept SSHExcepti
-00007120: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00007130: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007140: 6572 726f 7228 6529 0a20 2020 2020 2020  error(e).       
-00007150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007160: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
-00007170: 7475 726e 2063 6f6e 6e65 6374 6564 0a0a  turn connected..
-00007180: 2020 2020 6465 6620 6765 745f 7265 6365      def get_rece
-00007190: 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64 2873  nt_log_command(s
-000071a0: 656c 662c 206c 6f67 5f66 696c 653a 2073  elf, log_file: s
-000071b0: 7472 2c20 6e3a 2069 6e74 203d 2031 3029  tr, n: int = 10)
-000071c0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-000071d0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-000071e0: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
-000071f0: 7265 7472 6965 7665 2074 6865 2072 6563  retrieve the rec
-00007200: 656e 7420 6c6f 6720 656e 7472 6965 7320  ent log entries 
-00007210: 6672 6f6d 2061 0a20 2020 2020 2020 2073  from a.        s
-00007220: 7065 6369 6669 6564 206c 6f67 2066 696c  pecified log fil
-00007230: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-00007240: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00007250: 675f 6669 6c65 2028 7374 7229 3a20 5468  g_file (str): Th
-00007260: 6520 7061 7468 2074 6f20 7468 6520 6c6f  e path to the lo
-00007270: 6720 6669 6c65 2e0a 2020 2020 2020 2020  g file..        
-00007280: 2020 2020 6e20 2869 6e74 2c20 6f70 7469      n (int, opti
-00007290: 6f6e 616c 293a 2054 6865 206e 756d 6265  onal): The numbe
-000072a0: 7220 6f66 2072 6563 656e 7420 6c6f 6720  r of recent log 
-000072b0: 656e 7472 6965 7320 746f 2072 6574 7269  entries to retri
-000072c0: 6576 652e 0a20 2020 2020 2020 2020 2020  eve..           
-000072d0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-000072e0: 2031 302e 0a0a 2020 2020 2020 2020 5265   10...        Re
-000072f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00007300: 2020 2073 7472 3a20 5468 6520 636f 6d6d     str: The comm
-00007310: 616e 6420 746f 2072 6574 7269 6576 6520  and to retrieve 
-00007320: 7468 6520 7265 6365 6e74 206c 6f67 2065  the recent log e
-00007330: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
-00007340: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00007350: 726e 2073 656c 662e 5f54 4149 4c5f 4c4f  rn self._TAIL_LO
-00007360: 475f 434d 442e 666f 726d 6174 286e 3d6e  G_CMD.format(n=n
-00007370: 2c20 6c6f 675f 6669 6c65 3d6c 6f67 5f66  , log_file=log_f
-00007380: 696c 6529 0a0a 2020 2020 6465 6620 6765  ile)..    def ge
-00007390: 745f 6163 7469 7665 5f6a 6f62 5f70 726f  t_active_job_pro
-000073a0: 6772 6573 7328 7365 6c66 2c0a 2020 2020  gress(self,.    
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-000073d0: 6d5f 6a6f 625f 6964 3a20 7374 722c 0a20  m_job_id: str,. 
-000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007400: 6174 7465 726e 3a20 7374 7220 3d20 7222  attern: str = r"
-00007410: 5c64 2b25 222c 0a20 2020 2020 2020 2020  \d+%",.         
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00007440: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00007450: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-00007460: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-00007470: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
-00007480: 2070 726f 6772 6573 7320 6f66 2061 6e20   progress of an 
-00007490: 6163 7469 7665 2053 6c75 726d 206a 6f62  active Slurm job
-000074a0: 2066 726f 6d20 6974 7320 6c6f 6766 696c   from its logfil
-000074b0: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
-000074c0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-000074d0: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
-000074e0: 293a 2054 6865 2049 4420 6f66 2074 6865  ): The ID of the
-000074f0: 2053 6c75 726d 206a 6f62 2e0a 2020 2020   Slurm job..    
-00007500: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
-00007510: 2873 7472 293a 2054 6865 2070 6174 7465  (str): The patte
-00007520: 726e 2074 6f20 6d61 7463 6820 696e 2074  rn to match in t
-00007530: 6865 206a 6f62 206c 6f67 2074 6f20 6578  he job log to ex
-00007540: 7472 6163 740a 2020 2020 2020 2020 2020  tract.          
-00007550: 2020 2020 2020 7468 6520 7072 6f67 7265        the progre
-00007560: 7373 2028 6465 6661 756c 743a 2072 225c  ss (default: r"\
-00007570: 642b 2522 292e 0a0a 2020 2020 2020 2020  d+%")...        
-00007580: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
-00007590: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-000075a0: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
-000075b0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-000075c0: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
-000075d0: 2020 2020 746f 2073 6574 2077 6865 6e20      to set when 
-000075e0: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-000075f0: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-00007600: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00007610: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00007620: 2020 2020 2073 7472 3a20 5468 6520 7072       str: The pr
-00007630: 6f67 7265 7373 206f 6620 7468 6520 536c  ogress of the Sl
-00007640: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
-00007650: 2022 2222 0a20 2020 2020 2020 2063 6d64   """.        cmd
-00007660: 6c69 7374 203d 205b 5d0a 2020 2020 2020  list = [].      
-00007670: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
-00007680: 5f72 6563 656e 745f 6c6f 675f 636f 6d6d  _recent_log_comm
-00007690: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
-000076a0: 206c 6f67 5f66 696c 653d 7365 6c66 2e5f   log_file=self._
-000076b0: 4c4f 4746 494c 452e 666f 726d 6174 2873  LOGFILE.format(s
-000076c0: 6c75 726d 5f6a 6f62 5f69 643d 736c 7572  lurm_job_id=slur
-000076d0: 6d5f 6a6f 625f 6964 2929 0a20 2020 2020  m_job_id)).     
-000076e0: 2020 2063 6d64 6c69 7374 2e61 7070 656e     cmdlist.appen
-000076f0: 6428 636d 6429 0a20 2020 2020 2020 2069  d(cmd).        i
-00007700: 6620 656e 7620 6973 204e 6f6e 653a 0a20  f env is None:. 
-00007710: 2020 2020 2020 2020 2020 2065 6e76 203d             env =
-00007720: 207b 7d0a 2020 2020 2020 2020 7472 793a   {}.        try:
-00007730: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007740: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-00007750: 6f6d 6d61 6e64 7328 636d 646c 6973 742c  ommands(cmdlist,
-00007760: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
-00007770: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00007780: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00007790: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
-000077a0: 7228 6622 4973 7375 6520 7769 7468 2072  r(f"Issue with r
-000077b0: 756e 2063 6f6d 6d61 6e64 3a20 7b65 7d22  un command: {e}"
-000077c0: 290a 2020 2020 2020 2020 2320 4d61 7463  ).        # Matc
-000077d0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-000077e0: 7061 7474 6572 6e20 696e 2074 6865 2072  pattern in the r
-000077f0: 6573 756c 7427 7320 7374 646f 7574 0a20  esult's stdout. 
-00007800: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00007810: 2020 2020 2020 2020 6c61 7465 7374 5f70          latest_p
-00007820: 726f 6772 6573 7320 3d20 7265 2e66 696e  rogress = re.fin
-00007830: 6461 6c6c 280a 2020 2020 2020 2020 2020  dall(.          
-00007840: 2020 2020 2020 7061 7474 6572 6e2c 2072        pattern, r
-00007850: 6573 756c 742e 7374 646f 7574 295b 2d31  esult.stdout)[-1
-00007860: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
-00007870: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00007880: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00007890: 6765 722e 6572 726f 7228 6622 4973 7375  ger.error(f"Issu
-000078a0: 6520 7769 7468 2065 7874 7261 6374 696e  e with extractin
-000078b0: 6720 7072 6f67 7265 7373 3a20 7b65 7d22  g progress: {e}"
-000078c0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000078d0: 6e20 6622 5072 6f67 7265 7373 3a20 7b6c  n f"Progress: {l
-000078e0: 6174 6573 745f 7072 6f67 7265 7373 7d5c  atest_progress}\
-000078f0: 6e22 0a0a 2020 2020 6465 6620 7275 6e5f  n"..    def run_
-00007900: 636f 6d6d 616e 6473 2873 656c 662c 2063  commands(self, c
-00007910: 6d64 6c69 7374 3a20 4c69 7374 5b73 7472  mdlist: List[str
-00007920: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00007930: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
-00007940: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00007950: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 2073 6570 3a20 7374 7220 3d20 2720     sep: str = ' 
-00007980: 2626 2027 2c0a 2020 2020 2020 2020 2020  && ',.          
-00007990: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-000079a0: 7267 7329 202d 3e20 5265 7375 6c74 3a0a  rgs) -> Result:.
-000079b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000079c0: 2020 2020 5275 6e20 6120 6c69 7374 206f      Run a list o
-000079d0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
-000079e0: 2063 6f6e 7365 6375 7469 7665 6c79 206f   consecutively o
-000079f0: 6e20 7468 6520 536c 7572 6d20 636c 7573  n the Slurm clus
-00007a00: 7465 722c 0a20 2020 2020 2020 2065 6e73  ter,.        ens
-00007a10: 7572 696e 6720 7468 6520 7375 6363 6573  uring the succes
-00007a20: 7320 6f66 2065 6163 6820 6265 666f 7265  s of each before
-00007a30: 2070 726f 6365 6564 696e 6720 746f 2074   proceeding to t
-00007a40: 6865 206e 6578 742e 0a0a 2020 2020 2020  he next...      
-00007a50: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
-00007a60: 7420 7661 7269 6162 6c65 7320 6361 6e20  t variables can 
-00007a70: 6265 2073 6574 2075 7369 6e67 2074 6865  be set using the
-00007a80: 2060 656e 7660 2061 7267 756d 656e 742e   `env` argument.
-00007a90: 0a20 2020 2020 2020 2054 6865 7365 2063  .        These c
-00007aa0: 6f6d 6d61 6e64 7320 7265 7461 696e 2074  ommands retain t
-00007ab0: 6865 2073 616d 6520 7365 7373 696f 6e20  he same session 
-00007ac0: 2865 6e76 6972 6f6e 6d65 6e74 2076 6172  (environment var
-00007ad0: 6961 626c 6573 0a20 2020 2020 2020 2065  iables.        e
-00007ae0: 7463 2e29 2c20 756e 6c69 6b65 2072 756e  tc.), unlike run
-00007af0: 6e69 6e67 2074 6865 6d20 7365 7061 7261  ning them separa
-00007b00: 7465 6c79 2e0a 0a20 2020 2020 2020 2041  tely...        A
-00007b10: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00007b20: 2063 6d64 6c69 7374 2028 4c69 7374 5b73   cmdlist (List[s
-00007b30: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
-00007b40: 7368 656c 6c20 636f 6d6d 616e 6473 2074  shell commands t
-00007b50: 6f20 7275 6e20 6f6e 2053 6c75 726d 2e0a  o run on Slurm..
-00007b60: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00007b70: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
-00007b80: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
-00007b90: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
-00007ba0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007bc0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-00007bd0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-00007be0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00007bf0: 2020 2020 2020 2020 2020 7365 7020 2873            sep (s
-00007c00: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-00007c10: 6865 2073 6570 6172 6174 6f72 2075 7365  he separator use
-00007c20: 6420 746f 2063 6f6e 6361 7465 6e61 7465  d to concatenate
-00007c30: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
-00007c40: 2020 2020 2020 636f 6d6d 616e 6473 2e20        commands. 
-00007c50: 4465 6661 756c 7473 2074 6f20 2720 2626  Defaults to ' &&
-00007c60: 2027 2e0a 2020 2020 2020 2020 2020 2020   '..            
-00007c70: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
-00007c80: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
-00007c90: 756d 656e 7473 2e0a 0a20 2020 2020 2020  uments...       
-00007ca0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00007cb0: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
-00007cc0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
-00007cd0: 6c61 7374 2063 6f6d 6d61 6e64 2069 6e20  last command in 
-00007ce0: 7468 6520 6c69 7374 2e0a 2020 2020 2020  the list..      
-00007cf0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00007d00: 2065 6e76 2069 7320 4e6f 6e65 3a0a 2020   env is None:.  
-00007d10: 2020 2020 2020 2020 2020 656e 7620 3d20            env = 
-00007d20: 7b7d 0a20 2020 2020 2020 2063 6d64 203d  {}.        cmd =
-00007d30: 2073 6570 2e6a 6f69 6e28 636d 646c 6973   sep.join(cmdlis
-00007d40: 7429 0a20 2020 2020 2020 206c 6f67 6765  t).        logge
-00007d50: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-00007d60: 2020 2020 6622 5275 6e6e 696e 6720 636f      f"Running co
-00007d70: 6d6d 616e 6473 2c20 7769 7468 2065 6e76  mmands, with env
-00007d80: 207b 656e 767d 2061 6e64 2073 6570 207b   {env} and sep {
-00007d90: 7365 707d 205c 0a20 2020 2020 2020 2020  sep} \.         
-00007da0: 2020 2020 2020 2061 6e64 207b 6b77 6172         and {kwar
-00007db0: 6773 7d3a 207b 636d 647d 2229 0a20 2020  gs}: {cmd}").   
-00007dc0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00007dd0: 6c66 2e72 756e 2863 6d64 2c20 656e 763d  lf.run(cmd, env=
-00007de0: 656e 762c 202a 2a6b 7761 7267 7329 2020  env, **kwargs)  
-00007df0: 2320 6f75 745f 7374 7265 616d 3d6f 7574  # out_stream=out
-00007e00: 5f73 7472 6561 6d2c 0a0a 2020 2020 2020  _stream,..      
-00007e10: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00007e20: 2020 2023 2057 6174 6368 206f 7574 2066     # Watch out f
-00007e30: 6f72 2055 6e69 636f 6465 456e 636f 6465  or UnicodeEncode
-00007e40: 4572 726f 7220 7768 656e 2079 6f75 2073  Error when you s
-00007e50: 7472 2829 2074 6869 732e 0a20 2020 2020  tr() this..     
-00007e60: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00007e70: 666f 2866 227b 7265 7375 6c74 2e73 7464  fo(f"{result.std
-00007e80: 6f75 747d 2229 0a20 2020 2020 2020 2065  out}").        e
-00007e90: 7863 6570 7420 556e 6963 6f64 6545 6e63  xcept UnicodeEnc
-00007ea0: 6f64 6545 7272 6f72 2061 7320 653a 0a20  odeError as e:. 
-00007eb0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00007ec0: 722e 6572 726f 7228 6622 556e 6963 6f64  r.error(f"Unicod
-00007ed0: 6520 6572 726f 723a 207b 657d 2229 0a20  e error: {e}"). 
-00007ee0: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00007ef0: 4f3a 204f 4e4c 5920 7374 646f 7574 2052  O: ONLY stdout R
-00007f00: 4543 4f44 4520 4e45 4544 4544 3f3f 206f  ECODE NEEDED?? o
-00007f10: 7220 616c 736f 2065 7272 6f72 3f0a 2020  r also error?.  
-00007f20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00007f30: 2e73 7464 6f75 7420 3d20 7265 7375 6c74  .stdout = result
-00007f40: 2e73 7464 6f75 742e 656e 636f 6465 280a  .stdout.encode(.
-00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 2775 7466 2d38 272c 2027 6967 6e6f 7265  'utf-8', 'ignore
-00007f70: 2729 2e64 6563 6f64 6528 2775 7466 2d38  ').decode('utf-8
-00007f80: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00007f90: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00007fa0: 6620 7374 725f 746f 5f63 6c61 7373 2873  f str_to_class(s
-00007fb0: 656c 662c 206d 6f64 756c 655f 6e61 6d65  elf, module_name
-00007fc0: 3a20 7374 722c 2063 6c61 7373 5f6e 616d  : str, class_nam
-00007fd0: 653a 2073 7472 2c20 2a61 7267 732c 202a  e: str, *args, *
-00007fe0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00007ff0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00008000: 7475 726e 2061 2063 6c61 7373 2069 6e73  turn a class ins
-00008010: 7461 6e63 6520 6672 6f6d 2061 2073 7472  tance from a str
-00008020: 696e 6720 7265 6665 7265 6e63 652e 0a0a  ing reference...
-00008030: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00008040: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
-00008050: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
-00008060: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-00008070: 756c 652e 0a20 2020 2020 2020 2020 2020  ule..           
-00008080: 2063 6c61 7373 5f6e 616d 6520 2873 7472   class_name (str
-00008090: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
-000080a0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
-000080b0: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
-000080c0: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
-000080d0: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
-000080e0: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
-000080f0: 7275 6374 6f72 2e0a 2020 2020 2020 2020  ructor..        
-00008100: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
-00008110: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
-00008120: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-00008130: 6865 2063 6c61 7373 2063 6f6e 7374 7275  he class constru
-00008140: 6374 6f72 2e0a 0a20 2020 2020 2020 2052  ctor...        R
-00008150: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00008160: 2020 2020 6f62 6a65 6374 3a20 416e 2069      object: An i
-00008170: 6e73 7461 6e63 6520 6f66 2074 6865 2073  nstance of the s
-00008180: 7065 6369 6669 6564 2063 6c61 7373 2c20  pecified class, 
-00008190: 6f72 204e 6f6e 6520 6966 2074 6865 2063  or None if the c
-000081a0: 6c61 7373 206f 720a 2020 2020 2020 2020  lass or.        
-000081b0: 2020 2020 2020 2020 6d6f 6475 6c65 2064          module d
-000081c0: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
-000081d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000081e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000081f0: 2020 2020 6d6f 6475 6c65 5f20 3d20 696d      module_ = im
-00008200: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
-00008210: 6f64 756c 6528 6d6f 6475 6c65 5f6e 616d  odule(module_nam
-00008220: 6529 0a20 2020 2020 2020 2020 2020 2074  e).            t
-00008230: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00008240: 2020 2020 636c 6173 735f 203d 2067 6574      class_ = get
-00008250: 6174 7472 286d 6f64 756c 655f 2c20 636c  attr(module_, cl
-00008260: 6173 735f 6e61 6d65 2928 2a61 7267 732c  ass_name)(*args,
-00008270: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-00008280: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-00008290: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
-000082a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000082b0: 6767 6572 2e65 7272 6f72 2827 436c 6173  gger.error('Clas
-000082c0: 7320 646f 6573 206e 6f74 2065 7869 7374  s does not exist
-000082d0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
-000082e0: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-000082f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00008300: 722e 6572 726f 7228 274d 6f64 756c 6520  r.error('Module 
-00008310: 646f 6573 206e 6f74 2065 7869 7374 2729  does not exist')
-00008320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008330: 636c 6173 735f 206f 7220 4e6f 6e65 0a0a  class_ or None..
-00008340: 2020 2020 6465 6620 7275 6e5f 636f 6d6d      def run_comm
-00008350: 616e 6473 5f73 706c 6974 5f6f 7574 2873  ands_split_out(s
-00008360: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 636d 646c 6973 743a 204c 6973      cmdlist: Lis
-00008390: 745b 7374 725d 2c0a 2020 2020 2020 2020  t[str],.        
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-000083c0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-000083d0: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
-000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00008400: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-00008410: 2020 2022 2222 5275 6e20 6120 6c69 7374     """Run a list
-00008420: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
-00008430: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
-00008440: 2061 6e64 2073 706c 6974 2074 6865 206f   and split the o
-00008450: 7574 7075 740a 2020 2020 2020 2020 6f66  utput.        of
-00008460: 2065 6163 6820 636f 6d6d 616e 642e 0a0a   each command...
-00008470: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
-00008480: 6d61 6e64 2069 6e20 7468 6520 6c69 7374  mand in the list
-00008490: 2069 7320 6578 6563 7574 6564 2077 6974   is executed wit
-000084a0: 6820 6120 7365 7061 7261 746f 7220 696e  h a separator in
-000084b0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
-000084c0: 2074 6861 7420 6973 2075 6e69 7175 6520   that is unique 
-000084d0: 616e 6420 6361 6e20 6265 2075 7365 6420  and can be used 
-000084e0: 746f 2073 706c 6974 0a20 2020 2020 2020  to split.       
-000084f0: 2074 6865 206f 7574 7075 7420 6f66 2065   the output of e
-00008500: 6163 6820 636f 6d6d 616e 6420 6c61 7465  ach command late
-00008510: 722e 2054 6865 2073 6570 6172 6174 6f72  r. The separator
-00008520: 2075 7365 6420 6973 2073 7065 6369 6669   used is specifi
-00008530: 6564 0a20 2020 2020 2020 2062 7920 7468  ed.        by th
-00008540: 6520 605f 4f55 545f 5345 5060 2061 7474  e `_OUT_SEP` att
-00008550: 7269 6275 7465 206f 6620 7468 650a 2020  ribute of the.  
-00008560: 2020 2020 2020 536c 7572 6d43 6c69 656e        SlurmClien
-00008570: 7420 696e 7374 616e 6365 2e0a 0a20 2020  t instance...   
-00008580: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00008590: 2020 2020 2020 2063 6d64 6c69 7374 2028         cmdlist (
-000085a0: 4c69 7374 5b73 7472 5d29 3a20 4120 6c69  List[str]): A li
-000085b0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
-000085c0: 616e 6473 2074 6f20 7275 6e2e 0a20 2020  ands to run..   
-000085d0: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-000085e0: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-000085f0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-00008600: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-00008610: 7269 6162 6c65 7320 0a20 2020 2020 2020  riables .       
-00008620: 2020 2020 2020 2020 2074 6f20 7365 7420           to set 
-00008630: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
-00008640: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
-00008650: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
-00008660: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00008670: 2020 2020 2020 2020 2020 4c69 7374 5b73            List[s
-00008680: 7472 5d3a 0a20 2020 2020 2020 2020 2020  tr]:.           
-00008690: 2020 2020 2041 206c 6973 7420 6f66 2073       A list of s
-000086a0: 7472 696e 6773 2c20 7768 6572 6520 6561  trings, where ea
-000086b0: 6368 2073 7472 696e 6720 636f 7272 6573  ch string corres
-000086c0: 706f 6e64 7320 746f 0a20 2020 2020 2020  ponds to.       
-000086d0: 2020 2020 2020 2020 2074 6865 206f 7574           the out
-000086e0: 7075 7420 6f66 2061 2073 696e 676c 6520  put of a single 
-000086f0: 636f 6d6d 616e 6420 696e 2060 636d 646c  command in `cmdl
-00008700: 6973 7460 2073 706c 6974 0a20 2020 2020  ist` split.     
-00008710: 2020 2020 2020 2020 2020 2062 7920 7468             by th
-00008720: 6520 7365 7061 7261 746f 7220 605f 4f55  e separator `_OU
-00008730: 545f 5345 5060 2e0a 0a20 2020 2020 2020  T_SEP`...       
-00008740: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00008750: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
-00008760: 6e3a 2049 6620 616e 7920 6f66 2074 6865  n: If any of the
-00008770: 2063 6f6d 6d61 6e64 7320 6661 696c 2074   commands fail t
-00008780: 6f20 6578 6563 7574 6520 7375 6363 6573  o execute succes
-00008790: 7366 756c 6c79 2e0a 2020 2020 2020 2020  sfully..        
-000087a0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
-000087b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000087c0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-000087d0: 6f6d 6d61 6e64 7328 636d 646c 6973 743d  ommands(cmdlist=
-000087e0: 636d 646c 6973 742c 0a20 2020 2020 2020  cmdlist,.       
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 656e 763d 656e 762c 0a20 2020 2020 2020  env=env,.       
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008840: 7365 703d 6622 203b 2065 6368 6f20 7b73  sep=f" ; echo {s
-00008850: 656c 662e 5f4f 5554 5f53 4550 7d20 3b20  elf._OUT_SEP} ; 
-00008860: 2229 0a20 2020 2020 2020 2065 7863 6570  ").        excep
-00008870: 7420 556e 6578 7065 6374 6564 4578 6974  t UnexpectedExit
-00008880: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00008890: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-000088a0: 6728 6529 0a20 2020 2020 2020 2020 2020  g(e).           
-000088b0: 2072 6573 756c 7420 3d20 652e 7265 7375   result = e.resu
-000088c0: 6c74 0a20 2020 2020 2020 2069 6620 7265  lt.        if re
-000088d0: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
-000088e0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-000088f0: 7265 7375 6c74 2e73 7464 6f75 740a 2020  result.stdout.  
-00008900: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
-00008910: 7265 7370 6f6e 7365 7320 3d20 7265 7370  responses = resp
-00008920: 6f6e 7365 2e73 706c 6974 2873 656c 662e  onse.split(self.
-00008930: 5f4f 5554 5f53 4550 290a 2020 2020 2020  _OUT_SEP).      
-00008940: 2020 2020 2020 7265 7475 726e 2073 706c        return spl
-00008950: 6974 5f72 6573 706f 6e73 6573 0a20 2020  it_responses.   
-00008960: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008970: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
-00008980: 7265 7375 6c74 2069 7320 6e6f 7420 6f6b  result is not ok
-00008990: 2c20 6c6f 6720 7468 6520 6572 726f 7220  , log the error 
-000089a0: 616e 6420 7261 6973 6520 616e 2053 5348  and raise an SSH
-000089b0: 4578 6365 7074 696f 6e0a 2020 2020 2020  Exception.      
-000089c0: 2020 2020 2020 6572 726f 7220 3d20 6622        error = f"
-000089d0: 5265 7375 6c74 2069 7320 6e6f 7420 6f6b  Result is not ok
-000089e0: 3a20 7b72 6573 756c 747d 220a 2020 2020  : {result}".    
-000089f0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00008a00: 7272 6f72 2865 7272 6f72 290a 2020 2020  rror(error).    
-00008a10: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
-00008a20: 4845 7863 6570 7469 6f6e 2865 7272 6f72  HException(error
-00008a30: 290a 0a20 2020 2064 6566 206c 6973 745f  )..    def list_
-00008a40: 6163 7469 7665 5f6a 6f62 7328 7365 6c66  active_jobs(self
-00008a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008a60: 2020 2020 2020 2020 2020 2065 6e76 3a20             env: 
-00008a70: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00008a80: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
-00008a90: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-00008aa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008ab0: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
-00008ac0: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
-00008ad0: 6d20 534c 5552 4d2e 0a0a 2020 2020 2020  m SLURM...      
-00008ae0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00008af0: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
-00008b00: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-00008b10: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
-00008b20: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00008b30: 6573 2074 6f20 0a20 2020 2020 2020 2020  es to .         
-00008b40: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
-00008b50: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00008b60: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-00008b70: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00008b80: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00008b90: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
-00008ba0: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
-00008bb0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00008bc0: 2020 2020 2020 2023 2063 6d64 203d 2073         # cmd = s
-00008bd0: 656c 662e 5f41 4354 4956 455f 4a4f 4253  elf._ACTIVE_JOBS
-00008be0: 5f43 4d44 0a20 2020 2020 2020 2063 6d64  _CMD.        cmd
-00008bf0: 203d 2073 656c 662e 6765 745f 6a6f 6273   = self.get_jobs
-00008c00: 5f69 6e66 6f5f 636f 6d6d 616e 6428 7374  _info_command(st
-00008c10: 6172 745f 7469 6d65 3d22 6e6f 7722 2c20  art_time="now", 
-00008c20: 7374 6174 6573 3d22 7222 290a 2020 2020  states="r").    
-00008c30: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00008c40: 2252 6574 7269 6576 696e 6720 6c69 7374  "Retrieving list
-00008c50: 206f 6620 6163 7469 7665 206a 6f62 7320   of active jobs 
-00008c60: 6672 6f6d 2053 6c75 726d 2229 0a20 2020  from Slurm").   
-00008c70: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00008c80: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-00008c90: 5b63 6d64 5d2c 2065 6e76 3d65 6e76 290a  [cmd], env=env).
-00008ca0: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
-00008cb0: 203d 2072 6573 756c 742e 7374 646f 7574   = result.stdout
-00008cc0: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
-00008cd0: 5c6e 2729 0a20 2020 2020 2020 206a 6f62  \n').        job
-00008ce0: 5f6c 6973 742e 7265 7665 7273 6528 290a  _list.reverse().
-00008cf0: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-00008d00: 6f62 5f6c 6973 740a 0a20 2020 2064 6566  ob_list..    def
-00008d10: 206c 6973 745f 636f 6d70 6c65 7465 645f   list_completed_
-00008d20: 6a6f 6273 2873 656c 662c 0a20 2020 2020  jobs(self,.     
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-00008d50: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-00008d60: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-00008d70: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-00008d80: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00008d90: 6574 2061 206c 6973 7420 6f66 2063 6f6d  et a list of com
-00008da0: 706c 6574 6564 206a 6f62 7320 6672 6f6d  pleted jobs from
-00008db0: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
-00008dc0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00008dd0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-00008de0: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-00008df0: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-00008e00: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00008e10: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
-00008e20: 2020 2020 2073 6574 2077 6865 6e20 7275       set when ru
-00008e30: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-00008e40: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
-00008e50: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
-00008e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00008e70: 2020 204c 6973 745b 7374 725d 3a20 4120     List[str]: A 
-00008e80: 6c69 7374 206f 6620 6a6f 6220 4944 732e  list of job IDs.
-00008e90: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00008ea0: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-00008eb0: 2e67 6574 5f6a 6f62 735f 696e 666f 5f63  .get_jobs_info_c
-00008ec0: 6f6d 6d61 6e64 2873 7461 7465 733d 2263  ommand(states="c
-00008ed0: 6422 290a 2020 2020 2020 2020 6c6f 6767  d").        logg
-00008ee0: 6572 2e69 6e66 6f28 2252 6574 7269 6576  er.info("Retriev
-00008ef0: 696e 6720 6120 6c69 7374 206f 6620 636f  ing a list of co
-00008f00: 6d70 6c65 7465 6420 6a6f 6273 2066 726f  mpleted jobs fro
-00008f10: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
-00008f20: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00008f30: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-00008f40: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-00008f50: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
-00008f60: 5b6a 6f62 2e73 7472 6970 2829 2066 6f72  [job.strip() for
-00008f70: 206a 6f62 2069 6e20 7265 7375 6c74 2e73   job in result.s
-00008f80: 7464 6f75 742e 7374 7269 7028 292e 7370  tdout.strip().sp
-00008f90: 6c69 7428 275c 6e27 295d 0a20 2020 2020  lit('\n')].     
-00008fa0: 2020 206a 6f62 5f6c 6973 742e 7265 7665     job_list.reve
-00008fb0: 7273 6528 290a 2020 2020 2020 2020 7265  rse().        re
-00008fc0: 7475 726e 206a 6f62 5f6c 6973 740a 0a20  turn job_list.. 
-00008fd0: 2020 2064 6566 206c 6973 745f 616c 6c5f     def list_all_
-00008fe0: 6a6f 6273 2873 656c 662c 2065 6e76 3a20  jobs(self, env: 
-00008ff0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00009000: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
-00009010: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-00009020: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009030: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
-00009040: 2061 6c6c 206a 6f62 7320 6672 6f6d 2053   all jobs from S
-00009050: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
-00009060: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00009070: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
-00009080: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00009090: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
-000090a0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-000090b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000090c0: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
-000090d0: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
-000090e0: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-000090f0: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
-00009100: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00009110: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
-00009120: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
-00009130: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00009140: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
-00009150: 6765 745f 6a6f 6273 5f69 6e66 6f5f 636f  get_jobs_info_co
-00009160: 6d6d 616e 6428 290a 2020 2020 2020 2020  mmand().        
-00009170: 6c6f 6767 6572 2e69 6e66 6f28 2252 6574  logger.info("Ret
-00009180: 7269 6576 696e 6720 6120 6c69 7374 206f  rieving a list o
-00009190: 6620 616c 6c20 6a6f 6273 2066 726f 6d20  f all jobs from 
-000091a0: 536c 7572 6d22 290a 2020 2020 2020 2020  Slurm").        
-000091b0: 7265 7375 6c74 203d 2073 656c 662e 7275  result = self.ru
-000091c0: 6e5f 636f 6d6d 616e 6473 285b 636d 645d  n_commands([cmd]
-000091d0: 2c20 656e 763d 656e 7629 0a20 2020 2020  , env=env).     
-000091e0: 2020 206a 6f62 5f6c 6973 7420 3d20 7265     job_list = re
-000091f0: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
-00009200: 7028 292e 7370 6c69 7428 275c 6e27 290a  p().split('\n').
-00009210: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
-00009220: 2e72 6576 6572 7365 2829 0a20 2020 2020  .reverse().     
-00009230: 2020 2072 6574 7572 6e20 6a6f 625f 6c69     return job_li
-00009240: 7374 0a0a 2020 2020 6465 6620 6765 745f  st..    def get_
-00009250: 6a6f 6273 5f69 6e66 6f5f 636f 6d6d 616e  jobs_info_comman
-00009260: 6428 7365 6c66 2c20 7374 6172 745f 7469  d(self, start_ti
-00009270: 6d65 3a20 7374 7220 3d20 2232 3032 332d  me: str = "2023-
-00009280: 3031 2d30 3122 2c0a 2020 2020 2020 2020  01-01",.        
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 2020 656e 645f 7469 6d65 3a20        end_time: 
-000092b0: 7374 7220 3d20 226e 6f77 222c 0a20 2020  str = "now",.   
-000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092d0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-000092e0: 6e73 3a20 7374 7220 3d20 224a 6f62 4964  ns: str = "JobId
-000092f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2073 7461 7465 733a 2073 7472 203d 2022   states: str = "
-00009320: 722c 6364 2c66 2c74 6f2c 7273 2c64 6c2c  r,cd,f,to,rs,dl,
-00009330: 6e66 2229 202d 3e20 7374 723a 0a20 2020  nf") -> str:.   
-00009340: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00009350: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
-00009360: 2074 6f20 7265 7472 6965 7665 2069 6e66   to retrieve inf
-00009370: 6f72 6d61 7469 6f6e 2061 626f 7574 206f  ormation about o
-00009380: 6c64 206a 6f62 732e 0a0a 2020 2020 2020  ld jobs...      
-00009390: 2020 5468 6520 636f 6d6d 616e 6420 7769    The command wi
-000093a0: 6c6c 2062 6520 666f 726d 6174 7465 6420  ll be formatted 
-000093b0: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
-000093c0: 6564 2073 7461 7274 2074 696d 652c 2077  ed start time, w
-000093d0: 6869 6368 2069 730a 2020 2020 2020 2020  hich is.        
-000093e0: 6578 7065 6374 6564 2074 6f20 6265 2069  expected to be i
-000093f0: 6e20 7468 6520 4953 4f20 666f 726d 6174  n the ISO format
-00009400: 2022 5959 5959 2d4d 4d2d 4444 222e 0a20   "YYYY-MM-DD".. 
-00009410: 2020 2020 2020 2054 6865 2063 6f6d 6d61         The comma
-00009420: 6e64 2077 696c 6c20 7573 6520 7468 6520  nd will use the 
-00009430: 2273 6163 6374 2220 746f 6f6c 2074 6f20  "sacct" tool to 
-00009440: 7175 6572 7920 7468 650a 2020 2020 2020  query the.      
-00009450: 2020 536c 7572 6d20 6163 636f 756e 7469    Slurm accounti
-00009460: 6e67 2064 6174 6162 6173 6520 666f 7220  ng database for 
-00009470: 6a6f 6273 2074 6861 7420 7374 6172 7465  jobs that starte
-00009480: 6420 6f6e 206f 7220 6166 7465 7220 7468  d on or after th
-00009490: 650a 2020 2020 2020 2020 7370 6563 6966  e.        specif
-000094a0: 6965 6420 7374 6172 7420 7469 6d65 2c20  ied start time, 
-000094b0: 616e 6420 7769 6c6c 206f 7574 7075 7420  and will output 
-000094c0: 6f6e 6c79 2074 6865 206a 6f62 2049 4473  only the job IDs
-000094d0: 2028 2d6f 204a 6f62 4964 290a 2020 2020   (-o JobId).    
-000094e0: 2020 2020 7769 7468 6f75 7420 6865 6164      without head
-000094f0: 6572 206f 7220 7472 6169 6c65 7220 6c69  er or trailer li
-00009500: 6e65 7320 282d 6e20 2d58 292e 0a0a 2020  nes (-n -X)...  
-00009510: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009520: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
-00009530: 6d65 2028 7374 7229 3a20 5468 6520 7374  me (str): The st
-00009540: 6172 7420 7469 6d65 2066 726f 6d20 7768  art time from wh
-00009550: 6963 6820 746f 2072 6574 7269 6576 6520  ich to retrieve 
-00009560: 6a6f 620a 2020 2020 2020 2020 2020 2020  job.            
-00009570: 2020 2020 696e 666f 726d 6174 696f 6e2e      information.
-00009580: 2044 6566 6175 6c74 7320 746f 2022 3230   Defaults to "20
-00009590: 3233 2d30 312d 3031 222e 0a20 2020 2020  23-01-01"..     
-000095a0: 2020 2020 2020 2065 6e64 5f74 696d 6520         end_time 
-000095b0: 2873 7472 293a 2054 6865 2065 6e64 2074  (str): The end t
-000095c0: 696d 6520 756e 7469 6c20 7768 6963 6820  ime until which 
-000095d0: 746f 2072 6574 7269 6576 6520 6a6f 620a  to retrieve job.
-000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095f0: 696e 666f 726d 6174 696f 6e2e 2044 6566  information. Def
-00009600: 6175 6c74 7320 746f 2022 6e6f 7722 2e0a  aults to "now"..
-00009610: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00009620: 6d6e 7320 2873 7472 293a 2054 6865 2063  mns (str): The c
-00009630: 6f6c 756d 6e73 2074 6f20 7265 7472 6965  olumns to retrie
-00009640: 7665 2066 726f 6d20 7468 6520 6a6f 6220  ve from the job 
-00009650: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-00009660: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00009670: 6175 6c74 7320 746f 2022 4a6f 6249 6422  aults to "JobId"
-00009680: 2e20 4974 2069 7320 636f 6d6d 6120 7365  . It is comma se
-00009690: 7061 7261 7465 642c 2065 2e67 2e20 224a  parated, e.g. "J
-000096a0: 6f62 4964 2c53 7461 7465 222e 0a20 2020  obId,State"..   
-000096b0: 2020 2020 2020 2020 2073 7461 7465 7320           states 
-000096c0: 2873 7472 293a 2054 6865 206a 6f62 2073  (str): The job s
-000096d0: 7461 7465 7320 746f 2069 6e63 6c75 6465  tates to include
-000096e0: 2069 6e20 7468 6520 7175 6572 792e 0a20   in the query.. 
-000096f0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00009700: 6566 6175 6c74 7320 746f 2022 722c 6364  efaults to "r,cd
-00009710: 2c66 2c74 6f2c 7273 2c64 6c2c 6e66 222e  ,f,to,rs,dl,nf".
-00009720: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00009730: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00009740: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
-00009750: 2020 2020 4120 7374 7269 6e67 2072 6570      A string rep
-00009760: 7265 7365 6e74 696e 6720 7468 6520 536c  resenting the Sl
-00009770: 7572 6d20 636f 6d6d 616e 6420 746f 2072  urm command to r
-00009780: 6574 7269 6576 650a 2020 2020 2020 2020  etrieve.        
-00009790: 2020 2020 2020 2020 696e 666f 726d 6174          informat
-000097a0: 696f 6e20 6162 6f75 7420 6f6c 6420 6a6f  ion about old jo
-000097b0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
-000097c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000097d0: 656c 662e 5f41 4c4c 5f4a 4f42 535f 434d  elf._ALL_JOBS_CM
-000097e0: 442e 666f 726d 6174 2873 7461 7274 5f74  D.format(start_t
-000097f0: 696d 653d 7374 6172 745f 7469 6d65 2c0a  ime=start_time,.
+00003180: 2020 2075 7365 722c 0a20 2020 2020 2020     user,.       
+00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031b0: 2020 2070 6f72 742c 0a20 2020 2020 2020     port,.       
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 2020 2063 6f6e 6669 672c 0a20 2020 2020     config,.     
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2020 2067 6174 6577 6179 2c0a 2020       gateway,.  
+00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 2020 2020 2020 2020 666f 7277 6172 645f          forward_
+00003250: 6167 656e 742c 0a20 2020 2020 2020 2020  agent,.         
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2063 6f6e 6e65 6374 5f74 696d 656f 7574   connect_timeout
+00003290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032b0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+000032c0: 6563 745f 6b77 6172 6773 2c0a 2020 2020  ect_kwargs,.    
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 2020 2020 696e 6c69 6e65 5f73 7368        inline_ssh
+00003300: 5f65 6e76 290a 2020 2020 2020 2020 7365  _env).        se
+00003310: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
+00003320: 7468 203d 2073 6c75 726d 5f64 6174 615f  th = slurm_data_
+00003330: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
+00003340: 662e 736c 7572 6d5f 696d 6167 6573 5f70  f.slurm_images_p
+00003350: 6174 6820 3d20 736c 7572 6d5f 696d 6167  ath = slurm_imag
+00003360: 6573 5f70 6174 680a 2020 2020 2020 2020  es_path.        
+00003370: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
+00003380: 7274 6572 735f 7061 7468 203d 2073 6c75  rters_path = slu
+00003390: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+000033a0: 7468 0a20 2020 2020 2020 2073 656c 662e  th.        self.
+000033b0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
+000033c0: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
+000033d0: 7061 7468 730a 2020 2020 2020 2020 7365  paths.        se
+000033e0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
+000033f0: 7061 7468 203d 2073 6c75 726d 5f73 6372  path = slurm_scr
+00003400: 6970 745f 7061 7468 0a20 2020 2020 2020  ipt_path.       
+00003410: 2073 656c 662e 736c 7572 6d5f 7363 7269   self.slurm_scri
+00003420: 7074 5f72 6570 6f20 3d20 736c 7572 6d5f  pt_repo = slurm_
+00003430: 7363 7269 7074 5f72 6570 6f0a 2020 2020  script_repo.    
+00003440: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
+00003450: 6f64 656c 5f72 6570 6f73 203d 2073 6c75  odel_repos = slu
+00003460: 726d 5f6d 6f64 656c 5f72 6570 6f73 0a20  rm_model_repos. 
+00003470: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
+00003480: 6d5f 6d6f 6465 6c5f 696d 6167 6573 203d  m_model_images =
+00003490: 2073 6c75 726d 5f6d 6f64 656c 5f69 6d61   slurm_model_ima
+000034a0: 6765 730a 2020 2020 2020 2020 7365 6c66  ges.        self
+000034b0: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
+000034c0: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
+000034d0: 6a6f 6273 0a20 2020 2020 2020 2073 656c  jobs.        sel
+000034e0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
+000034f0: 6273 5f70 6172 616d 7320 3d20 736c 7572  bs_params = slur
+00003500: 6d5f 6d6f 6465 6c5f 6a6f 6273 5f70 6172  m_model_jobs_par
+00003510: 616d 730a 0a20 2020 2020 2020 2023 2049  ams..        # I
+00003520: 6e69 7420 6361 6368 652e 204b 6565 7020  nit cache. Keep 
+00003530: 7265 7370 6f6e 7365 7320 666f 7220 3336  responses for 36
+00003540: 3020 7365 636f 6e64 730a 2020 2020 2020  0 seconds.      
+00003550: 2020 7365 6c66 2e63 6163 6865 203d 2072    self.cache = r
+00003560: 6571 7565 7374 735f 6361 6368 652e 6261  equests_cache.ba
+00003570: 636b 656e 6473 2e73 716c 6974 652e 5351  ckends.sqlite.SQ
+00003580: 4c69 7465 4361 6368 6528 0a20 2020 2020  LiteCache(.     
+00003590: 2020 2020 2020 2064 625f 7061 7468 3d22         db_path="
+000035a0: 6769 7468 7562 5f63 6163 6865 222c 2075  github_cache", u
+000035b0: 7365 5f74 656d 703d 5472 7565 290a 2020  se_temp=True).  
+000035c0: 2020 2020 2020 7365 6c66 2e67 6574 5f6f        self.get_o
+000035d0: 725f 6372 6561 7465 5f67 6974 6875 625f  r_create_github_
+000035e0: 7365 7373 696f 6e28 290a 0a20 2020 2020  session()..     
+000035f0: 2020 2073 656c 662e 696e 6974 5f77 6f72     self.init_wor
+00003600: 6b66 6c6f 7773 2829 0a20 2020 2020 2020  kflows().       
+00003610: 2073 656c 662e 7661 6c69 6461 7465 2876   self.validate(v
+00003620: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
+00003630: 7475 703d 696e 6974 5f73 6c75 726d 290a  tup=init_slurm).
+00003640: 0a20 2020 2064 6566 2069 6e69 745f 776f  .    def init_wo
+00003650: 726b 666c 6f77 7328 7365 6c66 2c20 666f  rkflows(self, fo
+00003660: 7263 655f 7570 6461 7465 3a20 626f 6f6c  rce_update: bool
+00003670: 203d 2046 616c 7365 293a 0a20 2020 2020   = False):.     
+00003680: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00003690: 6574 7269 6576 6573 2074 6865 2072 6571  etrieves the req
+000036a0: 7569 7265 6420 696e 666f 2066 6f72 2074  uired info for t
+000036b0: 6865 2063 6f6e 6669 6775 7265 6420 776f  he configured wo
+000036c0: 726b 666c 6f77 7320 6672 6f6d 2067 6974  rkflows from git
+000036d0: 6875 622e 0a20 2020 2020 2020 2049 7420  hub..        It 
+000036e0: 7769 6c6c 2066 696c 6c20 6073 6c75 726d  will fill `slurm
+000036f0: 5f6d 6f64 656c 5f69 6d61 6765 7360 2077  _model_images` w
+00003700: 6974 6820 646f 636b 6572 6875 6220 6c69  ith dockerhub li
+00003710: 6e6b 732e 0a0a 2020 2020 2020 2020 4172  nks...        Ar
+00003720: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00003730: 666f 7263 655f 7570 6461 7465 2028 626f  force_update (bo
+00003740: 6f6c 293a 2057 696c 6c20 6f76 6572 7772  ol): Will overwr
+00003750: 6974 6520 616c 7265 6164 7920 6769 7665  ite already give
+00003760: 6e20 7061 7468 730a 2020 2020 2020 2020  n paths.        
+00003770: 2020 2020 2020 2020 696e 2060 736c 7572          in `slur
+00003780: 6d5f 6d6f 6465 6c5f 696d 6167 6573 600a  m_model_images`.
+00003790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000037a0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000037b0: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
+000037c0: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+000037d0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+000037e0: 6c5f 696d 6167 6573 203d 207b 7d0a 2020  l_images = {}.  
+000037f0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00003800: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7265  f.slurm_model_re
+00003810: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
+00003820: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+00003830: 224e 6f20 776f 726b 666c 6f77 7320 636f  "No workflows co
+00003840: 6e66 6967 7572 6564 2122 290a 2020 2020  nfigured!").    
+00003850: 2020 2020 2020 2020 7365 6c66 2e73 6c75          self.slu
+00003860: 726d 5f6d 6f64 656c 5f72 6570 6f73 203d  rm_model_repos =
+00003870: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00003880: 2320 736b 6970 7320 7468 6520 7365 7475  # skips the setu
+00003890: 700a 2020 2020 2020 2020 666f 7220 776f  p.        for wo
+000038a0: 726b 666c 6f77 2069 6e20 7365 6c66 2e73  rkflow in self.s
+000038b0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
+000038c0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+000038d0: 2020 2020 2069 6620 776f 726b 666c 6f77       if workflow
+000038e0: 206e 6f74 2069 6e20 7365 6c66 2e73 6c75   not in self.slu
+000038f0: 726d 5f6d 6f64 656c 5f69 6d61 6765 7320  rm_model_images 
+00003900: 6f72 2066 6f72 6365 5f75 7064 6174 653a  or force_update:
+00003910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003920: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
+00003930: 203d 2073 656c 662e 7075 6c6c 5f64 6573   = self.pull_des
+00003940: 6372 6970 746f 725f 6672 6f6d 5f67 6974  criptor_from_git
+00003950: 6875 6228 776f 726b 666c 6f77 290a 2020  hub(workflow).  
+00003960: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00003970: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
+00003980: 2573 272c 2077 6f72 6b66 6c6f 772c 206a  %s', workflow, j
+00003990: 736f 6e5f 6465 7363 7269 7074 6f72 290a  son_descriptor).
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 696d 6167 6520 3d20 6a73 6f6e 5f64 6573  image = json_des
+000039c0: 6372 6970 746f 725b 2763 6f6e 7461 696e  criptor['contain
+000039d0: 6572 2d69 6d61 6765 275d 5b27 696d 6167  er-image']['imag
+000039e0: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+000039f0: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
+00003a00: 6f64 656c 5f69 6d61 6765 735b 776f 726b  odel_images[work
+00003a10: 666c 6f77 5d20 3d20 696d 6167 650a 0a20  flow] = image.. 
+00003a20: 2020 2064 6566 2073 6574 7570 5f73 6c75     def setup_slu
+00003a30: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
+00003a40: 2020 2222 220a 2020 2020 2020 2020 5661    """.        Va
+00003a50: 6c69 6461 7465 7320 6f72 2063 7265 6174  lidates or creat
+00003a60: 6573 2074 6865 2072 6571 7569 7265 6420  es the required 
+00003a70: 7365 7475 7020 6f6e 2074 6865 2053 6c75  setup on the Slu
+00003a80: 726d 2063 6c75 7374 6572 2e0a 0a20 2020  rm cluster...   
+00003a90: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+00003aa0: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
+00003ab0: 7074 696f 6e3a 2069 6620 6974 2063 616e  ption: if it can
+00003ac0: 6e6f 7420 636f 6e6e 6563 7420 746f 2053  not connect to S
+00003ad0: 6c75 726d 2c20 6f72 2072 756e 7320 696e  lurm, or runs in
+00003ae0: 746f 2061 6e20 6572 726f 720a 2020 2020  to an error.    
+00003af0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00003b00: 6966 2073 656c 662e 7661 6c69 6461 7465  if self.validate
+00003b10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00003b20: 2320 312e 2043 7265 6174 6520 6469 7265  # 1. Create dire
+00003b30: 6374 6f72 6965 730a 2020 2020 2020 2020  ctories.        
+00003b40: 2020 2020 7365 6c66 2e73 6574 7570 5f64      self.setup_d
+00003b50: 6972 6563 746f 7269 6573 2829 0a0a 2020  irectories()..  
+00003b60: 2020 2020 2020 2020 2020 2320 322e 2043            # 2. C
+00003b70: 6c6f 6e65 2067 6974 0a20 2020 2020 2020  lone git.       
+00003b80: 2020 2020 2073 656c 662e 7365 7475 705f       self.setup_
+00003b90: 6a6f 625f 7363 7269 7074 7328 290a 0a20  job_scripts().. 
+00003ba0: 2020 2020 2020 2020 2020 2023 2033 2e20             # 3. 
+00003bb0: 5365 7475 7020 636f 6e76 6572 7465 7273  Setup converters
+00003bc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003bd0: 662e 7365 7475 705f 636f 6e76 6572 7465  f.setup_converte
+00003be0: 7273 2829 0a0a 2020 2020 2020 2020 2020  rs()..          
+00003bf0: 2020 2320 342e 2044 6f77 6e6c 6f61 6420    # 4. Download 
+00003c00: 776f 726b 666c 6f77 2069 6d61 6765 730a  workflow images.
+00003c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003c20: 2e73 6574 7570 5f63 6f6e 7461 696e 6572  .setup_container
+00003c30: 5f69 6d61 6765 7328 290a 0a20 2020 2020  _images()..     
+00003c40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003c50: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00003c60: 6365 7074 696f 6e28 2246 6169 6c75 7265  ception("Failure
+00003c70: 2069 6e20 636f 6e6e 6563 7469 6e67 2074   in connecting t
+00003c80: 6f20 536c 7572 6d20 636c 7573 7465 7222  o Slurm cluster"
+00003c90: 290a 0a20 2020 2064 6566 2073 6574 7570  )..    def setup
+00003ca0: 5f63 6f6e 7461 696e 6572 5f69 6d61 6765  _container_image
+00003cb0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00003cc0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+00003cd0: 7320 7570 2063 6f6e 7461 696e 6572 2069  s up container i
+00003ce0: 6d61 6765 7320 666f 7220 536c 7572 6d20  mages for Slurm 
+00003cf0: 6f70 6572 6174 696f 6e73 2e0a 0a20 2020  operations...   
+00003d00: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00003d10: 6f6e 2063 7265 6174 6573 2073 7065 6369  on creates speci
+00003d20: 6669 6320 6469 7265 6374 6f72 6965 7320  fic directories 
+00003d30: 666f 7220 636f 6e74 6169 6e65 7220 696d  for container im
+00003d40: 6167 6573 2061 6e64 2070 756c 6c73 0a20  ages and pulls. 
+00003d50: 2020 2020 2020 206e 6563 6573 7361 7279         necessary
+00003d60: 2069 6d61 6765 7320 6672 6f6d 2044 6f63   images from Doc
+00003d70: 6b65 7220 7265 706f 7369 746f 7269 6573  ker repositories
+00003d80: 2e20 4974 2067 656e 6572 6174 6573 2061  . It generates a
+00003d90: 6e64 2065 7865 6375 7465 730a 2020 2020  nd executes.    
+00003da0: 2020 2020 6120 7363 7269 7074 2074 6f20      a script to 
+00003db0: 7075 6c6c 2069 6d61 6765 7320 616e 6420  pull images and 
+00003dc0: 636f 7069 6573 2069 7420 746f 2074 6865  copies it to the
+00003dd0: 2072 656d 6f74 6520 6c6f 6361 7469 6f6e   remote location
+00003de0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00003df0: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+00003e00: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
+00003e10: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
+00003e20: 6520 6578 6563 7574 696e 6720 636f 6d6d  e executing comm
+00003e30: 616e 6473 206f 7220 636f 7079 696e 6720  ands or copying 
+00003e40: 6669 6c65 732e 0a20 2020 2020 2020 2022  files..        "
+00003e50: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
+00003e60: 6174 6520 7370 6563 6966 6963 2077 6f72  ate specific wor
+00003e70: 6b66 6c6f 7720 6469 7273 0a20 2020 2020  kflow dirs.     
+00003e80: 2020 2077 6974 6820 7365 6c66 2e63 6428     with self.cd(
+00003e90: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
+00003ea0: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
+00003eb0: 2020 2020 2069 6620 7365 6c66 2e73 6c75       if self.slu
+00003ec0: 726d 5f6d 6f64 656c 5f70 6174 6873 3a0a  rm_model_paths:.
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ee0: 6d6f 6465 6c70 6174 6873 203d 2022 2022  modelpaths = " "
+00003ef0: 2e6a 6f69 6e28 7365 6c66 2e73 6c75 726d  .join(self.slurm
+00003f00: 5f6d 6f64 656c 5f70 6174 6873 2e76 616c  _model_paths.val
+00003f10: 7565 7328 2929 0a20 2020 2020 2020 2020  ues()).         
+00003f20: 2020 2020 2020 2023 206d 6b64 6972 2063         # mkdir c
+00003f30: 656c 6c70 726f 6669 6c65 7220 696d 6167  ellprofiler imag
+00003f40: 656a 202e 2e2e 0a20 2020 2020 2020 2020  ej ....         
+00003f50: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
+00003f60: 7275 6e5f 636f 6d6d 616e 6473 285b 6622  run_commands([f"
+00003f70: 6d6b 6469 7220 2d70 207b 6d6f 6465 6c70  mkdir -p {modelp
+00003f80: 6174 6873 7d22 5d29 0a20 2020 2020 2020  aths}"]).       
+00003f90: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00003fa0: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
+00003fb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00003fc0: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+00003fd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003fe0: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00003ff0: 5f69 6d61 6765 733a 0a20 2020 2020 2020  _images:.       
+00004000: 2020 2020 2020 2020 2070 756c 6c5f 636f           pull_co
+00004010: 6d6d 616e 6473 203d 205b 5d0a 2020 2020  mmands = [].    
+00004020: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00004030: 7766 2c20 696d 6167 6520 696e 2073 656c  wf, image in sel
+00004040: 662e 736c 7572 6d5f 6d6f 6465 6c5f 696d  f.slurm_model_im
+00004050: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 7265 706f 203d 2073 656c 662e 736c    repo = self.sl
+00004080: 7572 6d5f 6d6f 6465 6c5f 7265 706f 735b  urm_model_repos[
+00004090: 7766 5d0a 2020 2020 2020 2020 2020 2020  wf].            
+000040a0: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
+000040b0: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+000040c0: 7061 7468 735b 7766 5d0a 2020 2020 2020  paths[wf].      
+000040d0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
+000040e0: 2076 6572 7369 6f6e 203d 2073 656c 662e   version = self.
+000040f0: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
+00004100: 6f6d 5f75 726c 2872 6570 6f29 0a20 2020  om_url(repo).   
+00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004120: 2069 6620 7665 7273 696f 6e20 3d3d 2022   if version == "
+00004130: 6d61 7374 6572 223a 0a20 2020 2020 2020  master":.       
+00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004150: 2076 6572 7369 6f6e 203d 2022 6c61 7465   version = "late
+00004160: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
+00004170: 2020 2020 2020 2020 7075 6c6c 5f74 656d          pull_tem
+00004180: 706c 6174 6520 3d20 2265 6368 6f20 2773  plate = "echo 's
+00004190: 7461 7274 696e 6720 2470 6174 6820 2476  tarting $path $v
+000041a0: 6572 7369 6f6e 2720 3e3e 2073 696e 672e  ersion' >> sing.
+000041b0: 6c6f 675c 6e6e 6f68 7570 2073 6820 2d63  log\nnohup sh -c
+000041c0: 205c 2273 696e 6775 6c61 7269 7479 2070   \"singularity p
+000041d0: 756c 6c20 2d2d 6469 7361 626c 652d 6361  ull --disable-ca
+000041e0: 6368 6520 2d2d 6469 7220 2470 6174 6820  che --dir $path 
+000041f0: 646f 636b 6572 3a2f 2f24 696d 6167 653a  docker://$image:
+00004200: 2476 6572 7369 6f6e 3b20 6563 686f 2027  $version; echo '
+00004210: 6669 6e69 7368 6564 2024 7061 7468 2024  finished $path $
+00004220: 7665 7273 696f 6e27 5c22 203e 3e20 7369  version'\" >> si
+00004230: 6e67 2e6c 6f67 2032 3e26 3120 2620 6469  ng.log 2>&1 & di
+00004240: 736f 776e 220a 2020 2020 2020 2020 2020  sown".          
+00004250: 2020 2020 2020 2020 2020 7420 3d20 5465            t = Te
+00004260: 6d70 6c61 7465 2870 756c 6c5f 7465 6d70  mplate(pull_temp
+00004270: 6c61 7465 290a 2020 2020 2020 2020 2020  late).          
+00004280: 2020 2020 2020 2020 2020 7375 6273 7469            substi
+00004290: 7475 7465 7320 3d20 7b7d 0a20 2020 2020  tutes = {}.     
+000042a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000042b0: 7562 7374 6974 7574 6573 5b27 7061 7468  ubstitutes['path
+000042c0: 275d 203d 2070 6174 680a 2020 2020 2020  '] = path.      
+000042d0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+000042e0: 6273 7469 7475 7465 735b 2769 6d61 6765  bstitutes['image
+000042f0: 275d 203d 2069 6d61 6765 0a20 2020 2020  '] = image.     
+00004300: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004310: 7562 7374 6974 7574 6573 5b27 7665 7273  ubstitutes['vers
+00004320: 696f 6e27 5d20 3d20 7665 7273 696f 6e0a  ion'] = version.
+00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004340: 2020 2020 636d 6420 3d20 742e 7361 6665      cmd = t.safe
+00004350: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+00004360: 7469 7475 7465 7329 0a20 2020 2020 2020  titutes).       
+00004370: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00004380: 6765 722e 6465 6275 6728 6622 7375 6273  ger.debug(f"subs
+00004390: 7469 7475 7465 643a 207b 636d 647d 2229  tituted: {cmd}")
+000043a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000043b0: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
+000043c0: 6473 2e61 7070 656e 6428 636d 6429 0a20  ds.append(cmd). 
+000043d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000043e0: 6372 6970 745f 6e61 6d65 203d 2022 7075  cript_name = "pu
+000043f0: 6c6c 5f69 6d61 6765 732e 7368 220a 2020  ll_images.sh".  
+00004400: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00004410: 6d70 6c61 7465 5f73 6372 6970 7420 3d20  mplate_script = 
+00004420: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+00004430: 2229 2e6a 6f69 6e70 6174 6828 7363 7269  ").joinpath(scri
+00004440: 7074 5f6e 616d 6529 0a20 2020 2020 2020  pt_name).       
+00004450: 2020 2020 2020 2020 2077 6974 6820 7465           with te
+00004460: 6d70 6c61 7465 5f73 6372 6970 742e 6f70  mplate_script.op
+00004470: 656e 2827 7227 2920 6173 2066 3a0a 2020  en('r') as f:.  
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 2020 7372 6320 3d20 5465 6d70 6c61 7465    src = Template
+000044a0: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000044c0: 7562 7374 6974 7574 6520 3d20 7b27 7075  ubstitute = {'pu
+000044d0: 6c6c 636f 6d6d 616e 6473 273a 2022 5c6e  llcommands': "\n
+000044e0: 222e 6a6f 696e 2870 756c 6c5f 636f 6d6d  ".join(pull_comm
+000044f0: 616e 6473 297d 0a20 2020 2020 2020 2020  ands)}.         
+00004500: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
+00004510: 6372 6970 7420 3d20 7372 632e 7361 6665  cript = src.safe
+00004520: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+00004530: 7469 7475 7465 290a 2020 2020 2020 2020  titute).        
+00004540: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00004550: 6562 7567 2866 2273 7562 7374 6974 7574  ebug(f"substitut
+00004560: 6564 3a5c 6e20 7b6a 6f62 5f73 6372 6970  ed:\n {job_scrip
+00004570: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
+00004580: 2020 2020 2023 2063 6f70 7920 746f 2072       # copy to r
+00004590: 656d 6f74 6520 6669 6c65 0a20 2020 2020  emote file.     
+000045a0: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+000045b0: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
+000045c0: 6d5f 696d 6167 6573 5f70 6174 682b 222f  m_images_path+"/
+000045d0: 222b 7363 7269 7074 5f6e 616d 650a 2020  "+script_name.  
+000045e0: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
+000045f0: 3d20 7365 6c66 2e70 7574 286c 6f63 616c  = self.put(local
+00004600: 3d69 6f2e 5374 7269 6e67 494f 286a 6f62  =io.StringIO(job
+00004610: 5f73 6372 6970 7429 2c0a 2020 2020 2020  _script),.      
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 2020 2072 656d 6f74 653d 6675         remote=fu
+00004640: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
+00004650: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+00004660: 2274 696d 6520 7368 207b 7363 7269 7074  "time sh {script
+00004670: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
+00004680: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+00004690: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
+000046a0: 6d64 5d29 0a20 2020 2020 2020 2020 2020  md]).           
+000046b0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
+000046c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000046d0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+000046e0: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
+000046f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00004700: 6572 2e69 6e66 6f28 722e 7374 646f 7574  er.info(r.stdout
+00004710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004720: 2020 6c6f 6767 6572 2e69 6e66 6f28 2249    logger.info("I
+00004730: 6e69 7469 6174 6564 2064 6f77 6e6c 6f61  nitiated downloa
+00004740: 6469 6e67 2061 6e64 2062 7569 6c64 696e  ding and buildin
+00004750: 6722 202b 0a20 2020 2020 2020 2020 2020  g" +.           
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2022 2063 6f6e 7461 696e 6572 2069 6d61   " container ima
+00004780: 6765 7320 6f6e 2053 6c75 726d 2e22 202b  ges on Slurm." +
+00004790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000047a0: 2020 2020 2020 2020 2020 2020 2022 2054               " T
+000047b0: 6869 7320 7769 6c6c 2074 616b 6520 6120  his will take a 
+000047c0: 7768 696c 6520 696e 2074 6865 2062 6163  while in the bac
+000047d0: 6b67 726f 756e 642e 2220 2b20 0a20 2020  kground." + .   
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 2020 2020 2020 2020 2022 2043 6865 636b           " Check
+00004800: 2027 7369 6e67 2e6c 6f67 2720 6f6e 2053   'sing.log' on S
+00004810: 6c75 726d 2066 6f72 2070 726f 6772 6573  lurm for progres
+00004820: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
+00004830: 2020 2020 2023 2023 2063 6c65 616e 7570       # # cleanup
+00004840: 2067 6961 6e74 2073 696e 6775 6c61 7269   giant singulari
+00004850: 7479 2063 6163 6865 210a 2020 2020 2020  ty cache!.      
+00004860: 2020 2020 2020 2020 2020 2320 7573 696e            # usin
+00004870: 6720 2d2d 6469 7361 626c 652d 6361 6368  g --disable-cach
+00004880: 6520 6265 6361 7573 6520 7765 2072 756e  e because we run
+00004890: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
+000048a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+000048b0: 2020 2023 2063 6d64 203d 2022 7369 6e67     # cmd = "sing
+000048c0: 756c 6172 6974 7920 6361 6368 6520 636c  ularity cache cl
+000048d0: 6561 6e20 2d66 220a 2020 2020 2020 2020  ean -f".        
+000048e0: 2020 2020 2020 2020 2320 7220 3d20 7365          # r = se
+000048f0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00004900: 5b63 6d64 5d29 0a0a 2020 2020 6465 6620  [cmd])..    def 
+00004910: 7365 7475 705f 636f 6e76 6572 7465 7273  setup_converters
+00004920: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004930: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
+00004940: 2075 7020 636f 6e76 6572 7465 7273 2066   up converters f
+00004950: 6f72 2053 6c75 726d 206f 7065 7261 7469  or Slurm operati
+00004960: 6f6e 732e 0a0a 2020 2020 2020 2020 5468  ons...        Th
+00004970: 6973 2066 756e 6374 696f 6e20 6372 6561  is function crea
+00004980: 7465 7320 6e65 6365 7373 6172 7920 6469  tes necessary di
+00004990: 7265 6374 6f72 6965 7320 666f 7220 636f  rectories for co
+000049a0: 6e76 6572 7465 7273 2061 6e64 2063 6f70  nverters and cop
+000049b0: 6965 730a 2020 2020 2020 2020 636f 6e76  ies.        conv
+000049c0: 6572 7465 7220 7363 7269 7074 7320 616e  erter scripts an
+000049d0: 6420 6465 6669 6e69 7469 6f6e 7320 746f  d definitions to
+000049e0: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
+000049f0: 206c 6f63 6174 696f 6e73 2e20 4974 2061   locations. It a
+00004a00: 6c73 6f0a 2020 2020 2020 2020 6275 696c  lso.        buil
+00004a10: 6473 2053 696e 6775 6c61 7269 7479 2063  ds Singularity c
+00004a20: 6f6e 7461 696e 6572 7320 6672 6f6d 2074  ontainers from t
+00004a30: 6865 2070 726f 7669 6465 6420 6465 6669  he provided defi
+00004a40: 6e69 7469 6f6e 732e 0a0a 2020 2020 2020  nitions...      
+00004a50: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00004a60: 2020 2020 2020 5353 4845 7863 6570 7469        SSHExcepti
+00004a70: 6f6e 3a20 4966 2074 6865 7265 2069 7320  on: If there is 
+00004a80: 616e 2069 7373 7565 2065 7865 6375 7469  an issue executi
+00004a90: 6e67 2063 6f6d 6d61 6e64 7320 6f72 2063  ng commands or c
+00004aa0: 6f70 7969 6e67 2066 696c 6573 2e0a 2020  opying files..  
+00004ab0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004ac0: 2020 636f 6e76 6572 745f 636d 6473 203d    convert_cmds =
+00004ad0: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
+00004ae0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
+00004af0: 7465 7273 5f70 6174 683a 0a20 2020 2020  ters_path:.     
+00004b00: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
+00004b10: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+00004b20: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+00004b30: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
+00004b40: 687d 2229 0a20 2020 2020 2020 2072 203d  h}").        r =
+00004b50: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00004b60: 6473 2863 6f6e 7665 7274 5f63 6d64 7329  ds(convert_cmds)
+00004b70: 0a20 2020 2020 2020 2023 2063 6f70 7920  .        # copy 
+00004b80: 6765 6e65 7269 6320 6a6f 6220 6172 7261  generic job arra
+00004b90: 7920 7363 7269 7074 206f 7665 7220 746f  y script over to
+00004ba0: 2073 6c75 726d 0a20 2020 2020 2020 2063   slurm.        c
+00004bb0: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
+00004bc0: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
+00004bd0: 6365 7322 292e 6a6f 696e 7061 7468 280a  ces").joinpath(.
+00004be0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00004bf0: 7665 7274 5f6a 6f62 5f61 7272 6179 2e73  vert_job_array.s
+00004c00: 6822 290a 2020 2020 2020 2020 5f20 3d20  h").        _ = 
+00004c10: 7365 6c66 2e70 7574 286c 6f63 616c 3d63  self.put(local=c
+00004c20: 6f6e 7665 7274 5f6a 6f62 5f6c 6f63 616c  onvert_job_local
+00004c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004c40: 2020 2020 2020 2072 656d 6f74 653d 7365         remote=se
+00004c50: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
+00004c60: 7061 7468 290a 2020 2020 2020 2020 2320  path).        # 
+00004c70: 6375 7272 656e 746c 7920 6b6e 6f77 6e20  currently known 
+00004c80: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
+00004c90: 2020 2023 2033 612e 205a 4152 5220 746f     # 3a. ZARR to
+00004ca0: 2054 4946 460a 2020 2020 2020 2020 2320   TIFF.        # 
+00004cb0: 544f 444f 2065 7874 7261 6374 2074 6865  TODO extract the
+00004cc0: 7365 2076 616c 7565 7320 746f 2065 2e67  se values to e.g
+00004cd0: 2e20 636f 6e66 6967 2069 6620 7765 2068  . config if we h
+00004ce0: 6176 6520 6d6f 7265 0a20 2020 2020 2020  ave more.       
+00004cf0: 2063 6f6e 7665 7274 5f6e 616d 6520 3d20   convert_name = 
+00004d00: 2263 6f6e 7665 7274 5f7a 6172 725f 746f  "convert_zarr_to
+00004d10: 5f74 6966 6622 0a20 2020 2020 2020 2063  _tiff".        c
+00004d20: 6f6e 7665 7274 5f70 7920 3d20 6622 7b63  onvert_py = f"{c
+00004d30: 6f6e 7665 7274 5f6e 616d 657d 2e70 7922  onvert_name}.py"
+00004d40: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
+00004d50: 5f73 6372 6970 745f 6c6f 6361 6c20 3d20  _script_local = 
+00004d60: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+00004d70: 2229 2e6a 6f69 6e70 6174 6828 0a20 2020  ").joinpath(.   
+00004d80: 2020 2020 2020 2020 2063 6f6e 7665 7274           convert
+00004d90: 5f70 7929 0a20 2020 2020 2020 2063 6f6e  _py).        con
+00004da0: 7665 7274 5f64 6566 203d 2066 227b 636f  vert_def = f"{co
+00004db0: 6e76 6572 745f 6e61 6d65 7d2e 6465 6622  nvert_name}.def"
+00004dc0: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
+00004dd0: 5f64 6566 5f6c 6f63 616c 203d 2066 696c  _def_local = fil
+00004de0: 6573 2822 7265 736f 7572 6365 7322 292e  es("resources").
+00004df0: 6a6f 696e 7061 7468 280a 2020 2020 2020  joinpath(.      
+00004e00: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
+00004e10: 6629 0a20 2020 2020 2020 205f 203d 2073  f).        _ = s
+00004e20: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
+00004e30: 6e76 6572 745f 7363 7269 7074 5f6c 6f63  nvert_script_loc
+00004e40: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
+00004e50: 2020 2020 2020 2020 2072 656d 6f74 653d           remote=
+00004e60: 7365 6c66 2e73 6c75 726d 5f63 6f6e 7665  self.slurm_conve
+00004e70: 7274 6572 735f 7061 7468 290a 2020 2020  rters_path).    
+00004e80: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
+00004e90: 286c 6f63 616c 3d63 6f6e 7665 7274 5f64  (local=convert_d
+00004ea0: 6566 5f6c 6f63 616c 2c0a 2020 2020 2020  ef_local,.      
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004ec0: 656d 6f74 653d 7365 6c66 2e73 6c75 726d  emote=self.slurm
+00004ed0: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
+00004ee0: 290a 2020 2020 2020 2020 2320 4275 696c  ).        # Buil
+00004ef0: 6420 7369 6e67 756c 6172 6974 7920 636f  d singularity co
+00004f00: 6e74 6169 6e65 7220 6672 6f6d 2064 6566  ntainer from def
+00004f10: 696e 6974 696f 6e0a 2020 2020 2020 2020  inition.        
+00004f20: 7769 7468 2073 656c 662e 6364 2873 656c  with self.cd(sel
+00004f30: 662e 736c 7572 6d5f 636f 6e76 6572 7465  f.slurm_converte
+00004f40: 7273 5f70 6174 6829 3a0a 2020 2020 2020  rs_path):.      
+00004f50: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
+00004f60: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
+00004f70: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00004f80: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004fa0: 2054 4f44 4f20 4368 616e 6765 2074 6865   TODO Change the
+00004fb0: 2074 6d70 2064 6972 3f0a 2020 2020 2020   tmp dir?.      
+00004fc0: 2020 2020 2020 2020 2020 2320 6578 706f            # expo
+00004fd0: 7274 2053 494e 4755 4c41 5249 5459 5f54  rt SINGULARITY_T
+00004fe0: 4d50 4449 523d 7e2f 6d79 2d73 6372 6174  MPDIR=~/my-scrat
+00004ff0: 6368 2f74 6d70 3b0a 2020 2020 2020 2020  ch/tmp;.        
+00005000: 2020 2020 2020 2020 2320 6f6e 6c79 2069          # only i
+00005010: 6620 6669 6c65 2064 6f65 7320 6e6f 7420  f file does not 
+00005020: 6578 6973 7420 7965 740a 2020 2020 2020  exist yet.      
+00005030: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
+00005040: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
+00005050: 6622 5b20 2120 2d66 207b 636f 6e76 6572  f"[ ! -f {conver
+00005060: 745f 6e61 6d65 7d2e 7369 6620 5d22 290a  t_name}.sif ]").
+00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005080: 2320 4544 4954 202d 2d20 4e4f 2c20 7468  # EDIT -- NO, th
+00005090: 656e 2077 6520 6361 6e27 7420 7570 6461  en we can't upda
+000050a0: 7465 2120 466f 7263 6520 7265 6275 696c  te! Force rebuil
+000050b0: 6421 0a20 2020 2020 2020 2020 2020 2020  d!.             
+000050c0: 2020 2023 2064 6f77 6e6c 6f61 6420 2f62     # download /b
+000050d0: 7569 6c64 206e 6577 2063 6f6e 7461 696e  uild new contain
+000050e0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+000050f0: 2020 2063 6f6e 7665 7274 5f63 6d64 732e     convert_cmds.
+00005100: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+00005110: 2020 2020 2020 2020 2020 2020 6622 7369              f"si
+00005120: 6e67 756c 6172 6974 7920 6275 696c 6420  ngularity build 
+00005130: 2d46 207b 636f 6e76 6572 745f 6e61 6d65  -F {convert_name
+00005140: 7d2e 7369 6620 7b63 6f6e 7665 7274 5f64  }.sif {convert_d
+00005150: 6566 7d20 3e3e 2073 696e 672e 6c6f 6720  ef} >> sing.log 
+00005160: 323e 2631 203b 2065 6368 6f20 2766 696e  2>&1 ; echo 'fin
+00005170: 6973 6865 6420 7b63 6f6e 7665 7274 5f6e  ished {convert_n
+00005180: 616d 657d 2e73 6966 2720 2622 290a 2020  ame}.sif' &").  
+00005190: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
+000051a0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+000051b0: 636f 6e76 6572 745f 636d 6473 290a 0a20  convert_cmds).. 
+000051c0: 2020 2064 6566 2073 6574 7570 5f6a 6f62     def setup_job
+000051d0: 5f73 6372 6970 7473 2873 656c 6629 3a0a  _scripts(self):.
+000051e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000051f0: 2020 2020 5365 7473 2075 7020 6a6f 6220      Sets up job 
+00005200: 7363 7269 7074 7320 666f 7220 536c 7572  scripts for Slur
+00005210: 6d20 6f70 6572 6174 696f 6e73 2e0a 0a20  m operations... 
+00005220: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
+00005230: 7469 6f6e 2065 6974 6865 7220 636c 6f6e  tion either clon
+00005240: 6573 2061 2047 6974 2072 6570 6f73 6974  es a Git reposit
+00005250: 6f72 7920 636f 6e74 6169 6e69 6e67 206a  ory containing j
+00005260: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
+00005270: 2020 2069 6e74 6f20 7468 6520 7370 6563     into the spec
+00005280: 6966 6965 6420 7363 7269 7074 2070 6174  ified script pat
+00005290: 6820 6f72 2067 656e 6572 6174 6573 2073  h or generates s
+000052a0: 6372 6970 7473 206c 6f63 616c 6c79 2069  cripts locally i
+000052b0: 6620 6e6f 2072 6570 6f73 6974 6f72 790a  f no repository.
+000052c0: 2020 2020 2020 2020 6973 2070 726f 7669          is provi
+000052d0: 6465 642e 0a0a 2020 2020 2020 2020 5261  ded...        Ra
+000052e0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+000052f0: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
+00005300: 4966 2074 6865 7265 2069 7320 616e 2069  If there is an i
+00005310: 7373 7565 2065 7865 6375 7469 6e67 2047  ssue executing G
+00005320: 6974 2063 6f6d 6d61 6e64 7320 6f72 2067  it commands or g
+00005330: 656e 6572 6174 696e 6720 7363 7269 7074  enerating script
+00005340: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00005350: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00005360: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+00005370: 2061 6e64 2073 656c 662e 736c 7572 6d5f   and self.slurm_
+00005380: 7363 7269 7074 5f70 6174 683a 0a20 2020  script_path:.   
+00005390: 2020 2020 2020 2020 2023 2067 6974 2063           # git c
+000053a0: 6c6f 6e65 2069 6e74 6f20 7363 7269 7074  lone into script
+000053b0: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
+000053c0: 2020 656e 7620 3d20 7b0a 2020 2020 2020    env = {.      
+000053d0: 2020 2020 2020 2020 2020 2252 4550 4f53            "REPOS
+000053e0: 5243 223a 2073 656c 662e 736c 7572 6d5f  RC": self.slurm_
+000053f0: 7363 7269 7074 5f72 6570 6f2c 0a20 2020  script_repo,.   
+00005400: 2020 2020 2020 2020 2020 2020 2022 4c4f               "LO
+00005410: 4341 4c52 4550 4f22 3a20 7365 6c66 2e73  CALREPO": self.s
+00005420: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
+00005430: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00005440: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00005450: 2027 6769 7420 636c 6f6e 6520 2224 5245   'git clone "$RE
+00005460: 504f 5352 4322 2022 244c 4f43 414c 5245  POSRC" "$LOCALRE
+00005470: 504f 2220 323e 202f 6465 762f 6e75 6c6c  PO" 2> /dev/null
+00005480: 207c 7c20 6769 7420 2d43 2022 244c 4f43   || git -C "$LOC
+00005490: 414c 5245 504f 2220 7075 6c6c 270a 2020  ALREPO" pull'.  
+000054a0: 2020 2020 2020 2020 2020 7220 3d20 7365            r = se
+000054b0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+000054c0: 5b63 6d64 5d2c 2065 6e76 290a 2020 2020  [cmd], env).    
+000054d0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+000054e0: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
+000054f0: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
+00005500: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
+00005510: 2020 2065 6c69 6620 7365 6c66 2e73 6c75     elif self.slu
+00005520: 726d 5f73 6372 6970 745f 7061 7468 3a0a  rm_script_path:.
+00005530: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+00005540: 6e65 7261 7465 2073 6372 6970 7473 0a20  nerate scripts. 
+00005550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005560: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
+00005570: 6970 7473 2867 656e 6572 6174 655f 6a6f  ipts(generate_jo
+00005580: 6273 3d54 7275 6529 0a0a 2020 2020 6465  bs=True)..    de
+00005590: 6620 7365 7475 705f 6469 7265 6374 6f72  f setup_director
+000055a0: 6965 7328 7365 6c66 293a 0a20 2020 2020  ies(self):.     
+000055b0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+000055c0: 7265 6174 6573 206e 6563 6573 7361 7279  reates necessary
+000055d0: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
+000055e0: 2053 6c75 726d 206f 7065 7261 7469 6f6e   Slurm operation
+000055f0: 732e 0a0a 2020 2020 2020 2020 5468 6973  s...        This
+00005600: 2066 756e 6374 696f 6e20 6372 6561 7465   function create
+00005610: 7320 6469 7265 6374 6f72 6965 7320 666f  s directories fo
+00005620: 7220 6461 7461 2073 746f 7261 6765 2c20  r data storage, 
+00005630: 7363 7269 7074 732c 2061 6e64 2077 6f72  scripts, and wor
+00005640: 6b66 6c6f 7773 0a20 2020 2020 2020 2061  kflows.        a
+00005650: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
+00005660: 6865 2053 6c75 726d 436c 6965 6e74 206f  he SlurmClient o
+00005670: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
+00005680: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00005690: 2020 2020 5353 4845 7863 6570 7469 6f6e      SSHException
+000056a0: 3a20 4966 2074 6865 7265 2069 7320 616e  : If there is an
+000056b0: 2069 7373 7565 2065 7865 6375 7469 6e67   issue executing
+000056c0: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
+000056d0: 696f 6e20 636f 6d6d 616e 6473 2e0a 2020  ion commands..  
+000056e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000056f0: 2020 6469 725f 636d 6473 203d 205b 5d0a    dir_cmds = [].
+00005700: 2020 2020 2020 2020 2320 612e 2064 6174          # a. dat
+00005710: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
+00005720: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
+00005730: 683a 0a20 2020 2020 2020 2020 2020 2064  h:.            d
+00005740: 6972 5f63 6d64 732e 6170 7065 6e64 2866  ir_cmds.append(f
+00005750: 226d 6b64 6972 202d 7020 7b73 656c 662e  "mkdir -p {self.
+00005760: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
+00005770: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
+00005780: 2062 2e20 7363 7269 7074 730a 2020 2020   b. scripts.    
+00005790: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+000057a0: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
+000057b0: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
+000057c0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+000057d0: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+000057e0: 6d5f 7363 7269 7074 5f70 6174 687d 2229  m_script_path}")
+000057f0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00005800: 2e20 776f 726b 666c 6f77 730a 2020 2020  . workflows.    
+00005810: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00005820: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
+00005830: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
+00005840: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+00005850: 6972 202d 7020 7b73 656c 662e 736c 7572  ir -p {self.slur
+00005860: 6d5f 696d 6167 6573 5f70 6174 687d 2229  m_images_path}")
+00005870: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
+00005880: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
+00005890: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
+000058a0: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
+000058b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000058c0: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+000058d0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+000058e0: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
+000058f0: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
+00005900: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
+00005910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005920: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
+00005930: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+00005940: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
+00005950: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+00005960: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
+00005970: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
+00005980: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
+00005990: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
+000059a0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+000059b0: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
+000059c0: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+000059d0: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
+000059e0: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
+000059f0: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
+00005a00: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
+00005a10: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
+00005a20: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
+00005a30: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
+00005a40: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
+00005a50: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
+00005a60: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
+00005a70: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
+00005a80: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
+00005a90: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
+00005aa0: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
+00005ab0: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
+00005ac0: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
+00005ad0: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
+00005ae0: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
+00005af0: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
+00005b00: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
+00005b10: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
+00005b20: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
+00005b30: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
+00005b40: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00005b50: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
+00005b60: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
+00005b70: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
+00005b80: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
+00005b90: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
+00005ba0: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
+00005bb0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00005bc0: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
+00005bd0: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
+00005be0: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
+00005bf0: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
+00005c00: 2020 2020 2020 2020 2020 2020 696e 6974              init
+00005c10: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
+00005c20: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
+00005c30: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
+00005c40: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
+00005c50: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
+00005c60: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
+00005c70: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
+00005c80: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
+00005c90: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
+00005ca0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00005cb0: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
+00005cc0: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
+00005cd0: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00005ce0: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
+00005cf0: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
+00005d00: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
+00005d10: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
+00005d20: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
+00005d30: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
+00005d40: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
+00005d50: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
+00005d60: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
+00005d70: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
+00005d80: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
+00005d90: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
+00005da0: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
+00005db0: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
+00005dc0: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
+00005df0: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
+00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
+00005e20: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
+00005e30: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
+00005e40: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
+00005e50: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00005e60: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
+00005e70: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
+00005e80: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
+00005e90: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
+00005ea0: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
+00005eb0: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
+00005ec0: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
+00005ed0: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
+00005ee0: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
+00005ef0: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
+00005f00: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
+00005f10: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
+00005f20: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
+00005f30: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
+00005f40: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
+00005f50: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
+00005f60: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
+00005f70: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
+00005f80: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
+00005f90: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
+00005fa0: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
+00005fb0: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+00005fc0: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+00005fd0: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
+00005fe0: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
+00005ff0: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
+00006000: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
+00006010: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+00006020: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+00006030: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
+00006040: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
+00006050: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
+00006060: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
+00006070: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
+00006080: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
+00006090: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
+000060a0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+000060b0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+000060c0: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
+000060d0: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
+000060e0: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
+000060f0: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
+00006100: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
+00006110: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
+00006120: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
+00006130: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
+00006140: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00006150: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
+00006160: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006170: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
+00006180: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006190: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
+000061a0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+000061b0: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
+000061c0: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
+000061d0: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
+000061e0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+000061f0: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
+00006200: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
+00006210: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
+00006220: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
+00006230: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00006240: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
+00006250: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
+00006260: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00006270: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
+00006280: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
+00006290: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
+000062a0: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
+000062b0: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
+000062c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000062d0: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
+000062e0: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
+000062f0: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
+00006300: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00006310: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
+00006320: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
+00006330: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006340: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
+00006350: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
+00006360: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
+00006370: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00006380: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
+00006390: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
+000063a0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+000063b0: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
+000063c0: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
+000063d0: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
+000063e0: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
+000063f0: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
+00006400: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006410: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00006420: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
+00006430: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
+00006440: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
+00006470: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
+00006480: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
+00006490: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
+000064a0: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
+000064b0: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
+000064c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000064d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000064e0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+000064f0: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
+00006500: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00006510: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
+00006520: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
+00006530: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
+00006540: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
+00006550: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
+00006560: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
+00006570: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
+00006580: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
+00006590: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
+000065a0: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
+000065b0: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+000065c0: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
+000065d0: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
+000065e0: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
+000065f0: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
+00006600: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00006610: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
+00006620: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+00006630: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
+00006640: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
+00006650: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
+00006660: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00006670: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
+000066a0: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
+000066b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066c0: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
+000066d0: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
+000066e0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+000066f0: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
+00006700: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
+00006710: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
+00006720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006730: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
+00006740: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
+00006750: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
+00006760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006770: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+00006780: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
+00006790: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
+000067a0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+000067b0: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
+000067c0: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
+000067d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000067e0: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
+000067f0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+00006800: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00006810: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
+00006820: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+00006850: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
+00006860: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
+00006870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006880: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00006890: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
+000068a0: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
+000068b0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+000068c0: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
+000068d0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+000068e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000068f0: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
+00006900: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
+00006910: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
+00006920: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
+00006950: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
+00006980: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00006990: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000069a0: 615f 6c6f 6361 7469 6f6e 3a20 7374 7220  a_location: str 
+000069b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
+000069e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2029 202d 3e20 5265 7375 6c74 3a0a 2020   ) -> Result:.  
+00006a10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006a20: 2020 436c 6561 6e75 7020 7a69 7020 616e    Cleanup zip an
+00006a30: 6420 756e 7a69 7070 6564 2066 696c 6573  d unzipped files
+00006a40: 2f66 6f6c 6465 7273 2061 7373 6f63 6961  /folders associa
+00006a50: 7465 6420 7769 7468 2061 2053 6c75 726d  ted with a Slurm
+00006a60: 206a 6f62 2e0a 0a20 2020 2020 2020 2041   job...        A
+00006a70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00006a80: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
+00006a90: 7472 293a 2054 6865 206a 6f62 2049 4420  tr): The job ID 
+00006aa0: 6f66 2074 6865 2053 6c75 726d 2073 6372  of the Slurm scr
+00006ab0: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
+00006ac0: 2066 696c 656e 616d 6520 2873 7472 293a   filename (str):
+00006ad0: 2054 6865 207a 6970 2066 696c 656e 616d   The zip filenam
+00006ae0: 6520 6f6e 2053 6c75 726d 2e0a 2020 2020  e on Slurm..    
+00006af0: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
+00006b00: 6174 696f 6e20 2873 7472 2c20 6f70 7469  ation (str, opti
+00006b10: 6f6e 616c 293a 2054 6865 206c 6f63 6174  onal): The locat
+00006b20: 696f 6e20 6f66 2064 6174 6120 6669 6c65  ion of data file
+00006b30: 7320 6f6e 2053 6c75 726d 2e0a 2020 2020  s on Slurm..    
+00006b40: 2020 2020 2020 2020 2020 2020 4966 206e              If n
+00006b50: 6f74 2070 726f 7669 6465 642c 2069 7420  ot provided, it 
+00006b60: 7769 6c6c 2062 6520 6578 7472 6163 7465  will be extracte
+00006b70: 6420 6672 6f6d 2074 6865 206c 6f67 2066  d from the log f
+00006b80: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
+00006b90: 206c 6f67 6669 6c65 2028 7374 722c 206f   logfile (str, o
+00006ba0: 7074 696f 6e61 6c29 3a20 5468 6520 6c6f  ptional): The lo
+00006bb0: 6720 6669 6c65 206f 6620 7468 6520 536c  g file of the Sl
+00006bc0: 7572 6d20 6a6f 622e 200a 2020 2020 2020  urm job. .      
+00006bd0: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
+00006be0: 2070 726f 7669 6465 642c 2061 2064 6566   provided, a def
+00006bf0: 6175 6c74 206c 6f67 2066 696c 6520 7769  ault log file wi
+00006c00: 6c6c 2062 6520 7573 6564 2e0a 0a20 2020  ll be used...   
+00006c10: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00006c20: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
+00006c30: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
+00006c40: 7468 6520 636c 6561 6e75 7020 6f70 6572  the cleanup oper
+00006c50: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00006c60: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
+00006c70: 2020 5468 6520 636c 6561 6e75 7020 7072    The cleanup pr
+00006c80: 6f63 6573 7320 696e 766f 6c76 6573 2072  ocess involves r
+00006c90: 656d 6f76 696e 6720 7468 6520 7370 6563  emoving the spec
+00006ca0: 6966 6965 6420 7a69 7020 6669 6c65 2c20  ified zip file, 
+00006cb0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00006cc0: 206c 6f67 2066 696c 652c 2061 6e64 2061   log file, and a
+00006cd0: 7373 6f63 6961 7465 6420 6461 7461 2066  ssociated data f
+00006ce0: 696c 6573 2061 6e64 2066 6f6c 6465 7273  iles and folders
+00006cf0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00006d00: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00006d10: 2320 436c 6561 6e75 7020 7465 6d70 6f72  # Cleanup tempor
+00006d20: 6172 7920 6669 6c65 7320 666f 7220 6120  ary files for a 
+00006d30: 536c 7572 6d20 6a6f 620a 2020 2020 2020  Slurm job.      
+00006d40: 2020 2020 2020 636c 6965 6e74 2e63 6c65        client.cle
+00006d50: 616e 7570 5f74 6d70 5f66 696c 6573 2822  anup_tmp_files("
+00006d60: 3132 3334 3522 2c20 226f 7574 7075 742e  12345", "output.
+00006d70: 7a69 7022 290a 2020 2020 2020 2020 2222  zip").        ""
+00006d80: 220a 2020 2020 2020 2020 636d 6473 203d  ".        cmds =
+00006d90: 205b 5d0a 2020 2020 2020 2020 2320 7a69   [].        # zi
+00006da0: 700a 2020 2020 2020 2020 726d 7a69 7020  p.        rmzip 
+00006db0: 3d20 6622 726d 207b 6669 6c65 6e61 6d65  = f"rm {filename
+00006dc0: 7d2e 2a22 0a20 2020 2020 2020 2063 6d64  }.*".        cmd
+00006dd0: 732e 6170 7065 6e64 2872 6d7a 6970 290a  s.append(rmzip).
+00006de0: 2020 2020 2020 2020 2320 6c6f 670a 2020          # log.  
+00006df0: 2020 2020 2020 6966 206c 6f67 6669 6c65        if logfile
+00006e00: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006e10: 2020 2020 2020 6c6f 6766 696c 6520 3d20        logfile = 
+00006e20: 7365 6c66 2e5f 4c4f 4746 494c 450a 2020  self._LOGFILE.  
+00006e30: 2020 2020 2020 2020 2020 6c6f 6766 696c            logfil
+00006e40: 6520 3d20 6c6f 6766 696c 652e 666f 726d  e = logfile.form
+00006e50: 6174 2873 6c75 726d 5f6a 6f62 5f69 643d  at(slurm_job_id=
+00006e60: 736c 7572 6d5f 6a6f 625f 6964 290a 2020  slurm_job_id).  
+00006e70: 2020 2020 2020 726d 6c6f 6720 3d20 6622        rmlog = f"
+00006e80: 726d 207b 6c6f 6766 696c 657d 220a 2020  rm {logfile}".  
+00006e90: 2020 2020 2020 636d 6473 2e61 7070 656e        cmds.appen
+00006ea0: 6428 726d 6c6f 6729 0a20 2020 2020 2020  d(rmlog).       
+00006eb0: 2023 2063 6f6e 7665 7274 6572 206c 6f67   # converter log
+00006ec0: 730a 2020 2020 2020 2020 636c 6f67 203d  s.        clog =
+00006ed0: 2073 656c 662e 5f43 4f4e 5645 5254 4552   self._CONVERTER
+00006ee0: 5f4c 4f47 4649 4c45 0a20 2020 2020 2020  _LOGFILE.       
+00006ef0: 2063 6c6f 6720 3d20 636c 6f67 2e66 6f72   clog = clog.for
+00006f00: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
+00006f10: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
+00006f20: 2020 2020 2020 2072 6d63 6c6f 6720 3d20         rmclog = 
+00006f30: 6622 726d 207b 636c 6f67 7d22 0a20 2020  f"rm {clog}".   
+00006f40: 2020 2020 2063 6d64 732e 6170 7065 6e64       cmds.append
+00006f50: 2872 6d63 6c6f 6729 0a20 2020 2020 2020  (rmclog).       
+00006f60: 2023 2064 6174 610a 2020 2020 2020 2020   # data.        
+00006f70: 6966 2064 6174 615f 6c6f 6361 7469 6f6e  if data_location
+00006f80: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006f90: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
+00006fa0: 696f 6e20 3d20 7365 6c66 2e65 7874 7261  ion = self.extra
+00006fb0: 6374 5f64 6174 615f 6c6f 6361 7469 6f6e  ct_data_location
+00006fc0: 5f66 726f 6d5f 6c6f 6728 6c6f 6766 696c  _from_log(logfil
+00006fd0: 6529 0a20 2020 2020 2020 2072 6d64 6174  e).        rmdat
+00006fe0: 6120 3d20 6622 726d 202d 7266 207b 6461  a = f"rm -rf {da
+00006ff0: 7461 5f6c 6f63 6174 696f 6e7d 207b 6461  ta_location} {da
+00007000: 7461 5f6c 6f63 6174 696f 6e7d 2e2a 220a  ta_location}.*".
+00007010: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
+00007020: 656e 6428 726d 6461 7461 290a 0a20 2020  end(rmdata)..   
+00007030: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00007040: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00007050: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+00007060: 2863 6d64 7329 0a20 2020 2020 2020 2065  (cmds).        e
+00007070: 7863 6570 7420 556e 6578 7065 6374 6564  xcept Unexpected
+00007080: 4578 6974 2061 7320 653a 0a20 2020 2020  Exit as e:.     
+00007090: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+000070a0: 726e 696e 6728 6529 0a20 2020 2020 2020  rning(e).       
+000070b0: 2020 2020 2072 6573 756c 7420 3d20 652e       result = e.
+000070c0: 7265 7375 6c74 0a20 2020 2020 2020 2072  result.        r
+000070d0: 6574 7572 6e20 7265 7375 6c74 206f 7220  eturn result or 
+000070e0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7661  None..    def va
+000070f0: 6c69 6461 7465 2873 656c 662c 2076 616c  lidate(self, val
+00007100: 6964 6174 655f 736c 7572 6d5f 7365 7475  idate_slurm_setu
+00007110: 703a 2062 6f6f 6c20 3d20 4661 6c73 6529  p: bool = False)
+00007120: 3a0a 2020 2020 2020 2020 2222 2256 616c  :.        """Val
+00007130: 6964 6174 6520 7468 6520 636f 6e6e 6563  idate the connec
+00007140: 7469 6f6e 2074 6f20 7468 6520 536c 7572  tion to the Slur
+00007150: 6d20 636c 7573 7465 7220 6279 2072 756e  m cluster by run
+00007160: 6e69 6e67 0a20 2020 2020 2020 2061 2073  ning.        a s
+00007170: 696d 706c 6520 636f 6d6d 616e 642e 0a0a  imple command...
+00007180: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00007190: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+000071a0: 7465 5f73 6c75 726d 5f73 6574 7570 2028  te_slurm_setup (
+000071b0: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+000071c0: 6f20 616c 736f 2063 6865 636b 0a20 2020  o also check.   
+000071d0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000071e0: 2066 6978 2074 6865 2053 6c75 726d 2073   fix the Slurm s
+000071f0: 6574 7570 2028 666f 6c64 6572 732c 2069  etup (folders, i
+00007200: 6d61 6765 732c 2065 7463 2e29 0a0a 2020  mages, etc.)..  
+00007210: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00007220: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
+00007230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007240: 2054 7275 6520 6966 2074 6865 2076 616c   True if the val
+00007250: 6964 6174 696f 6e20 6973 2073 7563 6365  idation is succe
+00007260: 7373 6675 6c2c 0a20 2020 2020 2020 2020  ssful,.         
+00007270: 2020 2020 2020 2046 616c 7365 206f 7468         False oth
+00007280: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
+00007290: 2222 220a 2020 2020 2020 2020 636f 6e6e  """.        conn
+000072a0: 6563 7465 6420 3d20 7365 6c66 2e72 756e  ected = self.run
+000072b0: 2827 6563 686f 2022 2022 2729 2e6f 6b0a  ('echo " "').ok.
+000072c0: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
+000072d0: 6374 6564 2061 6e64 2076 616c 6964 6174  cted and validat
+000072e0: 655f 736c 7572 6d5f 7365 7475 703a 0a20  e_slurm_setup:. 
+000072f0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 7365 6c66 2e73 6574 7570 5f73 6c75 726d  self.setup_slurm
+00007320: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
+00007330: 7863 6570 7420 5353 4845 7863 6570 7469  xcept SSHExcepti
+00007340: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00007350: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00007360: 6572 726f 7228 6529 0a20 2020 2020 2020  error(e).       
+00007370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007380: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
+00007390: 7475 726e 2063 6f6e 6e65 6374 6564 0a0a  turn connected..
+000073a0: 2020 2020 6465 6620 6765 745f 7265 6365      def get_rece
+000073b0: 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64 2873  nt_log_command(s
+000073c0: 656c 662c 206c 6f67 5f66 696c 653a 2073  elf, log_file: s
+000073d0: 7472 2c20 6e3a 2069 6e74 203d 2031 3029  tr, n: int = 10)
+000073e0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+000073f0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
+00007400: 2074 6865 2063 6f6d 6d61 6e64 2074 6f20   the command to 
+00007410: 7265 7472 6965 7665 2074 6865 2072 6563  retrieve the rec
+00007420: 656e 7420 6c6f 6720 656e 7472 6965 7320  ent log entries 
+00007430: 6672 6f6d 2061 0a20 2020 2020 2020 2073  from a.        s
+00007440: 7065 6369 6669 6564 206c 6f67 2066 696c  pecified log fil
+00007450: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+00007460: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00007470: 675f 6669 6c65 2028 7374 7229 3a20 5468  g_file (str): Th
+00007480: 6520 7061 7468 2074 6f20 7468 6520 6c6f  e path to the lo
+00007490: 6720 6669 6c65 2e0a 2020 2020 2020 2020  g file..        
+000074a0: 2020 2020 6e20 2869 6e74 2c20 6f70 7469      n (int, opti
+000074b0: 6f6e 616c 293a 2054 6865 206e 756d 6265  onal): The numbe
+000074c0: 7220 6f66 2072 6563 656e 7420 6c6f 6720  r of recent log 
+000074d0: 656e 7472 6965 7320 746f 2072 6574 7269  entries to retri
+000074e0: 6576 652e 0a20 2020 2020 2020 2020 2020  eve..           
+000074f0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00007500: 2031 302e 0a0a 2020 2020 2020 2020 5265   10...        Re
+00007510: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00007520: 2020 2073 7472 3a20 5468 6520 636f 6d6d     str: The comm
+00007530: 616e 6420 746f 2072 6574 7269 6576 6520  and to retrieve 
+00007540: 7468 6520 7265 6365 6e74 206c 6f67 2065  the recent log e
+00007550: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
+00007560: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00007570: 726e 2073 656c 662e 5f54 4149 4c5f 4c4f  rn self._TAIL_LO
+00007580: 475f 434d 442e 666f 726d 6174 286e 3d6e  G_CMD.format(n=n
+00007590: 2c20 6c6f 675f 6669 6c65 3d6c 6f67 5f66  , log_file=log_f
+000075a0: 696c 6529 0a0a 2020 2020 6465 6620 6765  ile)..    def ge
+000075b0: 745f 6163 7469 7665 5f6a 6f62 5f70 726f  t_active_job_pro
+000075c0: 6772 6573 7328 7365 6c66 2c0a 2020 2020  gress(self,.    
+000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075e0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+000075f0: 6d5f 6a6f 625f 6964 3a20 7374 722c 0a20  m_job_id: str,. 
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007620: 6174 7465 726e 3a20 7374 7220 3d20 7222  attern: str = r"
+00007630: 5c64 2b25 222c 0a20 2020 2020 2020 2020  \d+%",.         
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+00007660: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+00007670: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+00007680: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
+00007690: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+000076a0: 2070 726f 6772 6573 7320 6f66 2061 6e20   progress of an 
+000076b0: 6163 7469 7665 2053 6c75 726d 206a 6f62  active Slurm job
+000076c0: 2066 726f 6d20 6974 7320 6c6f 6766 696c   from its logfil
+000076d0: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
+000076e0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+000076f0: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
+00007700: 293a 2054 6865 2049 4420 6f66 2074 6865  ): The ID of the
+00007710: 2053 6c75 726d 206a 6f62 2e0a 2020 2020   Slurm job..    
+00007720: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
+00007730: 2873 7472 293a 2054 6865 2070 6174 7465  (str): The patte
+00007740: 726e 2074 6f20 6d61 7463 6820 696e 2074  rn to match in t
+00007750: 6865 206a 6f62 206c 6f67 2074 6f20 6578  he job log to ex
+00007760: 7472 6163 740a 2020 2020 2020 2020 2020  tract.          
+00007770: 2020 2020 2020 7468 6520 7072 6f67 7265        the progre
+00007780: 7373 2028 6465 6661 756c 743a 2072 225c  ss (default: r"\
+00007790: 642b 2522 292e 0a0a 2020 2020 2020 2020  d+%")...        
+000077a0: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
+000077b0: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
+000077c0: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
+000077d0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+000077e0: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
+000077f0: 2020 2020 746f 2073 6574 2077 6865 6e20      to set when 
+00007800: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+00007810: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
+00007820: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+00007830: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00007840: 2020 2020 2073 7472 3a20 5468 6520 7072       str: The pr
+00007850: 6f67 7265 7373 206f 6620 7468 6520 536c  ogress of the Sl
+00007860: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
+00007870: 2022 2222 0a20 2020 2020 2020 2063 6d64   """.        cmd
+00007880: 6c69 7374 203d 205b 5d0a 2020 2020 2020  list = [].      
+00007890: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
+000078a0: 5f72 6563 656e 745f 6c6f 675f 636f 6d6d  _recent_log_comm
+000078b0: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
+000078c0: 206c 6f67 5f66 696c 653d 7365 6c66 2e5f   log_file=self._
+000078d0: 4c4f 4746 494c 452e 666f 726d 6174 2873  LOGFILE.format(s
+000078e0: 6c75 726d 5f6a 6f62 5f69 643d 736c 7572  lurm_job_id=slur
+000078f0: 6d5f 6a6f 625f 6964 2929 0a20 2020 2020  m_job_id)).     
+00007900: 2020 2063 6d64 6c69 7374 2e61 7070 656e     cmdlist.appen
+00007910: 6428 636d 6429 0a20 2020 2020 2020 2069  d(cmd).        i
+00007920: 6620 656e 7620 6973 204e 6f6e 653a 0a20  f env is None:. 
+00007930: 2020 2020 2020 2020 2020 2065 6e76 203d             env =
+00007940: 207b 7d0a 2020 2020 2020 2020 7472 793a   {}.        try:
+00007950: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00007960: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+00007970: 6f6d 6d61 6e64 7328 636d 646c 6973 742c  ommands(cmdlist,
+00007980: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
+00007990: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+000079a0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+000079b0: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
+000079c0: 7228 6622 4973 7375 6520 7769 7468 2072  r(f"Issue with r
+000079d0: 756e 2063 6f6d 6d61 6e64 3a20 7b65 7d22  un command: {e}"
+000079e0: 290a 2020 2020 2020 2020 2320 4d61 7463  ).        # Matc
+000079f0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
+00007a00: 7061 7474 6572 6e20 696e 2074 6865 2072  pattern in the r
+00007a10: 6573 756c 7427 7320 7374 646f 7574 0a20  esult's stdout. 
+00007a20: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00007a30: 2020 2020 2020 2020 6c61 7465 7374 5f70          latest_p
+00007a40: 726f 6772 6573 7320 3d20 7265 2e66 696e  rogress = re.fin
+00007a50: 6461 6c6c 280a 2020 2020 2020 2020 2020  dall(.          
+00007a60: 2020 2020 2020 7061 7474 6572 6e2c 2072        pattern, r
+00007a70: 6573 756c 742e 7374 646f 7574 295b 2d31  esult.stdout)[-1
+00007a80: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
+00007a90: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00007aa0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00007ab0: 6765 722e 6572 726f 7228 6622 4973 7375  ger.error(f"Issu
+00007ac0: 6520 7769 7468 2065 7874 7261 6374 696e  e with extractin
+00007ad0: 6720 7072 6f67 7265 7373 3a20 7b65 7d22  g progress: {e}"
+00007ae0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00007af0: 6e20 6622 5072 6f67 7265 7373 3a20 7b6c  n f"Progress: {l
+00007b00: 6174 6573 745f 7072 6f67 7265 7373 7d5c  atest_progress}\
+00007b10: 6e22 0a0a 2020 2020 6465 6620 7275 6e5f  n"..    def run_
+00007b20: 636f 6d6d 616e 6473 2873 656c 662c 2063  commands(self, c
+00007b30: 6d64 6c69 7374 3a20 4c69 7374 5b73 7472  mdlist: List[str
+00007b40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007b50: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
+00007b60: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00007b70: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2020 2073 6570 3a20 7374 7220 3d20 2720     sep: str = ' 
+00007ba0: 2626 2027 2c0a 2020 2020 2020 2020 2020  && ',.          
+00007bb0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00007bc0: 7267 7329 202d 3e20 5265 7375 6c74 3a0a  rgs) -> Result:.
+00007bd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007be0: 2020 2020 5275 6e20 6120 6c69 7374 206f      Run a list o
+00007bf0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
+00007c00: 2063 6f6e 7365 6375 7469 7665 6c79 206f   consecutively o
+00007c10: 6e20 7468 6520 536c 7572 6d20 636c 7573  n the Slurm clus
+00007c20: 7465 722c 0a20 2020 2020 2020 2065 6e73  ter,.        ens
+00007c30: 7572 696e 6720 7468 6520 7375 6363 6573  uring the succes
+00007c40: 7320 6f66 2065 6163 6820 6265 666f 7265  s of each before
+00007c50: 2070 726f 6365 6564 696e 6720 746f 2074   proceeding to t
+00007c60: 6865 206e 6578 742e 0a0a 2020 2020 2020  he next...      
+00007c70: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
+00007c80: 7420 7661 7269 6162 6c65 7320 6361 6e20  t variables can 
+00007c90: 6265 2073 6574 2075 7369 6e67 2074 6865  be set using the
+00007ca0: 2060 656e 7660 2061 7267 756d 656e 742e   `env` argument.
+00007cb0: 0a20 2020 2020 2020 2054 6865 7365 2063  .        These c
+00007cc0: 6f6d 6d61 6e64 7320 7265 7461 696e 2074  ommands retain t
+00007cd0: 6865 2073 616d 6520 7365 7373 696f 6e20  he same session 
+00007ce0: 2865 6e76 6972 6f6e 6d65 6e74 2076 6172  (environment var
+00007cf0: 6961 626c 6573 0a20 2020 2020 2020 2065  iables.        e
+00007d00: 7463 2e29 2c20 756e 6c69 6b65 2072 756e  tc.), unlike run
+00007d10: 6e69 6e67 2074 6865 6d20 7365 7061 7261  ning them separa
+00007d20: 7465 6c79 2e0a 0a20 2020 2020 2020 2041  tely...        A
+00007d30: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00007d40: 2063 6d64 6c69 7374 2028 4c69 7374 5b73   cmdlist (List[s
+00007d50: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
+00007d60: 7368 656c 6c20 636f 6d6d 616e 6473 2074  shell commands t
+00007d70: 6f20 7275 6e20 6f6e 2053 6c75 726d 2e0a  o run on Slurm..
+00007d80: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+00007d90: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
+00007da0: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
+00007db0: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
+00007dc0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007de0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+00007df0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+00007e00: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00007e10: 2020 2020 2020 2020 2020 7365 7020 2873            sep (s
+00007e20: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
+00007e30: 6865 2073 6570 6172 6174 6f72 2075 7365  he separator use
+00007e40: 6420 746f 2063 6f6e 6361 7465 6e61 7465  d to concatenate
+00007e50: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+00007e60: 2020 2020 2020 636f 6d6d 616e 6473 2e20        commands. 
+00007e70: 4465 6661 756c 7473 2074 6f20 2720 2626  Defaults to ' &&
+00007e80: 2027 2e0a 2020 2020 2020 2020 2020 2020   '..            
+00007e90: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
+00007ea0: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+00007eb0: 756d 656e 7473 2e0a 0a20 2020 2020 2020  uments...       
+00007ec0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00007ed0: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
+00007ee0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+00007ef0: 6c61 7374 2063 6f6d 6d61 6e64 2069 6e20  last command in 
+00007f00: 7468 6520 6c69 7374 2e0a 2020 2020 2020  the list..      
+00007f10: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00007f20: 2065 6e76 2069 7320 4e6f 6e65 3a0a 2020   env is None:.  
+00007f30: 2020 2020 2020 2020 2020 656e 7620 3d20            env = 
+00007f40: 7b7d 0a20 2020 2020 2020 2063 6d64 203d  {}.        cmd =
+00007f50: 2073 6570 2e6a 6f69 6e28 636d 646c 6973   sep.join(cmdlis
+00007f60: 7429 0a20 2020 2020 2020 206c 6f67 6765  t).        logge
+00007f70: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+00007f80: 2020 2020 6622 5275 6e6e 696e 6720 636f      f"Running co
+00007f90: 6d6d 616e 6473 2c20 7769 7468 2065 6e76  mmands, with env
+00007fa0: 207b 656e 767d 2061 6e64 2073 6570 207b   {env} and sep {
+00007fb0: 7365 707d 205c 0a20 2020 2020 2020 2020  sep} \.         
+00007fc0: 2020 2020 2020 2061 6e64 207b 6b77 6172         and {kwar
+00007fd0: 6773 7d3a 207b 636d 647d 2229 0a20 2020  gs}: {cmd}").   
+00007fe0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00007ff0: 6c66 2e72 756e 2863 6d64 2c20 656e 763d  lf.run(cmd, env=
+00008000: 656e 762c 202a 2a6b 7761 7267 7329 2020  env, **kwargs)  
+00008010: 2320 6f75 745f 7374 7265 616d 3d6f 7574  # out_stream=out
+00008020: 5f73 7472 6561 6d2c 0a0a 2020 2020 2020  _stream,..      
+00008030: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00008040: 2020 2023 2057 6174 6368 206f 7574 2066     # Watch out f
+00008050: 6f72 2055 6e69 636f 6465 456e 636f 6465  or UnicodeEncode
+00008060: 4572 726f 7220 7768 656e 2079 6f75 2073  Error when you s
+00008070: 7472 2829 2074 6869 732e 0a20 2020 2020  tr() this..     
+00008080: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00008090: 666f 2866 227b 7265 7375 6c74 2e73 7464  fo(f"{result.std
+000080a0: 6f75 747d 2229 0a20 2020 2020 2020 2065  out}").        e
+000080b0: 7863 6570 7420 556e 6963 6f64 6545 6e63  xcept UnicodeEnc
+000080c0: 6f64 6545 7272 6f72 2061 7320 653a 0a20  odeError as e:. 
+000080d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000080e0: 722e 6572 726f 7228 6622 556e 6963 6f64  r.error(f"Unicod
+000080f0: 6520 6572 726f 723a 207b 657d 2229 0a20  e error: {e}"). 
+00008100: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00008110: 4f3a 204f 4e4c 5920 7374 646f 7574 2052  O: ONLY stdout R
+00008120: 4543 4f44 4520 4e45 4544 4544 3f3f 206f  ECODE NEEDED?? o
+00008130: 7220 616c 736f 2065 7272 6f72 3f0a 2020  r also error?.  
+00008140: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00008150: 2e73 7464 6f75 7420 3d20 7265 7375 6c74  .stdout = result
+00008160: 2e73 7464 6f75 742e 656e 636f 6465 280a  .stdout.encode(.
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2775 7466 2d38 272c 2027 6967 6e6f 7265  'utf-8', 'ignore
+00008190: 2729 2e64 6563 6f64 6528 2775 7466 2d38  ').decode('utf-8
+000081a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000081b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000081c0: 6620 7374 725f 746f 5f63 6c61 7373 2873  f str_to_class(s
+000081d0: 656c 662c 206d 6f64 756c 655f 6e61 6d65  elf, module_name
+000081e0: 3a20 7374 722c 2063 6c61 7373 5f6e 616d  : str, class_nam
+000081f0: 653a 2073 7472 2c20 2a61 7267 732c 202a  e: str, *args, *
+00008200: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00008210: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00008220: 7475 726e 2061 2063 6c61 7373 2069 6e73  turn a class ins
+00008230: 7461 6e63 6520 6672 6f6d 2061 2073 7472  tance from a str
+00008240: 696e 6720 7265 6665 7265 6e63 652e 0a0a  ing reference...
+00008250: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00008260: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
+00008270: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
+00008280: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
+00008290: 756c 652e 0a20 2020 2020 2020 2020 2020  ule..           
+000082a0: 2063 6c61 7373 5f6e 616d 6520 2873 7472   class_name (str
+000082b0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+000082c0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
+000082d0: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
+000082e0: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
+000082f0: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
+00008300: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
+00008310: 7275 6374 6f72 2e0a 2020 2020 2020 2020  ructor..        
+00008320: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
+00008330: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+00008340: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
+00008350: 6865 2063 6c61 7373 2063 6f6e 7374 7275  he class constru
+00008360: 6374 6f72 2e0a 0a20 2020 2020 2020 2052  ctor...        R
+00008370: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00008380: 2020 2020 6f62 6a65 6374 3a20 416e 2069      object: An i
+00008390: 6e73 7461 6e63 6520 6f66 2074 6865 2073  nstance of the s
+000083a0: 7065 6369 6669 6564 2063 6c61 7373 2c20  pecified class, 
+000083b0: 6f72 204e 6f6e 6520 6966 2074 6865 2063  or None if the c
+000083c0: 6c61 7373 206f 720a 2020 2020 2020 2020  lass or.        
+000083d0: 2020 2020 2020 2020 6d6f 6475 6c65 2064          module d
+000083e0: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
+000083f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008400: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00008410: 2020 2020 6d6f 6475 6c65 5f20 3d20 696d      module_ = im
+00008420: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
+00008430: 6f64 756c 6528 6d6f 6475 6c65 5f6e 616d  odule(module_nam
+00008440: 6529 0a20 2020 2020 2020 2020 2020 2074  e).            t
+00008450: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00008460: 2020 2020 636c 6173 735f 203d 2067 6574      class_ = get
+00008470: 6174 7472 286d 6f64 756c 655f 2c20 636c  attr(module_, cl
+00008480: 6173 735f 6e61 6d65 2928 2a61 7267 732c  ass_name)(*args,
+00008490: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+000084a0: 2020 2020 2020 2065 7863 6570 7420 4174         except At
+000084b0: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
+000084c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000084d0: 6767 6572 2e65 7272 6f72 2827 436c 6173  gger.error('Clas
+000084e0: 7320 646f 6573 206e 6f74 2065 7869 7374  s does not exist
+000084f0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
+00008500: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+00008510: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00008520: 722e 6572 726f 7228 274d 6f64 756c 6520  r.error('Module 
+00008530: 646f 6573 206e 6f74 2065 7869 7374 2729  does not exist')
+00008540: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008550: 636c 6173 735f 206f 7220 4e6f 6e65 0a0a  class_ or None..
+00008560: 2020 2020 6465 6620 7275 6e5f 636f 6d6d      def run_comm
+00008570: 616e 6473 5f73 706c 6974 5f6f 7574 2873  ands_split_out(s
+00008580: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085a0: 2020 2020 636d 646c 6973 743a 204c 6973      cmdlist: Lis
+000085b0: 745b 7374 725d 2c0a 2020 2020 2020 2020  t[str],.        
+000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+000085e0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+000085f0: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008610: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+00008620: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
+00008630: 2020 2022 2222 5275 6e20 6120 6c69 7374     """Run a list
+00008640: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
+00008650: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
+00008660: 2061 6e64 2073 706c 6974 2074 6865 206f   and split the o
+00008670: 7574 7075 740a 2020 2020 2020 2020 6f66  utput.        of
+00008680: 2065 6163 6820 636f 6d6d 616e 642e 0a0a   each command...
+00008690: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
+000086a0: 6d61 6e64 2069 6e20 7468 6520 6c69 7374  mand in the list
+000086b0: 2069 7320 6578 6563 7574 6564 2077 6974   is executed wit
+000086c0: 6820 6120 7365 7061 7261 746f 7220 696e  h a separator in
+000086d0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
+000086e0: 2074 6861 7420 6973 2075 6e69 7175 6520   that is unique 
+000086f0: 616e 6420 6361 6e20 6265 2075 7365 6420  and can be used 
+00008700: 746f 2073 706c 6974 0a20 2020 2020 2020  to split.       
+00008710: 2074 6865 206f 7574 7075 7420 6f66 2065   the output of e
+00008720: 6163 6820 636f 6d6d 616e 6420 6c61 7465  ach command late
+00008730: 722e 2054 6865 2073 6570 6172 6174 6f72  r. The separator
+00008740: 2075 7365 6420 6973 2073 7065 6369 6669   used is specifi
+00008750: 6564 0a20 2020 2020 2020 2062 7920 7468  ed.        by th
+00008760: 6520 605f 4f55 545f 5345 5060 2061 7474  e `_OUT_SEP` att
+00008770: 7269 6275 7465 206f 6620 7468 650a 2020  ribute of the.  
+00008780: 2020 2020 2020 536c 7572 6d43 6c69 656e        SlurmClien
+00008790: 7420 696e 7374 616e 6365 2e0a 0a20 2020  t instance...   
+000087a0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000087b0: 2020 2020 2020 2063 6d64 6c69 7374 2028         cmdlist (
+000087c0: 4c69 7374 5b73 7472 5d29 3a20 4120 6c69  List[str]): A li
+000087d0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
+000087e0: 616e 6473 2074 6f20 7275 6e2e 0a20 2020  ands to run..   
+000087f0: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+00008800: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+00008810: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+00008820: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+00008830: 7269 6162 6c65 7320 0a20 2020 2020 2020  riables .       
+00008840: 2020 2020 2020 2020 2074 6f20 7365 7420           to set 
+00008850: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
+00008860: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
+00008870: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
+00008880: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00008890: 2020 2020 2020 2020 2020 4c69 7374 5b73            List[s
+000088a0: 7472 5d3a 0a20 2020 2020 2020 2020 2020  tr]:.           
+000088b0: 2020 2020 2041 206c 6973 7420 6f66 2073       A list of s
+000088c0: 7472 696e 6773 2c20 7768 6572 6520 6561  trings, where ea
+000088d0: 6368 2073 7472 696e 6720 636f 7272 6573  ch string corres
+000088e0: 706f 6e64 7320 746f 0a20 2020 2020 2020  ponds to.       
+000088f0: 2020 2020 2020 2020 2074 6865 206f 7574           the out
+00008900: 7075 7420 6f66 2061 2073 696e 676c 6520  put of a single 
+00008910: 636f 6d6d 616e 6420 696e 2060 636d 646c  command in `cmdl
+00008920: 6973 7460 2073 706c 6974 0a20 2020 2020  ist` split.     
+00008930: 2020 2020 2020 2020 2020 2062 7920 7468             by th
+00008940: 6520 7365 7061 7261 746f 7220 605f 4f55  e separator `_OU
+00008950: 545f 5345 5060 2e0a 0a20 2020 2020 2020  T_SEP`...       
+00008960: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00008970: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
+00008980: 6e3a 2049 6620 616e 7920 6f66 2074 6865  n: If any of the
+00008990: 2063 6f6d 6d61 6e64 7320 6661 696c 2074   commands fail t
+000089a0: 6f20 6578 6563 7574 6520 7375 6363 6573  o execute succes
+000089b0: 7366 756c 6c79 2e0a 2020 2020 2020 2020  sfully..        
+000089c0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
+000089d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000089e0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+000089f0: 6f6d 6d61 6e64 7328 636d 646c 6973 743d  ommands(cmdlist=
+00008a00: 636d 646c 6973 742c 0a20 2020 2020 2020  cmdlist,.       
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 656e 763d 656e 762c 0a20 2020 2020 2020  env=env,.       
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a60: 7365 703d 6622 203b 2065 6368 6f20 7b73  sep=f" ; echo {s
+00008a70: 656c 662e 5f4f 5554 5f53 4550 7d20 3b20  elf._OUT_SEP} ; 
+00008a80: 2229 0a20 2020 2020 2020 2065 7863 6570  ").        excep
+00008a90: 7420 556e 6578 7065 6374 6564 4578 6974  t UnexpectedExit
+00008aa0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00008ab0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00008ac0: 6728 6529 0a20 2020 2020 2020 2020 2020  g(e).           
+00008ad0: 2072 6573 756c 7420 3d20 652e 7265 7375   result = e.resu
+00008ae0: 6c74 0a20 2020 2020 2020 2069 6620 7265  lt.        if re
+00008af0: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
+00008b00: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00008b10: 7265 7375 6c74 2e73 7464 6f75 740a 2020  result.stdout.  
+00008b20: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
+00008b30: 7265 7370 6f6e 7365 7320 3d20 7265 7370  responses = resp
+00008b40: 6f6e 7365 2e73 706c 6974 2873 656c 662e  onse.split(self.
+00008b50: 5f4f 5554 5f53 4550 290a 2020 2020 2020  _OUT_SEP).      
+00008b60: 2020 2020 2020 7265 7475 726e 2073 706c        return spl
+00008b70: 6974 5f72 6573 706f 6e73 6573 0a20 2020  it_responses.   
+00008b80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008b90: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00008ba0: 7265 7375 6c74 2069 7320 6e6f 7420 6f6b  result is not ok
+00008bb0: 2c20 6c6f 6720 7468 6520 6572 726f 7220  , log the error 
+00008bc0: 616e 6420 7261 6973 6520 616e 2053 5348  and raise an SSH
+00008bd0: 4578 6365 7074 696f 6e0a 2020 2020 2020  Exception.      
+00008be0: 2020 2020 2020 6572 726f 7220 3d20 6622        error = f"
+00008bf0: 5265 7375 6c74 2069 7320 6e6f 7420 6f6b  Result is not ok
+00008c00: 3a20 7b72 6573 756c 747d 220a 2020 2020  : {result}".    
+00008c10: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00008c20: 7272 6f72 2865 7272 6f72 290a 2020 2020  rror(error).    
+00008c30: 2020 2020 2020 2020 7261 6973 6520 5353          raise SS
+00008c40: 4845 7863 6570 7469 6f6e 2865 7272 6f72  HException(error
+00008c50: 290a 0a20 2020 2064 6566 206c 6973 745f  )..    def list_
+00008c60: 6163 7469 7665 5f6a 6f62 7328 7365 6c66  active_jobs(self
+00008c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008c80: 2020 2020 2020 2020 2020 2065 6e76 3a20             env: 
+00008c90: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00008ca0: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
+00008cb0: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
+00008cc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008cd0: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
+00008ce0: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
+00008cf0: 6d20 534c 5552 4d2e 0a0a 2020 2020 2020  m SLURM...      
+00008d00: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008d10: 2020 2020 656e 7620 2844 6963 745b 7374      env (Dict[st
+00008d20: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
+00008d30: 6c29 3a20 4f70 7469 6f6e 616c 2065 6e76  l): Optional env
+00008d40: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00008d50: 6573 2074 6f20 0a20 2020 2020 2020 2020  es to .         
+00008d60: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
+00008d70: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+00008d80: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
+00008d90: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+00008da0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00008db0: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
+00008dc0: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
+00008dd0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00008de0: 2020 2020 2020 2023 2063 6d64 203d 2073         # cmd = s
+00008df0: 656c 662e 5f41 4354 4956 455f 4a4f 4253  elf._ACTIVE_JOBS
+00008e00: 5f43 4d44 0a20 2020 2020 2020 2063 6d64  _CMD.        cmd
+00008e10: 203d 2073 656c 662e 6765 745f 6a6f 6273   = self.get_jobs
+00008e20: 5f69 6e66 6f5f 636f 6d6d 616e 6428 7374  _info_command(st
+00008e30: 6172 745f 7469 6d65 3d22 6e6f 7722 2c20  art_time="now", 
+00008e40: 7374 6174 6573 3d22 7222 290a 2020 2020  states="r").    
+00008e50: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00008e60: 2252 6574 7269 6576 696e 6720 6c69 7374  "Retrieving list
+00008e70: 206f 6620 6163 7469 7665 206a 6f62 7320   of active jobs 
+00008e80: 6672 6f6d 2053 6c75 726d 2229 0a20 2020  from Slurm").   
+00008e90: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00008ea0: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00008eb0: 5b63 6d64 5d2c 2065 6e76 3d65 6e76 290a  [cmd], env=env).
+00008ec0: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
+00008ed0: 203d 2072 6573 756c 742e 7374 646f 7574   = result.stdout
+00008ee0: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
+00008ef0: 5c6e 2729 0a20 2020 2020 2020 206a 6f62  \n').        job
+00008f00: 5f6c 6973 742e 7265 7665 7273 6528 290a  _list.reverse().
+00008f10: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+00008f20: 6f62 5f6c 6973 740a 0a20 2020 2064 6566  ob_list..    def
+00008f30: 206c 6973 745f 636f 6d70 6c65 7465 645f   list_completed_
+00008f40: 6a6f 6273 2873 656c 662c 0a20 2020 2020  jobs(self,.     
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+00008f70: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+00008f80: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+00008f90: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
+00008fa0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00008fb0: 6574 2061 206c 6973 7420 6f66 2063 6f6d  et a list of com
+00008fc0: 706c 6574 6564 206a 6f62 7320 6672 6f6d  pleted jobs from
+00008fd0: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
+00008fe0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00008ff0: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
+00009000: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
+00009010: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
+00009020: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00009030: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
+00009040: 2020 2020 2073 6574 2077 6865 6e20 7275       set when ru
+00009050: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
+00009060: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
+00009070: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
+00009080: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00009090: 2020 204c 6973 745b 7374 725d 3a20 4120     List[str]: A 
+000090a0: 6c69 7374 206f 6620 6a6f 6220 4944 732e  list of job IDs.
+000090b0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+000090c0: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
+000090d0: 2e67 6574 5f6a 6f62 735f 696e 666f 5f63  .get_jobs_info_c
+000090e0: 6f6d 6d61 6e64 2873 7461 7465 733d 2263  ommand(states="c
+000090f0: 6422 290a 2020 2020 2020 2020 6c6f 6767  d").        logg
+00009100: 6572 2e69 6e66 6f28 2252 6574 7269 6576  er.info("Retriev
+00009110: 696e 6720 6120 6c69 7374 206f 6620 636f  ing a list of co
+00009120: 6d70 6c65 7465 6420 6a6f 6273 2066 726f  mpleted jobs fro
+00009130: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
+00009140: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00009150: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+00009160: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
+00009170: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
+00009180: 5b6a 6f62 2e73 7472 6970 2829 2066 6f72  [job.strip() for
+00009190: 206a 6f62 2069 6e20 7265 7375 6c74 2e73   job in result.s
+000091a0: 7464 6f75 742e 7374 7269 7028 292e 7370  tdout.strip().sp
+000091b0: 6c69 7428 275c 6e27 295d 0a20 2020 2020  lit('\n')].     
+000091c0: 2020 206a 6f62 5f6c 6973 742e 7265 7665     job_list.reve
+000091d0: 7273 6528 290a 2020 2020 2020 2020 7265  rse().        re
+000091e0: 7475 726e 206a 6f62 5f6c 6973 740a 0a20  turn job_list.. 
+000091f0: 2020 2064 6566 206c 6973 745f 616c 6c5f     def list_all_
+00009200: 6a6f 6273 2873 656c 662c 2065 6e76 3a20  jobs(self, env: 
+00009210: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00009220: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
+00009230: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
+00009240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009250: 2020 2047 6574 2061 206c 6973 7420 6f66     Get a list of
+00009260: 2061 6c6c 206a 6f62 7320 6672 6f6d 2053   all jobs from S
+00009270: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
+00009280: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00009290: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
+000092a0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
+000092b0: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
+000092c0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092e0: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
+000092f0: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
+00009300: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00009310: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
+00009320: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00009330: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
+00009340: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
+00009350: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00009360: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
+00009370: 6765 745f 6a6f 6273 5f69 6e66 6f5f 636f  get_jobs_info_co
+00009380: 6d6d 616e 6428 290a 2020 2020 2020 2020  mmand().        
+00009390: 6c6f 6767 6572 2e69 6e66 6f28 2252 6574  logger.info("Ret
+000093a0: 7269 6576 696e 6720 6120 6c69 7374 206f  rieving a list o
+000093b0: 6620 616c 6c20 6a6f 6273 2066 726f 6d20  f all jobs from 
+000093c0: 536c 7572 6d22 290a 2020 2020 2020 2020  Slurm").        
+000093d0: 7265 7375 6c74 203d 2073 656c 662e 7275  result = self.ru
+000093e0: 6e5f 636f 6d6d 616e 6473 285b 636d 645d  n_commands([cmd]
+000093f0: 2c20 656e 763d 656e 7629 0a20 2020 2020  , env=env).     
+00009400: 2020 206a 6f62 5f6c 6973 7420 3d20 7265     job_list = re
+00009410: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
+00009420: 7028 292e 7370 6c69 7428 275c 6e27 290a  p().split('\n').
+00009430: 2020 2020 2020 2020 6a6f 625f 6c69 7374          job_list
+00009440: 2e72 6576 6572 7365 2829 0a20 2020 2020  .reverse().     
+00009450: 2020 2072 6574 7572 6e20 6a6f 625f 6c69     return job_li
+00009460: 7374 0a0a 2020 2020 6465 6620 6765 745f  st..    def get_
+00009470: 6a6f 6273 5f69 6e66 6f5f 636f 6d6d 616e  jobs_info_comman
+00009480: 6428 7365 6c66 2c20 7374 6172 745f 7469  d(self, start_ti
+00009490: 6d65 3a20 7374 7220 3d20 2232 3032 332d  me: str = "2023-
+000094a0: 3031 2d30 3122 2c0a 2020 2020 2020 2020  01-01",.        
+000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094c0: 2020 2020 2020 656e 645f 7469 6d65 3a20        end_time: 
+000094d0: 7374 7220 3d20 226e 6f77 222c 0a20 2020  str = "now",.   
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+00009500: 6e73 3a20 7374 7220 3d20 224a 6f62 4964  ns: str = "JobId
+00009510: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 2073 7461 7465 733a 2073 7472 203d 2022   states: str = "
+00009540: 722c 6364 2c66 2c74 6f2c 7273 2c64 6c2c  r,cd,f,to,rs,dl,
+00009550: 6e66 2229 202d 3e20 7374 723a 0a20 2020  nf") -> str:.   
+00009560: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+00009570: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
+00009580: 2074 6f20 7265 7472 6965 7665 2069 6e66   to retrieve inf
+00009590: 6f72 6d61 7469 6f6e 2061 626f 7574 206f  ormation about o
+000095a0: 6c64 206a 6f62 732e 0a0a 2020 2020 2020  ld jobs...      
+000095b0: 2020 5468 6520 636f 6d6d 616e 6420 7769    The command wi
+000095c0: 6c6c 2062 6520 666f 726d 6174 7465 6420  ll be formatted 
+000095d0: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
+000095e0: 6564 2073 7461 7274 2074 696d 652c 2077  ed start time, w
+000095f0: 6869 6368 2069 730a 2020 2020 2020 2020  hich is.        
+00009600: 6578 7065 6374 6564 2074 6f20 6265 2069  expected to be i
+00009610: 6e20 7468 6520 4953 4f20 666f 726d 6174  n the ISO format
+00009620: 2022 5959 5959 2d4d 4d2d 4444 222e 0a20   "YYYY-MM-DD".. 
+00009630: 2020 2020 2020 2054 6865 2063 6f6d 6d61         The comma
+00009640: 6e64 2077 696c 6c20 7573 6520 7468 6520  nd will use the 
+00009650: 2273 6163 6374 2220 746f 6f6c 2074 6f20  "sacct" tool to 
+00009660: 7175 6572 7920 7468 650a 2020 2020 2020  query the.      
+00009670: 2020 536c 7572 6d20 6163 636f 756e 7469    Slurm accounti
+00009680: 6e67 2064 6174 6162 6173 6520 666f 7220  ng database for 
+00009690: 6a6f 6273 2074 6861 7420 7374 6172 7465  jobs that starte
+000096a0: 6420 6f6e 206f 7220 6166 7465 7220 7468  d on or after th
+000096b0: 650a 2020 2020 2020 2020 7370 6563 6966  e.        specif
+000096c0: 6965 6420 7374 6172 7420 7469 6d65 2c20  ied start time, 
+000096d0: 616e 6420 7769 6c6c 206f 7574 7075 7420  and will output 
+000096e0: 6f6e 6c79 2074 6865 206a 6f62 2049 4473  only the job IDs
+000096f0: 2028 2d6f 204a 6f62 4964 290a 2020 2020   (-o JobId).    
+00009700: 2020 2020 7769 7468 6f75 7420 6865 6164      without head
+00009710: 6572 206f 7220 7472 6169 6c65 7220 6c69  er or trailer li
+00009720: 6e65 7320 282d 6e20 2d58 292e 0a0a 2020  nes (-n -X)...  
+00009730: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00009740: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+00009750: 6d65 2028 7374 7229 3a20 5468 6520 7374  me (str): The st
+00009760: 6172 7420 7469 6d65 2066 726f 6d20 7768  art time from wh
+00009770: 6963 6820 746f 2072 6574 7269 6576 6520  ich to retrieve 
+00009780: 6a6f 620a 2020 2020 2020 2020 2020 2020  job.            
+00009790: 2020 2020 696e 666f 726d 6174 696f 6e2e      information.
+000097a0: 2044 6566 6175 6c74 7320 746f 2022 3230   Defaults to "20
+000097b0: 3233 2d30 312d 3031 222e 0a20 2020 2020  23-01-01"..     
+000097c0: 2020 2020 2020 2065 6e64 5f74 696d 6520         end_time 
+000097d0: 2873 7472 293a 2054 6865 2065 6e64 2074  (str): The end t
+000097e0: 696d 6520 756e 7469 6c20 7768 6963 6820  ime until which 
+000097f0: 746f 2072 6574 7269 6576 6520 6a6f 620a  to retrieve job.
 00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
-00009830: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 2073 7461 7465 733d 7374 6174       states=stat
-00009870: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009890: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-000098a0: 756d 6e73 3d63 6f6c 756d 6e73 290a 0a20  umns=columns).. 
-000098b0: 2020 2064 6566 2074 7261 6e73 6665 725f     def transfer_
-000098c0: 6461 7461 2873 656c 662c 206c 6f63 616c  data(self, local
-000098d0: 5f70 6174 683a 2073 7472 2920 2d3e 2052  _path: str) -> R
-000098e0: 6573 756c 743a 0a20 2020 2020 2020 2022  esult:.        "
-000098f0: 2222 0a20 2020 2020 2020 2054 7261 6e73  "".        Trans
-00009900: 6665 7273 2061 2066 696c 6520 6f72 2064  fers a file or d
-00009910: 6972 6563 746f 7279 2066 726f 6d20 7468  irectory from th
-00009920: 6520 6c6f 6361 6c20 6d61 6368 696e 6520  e local machine 
-00009930: 746f 2074 6865 2072 656d 6f74 650a 2020  to the remote.  
-00009940: 2020 2020 2020 536c 7572 6d20 636c 7573        Slurm clus
-00009950: 7465 722e 0a0a 2020 2020 2020 2020 4172  ter...        Ar
-00009960: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00009970: 6c6f 6361 6c5f 7061 7468 2028 7374 7229  local_path (str)
-00009980: 3a20 5468 6520 6c6f 6361 6c20 7061 7468  : The local path
-00009990: 2074 6f20 7468 6520 6669 6c65 206f 7220   to the file or 
-000099a0: 6469 7265 6374 6f72 7920 746f 0a20 2020  directory to.   
-000099b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000099c0: 6e73 6665 722e 0a0a 2020 2020 2020 2020  nsfer...        
-000099d0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000099e0: 2020 2020 2052 6573 756c 743a 2054 6865       Result: The
-000099f0: 2072 6573 756c 7420 6f66 2074 6865 2066   result of the f
-00009a00: 696c 6520 7472 616e 7366 6572 206f 7065  ile transfer ope
-00009a10: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00009a20: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00009a30: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
-00009a40: 2020 2020 2066 2254 7261 6e73 6665 7269       f"Transferi
-00009a50: 6e67 2066 696c 6520 7b6c 6f63 616c 5f70  ng file {local_p
-00009a60: 6174 687d 2074 6f20 7b73 656c 662e 736c  ath} to {self.sl
-00009a70: 7572 6d5f 6461 7461 5f70 6174 687d 2229  urm_data_path}")
-00009a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009a90: 7365 6c66 2e70 7574 286c 6f63 616c 3d6c  self.put(local=l
-00009aa0: 6f63 616c 5f70 6174 682c 2072 656d 6f74  ocal_path, remot
-00009ab0: 653d 7365 6c66 2e73 6c75 726d 5f64 6174  e=self.slurm_dat
-00009ac0: 615f 7061 7468 290a 0a20 2020 2064 6566  a_path)..    def
-00009ad0: 2075 6e70 6163 6b5f 6461 7461 2873 656c   unpack_data(sel
-00009ae0: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
-00009af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b00: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
-00009b10: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
-00009b20: 5d5d 203d 204e 6f6e 6529 202d 3e20 5265  ]] = None) -> Re
-00009b30: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
-00009b40: 220a 2020 2020 2020 2020 556e 7061 636b  ".        Unpack
-00009b50: 7320 6120 7a69 7070 6564 2066 696c 6520  s a zipped file 
-00009b60: 6f6e 2074 6865 2072 656d 6f74 6520 536c  on the remote Sl
-00009b70: 7572 6d20 636c 7573 7465 722e 0a0a 2020  urm cluster...  
-00009b80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009b90: 2020 2020 2020 2020 7a69 7066 696c 6520          zipfile 
-00009ba0: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
-00009bb0: 6f66 2074 6865 207a 6970 7065 6420 6669  of the zipped fi
-00009bc0: 6c65 2074 6f20 6265 2075 6e70 6163 6b65  le to be unpacke
-00009bd0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00009be0: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
-00009bf0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-00009c00: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
-00009c10: 6d65 6e74 2076 6172 6961 626c 6573 200a  ment variables .
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 746f 2073 6574 2077 6865 6e20 7275 6e6e  to set when runn
-00009c40: 696e 6720 7468 6520 636f 6d6d 616e 642e  ing the command.
-00009c50: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00009c60: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00009c70: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00009c80: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
-00009c90: 756c 7420 6f66 2074 6865 2063 6f6d 6d61  ult of the comma
-00009ca0: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
-00009cb0: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00009cc0: 6c66 2e67 6574 5f75 6e7a 6970 5f63 6f6d  lf.get_unzip_com
-00009cd0: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
-00009ce0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00009cf0: 6f28 6622 556e 7061 636b 696e 6720 7b7a  o(f"Unpacking {z
-00009d00: 6970 6669 6c65 7d20 6f6e 2053 6c75 726d  ipfile} on Slurm
-00009d10: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00009d20: 6e20 7365 6c66 2e72 756e 5f63 6f6d 6d61  n self.run_comma
-00009d30: 6e64 7328 5b63 6d64 5d2c 2065 6e76 3d65  nds([cmd], env=e
-00009d40: 6e76 290a 0a20 2020 2064 6566 2063 6f6e  nv)..    def con
-00009d50: 7665 7274 5f64 6174 6128 7365 6c66 2c20  vert_data(self, 
-00009d60: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2065 6e76 3a20 4f70 7469 6f6e 616c     env: Optional
-00009d90: 5b44 6963 745b 7374 722c 2073 7472 5d5d  [Dict[str, str]]
-00009da0: 203d 204e 6f6e 6529 202d 3e20 5265 7375   = None) -> Resu
-00009db0: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
-00009dc0: 2020 2020 2020 2020 556e 7061 636b 7320          Unpacks 
-00009dd0: 6120 7a69 7070 6564 2066 696c 6520 6f6e  a zipped file on
-00009de0: 2074 6865 2072 656d 6f74 6520 536c 7572   the remote Slur
-00009df0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
-00009e00: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00009e10: 2020 2020 2020 7a69 7066 696c 6520 2873        zipfile (s
-00009e20: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-00009e30: 2074 6865 207a 6970 7065 6420 6669 6c65   the zipped file
-00009e40: 2074 6f20 6265 2075 6e70 6163 6b65 642e   to be unpacked.
-00009e50: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-00009e60: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
-00009e70: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
-00009e80: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
-00009e90: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00009eb0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
-00009ec0: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
-00009ed0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00009ee0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00009ef0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00009f00: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
-00009f10: 7420 6f66 2074 6865 2063 6f6d 6d61 6e64  t of the command
-00009f20: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00009f30: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-00009f40: 2e67 6574 5f63 6f6e 7665 7274 5f63 6f6d  .get_convert_com
-00009f50: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
-00009f60: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00009f70: 6f28 6622 436f 6e76 6572 7469 6e67 207b  o(f"Converting {
-00009f80: 7a69 7066 696c 657d 206f 6e20 536c 7572  zipfile} on Slur
-00009f90: 6d22 290a 2020 2020 2020 2020 7265 7475  m").        retu
-00009fa0: 726e 2073 656c 662e 7275 6e5f 636f 6d6d  rn self.run_comm
-00009fb0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
-00009fc0: 656e 7629 0a0a 2020 2020 6465 6620 6765  env)..    def ge
-00009fd0: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
-00009fe0: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7365  _for_workflow(se
-00009ff0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000a020: 666c 6f77 3a20 7374 722c 0a20 2020 2020  flow: str,.     
-0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 2020 2073 7562 7374 6974 7574 6573 3a20     substitutes: 
-0000a060: 4469 6374 5b73 7472 2c20 7374 725d 2c0a  Dict[str, str],.
-0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
-0000a0a0: 3a20 7374 7220 3d20 226a 6f62 5f74 656d  : str = "job_tem
-0000a0b0: 706c 6174 652e 7368 220a 2020 2020 2020  plate.sh".      
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0e0: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
-0000a0f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a100: 4765 6e65 7261 7465 2061 2053 6c75 726d  Generate a Slurm
-0000a110: 206a 6f62 2073 6372 6970 7420 666f 7220   job script for 
-0000a120: 6120 7370 6563 6966 6963 2077 6f72 6b66  a specific workf
-0000a130: 6c6f 772e 0a0a 2020 2020 2020 2020 4172  low...        Ar
-0000a140: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000a150: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
-0000a160: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000a170: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
-0000a180: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
-0000a190: 7320 2844 6963 745b 7374 722c 2073 7472  s (Dict[str, str
-0000a1a0: 5d29 3a20 4120 6469 6374 696f 6e61 7279  ]): A dictionary
-0000a1b0: 2063 6f6e 7461 696e 696e 6720 6b65 792d   containing key-
-0000a1c0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
-0000a1d0: 2020 2020 2020 7061 6972 7320 666f 7220        pairs for 
-0000a1e0: 7375 6273 7469 7475 7469 6e67 2070 6c61  substituting pla
-0000a1f0: 6365 686f 6c64 6572 7320 696e 2074 6865  ceholders in the
-0000a200: 206a 6f62 2074 656d 706c 6174 652e 0a20   job template.. 
-0000a210: 2020 2020 2020 2020 2020 2074 656d 706c             templ
-0000a220: 6174 6520 2873 7472 2c20 6f70 7469 6f6e  ate (str, option
-0000a230: 616c 293a 2054 6865 2066 696c 656e 616d  al): The filenam
-0000a240: 6520 6f66 2074 6865 206a 6f62 2074 656d  e of the job tem
-0000a250: 706c 6174 652e 0a20 2020 2020 2020 2020  plate..         
-0000a260: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-0000a270: 746f 2022 6a6f 625f 7465 6d70 6c61 7465  to "job_template
-0000a280: 2e73 6822 2e0a 0a20 2020 2020 2020 2052  .sh"...        R
-0000a290: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000a2a0: 2020 2020 7374 723a 2054 6865 2067 656e      str: The gen
-0000a2b0: 6572 6174 6564 2053 6c75 726d 206a 6f62  erated Slurm job
-0000a2c0: 2073 6372 6970 7420 6173 2061 2073 7472   script as a str
-0000a2d0: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
-0000a2e0: 0a20 2020 2020 2020 2023 2061 6464 2077  .        # add w
-0000a2f0: 6f72 6b66 6c6f 7720 746f 2073 7562 7374  orkflow to subst
-0000a300: 6974 7574 6573 0a20 2020 2020 2020 2073  itutes.        s
-0000a310: 7562 7374 6974 7574 6573 5b27 6a6f 626e  ubstitutes['jobn
-0000a320: 616d 6527 5d20 3d20 776f 726b 666c 6f77  ame'] = workflow
-0000a330: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
-0000a340: 6a6f 6220 7465 6d70 6c61 7465 0a20 2020  job template.   
-0000a350: 2020 2020 2074 656d 706c 6174 655f 6620       template_f 
-0000a360: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
-0000a370: 6573 2229 2e6a 6f69 6e70 6174 6828 7465  es").joinpath(te
-0000a380: 6d70 6c61 7465 290a 2020 2020 2020 2020  mplate).        
-0000a390: 7769 7468 2074 656d 706c 6174 655f 662e  with template_f.
-0000a3a0: 6f70 656e 2827 7227 2920 6173 2066 3a0a  open('r') as f:.
-0000a3b0: 2020 2020 2020 2020 2020 2020 7372 6320              src 
-0000a3c0: 3d20 5465 6d70 6c61 7465 2866 2e72 6561  = Template(f.rea
-0000a3d0: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
-0000a3e0: 206a 6f62 5f73 6372 6970 7420 3d20 7372   job_script = sr
-0000a3f0: 632e 7361 6665 5f73 7562 7374 6974 7574  c.safe_substitut
-0000a400: 6528 7375 6273 7469 7475 7465 7329 0a20  e(substitutes). 
-0000a410: 2020 2020 2020 2072 6574 7572 6e20 6a6f         return jo
-0000a420: 625f 7363 7269 7074 0a0a 2020 2020 6465  b_script..    de
-0000a430: 6620 776f 726b 666c 6f77 5f70 6172 616d  f workflow_param
-0000a440: 735f 746f 5f73 7562 7328 7365 6c66 2c20  s_to_subs(self, 
-0000a450: 7061 7261 6d73 2920 2d3e 2044 6963 745b  params) -> Dict[
-0000a460: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-0000a470: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000a480: 6f6e 7665 7274 2077 6f72 6b66 6c6f 7720  onvert workflow 
-0000a490: 7061 7261 6d65 7465 7273 2074 6f20 7375  parameters to su
-0000a4a0: 6273 7469 7475 7469 6f6e 2064 6963 7469  bstitution dicti
-0000a4b0: 6f6e 6172 7920 666f 7220 6a6f 6220 7363  onary for job sc
-0000a4c0: 7269 7074 2e0a 0a20 2020 2020 2020 2041  ript...        A
-0000a4d0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000a4e0: 2070 6172 616d 733a 2041 2064 6963 7469   params: A dicti
-0000a4f0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-0000a500: 2077 6f72 6b66 6c6f 7720 7061 7261 6d65   workflow parame
-0000a510: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
-0000a520: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000a530: 2020 2020 4469 6374 5b73 7472 2c20 7374      Dict[str, st
-0000a540: 725d 3a20 4120 6469 6374 696f 6e61 7279  r]: A dictionary
-0000a550: 2077 6974 6820 7061 7261 6d65 7465 7220   with parameter 
-0000a560: 6e61 6d65 7320 6173 206b 6579 7320 616e  names as keys an
-0000a570: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000a580: 2020 636f 7272 6573 706f 6e64 696e 6720    corresponding 
-0000a590: 666c 6167 7320 7769 7468 2070 6c61 6365  flags with place
-0000a5a0: 686f 6c64 6572 7320 6173 2076 616c 7565  holders as value
-0000a5b0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0000a5c0: 2020 2020 2020 2073 7562 7320 3d20 7b7d         subs = {}
-0000a5d0: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
-0000a5e0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0000a5f0: 5f2c 2070 6172 616d 2069 6e20 7061 7261  _, param in para
-0000a600: 6d73 2e69 7465 6d73 2829 3a0a 2020 2020  ms.items():.    
-0000a610: 2020 2020 2020 2020 666c 6167 203d 2070          flag = p
-0000a620: 6172 616d 5b27 636d 645f 666c 6167 275d  aram['cmd_flag']
-0000a630: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
-0000a640: 6720 3d20 666c 6167 202b 2022 2024 2220  g = flag + " $" 
-0000a650: 2b20 7061 7261 6d5b 276e 616d 6527 5d2e  + param['name'].
-0000a660: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-0000a670: 2020 2020 666c 6167 732e 6170 7065 6e64      flags.append
-0000a680: 2866 6c61 6729 0a20 2020 2020 2020 2073  (flag).        s
-0000a690: 7562 735b 2750 4152 414d 5327 5d20 3d20  ubs['PARAMS'] = 
-0000a6a0: 2220 222e 6a6f 696e 2866 6c61 6773 290a  " ".join(flags).
-0000a6b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000a6c0: 7562 730a 0a20 2020 2064 6566 2075 7064  ubs..    def upd
-0000a6d0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
-0000a6e0: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 2067 656e 6572 6174 655f 6a6f       generate_jo
-0000a710: 6273 3a20 626f 6f6c 203d 2046 616c 7365  bs: bool = False
-0000a720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a740: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
-0000a750: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
-0000a760: 6f6e 6529 202d 3e20 5265 7375 6c74 3a0a  one) -> Result:.
-0000a770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000a780: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
-0000a790: 6c6f 6361 6c20 636f 7079 206f 6620 7468  local copy of th
-0000a7a0: 6520 536c 7572 6d20 6a6f 6220 7375 626d  e Slurm job subm
-0000a7b0: 6973 7369 6f6e 2073 6372 6970 7473 2e0a  ission scripts..
-0000a7c0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
-0000a7d0: 6e63 7469 6f6e 2070 756c 6c73 2074 6865  nction pulls the
-0000a7e0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
-0000a7f0: 6f66 2074 6865 2073 6372 6970 7473 2066  of the scripts f
-0000a800: 726f 6d20 7468 6520 4769 740a 2020 2020  rom the Git.    
-0000a810: 2020 2020 7265 706f 7369 746f 7279 2061      repository a
-0000a820: 6e64 2063 6f70 6965 7320 7468 656d 2074  nd copies them t
-0000a830: 6f20 7468 6520 736c 7572 6d5f 7363 7269  o the slurm_scri
-0000a840: 7074 5f70 6174 6820 6469 7265 6374 6f72  pt_path director
-0000a850: 792e 0a20 2020 2020 2020 2041 6c74 6572  y..        Alter
-0000a860: 6e61 7469 7665 6c79 2c20 6974 2063 616e  natively, it can
-0000a870: 2067 656e 6572 6174 6520 7363 7269 7074   generate script
-0000a880: 7320 6672 6f6d 2061 2074 656d 706c 6174  s from a templat
-0000a890: 652e 2054 6869 7320 6973 2074 6865 0a20  e. This is the. 
-0000a8a0: 2020 2020 2020 2064 6566 6175 6c74 2062         default b
-0000a8b0: 6568 6176 696f 7220 6966 206e 6f20 4769  ehavior if no Gi
-0000a8c0: 7420 7265 706f 2069 7320 7072 6f76 6964  t repo is provid
-0000a8d0: 6564 206f 7220 6361 6e20 6265 2066 6f72  ed or can be for
-0000a8e0: 6365 6420 7669 6120 7468 650a 2020 2020  ced via the.    
-0000a8f0: 2020 2020 6067 656e 6572 6174 655f 6a6f      `generate_jo
-0000a900: 6273 6020 7061 7261 6d65 7465 722e 0a0a  bs` parameter...
-0000a910: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000a920: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
-0000a930: 7465 5f6a 6f62 7320 2862 6f6f 6c29 3a20  te_jobs (bool): 
-0000a940: 5768 6574 6865 7220 746f 2067 656e 6572  Whether to gener
-0000a950: 6174 6520 6e65 7720 736c 7572 6d20 6a6f  ate new slurm jo
-0000a960: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
-0000a970: 2020 2020 2020 2020 2020 494e 5354 4541            INSTEA
-0000a980: 4420 286f 6620 7075 6c6c 696e 6720 6672  D (of pulling fr
-0000a990: 6f6d 2067 6974 292e 2044 6566 6175 6c74  om git). Default
-0000a9a0: 7320 746f 2046 616c 7365 2c20 6578 6365  s to False, exce
-0000a9b0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
-0000a9c0: 2020 2069 6620 6e6f 2073 6c75 726d 5f73     if no slurm_s
-0000a9d0: 6372 6970 745f 7265 706f 2069 7320 636f  cript_repo is co
-0000a9e0: 6e66 6967 7572 6564 2e0a 2020 2020 2020  nfigured..      
-0000a9f0: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-0000aa00: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-0000aa10: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-0000aa20: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-0000aa30: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
-0000aa40: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
-0000aa50: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-0000aa60: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-0000aa70: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-0000aa80: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000aa90: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
-0000aaa0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-0000aab0: 2063 6f6d 6d61 6e64 2e0a 2020 2020 2020   command..      
-0000aac0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000aad0: 206e 6f74 2073 656c 662e 736c 7572 6d5f   not self.slurm_
-0000aae0: 7363 7269 7074 5f72 6570 6f3a 0a20 2020  script_repo:.   
-0000aaf0: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-0000ab00: 655f 6a6f 6273 203d 2054 7275 650a 0a20  e_jobs = True.. 
-0000ab10: 2020 2020 2020 2069 6620 6765 6e65 7261         if genera
-0000ab20: 7465 5f6a 6f62 733a 0a20 2020 2020 2020  te_jobs:.       
-0000ab30: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000ab40: 2822 4765 6e65 7261 7469 6e67 2053 6c75  ("Generating Slu
-0000ab50: 726d 206a 6f62 2073 6372 6970 7473 2229  rm job scripts")
-0000ab60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000ab70: 2077 662c 206a 6f62 5f70 6174 6820 696e   wf, job_path in
-0000ab80: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-0000ab90: 6c5f 6a6f 6273 2e69 7465 6d73 2829 3a0a  l_jobs.items():.
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2320 6765 6e65 7261 7465 206a 6f62 2073  # generate job s
-0000abc0: 6372 6970 740a 2020 2020 2020 2020 2020  cript.          
-0000abd0: 2020 2020 2020 7061 7261 6d73 203d 2073        params = s
-0000abe0: 656c 662e 6765 745f 776f 726b 666c 6f77  elf.get_workflow
-0000abf0: 5f70 6172 616d 6574 6572 7328 7766 290a  _parameters(wf).
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 7375 6273 203d 2073 656c 662e 776f 726b  subs = self.work
-0000ac20: 666c 6f77 5f70 6172 616d 735f 746f 5f73  flow_params_to_s
-0000ac30: 7562 7328 7061 7261 6d73 290a 2020 2020  ubs(params).    
-0000ac40: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000ac50: 7363 7269 7074 203d 2073 656c 662e 6765  script = self.ge
-0000ac60: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
-0000ac70: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7766  _for_workflow(wf
-0000ac80: 2c20 7375 6273 290a 2020 2020 2020 2020  , subs).        
-0000ac90: 2020 2020 2020 2020 2320 656e 7375 7265          # ensure
-0000aca0: 2061 6c6c 2064 6972 7320 6578 6973 7420   all dirs exist 
-0000acb0: 7265 6d6f 7465 6c79 0a20 2020 2020 2020  remotely.       
-0000acc0: 2020 2020 2020 2020 2066 756c 6c5f 7061           full_pa
-0000acd0: 7468 203d 2073 656c 662e 736c 7572 6d5f  th = self.slurm_
-0000ace0: 7363 7269 7074 5f70 6174 682b 222f 222b  script_path+"/"+
-0000acf0: 6a6f 625f 7061 7468 0a20 2020 2020 2020  job_path.       
-0000ad00: 2020 2020 2020 2020 206a 6f62 5f64 6972           job_dir
-0000ad10: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
-0000ad20: 6c69 7428 6675 6c6c 5f70 6174 6829 0a20  lit(full_path). 
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ad40: 656c 662e 7275 6e28 6622 6d6b 6469 7220  elf.run(f"mkdir 
-0000ad50: 2d70 207b 6a6f 625f 6469 727d 2229 0a20  -p {job_dir}"). 
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ad70: 2063 6f70 7920 746f 2072 656d 6f74 6520   copy to remote 
-0000ad80: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-0000ad90: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-0000ada0: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
-0000adb0: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
-0000adc0: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 2020 2020 2020 2020 7265 6d6f 7465 3d66          remote=f
-0000adf0: 756c 6c5f 7061 7468 290a 2020 2020 2020  ull_path).      
-0000ae00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ae10: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
-0000ae20: 6574 5f75 7064 6174 655f 736c 7572 6d5f  et_update_slurm_
-0000ae30: 7363 7269 7074 735f 636f 6d6d 616e 6428  scripts_command(
-0000ae40: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-0000ae50: 6767 6572 2e69 6e66 6f28 2255 7064 6174  gger.info("Updat
-0000ae60: 696e 6720 536c 7572 6d20 6a6f 6220 7363  ing Slurm job sc
-0000ae70: 7269 7074 7320 6f6e 2053 6c75 726d 2229  ripts on Slurm")
-0000ae80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000ae90: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-0000aea0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
-0000aeb0: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
-0000aec0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0000aed0: 2020 2064 6566 2072 756e 5f77 6f72 6b66     def run_workf
-0000aee0: 6c6f 7728 7365 6c66 2c0a 2020 2020 2020  low(self,.      
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000af00: 6f72 6b66 6c6f 775f 6e61 6d65 3a20 7374  orkflow_name: st
-0000af10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000af20: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000af30: 5f76 6572 7369 6f6e 3a20 7374 722c 0a20  _version: str,. 
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 696e 7075 745f 6461 7461 3a20      input_data: 
-0000af60: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000af70: 2020 2020 2020 2020 2020 656d 6169 6c3a            email:
-0000af80: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000af90: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0000afa0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000afb0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000afc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000afd0: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-0000afe0: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
-0000aff0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-0000b000: 5475 706c 655b 5265 7375 6c74 2c20 696e  Tuple[Result, in
-0000b010: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-0000b020: 2020 2020 2020 2020 5275 6e20 6120 7370          Run a sp
-0000b030: 6563 6966 6965 6420 776f 726b 666c 6f77  ecified workflow
-0000b040: 206f 6e20 536c 7572 6d20 7573 696e 6720   on Slurm using 
-0000b050: 7468 6520 6769 7665 6e20 7061 7261 6d65  the given parame
-0000b060: 7465 7273 2e0a 0a20 2020 2020 2020 2041  ters...        A
-0000b070: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000b080: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
-0000b090: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
-0000b0a0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
-0000b0b0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
-0000b0c0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
-0000b0d0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
-0000b0e0: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
-0000b0f0: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
-0000b100: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
-0000b110: 2020 206f 6e20 536c 7572 6d29 2e0a 2020     on Slurm)..  
-0000b120: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000b130: 6461 7461 2028 7374 7229 3a20 4e61 6d65  data (str): Name
-0000b140: 206f 6620 7468 6520 696e 7075 7420 6461   of the input da
-0000b150: 7461 2066 6f6c 6465 7220 636f 6e74 6169  ta folder contai
-0000b160: 6e69 6e67 2069 6e70 7574 0a20 2020 2020  ning input.     
-0000b170: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0000b180: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
-0000b190: 2020 2020 656d 6169 6c20 2873 7472 2c20      email (str, 
-0000b1a0: 6f70 7469 6f6e 616c 293a 2045 6d61 696c  optional): Email
-0000b1b0: 2061 6464 7265 7373 2066 6f72 2053 6c75   address for Slu
-0000b1c0: 726d 206a 6f62 206e 6f74 6966 6963 6174  rm job notificat
-0000b1d0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000b1e0: 2020 7469 6d65 2028 7374 722c 206f 7074    time (str, opt
-0000b1f0: 696f 6e61 6c29 3a20 5469 6d65 206c 696d  ional): Time lim
-0000b200: 6974 2066 6f72 2074 6865 2053 6c75 726d  it for the Slurm
-0000b210: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
-0000b220: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000b230: 6d61 7420 4848 3a4d 4d3a 5353 2e0a 2020  mat HH:MM:SS..  
-0000b240: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000b250: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
-0000b260: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000b270: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
-0000b280: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
-0000b290: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000b2a0: 2054 7570 6c65 5b52 6573 756c 742c 2069   Tuple[Result, i
-0000b2b0: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
-0000b2c0: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
-0000b2d0: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
-0000b2e0: 6c74 206f 6620 7374 6172 7469 6e67 2074  lt of starting t
-0000b2f0: 6865 2077 6f72 6b66 6c6f 7720 6a6f 6220  he workflow job 
-0000b300: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-0000b310: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
-0000b320: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
-0000b330: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
-0000b340: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
-0000b350: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
-0000b360: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0000b370: 2053 6c75 726d 206a 6f62 2049 4420 6973   Slurm job ID is
-0000b380: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
-0000b390: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
-0000b3a0: 6520 0a20 2020 2020 2020 2020 2020 2060  e .            `
-0000b3b0: 7275 6e5f 636f 6d6d 616e 6473 6020 6d65  run_commands` me
-0000b3c0: 7468 6f64 2e0a 2020 2020 2020 2020 2222  thod..        ""
-0000b3d0: 220a 2020 2020 2020 2020 7362 6174 6368  ".        sbatch
-0000b3e0: 5f63 6d64 2c20 7362 6174 6368 5f65 6e76  _cmd, sbatch_env
-0000b3f0: 203d 2073 656c 662e 6765 745f 776f 726b   = self.get_work
-0000b400: 666c 6f77 5f63 6f6d 6d61 6e64 280a 2020  flow_command(.  
-0000b410: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000b420: 6f77 5f6e 616d 652c 2077 6f72 6b66 6c6f  ow_name, workflo
-0000b430: 775f 7665 7273 696f 6e2c 2069 6e70 7574  w_version, input
-0000b440: 5f64 6174 612c 2065 6d61 696c 2c20 7469  _data, email, ti
-0000b450: 6d65 2c20 2a2a 6b77 6172 6773 290a 2020  me, **kwargs).  
-0000b460: 2020 2020 2020 7072 696e 7428 6622 5275        print(f"Ru
-0000b470: 6e6e 696e 6720 7b77 6f72 6b66 6c6f 775f  nning {workflow_
-0000b480: 6e61 6d65 7d20 6a6f 6220 6f6e 207b 696e  name} job on {in
-0000b490: 7075 745f 6461 7461 7d20 6f6e 2053 6c75  put_data} on Slu
-0000b4a0: 726d 3a5c 0a20 2020 2020 2020 2020 2020  rm:\.           
-0000b4b0: 207b 7362 6174 6368 5f63 6d64 7d20 772f   {sbatch_cmd} w/
-0000b4c0: 207b 7362 6174 6368 5f65 6e76 7d22 290a   {sbatch_env}").
-0000b4d0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-0000b4e0: 6e66 6f28 6622 5275 6e6e 696e 6720 7b77  nfo(f"Running {w
-0000b4f0: 6f72 6b66 6c6f 775f 6e61 6d65 7d20 6a6f  orkflow_name} jo
-0000b500: 6220 6f6e 207b 696e 7075 745f 6461 7461  b on {input_data
-0000b510: 7d20 6f6e 2053 6c75 726d 2229 0a20 2020  } on Slurm").   
-0000b520: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-0000b530: 7275 6e5f 636f 6d6d 616e 6473 285b 7362  run_commands([sb
-0000b540: 6174 6368 5f63 6d64 5d2c 2073 6261 7463  atch_cmd], sbatc
-0000b550: 685f 656e 7629 0a20 2020 2020 2020 2072  h_env).        r
-0000b560: 6574 7572 6e20 7265 732c 2073 656c 662e  eturn res, self.
-0000b570: 6578 7472 6163 745f 6a6f 625f 6964 2872  extract_job_id(r
-0000b580: 6573 290a 0a20 2020 2064 6566 2072 756e  es)..    def run
-0000b590: 5f77 6f72 6b66 6c6f 775f 6a6f 6228 7365  _workflow_job(se
-0000b5a0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000b5b0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000b5c0: 6b66 6c6f 775f 6e61 6d65 3a20 7374 722c  kflow_name: str,
-0000b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b5e0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000b5f0: 6f77 5f76 6572 7369 6f6e 3a20 7374 722c  ow_version: str,
-0000b600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b610: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000b620: 6461 7461 3a20 7374 722c 0a20 2020 2020  data: str,.     
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 656d 6169 6c3a 204f 7074 696f      email: Optio
-0000b650: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000b660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b670: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
-0000b680: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000b690: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000b6b0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
-0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 2029 202d 3e20 536c 7572 6d4a 6f62 3a0a   ) -> SlurmJob:.
-0000b6e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b6f0: 2020 2020 5275 6e20 6120 7370 6563 6966      Run a specif
-0000b700: 6965 6420 776f 726b 666c 6f77 206f 6e20  ied workflow on 
-0000b710: 536c 7572 6d20 7573 696e 6720 7468 6520  Slurm using the 
-0000b720: 6769 7665 6e20 7061 7261 6d65 7465 7273  given parameters
-0000b730: 2061 6e64 2072 6574 7572 6e20 6120 536c   and return a Sl
-0000b740: 7572 6d4a 6f62 2069 6e73 7461 6e63 652e  urmJob instance.
-0000b750: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000b760: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000b770: 666c 6f77 5f6e 616d 6520 2873 7472 293a  flow_name (str):
-0000b780: 204e 616d 6520 6f66 2074 6865 2077 6f72   Name of the wor
-0000b790: 6b66 6c6f 7720 746f 2065 7865 6375 7465  kflow to execute
-0000b7a0: 2e0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
-0000b7b0: 726b 666c 6f77 5f76 6572 7369 6f6e 2028  rkflow_version (
-0000b7c0: 7374 7229 3a20 5665 7273 696f 6e20 6f66  str): Version of
-0000b7d0: 2074 6865 2077 6f72 6b66 6c6f 7720 2869   the workflow (i
-0000b7e0: 6d61 6765 2076 6572 7369 6f6e 206f 6e20  mage version on 
-0000b7f0: 536c 7572 6d29 2e0a 2020 2020 2020 2020  Slurm)..        
-0000b800: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
-0000b810: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
-0000b820: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
-0000b830: 6465 7220 636f 6e74 6169 6e69 6e67 2069  der containing i
-0000b840: 6e70 7574 2069 6d61 6765 2066 696c 6573  nput image files
-0000b850: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
-0000b860: 6169 6c20 2873 7472 2c20 6f70 7469 6f6e  ail (str, option
-0000b870: 616c 293a 2045 6d61 696c 2061 6464 7265  al): Email addre
-0000b880: 7373 2066 6f72 2053 6c75 726d 206a 6f62  ss for Slurm job
-0000b890: 206e 6f74 6966 6963 6174 696f 6e73 2e0a   notifications..
-0000b8a0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000b8b0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0000b8c0: 3a20 5469 6d65 206c 696d 6974 2066 6f72  : Time limit for
-0000b8d0: 2074 6865 2053 6c75 726d 206a 6f62 2069   the Slurm job i
-0000b8e0: 6e20 7468 6520 666f 726d 6174 2048 483a  n the format HH:
-0000b8f0: 4d4d 3a53 532e 0a20 2020 2020 2020 2020  MM:SS..         
-0000b900: 2020 202a 2a6b 7761 7267 733a 2041 6464     **kwargs: Add
-0000b910: 6974 696f 6e61 6c20 6b65 7977 6f72 6420  itional keyword 
-0000b920: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
-0000b930: 6520 776f 726b 666c 6f77 2e0a 0a20 2020  e workflow...   
-0000b940: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000b950: 2020 2020 2020 2020 2020 536c 7572 6d4a            SlurmJ
-0000b960: 6f62 3a20 4120 536c 7572 6d4a 6f62 2069  ob: A SlurmJob i
-0000b970: 6e73 7461 6e63 6520 7265 7072 6573 656e  nstance represen
-0000b980: 7469 6e67 2074 6865 2073 7461 7274 6564  ting the started
-0000b990: 2077 6f72 6b66 6c6f 7720 6a6f 622e 0a20   workflow job.. 
-0000b9a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000b9b0: 2020 2072 6573 756c 742c 206a 6f62 5f69     result, job_i
-0000b9c0: 6420 3d20 7365 6c66 2e72 756e 5f77 6f72  d = self.run_wor
-0000b9d0: 6b66 6c6f 7728 0a20 2020 2020 2020 2020  kflow(.         
-0000b9e0: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
-0000b9f0: 2c20 776f 726b 666c 6f77 5f76 6572 7369  , workflow_versi
-0000ba00: 6f6e 2c20 696e 7075 745f 6461 7461 2c20  on, input_data, 
-0000ba10: 656d 6169 6c2c 2074 696d 652c 202a 2a6b  email, time, **k
-0000ba20: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
-0000ba30: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
-0000ba40: 6573 756c 742c 206a 6f62 5f69 6429 0a0a  esult, job_id)..
-0000ba50: 2020 2020 6465 6620 7275 6e5f 636f 6e76      def run_conv
-0000ba60: 6572 7369 6f6e 5f77 6f72 6b66 6c6f 775f  ersion_workflow_
-0000ba70: 6a6f 6228 7365 6c66 2c20 666f 6c64 6572  job(self, folder
-0000ba80: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bab0: 736f 7572 6365 5f66 6f72 6d61 743a 2073  source_format: s
-0000bac0: 7472 203d 2027 7a61 7272 272c 0a20 2020  tr = 'zarr',.   
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baf0: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
-0000bb00: 7374 7220 3d20 2774 6966 6627 0a20 2020  str = 'tiff'.   
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2029 202d 3e20 5475 706c 655b 5265 7375   ) -> Tuple[Resu
-0000bb40: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
-0000bb50: 2020 2222 220a 2020 2020 2020 2020 5275    """.        Ru
-0000bb60: 6e20 7468 6520 6461 7461 2063 6f6e 7665  n the data conve
-0000bb70: 7273 696f 6e20 776f 726b 666c 6f77 206f  rsion workflow o
-0000bb80: 6e20 536c 7572 6d20 7573 696e 6720 7468  n Slurm using th
-0000bb90: 6520 6769 7665 6e20 6461 7461 2066 6f6c  e given data fol
-0000bba0: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
-0000bbb0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000bbc0: 666f 6c64 6572 5f6e 616d 6520 2873 7472  folder_name (str
-0000bbd0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
-0000bbe0: 6865 2064 6174 6120 666f 6c64 6572 2063  he data folder c
-0000bbf0: 6f6e 7461 696e 696e 6720 736f 7572 6365  ontaining source
-0000bc00: 2066 6f72 6d61 7420 6669 6c65 732e 0a20   format files.. 
-0000bc10: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0000bc20: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
-0000bc30: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
-0000bc40: 6174 2066 6f72 2063 6f6e 7665 7273 696f  at for conversio
-0000bc50: 6e20 2864 6566 6175 6c74 2069 7320 277a  n (default is 'z
-0000bc60: 6172 7227 292e 0a20 2020 2020 2020 2020  arr')..         
-0000bc70: 2020 2074 6172 6765 745f 666f 726d 6174     target_format
-0000bc80: 2028 7374 7229 3a20 5461 7267 6574 2064   (str): Target d
-0000bc90: 6174 6120 666f 726d 6174 2061 6674 6572  ata format after
-0000bca0: 2063 6f6e 7665 7273 696f 6e20 2864 6566   conversion (def
-0000bcb0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
-0000bcc0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000bcd0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0000bce0: 7570 6c65 5b52 6573 756c 742c 2069 6e74  uple[Result, int
-0000bcf0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000bd00: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-0000bd10: 696e 696e 6720 7468 6520 7265 7375 6c74  ining the result
-0000bd20: 206f 6620 7374 6172 7469 6e67 2074 6865   of starting the
-0000bd30: 2063 6f6e 7665 7273 696f 6e20 6a6f 6220   conversion job 
-0000bd40: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-0000bd50: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
-0000bd60: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
-0000bd70: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
-0000bd80: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
-0000bd90: 2e0a 0a20 2020 2020 2020 2057 6172 6e69  ...        Warni
-0000bda0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-0000bdb0: 5468 6520 6465 6661 756c 7420 696d 706c  The default impl
-0000bdc0: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
-0000bdd0: 7375 7070 6f72 7473 2063 6f6e 7665 7273  supports convers
-0000bde0: 696f 6e20 6672 6f6d 2027 7a61 7272 2720  ion from 'zarr' 
-0000bdf0: 746f 2027 7469 6666 272e 0a20 2020 2020  to 'tiff'..     
-0000be00: 2020 2020 2020 2049 6620 7573 696e 6720         If using 
-0000be10: 6f74 6865 7220 736f 7572 6365 206f 7220  other source or 
-0000be20: 7461 7267 6574 2066 6f72 6d61 7473 2c20  target formats, 
-0000be30: 7573 6572 7320 6d75 7374 2069 6d70 6c65  users must imple
-0000be40: 6d65 6e74 2061 6e64 2063 6f6e 6669 6775  ment and configu
-0000be50: 7265 0a20 2020 2020 2020 2020 2020 2061  re.            a
-0000be60: 6464 6974 696f 6e61 6c20 636f 6e76 6572  dditional conver
-0000be70: 7465 7273 2074 6865 6d73 656c 7665 732e  ters themselves.
-0000be80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000be90: 2020 2020 2023 2047 656e 6572 6174 6520       # Generate 
-0000bea0: 6120 756e 6971 7565 2063 6f6e 6669 6720  a unique config 
-0000beb0: 6669 6c65 206e 616d 650a 2020 2020 2020  file name.      
-0000bec0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
-0000bed0: 6622 636f 6e66 6967 5f7b 666f 6c64 6572  f"config_{folder
-0000bee0: 5f6e 616d 657d 2e74 7874 220a 0a20 2020  _name}.txt"..   
-0000bef0: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
-0000bf00: 2061 6c6c 2063 6f6d 6d61 6e64 7320 746f   all commands to
-0000bf10: 2072 756e 2063 6f6e 7365 6375 7469 7665   run consecutive
-0000bf20: 6c79 0a20 2020 2020 2020 2064 6174 615f  ly.        data_
-0000bf30: 7061 7468 203d 2066 227b 7365 6c66 2e73  path = f"{self.s
-0000bf40: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
-0000bf50: 7b66 6f6c 6465 725f 6e61 6d65 7d22 0a20  {folder_name}". 
-0000bf60: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
-0000bf70: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
-0000bf80: 7620 3d20 7365 6c66 2e67 6574 5f63 6f6e  v = self.get_con
-0000bf90: 7665 7273 696f 6e5f 636f 6d6d 616e 6428  version_command(
-0000bfa0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000bfb0: 615f 7061 7468 2c20 636f 6e66 6967 5f66  a_path, config_f
-0000bfc0: 696c 652c 2073 6f75 7263 655f 666f 726d  ile, source_form
-0000bfd0: 6174 2c20 7461 7267 6574 5f66 6f72 6d61  at, target_forma
-0000bfe0: 7429 0a20 2020 2020 2020 2063 6f6d 6d61  t).        comma
-0000bff0: 6e64 7320 3d20 5b0a 2020 2020 2020 2020  nds = [.        
-0000c000: 2020 2020 6622 6669 6e64 207b 6461 7461      f"find {data
-0000c010: 5f70 6174 687d 2f64 6174 612f 696e 202d  _path}/data/in -
-0000c020: 6e61 6d65 2027 2a2e 7b73 6f75 7263 655f  name '*.{source_
-0000c030: 666f 726d 6174 7d27 207c 2061 776b 2027  format}' | awk '
-0000c040: 7b7b 7072 696e 7420 4e52 2c20 2430 7d7d  {{print NR, $0}}
-0000c050: 2720 3e20 7b63 6f6e 6669 675f 6669 6c65  ' > {config_file
-0000c060: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-0000c070: 6622 4e3d 2428 7763 202d 6c20 3c20 5c22  f"N=$(wc -l < \"
-0000c080: 7b63 6f6e 6669 675f 6669 6c65 7d5c 2229  {config_file}\")
-0000c090: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
-0000c0a0: 2265 6368 6f20 5c22 4e75 6d62 6572 206f  "echo \"Number o
-0000c0b0: 6620 2e7b 736f 7572 6365 5f66 6f72 6d61  f .{source_forma
-0000c0c0: 747d 2066 696c 6573 3a20 244e 5c22 222c  t} files: $N\"",
-0000c0d0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000c0e0: 7665 7273 696f 6e5f 636d 640a 2020 2020  version_cmd.    
-0000c0f0: 2020 2020 5d0a 0a20 2020 2020 2020 2023      ]..        #
-0000c100: 2052 756e 2061 6c6c 2063 6f6d 6d61 6e64   Run all command
-0000c110: 7320 636f 6e73 6563 7574 6976 656c 790a  s consecutively.
-0000c120: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-0000c130: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
-0000c140: 636f 6d6d 616e 6473 2c20 7362 6174 6368  commands, sbatch
-0000c150: 5f65 6e76 290a 0a20 2020 2020 2020 2072  _env)..        r
-0000c160: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
-0000c170: 6573 2c20 7365 6c66 2e65 7874 7261 6374  es, self.extract
-0000c180: 5f6a 6f62 5f69 6428 7265 7329 290a 0a20  _job_id(res)).. 
-0000c190: 2020 2064 6566 2065 7874 7261 6374 5f6a     def extract_j
-0000c1a0: 6f62 5f69 6428 7365 6c66 2c20 7265 7375  ob_id(self, resu
-0000c1b0: 6c74 3a20 5265 7375 6c74 2920 2d3e 2069  lt: Result) -> i
-0000c1c0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-0000c1d0: 2020 2020 2020 2020 4578 7472 6163 7420          Extract 
-0000c1e0: 7468 6520 536c 7572 6d20 6a6f 6220 4944  the Slurm job ID
-0000c1f0: 2066 726f 6d20 7468 6520 7265 7375 6c74   from the result
-0000c200: 206f 6620 6120 636f 6d6d 616e 642e 0a0a   of a command...
-0000c210: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c220: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000c230: 2028 5265 7375 6c74 293a 2054 6865 2072   (Result): The r
-0000c240: 6573 756c 7420 6f66 2061 2063 6f6d 6d61  esult of a comma
-0000c250: 6e64 2065 7865 6375 7469 6f6e 2e0a 0a20  nd execution... 
-0000c260: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000c270: 2020 2020 2020 2020 2020 2020 696e 743a              int:
-0000c280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c290: 2054 6865 2053 6c75 726d 206a 6f62 2049   The Slurm job I
-0000c2a0: 4420 6578 7472 6163 7465 6420 6672 6f6d  D extracted from
-0000c2b0: 2074 6865 2072 6573 756c 742c 0a20 2020   the result,.   
-0000c2c0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000c2d0: 2d31 2069 6620 6e6f 7420 666f 756e 642e  -1 if not found.
-0000c2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c2f0: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-0000c300: 6420 3d20 6e65 7874 2828 696e 7428 732e  d = next((int(s.
-0000c310: 7374 7269 7028 2929 2066 6f72 2073 2069  strip()) for s i
-0000c320: 6e20 7265 7375 6c74 2e73 7464 6f75 742e  n result.stdout.
-0000c330: 7370 6c69 7428 0a20 2020 2020 2020 2020  split(.         
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 2020 2022 5375 626d 6974 7465 6420 6261     "Submitted ba
-0000c360: 7463 6820 6a6f 6222 2920 6966 2073 2e73  tch job") if s.s
-0000c370: 7472 6970 2829 2e69 7364 6967 6974 2829  trip().isdigit()
-0000c380: 292c 202d 3129 0a20 2020 2020 2020 2072  ), -1).        r
-0000c390: 6574 7572 6e20 736c 7572 6d5f 6a6f 625f  eturn slurm_job_
-0000c3a0: 6964 0a0a 2020 2020 6465 6620 6765 745f  id..    def get_
-0000c3b0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
-0000c3c0: 6970 7473 5f63 6f6d 6d61 6e64 2873 656c  ipts_command(sel
-0000c3d0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-0000c3e0: 2020 2022 2222 4765 6e65 7261 7465 2074     """Generate t
-0000c3f0: 6865 2063 6f6d 6d61 6e64 2074 6f20 7570  he command to up
-0000c400: 6461 7465 2074 6865 2047 6974 2072 6570  date the Git rep
-0000c410: 6f73 6974 6f72 7920 636f 6e74 6169 6e69  ository containi
-0000c420: 6e67 0a20 2020 2020 2020 2074 6865 2053  ng.        the S
-0000c430: 6c75 726d 2073 6372 6970 7473 2c20 6966  lurm scripts, if
-0000c440: 206e 6563 6573 7361 7279 2e0a 0a20 2020   necessary...   
-0000c450: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000c460: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0000c480: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
-0000c490: 6e67 2074 6865 2047 6974 2063 6f6d 6d61  ng the Git comma
-0000c4a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-0000c4b0: 2020 2074 6f20 7570 6461 7465 2074 6865     to update the
-0000c4c0: 2053 6c75 726d 2073 6372 6970 7473 2e0a   Slurm scripts..
-0000c4d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c4e0: 2020 2020 7570 6461 7465 5f63 6d64 203d      update_cmd =
-0000c4f0: 2066 2267 6974 202d 4320 7b73 656c 662e   f"git -C {self.
-0000c500: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
-0000c510: 687d 2070 756c 6c22 0a20 2020 2020 2020  h} pull".       
-0000c520: 2072 6574 7572 6e20 7570 6461 7465 5f63   return update_c
-0000c530: 6d64 0a0a 2020 2020 6465 6620 6368 6563  md..    def chec
-0000c540: 6b5f 6a6f 625f 7374 6174 7573 2873 656c  k_job_status(sel
-0000c550: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-0000c560: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-0000c570: 6d5f 6a6f 625f 6964 733a 204c 6973 745b  m_job_ids: List[
-0000c580: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c5a0: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
-0000c5b0: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
-0000c5c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000c5d0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-0000c5e0: 3e20 5475 706c 655b 4469 6374 5b69 6e74  > Tuple[Dict[int
-0000c5f0: 2c20 7374 725d 2c20 5265 7375 6c74 5d3a  , str], Result]:
-0000c600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c610: 2020 2020 2043 6865 636b 2074 6865 2073       Check the s
-0000c620: 7461 7475 7320 6f66 2053 6c75 726d 206a  tatus of Slurm j
-0000c630: 6f62 7320 7769 7468 2074 6865 2067 6976  obs with the giv
-0000c640: 656e 206a 6f62 2049 4473 2e0a 0a20 2020  en job IDs...   
-0000c650: 2020 2020 204e 6f74 653a 2054 6869 7320       Note: This 
-0000c660: 646f 6573 6e27 7420 7265 7475 726e 206a  doesn't return j
-0000c670: 6f62 2061 7272 6179 7320 696e 6469 7669  ob arrays indivi
-0000c680: 6475 616c 6c79 2e0a 2020 2020 2020 2020  dually..        
-0000c690: 4974 2074 616b 6573 2074 6865 206c 6173  It takes the las
-0000c6a0: 7420 7661 6c75 6520 7265 7475 726e 6564  t value returned
-0000c6b0: 2066 6f72 2074 686f 7365 2073 7562 2069   for those sub i
-0000c6c0: 6473 200a 2020 2020 2020 2020 2867 656e  ds .        (gen
-0000c6d0: 6572 616c 6c79 2074 6865 206f 6e65 2073  erally the one s
-0000c6e0: 7469 6c6c 2050 454e 4449 4e47 292e 0a0a  till PENDING)...
-0000c6f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c700: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-0000c710: 6a6f 625f 6964 7320 284c 6973 745b 696e  job_ids (List[in
-0000c720: 745d 293a 2054 6865 206a 6f62 2049 4473  t]): The job IDs
-0000c730: 206f 6620 7468 6520 536c 7572 6d20 6a6f   of the Slurm jo
-0000c740: 6273 2074 6f20 6368 6563 6b2e 0a20 2020  bs to check..   
-0000c750: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-0000c760: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-0000c770: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-0000c780: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-0000c790: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
-0000c7a0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
-0000c7b0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
-0000c7c0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
-0000c7d0: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
-0000c7e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000c7f0: 2020 2020 2020 2020 2054 7570 6c65 5b44           Tuple[D
-0000c800: 6963 745b 696e 742c 2073 7472 5d2c 2052  ict[int, str], R
-0000c810: 6573 756c 745d 3a0a 2020 2020 2020 2020  esult]:.        
-0000c820: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
-0000c830: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
-0000c840: 7461 7475 7320 7065 7220 696e 7075 7420  tatus per input 
-0000c850: 4944 2061 6e64 2074 6865 2072 6573 756c  ID and the resul
-0000c860: 7420 6f66 200a 2020 2020 2020 2020 2020  t of .          
-0000c870: 2020 2020 2020 7468 6520 636f 6d6d 616e        the comman
-0000c880: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
-0000c890: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-0000c8a0: 2020 2020 2020 2020 2020 5353 4845 7863            SSHExc
-0000c8b0: 6570 7469 6f6e 3a20 4966 2074 6865 2063  eption: If the c
-0000c8c0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
-0000c8d0: 2066 6169 6c73 206f 7220 6e6f 2072 6573   fails or no res
-0000c8e0: 706f 6e73 6520 6973 0a20 2020 2020 2020  ponse is.       
-0000c8f0: 2020 2020 2020 2020 2072 6563 6569 7665           receive
-0000c900: 6420 6166 7465 7220 6d75 6c74 6970 6c65  d after multiple
-0000c910: 2072 6574 7269 6573 2e0a 2020 2020 2020   retries..      
-0000c920: 2020 2222 220a 2020 2020 2020 2020 636d    """.        cm
-0000c930: 6420 3d20 7365 6c66 2e67 6574 5f6a 6f62  d = self.get_job
-0000c940: 5f73 7461 7475 735f 636f 6d6d 616e 6428  _status_command(
-0000c950: 736c 7572 6d5f 6a6f 625f 6964 7329 0a20  slurm_job_ids). 
-0000c960: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000c970: 666f 2866 2247 6574 7469 6e67 2073 7461  fo(f"Getting sta
-0000c980: 7475 7320 6f66 207b 736c 7572 6d5f 6a6f  tus of {slurm_jo
-0000c990: 625f 6964 737d 206f 6e20 536c 7572 6d22  b_ids} on Slurm"
-0000c9a0: 290a 2020 2020 2020 2020 7265 7472 795f  ).        retry_
-0000c9b0: 7374 6174 7573 203d 2030 0a20 2020 2020  status = 0.     
-0000c9c0: 2020 2077 6869 6c65 2072 6574 7279 5f73     while retry_s
-0000c9d0: 7461 7475 7320 3c20 333a 0a20 2020 2020  tatus < 3:.     
-0000c9e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000c9f0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000ca00: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
-0000ca10: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-0000ca20: 6767 6572 2e69 6e66 6f28 7265 7375 6c74  gger.info(result
-0000ca30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000ca40: 2072 6573 756c 742e 6f6b 3a0a 2020 2020   result.ok:.    
-0000ca50: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000ca60: 6f74 2072 6573 756c 742e 7374 646f 7574  ot result.stdout
-0000ca70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ca80: 2020 2020 2020 2320 7761 6974 2066 6f72        # wait for
-0000ca90: 2033 2073 6563 6f6e 6473 2062 6566 6f72   3 seconds befor
-0000caa0: 6520 6368 6563 6b69 6e67 2061 6761 696e  e checking again
-0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cac0: 2020 2020 2074 696d 6573 6c65 6570 2e73       timesleep.s
-0000cad0: 6c65 6570 2833 290a 2020 2020 2020 2020  leep(3).        
-0000cae0: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-0000caf0: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
-0000cb00: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
-0000cb10: 6174 7573 202b 3d20 310a 2020 2020 2020  atus += 1.      
-0000cb20: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000cb30: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb50: 2020 2020 6622 5265 7472 7920 7b72 6574      f"Retry {ret
-0000cb60: 7279 5f73 7461 7475 737d 2067 6574 7469  ry_status} getti
-0000cb70: 6e67 2073 7461 7475 7320 5c0a 2020 2020  ng status \.    
-0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb90: 2020 2020 2020 2020 6f66 207b 736c 7572          of {slur
-0000cba0: 6d5f 6a6f 625f 6964 737d 2122 290a 2020  m_job_ids}!").  
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000cbc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cbd0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0000cbe0: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000cbf0: 625f 7374 6174 7573 5f64 6963 7420 3d20  b_status_dict = 
-0000cc00: 7b69 6e74 286c 696e 652e 7370 6c69 7428  {int(line.split(
-0000cc10: 295b 305d 2e73 706c 6974 2827 5f27 295b  )[0].split('_')[
-0000cc20: 305d 293a 206c 696e 652e 7370 6c69 7428  0]): line.split(
-0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc40: 2020 2020 2029 5b31 5d20 666f 7220 6c69       )[1] for li
-0000cc50: 6e65 2069 6e20 7265 7375 6c74 2e73 7464  ne in result.std
-0000cc60: 6f75 742e 7370 6c69 7428 225c 6e22 2920  out.split("\n") 
-0000cc70: 6966 206c 696e 657d 0a20 2020 2020 2020  if line}.       
-0000cc80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000cc90: 6765 722e 6465 6275 6728 6622 4a6f 6220  ger.debug(f"Job 
-0000cca0: 7374 6174 7573 6573 3a20 7b6a 6f62 5f73  statuses: {job_s
-0000ccb0: 7461 7475 735f 6469 6374 7d22 290a 2020  tatus_dict}").  
-0000ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccd0: 2020 7265 7475 726e 206a 6f62 5f73 7461    return job_sta
-0000cce0: 7475 735f 6469 6374 2c20 7265 7375 6c74  tus_dict, result
-0000ccf0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000cd00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000cd10: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
-0000cd20: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
-0000cd30: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
-0000cd40: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000cd50: 6572 726f 7228 6572 726f 7229 0a20 2020  error(error).   
-0000cd60: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000cd70: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
-0000cd80: 6572 726f 7229 0a20 2020 2020 2020 2065  error).        e
-0000cd90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cda0: 2065 7272 6f72 203d 2066 2245 7272 6f72   error = f"Error
-0000cdb0: 3a20 5265 7472 6965 6420 7b72 6574 7279  : Retried {retry
-0000cdc0: 5f73 7461 7475 737d 2074 696d 6573 2074  _status} times t
-0000cdd0: 6f20 6765 7420 5c0a 2020 2020 2020 2020  o get \.        
-0000cde0: 2020 2020 2020 2020 7374 6174 7573 206f          status o
-0000cdf0: 6620 7b73 6c75 726d 5f6a 6f62 5f69 6473  f {slurm_job_ids
-0000ce00: 7d2c 2062 7574 206e 6f20 7265 7370 6f6e  }, but no respon
-0000ce10: 7365 2e22 0a20 2020 2020 2020 2020 2020  se.".           
-0000ce20: 206c 6f67 6765 722e 6572 726f 7228 6572   logger.error(er
-0000ce30: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
-0000ce40: 2072 6169 7365 2053 5348 4578 6365 7074   raise SSHExcept
-0000ce50: 696f 6e28 6572 726f 7229 0a0a 2020 2020  ion(error)..    
-0000ce60: 6465 6620 6765 745f 6a6f 625f 7374 6174  def get_job_stat
-0000ce70: 7573 5f63 6f6d 6d61 6e64 2873 656c 662c  us_command(self,
-0000ce80: 2073 6c75 726d 5f6a 6f62 5f69 6473 3a20   slurm_job_ids: 
-0000ce90: 4c69 7374 5b69 6e74 5d29 202d 3e20 7374  List[int]) -> st
-0000cea0: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
-0000ceb0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0000cec0: 6520 536c 7572 6d20 636f 6d6d 616e 6420  e Slurm command 
-0000ced0: 746f 2067 6574 2074 6865 2073 7461 7475  to get the statu
-0000cee0: 7320 6f66 206a 6f62 7320 7769 7468 2074  s of jobs with t
-0000cef0: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
-0000cf00: 206a 6f62 2049 4473 2e0a 0a20 2020 2020   job IDs...     
-0000cf10: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000cf20: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-0000cf30: 6473 2028 4c69 7374 5b69 6e74 5d29 3a20  ds (List[int]): 
-0000cf40: 5468 6520 6a6f 6220 4944 7320 6f66 2074  The job IDs of t
-0000cf50: 6865 206a 6f62 7320 746f 2063 6865 636b  he jobs to check
-0000cf60: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000cf70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000cf80: 7374 723a 200a 2020 2020 2020 2020 2020  str: .          
-0000cf90: 2020 2020 2020 5468 6520 536c 7572 6d20        The Slurm 
-0000cfa0: 636f 6d6d 616e 6420 746f 2067 6574 2074  command to get t
-0000cfb0: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
-0000cfc0: 206a 6f62 732e 0a20 2020 2020 2020 2022   jobs..        "
-0000cfd0: 2222 0a20 2020 2020 2020 2023 2063 6f6e  "".        # con
-0000cfe0: 6361 7420 6d75 6c74 6970 6c65 206a 6f62  cat multiple job
-0000cff0: 7320 6966 206e 6565 6465 640a 2020 2020  s if needed.    
-0000d000: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
-0000d010: 203d 2022 202d 6a20 222e 6a6f 696e 285b   = " -j ".join([
-0000d020: 7374 7228 6964 2920 666f 7220 6964 2069  str(id) for id i
-0000d030: 6e20 736c 7572 6d5f 6a6f 625f 6964 735d  n slurm_job_ids]
-0000d040: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d050: 2073 656c 662e 5f4a 4f42 5f53 5441 5455   self._JOB_STATU
-0000d060: 535f 434d 442e 666f 726d 6174 2873 6c75  S_CMD.format(slu
-0000d070: 726d 5f6a 6f62 5f69 643d 736c 7572 6d5f  rm_job_id=slurm_
-0000d080: 6a6f 625f 6964 290a 0a20 2020 2064 6566  job_id)..    def
-0000d090: 2065 7874 7261 6374 5f64 6174 615f 6c6f   extract_data_lo
-0000d0a0: 6361 7469 6f6e 5f66 726f 6d5f 6c6f 6728  cation_from_log(
-0000d0b0: 7365 6c66 2c20 736c 7572 6d5f 6a6f 625f  self, slurm_job_
-0000d0c0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 2020 2020 2020 206c 6f67 6669 6c65 3a20         logfile: 
-0000d100: 7374 7220 3d20 4e6f 6e65 2920 2d3e 2073  str = None) -> s
-0000d110: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
-0000d120: 6561 6420 534c 5552 4d20 6a6f 6220 6c6f  ead SLURM job lo
-0000d130: 6766 696c 6520 746f 2066 696e 6420 6c6f  gfile to find lo
-0000d140: 6361 7469 6f6e 206f 6620 7468 6520 6461  cation of the da
-0000d150: 7461 2e0a 0a20 2020 2020 2020 204f 6e65  ta...        One
-0000d160: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
-0000d170: 7273 2069 7320 7265 7175 6972 6564 2c20  rs is required, 
-0000d180: 6569 7468 6572 2069 6420 6f72 2066 696c  either id or fil
-0000d190: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-0000d1a0: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
-0000d1b0: 7572 6d5f 6a6f 625f 6964 2028 7374 7229  urm_job_id (str)
-0000d1c0: 3a20 4964 206f 6620 7468 6520 736c 7572  : Id of the slur
-0000d1d0: 6d20 6a6f 620a 2020 2020 2020 2020 2020  m job.          
-0000d1e0: 2020 6c6f 6766 696c 6520 2873 7472 293a    logfile (str):
-0000d1f0: 2050 6174 6820 746f 2074 6865 206c 6f67   Path to the log
-0000d200: 6669 6c65 0a0a 2020 2020 2020 2020 5265  file..        Re
-0000d210: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000d220: 2020 2073 7472 3a20 4461 7461 206c 6f63     str: Data loc
-0000d230: 6174 696f 6e20 6163 636f 7264 696e 6720  ation according 
-0000d240: 746f 2074 6865 206c 6f67 0a0a 2020 2020  to the log..    
-0000d250: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-0000d260: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
-0000d270: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
-0000d280: 7320 616e 2069 7373 7565 2077 6974 6820  s an issue with 
-0000d290: 7468 6520 636f 6d6d 616e 6420 6578 6563  the command exec
-0000d2a0: 7574 696f 6e2e 0a20 2020 2020 2020 2022  ution..        "
-0000d2b0: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
-0000d2c0: 6766 696c 6520 6973 204e 6f6e 6520 616e  gfile is None an
-0000d2d0: 6420 736c 7572 6d5f 6a6f 625f 6964 2069  d slurm_job_id i
-0000d2e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000d2f0: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
-0000d300: 3d20 7365 6c66 2e5f 4c4f 4746 494c 450a  = self._LOGFILE.
-0000d310: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
-0000d320: 696c 6520 3d20 6c6f 6766 696c 652e 666f  ile = logfile.fo
-0000d330: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
-0000d340: 643d 736c 7572 6d5f 6a6f 625f 6964 290a  d=slurm_job_id).
-0000d350: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-0000d360: 6c66 2e5f 4c4f 4746 494c 455f 4441 5441  lf._LOGFILE_DATA
-0000d370: 5f43 4d44 2e66 6f72 6d61 7428 6c6f 675f  _CMD.format(log_
-0000d380: 6669 6c65 3d6c 6f67 6669 6c65 290a 2020  file=logfile).  
-0000d390: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-0000d3a0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-0000d3b0: 285b 636d 645d 290a 2020 2020 2020 2020  ([cmd]).        
-0000d3c0: 6966 2072 6573 756c 742e 6f6b 3a0a 2020  if result.ok:.  
-0000d3d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d3e0: 2072 6573 756c 742e 7374 646f 7574 0a20   result.stdout. 
-0000d3f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000d400: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000d410: 5348 4578 6365 7074 696f 6e28 7265 7375  SHException(resu
-0000d420: 6c74 290a 0a20 2020 2064 6566 2067 6574  lt)..    def get
-0000d430: 5f77 6f72 6b66 6c6f 775f 7061 7261 6d65  _workflow_parame
-0000d440: 7465 7273 2873 656c 662c 0a20 2020 2020  ters(self,.     
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000d470: 6c6f 773a 2073 7472 2920 2d3e 2044 6963  low: str) -> Dic
-0000d480: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
-0000d490: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
-0000d4a0: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
-0000d4b0: 6965 7665 2074 6865 2070 6172 616d 6574  ieve the paramet
-0000d4c0: 6572 7320 6f66 2061 2077 6f72 6b66 6c6f  ers of a workflo
-0000d4d0: 772e 0a0a 2020 2020 2020 2020 4172 6773  w...        Args
-0000d4e0: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
-0000d4f0: 726b 666c 6f77 2028 7374 7229 3a20 5468  rkflow (str): Th
-0000d500: 6520 776f 726b 666c 6f77 2066 6f72 2077  e workflow for w
-0000d510: 6869 6368 2074 6f20 7265 7472 6965 7665  hich to retrieve
-0000d520: 2074 6865 2070 6172 616d 6574 6572 732e   the parameters.
-0000d530: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000d540: 733a 0a20 2020 2020 2020 2020 2020 2044  s:.            D
-0000d550: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
-0000d560: 722c 2041 6e79 5d5d 3a0a 2020 2020 2020  r, Any]]:.      
-0000d570: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
-0000d580: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-0000d590: 6720 7468 6520 776f 726b 666c 6f77 2070  g the workflow p
-0000d5a0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-0000d5b0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-0000d5c0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-0000d5d0: 6f72 3a20 4966 2061 6e20 6572 726f 7220  or: If an error 
-0000d5e0: 6f63 6375 7273 2077 6869 6c65 2072 6574  occurs while ret
-0000d5f0: 7269 6576 696e 6720 7468 6520 776f 726b  rieving the work
-0000d600: 666c 6f77 0a20 2020 2020 2020 2020 2020  flow.           
-0000d610: 2020 2020 2070 6172 616d 6574 6572 732e       parameters.
-0000d620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d630: 2020 2020 206a 736f 6e5f 6465 7363 7269       json_descri
-0000d640: 7074 6f72 203d 2073 656c 662e 7075 6c6c  ptor = self.pull
-0000d650: 5f64 6573 6372 6970 746f 725f 6672 6f6d  _descriptor_from
-0000d660: 5f67 6974 6875 6228 776f 726b 666c 6f77  _github(workflow
-0000d670: 290a 2020 2020 2020 2020 2320 636f 6e76  ).        # conv
-0000d680: 6572 7420 746f 206f 6d65 726f 2074 7970  ert to omero typ
-0000d690: 6573 0a20 2020 2020 2020 206c 6f67 6765  es.        logge
-0000d6a0: 722e 6465 6275 6728 6a73 6f6e 5f64 6573  r.debug(json_des
-0000d6b0: 6372 6970 746f 7229 0a20 2020 2020 2020  criptor).       
-0000d6c0: 2077 6f72 6b66 6c6f 775f 6469 6374 203d   workflow_dict =
-0000d6d0: 207b 7d0a 2020 2020 2020 2020 666f 7220   {}.        for 
-0000d6e0: 696e 7075 7420 696e 206a 736f 6e5f 6465  input in json_de
-0000d6f0: 7363 7269 7074 6f72 5b27 696e 7075 7473  scriptor['inputs
-0000d700: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0000d710: 2320 6669 6c74 6572 2063 7974 6f6d 696e  # filter cytomin
-0000d720: 6520 7061 7261 6d65 7465 7273 0a20 2020  e parameters.   
-0000d730: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000d740: 696e 7075 745b 2769 6427 5d2e 7374 6172  input['id'].star
-0000d750: 7473 7769 7468 2827 6379 746f 6d69 6e65  tswith('cytomine
-0000d760: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0000d770: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
-0000d780: 616d 7320 3d20 7b7d 0a20 2020 2020 2020  ams = {}.       
-0000d790: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000d7a0: 775f 7061 7261 6d73 5b27 6e61 6d65 275d  w_params['name']
-0000d7b0: 203d 2069 6e70 7574 5b27 6964 275d 0a20   = input['id']. 
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000d7d0: 6f72 6b66 6c6f 775f 7061 7261 6d73 5b27  orkflow_params['
-0000d7e0: 6465 6661 756c 7427 5d20 3d20 696e 7075  default'] = inpu
-0000d7f0: 745b 2764 6566 6175 6c74 2d76 616c 7565  t['default-value
-0000d800: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0000d810: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
-0000d820: 6d73 5b27 6379 7479 7065 275d 203d 2069  ms['cytype'] = i
-0000d830: 6e70 7574 5b27 7479 7065 275d 0a20 2020  nput['type'].   
-0000d840: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000d850: 6b66 6c6f 775f 7061 7261 6d73 5b27 6f70  kflow_params['op
-0000d860: 7469 6f6e 616c 275d 203d 2069 6e70 7574  tional'] = input
-0000d870: 5b27 6f70 7469 6f6e 616c 275d 0a20 2020  ['optional'].   
-0000d880: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000d890: 5f66 6c61 6720 3d20 696e 7075 745b 2763  _flag = input['c
-0000d8a0: 6f6d 6d61 6e64 2d6c 696e 652d 666c 6167  ommand-line-flag
-0000d8b0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0000d8c0: 2020 2063 6d64 5f66 6c61 6720 3d20 636d     cmd_flag = cm
-0000d8d0: 645f 666c 6167 2e72 6570 6c61 6365 2822  d_flag.replace("
-0000d8e0: 4069 6422 2c20 696e 7075 745b 2769 6427  @id", input['id'
-0000d8f0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000d900: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
-0000d910: 6d73 5b27 636d 645f 666c 6167 275d 203d  ms['cmd_flag'] =
-0000d920: 2063 6d64 5f66 6c61 670a 2020 2020 2020   cmd_flag.      
-0000d930: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000d940: 6f77 5f70 6172 616d 735b 2764 6573 6372  ow_params['descr
-0000d950: 6970 7469 6f6e 275d 203d 2069 6e70 7574  iption'] = input
-0000d960: 5b27 6465 7363 7269 7074 696f 6e27 5d0a  ['description'].
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 776f 726b 666c 6f77 5f64 6963 745b 696e  workflow_dict[in
-0000d990: 7075 745b 2769 6427 5d5d 203d 2077 6f72  put['id']] = wor
-0000d9a0: 6b66 6c6f 775f 7061 7261 6d73 0a20 2020  kflow_params.   
-0000d9b0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
-0000d9c0: 666c 6f77 5f64 6963 740a 0a20 2020 2064  flow_dict..    d
-0000d9d0: 6566 2063 6f6e 7665 7274 5f63 7974 7970  ef convert_cytyp
-0000d9e0: 655f 746f 5f6f 6d74 7970 6528 7365 6c66  e_to_omtype(self
-0000d9f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da10: 2020 2063 7974 7970 653a 2073 7472 2c20     cytype: str, 
-0000da20: 5f64 6566 6175 6c74 2c20 2a61 7267 732c  _default, *args,
-0000da30: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-0000da60: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
-0000da70: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-0000da80: 2061 2043 7974 6f6d 696e 6520 7479 7065   a Cytomine type
-0000da90: 2074 6f20 616e 204f 4d45 524f 2074 7970   to an OMERO typ
-0000daa0: 6520 616e 6420 696e 7374 616e 7469 6174  e and instantiat
-0000dab0: 6573 2069 740a 2020 2020 2020 2020 7769  es it.        wi
-0000dac0: 7468 2061 7267 732f 6b77 6172 6773 2e0a  th args/kwargs..
-0000dad0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-0000dae0: 6174 2043 7974 6f6d 696e 6520 6861 7320  at Cytomine has 
-0000daf0: 6120 5079 7468 6f6e 2043 6c69 656e 742c  a Python Client,
-0000db00: 2061 6e64 2073 6f6d 6520 636f 6e76 6572   and some conver
-0000db10: 7369 6f6e 206d 6574 686f 6473 0a20 2020  sion methods.   
-0000db20: 2020 2020 2074 6f20 7079 7468 6f6e 2074       to python t
-0000db30: 7970 6573 2c20 6275 7420 6e6f 7468 696e  ypes, but nothin
-0000db40: 6720 7061 7274 6963 756c 6172 6c79 2077  g particularly w
-0000db50: 6f72 7468 2064 6570 656e 6469 6e67 206f  orth depending o
-0000db60: 6e20 7468 6174 0a20 2020 2020 2020 206c  n that.        l
-0000db70: 6962 7261 7279 2066 6f72 2079 6574 2e20  ibrary for yet. 
-0000db80: 4d69 6768 7420 6265 2075 7365 6675 6c20  Might be useful 
-0000db90: 696e 2074 6865 2066 7574 7572 6520 7065  in the future pe
-0000dba0: 7268 6170 732e 0a20 2020 2020 2020 2028  rhaps..        (
-0000dbb0: 652e 672e 2068 7474 7073 3a2f 2f67 6974  e.g. https://git
-0000dbc0: 6875 622e 636f 6d2f 4379 746f 6d69 6e65  hub.com/Cytomine
-0000dbd0: 2d55 4c69 6567 652f 4379 746f 6d69 6e65  -ULiege/Cytomine
-0000dbe0: 2d70 7974 686f 6e2d 636c 6965 6e74 2f0a  -python-client/.
-0000dbf0: 2020 2020 2020 2020 626c 6f62 2f6d 6173          blob/mas
-0000dc00: 7465 722f 6379 746f 6d69 6e65 2f63 7974  ter/cytomine/cyt
-0000dc10: 6f6d 696e 655f 6a6f 622e 7079 290a 0a20  omine_job.py).. 
-0000dc20: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000dc30: 2020 2020 2020 2020 2063 7974 7970 6520           cytype 
-0000dc40: 2873 7472 293a 2054 6865 2043 7974 6f6d  (str): The Cytom
-0000dc50: 696e 6520 7479 7065 2074 6f20 636f 6e76  ine type to conv
-0000dc60: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
-0000dc70: 205f 6465 6661 756c 743a 2054 6865 2064   _default: The d
-0000dc80: 6566 6175 6c74 2076 616c 7565 2e20 5265  efault value. Re
-0000dc90: 7175 6972 6564 2074 6f20 6469 7374 696e  quired to distin
-0000dca0: 6775 6973 6820 6265 7477 6565 6e20 666c  guish between fl
-0000dcb0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-0000dcc0: 2020 2020 616e 6420 696e 742e 0a20 2020      and int..   
-0000dcd0: 2020 2020 2020 2020 202a 6172 6773 3a20           *args: 
-0000dce0: 4164 6469 7469 6f6e 616c 2070 6f73 6974  Additional posit
-0000dcf0: 696f 6e61 6c20 6172 6775 6d65 6e74 732e  ional arguments.
-0000dd00: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-0000dd10: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-0000dd20: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-0000dd30: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
-0000dd40: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000dd50: 2020 2041 6e79 3a0a 2020 2020 2020 2020     Any:.        
-0000dd60: 2020 2020 2020 2020 5468 6520 636f 6e76          The conv
-0000dd70: 6572 7465 6420 4f4d 4552 4f20 7479 7065  erted OMERO type
-0000dd80: 2063 6c61 7373 2069 6e73 7461 6e63 650a   class instance.
-0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dda0: 6f72 204e 6f6e 6520 6966 2065 7272 6f72  or None if error
-0000ddb0: 7320 6f63 6375 7265 642e 0a0a 2020 2020  s occured...    
-0000ddc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ddd0: 2320 544f 444f 206d 616b 6520 456e 756d  # TODO make Enum
-0000dde0: 203f 0a20 2020 2020 2020 2069 6620 6379   ?.        if cy
-0000ddf0: 7479 7065 203d 3d20 274e 756d 6265 7227  type == 'Number'
-0000de00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000de10: 2069 7369 6e73 7461 6e63 6528 5f64 6566   isinstance(_def
-0000de20: 6175 6c74 2c20 666c 6f61 7429 3a0a 2020  ault, float):.  
-0000de30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000de40: 666c 6f61 7420 696e 7374 6561 640a 2020  float instead.  
-0000de50: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000de60: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
-0000de70: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
-0000de80: 7269 7074 7322 2c20 2246 6c6f 6174 222c  ripts", "Float",
-0000de90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000deb0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
-0000dec0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000ded0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000dee0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000def0: 7572 6e20 7365 6c66 2e73 7472 5f74 6f5f  urn self.str_to_
-0000df00: 636c 6173 7328 226f 6d65 726f 2e73 6372  class("omero.scr
-0000df10: 6970 7473 222c 2022 496e 7422 2c0a 2020  ipts", "Int",.  
-0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
-0000df50: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000df60: 656c 6966 2063 7974 7970 6520 3d3d 2027  elif cytype == '
-0000df70: 426f 6f6c 6561 6e27 3a0a 2020 2020 2020  Boolean':.      
-0000df80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000df90: 662e 7374 725f 746f 5f63 6c61 7373 2822  f.str_to_class("
-0000dfa0: 6f6d 6572 6f2e 7363 7269 7074 7322 2c20  omero.scripts", 
-0000dfb0: 2242 6f6f 6c22 2c0a 2020 2020 2020 2020  "Bool",.        
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 2020 2020 2020 2020 202a 6172               *ar
-0000dfe0: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-0000dff0: 2020 2020 2020 656c 6966 2063 7974 7970        elif cytyp
-0000e000: 6520 3d3d 2027 5374 7269 6e67 273a 0a20  e == 'String':. 
-0000e010: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e020: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
-0000e030: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
-0000e040: 7473 222c 2022 5374 7269 6e67 222c 0a20  ts", "String",. 
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
-0000e080: 7267 7329 0a0a 2020 2020 6465 6620 6578  rgs)..    def ex
-0000e090: 7472 6163 745f 7061 7274 735f 6672 6f6d  tract_parts_from
-0000e0a0: 5f75 726c 2873 656c 662c 2069 6e70 7574  _url(self, input
-0000e0b0: 5f75 726c 3a20 7374 7229 202d 3e20 5475  _url: str) -> Tu
-0000e0c0: 706c 655b 4c69 7374 5b73 7472 5d2c 2073  ple[List[str], s
-0000e0d0: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
-0000e0e0: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
-0000e0f0: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-0000e100: 616e 6420 6272 616e 6368 2069 6e66 6f72  and branch infor
-0000e110: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
-0000e120: 696e 7075 7420 5552 4c2e 0a0a 2020 2020  input URL...    
-0000e130: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000e140: 2020 2020 2020 696e 7075 745f 7572 6c20        input_url 
-0000e150: 2873 7472 293a 2054 6865 2069 6e70 7574  (str): The input
-0000e160: 2047 6974 4875 6220 5552 4c2e 0a0a 2020   GitHub URL...  
-0000e170: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000e180: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-0000e190: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
-0000e1a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e1b0: 2020 5468 6520 6c69 7374 206f 6620 7572    The list of ur
-0000e1c0: 6c20 7061 7274 7320 616e 6420 7468 6520  l parts and the 
-0000e1d0: 6272 616e 6368 2f76 6572 7369 6f6e 2e0a  branch/version..
+00009810: 696e 666f 726d 6174 696f 6e2e 2044 6566  information. Def
+00009820: 6175 6c74 7320 746f 2022 6e6f 7722 2e0a  aults to "now"..
+00009830: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00009840: 6d6e 7320 2873 7472 293a 2054 6865 2063  mns (str): The c
+00009850: 6f6c 756d 6e73 2074 6f20 7265 7472 6965  olumns to retrie
+00009860: 7665 2066 726f 6d20 7468 6520 6a6f 6220  ve from the job 
+00009870: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+00009880: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00009890: 6175 6c74 7320 746f 2022 4a6f 6249 6422  aults to "JobId"
+000098a0: 2e20 4974 2069 7320 636f 6d6d 6120 7365  . It is comma se
+000098b0: 7061 7261 7465 642c 2065 2e67 2e20 224a  parated, e.g. "J
+000098c0: 6f62 4964 2c53 7461 7465 222e 0a20 2020  obId,State"..   
+000098d0: 2020 2020 2020 2020 2073 7461 7465 7320           states 
+000098e0: 2873 7472 293a 2054 6865 206a 6f62 2073  (str): The job s
+000098f0: 7461 7465 7320 746f 2069 6e63 6c75 6465  tates to include
+00009900: 2069 6e20 7468 6520 7175 6572 792e 0a20   in the query.. 
+00009910: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00009920: 6566 6175 6c74 7320 746f 2022 722c 6364  efaults to "r,cd
+00009930: 2c66 2c74 6f2c 7273 2c64 6c2c 6e66 222e  ,f,to,rs,dl,nf".
+00009940: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009950: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00009960: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
+00009970: 2020 2020 4120 7374 7269 6e67 2072 6570      A string rep
+00009980: 7265 7365 6e74 696e 6720 7468 6520 536c  resenting the Sl
+00009990: 7572 6d20 636f 6d6d 616e 6420 746f 2072  urm command to r
+000099a0: 6574 7269 6576 650a 2020 2020 2020 2020  etrieve.        
+000099b0: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+000099c0: 696f 6e20 6162 6f75 7420 6f6c 6420 6a6f  ion about old jo
+000099d0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
+000099e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000099f0: 656c 662e 5f41 4c4c 5f4a 4f42 535f 434d  elf._ALL_JOBS_CM
+00009a00: 442e 666f 726d 6174 2873 7461 7274 5f74  D.format(start_t
+00009a10: 696d 653d 7374 6172 745f 7469 6d65 2c0a  ime=start_time,.
+00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a40: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
+00009a50: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
+00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a80: 2020 2020 2073 7461 7465 733d 7374 6174       states=stat
+00009a90: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00009ac0: 756d 6e73 3d63 6f6c 756d 6e73 290a 0a20  umns=columns).. 
+00009ad0: 2020 2064 6566 2074 7261 6e73 6665 725f     def transfer_
+00009ae0: 6461 7461 2873 656c 662c 206c 6f63 616c  data(self, local
+00009af0: 5f70 6174 683a 2073 7472 2920 2d3e 2052  _path: str) -> R
+00009b00: 6573 756c 743a 0a20 2020 2020 2020 2022  esult:.        "
+00009b10: 2222 0a20 2020 2020 2020 2054 7261 6e73  "".        Trans
+00009b20: 6665 7273 2061 2066 696c 6520 6f72 2064  fers a file or d
+00009b30: 6972 6563 746f 7279 2066 726f 6d20 7468  irectory from th
+00009b40: 6520 6c6f 6361 6c20 6d61 6368 696e 6520  e local machine 
+00009b50: 746f 2074 6865 2072 656d 6f74 650a 2020  to the remote.  
+00009b60: 2020 2020 2020 536c 7572 6d20 636c 7573        Slurm clus
+00009b70: 7465 722e 0a0a 2020 2020 2020 2020 4172  ter...        Ar
+00009b80: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00009b90: 6c6f 6361 6c5f 7061 7468 2028 7374 7229  local_path (str)
+00009ba0: 3a20 5468 6520 6c6f 6361 6c20 7061 7468  : The local path
+00009bb0: 2074 6f20 7468 6520 6669 6c65 206f 7220   to the file or 
+00009bc0: 6469 7265 6374 6f72 7920 746f 0a20 2020  directory to.   
+00009bd0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00009be0: 6e73 6665 722e 0a0a 2020 2020 2020 2020  nsfer...        
+00009bf0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00009c00: 2020 2020 2052 6573 756c 743a 2054 6865       Result: The
+00009c10: 2072 6573 756c 7420 6f66 2074 6865 2066   result of the f
+00009c20: 696c 6520 7472 616e 7366 6572 206f 7065  ile transfer ope
+00009c30: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00009c40: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+00009c50: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00009c60: 2020 2020 2066 2254 7261 6e73 6665 7269       f"Transferi
+00009c70: 6e67 2066 696c 6520 7b6c 6f63 616c 5f70  ng file {local_p
+00009c80: 6174 687d 2074 6f20 7b73 656c 662e 736c  ath} to {self.sl
+00009c90: 7572 6d5f 6461 7461 5f70 6174 687d 2229  urm_data_path}")
+00009ca0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009cb0: 7365 6c66 2e70 7574 286c 6f63 616c 3d6c  self.put(local=l
+00009cc0: 6f63 616c 5f70 6174 682c 2072 656d 6f74  ocal_path, remot
+00009cd0: 653d 7365 6c66 2e73 6c75 726d 5f64 6174  e=self.slurm_dat
+00009ce0: 615f 7061 7468 290a 0a20 2020 2064 6566  a_path)..    def
+00009cf0: 2075 6e70 6163 6b5f 6461 7461 2873 656c   unpack_data(sel
+00009d00: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
+00009d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009d20: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
+00009d30: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
+00009d40: 5d5d 203d 204e 6f6e 6529 202d 3e20 5265  ]] = None) -> Re
+00009d50: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
+00009d60: 220a 2020 2020 2020 2020 556e 7061 636b  ".        Unpack
+00009d70: 7320 6120 7a69 7070 6564 2066 696c 6520  s a zipped file 
+00009d80: 6f6e 2074 6865 2072 656d 6f74 6520 536c  on the remote Sl
+00009d90: 7572 6d20 636c 7573 7465 722e 0a0a 2020  urm cluster...  
+00009da0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00009db0: 2020 2020 2020 2020 7a69 7066 696c 6520          zipfile 
+00009dc0: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
+00009dd0: 6f66 2074 6865 207a 6970 7065 6420 6669  of the zipped fi
+00009de0: 6c65 2074 6f20 6265 2075 6e70 6163 6b65  le to be unpacke
+00009df0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
+00009e00: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
+00009e10: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+00009e20: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
+00009e30: 6d65 6e74 2076 6172 6961 626c 6573 200a  ment variables .
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 746f 2073 6574 2077 6865 6e20 7275 6e6e  to set when runn
+00009e60: 696e 6720 7468 6520 636f 6d6d 616e 642e  ing the command.
+00009e70: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00009e80: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+00009e90: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00009ea0: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
+00009eb0: 756c 7420 6f66 2074 6865 2063 6f6d 6d61  ult of the comma
+00009ec0: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+00009ed0: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+00009ee0: 6c66 2e67 6574 5f75 6e7a 6970 5f63 6f6d  lf.get_unzip_com
+00009ef0: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
+00009f00: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00009f10: 6f28 6622 556e 7061 636b 696e 6720 7b7a  o(f"Unpacking {z
+00009f20: 6970 6669 6c65 7d20 6f6e 2053 6c75 726d  ipfile} on Slurm
+00009f30: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00009f40: 6e20 7365 6c66 2e72 756e 5f63 6f6d 6d61  n self.run_comma
+00009f50: 6e64 7328 5b63 6d64 5d2c 2065 6e76 3d65  nds([cmd], env=e
+00009f60: 6e76 290a 0a20 2020 2064 6566 2063 6f6e  nv)..    def con
+00009f70: 7665 7274 5f64 6174 6128 7365 6c66 2c20  vert_data(self, 
+00009f80: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2065 6e76 3a20 4f70 7469 6f6e 616c     env: Optional
+00009fb0: 5b44 6963 745b 7374 722c 2073 7472 5d5d  [Dict[str, str]]
+00009fc0: 203d 204e 6f6e 6529 202d 3e20 5265 7375   = None) -> Resu
+00009fd0: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
+00009fe0: 2020 2020 2020 2020 556e 7061 636b 7320          Unpacks 
+00009ff0: 6120 7a69 7070 6564 2066 696c 6520 6f6e  a zipped file on
+0000a000: 2074 6865 2072 656d 6f74 6520 536c 7572   the remote Slur
+0000a010: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
+0000a020: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000a030: 2020 2020 2020 7a69 7066 696c 6520 2873        zipfile (s
+0000a040: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+0000a050: 2074 6865 207a 6970 7065 6420 6669 6c65   the zipped file
+0000a060: 2074 6f20 6265 2075 6e70 6163 6b65 642e   to be unpacked.
+0000a070: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+0000a080: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
+0000a090: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
+0000a0a0: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
+0000a0b0: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000a0d0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
+0000a0e0: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
+0000a0f0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+0000a100: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000a110: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+0000a120: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
+0000a130: 7420 6f66 2074 6865 2063 6f6d 6d61 6e64  t of the command
+0000a140: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000a150: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
+0000a160: 2e67 6574 5f63 6f6e 7665 7274 5f63 6f6d  .get_convert_com
+0000a170: 6d61 6e64 287a 6970 6669 6c65 290a 2020  mand(zipfile).  
+0000a180: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+0000a190: 6f28 6622 436f 6e76 6572 7469 6e67 207b  o(f"Converting {
+0000a1a0: 7a69 7066 696c 657d 206f 6e20 536c 7572  zipfile} on Slur
+0000a1b0: 6d22 290a 2020 2020 2020 2020 7265 7475  m").        retu
+0000a1c0: 726e 2073 656c 662e 7275 6e5f 636f 6d6d  rn self.run_comm
+0000a1d0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
+0000a1e0: 656e 7629 0a0a 2020 2020 6465 6620 6765  env)..    def ge
+0000a1f0: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
+0000a200: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7365  _for_workflow(se
+0000a210: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000a240: 666c 6f77 3a20 7374 722c 0a20 2020 2020  flow: str,.     
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a270: 2020 2073 7562 7374 6974 7574 6573 3a20     substitutes: 
+0000a280: 4469 6374 5b73 7472 2c20 7374 725d 2c0a  Dict[str, str],.
+0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2b0: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
+0000a2c0: 3a20 7374 7220 3d20 226a 6f62 5f74 656d  : str = "job_tem
+0000a2d0: 706c 6174 652e 7368 220a 2020 2020 2020  plate.sh".      
+0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
+0000a310: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a320: 4765 6e65 7261 7465 2061 2053 6c75 726d  Generate a Slurm
+0000a330: 206a 6f62 2073 6372 6970 7420 666f 7220   job script for 
+0000a340: 6120 7370 6563 6966 6963 2077 6f72 6b66  a specific workf
+0000a350: 6c6f 772e 0a0a 2020 2020 2020 2020 4172  low...        Ar
+0000a360: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000a370: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
+0000a380: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0000a390: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
+0000a3a0: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
+0000a3b0: 7320 2844 6963 745b 7374 722c 2073 7472  s (Dict[str, str
+0000a3c0: 5d29 3a20 4120 6469 6374 696f 6e61 7279  ]): A dictionary
+0000a3d0: 2063 6f6e 7461 696e 696e 6720 6b65 792d   containing key-
+0000a3e0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
+0000a3f0: 2020 2020 2020 7061 6972 7320 666f 7220        pairs for 
+0000a400: 7375 6273 7469 7475 7469 6e67 2070 6c61  substituting pla
+0000a410: 6365 686f 6c64 6572 7320 696e 2074 6865  ceholders in the
+0000a420: 206a 6f62 2074 656d 706c 6174 652e 0a20   job template.. 
+0000a430: 2020 2020 2020 2020 2020 2074 656d 706c             templ
+0000a440: 6174 6520 2873 7472 2c20 6f70 7469 6f6e  ate (str, option
+0000a450: 616c 293a 2054 6865 2066 696c 656e 616d  al): The filenam
+0000a460: 6520 6f66 2074 6865 206a 6f62 2074 656d  e of the job tem
+0000a470: 706c 6174 652e 0a20 2020 2020 2020 2020  plate..         
+0000a480: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+0000a490: 746f 2022 6a6f 625f 7465 6d70 6c61 7465  to "job_template
+0000a4a0: 2e73 6822 2e0a 0a20 2020 2020 2020 2052  .sh"...        R
+0000a4b0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000a4c0: 2020 2020 7374 723a 2054 6865 2067 656e      str: The gen
+0000a4d0: 6572 6174 6564 2053 6c75 726d 206a 6f62  erated Slurm job
+0000a4e0: 2073 6372 6970 7420 6173 2061 2073 7472   script as a str
+0000a4f0: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
+0000a500: 0a20 2020 2020 2020 2023 2061 6464 2077  .        # add w
+0000a510: 6f72 6b66 6c6f 7720 746f 2073 7562 7374  orkflow to subst
+0000a520: 6974 7574 6573 0a20 2020 2020 2020 2073  itutes.        s
+0000a530: 7562 7374 6974 7574 6573 5b27 6a6f 626e  ubstitutes['jobn
+0000a540: 616d 6527 5d20 3d20 776f 726b 666c 6f77  ame'] = workflow
+0000a550: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
+0000a560: 6a6f 6220 7465 6d70 6c61 7465 0a20 2020  job template.   
+0000a570: 2020 2020 2074 656d 706c 6174 655f 6620       template_f 
+0000a580: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
+0000a590: 6573 2229 2e6a 6f69 6e70 6174 6828 7465  es").joinpath(te
+0000a5a0: 6d70 6c61 7465 290a 2020 2020 2020 2020  mplate).        
+0000a5b0: 7769 7468 2074 656d 706c 6174 655f 662e  with template_f.
+0000a5c0: 6f70 656e 2827 7227 2920 6173 2066 3a0a  open('r') as f:.
+0000a5d0: 2020 2020 2020 2020 2020 2020 7372 6320              src 
+0000a5e0: 3d20 5465 6d70 6c61 7465 2866 2e72 6561  = Template(f.rea
+0000a5f0: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+0000a600: 206a 6f62 5f73 6372 6970 7420 3d20 7372   job_script = sr
+0000a610: 632e 7361 6665 5f73 7562 7374 6974 7574  c.safe_substitut
+0000a620: 6528 7375 6273 7469 7475 7465 7329 0a20  e(substitutes). 
+0000a630: 2020 2020 2020 2072 6574 7572 6e20 6a6f         return jo
+0000a640: 625f 7363 7269 7074 0a0a 2020 2020 6465  b_script..    de
+0000a650: 6620 776f 726b 666c 6f77 5f70 6172 616d  f workflow_param
+0000a660: 735f 746f 5f73 7562 7328 7365 6c66 2c20  s_to_subs(self, 
+0000a670: 7061 7261 6d73 2920 2d3e 2044 6963 745b  params) -> Dict[
+0000a680: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
+0000a690: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000a6a0: 6f6e 7665 7274 2077 6f72 6b66 6c6f 7720  onvert workflow 
+0000a6b0: 7061 7261 6d65 7465 7273 2074 6f20 7375  parameters to su
+0000a6c0: 6273 7469 7475 7469 6f6e 2064 6963 7469  bstitution dicti
+0000a6d0: 6f6e 6172 7920 666f 7220 6a6f 6220 7363  onary for job sc
+0000a6e0: 7269 7074 2e0a 0a20 2020 2020 2020 2041  ript...        A
+0000a6f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000a700: 2070 6172 616d 733a 2041 2064 6963 7469   params: A dicti
+0000a710: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+0000a720: 2077 6f72 6b66 6c6f 7720 7061 7261 6d65   workflow parame
+0000a730: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
+0000a740: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000a750: 2020 2020 4469 6374 5b73 7472 2c20 7374      Dict[str, st
+0000a760: 725d 3a20 4120 6469 6374 696f 6e61 7279  r]: A dictionary
+0000a770: 2077 6974 6820 7061 7261 6d65 7465 7220   with parameter 
+0000a780: 6e61 6d65 7320 6173 206b 6579 7320 616e  names as keys an
+0000a790: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000a7a0: 2020 636f 7272 6573 706f 6e64 696e 6720    corresponding 
+0000a7b0: 666c 6167 7320 7769 7468 2070 6c61 6365  flags with place
+0000a7c0: 686f 6c64 6572 7320 6173 2076 616c 7565  holders as value
+0000a7d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0000a7e0: 2020 2020 2020 2073 7562 7320 3d20 7b7d         subs = {}
+0000a7f0: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
+0000a800: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0000a810: 5f2c 2070 6172 616d 2069 6e20 7061 7261  _, param in para
+0000a820: 6d73 2e69 7465 6d73 2829 3a0a 2020 2020  ms.items():.    
+0000a830: 2020 2020 2020 2020 666c 6167 203d 2070          flag = p
+0000a840: 6172 616d 5b27 636d 645f 666c 6167 275d  aram['cmd_flag']
+0000a850: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
+0000a860: 6720 3d20 666c 6167 202b 2022 2024 2220  g = flag + " $" 
+0000a870: 2b20 7061 7261 6d5b 276e 616d 6527 5d2e  + param['name'].
+0000a880: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+0000a890: 2020 2020 666c 6167 732e 6170 7065 6e64      flags.append
+0000a8a0: 2866 6c61 6729 0a20 2020 2020 2020 2073  (flag).        s
+0000a8b0: 7562 735b 2750 4152 414d 5327 5d20 3d20  ubs['PARAMS'] = 
+0000a8c0: 2220 222e 6a6f 696e 2866 6c61 6773 290a  " ".join(flags).
+0000a8d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000a8e0: 7562 730a 0a20 2020 2064 6566 2075 7064  ubs..    def upd
+0000a8f0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
+0000a900: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
+0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a920: 2020 2020 2067 656e 6572 6174 655f 6a6f       generate_jo
+0000a930: 6273 3a20 626f 6f6c 203d 2046 616c 7365  bs: bool = False
+0000a940: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a950: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a960: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
+0000a970: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
+0000a980: 6f6e 6529 202d 3e20 5265 7375 6c74 3a0a  one) -> Result:.
+0000a990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000a9a0: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
+0000a9b0: 6c6f 6361 6c20 636f 7079 206f 6620 7468  local copy of th
+0000a9c0: 6520 536c 7572 6d20 6a6f 6220 7375 626d  e Slurm job subm
+0000a9d0: 6973 7369 6f6e 2073 6372 6970 7473 2e0a  ission scripts..
+0000a9e0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
+0000a9f0: 6e63 7469 6f6e 2070 756c 6c73 2074 6865  nction pulls the
+0000aa00: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+0000aa10: 6f66 2074 6865 2073 6372 6970 7473 2066  of the scripts f
+0000aa20: 726f 6d20 7468 6520 4769 740a 2020 2020  rom the Git.    
+0000aa30: 2020 2020 7265 706f 7369 746f 7279 2061      repository a
+0000aa40: 6e64 2063 6f70 6965 7320 7468 656d 2074  nd copies them t
+0000aa50: 6f20 7468 6520 736c 7572 6d5f 7363 7269  o the slurm_scri
+0000aa60: 7074 5f70 6174 6820 6469 7265 6374 6f72  pt_path director
+0000aa70: 792e 0a20 2020 2020 2020 2041 6c74 6572  y..        Alter
+0000aa80: 6e61 7469 7665 6c79 2c20 6974 2063 616e  natively, it can
+0000aa90: 2067 656e 6572 6174 6520 7363 7269 7074   generate script
+0000aaa0: 7320 6672 6f6d 2061 2074 656d 706c 6174  s from a templat
+0000aab0: 652e 2054 6869 7320 6973 2074 6865 0a20  e. This is the. 
+0000aac0: 2020 2020 2020 2064 6566 6175 6c74 2062         default b
+0000aad0: 6568 6176 696f 7220 6966 206e 6f20 4769  ehavior if no Gi
+0000aae0: 7420 7265 706f 2069 7320 7072 6f76 6964  t repo is provid
+0000aaf0: 6564 206f 7220 6361 6e20 6265 2066 6f72  ed or can be for
+0000ab00: 6365 6420 7669 6120 7468 650a 2020 2020  ced via the.    
+0000ab10: 2020 2020 6067 656e 6572 6174 655f 6a6f      `generate_jo
+0000ab20: 6273 6020 7061 7261 6d65 7465 722e 0a0a  bs` parameter...
+0000ab30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000ab40: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+0000ab50: 7465 5f6a 6f62 7320 2862 6f6f 6c29 3a20  te_jobs (bool): 
+0000ab60: 5768 6574 6865 7220 746f 2067 656e 6572  Whether to gener
+0000ab70: 6174 6520 6e65 7720 736c 7572 6d20 6a6f  ate new slurm jo
+0000ab80: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
+0000ab90: 2020 2020 2020 2020 2020 494e 5354 4541            INSTEA
+0000aba0: 4420 286f 6620 7075 6c6c 696e 6720 6672  D (of pulling fr
+0000abb0: 6f6d 2067 6974 292e 2044 6566 6175 6c74  om git). Default
+0000abc0: 7320 746f 2046 616c 7365 2c20 6578 6365  s to False, exce
+0000abd0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
+0000abe0: 2020 2069 6620 6e6f 2073 6c75 726d 5f73     if no slurm_s
+0000abf0: 6372 6970 745f 7265 706f 2069 7320 636f  cript_repo is co
+0000ac00: 6e66 6967 7572 6564 2e0a 2020 2020 2020  nfigured..      
+0000ac10: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+0000ac20: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+0000ac30: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+0000ac40: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+0000ac50: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
+0000ac60: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
+0000ac70: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+0000ac80: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+0000ac90: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+0000aca0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000acb0: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
+0000acc0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+0000acd0: 2063 6f6d 6d61 6e64 2e0a 2020 2020 2020   command..      
+0000ace0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000acf0: 206e 6f74 2073 656c 662e 736c 7572 6d5f   not self.slurm_
+0000ad00: 7363 7269 7074 5f72 6570 6f3a 0a20 2020  script_repo:.   
+0000ad10: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+0000ad20: 655f 6a6f 6273 203d 2054 7275 650a 0a20  e_jobs = True.. 
+0000ad30: 2020 2020 2020 2069 6620 6765 6e65 7261         if genera
+0000ad40: 7465 5f6a 6f62 733a 0a20 2020 2020 2020  te_jobs:.       
+0000ad50: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000ad60: 2822 4765 6e65 7261 7469 6e67 2053 6c75  ("Generating Slu
+0000ad70: 726d 206a 6f62 2073 6372 6970 7473 2229  rm job scripts")
+0000ad80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000ad90: 2077 662c 206a 6f62 5f70 6174 6820 696e   wf, job_path in
+0000ada0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+0000adb0: 6c5f 6a6f 6273 2e69 7465 6d73 2829 3a0a  l_jobs.items():.
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000add0: 2320 6765 6e65 7261 7465 206a 6f62 2073  # generate job s
+0000ade0: 6372 6970 740a 2020 2020 2020 2020 2020  cript.          
+0000adf0: 2020 2020 2020 7061 7261 6d73 203d 2073        params = s
+0000ae00: 656c 662e 6765 745f 776f 726b 666c 6f77  elf.get_workflow
+0000ae10: 5f70 6172 616d 6574 6572 7328 7766 290a  _parameters(wf).
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae30: 7375 6273 203d 2073 656c 662e 776f 726b  subs = self.work
+0000ae40: 666c 6f77 5f70 6172 616d 735f 746f 5f73  flow_params_to_s
+0000ae50: 7562 7328 7061 7261 6d73 290a 2020 2020  ubs(params).    
+0000ae60: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000ae70: 7363 7269 7074 203d 2073 656c 662e 6765  script = self.ge
+0000ae80: 6e65 7261 7465 5f73 6c75 726d 5f6a 6f62  nerate_slurm_job
+0000ae90: 5f66 6f72 5f77 6f72 6b66 6c6f 7728 7766  _for_workflow(wf
+0000aea0: 2c20 7375 6273 290a 2020 2020 2020 2020  , subs).        
+0000aeb0: 2020 2020 2020 2020 2320 656e 7375 7265          # ensure
+0000aec0: 2061 6c6c 2064 6972 7320 6578 6973 7420   all dirs exist 
+0000aed0: 7265 6d6f 7465 6c79 0a20 2020 2020 2020  remotely.       
+0000aee0: 2020 2020 2020 2020 2066 756c 6c5f 7061           full_pa
+0000aef0: 7468 203d 2073 656c 662e 736c 7572 6d5f  th = self.slurm_
+0000af00: 7363 7269 7074 5f70 6174 682b 222f 222b  script_path+"/"+
+0000af10: 6a6f 625f 7061 7468 0a20 2020 2020 2020  job_path.       
+0000af20: 2020 2020 2020 2020 206a 6f62 5f64 6972           job_dir
+0000af30: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
+0000af40: 6c69 7428 6675 6c6c 5f70 6174 6829 0a20  lit(full_path). 
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000af60: 656c 662e 7275 6e28 6622 6d6b 6469 7220  elf.run(f"mkdir 
+0000af70: 2d70 207b 6a6f 625f 6469 727d 2229 0a20  -p {job_dir}"). 
+0000af80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000af90: 2063 6f70 7920 746f 2072 656d 6f74 6520   copy to remote 
+0000afa0: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
+0000afb0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+0000afc0: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
+0000afd0: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
+0000afe0: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 7265 6d6f 7465 3d66          remote=f
+0000b010: 756c 6c5f 7061 7468 290a 2020 2020 2020  ull_path).      
+0000b020: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000b030: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
+0000b040: 6574 5f75 7064 6174 655f 736c 7572 6d5f  et_update_slurm_
+0000b050: 7363 7269 7074 735f 636f 6d6d 616e 6428  scripts_command(
+0000b060: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+0000b070: 6767 6572 2e69 6e66 6f28 2255 7064 6174  gger.info("Updat
+0000b080: 696e 6720 536c 7572 6d20 6a6f 6220 7363  ing Slurm job sc
+0000b090: 7269 7074 7320 6f6e 2053 6c75 726d 2229  ripts on Slurm")
+0000b0a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000b0b0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+0000b0c0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
+0000b0d0: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
+0000b0e0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0000b0f0: 2020 2064 6566 2072 756e 5f77 6f72 6b66     def run_workf
+0000b100: 6c6f 7728 7365 6c66 2c0a 2020 2020 2020  low(self,.      
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000b120: 6f72 6b66 6c6f 775f 6e61 6d65 3a20 7374  orkflow_name: st
+0000b130: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000b140: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000b150: 5f76 6572 7369 6f6e 3a20 7374 722c 0a20  _version: str,. 
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 696e 7075 745f 6461 7461 3a20      input_data: 
+0000b180: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000b190: 2020 2020 2020 2020 2020 656d 6169 6c3a            email:
+0000b1a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000b1b0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000b1c0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000b1d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000b1e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000b1f0: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+0000b200: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
+0000b210: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+0000b220: 5475 706c 655b 5265 7375 6c74 2c20 696e  Tuple[Result, in
+0000b230: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
+0000b240: 2020 2020 2020 2020 5275 6e20 6120 7370          Run a sp
+0000b250: 6563 6966 6965 6420 776f 726b 666c 6f77  ecified workflow
+0000b260: 206f 6e20 536c 7572 6d20 7573 696e 6720   on Slurm using 
+0000b270: 7468 6520 6769 7665 6e20 7061 7261 6d65  the given parame
+0000b280: 7465 7273 2e0a 0a20 2020 2020 2020 2041  ters...        A
+0000b290: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000b2a0: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
+0000b2b0: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
+0000b2c0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
+0000b2d0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
+0000b2e0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+0000b2f0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
+0000b300: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
+0000b310: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
+0000b320: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
+0000b330: 2020 206f 6e20 536c 7572 6d29 2e0a 2020     on Slurm)..  
+0000b340: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000b350: 6461 7461 2028 7374 7229 3a20 4e61 6d65  data (str): Name
+0000b360: 206f 6620 7468 6520 696e 7075 7420 6461   of the input da
+0000b370: 7461 2066 6f6c 6465 7220 636f 6e74 6169  ta folder contai
+0000b380: 6e69 6e67 2069 6e70 7574 0a20 2020 2020  ning input.     
+0000b390: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0000b3a0: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
+0000b3b0: 2020 2020 656d 6169 6c20 2873 7472 2c20      email (str, 
+0000b3c0: 6f70 7469 6f6e 616c 293a 2045 6d61 696c  optional): Email
+0000b3d0: 2061 6464 7265 7373 2066 6f72 2053 6c75   address for Slu
+0000b3e0: 726d 206a 6f62 206e 6f74 6966 6963 6174  rm job notificat
+0000b3f0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+0000b400: 2020 7469 6d65 2028 7374 722c 206f 7074    time (str, opt
+0000b410: 696f 6e61 6c29 3a20 5469 6d65 206c 696d  ional): Time lim
+0000b420: 6974 2066 6f72 2074 6865 2053 6c75 726d  it for the Slurm
+0000b430: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
+0000b440: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000b450: 6d61 7420 4848 3a4d 4d3a 5353 2e0a 2020  mat HH:MM:SS..  
+0000b460: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000b470: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000b480: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000b490: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
+0000b4a0: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
+0000b4b0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000b4c0: 2054 7570 6c65 5b52 6573 756c 742c 2069   Tuple[Result, i
+0000b4d0: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
+0000b4e0: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
+0000b4f0: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
+0000b500: 6c74 206f 6620 7374 6172 7469 6e67 2074  lt of starting t
+0000b510: 6865 2077 6f72 6b66 6c6f 7720 6a6f 6220  he workflow job 
+0000b520: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+0000b530: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
+0000b540: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
+0000b550: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
+0000b560: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
+0000b570: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
+0000b580: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000b590: 2053 6c75 726d 206a 6f62 2049 4420 6973   Slurm job ID is
+0000b5a0: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
+0000b5b0: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
+0000b5c0: 6520 0a20 2020 2020 2020 2020 2020 2060  e .            `
+0000b5d0: 7275 6e5f 636f 6d6d 616e 6473 6020 6d65  run_commands` me
+0000b5e0: 7468 6f64 2e0a 2020 2020 2020 2020 2222  thod..        ""
+0000b5f0: 220a 2020 2020 2020 2020 7362 6174 6368  ".        sbatch
+0000b600: 5f63 6d64 2c20 7362 6174 6368 5f65 6e76  _cmd, sbatch_env
+0000b610: 203d 2073 656c 662e 6765 745f 776f 726b   = self.get_work
+0000b620: 666c 6f77 5f63 6f6d 6d61 6e64 280a 2020  flow_command(.  
+0000b630: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000b640: 6f77 5f6e 616d 652c 2077 6f72 6b66 6c6f  ow_name, workflo
+0000b650: 775f 7665 7273 696f 6e2c 2069 6e70 7574  w_version, input
+0000b660: 5f64 6174 612c 2065 6d61 696c 2c20 7469  _data, email, ti
+0000b670: 6d65 2c20 2a2a 6b77 6172 6773 290a 2020  me, **kwargs).  
+0000b680: 2020 2020 2020 7072 696e 7428 6622 5275        print(f"Ru
+0000b690: 6e6e 696e 6720 7b77 6f72 6b66 6c6f 775f  nning {workflow_
+0000b6a0: 6e61 6d65 7d20 6a6f 6220 6f6e 207b 696e  name} job on {in
+0000b6b0: 7075 745f 6461 7461 7d20 6f6e 2053 6c75  put_data} on Slu
+0000b6c0: 726d 3a5c 0a20 2020 2020 2020 2020 2020  rm:\.           
+0000b6d0: 207b 7362 6174 6368 5f63 6d64 7d20 772f   {sbatch_cmd} w/
+0000b6e0: 207b 7362 6174 6368 5f65 6e76 7d22 290a   {sbatch_env}").
+0000b6f0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000b700: 6e66 6f28 6622 5275 6e6e 696e 6720 7b77  nfo(f"Running {w
+0000b710: 6f72 6b66 6c6f 775f 6e61 6d65 7d20 6a6f  orkflow_name} jo
+0000b720: 6220 6f6e 207b 696e 7075 745f 6461 7461  b on {input_data
+0000b730: 7d20 6f6e 2053 6c75 726d 2229 0a20 2020  } on Slurm").   
+0000b740: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+0000b750: 7275 6e5f 636f 6d6d 616e 6473 285b 7362  run_commands([sb
+0000b760: 6174 6368 5f63 6d64 5d2c 2073 6261 7463  atch_cmd], sbatc
+0000b770: 685f 656e 7629 0a20 2020 2020 2020 2072  h_env).        r
+0000b780: 6574 7572 6e20 7265 732c 2073 656c 662e  eturn res, self.
+0000b790: 6578 7472 6163 745f 6a6f 625f 6964 2872  extract_job_id(r
+0000b7a0: 6573 290a 0a20 2020 2064 6566 2072 756e  es)..    def run
+0000b7b0: 5f77 6f72 6b66 6c6f 775f 6a6f 6228 7365  _workflow_job(se
+0000b7c0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000b7d0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000b7e0: 6b66 6c6f 775f 6e61 6d65 3a20 7374 722c  kflow_name: str,
+0000b7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b800: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000b810: 6f77 5f76 6572 7369 6f6e 3a20 7374 722c  ow_version: str,
+0000b820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b830: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000b840: 6461 7461 3a20 7374 722c 0a20 2020 2020  data: str,.     
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2020 2020 656d 6169 6c3a 204f 7074 696f      email: Optio
+0000b870: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000b880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b890: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
+0000b8a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000b8b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000b8d0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
+0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2029 202d 3e20 536c 7572 6d4a 6f62 3a0a   ) -> SlurmJob:.
+0000b900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b910: 2020 2020 5275 6e20 6120 7370 6563 6966      Run a specif
+0000b920: 6965 6420 776f 726b 666c 6f77 206f 6e20  ied workflow on 
+0000b930: 536c 7572 6d20 7573 696e 6720 7468 6520  Slurm using the 
+0000b940: 6769 7665 6e20 7061 7261 6d65 7465 7273  given parameters
+0000b950: 2061 6e64 2072 6574 7572 6e20 6120 536c   and return a Sl
+0000b960: 7572 6d4a 6f62 2069 6e73 7461 6e63 652e  urmJob instance.
+0000b970: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000b980: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000b990: 666c 6f77 5f6e 616d 6520 2873 7472 293a  flow_name (str):
+0000b9a0: 204e 616d 6520 6f66 2074 6865 2077 6f72   Name of the wor
+0000b9b0: 6b66 6c6f 7720 746f 2065 7865 6375 7465  kflow to execute
+0000b9c0: 2e0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+0000b9d0: 726b 666c 6f77 5f76 6572 7369 6f6e 2028  rkflow_version (
+0000b9e0: 7374 7229 3a20 5665 7273 696f 6e20 6f66  str): Version of
+0000b9f0: 2074 6865 2077 6f72 6b66 6c6f 7720 2869   the workflow (i
+0000ba00: 6d61 6765 2076 6572 7369 6f6e 206f 6e20  mage version on 
+0000ba10: 536c 7572 6d29 2e0a 2020 2020 2020 2020  Slurm)..        
+0000ba20: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
+0000ba30: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
+0000ba40: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
+0000ba50: 6465 7220 636f 6e74 6169 6e69 6e67 2069  der containing i
+0000ba60: 6e70 7574 2069 6d61 6765 2066 696c 6573  nput image files
+0000ba70: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+0000ba80: 6169 6c20 2873 7472 2c20 6f70 7469 6f6e  ail (str, option
+0000ba90: 616c 293a 2045 6d61 696c 2061 6464 7265  al): Email addre
+0000baa0: 7373 2066 6f72 2053 6c75 726d 206a 6f62  ss for Slurm job
+0000bab0: 206e 6f74 6966 6963 6174 696f 6e73 2e0a   notifications..
+0000bac0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000bad0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+0000bae0: 3a20 5469 6d65 206c 696d 6974 2066 6f72  : Time limit for
+0000baf0: 2074 6865 2053 6c75 726d 206a 6f62 2069   the Slurm job i
+0000bb00: 6e20 7468 6520 666f 726d 6174 2048 483a  n the format HH:
+0000bb10: 4d4d 3a53 532e 0a20 2020 2020 2020 2020  MM:SS..         
+0000bb20: 2020 202a 2a6b 7761 7267 733a 2041 6464     **kwargs: Add
+0000bb30: 6974 696f 6e61 6c20 6b65 7977 6f72 6420  itional keyword 
+0000bb40: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
+0000bb50: 6520 776f 726b 666c 6f77 2e0a 0a20 2020  e workflow...   
+0000bb60: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000bb70: 2020 2020 2020 2020 2020 536c 7572 6d4a            SlurmJ
+0000bb80: 6f62 3a20 4120 536c 7572 6d4a 6f62 2069  ob: A SlurmJob i
+0000bb90: 6e73 7461 6e63 6520 7265 7072 6573 656e  nstance represen
+0000bba0: 7469 6e67 2074 6865 2073 7461 7274 6564  ting the started
+0000bbb0: 2077 6f72 6b66 6c6f 7720 6a6f 622e 0a20   workflow job.. 
+0000bbc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000bbd0: 2020 2072 6573 756c 742c 206a 6f62 5f69     result, job_i
+0000bbe0: 6420 3d20 7365 6c66 2e72 756e 5f77 6f72  d = self.run_wor
+0000bbf0: 6b66 6c6f 7728 0a20 2020 2020 2020 2020  kflow(.         
+0000bc00: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
+0000bc10: 2c20 776f 726b 666c 6f77 5f76 6572 7369  , workflow_versi
+0000bc20: 6f6e 2c20 696e 7075 745f 6461 7461 2c20  on, input_data, 
+0000bc30: 656d 6169 6c2c 2074 696d 652c 202a 2a6b  email, time, **k
+0000bc40: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
+0000bc50: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
+0000bc60: 6573 756c 742c 206a 6f62 5f69 6429 0a0a  esult, job_id)..
+0000bc70: 2020 2020 6465 6620 7275 6e5f 636f 6e76      def run_conv
+0000bc80: 6572 7369 6f6e 5f77 6f72 6b66 6c6f 775f  ersion_workflow_
+0000bc90: 6a6f 6228 7365 6c66 2c20 666f 6c64 6572  job(self, folder
+0000bca0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcd0: 736f 7572 6365 5f66 6f72 6d61 743a 2073  source_format: s
+0000bce0: 7472 203d 2027 7a61 7272 272c 0a20 2020  tr = 'zarr',.   
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
+0000bd20: 7374 7220 3d20 2774 6966 6627 0a20 2020  str = 'tiff'.   
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd50: 2029 202d 3e20 5475 706c 655b 5265 7375   ) -> Tuple[Resu
+0000bd60: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
+0000bd70: 2020 2222 220a 2020 2020 2020 2020 5275    """.        Ru
+0000bd80: 6e20 7468 6520 6461 7461 2063 6f6e 7665  n the data conve
+0000bd90: 7273 696f 6e20 776f 726b 666c 6f77 206f  rsion workflow o
+0000bda0: 6e20 536c 7572 6d20 7573 696e 6720 7468  n Slurm using th
+0000bdb0: 6520 6769 7665 6e20 6461 7461 2066 6f6c  e given data fol
+0000bdc0: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
+0000bdd0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000bde0: 666f 6c64 6572 5f6e 616d 6520 2873 7472  folder_name (str
+0000bdf0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+0000be00: 6865 2064 6174 6120 666f 6c64 6572 2063  he data folder c
+0000be10: 6f6e 7461 696e 696e 6720 736f 7572 6365  ontaining source
+0000be20: 2066 6f72 6d61 7420 6669 6c65 732e 0a20   format files.. 
+0000be30: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+0000be40: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
+0000be50: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
+0000be60: 6174 2066 6f72 2063 6f6e 7665 7273 696f  at for conversio
+0000be70: 6e20 2864 6566 6175 6c74 2069 7320 277a  n (default is 'z
+0000be80: 6172 7227 292e 0a20 2020 2020 2020 2020  arr')..         
+0000be90: 2020 2074 6172 6765 745f 666f 726d 6174     target_format
+0000bea0: 2028 7374 7229 3a20 5461 7267 6574 2064   (str): Target d
+0000beb0: 6174 6120 666f 726d 6174 2061 6674 6572  ata format after
+0000bec0: 2063 6f6e 7665 7273 696f 6e20 2864 6566   conversion (def
+0000bed0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
+0000bee0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000bef0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+0000bf00: 7570 6c65 5b52 6573 756c 742c 2069 6e74  uple[Result, int
+0000bf10: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000bf20: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+0000bf30: 696e 696e 6720 7468 6520 7265 7375 6c74  ining the result
+0000bf40: 206f 6620 7374 6172 7469 6e67 2074 6865   of starting the
+0000bf50: 2063 6f6e 7665 7273 696f 6e20 6a6f 6220   conversion job 
+0000bf60: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+0000bf70: 2020 2020 7468 6520 536c 7572 6d20 6a6f      the Slurm jo
+0000bf80: 6220 4944 2c20 6f72 202d 3120 6966 2074  b ID, or -1 if t
+0000bf90: 6865 206a 6f62 2049 4420 636f 756c 6420  he job ID could 
+0000bfa0: 6e6f 7420 6265 2065 7874 7261 6374 6564  not be extracted
+0000bfb0: 2e0a 0a20 2020 2020 2020 2057 6172 6e69  ...        Warni
+0000bfc0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+0000bfd0: 5468 6520 6465 6661 756c 7420 696d 706c  The default impl
+0000bfe0: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
+0000bff0: 7375 7070 6f72 7473 2063 6f6e 7665 7273  supports convers
+0000c000: 696f 6e20 6672 6f6d 2027 7a61 7272 2720  ion from 'zarr' 
+0000c010: 746f 2027 7469 6666 272e 0a20 2020 2020  to 'tiff'..     
+0000c020: 2020 2020 2020 2049 6620 7573 696e 6720         If using 
+0000c030: 6f74 6865 7220 736f 7572 6365 206f 7220  other source or 
+0000c040: 7461 7267 6574 2066 6f72 6d61 7473 2c20  target formats, 
+0000c050: 7573 6572 7320 6d75 7374 2069 6d70 6c65  users must imple
+0000c060: 6d65 6e74 2061 6e64 2063 6f6e 6669 6775  ment and configu
+0000c070: 7265 0a20 2020 2020 2020 2020 2020 2061  re.            a
+0000c080: 6464 6974 696f 6e61 6c20 636f 6e76 6572  dditional conver
+0000c090: 7465 7273 2074 6865 6d73 656c 7665 732e  ters themselves.
+0000c0a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c0b0: 2020 2020 2023 2047 656e 6572 6174 6520       # Generate 
+0000c0c0: 6120 756e 6971 7565 2063 6f6e 6669 6720  a unique config 
+0000c0d0: 6669 6c65 206e 616d 650a 2020 2020 2020  file name.      
+0000c0e0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
+0000c0f0: 6622 636f 6e66 6967 5f7b 666f 6c64 6572  f"config_{folder
+0000c100: 5f6e 616d 657d 2e74 7874 220a 0a20 2020  _name}.txt"..   
+0000c110: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
+0000c120: 2061 6c6c 2063 6f6d 6d61 6e64 7320 746f   all commands to
+0000c130: 2072 756e 2063 6f6e 7365 6375 7469 7665   run consecutive
+0000c140: 6c79 0a20 2020 2020 2020 2064 6174 615f  ly.        data_
+0000c150: 7061 7468 203d 2066 227b 7365 6c66 2e73  path = f"{self.s
+0000c160: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
+0000c170: 7b66 6f6c 6465 725f 6e61 6d65 7d22 0a20  {folder_name}". 
+0000c180: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
+0000c190: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
+0000c1a0: 7620 3d20 7365 6c66 2e67 6574 5f63 6f6e  v = self.get_con
+0000c1b0: 7665 7273 696f 6e5f 636f 6d6d 616e 6428  version_command(
+0000c1c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000c1d0: 615f 7061 7468 2c20 636f 6e66 6967 5f66  a_path, config_f
+0000c1e0: 696c 652c 2073 6f75 7263 655f 666f 726d  ile, source_form
+0000c1f0: 6174 2c20 7461 7267 6574 5f66 6f72 6d61  at, target_forma
+0000c200: 7429 0a20 2020 2020 2020 2063 6f6d 6d61  t).        comma
+0000c210: 6e64 7320 3d20 5b0a 2020 2020 2020 2020  nds = [.        
+0000c220: 2020 2020 6622 6669 6e64 207b 6461 7461      f"find {data
+0000c230: 5f70 6174 687d 2f64 6174 612f 696e 202d  _path}/data/in -
+0000c240: 6e61 6d65 2027 2a2e 7b73 6f75 7263 655f  name '*.{source_
+0000c250: 666f 726d 6174 7d27 207c 2061 776b 2027  format}' | awk '
+0000c260: 7b7b 7072 696e 7420 4e52 2c20 2430 7d7d  {{print NR, $0}}
+0000c270: 2720 3e20 7b63 6f6e 6669 675f 6669 6c65  ' > {config_file
+0000c280: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+0000c290: 6622 4e3d 2428 7763 202d 6c20 3c20 5c22  f"N=$(wc -l < \"
+0000c2a0: 7b63 6f6e 6669 675f 6669 6c65 7d5c 2229  {config_file}\")
+0000c2b0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+0000c2c0: 2265 6368 6f20 5c22 4e75 6d62 6572 206f  "echo \"Number o
+0000c2d0: 6620 2e7b 736f 7572 6365 5f66 6f72 6d61  f .{source_forma
+0000c2e0: 747d 2066 696c 6573 3a20 244e 5c22 222c  t} files: $N\"",
+0000c2f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000c300: 7665 7273 696f 6e5f 636d 640a 2020 2020  version_cmd.    
+0000c310: 2020 2020 5d0a 0a20 2020 2020 2020 2023      ]..        #
+0000c320: 2052 756e 2061 6c6c 2063 6f6d 6d61 6e64   Run all command
+0000c330: 7320 636f 6e73 6563 7574 6976 656c 790a  s consecutively.
+0000c340: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+0000c350: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+0000c360: 636f 6d6d 616e 6473 2c20 7362 6174 6368  commands, sbatch
+0000c370: 5f65 6e76 290a 0a20 2020 2020 2020 2072  _env)..        r
+0000c380: 6574 7572 6e20 536c 7572 6d4a 6f62 2872  eturn SlurmJob(r
+0000c390: 6573 2c20 7365 6c66 2e65 7874 7261 6374  es, self.extract
+0000c3a0: 5f6a 6f62 5f69 6428 7265 7329 290a 0a20  _job_id(res)).. 
+0000c3b0: 2020 2064 6566 2065 7874 7261 6374 5f6a     def extract_j
+0000c3c0: 6f62 5f69 6428 7365 6c66 2c20 7265 7375  ob_id(self, resu
+0000c3d0: 6c74 3a20 5265 7375 6c74 2920 2d3e 2069  lt: Result) -> i
+0000c3e0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+0000c3f0: 2020 2020 2020 2020 4578 7472 6163 7420          Extract 
+0000c400: 7468 6520 536c 7572 6d20 6a6f 6220 4944  the Slurm job ID
+0000c410: 2066 726f 6d20 7468 6520 7265 7375 6c74   from the result
+0000c420: 206f 6620 6120 636f 6d6d 616e 642e 0a0a   of a command...
+0000c430: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000c440: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000c450: 2028 5265 7375 6c74 293a 2054 6865 2072   (Result): The r
+0000c460: 6573 756c 7420 6f66 2061 2063 6f6d 6d61  esult of a comma
+0000c470: 6e64 2065 7865 6375 7469 6f6e 2e0a 0a20  nd execution... 
+0000c480: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000c490: 2020 2020 2020 2020 2020 2020 696e 743a              int:
+0000c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4b0: 2054 6865 2053 6c75 726d 206a 6f62 2049   The Slurm job I
+0000c4c0: 4420 6578 7472 6163 7465 6420 6672 6f6d  D extracted from
+0000c4d0: 2074 6865 2072 6573 756c 742c 0a20 2020   the result,.   
+0000c4e0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000c4f0: 2d31 2069 6620 6e6f 7420 666f 756e 642e  -1 if not found.
+0000c500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c510: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+0000c520: 6420 3d20 6e65 7874 2828 696e 7428 732e  d = next((int(s.
+0000c530: 7374 7269 7028 2929 2066 6f72 2073 2069  strip()) for s i
+0000c540: 6e20 7265 7375 6c74 2e73 7464 6f75 742e  n result.stdout.
+0000c550: 7370 6c69 7428 0a20 2020 2020 2020 2020  split(.         
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2022 5375 626d 6974 7465 6420 6261     "Submitted ba
+0000c580: 7463 6820 6a6f 6222 2920 6966 2073 2e73  tch job") if s.s
+0000c590: 7472 6970 2829 2e69 7364 6967 6974 2829  trip().isdigit()
+0000c5a0: 292c 202d 3129 0a20 2020 2020 2020 2072  ), -1).        r
+0000c5b0: 6574 7572 6e20 736c 7572 6d5f 6a6f 625f  eturn slurm_job_
+0000c5c0: 6964 0a0a 2020 2020 6465 6620 6765 745f  id..    def get_
+0000c5d0: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
+0000c5e0: 6970 7473 5f63 6f6d 6d61 6e64 2873 656c  ipts_command(sel
+0000c5f0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+0000c600: 2020 2022 2222 4765 6e65 7261 7465 2074     """Generate t
+0000c610: 6865 2063 6f6d 6d61 6e64 2074 6f20 7570  he command to up
+0000c620: 6461 7465 2074 6865 2047 6974 2072 6570  date the Git rep
+0000c630: 6f73 6974 6f72 7920 636f 6e74 6169 6e69  ository containi
+0000c640: 6e67 0a20 2020 2020 2020 2074 6865 2053  ng.        the S
+0000c650: 6c75 726d 2073 6372 6970 7473 2c20 6966  lurm scripts, if
+0000c660: 206e 6563 6573 7361 7279 2e0a 0a20 2020   necessary...   
+0000c670: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000c680: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0000c6a0: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
+0000c6b0: 6e67 2074 6865 2047 6974 2063 6f6d 6d61  ng the Git comma
+0000c6c0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0000c6d0: 2020 2074 6f20 7570 6461 7465 2074 6865     to update the
+0000c6e0: 2053 6c75 726d 2073 6372 6970 7473 2e0a   Slurm scripts..
+0000c6f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c700: 2020 2020 7570 6461 7465 5f63 6d64 203d      update_cmd =
+0000c710: 2066 2267 6974 202d 4320 7b73 656c 662e   f"git -C {self.
+0000c720: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
+0000c730: 687d 2070 756c 6c22 0a20 2020 2020 2020  h} pull".       
+0000c740: 2072 6574 7572 6e20 7570 6461 7465 5f63   return update_c
+0000c750: 6d64 0a0a 2020 2020 6465 6620 6368 6563  md..    def chec
+0000c760: 6b5f 6a6f 625f 7374 6174 7573 2873 656c  k_job_status(sel
+0000c770: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000c780: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+0000c790: 6d5f 6a6f 625f 6964 733a 204c 6973 745b  m_job_ids: List[
+0000c7a0: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000c7c0: 6e76 3a20 4f70 7469 6f6e 616c 5b44 6963  nv: Optional[Dic
+0000c7d0: 745b 7374 722c 2073 7472 5d5d 203d 204e  t[str, str]] = N
+0000c7e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000c7f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+0000c800: 3e20 5475 706c 655b 4469 6374 5b69 6e74  > Tuple[Dict[int
+0000c810: 2c20 7374 725d 2c20 5265 7375 6c74 5d3a  , str], Result]:
+0000c820: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c830: 2020 2020 2043 6865 636b 2074 6865 2073       Check the s
+0000c840: 7461 7475 7320 6f66 2053 6c75 726d 206a  tatus of Slurm j
+0000c850: 6f62 7320 7769 7468 2074 6865 2067 6976  obs with the giv
+0000c860: 656e 206a 6f62 2049 4473 2e0a 0a20 2020  en job IDs...   
+0000c870: 2020 2020 204e 6f74 653a 2054 6869 7320       Note: This 
+0000c880: 646f 6573 6e27 7420 7265 7475 726e 206a  doesn't return j
+0000c890: 6f62 2061 7272 6179 7320 696e 6469 7669  ob arrays indivi
+0000c8a0: 6475 616c 6c79 2e0a 2020 2020 2020 2020  dually..        
+0000c8b0: 4974 2074 616b 6573 2074 6865 206c 6173  It takes the las
+0000c8c0: 7420 7661 6c75 6520 7265 7475 726e 6564  t value returned
+0000c8d0: 2066 6f72 2074 686f 7365 2073 7562 2069   for those sub i
+0000c8e0: 6473 200a 2020 2020 2020 2020 2867 656e  ds .        (gen
+0000c8f0: 6572 616c 6c79 2074 6865 206f 6e65 2073  erally the one s
+0000c900: 7469 6c6c 2050 454e 4449 4e47 292e 0a0a  till PENDING)...
+0000c910: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000c920: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+0000c930: 6a6f 625f 6964 7320 284c 6973 745b 696e  job_ids (List[in
+0000c940: 745d 293a 2054 6865 206a 6f62 2049 4473  t]): The job IDs
+0000c950: 206f 6620 7468 6520 536c 7572 6d20 6a6f   of the Slurm jo
+0000c960: 6273 2074 6f20 6368 6563 6b2e 0a20 2020  bs to check..   
+0000c970: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+0000c980: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+0000c990: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+0000c9a0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+0000c9b0: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
+0000c9c0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
+0000c9d0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
+0000c9e0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
+0000c9f0: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
+0000ca00: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000ca10: 2020 2020 2020 2020 2054 7570 6c65 5b44           Tuple[D
+0000ca20: 6963 745b 696e 742c 2073 7472 5d2c 2052  ict[int, str], R
+0000ca30: 6573 756c 745d 3a0a 2020 2020 2020 2020  esult]:.        
+0000ca40: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+0000ca50: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
+0000ca60: 7461 7475 7320 7065 7220 696e 7075 7420  tatus per input 
+0000ca70: 4944 2061 6e64 2074 6865 2072 6573 756c  ID and the resul
+0000ca80: 7420 6f66 200a 2020 2020 2020 2020 2020  t of .          
+0000ca90: 2020 2020 2020 7468 6520 636f 6d6d 616e        the comman
+0000caa0: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
+0000cab0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+0000cac0: 2020 2020 2020 2020 2020 5353 4845 7863            SSHExc
+0000cad0: 6570 7469 6f6e 3a20 4966 2074 6865 2063  eption: If the c
+0000cae0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
+0000caf0: 2066 6169 6c73 206f 7220 6e6f 2072 6573   fails or no res
+0000cb00: 706f 6e73 6520 6973 0a20 2020 2020 2020  ponse is.       
+0000cb10: 2020 2020 2020 2020 2072 6563 6569 7665           receive
+0000cb20: 6420 6166 7465 7220 6d75 6c74 6970 6c65  d after multiple
+0000cb30: 2072 6574 7269 6573 2e0a 2020 2020 2020   retries..      
+0000cb40: 2020 2222 220a 2020 2020 2020 2020 636d    """.        cm
+0000cb50: 6420 3d20 7365 6c66 2e67 6574 5f6a 6f62  d = self.get_job
+0000cb60: 5f73 7461 7475 735f 636f 6d6d 616e 6428  _status_command(
+0000cb70: 736c 7572 6d5f 6a6f 625f 6964 7329 0a20  slurm_job_ids). 
+0000cb80: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000cb90: 666f 2866 2247 6574 7469 6e67 2073 7461  fo(f"Getting sta
+0000cba0: 7475 7320 6f66 207b 736c 7572 6d5f 6a6f  tus of {slurm_jo
+0000cbb0: 625f 6964 737d 206f 6e20 536c 7572 6d22  b_ids} on Slurm"
+0000cbc0: 290a 2020 2020 2020 2020 7265 7472 795f  ).        retry_
+0000cbd0: 7374 6174 7573 203d 2030 0a20 2020 2020  status = 0.     
+0000cbe0: 2020 2077 6869 6c65 2072 6574 7279 5f73     while retry_s
+0000cbf0: 7461 7475 7320 3c20 333a 0a20 2020 2020  tatus < 3:.     
+0000cc00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000cc10: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+0000cc20: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
+0000cc30: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+0000cc40: 6767 6572 2e69 6e66 6f28 7265 7375 6c74  gger.info(result
+0000cc50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000cc60: 2072 6573 756c 742e 6f6b 3a0a 2020 2020   result.ok:.    
+0000cc70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000cc80: 6f74 2072 6573 756c 742e 7374 646f 7574  ot result.stdout
+0000cc90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cca0: 2020 2020 2020 2320 7761 6974 2066 6f72        # wait for
+0000ccb0: 2033 2073 6563 6f6e 6473 2062 6566 6f72   3 seconds befor
+0000ccc0: 6520 6368 6563 6b69 6e67 2061 6761 696e  e checking again
+0000ccd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cce0: 2020 2020 2074 696d 6573 6c65 6570 2e73       timesleep.s
+0000ccf0: 6c65 6570 2833 290a 2020 2020 2020 2020  leep(3).        
+0000cd00: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+0000cd10: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
+0000cd20: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
+0000cd30: 6174 7573 202b 3d20 310a 2020 2020 2020  atus += 1.      
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000cd50: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 6622 5265 7472 7920 7b72 6574      f"Retry {ret
+0000cd80: 7279 5f73 7461 7475 737d 2067 6574 7469  ry_status} getti
+0000cd90: 6e67 2073 7461 7475 7320 5c0a 2020 2020  ng status \.    
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2020 2020 2020 6f66 207b 736c 7572          of {slur
+0000cdc0: 6d5f 6a6f 625f 6964 737d 2122 290a 2020  m_job_ids}!").  
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000cde0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000cdf0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
+0000ce10: 625f 7374 6174 7573 5f64 6963 7420 3d20  b_status_dict = 
+0000ce20: 7b69 6e74 286c 696e 652e 7370 6c69 7428  {int(line.split(
+0000ce30: 295b 305d 2e73 706c 6974 2827 5f27 295b  )[0].split('_')[
+0000ce40: 305d 293a 206c 696e 652e 7370 6c69 7428  0]): line.split(
+0000ce50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce60: 2020 2020 2029 5b31 5d20 666f 7220 6c69       )[1] for li
+0000ce70: 6e65 2069 6e20 7265 7375 6c74 2e73 7464  ne in result.std
+0000ce80: 6f75 742e 7370 6c69 7428 225c 6e22 2920  out.split("\n") 
+0000ce90: 6966 206c 696e 657d 0a20 2020 2020 2020  if line}.       
+0000cea0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000ceb0: 6765 722e 6465 6275 6728 6622 4a6f 6220  ger.debug(f"Job 
+0000cec0: 7374 6174 7573 6573 3a20 7b6a 6f62 5f73  statuses: {job_s
+0000ced0: 7461 7475 735f 6469 6374 7d22 290a 2020  tatus_dict}").  
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 2020 7265 7475 726e 206a 6f62 5f73 7461    return job_sta
+0000cf00: 7475 735f 6469 6374 2c20 7265 7375 6c74  tus_dict, result
+0000cf10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000cf20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000cf30: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
+0000cf40: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
+0000cf50: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
+0000cf60: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000cf70: 6572 726f 7228 6572 726f 7229 0a20 2020  error(error).   
+0000cf80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000cf90: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
+0000cfa0: 6572 726f 7229 0a20 2020 2020 2020 2065  error).        e
+0000cfb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000cfc0: 2065 7272 6f72 203d 2066 2245 7272 6f72   error = f"Error
+0000cfd0: 3a20 5265 7472 6965 6420 7b72 6574 7279  : Retried {retry
+0000cfe0: 5f73 7461 7475 737d 2074 696d 6573 2074  _status} times t
+0000cff0: 6f20 6765 7420 5c0a 2020 2020 2020 2020  o get \.        
+0000d000: 2020 2020 2020 2020 7374 6174 7573 206f          status o
+0000d010: 6620 7b73 6c75 726d 5f6a 6f62 5f69 6473  f {slurm_job_ids
+0000d020: 7d2c 2062 7574 206e 6f20 7265 7370 6f6e  }, but no respon
+0000d030: 7365 2e22 0a20 2020 2020 2020 2020 2020  se.".           
+0000d040: 206c 6f67 6765 722e 6572 726f 7228 6572   logger.error(er
+0000d050: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+0000d060: 2072 6169 7365 2053 5348 4578 6365 7074   raise SSHExcept
+0000d070: 696f 6e28 6572 726f 7229 0a0a 2020 2020  ion(error)..    
+0000d080: 6465 6620 6765 745f 6a6f 625f 7374 6174  def get_job_stat
+0000d090: 7573 5f63 6f6d 6d61 6e64 2873 656c 662c  us_command(self,
+0000d0a0: 2073 6c75 726d 5f6a 6f62 5f69 6473 3a20   slurm_job_ids: 
+0000d0b0: 4c69 7374 5b69 6e74 5d29 202d 3e20 7374  List[int]) -> st
+0000d0c0: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+0000d0d0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+0000d0e0: 6520 536c 7572 6d20 636f 6d6d 616e 6420  e Slurm command 
+0000d0f0: 746f 2067 6574 2074 6865 2073 7461 7475  to get the statu
+0000d100: 7320 6f66 206a 6f62 7320 7769 7468 2074  s of jobs with t
+0000d110: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
+0000d120: 206a 6f62 2049 4473 2e0a 0a20 2020 2020   job IDs...     
+0000d130: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000d140: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+0000d150: 6473 2028 4c69 7374 5b69 6e74 5d29 3a20  ds (List[int]): 
+0000d160: 5468 6520 6a6f 6220 4944 7320 6f66 2074  The job IDs of t
+0000d170: 6865 206a 6f62 7320 746f 2063 6865 636b  he jobs to check
+0000d180: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000d190: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000d1a0: 7374 723a 200a 2020 2020 2020 2020 2020  str: .          
+0000d1b0: 2020 2020 2020 5468 6520 536c 7572 6d20        The Slurm 
+0000d1c0: 636f 6d6d 616e 6420 746f 2067 6574 2074  command to get t
+0000d1d0: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
+0000d1e0: 206a 6f62 732e 0a20 2020 2020 2020 2022   jobs..        "
+0000d1f0: 2222 0a20 2020 2020 2020 2023 2063 6f6e  "".        # con
+0000d200: 6361 7420 6d75 6c74 6970 6c65 206a 6f62  cat multiple job
+0000d210: 7320 6966 206e 6565 6465 640a 2020 2020  s if needed.    
+0000d220: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
+0000d230: 203d 2022 202d 6a20 222e 6a6f 696e 285b   = " -j ".join([
+0000d240: 7374 7228 6964 2920 666f 7220 6964 2069  str(id) for id i
+0000d250: 6e20 736c 7572 6d5f 6a6f 625f 6964 735d  n slurm_job_ids]
+0000d260: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d270: 2073 656c 662e 5f4a 4f42 5f53 5441 5455   self._JOB_STATU
+0000d280: 535f 434d 442e 666f 726d 6174 2873 6c75  S_CMD.format(slu
+0000d290: 726d 5f6a 6f62 5f69 643d 736c 7572 6d5f  rm_job_id=slurm_
+0000d2a0: 6a6f 625f 6964 290a 0a20 2020 2064 6566  job_id)..    def
+0000d2b0: 2065 7874 7261 6374 5f64 6174 615f 6c6f   extract_data_lo
+0000d2c0: 6361 7469 6f6e 5f66 726f 6d5f 6c6f 6728  cation_from_log(
+0000d2d0: 7365 6c66 2c20 736c 7572 6d5f 6a6f 625f  self, slurm_job_
+0000d2e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d310: 2020 2020 2020 206c 6f67 6669 6c65 3a20         logfile: 
+0000d320: 7374 7220 3d20 4e6f 6e65 2920 2d3e 2073  str = None) -> s
+0000d330: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
+0000d340: 6561 6420 534c 5552 4d20 6a6f 6220 6c6f  ead SLURM job lo
+0000d350: 6766 696c 6520 746f 2066 696e 6420 6c6f  gfile to find lo
+0000d360: 6361 7469 6f6e 206f 6620 7468 6520 6461  cation of the da
+0000d370: 7461 2e0a 0a20 2020 2020 2020 204f 6e65  ta...        One
+0000d380: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
+0000d390: 7273 2069 7320 7265 7175 6972 6564 2c20  rs is required, 
+0000d3a0: 6569 7468 6572 2069 6420 6f72 2066 696c  either id or fil
+0000d3b0: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+0000d3c0: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
+0000d3d0: 7572 6d5f 6a6f 625f 6964 2028 7374 7229  urm_job_id (str)
+0000d3e0: 3a20 4964 206f 6620 7468 6520 736c 7572  : Id of the slur
+0000d3f0: 6d20 6a6f 620a 2020 2020 2020 2020 2020  m job.          
+0000d400: 2020 6c6f 6766 696c 6520 2873 7472 293a    logfile (str):
+0000d410: 2050 6174 6820 746f 2074 6865 206c 6f67   Path to the log
+0000d420: 6669 6c65 0a0a 2020 2020 2020 2020 5265  file..        Re
+0000d430: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000d440: 2020 2073 7472 3a20 4461 7461 206c 6f63     str: Data loc
+0000d450: 6174 696f 6e20 6163 636f 7264 696e 6720  ation according 
+0000d460: 746f 2074 6865 206c 6f67 0a0a 2020 2020  to the log..    
+0000d470: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000d480: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
+0000d490: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
+0000d4a0: 7320 616e 2069 7373 7565 2077 6974 6820  s an issue with 
+0000d4b0: 7468 6520 636f 6d6d 616e 6420 6578 6563  the command exec
+0000d4c0: 7574 696f 6e2e 0a20 2020 2020 2020 2022  ution..        "
+0000d4d0: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
+0000d4e0: 6766 696c 6520 6973 204e 6f6e 6520 616e  gfile is None an
+0000d4f0: 6420 736c 7572 6d5f 6a6f 625f 6964 2069  d slurm_job_id i
+0000d500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000d510: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
+0000d520: 3d20 7365 6c66 2e5f 4c4f 4746 494c 450a  = self._LOGFILE.
+0000d530: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
+0000d540: 696c 6520 3d20 6c6f 6766 696c 652e 666f  ile = logfile.fo
+0000d550: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
+0000d560: 643d 736c 7572 6d5f 6a6f 625f 6964 290a  d=slurm_job_id).
+0000d570: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+0000d580: 6c66 2e5f 4c4f 4746 494c 455f 4441 5441  lf._LOGFILE_DATA
+0000d590: 5f43 4d44 2e66 6f72 6d61 7428 6c6f 675f  _CMD.format(log_
+0000d5a0: 6669 6c65 3d6c 6f67 6669 6c65 290a 2020  file=logfile).  
+0000d5b0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d5c0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+0000d5d0: 285b 636d 645d 290a 2020 2020 2020 2020  ([cmd]).        
+0000d5e0: 6966 2072 6573 756c 742e 6f6b 3a0a 2020  if result.ok:.  
+0000d5f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d600: 2072 6573 756c 742e 7374 646f 7574 0a20   result.stdout. 
+0000d610: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000d620: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+0000d630: 5348 4578 6365 7074 696f 6e28 7265 7375  SHException(resu
+0000d640: 6c74 290a 0a20 2020 2064 6566 2067 6574  lt)..    def get
+0000d650: 5f77 6f72 6b66 6c6f 775f 7061 7261 6d65  _workflow_parame
+0000d660: 7465 7273 2873 656c 662c 0a20 2020 2020  ters(self,.     
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000d690: 6c6f 773a 2073 7472 2920 2d3e 2044 6963  low: str) -> Dic
+0000d6a0: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
+0000d6b0: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
+0000d6c0: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
+0000d6d0: 6965 7665 2074 6865 2070 6172 616d 6574  ieve the paramet
+0000d6e0: 6572 7320 6f66 2061 2077 6f72 6b66 6c6f  ers of a workflo
+0000d6f0: 772e 0a0a 2020 2020 2020 2020 4172 6773  w...        Args
+0000d700: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
+0000d710: 726b 666c 6f77 2028 7374 7229 3a20 5468  rkflow (str): Th
+0000d720: 6520 776f 726b 666c 6f77 2066 6f72 2077  e workflow for w
+0000d730: 6869 6368 2074 6f20 7265 7472 6965 7665  hich to retrieve
+0000d740: 2074 6865 2070 6172 616d 6574 6572 732e   the parameters.
+0000d750: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000d760: 733a 0a20 2020 2020 2020 2020 2020 2044  s:.            D
+0000d770: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
+0000d780: 722c 2041 6e79 5d5d 3a0a 2020 2020 2020  r, Any]]:.      
+0000d790: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
+0000d7a0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+0000d7b0: 6720 7468 6520 776f 726b 666c 6f77 2070  g the workflow p
+0000d7c0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+0000d7d0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000d7e0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+0000d7f0: 6f72 3a20 4966 2061 6e20 6572 726f 7220  or: If an error 
+0000d800: 6f63 6375 7273 2077 6869 6c65 2072 6574  occurs while ret
+0000d810: 7269 6576 696e 6720 7468 6520 776f 726b  rieving the work
+0000d820: 666c 6f77 0a20 2020 2020 2020 2020 2020  flow.           
+0000d830: 2020 2020 2070 6172 616d 6574 6572 732e       parameters.
+0000d840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d850: 2020 2020 206a 736f 6e5f 6465 7363 7269       json_descri
+0000d860: 7074 6f72 203d 2073 656c 662e 7075 6c6c  ptor = self.pull
+0000d870: 5f64 6573 6372 6970 746f 725f 6672 6f6d  _descriptor_from
+0000d880: 5f67 6974 6875 6228 776f 726b 666c 6f77  _github(workflow
+0000d890: 290a 2020 2020 2020 2020 2320 636f 6e76  ).        # conv
+0000d8a0: 6572 7420 746f 206f 6d65 726f 2074 7970  ert to omero typ
+0000d8b0: 6573 0a20 2020 2020 2020 206c 6f67 6765  es.        logge
+0000d8c0: 722e 6465 6275 6728 6a73 6f6e 5f64 6573  r.debug(json_des
+0000d8d0: 6372 6970 746f 7229 0a20 2020 2020 2020  criptor).       
+0000d8e0: 2077 6f72 6b66 6c6f 775f 6469 6374 203d   workflow_dict =
+0000d8f0: 207b 7d0a 2020 2020 2020 2020 666f 7220   {}.        for 
+0000d900: 696e 7075 7420 696e 206a 736f 6e5f 6465  input in json_de
+0000d910: 7363 7269 7074 6f72 5b27 696e 7075 7473  scriptor['inputs
+0000d920: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0000d930: 2320 6669 6c74 6572 2063 7974 6f6d 696e  # filter cytomin
+0000d940: 6520 7061 7261 6d65 7465 7273 0a20 2020  e parameters.   
+0000d950: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000d960: 696e 7075 745b 2769 6427 5d2e 7374 6172  input['id'].star
+0000d970: 7473 7769 7468 2827 6379 746f 6d69 6e65  tswith('cytomine
+0000d980: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000d990: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
+0000d9a0: 616d 7320 3d20 7b7d 0a20 2020 2020 2020  ams = {}.       
+0000d9b0: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000d9c0: 775f 7061 7261 6d73 5b27 6e61 6d65 275d  w_params['name']
+0000d9d0: 203d 2069 6e70 7574 5b27 6964 275d 0a20   = input['id']. 
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000d9f0: 6f72 6b66 6c6f 775f 7061 7261 6d73 5b27  orkflow_params['
+0000da00: 6465 6661 756c 7427 5d20 3d20 696e 7075  default'] = inpu
+0000da10: 745b 2764 6566 6175 6c74 2d76 616c 7565  t['default-value
+0000da20: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000da30: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
+0000da40: 6d73 5b27 6379 7479 7065 275d 203d 2069  ms['cytype'] = i
+0000da50: 6e70 7574 5b27 7479 7065 275d 0a20 2020  nput['type'].   
+0000da60: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000da70: 6b66 6c6f 775f 7061 7261 6d73 5b27 6f70  kflow_params['op
+0000da80: 7469 6f6e 616c 275d 203d 2069 6e70 7574  tional'] = input
+0000da90: 5b27 6f70 7469 6f6e 616c 275d 0a20 2020  ['optional'].   
+0000daa0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+0000dab0: 5f66 6c61 6720 3d20 696e 7075 745b 2763  _flag = input['c
+0000dac0: 6f6d 6d61 6e64 2d6c 696e 652d 666c 6167  ommand-line-flag
+0000dad0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000dae0: 2020 2063 6d64 5f66 6c61 6720 3d20 636d     cmd_flag = cm
+0000daf0: 645f 666c 6167 2e72 6570 6c61 6365 2822  d_flag.replace("
+0000db00: 4069 6422 2c20 696e 7075 745b 2769 6427  @id", input['id'
+0000db10: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000db20: 2020 2077 6f72 6b66 6c6f 775f 7061 7261     workflow_para
+0000db30: 6d73 5b27 636d 645f 666c 6167 275d 203d  ms['cmd_flag'] =
+0000db40: 2063 6d64 5f66 6c61 670a 2020 2020 2020   cmd_flag.      
+0000db50: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000db60: 6f77 5f70 6172 616d 735b 2764 6573 6372  ow_params['descr
+0000db70: 6970 7469 6f6e 275d 203d 2069 6e70 7574  iption'] = input
+0000db80: 5b27 6465 7363 7269 7074 696f 6e27 5d0a  ['description'].
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 776f 726b 666c 6f77 5f64 6963 745b 696e  workflow_dict[in
+0000dbb0: 7075 745b 2769 6427 5d5d 203d 2077 6f72  put['id']] = wor
+0000dbc0: 6b66 6c6f 775f 7061 7261 6d73 0a20 2020  kflow_params.   
+0000dbd0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
+0000dbe0: 666c 6f77 5f64 6963 740a 0a20 2020 2064  flow_dict..    d
+0000dbf0: 6566 2063 6f6e 7665 7274 5f63 7974 7970  ef convert_cytyp
+0000dc00: 655f 746f 5f6f 6d74 7970 6528 7365 6c66  e_to_omtype(self
+0000dc10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2020 2063 7974 7970 653a 2073 7472 2c20     cytype: str, 
+0000dc40: 5f64 6566 6175 6c74 2c20 2a61 7267 732c  _default, *args,
+0000dc50: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+0000dc80: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+0000dc90: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
+0000dca0: 2061 2043 7974 6f6d 696e 6520 7479 7065   a Cytomine type
+0000dcb0: 2074 6f20 616e 204f 4d45 524f 2074 7970   to an OMERO typ
+0000dcc0: 6520 616e 6420 696e 7374 616e 7469 6174  e and instantiat
+0000dcd0: 6573 2069 740a 2020 2020 2020 2020 7769  es it.        wi
+0000dce0: 7468 2061 7267 732f 6b77 6172 6773 2e0a  th args/kwargs..
+0000dcf0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
+0000dd00: 6174 2043 7974 6f6d 696e 6520 6861 7320  at Cytomine has 
+0000dd10: 6120 5079 7468 6f6e 2043 6c69 656e 742c  a Python Client,
+0000dd20: 2061 6e64 2073 6f6d 6520 636f 6e76 6572   and some conver
+0000dd30: 7369 6f6e 206d 6574 686f 6473 0a20 2020  sion methods.   
+0000dd40: 2020 2020 2074 6f20 7079 7468 6f6e 2074       to python t
+0000dd50: 7970 6573 2c20 6275 7420 6e6f 7468 696e  ypes, but nothin
+0000dd60: 6720 7061 7274 6963 756c 6172 6c79 2077  g particularly w
+0000dd70: 6f72 7468 2064 6570 656e 6469 6e67 206f  orth depending o
+0000dd80: 6e20 7468 6174 0a20 2020 2020 2020 206c  n that.        l
+0000dd90: 6962 7261 7279 2066 6f72 2079 6574 2e20  ibrary for yet. 
+0000dda0: 4d69 6768 7420 6265 2075 7365 6675 6c20  Might be useful 
+0000ddb0: 696e 2074 6865 2066 7574 7572 6520 7065  in the future pe
+0000ddc0: 7268 6170 732e 0a20 2020 2020 2020 2028  rhaps..        (
+0000ddd0: 652e 672e 2068 7474 7073 3a2f 2f67 6974  e.g. https://git
+0000dde0: 6875 622e 636f 6d2f 4379 746f 6d69 6e65  hub.com/Cytomine
+0000ddf0: 2d55 4c69 6567 652f 4379 746f 6d69 6e65  -ULiege/Cytomine
+0000de00: 2d70 7974 686f 6e2d 636c 6965 6e74 2f0a  -python-client/.
+0000de10: 2020 2020 2020 2020 626c 6f62 2f6d 6173          blob/mas
+0000de20: 7465 722f 6379 746f 6d69 6e65 2f63 7974  ter/cytomine/cyt
+0000de30: 6f6d 696e 655f 6a6f 622e 7079 290a 0a20  omine_job.py).. 
+0000de40: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000de50: 2020 2020 2020 2020 2063 7974 7970 6520           cytype 
+0000de60: 2873 7472 293a 2054 6865 2043 7974 6f6d  (str): The Cytom
+0000de70: 696e 6520 7479 7065 2074 6f20 636f 6e76  ine type to conv
+0000de80: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
+0000de90: 205f 6465 6661 756c 743a 2054 6865 2064   _default: The d
+0000dea0: 6566 6175 6c74 2076 616c 7565 2e20 5265  efault value. Re
+0000deb0: 7175 6972 6564 2074 6f20 6469 7374 696e  quired to distin
+0000dec0: 6775 6973 6820 6265 7477 6565 6e20 666c  guish between fl
+0000ded0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+0000dee0: 2020 2020 616e 6420 696e 742e 0a20 2020      and int..   
+0000def0: 2020 2020 2020 2020 202a 6172 6773 3a20           *args: 
+0000df00: 4164 6469 7469 6f6e 616c 2070 6f73 6974  Additional posit
+0000df10: 696f 6e61 6c20 6172 6775 6d65 6e74 732e  ional arguments.
+0000df20: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000df30: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
+0000df40: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+0000df50: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
+0000df60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000df70: 2020 2041 6e79 3a0a 2020 2020 2020 2020     Any:.        
+0000df80: 2020 2020 2020 2020 5468 6520 636f 6e76          The conv
+0000df90: 6572 7465 6420 4f4d 4552 4f20 7479 7065  erted OMERO type
+0000dfa0: 2063 6c61 7373 2069 6e73 7461 6e63 650a   class instance.
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 6f72 204e 6f6e 6520 6966 2065 7272 6f72  or None if error
+0000dfd0: 7320 6f63 6375 7265 642e 0a0a 2020 2020  s occured...    
+0000dfe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000dff0: 2320 544f 444f 206d 616b 6520 456e 756d  # TODO make Enum
+0000e000: 203f 0a20 2020 2020 2020 2069 6620 6379   ?.        if cy
+0000e010: 7479 7065 203d 3d20 274e 756d 6265 7227  type == 'Number'
+0000e020: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000e030: 2069 7369 6e73 7461 6e63 6528 5f64 6566   isinstance(_def
+0000e040: 6175 6c74 2c20 666c 6f61 7429 3a0a 2020  ault, float):.  
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e060: 666c 6f61 7420 696e 7374 6561 640a 2020  float instead.  
+0000e070: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000e080: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
+0000e090: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
+0000e0a0: 7269 7074 7322 2c20 2246 6c6f 6174 222c  ripts", "Float",
+0000e0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0d0: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
+0000e0e0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000e0f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e100: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e110: 7572 6e20 7365 6c66 2e73 7472 5f74 6f5f  urn self.str_to_
+0000e120: 636c 6173 7328 226f 6d65 726f 2e73 6372  class("omero.scr
+0000e130: 6970 7473 222c 2022 496e 7422 2c0a 2020  ipts", "Int",.  
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e160: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
+0000e170: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+0000e180: 656c 6966 2063 7974 7970 6520 3d3d 2027  elif cytype == '
+0000e190: 426f 6f6c 6561 6e27 3a0a 2020 2020 2020  Boolean':.      
+0000e1a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000e1b0: 662e 7374 725f 746f 5f63 6c61 7373 2822  f.str_to_class("
+0000e1c0: 6f6d 6572 6f2e 7363 7269 7074 7322 2c20  omero.scripts", 
+0000e1d0: 2242 6f6f 6c22 2c0a 2020 2020 2020 2020  "Bool",.        
 0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 4966 206e 6f20 6272 616e 6368 2069 7320  If no branch is 
-0000e200: 666f 756e 642c 2069 7420 7769 6c6c 2072  found, it will r
-0000e210: 6574 7572 6e20 226d 6173 7465 7222 0a0a  eturn "master"..
-0000e220: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-0000e230: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-0000e240: 6545 7272 6f72 3a20 4966 2074 6865 2069  eError: If the i
-0000e250: 6e70 7574 2055 524c 2069 7320 6e6f 7420  nput URL is not 
-0000e260: 6120 7661 6c69 6420 4769 7448 7562 2055  a valid GitHub U
-0000e270: 524c 2e0a 2020 2020 2020 2020 2222 220a  RL..        """.
-0000e280: 2020 2020 2020 2020 7572 6c5f 7061 7274          url_part
-0000e290: 7320 3d20 696e 7075 745f 7572 6c2e 7370  s = input_url.sp
-0000e2a0: 6c69 7428 222f 2229 0a20 2020 2020 2020  lit("/").       
-0000e2b0: 2069 6620 6c65 6e28 7572 6c5f 7061 7274   if len(url_part
-0000e2c0: 7329 203c 2035 206f 7220 7572 6c5f 7061  s) < 5 or url_pa
-0000e2d0: 7274 735b 325d 2021 3d20 2267 6974 6875  rts[2] != "githu
-0000e2e0: 622e 636f 6d22 3a0a 2020 2020 2020 2020  b.com":.        
-0000e2f0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000e300: 7272 6f72 2822 496e 7661 6c69 6420 4769  rror("Invalid Gi
-0000e310: 7448 7562 2055 524c 2229 0a0a 2020 2020  tHub URL")..    
-0000e320: 2020 2020 6966 2022 7472 6565 2220 696e      if "tree" in
-0000e330: 2075 726c 5f70 6172 7473 3a0a 2020 2020   url_parts:.    
-0000e340: 2020 2020 2020 2020 2320 4361 7365 3a20          # Case: 
-0000e350: 5552 4c20 636f 6e74 6169 6e73 2061 2062  URL contains a b
-0000e360: 7261 6e63 680a 2020 2020 2020 2020 2020  ranch.          
-0000e370: 2020 6272 616e 6368 5f69 6e64 6578 203d    branch_index =
-0000e380: 2075 726c 5f70 6172 7473 2e69 6e64 6578   url_parts.index
-0000e390: 2822 7472 6565 2229 202b 2031 0a20 2020  ("tree") + 1.   
-0000e3a0: 2020 2020 2020 2020 2062 7261 6e63 6820           branch 
-0000e3b0: 3d20 7572 6c5f 7061 7274 735b 6272 616e  = url_parts[bran
-0000e3c0: 6368 5f69 6e64 6578 5d0a 2020 2020 2020  ch_index].      
-0000e3d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e3e0: 2020 2020 2320 4361 7365 3a20 5552 4c20      # Case: URL 
-0000e3f0: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
-0000e400: 2061 2062 7261 6e63 680a 2020 2020 2020   a branch.      
-0000e410: 2020 2020 2020 6272 616e 6368 203d 2022        branch = "
-0000e420: 6d61 7374 6572 220a 0a20 2020 2020 2020  master"..       
-0000e430: 2072 6574 7572 6e20 7572 6c5f 7061 7274   return url_part
-0000e440: 732c 2062 7261 6e63 680a 0a20 2020 2064  s, branch..    d
-0000e450: 6566 2063 6f6e 7665 7274 5f75 726c 2873  ef convert_url(s
-0000e460: 656c 662c 2069 6e70 7574 5f75 726c 3a20  elf, input_url: 
-0000e470: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
-0000e480: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000e490: 2043 6f6e 7665 7274 2074 6865 2069 6e70   Convert the inp
-0000e4a0: 7574 2047 6974 4875 6220 5552 4c20 746f  ut GitHub URL to
-0000e4b0: 2061 6e20 6f75 7470 7574 2055 524c 2074   an output URL t
-0000e4c0: 6861 7420 7265 7472 6965 7665 730a 2020  hat retrieves.  
-0000e4d0: 2020 2020 2020 7468 6520 2764 6573 6372        the 'descr
-0000e4e0: 6970 746f 722e 6a73 6f6e 2720 6669 6c65  iptor.json' file
-0000e4f0: 2069 6e20 7261 7720 666f 726d 6174 2e0a   in raw format..
-0000e500: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000e510: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-0000e520: 5f75 726c 2028 7374 7229 3a20 5468 6520  _url (str): The 
-0000e530: 696e 7075 7420 4769 7448 7562 2055 524c  input GitHub URL
-0000e540: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000e550: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000e560: 7374 723a 2054 6865 206f 7574 7075 7420  str: The output 
-0000e570: 5552 4c20 746f 2074 6865 2027 6465 7363  URL to the 'desc
-0000e580: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
-0000e590: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
-0000e5a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000e5b0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
-0000e5c0: 6865 2069 6e70 7574 2055 524c 2069 7320  he input URL is 
-0000e5d0: 6e6f 7420 6120 7661 6c69 6420 4769 7448  not a valid GitH
-0000e5e0: 7562 2055 524c 2e0a 2020 2020 2020 2020  ub URL..        
-0000e5f0: 2222 220a 2020 2020 2020 2020 7572 6c5f  """.        url_
-0000e600: 7061 7274 732c 2062 7261 6e63 6820 3d20  parts, branch = 
-0000e610: 7365 6c66 2e65 7874 7261 6374 5f70 6172  self.extract_par
-0000e620: 7473 5f66 726f 6d5f 7572 6c28 696e 7075  ts_from_url(inpu
-0000e630: 745f 7572 6c29 0a0a 2020 2020 2020 2020  t_url)..        
-0000e640: 2320 436f 6e73 7472 7563 7420 7468 6520  # Construct the 
-0000e650: 6f75 7470 7574 2055 524c 2062 7920 636f  output URL by co
-0000e660: 6d62 696e 696e 6720 7468 6520 6578 7472  mbining the extr
-0000e670: 6163 7465 6420 696e 666f 726d 6174 696f  acted informatio
-0000e680: 6e0a 2020 2020 2020 2020 2320 7769 7468  n.        # with
-0000e690: 2074 6865 2064 6573 6972 6564 2066 696c   the desired fil
-0000e6a0: 6520 7061 7468 0a20 2020 2020 2020 206f  e path.        o
-0000e6b0: 7574 7075 745f 7572 6c20 3d20 6622 6874  utput_url = f"ht
-0000e6c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000e6d0: 2f7b 7572 6c5f 7061 7274 735b 335d 7d2f  /{url_parts[3]}/
-0000e6e0: 7b75 726c 5f70 6172 7473 5b34 5d7d 2f72  {url_parts[4]}/r
-0000e6f0: 6177 2f7b 6272 616e 6368 7d2f 6465 7363  aw/{branch}/desc
-0000e700: 7269 7074 6f72 2e6a 736f 6e22 0a0a 2020  riptor.json"..  
-0000e710: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-0000e720: 7075 745f 7572 6c0a 0a20 2020 2064 6566  put_url..    def
-0000e730: 2070 756c 6c5f 6465 7363 7269 7074 6f72   pull_descriptor
-0000e740: 5f66 726f 6d5f 6769 7468 7562 2873 656c  _from_github(sel
-0000e750: 662c 2077 6f72 6b66 6c6f 773a 2073 7472  f, workflow: str
-0000e760: 2920 2d3e 2044 6963 743a 0a20 2020 2020  ) -> Dict:.     
-0000e770: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-0000e780: 756c 6c20 7468 6520 776f 726b 666c 6f77  ull the workflow
-0000e790: 2064 6573 6372 6970 746f 7220 6672 6f6d   descriptor from
-0000e7a0: 2047 6974 4875 622e 0a0a 2020 2020 2020   GitHub...      
-0000e7b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000e7c0: 2020 2020 776f 726b 666c 6f77 2028 7374      workflow (st
-0000e7d0: 7229 3a20 5468 6520 776f 726b 666c 6f77  r): The workflow
-0000e7e0: 2066 6f72 2077 6869 6368 2074 6f20 7075   for which to pu
-0000e7f0: 6c6c 2074 6865 2064 6573 6372 6970 746f  ll the descripto
-0000e800: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
-0000e810: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000e820: 2044 6963 743a 2054 6865 204a 534f 4e20   Dict: The JSON 
-0000e830: 6465 7363 7269 7074 6f72 2e0a 0a20 2020  descriptor...   
-0000e840: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-0000e850: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-0000e860: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
-0000e870: 206f 6363 7572 7320 7768 696c 6520 7075   occurs while pu
-0000e880: 6c6c 696e 6720 7468 6520 6465 7363 7269  lling the descri
-0000e890: 7074 6f72 2066 696c 652e 0a20 2020 2020  ptor file..     
-0000e8a0: 2020 2022 2222 0a20 2020 2020 2020 2067     """.        g
-0000e8b0: 6974 5f72 6570 6f20 3d20 7365 6c66 2e73  it_repo = self.s
-0000e8c0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
-0000e8d0: 5b77 6f72 6b66 6c6f 775d 0a20 2020 2020  [workflow].     
-0000e8e0: 2020 2023 2063 6f6e 7665 7274 2067 6974     # convert git
-0000e8f0: 2072 6570 6f20 746f 206a 736f 6e20 6669   repo to json fi
-0000e900: 6c65 0a20 2020 2020 2020 2072 6177 5f75  le.        raw_u
-0000e910: 726c 203d 2073 656c 662e 636f 6e76 6572  rl = self.conver
-0000e920: 745f 7572 6c28 6769 745f 7265 706f 290a  t_url(git_repo).
-0000e930: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000e940: 6562 7567 2866 2250 756c 6c20 776f 726b  ebug(f"Pull work
-0000e950: 666c 6f77 3a20 7b77 6f72 6b66 6c6f 777d  flow: {workflow}
-0000e960: 3a20 7b67 6974 5f72 6570 6f7d 203e 3e20  : {git_repo} >> 
-0000e970: 7b72 6177 5f75 726c 7d22 290a 2020 2020  {raw_url}").    
-0000e980: 2020 2020 2320 7075 6c6c 2077 6f72 6b66      # pull workf
-0000e990: 6c6f 7720 7061 7261 6d73 0a20 2020 2020  low params.     
-0000e9a0: 2020 2067 6974 6875 625f 7365 7373 696f     github_sessio
-0000e9b0: 6e20 3d20 7365 6c66 2e67 6574 5f6f 725f  n = self.get_or_
-0000e9c0: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
-0000e9d0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
-0000e9e0: 6768 6669 6c65 203d 2067 6974 6875 625f  ghfile = github_
-0000e9f0: 7365 7373 696f 6e2e 6765 7428 7261 775f  session.get(raw_
-0000ea00: 7572 6c29 0a20 2020 2020 2020 2069 6620  url).        if 
-0000ea10: 6768 6669 6c65 2e6f 6b3a 0a20 2020 2020  ghfile.ok:.     
-0000ea20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000ea30: 6275 6728 6622 4361 6368 6564 3f20 7b67  bug(f"Cached? {g
-0000ea40: 6866 696c 652e 6672 6f6d 5f63 6163 6865  hfile.from_cache
-0000ea50: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-0000ea60: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
-0000ea70: 3d20 6768 6669 6c65 2e6a 736f 6e28 290a  = ghfile.json().
-0000ea80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ea90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000eaa0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000eab0: 2020 2020 2020 2020 2020 2020 6627 4572              f'Er
-0000eac0: 726f 7220 7768 696c 6520 7075 6c6c 696e  ror while pullin
-0000ead0: 6720 6465 7363 7269 7074 6f72 2066 696c  g descriptor fil
-0000eae0: 6520 666f 7220 776f 726b 666c 6f77 207b  e for workflow {
-0000eaf0: 776f 726b 666c 6f77 7d2c 5c0a 2020 2020  workflow},\.    
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 6672 6f6d 207b 7261 775f 7572 6c7d 3a20  from {raw_url}: 
-0000eb20: 7b67 6866 696c 652e 5f5f 6469 6374 5f5f  {ghfile.__dict__
-0000eb30: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
-0000eb40: 726e 206a 736f 6e5f 6465 7363 7269 7074  rn json_descript
-0000eb50: 6f72 0a0a 2020 2020 6465 6620 6765 745f  or..    def get_
-0000eb60: 6f72 5f63 7265 6174 655f 6769 7468 7562  or_create_github
-0000eb70: 5f73 6573 7369 6f6e 2873 656c 6629 3a0a  _session(self):.
-0000eb80: 2020 2020 2020 2020 2320 4e6f 7465 2c20          # Note, 
-0000eb90: 7573 696e 6720 7265 7175 6573 7473 5f63  using requests_c
-0000eba0: 6163 6865 2031 2e31 2e31 2c20 636f 6e64  ache 1.1.1, cond
-0000ebb0: 6974 696f 6e61 6c20 7175 6572 6965 7320  itional queries 
-0000ebc0: 6172 6520 6465 6661 756c 743a 0a20 2020  are default:.   
-0000ebd0: 2020 2020 2023 2054 6865 2063 6163 6865       # The cache
-0000ebe0: 6420 7265 7370 6f6e 7365 2077 696c 6c20  d response will 
-0000ebf0: 7374 696c 6c20 6265 2075 7365 6420 756e  still be used un
-0000ec00: 7469 6c20 7468 6520 7265 6d6f 7465 2063  til the remote c
-0000ec10: 6f6e 7465 6e74 2061 6374 7561 6c6c 7920  ontent actually 
-0000ec20: 6368 616e 6765 730a 2020 2020 2020 2020  changes.        
-0000ec30: 2320 4576 656e 2069 6620 7468 6520 2765  # Even if the 'e
-0000ec40: 7870 6972 655f 6166 7465 7227 2069 7320  xpire_after' is 
-0000ec50: 7472 6967 6765 7265 642e 2054 6869 7320  triggered. This 
-0000ec60: 6973 2062 7569 6c74 2069 6e74 6f20 4769  is built into Gi
-0000ec70: 7448 7562 2c20 7768 6963 6820 7265 7475  tHub, which retu
-0000ec80: 726e 730a 2020 2020 2020 2020 2320 6120  rns.        # a 
-0000ec90: 4574 6167 2069 6e20 7468 6520 6865 6164  Etag in the head
-0000eca0: 6572 2074 6861 7420 6f6e 6c79 2063 6861  er that only cha
-0000ecb0: 6e67 6573 2077 6865 6e20 7468 6520 636f  nges when the co
-0000ecc0: 6e74 656e 7420 2865 2e67 2e20 7468 6520  ntent (e.g. the 
-0000ecd0: 6465 7363 7269 7074 6f72 2920 6368 616e  descriptor) chan
-0000ece0: 6765 732e 0a20 2020 2020 2020 2023 2049  ges..        # I
-0000ecf0: 6620 796f 7520 7072 6f76 6964 6520 7468  f you provide th
-0000ed00: 6973 2045 7461 6720 7768 656e 2071 7565  is Etag when que
-0000ed10: 7279 696e 672c 2079 6f75 2077 696c 6c20  rying, you will 
-0000ed20: 6765 7420 6120 3330 3420 2827 6e6f 2063  get a 304 ('no c
-0000ed30: 6861 6e67 6527 2920 616e 6420 6974 2077  hange') and it w
-0000ed40: 696c 6c0a 2020 2020 2020 2020 2320 4e4f  ill.        # NO
-0000ed50: 5420 636f 756e 7420 746f 7761 7264 7320  T count towards 
-0000ed60: 796f 7572 2047 6974 6875 6220 6c69 6d69  your Github limi
-0000ed70: 7473 2e20 416e 6420 7265 7175 6573 7473  ts. And requests
-0000ed80: 5f63 6163 6865 2064 6f65 7320 7468 6174  _cache does that
-0000ed90: 2066 6f72 2075 7320 6e6f 772e 0a20 2020   for us now..   
-0000eda0: 2020 2020 2023 204e 6f74 2061 7661 696c       # Not avail
-0000edb0: 6162 6c65 2069 6e20 5079 7468 6f6e 332e  able in Python3.
-0000edc0: 3620 7468 6f75 6768 2e0a 2020 2020 2020  6 though..      
-0000edd0: 2020 7320 3d20 7265 7175 6573 7473 5f63    s = requests_c
-0000ede0: 6163 6865 2e43 6163 6865 6453 6573 7369  ache.CachedSessi
-0000edf0: 6f6e 2827 6769 7468 7562 5f63 6163 6865  on('github_cache
-0000ee00: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee20: 2020 2020 2020 2020 2020 2020 6261 636b              back
-0000ee30: 656e 643d 7365 6c66 2e63 6163 6865 2c0a  end=self.cache,.
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee60: 2020 2020 2020 2020 2065 7870 6972 655f           expire_
-0000ee70: 6166 7465 723d 312c 0a20 2020 2020 2020  after=1,.       
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 2020 6361 6368 655f 636f 6e74 726f 6c3d    cache_control=
-0000eeb0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000eee0: 2020 2020 2020 2020 2320 4d69 6768 7420          # Might 
-0000eef0: 6861 7665 2062 6967 6765 7220 6973 7375  have bigger issu
-0000ef00: 6573 2c20 7468 6973 2069 7320 7265 6c61  es, this is rela
-0000ef10: 7465 6420 746f 2072 6174 6520 6c69 6d69  ted to rate limi
-0000ef20: 7473 206f 6e20 4769 7448 7562 0a20 2020  ts on GitHub.   
-0000ef30: 2020 2020 2023 2068 7474 7073 3a2f 2f64       # https://d
-0000ef40: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
-0000ef50: 6e2f 7265 7374 2f75 7369 6e67 2d74 6865  n/rest/using-the
-0000ef60: 2d72 6573 742d 6170 692f 7261 7465 2d6c  -rest-api/rate-l
-0000ef70: 696d 6974 732d 666f 722d 7468 652d 7265  imits-for-the-re
-0000ef80: 7374 2d61 7069 0a20 2020 2020 2020 2023  st-api.        #
-0000ef90: 2049 6620 6974 2073 7461 7973 2061 2070   If it stays a p
-0000efa0: 726f 626c 656d 2c20 7765 2068 6176 6520  roblem, we have 
-0000efb0: 746f 2061 6464 2061 6e20 6f70 7469 6f6e  to add an option
-0000efc0: 2074 6f20 6164 6420 6120 4748 206b 6579   to add a GH key
-0000efd0: 2074 6f20 7468 6520 636f 6e66 6967 0a20   to the config. 
-0000efe0: 2020 2020 2020 2023 2045 2e67 2e20 7365         # E.g. se
-0000eff0: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-0000f000: 2e63 6f6d 2f72 6571 7565 7374 732d 6361  .com/requests-ca
-0000f010: 6368 652f 7265 7175 6573 7473 2d63 6163  che/requests-cac
-0000f020: 6865 2f62 6c6f 622f 3533 3133 3465 6630  he/blob/53134ef0
-0000f030: 6539 3964 3731 3366 6564 3632 3531 3564  e99d713fed62515d
-0000f040: 6662 3762 6366 6161 6335 6636 3366 3964  fb7bcfaac5f63f9d
-0000f050: 2f65 7861 6d70 6c65 732f 7079 6769 7468  /examples/pygith
-0000f060: 7562 2e70 790a 2020 2020 2020 2020 2320  ub.py.        # 
-0000f070: 4865 7265 2079 6f75 2063 6f75 6c64 2068  Here you could h
-0000f080: 6176 6520 616e 2041 4343 4553 535f 544f  ave an ACCESS_TO
-0000f090: 4b45 4e2e 0a20 2020 2020 2020 2023 2041  KEN..        # A
-0000f0a0: 6e20 4143 4345 5353 5f54 4f4b 454e 2063  n ACCESS_TOKEN c
-0000f0b0: 6f75 6c64 2069 6d70 726f 7665 2061 7069  ould improve api
-0000f0c0: 206c 696d 6974 7320 746f 2035 3030 302f   limits to 5000/
-0000f0d0: 6820 2866 726f 6d20 3630 2f68 292e 0a20  h (from 60/h).. 
-0000f0e0: 2020 2020 2020 2072 6574 7279 5f73 7472         retry_str
-0000f0f0: 6174 6567 7920 3d20 5265 7472 7928 0a20  ategy = Retry(. 
-0000f100: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-0000f110: 3d35 2c20 2020 2020 2020 2020 2020 2020  =5,             
-0000f120: 2020 2320 4d61 7869 6d75 6d20 6e75 6d62    # Maximum numb
-0000f130: 6572 206f 6620 7265 7472 6965 730a 2020  er of retries.  
-0000f140: 2020 2020 2020 2020 2020 2320 4578 706f            # Expo
-0000f150: 6e65 6e74 6961 6c20 6261 636b 6f66 6620  nential backoff 
-0000f160: 6661 6374 6f72 2028 6465 6c61 7920 6265  factor (delay be
-0000f170: 7477 6565 6e20 7265 7472 6965 7329 0a20  tween retries). 
-0000f180: 2020 2020 2020 2020 2020 2062 6163 6b6f             backo
-0000f190: 6666 5f66 6163 746f 723d 352c 0a20 2020  ff_factor=5,.   
-0000f1a0: 2020 2020 2020 2020 2023 2052 6574 7279           # Retry
-0000f1b0: 206f 6e20 7468 6573 6520 4854 5450 2073   on these HTTP s
-0000f1c0: 7461 7475 7320 636f 6465 730a 2020 2020  tatus codes.    
-0000f1d0: 2020 2020 2020 2020 7374 6174 7573 5f66          status_f
-0000f1e0: 6f72 6365 6c69 7374 3d5b 3530 302c 2035  orcelist=[500, 5
-0000f1f0: 3032 2c20 3530 332c 2035 3034 2c20 3430  02, 503, 504, 40
-0000f200: 332c 2034 3239 5d2c 0a20 2020 2020 2020  3, 429],.       
-0000f210: 2020 2020 2061 6c6c 6f77 6564 5f6d 6574       allowed_met
-0000f220: 686f 6473 3d66 726f 7a65 6e73 6574 285b  hods=frozenset([
-0000f230: 2747 4554 275d 2920 2023 204f 6e6c 7920  'GET'])  # Only 
-0000f240: 7265 7472 7920 666f 7220 4745 5420 7265  retry for GET re
-0000f250: 7175 6573 7473 0a20 2020 2020 2020 2029  quests.        )
-0000f260: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
-0000f270: 2827 6874 7470 733a 2f2f 6769 7468 7562  ('https://github
-0000f280: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
-0000f290: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
-0000f2a0: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
-0000f2b0: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
-0000f2c0: 2827 6874 7470 3a2f 2f67 6974 6875 622e  ('http://github.
-0000f2d0: 636f 6d2f 272c 2048 5454 5041 6461 7074  com/', HTTPAdapt
-0000f2e0: 6572 286d 6178 5f72 6574 7269 6573 3d72  er(max_retries=r
-0000f2f0: 6574 7279 5f73 7472 6174 6567 7929 290a  etry_strategy)).
-0000f300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000f310: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
-0000f320: 726b 666c 6f77 5f63 6f6d 6d61 6e64 2873  rkflow_command(s
-0000f330: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 2020 776f 726b 666c 6f77 3a20 7374 722c    workflow: str,
-0000f360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f370: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0000f380: 726b 666c 6f77 5f76 6572 7369 6f6e 3a20  rkflow_version: 
-0000f390: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 2020 696e 7075 745f 6461 7461 3a20 7374    input_data: st
-0000f3c0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3e0: 656d 6169 6c3a 204f 7074 696f 6e61 6c5b  email: Optional[
-0000f3f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f410: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
-0000f420: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000f430: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 2020 202a 2a6b 7761 7267 7329 202d 3e20     **kwargs) -> 
-0000f460: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
-0000f470: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f480: 2020 2020 2020 4765 6e65 7261 7465 2074        Generate t
-0000f490: 6865 2053 6c75 726d 2077 6f72 6b66 6c6f  he Slurm workflo
-0000f4a0: 7720 636f 6d6d 616e 6420 616e 6420 656e  w command and en
-0000f4b0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-0000f4c0: 6c65 732e 0a0a 2020 2020 2020 2020 4172  les...        Ar
-0000f4d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000f4e0: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
-0000f4f0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000f500: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
-0000f510: 2020 2020 2020 776f 726b 666c 6f77 5f76        workflow_v
-0000f520: 6572 7369 6f6e 2028 7374 7229 3a20 5468  ersion (str): Th
-0000f530: 6520 7665 7273 696f 6e20 6f66 2074 6865  e version of the
-0000f540: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-0000f550: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-0000f560: 6120 2873 7472 293a 2054 6865 206e 616d  a (str): The nam
-0000f570: 6520 6f66 2074 6865 2069 6e70 7574 2064  e of the input d
-0000f580: 6174 6120 666f 6c64 6572 2063 6f6e 7461  ata folder conta
-0000f590: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
-0000f5a0: 2020 2020 2020 7468 6520 696e 7075 7420        the input 
-0000f5b0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
-0000f5c0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
-0000f5d0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-0000f5e0: 5468 6520 656d 6169 6c20 6164 6472 6573  The email addres
-0000f5f0: 7320 666f 7220 6a6f 6220 6e6f 7469 6669  s for job notifi
-0000f600: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
-0000f610: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0000f620: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
-0000f630: 2064 6566 6175 6c74 7320 746f 2077 6861   defaults to wha
-0000f640: 7420 6973 2069 6e20 7468 6520 6a6f 6220  t is in the job 
-0000f650: 7363 7269 7074 2e0a 2020 2020 2020 2020  script..        
-0000f660: 2020 2020 7469 6d65 2028 7374 722c 206f      time (str, o
-0000f670: 7074 696f 6e61 6c29 3a20 5468 6520 7469  ptional): The ti
-0000f680: 6d65 206c 696d 6974 2066 6f72 2074 6865  me limit for the
-0000f690: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
-0000f6a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f6b0: 6d61 7420 4848 3a4d 4d3a 5353 2e20 4465  mat HH:MM:SS. De
-0000f6c0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
-0000f6d0: 7768 6963 6820 6465 6661 756c 7473 2074  which defaults t
-0000f6e0: 6f20 7768 6174 200a 2020 2020 2020 2020  o what .        
-0000f6f0: 2020 2020 2020 2020 6973 2069 6e20 7468          is in th
-0000f700: 6520 6a6f 6220 7363 7269 7074 2e0a 2020  e job script..  
-0000f710: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000f720: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
-0000f730: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000f740: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
-0000f750: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
-0000f760: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000f770: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
-0000f780: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000f790: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-0000f7a0: 696e 696e 6720 7468 6520 536c 7572 6d20  ining the Slurm 
-0000f7b0: 776f 726b 666c 6f77 2063 6f6d 6d61 6e64  workflow command
-0000f7c0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000f7d0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
-0000f7e0: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-0000f7f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f800: 2020 2020 206d 6f64 656c 5f70 6174 6820       model_path 
-0000f810: 3d20 7365 6c66 2e73 6c75 726d 5f6d 6f64  = self.slurm_mod
-0000f820: 656c 5f70 6174 6873 5b77 6f72 6b66 6c6f  el_paths[workflo
-0000f830: 772e 6c6f 7765 7228 295d 0a20 2020 2020  w.lower()].     
-0000f840: 2020 206a 6f62 5f73 6372 6970 7420 3d20     job_script = 
-0000f850: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-0000f860: 5f6a 6f62 735b 776f 726b 666c 6f77 2e6c  _jobs[workflow.l
-0000f870: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
-0000f880: 6a6f 625f 7061 7261 6d73 203d 2073 656c  job_params = sel
-0000f890: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
-0000f8a0: 6273 5f70 6172 616d 735b 776f 726b 666c  bs_params[workfl
-0000f8b0: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
-0000f8c0: 2020 2020 2320 6772 6162 206f 6e6c 7920      # grab only 
-0000f8d0: 7468 6520 696d 6167 6520 6e61 6d65 2c20  the image name, 
-0000f8e0: 6e6f 7420 7468 6520 6772 6f75 702f 6372  not the group/cr
-0000f8f0: 6561 746f 720a 2020 2020 2020 2020 696d  eator.        im
-0000f900: 6167 6520 3d20 7365 6c66 2e73 6c75 726d  age = self.slurm
-0000f910: 5f6d 6f64 656c 5f69 6d61 6765 735b 776f  _model_images[wo
-0000f920: 726b 666c 6f77 2e6c 6f77 6572 2829 5d2e  rkflow.lower()].
-0000f930: 7370 6c69 7428 222f 2229 5b31 5d0a 0a20  split("/")[1].. 
-0000f940: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
-0000f950: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
-0000f960: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
-0000f970: 227b 7365 6c66 2e73 6c75 726d 5f64 6174  "{self.slurm_dat
-0000f980: 615f 7061 7468 7d2f 7b69 6e70 7574 5f64  a_path}/{input_d
-0000f990: 6174 617d 222c 0a20 2020 2020 2020 2020  ata}",.         
-0000f9a0: 2020 2022 494d 4147 455f 5041 5448 223a     "IMAGE_PATH":
-0000f9b0: 2066 227b 7365 6c66 2e73 6c75 726d 5f69   f"{self.slurm_i
-0000f9c0: 6d61 6765 735f 7061 7468 7d2f 7b6d 6f64  mages_path}/{mod
-0000f9d0: 656c 5f70 6174 687d 222c 0a20 2020 2020  el_path}",.     
-0000f9e0: 2020 2020 2020 2022 494d 4147 455f 5645         "IMAGE_VE
-0000f9f0: 5253 494f 4e22 3a20 6622 7b77 6f72 6b66  RSION": f"{workf
-0000fa00: 6c6f 775f 7665 7273 696f 6e7d 222c 0a20  low_version}",. 
-0000fa10: 2020 2020 2020 2020 2020 2022 5349 4e47             "SING
-0000fa20: 554c 4152 4954 595f 494d 4147 4522 3a20  ULARITY_IMAGE": 
-0000fa30: 6622 7b69 6d61 6765 7d5f 7b77 6f72 6b66  f"{image}_{workf
-0000fa40: 6c6f 775f 7665 7273 696f 6e7d 2e73 6966  low_version}.sif
-0000fa50: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0000fa60: 5343 5249 5054 5f50 4154 4822 3a20 6622  SCRIPT_PATH": f"
-0000fa70: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
-0000fa80: 7074 5f70 6174 687d 220a 2020 2020 2020  pt_path}".      
-0000fa90: 2020 7d0a 2020 2020 2020 2020 776f 726b    }.        work
-0000faa0: 666c 6f77 5f65 6e76 203d 2073 656c 662e  flow_env = self.
-0000fab0: 776f 726b 666c 6f77 5f70 6172 616d 735f  workflow_params_
-0000fac0: 746f 5f65 6e76 7661 7273 282a 2a6b 7761  to_envvars(**kwa
-0000fad0: 7267 7329 0a20 2020 2020 2020 2065 6e76  rgs).        env
-0000fae0: 203d 207b 2a2a 7362 6174 6368 5f65 6e76   = {**sbatch_env
-0000faf0: 2c20 2a2a 776f 726b 666c 6f77 5f65 6e76  , **workflow_env
-0000fb00: 7d0a 0a20 2020 2020 2020 2065 6d61 696c  }..        email
-0000fb10: 5f70 6172 616d 203d 2022 2220 6966 2065  _param = "" if e
-0000fb20: 6d61 696c 2069 7320 4e6f 6e65 2065 6c73  mail is None els
-0000fb30: 6520 6622 202d 2d6d 6169 6c2d 7573 6572  e f" --mail-user
-0000fb40: 3d7b 656d 6169 6c7d 220a 2020 2020 2020  ={email}".      
-0000fb50: 2020 7469 6d65 5f70 6172 616d 203d 2022    time_param = "
-0000fb60: 2220 6966 2074 696d 6520 6973 204e 6f6e  " if time is Non
-0000fb70: 6520 656c 7365 2066 2220 2d2d 7469 6d65  e else f" --time
-0000fb80: 3d7b 7469 6d65 7d22 0a20 2020 2020 2020  ={time}".       
-0000fb90: 206a 6f62 5f70 6172 616d 732e 6170 7065   job_params.appe
-0000fba0: 6e64 2874 696d 655f 7061 7261 6d29 0a20  nd(time_param). 
-0000fbb0: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
-0000fbc0: 732e 6170 7065 6e64 2865 6d61 696c 5f70  s.append(email_p
-0000fbd0: 6172 616d 290a 2020 2020 2020 2020 6a6f  aram).        jo
-0000fbe0: 625f 7061 7261 6d20 3d20 2222 2e6a 6f69  b_param = "".joi
-0000fbf0: 6e28 6a6f 625f 7061 7261 6d73 290a 2020  n(job_params).  
-0000fc00: 2020 2020 2020 7362 6174 6368 5f63 6d64        sbatch_cmd
-0000fc10: 203d 2066 2273 6261 7463 687b 6a6f 625f   = f"sbatch{job_
-0000fc20: 7061 7261 6d7d 202d 2d6f 7574 7075 743d  param} --output=
-0000fc30: 6f6d 6572 6f2d 256a 2e6c 6f67 205c 0a20  omero-%j.log \. 
-0000fc40: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-0000fc50: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
-0000fc60: 7468 7d2f 7b6a 6f62 5f73 6372 6970 747d  th}/{job_script}
-0000fc70: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000fc80: 6e20 7362 6174 6368 5f63 6d64 2c20 656e  n sbatch_cmd, en
-0000fc90: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
-0000fca0: 6f6e 7665 7273 696f 6e5f 636f 6d6d 616e  onversion_comman
-0000fcb0: 6428 7365 6c66 2c20 6461 7461 5f70 6174  d(self, data_pat
-0000fcc0: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
-0000fcf0: 6c65 3a20 7374 722c 0a20 2020 2020 2020  le: str,.       
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
-0000fd20: 6f72 6d61 743a 2073 7472 203d 2027 7a61  ormat: str = 'za
-0000fd30: 7272 272c 0a20 2020 2020 2020 2020 2020  rr',.           
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
-0000fd60: 743a 2073 7472 203d 2027 7469 6666 2729  t: str = 'tiff')
-0000fd70: 202d 3e20 5475 706c 655b 7374 722c 2044   -> Tuple[str, D
-0000fd80: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
-0000fd90: 220a 2020 2020 2020 2020 4765 6e65 7261  ".        Genera
-0000fda0: 7465 2053 6c75 726d 2063 6f6e 7665 7273  te Slurm convers
-0000fdb0: 696f 6e20 636f 6d6d 616e 6420 616e 6420  ion command and 
-0000fdc0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-0000fdd0: 6162 6c65 7320 666f 7220 6461 7461 2063  ables for data c
-0000fde0: 6f6e 7665 7273 696f 6e2e 0a0a 2020 2020  onversion...    
-0000fdf0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000fe00: 2020 2020 2020 6461 7461 5f70 6174 6820        data_path 
-0000fe10: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
-0000fe20: 6865 2064 6174 6120 666f 6c64 6572 2e0a  he data folder..
-0000fe30: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-0000fe40: 6967 5f66 696c 6520 2873 7472 293a 2050  ig_file (str): P
-0000fe50: 6174 6820 746f 2074 6865 2063 6f6e 6669  ath to the confi
-0000fe60: 6775 7261 7469 6f6e 2066 696c 652e 0a20  guration file.. 
-0000fe70: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0000fe80: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
-0000fe90: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
-0000fea0: 6174 2028 6465 6661 756c 7420 6973 2027  at (default is '
-0000feb0: 7a61 7272 2729 2e0a 2020 2020 2020 2020  zarr')..        
-0000fec0: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
-0000fed0: 7420 2873 7472 293a 2054 6172 6765 7420  t (str): Target 
-0000fee0: 6461 7461 2066 6f72 6d61 7420 2864 6566  data format (def
-0000fef0: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
-0000ff00: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000ff10: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0000ff20: 7570 6c65 5b73 7472 2c20 4469 6374 5d3a  uple[str, Dict]:
-0000ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ff40: 2041 2074 7570 6c65 2063 6f6e 7461 696e   A tuple contain
-0000ff50: 696e 6720 7468 6520 536c 7572 6d20 636f  ing the Slurm co
-0000ff60: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
-0000ff70: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000ff80: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
-0000ff90: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-0000ffa0: 0a20 2020 2020 2020 2057 6172 6e69 6e67  .        Warning
-0000ffb0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-0000ffc0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
-0000ffd0: 656e 7461 7469 6f6e 206f 6e6c 7920 7375  entation only su
-0000ffe0: 7070 6f72 7473 2063 6f6e 7665 7273 696f  pports conversio
-0000fff0: 6e20 6672 6f6d 2027 7a61 7272 2720 746f  n from 'zarr' to
-00010000: 2027 7469 6666 272e 0a20 2020 2020 2020   'tiff'..       
-00010010: 2020 2020 2049 6620 7573 696e 6720 6f74       If using ot
-00010020: 6865 7220 736f 7572 6365 206f 7220 7461  her source or ta
-00010030: 7267 6574 2066 6f72 6d61 7473 2c20 7573  rget formats, us
-00010040: 6572 7320 6d75 7374 2069 6d70 6c65 6d65  ers must impleme
-00010050: 6e74 2061 6e64 2063 6f6e 6669 6775 7265  nt and configure
-00010060: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00010070: 6974 696f 6e61 6c20 636f 6e76 6572 7465  itional converte
-00010080: 7273 2074 6865 6d73 656c 7665 732e 0a20  rs themselves.. 
-00010090: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000100a0: 2020 2069 6620 736f 7572 6365 5f66 6f72     if source_for
-000100b0: 6d61 7420 213d 2022 7a61 7272 2220 6f72  mat != "zarr" or
-000100c0: 2074 6172 6765 745f 666f 726d 6174 2021   target_format !
-000100d0: 3d20 2274 6966 6622 3a0a 2020 2020 2020  = "tiff":.      
-000100e0: 2020 2020 2020 2320 5761 726e 2061 626f        # Warn abo
-000100f0: 7574 2075 6e73 7570 706f 7274 6564 2063  ut unsupported c
-00010100: 6f6e 7665 7273 696f 6e3b 2061 6464 6974  onversion; addit
-00010110: 696f 6e61 6c20 636f 6e76 6572 7465 7273  ional converters
-00010120: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
-00010130: 2020 2020 2320 6164 6465 6420 6f75 7473      # added outs
-00010140: 6964 6520 6f75 7220 6b6e 6f77 6c65 6467  ide our knowledg
-00010150: 652e 0a20 2020 2020 2020 2020 2020 2023  e..            #
-00010160: 2043 6865 636b 696e 6720 536c 7572 6d27   Checking Slurm'
-00010170: 7320 6073 6c75 726d 5f63 6f6e 7665 7274  s `slurm_convert
-00010180: 6572 735f 7061 7468 6020 6973 2073 6b69  ers_path` is ski
-00010190: 7070 6564 2066 6f72 0a20 2020 2020 2020  pped for.       
-000101a0: 2020 2020 2023 2070 6572 666f 726d 616e       # performan
-000101b0: 6365 2072 6561 736f 6e73 2e0a 2020 2020  ce reasons..    
-000101c0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-000101d0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-000101e0: 2020 2020 2020 2020 6622 436f 6e76 6572          f"Conver
-000101f0: 7369 6f6e 2066 726f 6d20 7b73 6f75 7263  sion from {sourc
-00010200: 655f 666f 726d 6174 7d20 746f 207b 7461  e_format} to {ta
-00010210: 7267 6574 5f66 6f72 6d61 747d 2069 7320  rget_format} is 
-00010220: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00010230: 2064 6566 6175 6c74 2122 290a 0a20 2020   default!")..   
-00010240: 2020 2020 2063 686f 7365 6e5f 636f 6e76       chosen_conv
-00010250: 6572 7465 7220 3d20 6622 636f 6e76 6572  erter = f"conver
-00010260: 745f 7b73 6f75 7263 655f 666f 726d 6174  t_{source_format
-00010270: 7d5f 746f 5f7b 7461 7267 6574 5f66 6f72  }_to_{target_for
-00010280: 6d61 747d 2e73 6966 220a 2020 2020 2020  mat}.sif".      
-00010290: 2020 7362 6174 6368 5f65 6e76 203d 207b    sbatch_env = {
-000102a0: 0a20 2020 2020 2020 2020 2020 2022 4441  .            "DA
-000102b0: 5441 5f50 4154 4822 3a20 6622 7b64 6174  TA_PATH": f"{dat
-000102c0: 615f 7061 7468 7d22 2c0a 2020 2020 2020  a_path}",.      
-000102d0: 2020 2020 2020 2243 4f4e 5645 5253 494f        "CONVERSIO
-000102e0: 4e5f 5041 5448 223a 2066 227b 7365 6c66  N_PATH": f"{self
-000102f0: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
-00010300: 735f 7061 7468 7d22 2c0a 2020 2020 2020  s_path}",.      
-00010310: 2020 2020 2020 2243 4f4e 5645 5254 4552        "CONVERTER
-00010320: 5f49 4d41 4745 223a 2063 686f 7365 6e5f  _IMAGE": chosen_
-00010330: 636f 6e76 6572 7465 722c 0a20 2020 2020  converter,.     
-00010340: 2020 2020 2020 2022 5343 5249 5054 5f50         "SCRIPT_P
-00010350: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
-00010360: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
-00010370: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00010380: 434f 4e46 4947 5f46 494c 4522 3a20 6622  CONFIG_FILE": f"
-00010390: 7b63 6f6e 6669 675f 6669 6c65 7d22 0a20  {config_file}". 
-000103a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000103b0: 2020 636f 6e76 6572 7369 6f6e 5f63 6d64    conversion_cmd
-000103c0: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
-000103d0: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
-000103e0: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
-000103f0: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
-00010400: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
-00010410: 2d2d 6172 7261 793d 312d 244e 2024 5343  --array=1-$N $SC
-00010420: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
-00010430: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
-00010440: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-00010450: 7369 6f6e 5f63 6d64 5f77 6169 7469 6e67  sion_cmd_waiting
-00010460: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
-00010470: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
-00010480: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
-00010490: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
-000104a0: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
-000104b0: 2d2d 6172 7261 793d 312d 244e 202d 2d77  --array=1-$N --w
-000104c0: 6169 7420 2453 4352 4950 545f 5041 5448  ait $SCRIPT_PATH
-000104d0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
-000104e0: 6179 2e73 6822 0a0a 2020 2020 2020 2020  ay.sh"..        
-000104f0: 7265 7475 726e 2063 6f6e 7665 7273 696f  return conversio
-00010500: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
-00010510: 760a 0a20 2020 2064 6566 2077 6f72 6b66  v..    def workf
-00010520: 6c6f 775f 7061 7261 6d73 5f74 6f5f 656e  low_params_to_en
-00010530: 7676 6172 7328 7365 6c66 2c20 2a2a 6b77  vvars(self, **kw
-00010540: 6172 6773 2920 2d3e 2044 6963 743a 0a20  args) -> Dict:. 
-00010550: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010560: 2020 2043 6f6e 7665 7274 2077 6f72 6b66     Convert workf
-00010570: 6c6f 7720 7061 7261 6d65 7465 7273 2074  low parameters t
-00010580: 6f20 656e 7669 726f 6e6d 656e 7420 7661  o environment va
-00010590: 7269 6162 6c65 732e 0a0a 2020 2020 2020  riables...      
-000105a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000105b0: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
-000105c0: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
-000105d0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-000105e0: 6865 2077 6f72 6b66 6c6f 772e 0a0a 2020  he workflow...  
-000105f0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00010600: 2020 2020 2020 2020 2020 2044 6963 743a             Dict:
-00010610: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
-00010620: 6e74 6169 6e69 6e67 2074 6865 2065 6e76  ntaining the env
-00010630: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00010640: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00010650: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-00010660: 5f65 6e76 203d 207b 6b65 792e 7570 7065  _env = {key.uppe
-00010670: 7228 293a 2066 227b 7661 6c75 657d 2220  r(): f"{value}" 
-00010680: 666f 7220 6b65 792c 0a20 2020 2020 2020  for key,.       
-00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2076 616c 7565 2069 6e20 6b77 6172 6773   value in kwargs
-000106b0: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
-000106c0: 2020 6c6f 6767 6572 2e64 6562 7567 2877    logger.debug(w
-000106d0: 6f72 6b66 6c6f 775f 656e 7629 0a20 2020  orkflow_env).   
-000106e0: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
-000106f0: 666c 6f77 5f65 6e76 0a0a 2020 2020 6465  flow_env..    de
-00010700: 6620 6765 745f 6365 6c6c 706f 7365 5f63  f get_cellpose_c
-00010710: 6f6d 6d61 6e64 2873 656c 662c 2069 6d61  ommand(self, ima
-00010720: 6765 5f76 6572 7369 6f6e 3a20 7374 722c  ge_version: str,
-00010730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010740: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00010750: 7075 745f 6461 7461 3a20 7374 722c 0a20  put_data: str,. 
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2020 2020 2020 2020 2020 6370 5f6d              cp_m
-00010780: 6f64 656c 3a20 7374 722c 0a20 2020 2020  odel: str,.     
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 6e75 635f 6368 616e          nuc_chan
-000107b0: 6e65 6c3a 2069 6e74 2c0a 2020 2020 2020  nel: int,.      
-000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 2020 2020 2020 2070 726f 625f 7468 7265         prob_thre
-000107e0: 7368 6f6c 643a 2066 6c6f 6174 2c0a 2020  shold: float,.  
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-00010810: 6469 616d 6574 6572 3a20 666c 6f61 742c  diameter: float,
-00010820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010830: 2020 2020 2020 2020 2020 2020 2020 656d                em
-00010840: 6169 6c3a 204f 7074 696f 6e61 6c5b 7374  ail: Optional[st
-00010850: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2020 2020 2020 7469 6d65 3a20 4f70          time: Op
-00010880: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00010890: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2075 7365 5f67 7075 3a20 626f 6f6c 203d   use_gpu: bool =
-000108c0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 6d6f 6465 6c3a 2073 7472 203d      model: str =
-000108f0: 2022 6365 6c6c 706f 7365 2229 202d 3e20   "cellpose") -> 
-00010900: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
-00010910: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010920: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
-00010930: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
-00010940: 6972 6f6e 6d65 6e74 2064 6963 7469 6f6e  ironment diction
-00010950: 6172 7920 746f 2072 756e 2061 2043 656c  ary to run a Cel
-00010960: 6c50 6f73 6520 6a6f 620a 2020 2020 2020  lPose job.      
-00010970: 2020 6f6e 2074 6865 2053 6c75 726d 2077    on the Slurm w
-00010980: 6f72 6b6c 6f61 6420 6d61 6e61 6765 722e  orkload manager.
-00010990: 0a20 2020 2020 2020 2041 2073 7065 6369  .        A speci
-000109a0: 6669 6320 6578 616d 706c 6520 6f66 2075  fic example of u
-000109b0: 7369 6e67 2074 6865 2067 656e 6572 6963  sing the generic
-000109c0: 2027 6765 745f 776f 726b 666c 6f77 5f63   'get_workflow_c
-000109d0: 6f6d 6d61 6e64 272e 0a0a 2020 2020 2020  ommand'...      
-000109e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000109f0: 2020 2020 696d 6167 655f 7665 7273 696f      image_versio
-00010a00: 6e20 2873 7472 293a 2054 6865 2076 6572  n (str): The ver
-00010a10: 7369 6f6e 206f 6620 7468 6520 5369 6e67  sion of the Sing
-00010a20: 756c 6172 6974 7920 696d 6167 6520 746f  ularity image to
-00010a30: 2075 7365 2e0a 2020 2020 2020 2020 2020   use..          
-00010a40: 2020 696e 7075 745f 6461 7461 2028 7374    input_data (st
-00010a50: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
-00010a60: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
-00010a70: 6f6c 6465 7220 6f6e 2074 6865 2073 6861  older on the sha
-00010a80: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
-00010a90: 2020 2020 6669 6c65 2073 7973 7465 6d2e      file system.
-00010aa0: 0a20 2020 2020 2020 2020 2020 2063 705f  .            cp_
-00010ab0: 6d6f 6465 6c20 2873 7472 293a 2054 6865  model (str): The
-00010ac0: 206e 616d 6520 6f66 2074 6865 2043 656c   name of the Cel
-00010ad0: 6c50 6f73 6520 6d6f 6465 6c20 746f 2075  lPose model to u
-00010ae0: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
-00010af0: 6e75 635f 6368 616e 6e65 6c20 2869 6e74  nuc_channel (int
-00010b00: 293a 2054 6865 2069 6e64 6578 206f 6620  ): The index of 
-00010b10: 7468 6520 6e75 636c 6561 7220 6368 616e  the nuclear chan
-00010b20: 6e65 6c2e 0a20 2020 2020 2020 2020 2020  nel..           
-00010b30: 2070 726f 625f 7468 7265 7368 6f6c 6420   prob_threshold 
-00010b40: 2866 6c6f 6174 293a 2054 6865 2070 726f  (float): The pro
-00010b50: 6261 6269 6c69 7479 2074 6872 6573 686f  bability thresho
-00010b60: 6c64 2066 6f72 0a20 2020 2020 2020 2020  ld for.         
-00010b70: 2020 2020 2020 206e 7563 6c65 6920 6465         nuclei de
-00010b80: 7465 6374 696f 6e2e 0a20 2020 2020 2020  tection..       
-00010b90: 2020 2020 2063 656c 6c5f 6469 616d 6574       cell_diamet
-00010ba0: 6572 2028 666c 6f61 7429 3a20 5468 6520  er (float): The 
-00010bb0: 6578 7065 6374 6564 2063 656c 6c20 6469  expected cell di
-00010bc0: 616d 6574 6572 2069 6e20 7069 7865 6c73  ameter in pixels
-00010bd0: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
-00010be0: 6169 6c20 284f 7074 696f 6e61 6c5b 7374  ail (Optional[st
-00010bf0: 725d 293a 2054 6865 2065 6d61 696c 2061  r]): The email a
-00010c00: 6464 7265 7373 2074 6f20 7365 6e64 206e  ddress to send n
-00010c10: 6f74 6966 6963 6174 696f 6e73 2074 6f2e  otifications to.
-00010c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c30: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00010c40: 652e 0a20 2020 2020 2020 2020 2020 2074  e..            t
-00010c50: 696d 6520 284f 7074 696f 6e61 6c5b 7374  ime (Optional[st
-00010c60: 725d 293a 2054 6865 206d 6178 696d 756d  r]): The maximum
-00010c70: 2074 696d 6520 666f 7220 7468 6520 6a6f   time for the jo
-00010c80: 6220 746f 2072 756e 2e0a 2020 2020 2020  b to run..      
-00010c90: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00010ca0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00010cb0: 2020 2020 2020 2020 7573 655f 6770 7520          use_gpu 
-00010cc0: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
-00010cd0: 746f 2075 7365 2047 5055 2066 6f72 2074  to use GPU for t
-00010ce0: 6865 2043 656c 6c50 6f73 6520 6a6f 622e  he CellPose job.
-00010cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d00: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00010d10: 652e 0a20 2020 2020 2020 2020 2020 206d  e..            m
-00010d20: 6f64 656c 2028 7374 7229 3a20 5468 6520  odel (str): The 
-00010d30: 6e61 6d65 206f 6620 7468 6520 666f 6c64  name of the fold
-00010d40: 6572 206f 6620 7468 6520 446f 636b 6572  er of the Docker
-00010d50: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00010d70: 6566 6175 6c74 7320 746f 2022 6365 6c6c  efaults to "cell
-00010d80: 706f 7365 222e 0a0a 2020 2020 2020 2020  pose"...        
-00010d90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00010da0: 2020 2020 2054 7570 6c65 5b73 7472 2c20       Tuple[str, 
-00010db0: 6469 6374 5d3a 0a20 2020 2020 2020 2020  dict]:.         
-00010dc0: 2020 2020 2020 2041 2074 7570 6c65 2063         A tuple c
-00010dd0: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
-00010de0: 7572 6d20 7362 6174 6368 2063 6f6d 6d61  urm sbatch comma
-00010df0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00010e00: 2020 2061 6e64 2074 6865 2065 6e76 6972     and the envir
-00010e10: 6f6e 6d65 6e74 2064 6963 7469 6f6e 6172  onment dictionar
-00010e20: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-00010e30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00010e40: 6c66 2e67 6574 5f77 6f72 6b66 6c6f 775f  lf.get_workflow_
-00010e50: 636f 6d6d 616e 6428 776f 726b 666c 6f77  command(workflow
-00010e60: 3d6d 6f64 656c 2c0a 2020 2020 2020 2020  =model,.        
-00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
-00010ea0: 6e3d 696d 6167 655f 7665 7273 696f 6e2c  n=image_version,
-00010eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-00010ee0: 6461 7461 3d69 6e70 7574 5f64 6174 612c  data=input_data,
-00010ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 2020 2020 2020 2020 656d 6169 6c3d            email=
-00010f20: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 7469 6d65 3d74 696d 652c 0a20 2020 2020  time=time,.     
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 2020 6370 5f6d 6f64 656c 3d63 705f      cp_model=cp_
-00010f90: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fc0: 6e75 635f 6368 616e 6e65 6c3d 6e75 635f  nuc_channel=nuc_
-00010fd0: 6368 616e 6e65 6c2c 0a20 2020 2020 2020  channel,.       
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 7072 6f62 5f74 6872 6573 686f 6c64    prob_threshold
-00011010: 3d70 726f 625f 7468 7265 7368 6f6c 642c  =prob_threshold,
-00011020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 2020 2020 2020 6365 6c6c 5f64            cell_d
-00011050: 6961 6d65 7465 723d 6365 6c6c 5f64 6961  iameter=cell_dia
-00011060: 6d65 7465 722c 0a20 2020 2020 2020 2020  meter,.         
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 7573 655f 6770 753d 7573 655f 6770 7529  use_gpu=use_gpu)
-000110a0: 0a0a 2020 2020 6465 6620 636f 7079 5f7a  ..    def copy_z
-000110b0: 6970 5f6c 6f63 616c 6c79 2873 656c 662c  ip_locally(self,
-000110c0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
-000110d0: 6765 3a20 7374 722c 2066 696c 656e 616d  ge: str, filenam
-000110e0: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011100: 2920 2d3e 2054 7261 6e73 6665 7252 6573  ) -> TransferRes
-00011110: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
-00011120: 2043 6f70 7920 6120 7a69 7020 6669 6c65   Copy a zip file
-00011130: 2066 726f 6d20 536c 7572 6d20 746f 2074   from Slurm to t
-00011140: 6865 206c 6f63 616c 2073 6572 7665 722e  he local server.
-00011150: 0a0a 2020 2020 2020 2020 4e6f 7465 2061  ..        Note a
-00011160: 626f 7574 2028 5472 616e 7366 6572 2952  bout (Transfer)R
-00011170: 6573 756c 743a 0a0a 2020 2020 2020 2020  esult:..        
-00011180: 556e 6c69 6b65 2073 696d 696c 6172 2063  Unlike similar c
-00011190: 6c61 7373 6573 2073 7563 6820 6173 2069  lasses such as i
-000111a0: 6e76 6f6b 652e 7275 6e6e 6572 732e 5265  nvoke.runners.Re
-000111b0: 7375 6c74 206f 720a 2020 2020 2020 2020  sult or.        
-000111c0: 6661 6272 6963 2e72 756e 6e65 7273 2e52  fabric.runners.R
-000111d0: 6573 756c 740a 2020 2020 2020 2020 2877  esult.        (w
-000111e0: 6869 6368 2068 6176 6520 6120 636f 6e63  hich have a conc
-000111f0: 6570 7420 6f66 20e2 809c 7761 726e 2061  ept of ...warn a
-00011200: 6e64 2072 6574 7572 6e20 616e 7977 6179  nd return anyway
-00011210: 7320 6f6e 2066 6169 6c75 7265 e280 9d29  s on failure...)
-00011220: 0a20 2020 2020 2020 2074 6869 7320 636c  .        this cl
-00011230: 6173 7320 6861 7320 6e6f 2075 7365 6675  ass has no usefu
-00011240: 6c20 7472 7574 6869 6e65 7373 2062 6568  l truthiness beh
-00011250: 6176 696f 722e 0a20 2020 2020 2020 2049  avior..        I
-00011260: 6620 6120 6669 6c65 2074 7261 6e73 6665  f a file transfe
-00011270: 7220 6661 696c 732c 2073 6f6d 6520 6578  r fails, some ex
-00011280: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
-00011290: 7261 6973 6564 2c0a 2020 2020 2020 2020  raised,.        
-000112a0: 6569 7468 6572 2061 6e20 4f53 4572 726f  either an OSErro
-000112b0: 7220 6f72 2061 6e20 6572 726f 7220 6672  r or an error fr
-000112c0: 6f6d 2077 6974 6869 6e20 5061 7261 6d69  om within Parami
-000112d0: 6b6f 2e0a 0a20 2020 2020 2020 2041 7267  ko...        Arg
-000112e0: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-000112f0: 6f63 616c 5f74 6d70 5f73 746f 7261 6765  ocal_tmp_storage
-00011300: 2028 5374 7269 6e67 293a 2050 6174 6820   (String): Path 
-00011310: 746f 2073 746f 7265 2074 6865 207a 6970  to store the zip
-00011320: 2066 696c 6520 6c6f 6361 6c6c 792e 0a20   file locally.. 
-00011330: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-00011340: 616d 6520 2853 7472 696e 6729 3a20 5a69  ame (String): Zi
-00011350: 7020 6669 6c65 6e61 6d65 206f 6e20 536c  p filename on Sl
-00011360: 7572 6d2e 0a0a 2020 2020 2020 2020 5265  urm...        Re
-00011370: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00011380: 2020 2054 7261 6e73 6665 7252 6573 756c     TransferResul
-00011390: 743a 2054 6865 2072 6573 756c 7420 6f66  t: The result of
-000113a0: 2074 6865 2073 6370 2061 7474 656d 7074   the scp attempt
-000113b0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000113c0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000113d0: 6f28 6622 436f 7079 696e 6720 7a69 7020  o(f"Copying zip 
-000113e0: 7b66 696c 656e 616d 657d 2066 726f 6d5c  {filename} from\
-000113f0: 0a20 2020 2020 2020 2020 2020 2053 6c75  .            Slu
-00011400: 726d 2074 6f20 7b6c 6f63 616c 5f74 6d70  rm to {local_tmp
-00011410: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
-00011420: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011430: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00011440: 2072 656d 6f74 653d 6622 7b66 696c 656e   remote=f"{filen
-00011450: 616d 657d 2e7a 6970 222c 0a20 2020 2020  ame}.zip",.     
-00011460: 2020 2020 2020 206c 6f63 616c 3d6c 6f63         local=loc
-00011470: 616c 5f74 6d70 5f73 746f 7261 6765 290a  al_tmp_storage).
-00011480: 0a20 2020 2064 6566 207a 6970 5f64 6174  .    def zip_dat
-00011490: 615f 6f6e 5f73 6c75 726d 5f73 6572 7665  a_on_slurm_serve
-000114a0: 7228 7365 6c66 2c20 6461 7461 5f6c 6f63  r(self, data_loc
-000114b0: 6174 696f 6e3a 2073 7472 2c20 6669 6c65  ation: str, file
-000114c0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 2020 2020 2020 2020 2020 2020 656e 763a              env:
-000114f0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-00011500: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
-00011510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2920 2d3e 2052 6573 756c 743a 0a20    ) -> Result:. 
-00011540: 2020 2020 2020 2022 2222 5a69 7020 7468         """Zip th
-00011550: 6520 6f75 7470 7574 2066 6f6c 6465 7220  e output folder 
-00011560: 6f66 2061 206a 6f62 206f 6e20 536c 7572  of a job on Slur
-00011570: 6d0a 0a20 2020 2020 2020 2041 7267 733a  m..        Args:
-00011580: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00011590: 615f 6c6f 6361 7469 6f6e 2028 5374 7269  a_location (Stri
-000115a0: 6e67 293a 2046 6f6c 6465 7220 6f6e 2053  ng): Folder on S
-000115b0: 4c55 524d 2077 6974 6820 7468 6520 2264  LURM with the "d
-000115c0: 6174 612f 6f75 7422 0a20 2020 2020 2020  ata/out".       
-000115d0: 2020 2020 2020 2020 2073 7562 666f 6c64           subfold
-000115e0: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-000115f0: 6669 6c65 6e61 6d65 2028 5374 7269 6e67  filename (String
-00011600: 293a 204e 616d 6520 746f 2067 6976 6520  ): Name to give 
-00011610: 746f 2074 6865 207a 6970 6669 6c65 2e0a  to the zipfile..
-00011620: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00011630: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
-00011640: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
-00011650: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
-00011660: 2076 6172 6961 626c 6573 2074 6f20 0a20   variables to . 
-00011670: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011680: 6574 2077 6865 6e20 7275 6e6e 696e 6720  et when running 
-00011690: 7468 6520 636f 6d6d 616e 642e 2044 6566  the command. Def
-000116a0: 6175 6c74 7320 746f 204e 6f6e 652e 0a0a  aults to None...
-000116b0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000116c0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
-000116d0: 756c 743a 2054 6865 2072 6573 756c 7420  ult: The result 
-000116e0: 6f66 2074 6865 207a 6970 2061 7474 656d  of the zip attem
-000116f0: 7074 2e0a 2020 2020 2020 2020 2222 220a  pt..        """.
-00011700: 2020 2020 2020 2020 2320 7a69 700a 2020          # zip.  
-00011710: 2020 2020 2020 7a69 705f 636d 6420 3d20        zip_cmd = 
-00011720: 7365 6c66 2e67 6574 5f7a 6970 5f63 6f6d  self.get_zip_com
-00011730: 6d61 6e64 2864 6174 615f 6c6f 6361 7469  mand(data_locati
-00011740: 6f6e 2c20 6669 6c65 6e61 6d65 290a 2020  on, filename).  
-00011750: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00011760: 6f28 6622 5a69 7070 696e 6720 7b64 6174  o(f"Zipping {dat
-00011770: 615f 6c6f 6361 7469 6f6e 7d20 6173 207b  a_location} as {
-00011780: 6669 6c65 6e61 6d65 7d20 6f6e 2053 6c75  filename} on Slu
-00011790: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
-000117a0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
-000117b0: 6d61 6e64 7328 5b7a 6970 5f63 6d64 5d2c  mands([zip_cmd],
-000117c0: 2065 6e76 3d65 6e76 290a 0a20 2020 2064   env=env)..    d
-000117d0: 6566 2067 6574 5f7a 6970 5f63 6f6d 6d61  ef get_zip_comma
-000117e0: 6e64 2873 656c 662c 2064 6174 615f 6c6f  nd(self, data_lo
-000117f0: 6361 7469 6f6e 3a20 7374 722c 2066 696c  cation: str, fil
-00011800: 656e 616d 653a 2073 7472 2920 2d3e 2073  ename: str) -> s
-00011810: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
-00011820: 2020 2020 2020 2020 4765 6e65 7261 7465          Generate
-00011830: 2061 2063 6f6d 6d61 6e64 2073 7472 696e   a command strin
-00011840: 6720 666f 7220 7a69 7070 696e 6720 7468  g for zipping th
-00011850: 6520 6461 7461 206f 6e20 536c 7572 6d2e  e data on Slurm.
-00011860: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00011870: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00011880: 5f6c 6f63 6174 696f 6e20 2873 7472 293a  _location (str):
-00011890: 2054 6865 2066 6f6c 6465 7220 746f 2062   The folder to b
-000118a0: 6520 7a69 7070 6564 2e0a 2020 2020 2020  e zipped..      
-000118b0: 2020 2020 2020 6669 6c65 6e61 6d65 2028        filename (
-000118c0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-000118d0: 6620 7468 6520 7a69 7020 6172 6368 6976  f the zip archiv
-000118e0: 6520 6669 6c65 2074 6f20 6578 7472 6163  e file to extrac
-000118f0: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
-00011900: 2020 2057 6974 686f 7574 2065 7874 656e     Without exten
-00011910: 7369 6f6e 2e0a 0a20 2020 2020 2020 2052  sion...        R
-00011920: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00011930: 2020 2020 7374 723a 2054 6865 2063 6f6d      str: The com
-00011940: 6d61 6e64 2074 6f20 6372 6561 7465 2074  mand to create t
-00011950: 6865 207a 6970 2066 696c 652e 0a20 2020  he zip file..   
-00011960: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011970: 2072 6574 7572 6e20 7365 6c66 2e5f 5a49   return self._ZI
-00011980: 505f 434d 442e 666f 726d 6174 2866 696c  P_CMD.format(fil
-00011990: 656e 616d 653d 6669 6c65 6e61 6d65 2c0a  ename=filename,.
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
-000119d0: 6e3d 6461 7461 5f6c 6f63 6174 696f 6e29  n=data_location)
-000119e0: 0a0a 2020 2020 6465 6620 6765 745f 6c6f  ..    def get_lo
-000119f0: 6766 696c 655f 6672 6f6d 5f73 6c75 726d  gfile_from_slurm
-00011a00: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
-00011a30: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
-00011a60: 705f 7374 6f72 6167 653a 2073 7472 203d  p_storage: str =
-00011a70: 2022 2f74 6d70 2f22 2c0a 2020 2020 2020   "/tmp/",.      
-00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00011aa0: 3a20 7374 7220 3d20 4e6f 6e65 0a20 2020  : str = None.   
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-00011ad0: 2054 7570 6c65 5b73 7472 2c20 7374 722c   Tuple[str, str,
-00011ae0: 2054 7261 6e73 6665 7252 6573 756c 745d   TransferResult]
-00011af0: 3a0a 2020 2020 2020 2020 2222 2243 6f70  :.        """Cop
-00011b00: 7920 7468 6520 6c6f 6766 696c 6520 6f66  y the logfile of
-00011b10: 2074 6865 2067 6976 656e 2053 4c55 524d   the given SLURM
-00011b20: 206a 6f62 2074 6f20 7468 6520 6c6f 6361   job to the loca
-00011b30: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
-00011b40: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
-00011b50: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
-00011b60: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
-00011b70: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
-00011b80: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
-00011b90: 756e 6e65 7273 2e52 6573 756c 740a 2020  unners.Result.  
-00011ba0: 2020 2020 2020 6f72 2066 6162 7269 632e        or fabric.
-00011bb0: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
-00011bc0: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
-00011bd0: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
-00011be0: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
-00011bf0: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
-00011c00: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
-00011c10: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
-00011c20: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
-00011c30: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
-00011c40: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
-00011c50: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
-00011c60: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
-00011c70: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
-00011c80: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
-00011c90: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
-00011ca0: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
-00011cb0: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
-00011cc0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00011cd0: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
-00011ce0: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
-00011cf0: 4944 206f 6620 7468 6520 534c 5552 4d20  ID of the SLURM 
-00011d00: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
-00011d10: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
-00011d20: 6765 2028 7374 722c 206f 7074 696f 6e61  ge (str, optiona
-00011d30: 6c29 3a20 5061 7468 2074 6f20 7374 6f72  l): Path to stor
-00011d40: 6520 7468 6520 6c6f 6766 696c 6520 0a20  e the logfile . 
-00011d50: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011d60: 6f63 616c 6c79 2e20 4465 6661 756c 7473  ocally. Defaults
-00011d70: 2074 6f20 222f 746d 702f 222e 0a20 2020   to "/tmp/"..   
-00011d80: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00011d90: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00011da0: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
-00011db0: 6766 696c 6520 6f6e 2074 6865 2053 4c55  gfile on the SLU
-00011dc0: 524d 2073 6572 7665 722e 0a20 2020 2020  RM server..     
-00011dd0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00011de0: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
-00011df0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00011e00: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00011e10: 3a20 6469 7265 6374 6f72 792c 2066 756c  : directory, ful
-00011e20: 6c20 7061 7468 206f 6620 7468 6520 6c6f  l path of the lo
-00011e30: 6766 696c 652c 2061 6e64 2054 7261 6e73  gfile, and Trans
-00011e40: 6665 7252 6573 756c 740a 2020 2020 2020  ferResult.      
-00011e50: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00011e60: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
-00011e70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00011e80: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
-00011e90: 4746 494c 450a 2020 2020 2020 2020 6c6f  GFILE.        lo
-00011ea0: 6766 696c 6520 3d20 6c6f 6766 696c 652e  gfile = logfile.
-00011eb0: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
-00011ec0: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
-00011ed0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-00011ee0: 2e69 6e66 6f28 6622 436f 7079 696e 6720  .info(f"Copying 
-00011ef0: 6c6f 6766 696c 6520 7b6c 6f67 6669 6c65  logfile {logfile
-00011f00: 7d20 6672 6f6d 2053 6c75 726d 5c0a 2020  } from Slurm\.  
-00011f10: 2020 2020 2020 2020 2020 746f 207b 6c6f            to {lo
-00011f20: 6361 6c5f 746d 705f 7374 6f72 6167 657d  cal_tmp_storage}
-00011f30: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
-00011f40: 7420 3d20 7365 6c66 2e67 6574 280a 2020  t = self.get(.  
-00011f50: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-00011f60: 3d6c 6f67 6669 6c65 2c0a 2020 2020 2020  =logfile,.      
-00011f70: 2020 2020 2020 6c6f 6361 6c3d 6c6f 6361        local=loca
-00011f80: 6c5f 746d 705f 7374 6f72 6167 6529 0a20  l_tmp_storage). 
-00011f90: 2020 2020 2020 2065 7870 6f72 745f 6669         export_fi
-00011fa0: 6c65 203d 206c 6f63 616c 5f74 6d70 5f73  le = local_tmp_s
-00011fb0: 746f 7261 6765 2b6c 6f67 6669 6c65 0a20  torage+logfile. 
-00011fc0: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
-00011fd0: 6361 6c5f 746d 705f 7374 6f72 6167 652c  cal_tmp_storage,
-00011fe0: 2065 7870 6f72 745f 6669 6c65 2c20 7265   export_file, re
-00011ff0: 7375 6c74 0a0a 2020 2020 6465 6620 6765  sult..    def ge
-00012000: 745f 756e 7a69 705f 636f 6d6d 616e 6428  t_unzip_command(
-00012010: 7365 6c66 2c20 7a69 7066 696c 653a 2073  self, zipfile: s
-00012020: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-00012030: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00012040: 6c74 6572 5f66 696c 6574 7970 6573 3a20  lter_filetypes: 
-00012050: 7374 7220 3d20 222a 2e7a 6172 7220 2a2e  str = "*.zarr *.
-00012060: 7469 6666 202a 2e74 6966 220a 2020 2020  tiff *.tif".    
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2020 2020 2020 2920 2d3e 2073 7472 3a0a        ) -> str:.
-00012090: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000120a0: 2020 2020 4765 6e65 7261 7465 2061 2063      Generate a c
-000120b0: 6f6d 6d61 6e64 2073 7472 696e 6720 666f  ommand string fo
-000120c0: 7220 756e 7a69 7070 696e 6720 6120 6461  r unzipping a da
-000120d0: 7461 2061 7263 6869 7665 2061 6e64 2063  ta archive and c
-000120e0: 7265 6174 696e 670a 2020 2020 2020 2020  reating.        
-000120f0: 7265 7175 6972 6564 2064 6972 6563 746f  required directo
-00012100: 7269 6573 2066 6f72 2053 6c75 726d 206a  ries for Slurm j
-00012110: 6f62 732e 0a0a 2020 2020 2020 2020 4172  obs...        Ar
-00012120: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00012130: 7a69 7066 696c 6520 2873 7472 293a 2054  zipfile (str): T
-00012140: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
-00012150: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
-00012160: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
-00012170: 2020 2020 2020 2020 2020 2020 5769 7468              With
-00012180: 6f75 7420 6578 7465 6e73 696f 6e2e 0a20  out extension.. 
-00012190: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-000121a0: 725f 6669 6c65 7479 7065 7320 2873 7472  r_filetypes (str
-000121b0: 2c20 6f70 7469 6f6e 616c 293a 2041 2073  , optional): A s
-000121c0: 7061 6365 2d73 6570 6172 6174 6564 2073  pace-separated s
-000121d0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-000121e0: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
-000121f0: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
-00012200: 696f 6e73 2074 6f20 6578 7472 6163 7420  ions to extract 
-00012210: 6672 6f6d 2074 6865 207a 6970 2066 696c  from the zip fil
-00012220: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-00012230: 2020 2045 2e67 2e20 6465 6661 756c 7473     E.g. defaults
-00012240: 2074 6f20 222a 2e7a 6172 7220 2a2e 7469   to "*.zarr *.ti
-00012250: 6666 202a 2e74 6966 222e 0a20 2020 2020  ff *.tif"..     
-00012260: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
-00012270: 6e67 2074 6869 7320 6172 6775 6d65 6e74  ng this argument
-00012280: 2074 6f20 604e 6f6e 6560 2077 696c 6c20   to `None` will 
-00012290: 6f6d 6974 2074 6865 2066 696c 650a 2020  omit the file.  
-000122a0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-000122b0: 6c74 6572 2061 6e64 2065 7874 7261 6374  lter and extract
-000122c0: 2061 6c6c 2066 696c 6573 2e0a 0a20 2020   all files...   
-000122d0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-000122e0: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
-000122f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00012300: 6865 2063 6f6d 6d61 6e64 2074 6f20 6578  he command to ex
-00012310: 7472 6163 7420 7468 6520 7370 6563 6966  tract the specif
-00012320: 6965 640a 2020 2020 2020 2020 2020 2020  ied.            
-00012330: 2020 2020 6669 6c65 7479 7065 7320 6672      filetypes fr
-00012340: 6f6d 2074 6865 207a 6970 2066 696c 652e  om the zip file.
-00012350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012360: 2020 2020 2075 6e7a 6970 5f63 6d64 203d       unzip_cmd =
-00012370: 2066 226d 6b64 6972 207b 7365 6c66 2e73   f"mkdir {self.s
-00012380: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
-00012390: 7b7a 6970 6669 6c65 7d20 5c0a 2020 2020  {zipfile} \.    
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123b0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
-000123c0: 5f70 6174 687d 2f7b 7a69 7066 696c 657d  _path}/{zipfile}
-000123d0: 2f64 6174 6120 5c0a 2020 2020 2020 2020  /data \.        
-000123e0: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
-000123f0: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-00012400: 687d 2f7b 7a69 7066 696c 657d 2f64 6174  h}/{zipfile}/dat
-00012410: 612f 696e 205c 0a20 2020 2020 2020 2020  a/in \.         
-00012420: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00012430: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-00012440: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
-00012450: 2f6f 7574 205c 0a20 2020 2020 2020 2020  /out \.         
-00012460: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00012470: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-00012480: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
-00012490: 2f67 743b 205c 0a20 2020 2020 2020 2020  /gt; \.         
-000124a0: 2020 2020 2020 2020 2020 2037 7a20 7820             7z x 
-000124b0: 2d79 202d 6f7b 7365 6c66 2e73 6c75 726d  -y -o{self.slurm
-000124c0: 5f64 6174 615f 7061 7468 7d2f 7b7a 6970  _data_path}/{zip
-000124d0: 6669 6c65 7d2f 6461 7461 2f69 6e20 5c0a  file}/data/in \.
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 2020 7b73 656c 662e 736c 7572 6d5f      {self.slurm_
-00012500: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
-00012510: 696c 657d 2e7a 6970 207b 6669 6c74 6572  ile}.zip {filter
-00012520: 5f66 696c 6574 7970 6573 7d22 0a0a 2020  _filetypes}"..  
-00012530: 2020 2020 2020 7265 7475 726e 2075 6e7a        return unz
-00012540: 6970 5f63 6d64 0a0a 2020 2020 6465 6620  ip_cmd..    def 
-00012550: 6765 745f 696d 6167 655f 7665 7273 696f  get_image_versio
-00012560: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
-00012570: 7328 7365 6c66 2c20 6d6f 6465 6c3a 2073  s(self, model: s
-00012580: 7472 0a20 2020 2020 2020 2020 2020 2020  tr.             
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-000125b0: 3e20 5475 706c 655b 4c69 7374 5b73 7472  > Tuple[List[str
-000125c0: 5d2c 204c 6973 745b 7374 725d 5d3a 0a20  ], List[str]]:. 
-000125d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000125e0: 2020 2052 6574 7269 6576 6520 7468 6520     Retrieve the 
-000125f0: 6176 6169 6c61 626c 6520 696d 6167 6520  available image 
-00012600: 7665 7273 696f 6e73 2061 6e64 2069 6e70  versions and inp
-00012610: 7574 2064 6174 6120 6669 6c65 7320 666f  ut data files fo
-00012620: 7220 610a 2020 2020 2020 2020 6769 7665  r a.        give
-00012630: 6e20 6d6f 6465 6c2e 0a0a 2020 2020 2020  n model...      
-00012640: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00012650: 2020 2020 6d6f 6465 6c20 2873 7472 293a      model (str):
-00012660: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00012670: 206d 6f64 656c 2074 6f20 7175 6572 7920   model to query 
-00012680: 666f 722e 0a0a 2020 2020 2020 2020 5265  for...        Re
-00012690: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000126a0: 2020 2054 7570 6c65 5b4c 6973 745b 7374     Tuple[List[st
-000126b0: 725d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  r], List[str]]:.
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-000126e0: 6e67 2074 776f 206c 6973 7473 3a0a 2020  ng two lists:.  
-000126f0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00012700: 5468 6520 6669 7273 7420 6c69 7374 2069  The first list i
-00012710: 6e63 6c75 6465 7320 7468 6520 6176 6169  ncludes the avai
-00012720: 6c61 626c 6520 696d 6167 6520 7665 7273  lable image vers
-00012730: 696f 6e73 2c20 0a20 2020 2020 2020 2020  ions, .         
-00012740: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00012750: 6420 696e 2064 6573 6365 6e64 696e 6720  d in descending 
-00012760: 6f72 6465 722e 0a20 2020 2020 2020 2020  order..         
-00012770: 2020 2020 2020 202d 2054 6865 2073 6563         - The sec
-00012780: 6f6e 6420 6c69 7374 2069 6e63 6c75 6465  ond list include
-00012790: 7320 7468 6520 6176 6169 6c61 626c 6520  s the available 
-000127a0: 6461 7461 2066 696c 6573 2e0a 0a20 2020  data files...   
-000127b0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-000127c0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-000127d0: 726f 723a 2049 6620 7468 6520 7072 6f76  ror: If the prov
-000127e0: 6964 6564 206d 6f64 656c 2069 7320 6e6f  ided model is no
-000127f0: 7420 666f 756e 6420 696e 2074 6865 0a20  t found in the. 
-00012800: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00012810: 6c75 726d 436c 6965 6e74 2773 206b 6e6f  lurmClient's kno
-00012820: 776e 206d 6f64 656c 2070 6174 6873 2e0a  wn model paths..
-00012830: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012840: 2020 2020 696d 6167 655f 7061 7468 203d      image_path =
-00012850: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-00012860: 6c5f 7061 7468 732e 6765 7428 6d6f 6465  l_paths.get(mode
-00012870: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
-00012880: 7420 696d 6167 655f 7061 7468 3a0a 2020  t image_path:.  
-00012890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000128a0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-000128b0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
-000128c0: 2070 6174 6820 6b6e 6f77 6e20 666f 7220   path known for 
-000128d0: 7072 6f76 6964 6564 206d 6f64 656c 207b  provided model {
-000128e0: 6d6f 6465 6c7d 2c20 5c0a 2020 2020 2020  model}, \.      
-000128f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00012900: 207b 7365 6c66 2e73 6c75 726d 5f6d 6f64   {self.slurm_mod
-00012910: 656c 5f70 6174 6873 7d22 290a 2020 2020  el_paths}").    
-00012920: 2020 2020 636d 646c 6973 7420 3d20 5b0a      cmdlist = [.
-00012930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012940: 2e5f 5645 5253 494f 4e5f 434d 442e 666f  ._VERSION_CMD.fo
-00012950: 726d 6174 2873 6c75 726d 5f69 6d61 6765  rmat(slurm_image
-00012960: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
-00012970: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
-00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 2020 696d 6167 655f 7061 7468 3d69      image_path=i
-000129b0: 6d61 6765 5f70 6174 6829 2c0a 2020 2020  mage_path),.    
-000129c0: 2020 2020 2020 2020 7365 6c66 2e5f 4441          self._DA
-000129d0: 5441 5f43 4d44 2e66 6f72 6d61 7428 736c  TA_CMD.format(sl
-000129e0: 7572 6d5f 6461 7461 5f70 6174 683d 7365  urm_data_path=se
-000129f0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
-00012a00: 7468 295d 0a20 2020 2020 2020 2023 2073  th)].        # s
-00012a10: 706c 6974 2072 6573 706f 6e73 6573 2070  plit responses p
-00012a20: 6572 2063 6f6d 6d61 6e64 0a20 2020 2020  er command.     
-00012a30: 2020 2072 6573 706f 6e73 655f 6c69 7374     response_list
-00012a40: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00012a50: 616e 6473 5f73 706c 6974 5f6f 7574 2863  ands_split_out(c
-00012a60: 6d64 6c69 7374 290a 2020 2020 2020 2020  mdlist).        
-00012a70: 2320 7370 6c69 7420 6c69 6e65 7320 6675  # split lines fu
-00012a80: 7274 6865 7220 696e 746f 2073 7562 6c69  rther into subli
-00012a90: 7374 730a 2020 2020 2020 2020 7265 7370  sts.        resp
-00012aa0: 6f6e 7365 5f6c 6973 7420 3d20 5b72 6573  onse_list = [res
-00012ab0: 706f 6e73 652e 7374 7269 7028 292e 7370  ponse.strip().sp
-00012ac0: 6c69 7428 275c 6e27 290a 2020 2020 2020  lit('\n').      
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2066 6f72 2072 6573 706f 6e73 6520     for response 
-00012af0: 696e 2072 6573 706f 6e73 655f 6c69 7374  in response_list
-00012b00: 5d0a 2020 2020 2020 2020 7265 7370 6f6e  ].        respon
-00012b10: 7365 5f6c 6973 745b 305d 203d 2073 6f72  se_list[0] = sor
-00012b20: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
-00012b30: 745b 305d 2c20 7265 7665 7273 653d 5472  t[0], reverse=Tr
-00012b40: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
-00012b50: 726e 2072 6573 706f 6e73 655f 6c69 7374  rn response_list
-00012b60: 5b30 5d2c 2072 6573 706f 6e73 655f 6c69  [0], response_li
-00012b70: 7374 5b31 5d0a 0a20 2020 2064 6566 2067  st[1]..    def g
-00012b80: 6574 5f61 6c6c 5f69 6d61 6765 5f76 6572  et_all_image_ver
-00012b90: 7369 6f6e 735f 616e 645f 6461 7461 5f66  sions_and_data_f
-00012ba0: 696c 6573 2873 656c 660a 2020 2020 2020  iles(self.      
+0000e1f0: 2020 2020 2020 2020 2020 2020 202a 6172               *ar
+0000e200: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+0000e210: 2020 2020 2020 656c 6966 2063 7974 7970        elif cytyp
+0000e220: 6520 3d3d 2027 5374 7269 6e67 273a 0a20  e == 'String':. 
+0000e230: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e240: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
+0000e250: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
+0000e260: 7473 222c 2022 5374 7269 6e67 222c 0a20  ts", "String",. 
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
+0000e2a0: 7267 7329 0a0a 2020 2020 6465 6620 6578  rgs)..    def ex
+0000e2b0: 7472 6163 745f 7061 7274 735f 6672 6f6d  tract_parts_from
+0000e2c0: 5f75 726c 2873 656c 662c 2069 6e70 7574  _url(self, input
+0000e2d0: 5f75 726c 3a20 7374 7229 202d 3e20 5475  _url: str) -> Tu
+0000e2e0: 706c 655b 4c69 7374 5b73 7472 5d2c 2073  ple[List[str], s
+0000e2f0: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
+0000e300: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
+0000e310: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
+0000e320: 616e 6420 6272 616e 6368 2069 6e66 6f72  and branch infor
+0000e330: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
+0000e340: 696e 7075 7420 5552 4c2e 0a0a 2020 2020  input URL...    
+0000e350: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000e360: 2020 2020 2020 696e 7075 745f 7572 6c20        input_url 
+0000e370: 2873 7472 293a 2054 6865 2069 6e70 7574  (str): The input
+0000e380: 2047 6974 4875 6220 5552 4c2e 0a0a 2020   GitHub URL...  
+0000e390: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0000e3a0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+0000e3b0: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
+0000e3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e3d0: 2020 5468 6520 6c69 7374 206f 6620 7572    The list of ur
+0000e3e0: 6c20 7061 7274 7320 616e 6420 7468 6520  l parts and the 
+0000e3f0: 6272 616e 6368 2f76 6572 7369 6f6e 2e0a  branch/version..
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 4966 206e 6f20 6272 616e 6368 2069 7320  If no branch is 
+0000e420: 666f 756e 642c 2069 7420 7769 6c6c 2072  found, it will r
+0000e430: 6574 7572 6e20 226d 6173 7465 7222 0a0a  eturn "master"..
+0000e440: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+0000e450: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+0000e460: 6545 7272 6f72 3a20 4966 2074 6865 2069  eError: If the i
+0000e470: 6e70 7574 2055 524c 2069 7320 6e6f 7420  nput URL is not 
+0000e480: 6120 7661 6c69 6420 4769 7448 7562 2055  a valid GitHub U
+0000e490: 524c 2e0a 2020 2020 2020 2020 2222 220a  RL..        """.
+0000e4a0: 2020 2020 2020 2020 7572 6c5f 7061 7274          url_part
+0000e4b0: 7320 3d20 696e 7075 745f 7572 6c2e 7370  s = input_url.sp
+0000e4c0: 6c69 7428 222f 2229 0a20 2020 2020 2020  lit("/").       
+0000e4d0: 2069 6620 6c65 6e28 7572 6c5f 7061 7274   if len(url_part
+0000e4e0: 7329 203c 2035 206f 7220 7572 6c5f 7061  s) < 5 or url_pa
+0000e4f0: 7274 735b 325d 2021 3d20 2267 6974 6875  rts[2] != "githu
+0000e500: 622e 636f 6d22 3a0a 2020 2020 2020 2020  b.com":.        
+0000e510: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000e520: 7272 6f72 2822 496e 7661 6c69 6420 4769  rror("Invalid Gi
+0000e530: 7448 7562 2055 524c 2229 0a0a 2020 2020  tHub URL")..    
+0000e540: 2020 2020 6966 2022 7472 6565 2220 696e      if "tree" in
+0000e550: 2075 726c 5f70 6172 7473 3a0a 2020 2020   url_parts:.    
+0000e560: 2020 2020 2020 2020 2320 4361 7365 3a20          # Case: 
+0000e570: 5552 4c20 636f 6e74 6169 6e73 2061 2062  URL contains a b
+0000e580: 7261 6e63 680a 2020 2020 2020 2020 2020  ranch.          
+0000e590: 2020 6272 616e 6368 5f69 6e64 6578 203d    branch_index =
+0000e5a0: 2075 726c 5f70 6172 7473 2e69 6e64 6578   url_parts.index
+0000e5b0: 2822 7472 6565 2229 202b 2031 0a20 2020  ("tree") + 1.   
+0000e5c0: 2020 2020 2020 2020 2062 7261 6e63 6820           branch 
+0000e5d0: 3d20 7572 6c5f 7061 7274 735b 6272 616e  = url_parts[bran
+0000e5e0: 6368 5f69 6e64 6578 5d0a 2020 2020 2020  ch_index].      
+0000e5f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000e600: 2020 2020 2320 4361 7365 3a20 5552 4c20      # Case: URL 
+0000e610: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
+0000e620: 2061 2062 7261 6e63 680a 2020 2020 2020   a branch.      
+0000e630: 2020 2020 2020 6272 616e 6368 203d 2022        branch = "
+0000e640: 6d61 7374 6572 220a 0a20 2020 2020 2020  master"..       
+0000e650: 2072 6574 7572 6e20 7572 6c5f 7061 7274   return url_part
+0000e660: 732c 2062 7261 6e63 680a 0a20 2020 2064  s, branch..    d
+0000e670: 6566 2063 6f6e 7665 7274 5f75 726c 2873  ef convert_url(s
+0000e680: 656c 662c 2069 6e70 7574 5f75 726c 3a20  elf, input_url: 
+0000e690: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
+0000e6a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000e6b0: 2043 6f6e 7665 7274 2074 6865 2069 6e70   Convert the inp
+0000e6c0: 7574 2047 6974 4875 6220 5552 4c20 746f  ut GitHub URL to
+0000e6d0: 2061 6e20 6f75 7470 7574 2055 524c 2074   an output URL t
+0000e6e0: 6861 7420 7265 7472 6965 7665 730a 2020  hat retrieves.  
+0000e6f0: 2020 2020 2020 7468 6520 2764 6573 6372        the 'descr
+0000e700: 6970 746f 722e 6a73 6f6e 2720 6669 6c65  iptor.json' file
+0000e710: 2069 6e20 7261 7720 666f 726d 6174 2e0a   in raw format..
+0000e720: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000e730: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000e740: 5f75 726c 2028 7374 7229 3a20 5468 6520  _url (str): The 
+0000e750: 696e 7075 7420 4769 7448 7562 2055 524c  input GitHub URL
+0000e760: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000e770: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000e780: 7374 723a 2054 6865 206f 7574 7075 7420  str: The output 
+0000e790: 5552 4c20 746f 2074 6865 2027 6465 7363  URL to the 'desc
+0000e7a0: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
+0000e7b0: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
+0000e7c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000e7d0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
+0000e7e0: 6865 2069 6e70 7574 2055 524c 2069 7320  he input URL is 
+0000e7f0: 6e6f 7420 6120 7661 6c69 6420 4769 7448  not a valid GitH
+0000e800: 7562 2055 524c 2e0a 2020 2020 2020 2020  ub URL..        
+0000e810: 2222 220a 2020 2020 2020 2020 7572 6c5f  """.        url_
+0000e820: 7061 7274 732c 2062 7261 6e63 6820 3d20  parts, branch = 
+0000e830: 7365 6c66 2e65 7874 7261 6374 5f70 6172  self.extract_par
+0000e840: 7473 5f66 726f 6d5f 7572 6c28 696e 7075  ts_from_url(inpu
+0000e850: 745f 7572 6c29 0a0a 2020 2020 2020 2020  t_url)..        
+0000e860: 2320 436f 6e73 7472 7563 7420 7468 6520  # Construct the 
+0000e870: 6f75 7470 7574 2055 524c 2062 7920 636f  output URL by co
+0000e880: 6d62 696e 696e 6720 7468 6520 6578 7472  mbining the extr
+0000e890: 6163 7465 6420 696e 666f 726d 6174 696f  acted informatio
+0000e8a0: 6e0a 2020 2020 2020 2020 2320 7769 7468  n.        # with
+0000e8b0: 2074 6865 2064 6573 6972 6564 2066 696c   the desired fil
+0000e8c0: 6520 7061 7468 0a20 2020 2020 2020 206f  e path.        o
+0000e8d0: 7574 7075 745f 7572 6c20 3d20 6622 6874  utput_url = f"ht
+0000e8e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e8f0: 2f7b 7572 6c5f 7061 7274 735b 335d 7d2f  /{url_parts[3]}/
+0000e900: 7b75 726c 5f70 6172 7473 5b34 5d7d 2f72  {url_parts[4]}/r
+0000e910: 6177 2f7b 6272 616e 6368 7d2f 6465 7363  aw/{branch}/desc
+0000e920: 7269 7074 6f72 2e6a 736f 6e22 0a0a 2020  riptor.json"..  
+0000e930: 2020 2020 2020 7265 7475 726e 206f 7574        return out
+0000e940: 7075 745f 7572 6c0a 0a20 2020 2064 6566  put_url..    def
+0000e950: 2070 756c 6c5f 6465 7363 7269 7074 6f72   pull_descriptor
+0000e960: 5f66 726f 6d5f 6769 7468 7562 2873 656c  _from_github(sel
+0000e970: 662c 2077 6f72 6b66 6c6f 773a 2073 7472  f, workflow: str
+0000e980: 2920 2d3e 2044 6963 743a 0a20 2020 2020  ) -> Dict:.     
+0000e990: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+0000e9a0: 756c 6c20 7468 6520 776f 726b 666c 6f77  ull the workflow
+0000e9b0: 2064 6573 6372 6970 746f 7220 6672 6f6d   descriptor from
+0000e9c0: 2047 6974 4875 622e 0a0a 2020 2020 2020   GitHub...      
+0000e9d0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000e9e0: 2020 2020 776f 726b 666c 6f77 2028 7374      workflow (st
+0000e9f0: 7229 3a20 5468 6520 776f 726b 666c 6f77  r): The workflow
+0000ea00: 2066 6f72 2077 6869 6368 2074 6f20 7075   for which to pu
+0000ea10: 6c6c 2074 6865 2064 6573 6372 6970 746f  ll the descripto
+0000ea20: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
+0000ea30: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000ea40: 2044 6963 743a 2054 6865 204a 534f 4e20   Dict: The JSON 
+0000ea50: 6465 7363 7269 7074 6f72 2e0a 0a20 2020  descriptor...   
+0000ea60: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0000ea70: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+0000ea80: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
+0000ea90: 206f 6363 7572 7320 7768 696c 6520 7075   occurs while pu
+0000eaa0: 6c6c 696e 6720 7468 6520 6465 7363 7269  lling the descri
+0000eab0: 7074 6f72 2066 696c 652e 0a20 2020 2020  ptor file..     
+0000eac0: 2020 2022 2222 0a20 2020 2020 2020 2067     """.        g
+0000ead0: 6974 5f72 6570 6f20 3d20 7365 6c66 2e73  it_repo = self.s
+0000eae0: 6c75 726d 5f6d 6f64 656c 5f72 6570 6f73  lurm_model_repos
+0000eaf0: 5b77 6f72 6b66 6c6f 775d 0a20 2020 2020  [workflow].     
+0000eb00: 2020 2023 2063 6f6e 7665 7274 2067 6974     # convert git
+0000eb10: 2072 6570 6f20 746f 206a 736f 6e20 6669   repo to json fi
+0000eb20: 6c65 0a20 2020 2020 2020 2072 6177 5f75  le.        raw_u
+0000eb30: 726c 203d 2073 656c 662e 636f 6e76 6572  rl = self.conver
+0000eb40: 745f 7572 6c28 6769 745f 7265 706f 290a  t_url(git_repo).
+0000eb50: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000eb60: 6562 7567 2866 2250 756c 6c20 776f 726b  ebug(f"Pull work
+0000eb70: 666c 6f77 3a20 7b77 6f72 6b66 6c6f 777d  flow: {workflow}
+0000eb80: 3a20 7b67 6974 5f72 6570 6f7d 203e 3e20  : {git_repo} >> 
+0000eb90: 7b72 6177 5f75 726c 7d22 290a 2020 2020  {raw_url}").    
+0000eba0: 2020 2020 2320 7075 6c6c 2077 6f72 6b66      # pull workf
+0000ebb0: 6c6f 7720 7061 7261 6d73 0a20 2020 2020  low params.     
+0000ebc0: 2020 2067 6974 6875 625f 7365 7373 696f     github_sessio
+0000ebd0: 6e20 3d20 7365 6c66 2e67 6574 5f6f 725f  n = self.get_or_
+0000ebe0: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
+0000ebf0: 7373 696f 6e28 290a 2020 2020 2020 2020  ssion().        
+0000ec00: 6768 6669 6c65 203d 2067 6974 6875 625f  ghfile = github_
+0000ec10: 7365 7373 696f 6e2e 6765 7428 7261 775f  session.get(raw_
+0000ec20: 7572 6c29 0a20 2020 2020 2020 2069 6620  url).        if 
+0000ec30: 6768 6669 6c65 2e6f 6b3a 0a20 2020 2020  ghfile.ok:.     
+0000ec40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000ec50: 6275 6728 6622 4361 6368 6564 3f20 7b67  bug(f"Cached? {g
+0000ec60: 6866 696c 652e 6672 6f6d 5f63 6163 6865  hfile.from_cache
+0000ec70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000ec80: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
+0000ec90: 3d20 6768 6669 6c65 2e6a 736f 6e28 290a  = ghfile.json().
+0000eca0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ecb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000ecc0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+0000ecd0: 2020 2020 2020 2020 2020 2020 6627 4572              f'Er
+0000ece0: 726f 7220 7768 696c 6520 7075 6c6c 696e  ror while pullin
+0000ecf0: 6720 6465 7363 7269 7074 6f72 2066 696c  g descriptor fil
+0000ed00: 6520 666f 7220 776f 726b 666c 6f77 207b  e for workflow {
+0000ed10: 776f 726b 666c 6f77 7d2c 5c0a 2020 2020  workflow},\.    
+0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed30: 6672 6f6d 207b 7261 775f 7572 6c7d 3a20  from {raw_url}: 
+0000ed40: 7b67 6866 696c 652e 5f5f 6469 6374 5f5f  {ghfile.__dict__
+0000ed50: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
+0000ed60: 726e 206a 736f 6e5f 6465 7363 7269 7074  rn json_descript
+0000ed70: 6f72 0a0a 2020 2020 6465 6620 6765 745f  or..    def get_
+0000ed80: 6f72 5f63 7265 6174 655f 6769 7468 7562  or_create_github
+0000ed90: 5f73 6573 7369 6f6e 2873 656c 6629 3a0a  _session(self):.
+0000eda0: 2020 2020 2020 2020 2320 4e6f 7465 2c20          # Note, 
+0000edb0: 7573 696e 6720 7265 7175 6573 7473 5f63  using requests_c
+0000edc0: 6163 6865 2031 2e31 2e31 2c20 636f 6e64  ache 1.1.1, cond
+0000edd0: 6974 696f 6e61 6c20 7175 6572 6965 7320  itional queries 
+0000ede0: 6172 6520 6465 6661 756c 743a 0a20 2020  are default:.   
+0000edf0: 2020 2020 2023 2054 6865 2063 6163 6865       # The cache
+0000ee00: 6420 7265 7370 6f6e 7365 2077 696c 6c20  d response will 
+0000ee10: 7374 696c 6c20 6265 2075 7365 6420 756e  still be used un
+0000ee20: 7469 6c20 7468 6520 7265 6d6f 7465 2063  til the remote c
+0000ee30: 6f6e 7465 6e74 2061 6374 7561 6c6c 7920  ontent actually 
+0000ee40: 6368 616e 6765 730a 2020 2020 2020 2020  changes.        
+0000ee50: 2320 4576 656e 2069 6620 7468 6520 2765  # Even if the 'e
+0000ee60: 7870 6972 655f 6166 7465 7227 2069 7320  xpire_after' is 
+0000ee70: 7472 6967 6765 7265 642e 2054 6869 7320  triggered. This 
+0000ee80: 6973 2062 7569 6c74 2069 6e74 6f20 4769  is built into Gi
+0000ee90: 7448 7562 2c20 7768 6963 6820 7265 7475  tHub, which retu
+0000eea0: 726e 730a 2020 2020 2020 2020 2320 6120  rns.        # a 
+0000eeb0: 4574 6167 2069 6e20 7468 6520 6865 6164  Etag in the head
+0000eec0: 6572 2074 6861 7420 6f6e 6c79 2063 6861  er that only cha
+0000eed0: 6e67 6573 2077 6865 6e20 7468 6520 636f  nges when the co
+0000eee0: 6e74 656e 7420 2865 2e67 2e20 7468 6520  ntent (e.g. the 
+0000eef0: 6465 7363 7269 7074 6f72 2920 6368 616e  descriptor) chan
+0000ef00: 6765 732e 0a20 2020 2020 2020 2023 2049  ges..        # I
+0000ef10: 6620 796f 7520 7072 6f76 6964 6520 7468  f you provide th
+0000ef20: 6973 2045 7461 6720 7768 656e 2071 7565  is Etag when que
+0000ef30: 7279 696e 672c 2079 6f75 2077 696c 6c20  rying, you will 
+0000ef40: 6765 7420 6120 3330 3420 2827 6e6f 2063  get a 304 ('no c
+0000ef50: 6861 6e67 6527 2920 616e 6420 6974 2077  hange') and it w
+0000ef60: 696c 6c0a 2020 2020 2020 2020 2320 4e4f  ill.        # NO
+0000ef70: 5420 636f 756e 7420 746f 7761 7264 7320  T count towards 
+0000ef80: 796f 7572 2047 6974 6875 6220 6c69 6d69  your Github limi
+0000ef90: 7473 2e20 416e 6420 7265 7175 6573 7473  ts. And requests
+0000efa0: 5f63 6163 6865 2064 6f65 7320 7468 6174  _cache does that
+0000efb0: 2066 6f72 2075 7320 6e6f 772e 0a20 2020   for us now..   
+0000efc0: 2020 2020 2023 204e 6f74 2061 7661 696c       # Not avail
+0000efd0: 6162 6c65 2069 6e20 5079 7468 6f6e 332e  able in Python3.
+0000efe0: 3620 7468 6f75 6768 2e0a 2020 2020 2020  6 though..      
+0000eff0: 2020 7320 3d20 7265 7175 6573 7473 5f63    s = requests_c
+0000f000: 6163 6865 2e43 6163 6865 6453 6573 7369  ache.CachedSessi
+0000f010: 6f6e 2827 6769 7468 7562 5f63 6163 6865  on('github_cache
+0000f020: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f040: 2020 2020 2020 2020 2020 2020 6261 636b              back
+0000f050: 656e 643d 7365 6c66 2e63 6163 6865 2c0a  end=self.cache,.
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f080: 2020 2020 2020 2020 2065 7870 6972 655f           expire_
+0000f090: 6166 7465 723d 312c 0a20 2020 2020 2020  after=1,.       
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0c0: 2020 6361 6368 655f 636f 6e74 726f 6c3d    cache_control=
+0000f0d0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000f100: 2020 2020 2020 2020 2320 4d69 6768 7420          # Might 
+0000f110: 6861 7665 2062 6967 6765 7220 6973 7375  have bigger issu
+0000f120: 6573 2c20 7468 6973 2069 7320 7265 6c61  es, this is rela
+0000f130: 7465 6420 746f 2072 6174 6520 6c69 6d69  ted to rate limi
+0000f140: 7473 206f 6e20 4769 7448 7562 0a20 2020  ts on GitHub.   
+0000f150: 2020 2020 2023 2068 7474 7073 3a2f 2f64       # https://d
+0000f160: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+0000f170: 6e2f 7265 7374 2f75 7369 6e67 2d74 6865  n/rest/using-the
+0000f180: 2d72 6573 742d 6170 692f 7261 7465 2d6c  -rest-api/rate-l
+0000f190: 696d 6974 732d 666f 722d 7468 652d 7265  imits-for-the-re
+0000f1a0: 7374 2d61 7069 0a20 2020 2020 2020 2023  st-api.        #
+0000f1b0: 2049 6620 6974 2073 7461 7973 2061 2070   If it stays a p
+0000f1c0: 726f 626c 656d 2c20 7765 2068 6176 6520  roblem, we have 
+0000f1d0: 746f 2061 6464 2061 6e20 6f70 7469 6f6e  to add an option
+0000f1e0: 2074 6f20 6164 6420 6120 4748 206b 6579   to add a GH key
+0000f1f0: 2074 6f20 7468 6520 636f 6e66 6967 0a20   to the config. 
+0000f200: 2020 2020 2020 2023 2045 2e67 2e20 7365         # E.g. se
+0000f210: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+0000f220: 2e63 6f6d 2f72 6571 7565 7374 732d 6361  .com/requests-ca
+0000f230: 6368 652f 7265 7175 6573 7473 2d63 6163  che/requests-cac
+0000f240: 6865 2f62 6c6f 622f 3533 3133 3465 6630  he/blob/53134ef0
+0000f250: 6539 3964 3731 3366 6564 3632 3531 3564  e99d713fed62515d
+0000f260: 6662 3762 6366 6161 6335 6636 3366 3964  fb7bcfaac5f63f9d
+0000f270: 2f65 7861 6d70 6c65 732f 7079 6769 7468  /examples/pygith
+0000f280: 7562 2e70 790a 2020 2020 2020 2020 2320  ub.py.        # 
+0000f290: 4865 7265 2079 6f75 2063 6f75 6c64 2068  Here you could h
+0000f2a0: 6176 6520 616e 2041 4343 4553 535f 544f  ave an ACCESS_TO
+0000f2b0: 4b45 4e2e 0a20 2020 2020 2020 2023 2041  KEN..        # A
+0000f2c0: 6e20 4143 4345 5353 5f54 4f4b 454e 2063  n ACCESS_TOKEN c
+0000f2d0: 6f75 6c64 2069 6d70 726f 7665 2061 7069  ould improve api
+0000f2e0: 206c 696d 6974 7320 746f 2035 3030 302f   limits to 5000/
+0000f2f0: 6820 2866 726f 6d20 3630 2f68 292e 0a20  h (from 60/h).. 
+0000f300: 2020 2020 2020 2072 6574 7279 5f73 7472         retry_str
+0000f310: 6174 6567 7920 3d20 5265 7472 7928 0a20  ategy = Retry(. 
+0000f320: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+0000f330: 3d35 2c20 2020 2020 2020 2020 2020 2020  =5,             
+0000f340: 2020 2320 4d61 7869 6d75 6d20 6e75 6d62    # Maximum numb
+0000f350: 6572 206f 6620 7265 7472 6965 730a 2020  er of retries.  
+0000f360: 2020 2020 2020 2020 2020 2320 4578 706f            # Expo
+0000f370: 6e65 6e74 6961 6c20 6261 636b 6f66 6620  nential backoff 
+0000f380: 6661 6374 6f72 2028 6465 6c61 7920 6265  factor (delay be
+0000f390: 7477 6565 6e20 7265 7472 6965 7329 0a20  tween retries). 
+0000f3a0: 2020 2020 2020 2020 2020 2062 6163 6b6f             backo
+0000f3b0: 6666 5f66 6163 746f 723d 352c 0a20 2020  ff_factor=5,.   
+0000f3c0: 2020 2020 2020 2020 2023 2052 6574 7279           # Retry
+0000f3d0: 206f 6e20 7468 6573 6520 4854 5450 2073   on these HTTP s
+0000f3e0: 7461 7475 7320 636f 6465 730a 2020 2020  tatus codes.    
+0000f3f0: 2020 2020 2020 2020 7374 6174 7573 5f66          status_f
+0000f400: 6f72 6365 6c69 7374 3d5b 3530 302c 2035  orcelist=[500, 5
+0000f410: 3032 2c20 3530 332c 2035 3034 2c20 3430  02, 503, 504, 40
+0000f420: 332c 2034 3239 5d2c 0a20 2020 2020 2020  3, 429],.       
+0000f430: 2020 2020 2061 6c6c 6f77 6564 5f6d 6574       allowed_met
+0000f440: 686f 6473 3d66 726f 7a65 6e73 6574 285b  hods=frozenset([
+0000f450: 2747 4554 275d 2920 2023 204f 6e6c 7920  'GET'])  # Only 
+0000f460: 7265 7472 7920 666f 7220 4745 5420 7265  retry for GET re
+0000f470: 7175 6573 7473 0a20 2020 2020 2020 2029  quests.        )
+0000f480: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
+0000f490: 2827 6874 7470 733a 2f2f 6769 7468 7562  ('https://github
+0000f4a0: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
+0000f4b0: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
+0000f4c0: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
+0000f4d0: 0a20 2020 2020 2020 2073 2e6d 6f75 6e74  .        s.mount
+0000f4e0: 2827 6874 7470 3a2f 2f67 6974 6875 622e  ('http://github.
+0000f4f0: 636f 6d2f 272c 2048 5454 5041 6461 7074  com/', HTTPAdapt
+0000f500: 6572 286d 6178 5f72 6574 7269 6573 3d72  er(max_retries=r
+0000f510: 6574 7279 5f73 7472 6174 6567 7929 290a  etry_strategy)).
+0000f520: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000f530: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
+0000f540: 726b 666c 6f77 5f63 6f6d 6d61 6e64 2873  rkflow_command(s
+0000f550: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f570: 2020 776f 726b 666c 6f77 3a20 7374 722c    workflow: str,
+0000f580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f590: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+0000f5a0: 726b 666c 6f77 5f76 6572 7369 6f6e 3a20  rkflow_version: 
+0000f5b0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5d0: 2020 696e 7075 745f 6461 7461 3a20 7374    input_data: st
+0000f5e0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f600: 656d 6169 6c3a 204f 7074 696f 6e61 6c5b  email: Optional[
+0000f610: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 2020 2020 2020 2020 2020 7469 6d65 3a20            time: 
+0000f640: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000f650: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 2020 202a 2a6b 7761 7267 7329 202d 3e20     **kwargs) -> 
+0000f680: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
+0000f690: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f6a0: 2020 2020 2020 4765 6e65 7261 7465 2074        Generate t
+0000f6b0: 6865 2053 6c75 726d 2077 6f72 6b66 6c6f  he Slurm workflo
+0000f6c0: 7720 636f 6d6d 616e 6420 616e 6420 656e  w command and en
+0000f6d0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+0000f6e0: 6c65 732e 0a0a 2020 2020 2020 2020 4172  les...        Ar
+0000f6f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000f700: 776f 726b 666c 6f77 2028 7374 7229 3a20  workflow (str): 
+0000f710: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+0000f720: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
+0000f730: 2020 2020 2020 776f 726b 666c 6f77 5f76        workflow_v
+0000f740: 6572 7369 6f6e 2028 7374 7229 3a20 5468  ersion (str): Th
+0000f750: 6520 7665 7273 696f 6e20 6f66 2074 6865  e version of the
+0000f760: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+0000f770: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+0000f780: 6120 2873 7472 293a 2054 6865 206e 616d  a (str): The nam
+0000f790: 6520 6f66 2074 6865 2069 6e70 7574 2064  e of the input d
+0000f7a0: 6174 6120 666f 6c64 6572 2063 6f6e 7461  ata folder conta
+0000f7b0: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
+0000f7c0: 2020 2020 2020 7468 6520 696e 7075 7420        the input 
+0000f7d0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
+0000f7e0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
+0000f7f0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0000f800: 5468 6520 656d 6169 6c20 6164 6472 6573  The email addres
+0000f810: 7320 666f 7220 6a6f 6220 6e6f 7469 6669  s for job notifi
+0000f820: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
+0000f830: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+0000f840: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
+0000f850: 2064 6566 6175 6c74 7320 746f 2077 6861   defaults to wha
+0000f860: 7420 6973 2069 6e20 7468 6520 6a6f 6220  t is in the job 
+0000f870: 7363 7269 7074 2e0a 2020 2020 2020 2020  script..        
+0000f880: 2020 2020 7469 6d65 2028 7374 722c 206f      time (str, o
+0000f890: 7074 696f 6e61 6c29 3a20 5468 6520 7469  ptional): The ti
+0000f8a0: 6d65 206c 696d 6974 2066 6f72 2074 6865  me limit for the
+0000f8b0: 206a 6f62 2069 6e20 7468 6520 0a20 2020   job in the .   
+0000f8c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f8d0: 6d61 7420 4848 3a4d 4d3a 5353 2e20 4465  mat HH:MM:SS. De
+0000f8e0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
+0000f8f0: 7768 6963 6820 6465 6661 756c 7473 2074  which defaults t
+0000f900: 6f20 7768 6174 200a 2020 2020 2020 2020  o what .        
+0000f910: 2020 2020 2020 2020 6973 2069 6e20 7468          is in th
+0000f920: 6520 6a6f 6220 7363 7269 7074 2e0a 2020  e job script..  
+0000f930: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000f940: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000f950: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000f960: 2066 6f72 2074 6865 2077 6f72 6b66 6c6f   for the workflo
+0000f970: 772e 0a0a 2020 2020 2020 2020 5265 7475  w...        Retu
+0000f980: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000f990: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
+0000f9a0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000f9b0: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+0000f9c0: 696e 696e 6720 7468 6520 536c 7572 6d20  ining the Slurm 
+0000f9d0: 776f 726b 666c 6f77 2063 6f6d 6d61 6e64  workflow command
+0000f9e0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000f9f0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
+0000fa00: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
+0000fa10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fa20: 2020 2020 206d 6f64 656c 5f70 6174 6820       model_path 
+0000fa30: 3d20 7365 6c66 2e73 6c75 726d 5f6d 6f64  = self.slurm_mod
+0000fa40: 656c 5f70 6174 6873 5b77 6f72 6b66 6c6f  el_paths[workflo
+0000fa50: 772e 6c6f 7765 7228 295d 0a20 2020 2020  w.lower()].     
+0000fa60: 2020 206a 6f62 5f73 6372 6970 7420 3d20     job_script = 
+0000fa70: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+0000fa80: 5f6a 6f62 735b 776f 726b 666c 6f77 2e6c  _jobs[workflow.l
+0000fa90: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
+0000faa0: 6a6f 625f 7061 7261 6d73 203d 2073 656c  job_params = sel
+0000fab0: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
+0000fac0: 6273 5f70 6172 616d 735b 776f 726b 666c  bs_params[workfl
+0000fad0: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
+0000fae0: 2020 2020 2320 6772 6162 206f 6e6c 7920      # grab only 
+0000faf0: 7468 6520 696d 6167 6520 6e61 6d65 2c20  the image name, 
+0000fb00: 6e6f 7420 7468 6520 6772 6f75 702f 6372  not the group/cr
+0000fb10: 6561 746f 720a 2020 2020 2020 2020 696d  eator.        im
+0000fb20: 6167 6520 3d20 7365 6c66 2e73 6c75 726d  age = self.slurm
+0000fb30: 5f6d 6f64 656c 5f69 6d61 6765 735b 776f  _model_images[wo
+0000fb40: 726b 666c 6f77 2e6c 6f77 6572 2829 5d2e  rkflow.lower()].
+0000fb50: 7370 6c69 7428 222f 2229 5b31 5d0a 0a20  split("/")[1].. 
+0000fb60: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
+0000fb70: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
+0000fb80: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
+0000fb90: 227b 7365 6c66 2e73 6c75 726d 5f64 6174  "{self.slurm_dat
+0000fba0: 615f 7061 7468 7d2f 7b69 6e70 7574 5f64  a_path}/{input_d
+0000fbb0: 6174 617d 222c 0a20 2020 2020 2020 2020  ata}",.         
+0000fbc0: 2020 2022 494d 4147 455f 5041 5448 223a     "IMAGE_PATH":
+0000fbd0: 2066 227b 7365 6c66 2e73 6c75 726d 5f69   f"{self.slurm_i
+0000fbe0: 6d61 6765 735f 7061 7468 7d2f 7b6d 6f64  mages_path}/{mod
+0000fbf0: 656c 5f70 6174 687d 222c 0a20 2020 2020  el_path}",.     
+0000fc00: 2020 2020 2020 2022 494d 4147 455f 5645         "IMAGE_VE
+0000fc10: 5253 494f 4e22 3a20 6622 7b77 6f72 6b66  RSION": f"{workf
+0000fc20: 6c6f 775f 7665 7273 696f 6e7d 222c 0a20  low_version}",. 
+0000fc30: 2020 2020 2020 2020 2020 2022 5349 4e47             "SING
+0000fc40: 554c 4152 4954 595f 494d 4147 4522 3a20  ULARITY_IMAGE": 
+0000fc50: 6622 7b69 6d61 6765 7d5f 7b77 6f72 6b66  f"{image}_{workf
+0000fc60: 6c6f 775f 7665 7273 696f 6e7d 2e73 6966  low_version}.sif
+0000fc70: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000fc80: 5343 5249 5054 5f50 4154 4822 3a20 6622  SCRIPT_PATH": f"
+0000fc90: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
+0000fca0: 7074 5f70 6174 687d 220a 2020 2020 2020  pt_path}".      
+0000fcb0: 2020 7d0a 2020 2020 2020 2020 776f 726b    }.        work
+0000fcc0: 666c 6f77 5f65 6e76 203d 2073 656c 662e  flow_env = self.
+0000fcd0: 776f 726b 666c 6f77 5f70 6172 616d 735f  workflow_params_
+0000fce0: 746f 5f65 6e76 7661 7273 282a 2a6b 7761  to_envvars(**kwa
+0000fcf0: 7267 7329 0a20 2020 2020 2020 2065 6e76  rgs).        env
+0000fd00: 203d 207b 2a2a 7362 6174 6368 5f65 6e76   = {**sbatch_env
+0000fd10: 2c20 2a2a 776f 726b 666c 6f77 5f65 6e76  , **workflow_env
+0000fd20: 7d0a 0a20 2020 2020 2020 2065 6d61 696c  }..        email
+0000fd30: 5f70 6172 616d 203d 2022 2220 6966 2065  _param = "" if e
+0000fd40: 6d61 696c 2069 7320 4e6f 6e65 2065 6c73  mail is None els
+0000fd50: 6520 6622 202d 2d6d 6169 6c2d 7573 6572  e f" --mail-user
+0000fd60: 3d7b 656d 6169 6c7d 220a 2020 2020 2020  ={email}".      
+0000fd70: 2020 7469 6d65 5f70 6172 616d 203d 2022    time_param = "
+0000fd80: 2220 6966 2074 696d 6520 6973 204e 6f6e  " if time is Non
+0000fd90: 6520 656c 7365 2066 2220 2d2d 7469 6d65  e else f" --time
+0000fda0: 3d7b 7469 6d65 7d22 0a20 2020 2020 2020  ={time}".       
+0000fdb0: 206a 6f62 5f70 6172 616d 732e 6170 7065   job_params.appe
+0000fdc0: 6e64 2874 696d 655f 7061 7261 6d29 0a20  nd(time_param). 
+0000fdd0: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
+0000fde0: 732e 6170 7065 6e64 2865 6d61 696c 5f70  s.append(email_p
+0000fdf0: 6172 616d 290a 2020 2020 2020 2020 6a6f  aram).        jo
+0000fe00: 625f 7061 7261 6d20 3d20 2222 2e6a 6f69  b_param = "".joi
+0000fe10: 6e28 6a6f 625f 7061 7261 6d73 290a 2020  n(job_params).  
+0000fe20: 2020 2020 2020 7362 6174 6368 5f63 6d64        sbatch_cmd
+0000fe30: 203d 2066 2273 6261 7463 687b 6a6f 625f   = f"sbatch{job_
+0000fe40: 7061 7261 6d7d 202d 2d6f 7574 7075 743d  param} --output=
+0000fe50: 6f6d 6572 6f2d 256a 2e6c 6f67 205c 0a20  omero-%j.log \. 
+0000fe60: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+0000fe70: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
+0000fe80: 7468 7d2f 7b6a 6f62 5f73 6372 6970 747d  th}/{job_script}
+0000fe90: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000fea0: 6e20 7362 6174 6368 5f63 6d64 2c20 656e  n sbatch_cmd, en
+0000feb0: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
+0000fec0: 6f6e 7665 7273 696f 6e5f 636f 6d6d 616e  onversion_comman
+0000fed0: 6428 7365 6c66 2c20 6461 7461 5f70 6174  d(self, data_pat
+0000fee0: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff00: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
+0000ff10: 6c65 3a20 7374 722c 0a20 2020 2020 2020  le: str,.       
+0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff30: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
+0000ff40: 6f72 6d61 743a 2073 7472 203d 2027 7a61  ormat: str = 'za
+0000ff50: 7272 272c 0a20 2020 2020 2020 2020 2020  rr',.           
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff70: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
+0000ff80: 743a 2073 7472 203d 2027 7469 6666 2729  t: str = 'tiff')
+0000ff90: 202d 3e20 5475 706c 655b 7374 722c 2044   -> Tuple[str, D
+0000ffa0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+0000ffb0: 220a 2020 2020 2020 2020 4765 6e65 7261  ".        Genera
+0000ffc0: 7465 2053 6c75 726d 2063 6f6e 7665 7273  te Slurm convers
+0000ffd0: 696f 6e20 636f 6d6d 616e 6420 616e 6420  ion command and 
+0000ffe0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+0000fff0: 6162 6c65 7320 666f 7220 6461 7461 2063  ables for data c
+00010000: 6f6e 7665 7273 696f 6e2e 0a0a 2020 2020  onversion...    
+00010010: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00010020: 2020 2020 2020 6461 7461 5f70 6174 6820        data_path 
+00010030: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
+00010040: 6865 2064 6174 6120 666f 6c64 6572 2e0a  he data folder..
+00010050: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00010060: 6967 5f66 696c 6520 2873 7472 293a 2050  ig_file (str): P
+00010070: 6174 6820 746f 2074 6865 2063 6f6e 6669  ath to the confi
+00010080: 6775 7261 7469 6f6e 2066 696c 652e 0a20  guration file.. 
+00010090: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000100a0: 655f 666f 726d 6174 2028 7374 7229 3a20  e_format (str): 
+000100b0: 536f 7572 6365 2064 6174 6120 666f 726d  Source data form
+000100c0: 6174 2028 6465 6661 756c 7420 6973 2027  at (default is '
+000100d0: 7a61 7272 2729 2e0a 2020 2020 2020 2020  zarr')..        
+000100e0: 2020 2020 7461 7267 6574 5f66 6f72 6d61      target_forma
+000100f0: 7420 2873 7472 293a 2054 6172 6765 7420  t (str): Target 
+00010100: 6461 7461 2066 6f72 6d61 7420 2864 6566  data format (def
+00010110: 6175 6c74 2069 7320 2774 6966 6627 292e  ault is 'tiff').
+00010120: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00010130: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00010140: 7570 6c65 5b73 7472 2c20 4469 6374 5d3a  uple[str, Dict]:
+00010150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010160: 2041 2074 7570 6c65 2063 6f6e 7461 696e   A tuple contain
+00010170: 696e 6720 7468 6520 536c 7572 6d20 636f  ing the Slurm co
+00010180: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
+00010190: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+000101a0: 2020 2020 2074 6865 2065 6e76 6972 6f6e       the environ
+000101b0: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
+000101c0: 0a20 2020 2020 2020 2057 6172 6e69 6e67  .        Warning
+000101d0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+000101e0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
+000101f0: 656e 7461 7469 6f6e 206f 6e6c 7920 7375  entation only su
+00010200: 7070 6f72 7473 2063 6f6e 7665 7273 696f  pports conversio
+00010210: 6e20 6672 6f6d 2027 7a61 7272 2720 746f  n from 'zarr' to
+00010220: 2027 7469 6666 272e 0a20 2020 2020 2020   'tiff'..       
+00010230: 2020 2020 2049 6620 7573 696e 6720 6f74       If using ot
+00010240: 6865 7220 736f 7572 6365 206f 7220 7461  her source or ta
+00010250: 7267 6574 2066 6f72 6d61 7473 2c20 7573  rget formats, us
+00010260: 6572 7320 6d75 7374 2069 6d70 6c65 6d65  ers must impleme
+00010270: 6e74 2061 6e64 2063 6f6e 6669 6775 7265  nt and configure
+00010280: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00010290: 6974 696f 6e61 6c20 636f 6e76 6572 7465  itional converte
+000102a0: 7273 2074 6865 6d73 656c 7665 732e 0a20  rs themselves.. 
+000102b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000102c0: 2020 2069 6620 736f 7572 6365 5f66 6f72     if source_for
+000102d0: 6d61 7420 213d 2022 7a61 7272 2220 6f72  mat != "zarr" or
+000102e0: 2074 6172 6765 745f 666f 726d 6174 2021   target_format !
+000102f0: 3d20 2274 6966 6622 3a0a 2020 2020 2020  = "tiff":.      
+00010300: 2020 2020 2020 2320 5761 726e 2061 626f        # Warn abo
+00010310: 7574 2075 6e73 7570 706f 7274 6564 2063  ut unsupported c
+00010320: 6f6e 7665 7273 696f 6e3b 2061 6464 6974  onversion; addit
+00010330: 696f 6e61 6c20 636f 6e76 6572 7465 7273  ional converters
+00010340: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00010350: 2020 2020 2320 6164 6465 6420 6f75 7473      # added outs
+00010360: 6964 6520 6f75 7220 6b6e 6f77 6c65 6467  ide our knowledg
+00010370: 652e 0a20 2020 2020 2020 2020 2020 2023  e..            #
+00010380: 2043 6865 636b 696e 6720 536c 7572 6d27   Checking Slurm'
+00010390: 7320 6073 6c75 726d 5f63 6f6e 7665 7274  s `slurm_convert
+000103a0: 6572 735f 7061 7468 6020 6973 2073 6b69  ers_path` is ski
+000103b0: 7070 6564 2066 6f72 0a20 2020 2020 2020  pped for.       
+000103c0: 2020 2020 2023 2070 6572 666f 726d 616e       # performan
+000103d0: 6365 2072 6561 736f 6e73 2e0a 2020 2020  ce reasons..    
+000103e0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+000103f0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+00010400: 2020 2020 2020 2020 6622 436f 6e76 6572          f"Conver
+00010410: 7369 6f6e 2066 726f 6d20 7b73 6f75 7263  sion from {sourc
+00010420: 655f 666f 726d 6174 7d20 746f 207b 7461  e_format} to {ta
+00010430: 7267 6574 5f66 6f72 6d61 747d 2069 7320  rget_format} is 
+00010440: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00010450: 2064 6566 6175 6c74 2122 290a 0a20 2020   default!")..   
+00010460: 2020 2020 2063 686f 7365 6e5f 636f 6e76       chosen_conv
+00010470: 6572 7465 7220 3d20 6622 636f 6e76 6572  erter = f"conver
+00010480: 745f 7b73 6f75 7263 655f 666f 726d 6174  t_{source_format
+00010490: 7d5f 746f 5f7b 7461 7267 6574 5f66 6f72  }_to_{target_for
+000104a0: 6d61 747d 2e73 6966 220a 2020 2020 2020  mat}.sif".      
+000104b0: 2020 7362 6174 6368 5f65 6e76 203d 207b    sbatch_env = {
+000104c0: 0a20 2020 2020 2020 2020 2020 2022 4441  .            "DA
+000104d0: 5441 5f50 4154 4822 3a20 6622 7b64 6174  TA_PATH": f"{dat
+000104e0: 615f 7061 7468 7d22 2c0a 2020 2020 2020  a_path}",.      
+000104f0: 2020 2020 2020 2243 4f4e 5645 5253 494f        "CONVERSIO
+00010500: 4e5f 5041 5448 223a 2066 227b 7365 6c66  N_PATH": f"{self
+00010510: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
+00010520: 735f 7061 7468 7d22 2c0a 2020 2020 2020  s_path}",.      
+00010530: 2020 2020 2020 2243 4f4e 5645 5254 4552        "CONVERTER
+00010540: 5f49 4d41 4745 223a 2063 686f 7365 6e5f  _IMAGE": chosen_
+00010550: 636f 6e76 6572 7465 722c 0a20 2020 2020  converter,.     
+00010560: 2020 2020 2020 2022 5343 5249 5054 5f50         "SCRIPT_P
+00010570: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
+00010580: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
+00010590: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000105a0: 434f 4e46 4947 5f46 494c 4522 3a20 6622  CONFIG_FILE": f"
+000105b0: 7b63 6f6e 6669 675f 6669 6c65 7d22 0a20  {config_file}". 
+000105c0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+000105d0: 2020 636f 6e76 6572 7369 6f6e 5f63 6d64    conversion_cmd
+000105e0: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
+000105f0: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
+00010600: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
+00010610: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
+00010620: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
+00010630: 2d2d 6172 7261 793d 312d 244e 2024 5343  --array=1-$N $SC
+00010640: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
+00010650: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
+00010660: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
+00010670: 7369 6f6e 5f63 6d64 5f77 6169 7469 6e67  sion_cmd_waiting
+00010680: 203d 2022 7362 6174 6368 202d 2d6a 6f62   = "sbatch --job
+00010690: 2d6e 616d 653d 636f 6e76 6572 7369 6f6e  -name=conversion
+000106a0: 202d 2d65 7870 6f72 743d 414c 4c2c 434f   --export=ALL,CO
+000106b0: 4e46 4947 5f50 4154 483d 5c22 2450 5744  NFIG_PATH=\"$PWD
+000106c0: 2f24 434f 4e46 4947 5f46 494c 455c 2220  /$CONFIG_FILE\" 
+000106d0: 2d2d 6172 7261 793d 312d 244e 202d 2d77  --array=1-$N --w
+000106e0: 6169 7420 2453 4352 4950 545f 5041 5448  ait $SCRIPT_PATH
+000106f0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
+00010700: 6179 2e73 6822 0a0a 2020 2020 2020 2020  ay.sh"..        
+00010710: 7265 7475 726e 2063 6f6e 7665 7273 696f  return conversio
+00010720: 6e5f 636d 642c 2073 6261 7463 685f 656e  n_cmd, sbatch_en
+00010730: 760a 0a20 2020 2064 6566 2077 6f72 6b66  v..    def workf
+00010740: 6c6f 775f 7061 7261 6d73 5f74 6f5f 656e  low_params_to_en
+00010750: 7676 6172 7328 7365 6c66 2c20 2a2a 6b77  vvars(self, **kw
+00010760: 6172 6773 2920 2d3e 2044 6963 743a 0a20  args) -> Dict:. 
+00010770: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010780: 2020 2043 6f6e 7665 7274 2077 6f72 6b66     Convert workf
+00010790: 6c6f 7720 7061 7261 6d65 7465 7273 2074  low parameters t
+000107a0: 6f20 656e 7669 726f 6e6d 656e 7420 7661  o environment va
+000107b0: 7269 6162 6c65 732e 0a0a 2020 2020 2020  riables...      
+000107c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000107d0: 2020 2020 2a2a 6b77 6172 6773 3a20 4164      **kwargs: Ad
+000107e0: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+000107f0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
+00010800: 6865 2077 6f72 6b66 6c6f 772e 0a0a 2020  he workflow...  
+00010810: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00010820: 2020 2020 2020 2020 2020 2044 6963 743a             Dict:
+00010830: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00010840: 6e74 6169 6e69 6e67 2074 6865 2065 6e76  ntaining the env
+00010850: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00010860: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00010870: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+00010880: 5f65 6e76 203d 207b 6b65 792e 7570 7065  _env = {key.uppe
+00010890: 7228 293a 2066 227b 7661 6c75 657d 2220  r(): f"{value}" 
+000108a0: 666f 7220 6b65 792c 0a20 2020 2020 2020  for key,.       
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2076 616c 7565 2069 6e20 6b77 6172 6773   value in kwargs
+000108d0: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
+000108e0: 2020 6c6f 6767 6572 2e64 6562 7567 2877    logger.debug(w
+000108f0: 6f72 6b66 6c6f 775f 656e 7629 0a20 2020  orkflow_env).   
+00010900: 2020 2020 2072 6574 7572 6e20 776f 726b       return work
+00010910: 666c 6f77 5f65 6e76 0a0a 2020 2020 6465  flow_env..    de
+00010920: 6620 6765 745f 6365 6c6c 706f 7365 5f63  f get_cellpose_c
+00010930: 6f6d 6d61 6e64 2873 656c 662c 2069 6d61  ommand(self, ima
+00010940: 6765 5f76 6572 7369 6f6e 3a20 7374 722c  ge_version: str,
+00010950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010960: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00010970: 7075 745f 6461 7461 3a20 7374 722c 0a20  put_data: str,. 
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 2020 2020 2020 2020 2020 2020 6370 5f6d              cp_m
+000109a0: 6f64 656c 3a20 7374 722c 0a20 2020 2020  odel: str,.     
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109c0: 2020 2020 2020 2020 6e75 635f 6368 616e          nuc_chan
+000109d0: 6e65 6c3a 2069 6e74 2c0a 2020 2020 2020  nel: int,.      
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 2020 2020 2020 2070 726f 625f 7468 7265         prob_thre
+00010a00: 7368 6f6c 643a 2066 6c6f 6174 2c0a 2020  shold: float,.  
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00010a30: 6469 616d 6574 6572 3a20 666c 6f61 742c  diameter: float,
+00010a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a50: 2020 2020 2020 2020 2020 2020 2020 656d                em
+00010a60: 6169 6c3a 204f 7074 696f 6e61 6c5b 7374  ail: Optional[st
+00010a70: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a90: 2020 2020 2020 2020 7469 6d65 3a20 4f70          time: Op
+00010aa0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00010ab0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ad0: 2075 7365 5f67 7075 3a20 626f 6f6c 203d   use_gpu: bool =
+00010ae0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 6d6f 6465 6c3a 2073 7472 203d      model: str =
+00010b10: 2022 6365 6c6c 706f 7365 2229 202d 3e20   "cellpose") -> 
+00010b20: 5475 706c 655b 7374 722c 2044 6963 745d  Tuple[str, Dict]
+00010b30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010b40: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00010b50: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
+00010b60: 6972 6f6e 6d65 6e74 2064 6963 7469 6f6e  ironment diction
+00010b70: 6172 7920 746f 2072 756e 2061 2043 656c  ary to run a Cel
+00010b80: 6c50 6f73 6520 6a6f 620a 2020 2020 2020  lPose job.      
+00010b90: 2020 6f6e 2074 6865 2053 6c75 726d 2077    on the Slurm w
+00010ba0: 6f72 6b6c 6f61 6420 6d61 6e61 6765 722e  orkload manager.
+00010bb0: 0a20 2020 2020 2020 2041 2073 7065 6369  .        A speci
+00010bc0: 6669 6320 6578 616d 706c 6520 6f66 2075  fic example of u
+00010bd0: 7369 6e67 2074 6865 2067 656e 6572 6963  sing the generic
+00010be0: 2027 6765 745f 776f 726b 666c 6f77 5f63   'get_workflow_c
+00010bf0: 6f6d 6d61 6e64 272e 0a0a 2020 2020 2020  ommand'...      
+00010c00: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00010c10: 2020 2020 696d 6167 655f 7665 7273 696f      image_versio
+00010c20: 6e20 2873 7472 293a 2054 6865 2076 6572  n (str): The ver
+00010c30: 7369 6f6e 206f 6620 7468 6520 5369 6e67  sion of the Sing
+00010c40: 756c 6172 6974 7920 696d 6167 6520 746f  ularity image to
+00010c50: 2075 7365 2e0a 2020 2020 2020 2020 2020   use..          
+00010c60: 2020 696e 7075 745f 6461 7461 2028 7374    input_data (st
+00010c70: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
+00010c80: 7468 6520 696e 7075 7420 6461 7461 2066  the input data f
+00010c90: 6f6c 6465 7220 6f6e 2074 6865 2073 6861  older on the sha
+00010ca0: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
+00010cb0: 2020 2020 6669 6c65 2073 7973 7465 6d2e      file system.
+00010cc0: 0a20 2020 2020 2020 2020 2020 2063 705f  .            cp_
+00010cd0: 6d6f 6465 6c20 2873 7472 293a 2054 6865  model (str): The
+00010ce0: 206e 616d 6520 6f66 2074 6865 2043 656c   name of the Cel
+00010cf0: 6c50 6f73 6520 6d6f 6465 6c20 746f 2075  lPose model to u
+00010d00: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+00010d10: 6e75 635f 6368 616e 6e65 6c20 2869 6e74  nuc_channel (int
+00010d20: 293a 2054 6865 2069 6e64 6578 206f 6620  ): The index of 
+00010d30: 7468 6520 6e75 636c 6561 7220 6368 616e  the nuclear chan
+00010d40: 6e65 6c2e 0a20 2020 2020 2020 2020 2020  nel..           
+00010d50: 2070 726f 625f 7468 7265 7368 6f6c 6420   prob_threshold 
+00010d60: 2866 6c6f 6174 293a 2054 6865 2070 726f  (float): The pro
+00010d70: 6261 6269 6c69 7479 2074 6872 6573 686f  bability thresho
+00010d80: 6c64 2066 6f72 0a20 2020 2020 2020 2020  ld for.         
+00010d90: 2020 2020 2020 206e 7563 6c65 6920 6465         nuclei de
+00010da0: 7465 6374 696f 6e2e 0a20 2020 2020 2020  tection..       
+00010db0: 2020 2020 2063 656c 6c5f 6469 616d 6574       cell_diamet
+00010dc0: 6572 2028 666c 6f61 7429 3a20 5468 6520  er (float): The 
+00010dd0: 6578 7065 6374 6564 2063 656c 6c20 6469  expected cell di
+00010de0: 616d 6574 6572 2069 6e20 7069 7865 6c73  ameter in pixels
+00010df0: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+00010e00: 6169 6c20 284f 7074 696f 6e61 6c5b 7374  ail (Optional[st
+00010e10: 725d 293a 2054 6865 2065 6d61 696c 2061  r]): The email a
+00010e20: 6464 7265 7373 2074 6f20 7365 6e64 206e  ddress to send n
+00010e30: 6f74 6966 6963 6174 696f 6e73 2074 6f2e  otifications to.
+00010e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e50: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00010e60: 652e 0a20 2020 2020 2020 2020 2020 2074  e..            t
+00010e70: 696d 6520 284f 7074 696f 6e61 6c5b 7374  ime (Optional[st
+00010e80: 725d 293a 2054 6865 206d 6178 696d 756d  r]): The maximum
+00010e90: 2074 696d 6520 666f 7220 7468 6520 6a6f   time for the jo
+00010ea0: 6220 746f 2072 756e 2e0a 2020 2020 2020  b to run..      
+00010eb0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00010ec0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00010ed0: 2020 2020 2020 2020 7573 655f 6770 7520          use_gpu 
+00010ee0: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+00010ef0: 746f 2075 7365 2047 5055 2066 6f72 2074  to use GPU for t
+00010f00: 6865 2043 656c 6c50 6f73 6520 6a6f 622e  he CellPose job.
+00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f20: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+00010f30: 652e 0a20 2020 2020 2020 2020 2020 206d  e..            m
+00010f40: 6f64 656c 2028 7374 7229 3a20 5468 6520  odel (str): The 
+00010f50: 6e61 6d65 206f 6620 7468 6520 666f 6c64  name of the fold
+00010f60: 6572 206f 6620 7468 6520 446f 636b 6572  er of the Docker
+00010f70: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00010f90: 6566 6175 6c74 7320 746f 2022 6365 6c6c  efaults to "cell
+00010fa0: 706f 7365 222e 0a0a 2020 2020 2020 2020  pose"...        
+00010fb0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00010fc0: 2020 2020 2054 7570 6c65 5b73 7472 2c20       Tuple[str, 
+00010fd0: 6469 6374 5d3a 0a20 2020 2020 2020 2020  dict]:.         
+00010fe0: 2020 2020 2020 2041 2074 7570 6c65 2063         A tuple c
+00010ff0: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00011000: 7572 6d20 7362 6174 6368 2063 6f6d 6d61  urm sbatch comma
+00011010: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00011020: 2020 2061 6e64 2074 6865 2065 6e76 6972     and the envir
+00011030: 6f6e 6d65 6e74 2064 6963 7469 6f6e 6172  onment dictionar
+00011040: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+00011050: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011060: 6c66 2e67 6574 5f77 6f72 6b66 6c6f 775f  lf.get_workflow_
+00011070: 636f 6d6d 616e 6428 776f 726b 666c 6f77  command(workflow
+00011080: 3d6d 6f64 656c 2c0a 2020 2020 2020 2020  =model,.        
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
+000110c0: 6e3d 696d 6167 655f 7665 7273 696f 6e2c  n=image_version,
+000110d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+00011100: 6461 7461 3d69 6e70 7574 5f64 6174 612c  data=input_data,
+00011110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011130: 2020 2020 2020 2020 2020 656d 6169 6c3d            email=
+00011140: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 7469 6d65 3d74 696d 652c 0a20 2020 2020  time=time,.     
+00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2020 2020 6370 5f6d 6f64 656c 3d63 705f      cp_model=cp_
+000111b0: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111e0: 6e75 635f 6368 616e 6e65 6c3d 6e75 635f  nuc_channel=nuc_
+000111f0: 6368 616e 6e65 6c2c 0a20 2020 2020 2020  channel,.       
+00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011220: 2020 7072 6f62 5f74 6872 6573 686f 6c64    prob_threshold
+00011230: 3d70 726f 625f 7468 7265 7368 6f6c 642c  =prob_threshold,
+00011240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011260: 2020 2020 2020 2020 2020 6365 6c6c 5f64            cell_d
+00011270: 6961 6d65 7465 723d 6365 6c6c 5f64 6961  iameter=cell_dia
+00011280: 6d65 7465 722c 0a20 2020 2020 2020 2020  meter,.         
+00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112b0: 7573 655f 6770 753d 7573 655f 6770 7529  use_gpu=use_gpu)
+000112c0: 0a0a 2020 2020 6465 6620 636f 7079 5f7a  ..    def copy_z
+000112d0: 6970 5f6c 6f63 616c 6c79 2873 656c 662c  ip_locally(self,
+000112e0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
+000112f0: 6765 3a20 7374 722c 2066 696c 656e 616d  ge: str, filenam
+00011300: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2920 2d3e 2054 7261 6e73 6665 7252 6573  ) -> TransferRes
+00011330: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
+00011340: 2043 6f70 7920 6120 7a69 7020 6669 6c65   Copy a zip file
+00011350: 2066 726f 6d20 536c 7572 6d20 746f 2074   from Slurm to t
+00011360: 6865 206c 6f63 616c 2073 6572 7665 722e  he local server.
+00011370: 0a0a 2020 2020 2020 2020 4e6f 7465 2061  ..        Note a
+00011380: 626f 7574 2028 5472 616e 7366 6572 2952  bout (Transfer)R
+00011390: 6573 756c 743a 0a0a 2020 2020 2020 2020  esult:..        
+000113a0: 556e 6c69 6b65 2073 696d 696c 6172 2063  Unlike similar c
+000113b0: 6c61 7373 6573 2073 7563 6820 6173 2069  lasses such as i
+000113c0: 6e76 6f6b 652e 7275 6e6e 6572 732e 5265  nvoke.runners.Re
+000113d0: 7375 6c74 206f 720a 2020 2020 2020 2020  sult or.        
+000113e0: 6661 6272 6963 2e72 756e 6e65 7273 2e52  fabric.runners.R
+000113f0: 6573 756c 740a 2020 2020 2020 2020 2877  esult.        (w
+00011400: 6869 6368 2068 6176 6520 6120 636f 6e63  hich have a conc
+00011410: 6570 7420 6f66 20e2 809c 7761 726e 2061  ept of ...warn a
+00011420: 6e64 2072 6574 7572 6e20 616e 7977 6179  nd return anyway
+00011430: 7320 6f6e 2066 6169 6c75 7265 e280 9d29  s on failure...)
+00011440: 0a20 2020 2020 2020 2074 6869 7320 636c  .        this cl
+00011450: 6173 7320 6861 7320 6e6f 2075 7365 6675  ass has no usefu
+00011460: 6c20 7472 7574 6869 6e65 7373 2062 6568  l truthiness beh
+00011470: 6176 696f 722e 0a20 2020 2020 2020 2049  avior..        I
+00011480: 6620 6120 6669 6c65 2074 7261 6e73 6665  f a file transfe
+00011490: 7220 6661 696c 732c 2073 6f6d 6520 6578  r fails, some ex
+000114a0: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
+000114b0: 7261 6973 6564 2c0a 2020 2020 2020 2020  raised,.        
+000114c0: 6569 7468 6572 2061 6e20 4f53 4572 726f  either an OSErro
+000114d0: 7220 6f72 2061 6e20 6572 726f 7220 6672  r or an error fr
+000114e0: 6f6d 2077 6974 6869 6e20 5061 7261 6d69  om within Parami
+000114f0: 6b6f 2e0a 0a20 2020 2020 2020 2041 7267  ko...        Arg
+00011500: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+00011510: 6f63 616c 5f74 6d70 5f73 746f 7261 6765  ocal_tmp_storage
+00011520: 2028 5374 7269 6e67 293a 2050 6174 6820   (String): Path 
+00011530: 746f 2073 746f 7265 2074 6865 207a 6970  to store the zip
+00011540: 2066 696c 6520 6c6f 6361 6c6c 792e 0a20   file locally.. 
+00011550: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+00011560: 616d 6520 2853 7472 696e 6729 3a20 5a69  ame (String): Zi
+00011570: 7020 6669 6c65 6e61 6d65 206f 6e20 536c  p filename on Sl
+00011580: 7572 6d2e 0a0a 2020 2020 2020 2020 5265  urm...        Re
+00011590: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000115a0: 2020 2054 7261 6e73 6665 7252 6573 756c     TransferResul
+000115b0: 743a 2054 6865 2072 6573 756c 7420 6f66  t: The result of
+000115c0: 2074 6865 2073 6370 2061 7474 656d 7074   the scp attempt
+000115d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000115e0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+000115f0: 6f28 6622 436f 7079 696e 6720 7a69 7020  o(f"Copying zip 
+00011600: 7b66 696c 656e 616d 657d 2066 726f 6d5c  {filename} from\
+00011610: 0a20 2020 2020 2020 2020 2020 2053 6c75  .            Slu
+00011620: 726d 2074 6f20 7b6c 6f63 616c 5f74 6d70  rm to {local_tmp
+00011630: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
+00011640: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00011650: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
+00011660: 2072 656d 6f74 653d 6622 7b66 696c 656e   remote=f"{filen
+00011670: 616d 657d 2e7a 6970 222c 0a20 2020 2020  ame}.zip",.     
+00011680: 2020 2020 2020 206c 6f63 616c 3d6c 6f63         local=loc
+00011690: 616c 5f74 6d70 5f73 746f 7261 6765 290a  al_tmp_storage).
+000116a0: 0a20 2020 2064 6566 207a 6970 5f64 6174  .    def zip_dat
+000116b0: 615f 6f6e 5f73 6c75 726d 5f73 6572 7665  a_on_slurm_serve
+000116c0: 7228 7365 6c66 2c20 6461 7461 5f6c 6f63  r(self, data_loc
+000116d0: 6174 696f 6e3a 2073 7472 2c20 6669 6c65  ation: str, file
+000116e0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 2020 2020 2020 2020 2020 2020 656e 763a              env:
+00011710: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00011720: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
+00011730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011750: 2020 2920 2d3e 2052 6573 756c 743a 0a20    ) -> Result:. 
+00011760: 2020 2020 2020 2022 2222 5a69 7020 7468         """Zip th
+00011770: 6520 6f75 7470 7574 2066 6f6c 6465 7220  e output folder 
+00011780: 6f66 2061 206a 6f62 206f 6e20 536c 7572  of a job on Slur
+00011790: 6d0a 0a20 2020 2020 2020 2041 7267 733a  m..        Args:
+000117a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000117b0: 615f 6c6f 6361 7469 6f6e 2028 5374 7269  a_location (Stri
+000117c0: 6e67 293a 2046 6f6c 6465 7220 6f6e 2053  ng): Folder on S
+000117d0: 4c55 524d 2077 6974 6820 7468 6520 2264  LURM with the "d
+000117e0: 6174 612f 6f75 7422 0a20 2020 2020 2020  ata/out".       
+000117f0: 2020 2020 2020 2020 2073 7562 666f 6c64           subfold
+00011800: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+00011810: 6669 6c65 6e61 6d65 2028 5374 7269 6e67  filename (String
+00011820: 293a 204e 616d 6520 746f 2067 6976 6520  ): Name to give 
+00011830: 746f 2074 6865 207a 6970 6669 6c65 2e0a  to the zipfile..
+00011840: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+00011850: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
+00011860: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
+00011870: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
+00011880: 2076 6172 6961 626c 6573 2074 6f20 0a20   variables to . 
+00011890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000118a0: 6574 2077 6865 6e20 7275 6e6e 696e 6720  et when running 
+000118b0: 7468 6520 636f 6d6d 616e 642e 2044 6566  the command. Def
+000118c0: 6175 6c74 7320 746f 204e 6f6e 652e 0a0a  aults to None...
+000118d0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000118e0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+000118f0: 756c 743a 2054 6865 2072 6573 756c 7420  ult: The result 
+00011900: 6f66 2074 6865 207a 6970 2061 7474 656d  of the zip attem
+00011910: 7074 2e0a 2020 2020 2020 2020 2222 220a  pt..        """.
+00011920: 2020 2020 2020 2020 2320 7a69 700a 2020          # zip.  
+00011930: 2020 2020 2020 7a69 705f 636d 6420 3d20        zip_cmd = 
+00011940: 7365 6c66 2e67 6574 5f7a 6970 5f63 6f6d  self.get_zip_com
+00011950: 6d61 6e64 2864 6174 615f 6c6f 6361 7469  mand(data_locati
+00011960: 6f6e 2c20 6669 6c65 6e61 6d65 290a 2020  on, filename).  
+00011970: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00011980: 6f28 6622 5a69 7070 696e 6720 7b64 6174  o(f"Zipping {dat
+00011990: 615f 6c6f 6361 7469 6f6e 7d20 6173 207b  a_location} as {
+000119a0: 6669 6c65 6e61 6d65 7d20 6f6e 2053 6c75  filename} on Slu
+000119b0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
+000119c0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
+000119d0: 6d61 6e64 7328 5b7a 6970 5f63 6d64 5d2c  mands([zip_cmd],
+000119e0: 2065 6e76 3d65 6e76 290a 0a20 2020 2064   env=env)..    d
+000119f0: 6566 2067 6574 5f7a 6970 5f63 6f6d 6d61  ef get_zip_comma
+00011a00: 6e64 2873 656c 662c 2064 6174 615f 6c6f  nd(self, data_lo
+00011a10: 6361 7469 6f6e 3a20 7374 722c 2066 696c  cation: str, fil
+00011a20: 656e 616d 653a 2073 7472 2920 2d3e 2073  ename: str) -> s
+00011a30: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
+00011a40: 2020 2020 2020 2020 4765 6e65 7261 7465          Generate
+00011a50: 2061 2063 6f6d 6d61 6e64 2073 7472 696e   a command strin
+00011a60: 6720 666f 7220 7a69 7070 696e 6720 7468  g for zipping th
+00011a70: 6520 6461 7461 206f 6e20 536c 7572 6d2e  e data on Slurm.
+00011a80: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00011a90: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00011aa0: 5f6c 6f63 6174 696f 6e20 2873 7472 293a  _location (str):
+00011ab0: 2054 6865 2066 6f6c 6465 7220 746f 2062   The folder to b
+00011ac0: 6520 7a69 7070 6564 2e0a 2020 2020 2020  e zipped..      
+00011ad0: 2020 2020 2020 6669 6c65 6e61 6d65 2028        filename (
+00011ae0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+00011af0: 6620 7468 6520 7a69 7020 6172 6368 6976  f the zip archiv
+00011b00: 6520 6669 6c65 2074 6f20 6578 7472 6163  e file to extrac
+00011b10: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+00011b20: 2020 2057 6974 686f 7574 2065 7874 656e     Without exten
+00011b30: 7369 6f6e 2e0a 0a20 2020 2020 2020 2052  sion...        R
+00011b40: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00011b50: 2020 2020 7374 723a 2054 6865 2063 6f6d      str: The com
+00011b60: 6d61 6e64 2074 6f20 6372 6561 7465 2074  mand to create t
+00011b70: 6865 207a 6970 2066 696c 652e 0a20 2020  he zip file..   
+00011b80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011b90: 2072 6574 7572 6e20 7365 6c66 2e5f 5a49   return self._ZI
+00011ba0: 505f 434d 442e 666f 726d 6174 2866 696c  P_CMD.format(fil
+00011bb0: 656e 616d 653d 6669 6c65 6e61 6d65 2c0a  ename=filename,.
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
+00011bf0: 6e3d 6461 7461 5f6c 6f63 6174 696f 6e29  n=data_location)
+00011c00: 0a0a 2020 2020 6465 6620 6765 745f 6c6f  ..    def get_lo
+00011c10: 6766 696c 655f 6672 6f6d 5f73 6c75 726d  gfile_from_slurm
+00011c20: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c40: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
+00011c50: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
+00011c80: 705f 7374 6f72 6167 653a 2073 7472 203d  p_storage: str =
+00011c90: 2022 2f74 6d70 2f22 2c0a 2020 2020 2020   "/tmp/",.      
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00011cc0: 3a20 7374 7220 3d20 4e6f 6e65 0a20 2020  : str = None.   
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ce0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
+00011cf0: 2054 7570 6c65 5b73 7472 2c20 7374 722c   Tuple[str, str,
+00011d00: 2054 7261 6e73 6665 7252 6573 756c 745d   TransferResult]
+00011d10: 3a0a 2020 2020 2020 2020 2222 2243 6f70  :.        """Cop
+00011d20: 7920 7468 6520 6c6f 6766 696c 6520 6f66  y the logfile of
+00011d30: 2074 6865 2067 6976 656e 2053 4c55 524d   the given SLURM
+00011d40: 206a 6f62 2074 6f20 7468 6520 6c6f 6361   job to the loca
+00011d50: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
+00011d60: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
+00011d70: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
+00011d80: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
+00011d90: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
+00011da0: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
+00011db0: 756e 6e65 7273 2e52 6573 756c 740a 2020  unners.Result.  
+00011dc0: 2020 2020 2020 6f72 2066 6162 7269 632e        or fabric.
+00011dd0: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
+00011de0: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
+00011df0: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
+00011e00: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
+00011e10: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
+00011e20: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
+00011e30: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
+00011e40: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
+00011e50: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
+00011e60: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
+00011e70: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
+00011e80: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
+00011e90: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
+00011ea0: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
+00011eb0: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
+00011ec0: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
+00011ed0: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
+00011ee0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00011ef0: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
+00011f00: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
+00011f10: 4944 206f 6620 7468 6520 534c 5552 4d20  ID of the SLURM 
+00011f20: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
+00011f30: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
+00011f40: 6765 2028 7374 722c 206f 7074 696f 6e61  ge (str, optiona
+00011f50: 6c29 3a20 5061 7468 2074 6f20 7374 6f72  l): Path to stor
+00011f60: 6520 7468 6520 6c6f 6766 696c 6520 0a20  e the logfile . 
+00011f70: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011f80: 6f63 616c 6c79 2e20 4465 6661 756c 7473  ocally. Defaults
+00011f90: 2074 6f20 222f 746d 702f 222e 0a20 2020   to "/tmp/"..   
+00011fa0: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00011fb0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00011fc0: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
+00011fd0: 6766 696c 6520 6f6e 2074 6865 2053 4c55  gfile on the SLU
+00011fe0: 524d 2073 6572 7665 722e 0a20 2020 2020  RM server..     
+00011ff0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00012000: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
+00012010: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00012020: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+00012030: 3a20 6469 7265 6374 6f72 792c 2066 756c  : directory, ful
+00012040: 6c20 7061 7468 206f 6620 7468 6520 6c6f  l path of the lo
+00012050: 6766 696c 652c 2061 6e64 2054 7261 6e73  gfile, and Trans
+00012060: 6665 7252 6573 756c 740a 2020 2020 2020  ferResult.      
+00012070: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00012080: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
+00012090: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000120a0: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
+000120b0: 4746 494c 450a 2020 2020 2020 2020 6c6f  GFILE.        lo
+000120c0: 6766 696c 6520 3d20 6c6f 6766 696c 652e  gfile = logfile.
+000120d0: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
+000120e0: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
+000120f0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00012100: 2e69 6e66 6f28 6622 436f 7079 696e 6720  .info(f"Copying 
+00012110: 6c6f 6766 696c 6520 7b6c 6f67 6669 6c65  logfile {logfile
+00012120: 7d20 6672 6f6d 2053 6c75 726d 5c0a 2020  } from Slurm\.  
+00012130: 2020 2020 2020 2020 2020 746f 207b 6c6f            to {lo
+00012140: 6361 6c5f 746d 705f 7374 6f72 6167 657d  cal_tmp_storage}
+00012150: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
+00012160: 7420 3d20 7365 6c66 2e67 6574 280a 2020  t = self.get(.  
+00012170: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
+00012180: 3d6c 6f67 6669 6c65 2c0a 2020 2020 2020  =logfile,.      
+00012190: 2020 2020 2020 6c6f 6361 6c3d 6c6f 6361        local=loca
+000121a0: 6c5f 746d 705f 7374 6f72 6167 6529 0a20  l_tmp_storage). 
+000121b0: 2020 2020 2020 2065 7870 6f72 745f 6669         export_fi
+000121c0: 6c65 203d 206c 6f63 616c 5f74 6d70 5f73  le = local_tmp_s
+000121d0: 746f 7261 6765 2b6c 6f67 6669 6c65 0a20  torage+logfile. 
+000121e0: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+000121f0: 6361 6c5f 746d 705f 7374 6f72 6167 652c  cal_tmp_storage,
+00012200: 2065 7870 6f72 745f 6669 6c65 2c20 7265   export_file, re
+00012210: 7375 6c74 0a0a 2020 2020 6465 6620 6765  sult..    def ge
+00012220: 745f 756e 7a69 705f 636f 6d6d 616e 6428  t_unzip_command(
+00012230: 7365 6c66 2c20 7a69 7066 696c 653a 2073  self, zipfile: s
+00012240: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00012250: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00012260: 6c74 6572 5f66 696c 6574 7970 6573 3a20  lter_filetypes: 
+00012270: 7374 7220 3d20 222a 2e7a 6172 7220 2a2e  str = "*.zarr *.
+00012280: 7469 6666 202a 2e74 6966 220a 2020 2020  tiff *.tif".    
+00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122a0: 2020 2020 2020 2920 2d3e 2073 7472 3a0a        ) -> str:.
+000122b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000122c0: 2020 2020 4765 6e65 7261 7465 2061 2063      Generate a c
+000122d0: 6f6d 6d61 6e64 2073 7472 696e 6720 666f  ommand string fo
+000122e0: 7220 756e 7a69 7070 696e 6720 6120 6461  r unzipping a da
+000122f0: 7461 2061 7263 6869 7665 2061 6e64 2063  ta archive and c
+00012300: 7265 6174 696e 670a 2020 2020 2020 2020  reating.        
+00012310: 7265 7175 6972 6564 2064 6972 6563 746f  required directo
+00012320: 7269 6573 2066 6f72 2053 6c75 726d 206a  ries for Slurm j
+00012330: 6f62 732e 0a0a 2020 2020 2020 2020 4172  obs...        Ar
+00012340: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00012350: 7a69 7066 696c 6520 2873 7472 293a 2054  zipfile (str): T
+00012360: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
+00012370: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
+00012380: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
+00012390: 2020 2020 2020 2020 2020 2020 5769 7468              With
+000123a0: 6f75 7420 6578 7465 6e73 696f 6e2e 0a20  out extension.. 
+000123b0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+000123c0: 725f 6669 6c65 7479 7065 7320 2873 7472  r_filetypes (str
+000123d0: 2c20 6f70 7469 6f6e 616c 293a 2041 2073  , optional): A s
+000123e0: 7061 6365 2d73 6570 6172 6174 6564 2073  pace-separated s
+000123f0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+00012400: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
+00012410: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
+00012420: 696f 6e73 2074 6f20 6578 7472 6163 7420  ions to extract 
+00012430: 6672 6f6d 2074 6865 207a 6970 2066 696c  from the zip fil
+00012440: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00012450: 2020 2045 2e67 2e20 6465 6661 756c 7473     E.g. defaults
+00012460: 2074 6f20 222a 2e7a 6172 7220 2a2e 7469   to "*.zarr *.ti
+00012470: 6666 202a 2e74 6966 222e 0a20 2020 2020  ff *.tif"..     
+00012480: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
+00012490: 6e67 2074 6869 7320 6172 6775 6d65 6e74  ng this argument
+000124a0: 2074 6f20 604e 6f6e 6560 2077 696c 6c20   to `None` will 
+000124b0: 6f6d 6974 2074 6865 2066 696c 650a 2020  omit the file.  
+000124c0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000124d0: 6c74 6572 2061 6e64 2065 7874 7261 6374  lter and extract
+000124e0: 2061 6c6c 2066 696c 6573 2e0a 0a20 2020   all files...   
+000124f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00012500: 2020 2020 2020 2020 2020 7374 723a 0a20            str:. 
+00012510: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00012520: 6865 2063 6f6d 6d61 6e64 2074 6f20 6578  he command to ex
+00012530: 7472 6163 7420 7468 6520 7370 6563 6966  tract the specif
+00012540: 6965 640a 2020 2020 2020 2020 2020 2020  ied.            
+00012550: 2020 2020 6669 6c65 7479 7065 7320 6672      filetypes fr
+00012560: 6f6d 2074 6865 207a 6970 2066 696c 652e  om the zip file.
+00012570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012580: 2020 2020 2075 6e7a 6970 5f63 6d64 203d       unzip_cmd =
+00012590: 2066 226d 6b64 6972 207b 7365 6c66 2e73   f"mkdir {self.s
+000125a0: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
+000125b0: 7b7a 6970 6669 6c65 7d20 5c0a 2020 2020  {zipfile} \.    
+000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125d0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
+000125e0: 5f70 6174 687d 2f7b 7a69 7066 696c 657d  _path}/{zipfile}
+000125f0: 2f64 6174 6120 5c0a 2020 2020 2020 2020  /data \.        
+00012600: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
+00012610: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
+00012620: 687d 2f7b 7a69 7066 696c 657d 2f64 6174  h}/{zipfile}/dat
+00012630: 612f 696e 205c 0a20 2020 2020 2020 2020  a/in \.         
+00012640: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+00012650: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+00012660: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
+00012670: 2f6f 7574 205c 0a20 2020 2020 2020 2020  /out \.         
+00012680: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+00012690: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+000126a0: 7d2f 7b7a 6970 6669 6c65 7d2f 6461 7461  }/{zipfile}/data
+000126b0: 2f67 743b 205c 0a20 2020 2020 2020 2020  /gt; \.         
+000126c0: 2020 2020 2020 2020 2020 2037 7a20 7820             7z x 
+000126d0: 2d79 202d 6f7b 7365 6c66 2e73 6c75 726d  -y -o{self.slurm
+000126e0: 5f64 6174 615f 7061 7468 7d2f 7b7a 6970  _data_path}/{zip
+000126f0: 6669 6c65 7d2f 6461 7461 2f69 6e20 5c0a  file}/data/in \.
+00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012710: 2020 2020 7b73 656c 662e 736c 7572 6d5f      {self.slurm_
+00012720: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
+00012730: 696c 657d 2e7a 6970 207b 6669 6c74 6572  ile}.zip {filter
+00012740: 5f66 696c 6574 7970 6573 7d22 0a0a 2020  _filetypes}"..  
+00012750: 2020 2020 2020 7265 7475 726e 2075 6e7a        return unz
+00012760: 6970 5f63 6d64 0a0a 2020 2020 6465 6620  ip_cmd..    def 
+00012770: 6765 745f 696d 6167 655f 7665 7273 696f  get_image_versio
+00012780: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
+00012790: 7328 7365 6c66 2c20 6d6f 6465 6c3a 2073  s(self, model: s
+000127a0: 7472 0a20 2020 2020 2020 2020 2020 2020  tr.             
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+000127d0: 3e20 5475 706c 655b 4c69 7374 5b73 7472  > Tuple[List[str
+000127e0: 5d2c 204c 6973 745b 7374 725d 5d3a 0a20  ], List[str]]:. 
+000127f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012800: 2020 2052 6574 7269 6576 6520 7468 6520     Retrieve the 
+00012810: 6176 6169 6c61 626c 6520 696d 6167 6520  available image 
+00012820: 7665 7273 696f 6e73 2061 6e64 2069 6e70  versions and inp
+00012830: 7574 2064 6174 6120 6669 6c65 7320 666f  ut data files fo
+00012840: 7220 610a 2020 2020 2020 2020 6769 7665  r a.        give
+00012850: 6e20 6d6f 6465 6c2e 0a0a 2020 2020 2020  n model...      
+00012860: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00012870: 2020 2020 6d6f 6465 6c20 2873 7472 293a      model (str):
+00012880: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00012890: 206d 6f64 656c 2074 6f20 7175 6572 7920   model to query 
+000128a0: 666f 722e 0a0a 2020 2020 2020 2020 5265  for...        Re
+000128b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000128c0: 2020 2054 7570 6c65 5b4c 6973 745b 7374     Tuple[List[st
+000128d0: 725d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  r], List[str]]:.
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128f0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+00012900: 6e67 2074 776f 206c 6973 7473 3a0a 2020  ng two lists:.  
+00012910: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00012920: 5468 6520 6669 7273 7420 6c69 7374 2069  The first list i
+00012930: 6e63 6c75 6465 7320 7468 6520 6176 6169  ncludes the avai
+00012940: 6c61 626c 6520 696d 6167 6520 7665 7273  lable image vers
+00012950: 696f 6e73 2c20 0a20 2020 2020 2020 2020  ions, .         
+00012960: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00012970: 6420 696e 2064 6573 6365 6e64 696e 6720  d in descending 
+00012980: 6f72 6465 722e 0a20 2020 2020 2020 2020  order..         
+00012990: 2020 2020 2020 202d 2054 6865 2073 6563         - The sec
+000129a0: 6f6e 6420 6c69 7374 2069 6e63 6c75 6465  ond list include
+000129b0: 7320 7468 6520 6176 6169 6c61 626c 6520  s the available 
+000129c0: 6461 7461 2066 696c 6573 2e0a 0a20 2020  data files...   
+000129d0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+000129e0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+000129f0: 726f 723a 2049 6620 7468 6520 7072 6f76  ror: If the prov
+00012a00: 6964 6564 206d 6f64 656c 2069 7320 6e6f  ided model is no
+00012a10: 7420 666f 756e 6420 696e 2074 6865 0a20  t found in the. 
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00012a30: 6c75 726d 436c 6965 6e74 2773 206b 6e6f  lurmClient's kno
+00012a40: 776e 206d 6f64 656c 2070 6174 6873 2e0a  wn model paths..
+00012a50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012a60: 2020 2020 696d 6167 655f 7061 7468 203d      image_path =
+00012a70: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+00012a80: 6c5f 7061 7468 732e 6765 7428 6d6f 6465  l_paths.get(mode
+00012a90: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
+00012aa0: 7420 696d 6167 655f 7061 7468 3a0a 2020  t image_path:.  
+00012ab0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00012ac0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00012ad0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
+00012ae0: 2070 6174 6820 6b6e 6f77 6e20 666f 7220   path known for 
+00012af0: 7072 6f76 6964 6564 206d 6f64 656c 207b  provided model {
+00012b00: 6d6f 6465 6c7d 2c20 5c0a 2020 2020 2020  model}, \.      
+00012b10: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00012b20: 207b 7365 6c66 2e73 6c75 726d 5f6d 6f64   {self.slurm_mod
+00012b30: 656c 5f70 6174 6873 7d22 290a 2020 2020  el_paths}").    
+00012b40: 2020 2020 636d 646c 6973 7420 3d20 5b0a      cmdlist = [.
+00012b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012b60: 2e5f 5645 5253 494f 4e5f 434d 442e 666f  ._VERSION_CMD.fo
+00012b70: 726d 6174 2873 6c75 726d 5f69 6d61 6765  rmat(slurm_image
+00012b80: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
+00012b90: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
-00012be0: 6c65 5b44 6963 745b 7374 722c 204c 6973  le[Dict[str, Lis
-00012bf0: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c30: 2020 4c69 7374 5b73 7472 5d5d 3a0a 2020    List[str]]:.  
-00012c40: 2020 2020 2020 2222 2252 6574 7269 6576        """Retriev
-00012c50: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
-00012c60: 696d 6167 6520 7665 7273 696f 6e73 2061  image versions a
-00012c70: 6e64 2064 6174 6120 6669 6c65 7320 6672  nd data files fr
-00012c80: 6f6d 0a20 2020 2020 2020 2074 6865 2053  om.        the S
-00012c90: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
-00012ca0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00012cb0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00012cc0: 5b44 6963 745b 7374 722c 204c 6973 745b  [Dict[str, List[
-00012cd0: 7374 725d 5d2c 204c 6973 745b 7374 725d  str]], List[str]
-00012ce0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012cf0: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
-00012d00: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
-00012d10: 2020 2020 2020 202d 2041 2064 6963 7469         - A dicti
-00012d20: 6f6e 6172 7920 6d61 7070 696e 6720 6d6f  onary mapping mo
-00012d30: 6465 6c73 2074 6f20 6176 6169 6c61 626c  dels to availabl
-00012d40: 6520 7665 7273 696f 6e73 2e0a 2020 2020  e versions..    
-00012d50: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
-00012d60: 6c69 7374 206f 6620 6176 6169 6c61 626c  list of availabl
-00012d70: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
-00012d80: 6465 7273 2e0a 2020 2020 2020 2020 2222  ders..        ""
-00012d90: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
-00012da0: 6469 6374 203d 207b 7d0a 2020 2020 2020  dict = {}.      
-00012db0: 2020 636d 646c 6973 7420 3d20 5b5d 0a0a    cmdlist = []..
-00012dc0: 2020 2020 2020 2020 666f 7220 7061 7468          for path
-00012dd0: 2069 6e20 7365 6c66 2e73 6c75 726d 5f6d   in self.slurm_m
-00012de0: 6f64 656c 5f70 6174 6873 2e76 616c 7565  odel_paths.value
-00012df0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00012e00: 2070 6174 6863 6d64 203d 2073 656c 662e   pathcmd = self.
-00012e10: 5f56 4552 5349 4f4e 5f43 4d44 2e66 6f72  _VERSION_CMD.for
-00012e20: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00012e30: 2020 2020 2073 6c75 726d 5f69 6d61 6765       slurm_image
-00012e40: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
-00012e50: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012e70: 6d61 6765 5f70 6174 683d 7061 7468 290a  mage_path=path).
-00012e80: 2020 2020 2020 2020 2020 2020 636d 646c              cmdl
-00012e90: 6973 742e 6170 7065 6e64 2870 6174 6863  ist.append(pathc
-00012ea0: 6d64 290a 0a20 2020 2020 2020 2023 2041  md)..        # A
-00012eb0: 6464 2064 6174 6120 7061 7468 2074 6f6f  dd data path too
-00012ec0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
-00012ed0: 2e61 7070 656e 6428 7365 6c66 2e5f 4441  .append(self._DA
-00012ee0: 5441 5f43 4d44 2e66 6f72 6d61 7428 0a20  TA_CMD.format(. 
-00012ef0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-00012f00: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
-00012f10: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
-00012f20: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
-00012f30: 6974 2072 6573 706f 6e73 6573 2070 6572  it responses per
-00012f40: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
-00012f50: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
-00012f60: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00012f70: 6473 5f73 706c 6974 5f6f 7574 2863 6d64  ds_split_out(cmd
-00012f80: 6c69 7374 290a 0a20 2020 2020 2020 2023  list)..        #
-00012f90: 2053 706c 6974 206c 696e 6573 2066 7572   Split lines fur
-00012fa0: 7468 6572 2069 6e74 6f20 7375 626c 6973  ther into sublis
-00012fb0: 7473 0a20 2020 2020 2020 2072 6573 706f  ts.        respo
-00012fc0: 6e73 655f 6c69 7374 203d 205b 7265 7370  nse_list = [resp
-00012fd0: 6f6e 7365 2e73 7472 6970 2829 2e73 706c  onse.strip().spl
-00012fe0: 6974 2827 5c6e 2729 0a20 2020 2020 2020  it('\n').       
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2020 666f 7220 7265 7370 6f6e 7365 2069    for response i
-00013010: 6e20 7265 7370 6f6e 7365 5f6c 6973 745d  n response_list]
-00013020: 0a0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-00013030: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
-00013040: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00013050: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
-00013060: 2020 2020 2023 2052 6574 7572 6e20 6869       # Return hi
-00013070: 6768 6573 7420 7665 7273 696f 6e20 6669  ghest version fi
-00013080: 7273 740a 2020 2020 2020 2020 2020 2020  rst.            
-00013090: 7265 7375 6c74 6469 6374 5b6b 5d20 3d20  resultdict[k] = 
-000130a0: 736f 7274 6564 2872 6573 706f 6e73 655f  sorted(response_
-000130b0: 6c69 7374 5b69 5d2c 2072 6576 6572 7365  list[i], reverse
-000130c0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-000130d0: 7265 7475 726e 2072 6573 756c 7464 6963  return resultdic
-000130e0: 742c 2072 6573 706f 6e73 655f 6c69 7374  t, response_list
-000130f0: 5b2d 315d 0a                             [-1].
+00012bc0: 2020 2020 696d 6167 655f 7061 7468 3d69      image_path=i
+00012bd0: 6d61 6765 5f70 6174 6829 2c0a 2020 2020  mage_path),.    
+00012be0: 2020 2020 2020 2020 7365 6c66 2e5f 4441          self._DA
+00012bf0: 5441 5f43 4d44 2e66 6f72 6d61 7428 736c  TA_CMD.format(sl
+00012c00: 7572 6d5f 6461 7461 5f70 6174 683d 7365  urm_data_path=se
+00012c10: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
+00012c20: 7468 295d 0a20 2020 2020 2020 2023 2073  th)].        # s
+00012c30: 706c 6974 2072 6573 706f 6e73 6573 2070  plit responses p
+00012c40: 6572 2063 6f6d 6d61 6e64 0a20 2020 2020  er command.     
+00012c50: 2020 2072 6573 706f 6e73 655f 6c69 7374     response_list
+00012c60: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00012c70: 616e 6473 5f73 706c 6974 5f6f 7574 2863  ands_split_out(c
+00012c80: 6d64 6c69 7374 290a 2020 2020 2020 2020  mdlist).        
+00012c90: 2320 7370 6c69 7420 6c69 6e65 7320 6675  # split lines fu
+00012ca0: 7274 6865 7220 696e 746f 2073 7562 6c69  rther into subli
+00012cb0: 7374 730a 2020 2020 2020 2020 7265 7370  sts.        resp
+00012cc0: 6f6e 7365 5f6c 6973 7420 3d20 5b72 6573  onse_list = [res
+00012cd0: 706f 6e73 652e 7374 7269 7028 292e 7370  ponse.strip().sp
+00012ce0: 6c69 7428 275c 6e27 290a 2020 2020 2020  lit('\n').      
+00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d00: 2020 2066 6f72 2072 6573 706f 6e73 6520     for response 
+00012d10: 696e 2072 6573 706f 6e73 655f 6c69 7374  in response_list
+00012d20: 5d0a 2020 2020 2020 2020 7265 7370 6f6e  ].        respon
+00012d30: 7365 5f6c 6973 745b 305d 203d 2073 6f72  se_list[0] = sor
+00012d40: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
+00012d50: 745b 305d 2c20 7265 7665 7273 653d 5472  t[0], reverse=Tr
+00012d60: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+00012d70: 726e 2072 6573 706f 6e73 655f 6c69 7374  rn response_list
+00012d80: 5b30 5d2c 2072 6573 706f 6e73 655f 6c69  [0], response_li
+00012d90: 7374 5b31 5d0a 0a20 2020 2064 6566 2067  st[1]..    def g
+00012da0: 6574 5f61 6c6c 5f69 6d61 6765 5f76 6572  et_all_image_ver
+00012db0: 7369 6f6e 735f 616e 645f 6461 7461 5f66  sions_and_data_f
+00012dc0: 696c 6573 2873 656c 660a 2020 2020 2020  iles(self.      
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012df0: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
+00012e00: 6c65 5b44 6963 745b 7374 722c 204c 6973  le[Dict[str, Lis
+00012e10: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 4c69 7374 5b73 7472 5d5d 3a0a 2020    List[str]]:.  
+00012e60: 2020 2020 2020 2222 2252 6574 7269 6576        """Retriev
+00012e70: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
+00012e80: 696d 6167 6520 7665 7273 696f 6e73 2061  image versions a
+00012e90: 6e64 2064 6174 6120 6669 6c65 7320 6672  nd data files fr
+00012ea0: 6f6d 0a20 2020 2020 2020 2074 6865 2053  om.        the S
+00012eb0: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
+00012ec0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00012ed0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
+00012ee0: 5b44 6963 745b 7374 722c 204c 6973 745b  [Dict[str, List[
+00012ef0: 7374 725d 5d2c 204c 6973 745b 7374 725d  str]], List[str]
+00012f00: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00012f10: 2020 2041 2074 7570 6c65 2063 6f6e 7461     A tuple conta
+00012f20: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+00012f30: 2020 2020 2020 202d 2041 2064 6963 7469         - A dicti
+00012f40: 6f6e 6172 7920 6d61 7070 696e 6720 6d6f  onary mapping mo
+00012f50: 6465 6c73 2074 6f20 6176 6169 6c61 626c  dels to availabl
+00012f60: 6520 7665 7273 696f 6e73 2e0a 2020 2020  e versions..    
+00012f70: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
+00012f80: 6c69 7374 206f 6620 6176 6169 6c61 626c  list of availabl
+00012f90: 6520 696e 7075 7420 6461 7461 2066 6f6c  e input data fol
+00012fa0: 6465 7273 2e0a 2020 2020 2020 2020 2222  ders..        ""
+00012fb0: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
+00012fc0: 6469 6374 203d 207b 7d0a 2020 2020 2020  dict = {}.      
+00012fd0: 2020 636d 646c 6973 7420 3d20 5b5d 0a0a    cmdlist = []..
+00012fe0: 2020 2020 2020 2020 666f 7220 7061 7468          for path
+00012ff0: 2069 6e20 7365 6c66 2e73 6c75 726d 5f6d   in self.slurm_m
+00013000: 6f64 656c 5f70 6174 6873 2e76 616c 7565  odel_paths.value
+00013010: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00013020: 2070 6174 6863 6d64 203d 2073 656c 662e   pathcmd = self.
+00013030: 5f56 4552 5349 4f4e 5f43 4d44 2e66 6f72  _VERSION_CMD.for
+00013040: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00013050: 2020 2020 2073 6c75 726d 5f69 6d61 6765       slurm_image
+00013060: 735f 7061 7468 3d73 656c 662e 736c 7572  s_path=self.slur
+00013070: 6d5f 696d 6167 6573 5f70 6174 682c 0a20  m_images_path,. 
+00013080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013090: 6d61 6765 5f70 6174 683d 7061 7468 290a  mage_path=path).
+000130a0: 2020 2020 2020 2020 2020 2020 636d 646c              cmdl
+000130b0: 6973 742e 6170 7065 6e64 2870 6174 6863  ist.append(pathc
+000130c0: 6d64 290a 0a20 2020 2020 2020 2023 2041  md)..        # A
+000130d0: 6464 2064 6174 6120 7061 7468 2074 6f6f  dd data path too
+000130e0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
+000130f0: 2e61 7070 656e 6428 7365 6c66 2e5f 4441  .append(self._DA
+00013100: 5441 5f43 4d44 2e66 6f72 6d61 7428 0a20  TA_CMD.format(. 
+00013110: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00013120: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
+00013130: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
+00013140: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
+00013150: 6974 2072 6573 706f 6e73 6573 2070 6572  it responses per
+00013160: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
+00013170: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
+00013180: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00013190: 6473 5f73 706c 6974 5f6f 7574 2863 6d64  ds_split_out(cmd
+000131a0: 6c69 7374 290a 0a20 2020 2020 2020 2023  list)..        #
+000131b0: 2053 706c 6974 206c 696e 6573 2066 7572   Split lines fur
+000131c0: 7468 6572 2069 6e74 6f20 7375 626c 6973  ther into sublis
+000131d0: 7473 0a20 2020 2020 2020 2072 6573 706f  ts.        respo
+000131e0: 6e73 655f 6c69 7374 203d 205b 7265 7370  nse_list = [resp
+000131f0: 6f6e 7365 2e73 7472 6970 2829 2e73 706c  onse.strip().spl
+00013200: 6974 2827 5c6e 2729 0a20 2020 2020 2020  it('\n').       
+00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013220: 2020 666f 7220 7265 7370 6f6e 7365 2069    for response i
+00013230: 6e20 7265 7370 6f6e 7365 5f6c 6973 745d  n response_list]
+00013240: 0a0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
+00013250: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
+00013260: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00013270: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
+00013280: 2020 2020 2023 2052 6574 7572 6e20 6869       # Return hi
+00013290: 6768 6573 7420 7665 7273 696f 6e20 6669  ghest version fi
+000132a0: 7273 740a 2020 2020 2020 2020 2020 2020  rst.            
+000132b0: 7265 7375 6c74 6469 6374 5b6b 5d20 3d20  resultdict[k] = 
+000132c0: 736f 7274 6564 2872 6573 706f 6e73 655f  sorted(response_
+000132d0: 6c69 7374 5b69 5d2c 2072 6576 6572 7365  list[i], reverse
+000132e0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+000132f0: 7265 7475 726e 2072 6573 756c 7464 6963  return resultdic
+00013300: 742c 2072 6573 706f 6e73 655f 6c69 7374  t, response_list
+00013310: 5b2d 315d 0a                             [-1].
```

### Comparing `biomero-1.7.0/biomero.egg-info/PKG-INFO` & `biomero-1.7.1/biomero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.7.0/biomero.egg-info/SOURCES.txt` & `biomero-1.7.1/biomero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/docs/Makefile` & `biomero-1.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/docs/conf.py` & `biomero-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/docs/index.rst` & `biomero-1.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/docs/make.bat` & `biomero-1.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/pyproject.toml` & `biomero-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/convert_job_array.sh` & `biomero-1.7.1/resources/convert_job_array.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/convert_zarr_to_tiff.py` & `biomero-1.7.1/resources/convert_zarr_to_tiff.py`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/job_template.sh` & `biomero-1.7.1/resources/job_template.sh`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 ##############################
 
 # Std out will get parsed into the logfile, so it is useful to log all your steps and variables
 echo "Running $jobname Job w/ $IMAGE_PATH | $SINGULARITY_IMAGE | $DATA_PATH | $SCRIPT_PATH | $DO_CONVERT | \
 	$PARAMS" 
 
 # Load singularity module if needed
-echo "Loading Singularity/Apptainer..."
-module load singularity || true
+echo "Loading Singularity/Apptainer if needed..."
+module load singularity > /dev/null 2>&1 || true
 
 # WE MOVED THIS CONVERSION LOGIC TO A SEPARATE BIOMERO FUNCTION
 # APPLYING IT HERE HAS A POSSIBILITY TO CLOG THE QUEUE AND TIMEOUT WHILE WAITING
 # SEE https://github.com/Cellular-Imaging-Amsterdam-UMC/NL-BIOMERO/issues/6
 # # Convert datatype if needed
 # echo "Preprocessing data..."
 # if $DO_CONVERT; then
```

### Comparing `biomero-1.7.0/resources/slurm-config.ini` & `biomero-1.7.1/resources/slurm-config.ini`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/Cells.tif` & `biomero-1.7.1/resources/tutorials/images/Cells.tif`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/cellexpansion.png` & `biomero-1.7.1/resources/tutorials/images/cellexpansion.png`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/gc_allow_ssh.PNG` & `biomero-1.7.1/resources/tutorials/images/gc_allow_ssh.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/nuclei_labels.png` & `biomero-1.7.1/resources/tutorials/images/nuclei_labels.png`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/webclient_init_env.PNG` & `biomero-1.7.1/resources/tutorials/images/webclient_init_env.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/webclient_init_env_done.PNG` & `biomero-1.7.1/resources/tutorials/images/webclient_init_env_done.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/webclient_run_cellpose.PNG` & `biomero-1.7.1/resources/tutorials/images/webclient_run_cellpose.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/images/webclient_run_workflow.PNG` & `biomero-1.7.1/resources/tutorials/images/webclient_run_workflow.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/tutorial_Azure_slurm.md` & `biomero-1.7.1/resources/tutorials/tutorial_Azure_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/tutorial_GoogleCloud_slurm.md` & `biomero-1.7.1/resources/tutorials/tutorial_GoogleCloud_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/tutorial_cellexpansion.md` & `biomero-1.7.1/resources/tutorials/tutorial_cellexpansion.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/tutorial_cellprofiler.md` & `biomero-1.7.1/resources/tutorials/tutorial_cellprofiler.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/resources/tutorials/tutorial_local_slurm.md` & `biomero-1.7.1/resources/tutorials/tutorial_local_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.7.0/tests/unit/test_slurm_client.py` & `biomero-1.7.1/tests/unit/test_slurm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -852,14 +852,15 @@
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_not_called()
     mock_run_commands.assert_called_once_with([
         f"rm {filename}.*",
         f"rm {logfile}",
+        f"rm slurm-{slurm_job_id}_*.out",
         f"rm -rf {data_location} {data_location}.*"
     ])
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.SlurmClient.run_commands')
@@ -883,14 +884,15 @@
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_called_once_with(logfile)
     mock_run_commands.assert_called_once_with([
         f"rm {filename}.*",
         f"rm {logfile}",
+        f"rm slurm-{slurm_job_id}_*.out",
         f"rm -rf {data_location} {data_location}.*"
     ])
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.Connection.create_session')
```


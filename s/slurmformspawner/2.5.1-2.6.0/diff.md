# Comparing `tmp/slurmformspawner-2.5.1.tar.gz` & `tmp/slurmformspawner-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmformspawner-2.5.1.tar", last modified: Tue Mar  5 15:44:50 2024, max compression
+gzip compressed data, was "slurmformspawner-2.6.0.tar", last modified: Thu Apr  4 20:19:38 2024, max compression
```

## Comparing `slurmformspawner-2.5.1.tar` & `slurmformspawner-2.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:44:50.323841 slurmformspawner-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-05 15:44:50.323841 slurmformspawner-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 15:44:50.323841 slurmformspawner-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:44:50.319841 slurmformspawner-2.5.1/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:44:50.319841 slurmformspawner-2.5.1/share/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/share/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/share/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/share/templates/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:44:50.319841 slurmformspawner-2.5.1/slurmformspawner/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/slurmformspawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12582 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/slurmformspawner/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/slurmformspawner/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/slurmformspawner/spawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-05 15:44:43.000000 slurmformspawner-2.5.1/slurmformspawner/traitlets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:44:50.323841 slurmformspawner-2.5.1/slurmformspawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-05 15:44:50.000000 slurmformspawner-2.5.1/slurmformspawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-05 15:44:50.000000 slurmformspawner-2.5.1/slurmformspawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:44:50.000000 slurmformspawner-2.5.1/slurmformspawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-05 15:44:50.000000 slurmformspawner-2.5.1/slurmformspawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 15:44:50.000000 slurmformspawner-2.5.1/slurmformspawner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:19:38.320820 slurmformspawner-2.6.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/share/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/share/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/share/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/share/templates/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/slurmformspawner/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/slurmformspawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12582 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/slurmformspawner/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/slurmformspawner/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/slurmformspawner/spawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-04 20:19:34.000000 slurmformspawner-2.6.0/slurmformspawner/traitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:19:38.324820 slurmformspawner-2.6.0/slurmformspawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-04 20:19:38.000000 slurmformspawner-2.6.0/slurmformspawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-04 20:19:38.000000 slurmformspawner-2.6.0/slurmformspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:19:38.000000 slurmformspawner-2.6.0/slurmformspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 20:19:38.000000 slurmformspawner-2.6.0/slurmformspawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 20:19:38.000000 slurmformspawner-2.6.0/slurmformspawner.egg-info/top_level.txt
```

### Comparing `slurmformspawner-2.5.1/LICENSE` & `slurmformspawner-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/PKG-INFO` & `slurmformspawner-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmformspawner
-Version: 2.5.1
+Version: 2.6.0
 Summary: slurmformspawner: JupyterHub SlurmSpawner with a dynamic spawn form
 Home-page: https://github.com/cmd-ntrf/slurmformspawner
 Author: Félix-Antoine Fortin
 Author-email: felix-antoine.fortin@calculquebec.ca
 License: MIT
 Keywords: Interactive,Web,JupyterHub
 Platform: Linux
@@ -13,27 +13,27 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: batchspawner>=0.9.0.dev0
+Requires-Dist: batchspawner>=1.3.0
 Requires-Dist: WTForms==2.3.1
 Requires-Dist: jinja2>=2.10.1
 Requires-Dist: cachetools
 
 # slurmformspawner
 JupyterHub SlurmSpawner with a dynamic spawn form
 
 ## Requirements
 
-- Python >= 3.6
-- JupyterHub >= 1.0
-- batchspawner>=0.9.0.dev0
+- Python >= 3.7
+- JupyterHub >= 4.0.0
+- batchspawner>= 1.3.0
 - cachetools
 - traitlets
 
 ## Configuration
 
 ### SlurmFormSpawner
 
@@ -45,30 +45,31 @@
 | `c.SlurmFormSpawner.ui_args` | `Dict` | Dictionary of dictionaries describing the UI options | refer to `ui_args` section |
 
 #### `ui_args`
 
 `ui_args` is a dictionary where the keys are labels that will be re-used in `SbatchForm.ui` and the values are dictionnaries describing how to launch the user interface.
 Each option dictionary can have the following keys:
 - `name` (required): string that will appear in the Spawner form
+- `url`  (optional): url user is being redirected to after spawning the single-user server (refer to `JUPYTERHUB_DEFAULT_URL` documentation)
 - `args` (optional): list of flags and options that will be appended to jupyter single-user command that should redirect to the UI.
 - `modules` (optional): list of module names that needs to be loaded to make the user interface work
 
 Here is an example of a dictionary that would configure Jupyter Notebook, a terminal and RStudio.
 ```
 c.SlurmFormSpawner.ui_args = {
     'notebook' : {
         'name': 'Jupyter Notebook'
     },
     'terminal' : {
         'name': 'Terminal',
-        'args': ['--SingleUserNotebookApp.default_url=/terminal/1']
+        'url': '/terminal/1'
     },
     'rstudio' : {
         'name': 'RStudio',
-        'args': ['--SingleUserNotebookApp.default_url=/rstudio'],
+        'url': '/rstudio',
         'modules': ['rstudio-server']
     }
 }
 ```
 
 ### SbatchForm
```

### Comparing `slurmformspawner-2.5.1/README.md` & `slurmformspawner-2.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # slurmformspawner
 JupyterHub SlurmSpawner with a dynamic spawn form
 
 ## Requirements
 
-- Python >= 3.6
-- JupyterHub >= 1.0
-- batchspawner>=0.9.0.dev0
+- Python >= 3.7
+- JupyterHub >= 4.0.0
+- batchspawner>= 1.3.0
 - cachetools
 - traitlets
 
 ## Configuration
 
 ### SlurmFormSpawner
 
@@ -21,30 +21,31 @@
 | `c.SlurmFormSpawner.ui_args` | `Dict` | Dictionary of dictionaries describing the UI options | refer to `ui_args` section |
 
 #### `ui_args`
 
 `ui_args` is a dictionary where the keys are labels that will be re-used in `SbatchForm.ui` and the values are dictionnaries describing how to launch the user interface.
 Each option dictionary can have the following keys:
 - `name` (required): string that will appear in the Spawner form
+- `url`  (optional): url user is being redirected to after spawning the single-user server (refer to `JUPYTERHUB_DEFAULT_URL` documentation)
 - `args` (optional): list of flags and options that will be appended to jupyter single-user command that should redirect to the UI.
 - `modules` (optional): list of module names that needs to be loaded to make the user interface work
 
 Here is an example of a dictionary that would configure Jupyter Notebook, a terminal and RStudio.
 ```
 c.SlurmFormSpawner.ui_args = {
     'notebook' : {
         'name': 'Jupyter Notebook'
     },
     'terminal' : {
         'name': 'Terminal',
-        'args': ['--SingleUserNotebookApp.default_url=/terminal/1']
+        'url': '/terminal/1'
     },
     'rstudio' : {
         'name': 'RStudio',
-        'args': ['--SingleUserNotebookApp.default_url=/rstudio'],
+        'url': '/rstudio',
         'modules': ['rstudio-server']
     }
 }
 ```
 
 ### SbatchForm
```

### Comparing `slurmformspawner-2.5.1/setup.py` & `slurmformspawner-2.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup_args = dict(
     name                = 'slurmformspawner',
     packages            = ['slurmformspawner'],
-    version             = "2.5.1",
+    version             = "2.6.0",
     description         = "slurmformspawner: JupyterHub SlurmSpawner with a dynamic spawn form",
     long_description    = long_description,
     long_description_content_type = 'text/markdown',
     author              = "Félix-Antoine Fortin",
     author_email        = "felix-antoine.fortin@calculquebec.ca",
     url                 = "https://github.com/cmd-ntrf/slurmformspawner",
     license             = "MIT",
@@ -26,15 +26,15 @@
         'Intended Audience :: System Administrators',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     install_requires   = [
-      'batchspawner>=0.9.0.dev0',
+      'batchspawner>=1.3.0',
       'WTForms==2.3.1',
       'jinja2>=2.10.1',
       'cachetools'
     ],
     data_files = [('share/slurmformspawner/templates', ['share/templates/submit.sh',
                                                         'share/templates/form.html',
                                                         'share/templates/error.html'])]
```

### Comparing `slurmformspawner-2.5.1/share/templates/error.html` & `slurmformspawner-2.6.0/share/templates/error.html`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/share/templates/form.html` & `slurmformspawner-2.6.0/share/templates/form.html`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/share/templates/submit.sh` & `slurmformspawner-2.6.0/share/templates/submit.sh`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/slurmformspawner/form.py` & `slurmformspawner-2.6.0/slurmformspawner/form.py`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/slurmformspawner/slurm.py` & `slurmformspawner-2.6.0/slurmformspawner/slurm.py`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/slurmformspawner/spawner.py` & `slurmformspawner-2.6.0/slurmformspawner/spawner.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         help="Disable the spawner input form"
     ).tag(config=True)
 
     ui_args = Dict(
         {
             'notebook' : {
                 'name' : 'Jupyter Notebook',
+                'url' : '/tree',
             },
             'lab' : {
                 'name' : 'JupyterLab',
-                'args' : ['--SingleUserNotebookApp.default_url=/lab']
             },
             'terminal' : {
                 'name' : 'Terminal',
-                'args' : ['--SingleUserNotebookApp.default_url=/terminals/1']
+                'url' : '/terminals/1',
             },
         },
         help="Dictionary of dictionaries describing the names and args of UI options"
     ).tag(config=True)
 
     slurm_bin_path = Unicode(
         '/opt/slurm/bin',
@@ -91,14 +91,22 @@
         pass
 
     def get_args(self):
         args = super().get_args()
         ui = self.form.data.get('ui')
         return args + self.ui_args[ui].get('args', [])
 
+    def get_env(self):
+        env = super().get_env()
+        ui = self.form.data.get('ui')
+        url = self.ui_args[ui].get('url', None)
+        if url:
+            env["JUPYTERHUB_DEFAULT_URL"] = url
+        return env
+
     @property
     def options_form(self):
         if self.slurm_api.is_online():
             if self.disable_form:
                 return None
             if self.form is not None:
                 return self.form.render()
```

### Comparing `slurmformspawner-2.5.1/slurmformspawner/traitlets.py` & `slurmformspawner-2.6.0/slurmformspawner/traitlets.py`

 * *Files identical despite different names*

### Comparing `slurmformspawner-2.5.1/slurmformspawner.egg-info/PKG-INFO` & `slurmformspawner-2.6.0/slurmformspawner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmformspawner
-Version: 2.5.1
+Version: 2.6.0
 Summary: slurmformspawner: JupyterHub SlurmSpawner with a dynamic spawn form
 Home-page: https://github.com/cmd-ntrf/slurmformspawner
 Author: Félix-Antoine Fortin
 Author-email: felix-antoine.fortin@calculquebec.ca
 License: MIT
 Keywords: Interactive,Web,JupyterHub
 Platform: Linux
@@ -13,27 +13,27 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: batchspawner>=0.9.0.dev0
+Requires-Dist: batchspawner>=1.3.0
 Requires-Dist: WTForms==2.3.1
 Requires-Dist: jinja2>=2.10.1
 Requires-Dist: cachetools
 
 # slurmformspawner
 JupyterHub SlurmSpawner with a dynamic spawn form
 
 ## Requirements
 
-- Python >= 3.6
-- JupyterHub >= 1.0
-- batchspawner>=0.9.0.dev0
+- Python >= 3.7
+- JupyterHub >= 4.0.0
+- batchspawner>= 1.3.0
 - cachetools
 - traitlets
 
 ## Configuration
 
 ### SlurmFormSpawner
 
@@ -45,30 +45,31 @@
 | `c.SlurmFormSpawner.ui_args` | `Dict` | Dictionary of dictionaries describing the UI options | refer to `ui_args` section |
 
 #### `ui_args`
 
 `ui_args` is a dictionary where the keys are labels that will be re-used in `SbatchForm.ui` and the values are dictionnaries describing how to launch the user interface.
 Each option dictionary can have the following keys:
 - `name` (required): string that will appear in the Spawner form
+- `url`  (optional): url user is being redirected to after spawning the single-user server (refer to `JUPYTERHUB_DEFAULT_URL` documentation)
 - `args` (optional): list of flags and options that will be appended to jupyter single-user command that should redirect to the UI.
 - `modules` (optional): list of module names that needs to be loaded to make the user interface work
 
 Here is an example of a dictionary that would configure Jupyter Notebook, a terminal and RStudio.
 ```
 c.SlurmFormSpawner.ui_args = {
     'notebook' : {
         'name': 'Jupyter Notebook'
     },
     'terminal' : {
         'name': 'Terminal',
-        'args': ['--SingleUserNotebookApp.default_url=/terminal/1']
+        'url': '/terminal/1'
     },
     'rstudio' : {
         'name': 'RStudio',
-        'args': ['--SingleUserNotebookApp.default_url=/rstudio'],
+        'url': '/rstudio',
         'modules': ['rstudio-server']
     }
 }
 ```
 
 ### SbatchForm
```


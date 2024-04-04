# Comparing `tmp/cybershuttle_tune-0.1.2.tar.gz` & `tmp/cybershuttle_tune-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybershuttle_tune-0.1.2.tar", max compression
+gzip compressed data, was "cybershuttle_tune-0.1.3.tar", max compression
```

## Comparing `cybershuttle_tune-0.1.2.tar` & `cybershuttle_tune-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-10-09 21:06:40.772241 cybershuttle_tune-0.1.2/LICENSE
--rw-r--r--   0        0        0      151 2023-10-11 08:07:37.750712 cybershuttle_tune-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-10-09 23:24:08.009114 cybershuttle_tune-0.1.2/cybershuttle_tune/__init__.py
--rw-r--r--   0        0        0    10943 2023-10-10 23:20:04.787568 cybershuttle_tune-0.1.2/cybershuttle_tune/airavata_operator.py
--rw-r--r--   0        0        0        0 2023-10-09 23:24:34.587631 cybershuttle_tune-0.1.2/cybershuttle_tune/cli/__init__.py
--rw-r--r--   0        0        0      165 2023-10-10 00:38:37.531093 cybershuttle_tune-0.1.2/cybershuttle_tune/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6320 2023-10-11 06:32:40.785306 cybershuttle_tune-0.1.2/cybershuttle_tune/cli/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     3995 2023-10-11 06:36:51.570528 cybershuttle_tune-0.1.2/cybershuttle_tune/cli/main.py
--rw-r--r--   0        0        0      756 2023-10-10 07:29:16.168435 cybershuttle_tune-0.1.2/cybershuttle_tune/param_types.py
--rw-r--r--   0        0        0      562 2023-10-10 07:11:04.748395 cybershuttle_tune-0.1.2/cybershuttle_tune/parser.py
--rw-r--r--   0        0        0     2593 2023-10-11 06:36:51.567286 cybershuttle_tune-0.1.2/cybershuttle_tune/sweeper.py
--rw-r--r--   0        0        0      899 2023-10-11 08:07:37.747153 cybershuttle_tune-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 cybershuttle_tune-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-09 21:06:40.772241 cybershuttle_tune-0.1.3/LICENSE
+-rw-r--r--   0        0        0      365 2023-10-11 08:23:19.790495 cybershuttle_tune-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-10-09 23:24:08.009114 cybershuttle_tune-0.1.3/cybershuttle_tune/__init__.py
+-rw-r--r--   0        0        0    12532 2024-04-01 18:02:32.862642 cybershuttle_tune-0.1.3/cybershuttle_tune/airavata_operator.py
+-rw-r--r--   0        0        0        0 2023-10-09 23:24:34.587631 cybershuttle_tune-0.1.3/cybershuttle_tune/cli/__init__.py
+-rw-r--r--   0        0        0     8085 2024-03-22 16:16:58.171901 cybershuttle_tune-0.1.3/cybershuttle_tune/cli/auth.py
+-rw-r--r--   0        0        0     8256 2024-04-01 18:29:22.276612 cybershuttle_tune-0.1.3/cybershuttle_tune/cli/main.py
+-rw-r--r--   0        0        0      878 2024-04-04 00:09:27.372873 cybershuttle_tune-0.1.3/cybershuttle_tune/param_types.py
+-rw-r--r--   0        0        0      562 2023-10-10 07:11:04.748395 cybershuttle_tune-0.1.3/cybershuttle_tune/parser.py
+-rw-r--r--   0        0        0     3792 2024-04-04 01:56:31.469344 cybershuttle_tune-0.1.3/cybershuttle_tune/sdk.py
+-rw-r--r--   0        0        0     4046 2024-04-04 01:13:34.202947 cybershuttle_tune-0.1.3/cybershuttle_tune/sweeper.py
+-rw-r--r--   0        0        0      919 2024-04-04 02:01:18.036266 cybershuttle_tune-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 cybershuttle_tune-0.1.3/PKG-INFO
```

### Comparing `cybershuttle_tune-0.1.2/LICENSE` & `cybershuttle_tune-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cybershuttle_tune-0.1.2/cybershuttle_tune/airavata_operator.py` & `cybershuttle_tune-0.1.3/cybershuttle_tune/airavata_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from airavata.model.security.ttypes import AuthzToken
 from airavata_sdk.transport.settings import GatewaySettings, ExperimentSettings
 from airavata_sdk.clients.utils.api_server_client_util import APIServerClientUtil
 from airavata_sdk.clients.utils.data_model_creation_util import DataModelCreationUtil
 from airavata_sdk.clients.sftp_file_handling_client import SFTPConnector
 import logging
 import os
+import configparser
 
 logger = logging.getLogger('airavata_sdk.clients')
 logger.setLevel(logging.INFO)
 
 class AiravataOperator:
 
     def __init__(self, configuration_file_location):
@@ -149,20 +150,22 @@
                     data_uri = data_model_util.register_input_file(file_identifier=x,
                                                                           storage_name=self.experiment_conf.STORAGE_RESOURCE_HOST,
                                                                           storageId=storage_id,
                                                                           input_file_name=x,
                                                                           uploaded_storage_path=path)
                     new_file_mapping[key] = data_uri
             experiment = data_model_util.configure_input_and_outputs(experiment, input_files=None,
-                                                                            application_name=self.experiment_conf.APPLICATION_NAME,
+                                                                            application_name=application_name,
                                                                             file_mapping=new_file_mapping)
 
             print(new_file_mapping)
         else:
             for x in os.listdir(local_input_path):
+                if x == 'inputs.ini': # Ignore command line inputs file. In future, read all input file locations from this one 
+                    continue
                 if os.path.isfile(local_input_path + '/' + x):
                     input_files.append(x)
 
             if len(input_files) > 0:
                 data_uris = []
                 for x in input_files:
                     data_uri = data_model_util.register_input_file(file_identifier=x,
@@ -177,19 +180,56 @@
                 inputs = self.api_server_client.get_application_inputs(airavata_token, app_id)
                 experiment.experimentInputs = inputs
 
         outputs = self.api_server_client.get_application_outputs(airavata_token, app_id)
 
         experiment.experimentOutputs = outputs
 
+        ## Setting up command line inputs
+
+        exp_inputs = experiment.experimentInputs
+        if not exp_inputs:
+            exp_inputs = []
+
+        execution_id = api_util.get_execution_id(application_name)
+        all_inputs = self.api_server_client.get_application_inputs(airavata_token, execution_id)
+
+        config = configparser.ConfigParser()
+        config.read(local_input_path + '/inputs.ini')
+        
+        inputs_to_replace = []
+        for input in all_inputs:
+            for input_name in list(config[application_name].keys()):
+                if input.name.lower() == input_name and input.type < 3: ## Command line input types
+                    input.value  = config[application_name][input_name]
+                    inputs_to_replace.append(input)
+
+        for input in inputs_to_replace:
+            found = False
+            for exp_in in exp_inputs:
+                if exp_in.name == input.name:
+                    exp_in.value = input.value
+                    found = True
+                    continue
+            if not found:
+                exp_inputs.append(input)
+
+        experiment.experimentInputs = exp_inputs
+
         # create experiment
         ex_id = self.api_server_client.create_experiment(airavata_token, self.gateway_conf.GATEWAY_ID, experiment)
 
         # launch experiment
         self.api_server_client.launch_experiment(airavata_token, ex_id, self.gateway_conf.GATEWAY_ID)
 
 
         return ex_id
         #if not grp_id:
 
+    def get_experiment_status(self, access_token, experiment_id):
+        airavata_token = self.get_airavata_token(access_token, self.gateway_conf.GATEWAY_ID)
+        status = self.api_server_client.get_experiment_status(airavata_token, experiment_id)
+        return status
+
+
```

### Comparing `cybershuttle_tune-0.1.2/cybershuttle_tune/param_types.py` & `cybershuttle_tune-0.1.3/cybershuttle_tune/param_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,8 +20,13 @@
 class FloatParamType:
     def __init__(self, name, values = []):
         self.values = values
         self.name = name
 
     def set_values(self, values):
         for i in values:
-            self.values.append(i)
+            self.values.append(i)
+
+class GenericParamType:
+    def __init__(self, name, values = []):
+        self.values = values
+        self.name = name
```

### Comparing `cybershuttle_tune-0.1.2/cybershuttle_tune/parser.py` & `cybershuttle_tune-0.1.3/cybershuttle_tune/parser.py`

 * *Files identical despite different names*

### Comparing `cybershuttle_tune-0.1.2/cybershuttle_tune/sweeper.py` & `cybershuttle_tune-0.1.3/cybershuttle_tune/sweeper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import cybershuttle_tune.parser as parser
 import cybershuttle_tune.airavata_operator as operator
 import itertools
 import os
+import pandas as pd
+from airavata.model.status.ttypes import ExperimentState
 
 def generate_inputs(job_name, template_dir, parameter_values, working_dir):
 
     template_files = [f for f in os.listdir(template_dir) if not os.path.isdir(f)]
 
     all_variable_values = []
     param_grid = get_grid(parameter_values)
@@ -28,36 +30,76 @@
             content = parser.apply_values(
                 file_path=os.path.join(template_dir, template_file),
                 variable_values=cur_variable_values)
 
             with open(os.path.join(input_dir, template_file), "w") as text_file:
                 text_file.write(content)
 
+    return all_variable_values
+
 def sweep_params(access_token, job_name, application_name,
-                 computation_resource_name, working_dir, config_file_location):
+                 computation_resource_name, working_dir, config_file_location, all_variable_values):
 
     job_input_path = os.path.join(working_dir, job_name)
 
     sub_dirs = os.listdir(job_input_path)
 
+    csv_data = {
+        'index': [],
+        'exp_id': []
+    }
     for sub_dir in sub_dirs:
         local_input_path = os.path.join(job_input_path, sub_dir)
         airavata_op = operator.AiravataOperator(config_file_location)
 
         ex_id = airavata_op.submit_experiment(access_token=access_token,
                                       experiment_name=job_name + "_" + sub_dir,
                                       application_name=application_name,
                                       computation_resource_name=computation_resource_name,
                                       local_input_path=local_input_path)
 
-        with open(os.path.join(job_input_path, "summary.txt"), 'a+') as f:
-            f.write(sub_dir + ":" + ex_id + "\n")
+        variables = all_variable_values[int(sub_dir)]
+
+        csv_data['index'].append(sub_dir)
+        csv_data['exp_id'].append(ex_id)
+
+        variable_names = variables.keys()
+        for variable_name in variable_names:
+            if not (variable_name in csv_data):
+                csv_data[variable_name] = []
+
+            csv_data[variable_name].append(variables[variable_name])
+        #with open(os.path.join(job_input_path, "summary.txt"), 'a+') as f:
+        #    f.write(sub_dir + ":" + ex_id + "\n")
         print("Airavata experiment " + ex_id + " was launched for sweep config " + sub_dir)
 
+    df = pd.DataFrame(csv_data)
+    # Writing the DataFrame to a CSV file
+    df.to_csv(os.path.join(job_input_path, "summary.csv"), index=False, header=True)
+
+    csv_data['job_name'] = job_name
+    csv_data['working_dir'] = working_dir
+    return csv_data
+
+def get_sweep_status(access_token, job_name, working_dir, config_file_location):
+    airavata_operator = operator.AiravataOperator(config_file_location)
+    job_input_path = os.path.join(working_dir, job_name)
+    summary_file = os.path.join(job_input_path, "summary.csv")
+
+    df = pd.read_csv(summary_file)
+
+    exp_ids = column_data = df['exp_id']
+    indexes = df['index']
+
+    states = []
+    for exp_id in exp_ids:
+        status = airavata_operator.get_experiment_status(access_token, exp_id)
+        states.append([exp_id,  ExperimentState._VALUES_TO_NAMES[status.state]])
 
+    return states, indexes
 
 def get_grid(parameter_values):
     vals_arr = []
     for param_val in parameter_values:
         vals_arr.append(param_val.values)
 
     return list(itertools.product(*vals_arr))
```

### Comparing `cybershuttle_tune-0.1.2/pyproject.toml` & `cybershuttle_tune-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybershuttle-tune"
-version = "0.1.2"
+version = "0.1.3"
 description = "Parameter Tunning Library for CyberShuttle"
 authors = [
     "Dimuthu Wannipurage <dimuthuw@gatech.edu>",
 ]
 maintainers = [
     "Apache Airavata Developers <dev@apache.airavata.org>",
 ]
@@ -25,11 +25,12 @@
 airavata-python-sdk = "^1.1.7"
 thrift-connector = "^0.24"
 thrift = "^0.16.0"
 requests-oauthlib = "^1.3.1"
 pyjwt = "^2.8.0"
 paramiko = "^3.3.1"
 scp = "^0.14.5"
+tabulate = "^0.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cybershuttle_tune-0.1.2/PKG-INFO` & `cybershuttle_tune-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybershuttle-tune
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parameter Tunning Library for CyberShuttle
 Home-page: https://github.com/cyber-shuttle/cybershuttle-tune
 License: Apache-2.0
 Keywords: CyberShuttle,Prameter Tunning,Parameter Sweeping
 Author: Dimuthu Wannipurage
 Author-email: dimuthuw@gatech.edu
 Maintainer: Apache Airavata Developers
@@ -18,19 +18,32 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: paramiko (>=3.3.1,<4.0.0)
 Requires-Dist: pick (==2.2.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: scp (>=0.14.5,<0.15.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: thrift (>=0.16.0,<0.17.0)
 Requires-Dist: thrift-connector (>=0.24,<0.25)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
+Parameter Sweeping Library and Command line Interface for CyberShuttle Project
+
+### How to use
+```
+pip install cybershuttle-tune
+```
+
+Refer to examples for further usage information
+
+### Build instructions
+```
 python3.10 -m venv venv  ## Use python 3.10.6 or higher
 source venv/bin/activate
 pip install poetry
 poetry shell
 
 poetry install
 poetry publish --build
+```
```


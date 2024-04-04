# Comparing `tmp/cluster_experiment_utils-0.0.7.tar.gz` & `tmp/cluster_experiment_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_experiment_utils-0.0.7.tar", last modified: Fri Mar  8 19:46:38 2024, max compression
+gzip compressed data, was "cluster_experiment_utils-0.0.9.tar", last modified: Fri Mar  8 20:47:18 2024, max compression
```

## Comparing `cluster_experiment_utils-0.0.7.tar` & `cluster_experiment_utils-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:38.801876 cluster_experiment_utils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-08 19:46:38.801876 cluster_experiment_utils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:38.797876 cluster_experiment_utils-0.0.7/cluster_experiment_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:38.797876 cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/base_cluster_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/lsf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/slurm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/flowcept_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:38.801876 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-08 19:46:38.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-08 19:46:38.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 19:46:38.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-08 19:46:38.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-08 19:46:38.000000 cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 19:46:38.801876 cluster_experiment_utils-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:38.801876 cluster_experiment_utils-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-08 19:46:32.000000 cluster_experiment_utils-0.0.7/tests/test_the_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/cluster_experiment_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/base_cluster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/lsf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/slurm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/flowcept_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-08 20:47:18.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-08 20:47:18.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:47:18.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-08 20:47:18.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-08 20:47:18.000000 cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:18.592771 cluster_experiment_utils-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-08 20:47:14.000000 cluster_experiment_utils-0.0.9/tests/test_the_utils.py
```

### Comparing `cluster_experiment_utils-0.0.7/PKG-INFO` & `cluster_experiment_utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiment_utils
-Version: 0.0.7
+Version: 0.0.9
 Summary: Cluster Experiment Utils
 Home-page: https://github.com/renan-souza/experiment_utils
 Author: Renan Souza
 Author-email: contact@renansouza.org
 License: MIT
 Keywords: experiment-utils,experiment_utils
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/base_cluster_utils.py` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/base_cluster_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,35 +20,38 @@
 
 class Runner:
     JSRUN = "jsrun"
     SRUN = "srun"
 
 
 class BaseClusterUtils(object, metaclass=ABCMeta):
-
     _subclasses = {}
+
     @classmethod
     def register_subclass(cls, subclass_name, subclass):
         cls._subclasses[subclass_name] = subclass
 
     _instance = None
     RESOURCE_MANAGER = get_resource_manager_type()
-    
+
     @staticmethod
     def get_instance():
         if BaseClusterUtils._instance is not None:
             return BaseClusterUtils._instance
         else:
             if BaseClusterUtils.RESOURCE_MANAGER == ResourceManager.SLURM:
-                BaseClusterUtils._instance = BaseClusterUtils._subclasses.get(ResourceManager.SLURM)()
+                BaseClusterUtils._instance = BaseClusterUtils._subclasses.get(
+                    ResourceManager.SLURM
+                )()
             elif BaseClusterUtils.RESOURCE_MANAGER == ResourceManager.LSF:
-                BaseClusterUtils._instance = BaseClusterUtils._subclasses.get(ResourceManager.LSF)()
+                BaseClusterUtils._instance = BaseClusterUtils._subclasses.get(
+                    ResourceManager.LSF
+                )()
         return BaseClusterUtils._instance
 
-    
     def kill_job(self, job_id):
         raise NotImplementedError()
 
     def get_this_job_id(self):
         raise NotImplementedError()
 
     def kill_this_job(self):
@@ -63,15 +66,15 @@
         raise NotImplementedError()
 
     def get_resource_usage_info(self, job_dir) -> Dict:
         raise NotImplementedError()
 
     def kill_all_running_job_steps():
         raise NotImplementedError()
-    
+
     def run_job(
         self,
         cmd,
         stdout=None,
         stderr=None,
         node_count=None,
         process_count=None,
@@ -96,15 +99,15 @@
         self,
         cmd,
         proj_id,
         queue_name=None,
         job_name=None,
         wall_time: str = None,  # format: HH:MM
         stdout=None,
-        stderr=None,        
+        stderr=None,
         node_count=None,
         process_count=None,
         processes_per_node=None,
         custom_attributes=None,
         cpu_cores_per_process=None,
         gpu_cores_per_process=None,
     ):
@@ -140,15 +143,15 @@
         custom_attributes=None,
         cpu_cores_per_process=None,
         gpu_cores_per_process=None,
         job_type="batch",  # or "runner"
     ) -> Union[psij.Job, subprocess.Popen]:
         job = BaseClusterUtils._build_job(
             cmd=cmd,
-            proj_id=proj_id,            
+            proj_id=proj_id,
             queue_name=queue_name,
             job_name=job_name,
             wall_time=wall_time,
             stdout=stdout,
             stderr=stderr,
             node_count=node_count,
             process_count=process_count,
@@ -183,45 +186,44 @@
             text=True,
         )
         return process
 
     @staticmethod
     def _build_job(
         cmd,
-        proj_id=None,        
+        proj_id=None,
         queue_name=None,
         job_name=None,
         wall_time: str = None,  # format: HH:MM
         stdout=None,
         stderr=None,
         node_count=None,
         process_count=None,
         processes_per_node=None,
         custom_attributes=None,
         cpu_cores_per_process=None,
         gpu_cores_per_process=None,
     ) -> psij.Job:
-        
         # shell_script_file = os.path.join(str(uuid4())+".sh")
         # print(f"Written the following command into the file {shell_script_file}\n{cmd}")
         # with open(shell_script_file, "w+") as f:
         #     f.write(cmd)
 
         cmd_split = cmd.split()
-        
+
         job = psij.Job()
         spec = psij.JobSpec()
         spec.executable = cmd_split[0]
         spec.arguments = cmd_split[1:]
         print(spec.executable, spec.arguments)
-        # cmds = cmd.split()        
+        # cmds = cmd.split()
         # spec.executable = " ".join(cmds)
         # print(spec.executable)
-        #spec.arguments = cmds[1:]
-        
+        # spec.arguments = cmds[1:]
+
         spec.name = job_name
         spec.attributes.project_name = proj_id
         spec.attributes.queue_name = queue_name
         spec.attributes.custom_attributes = custom_attributes
         if custom_attributes:
             print(custom_attributes)
         if wall_time:
@@ -257,15 +259,15 @@
         t0,
         t1,
         t_c_f,
         t_c_i,
         varying_param_key,
         wf_result,
         with_flowcept,
-        flowcept_settings
+        flowcept_settings,
     ):
         out_job = {
             "my_job_id": my_job_id,
             "job_dir": job_dir,
             "rep_dir": rep_dir,
             "job_id": self.get_this_job_id(),
             "job_hosts": job_hosts,
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/lsf_utils.py` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/lsf_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,42 +17,49 @@
         print("Killing LSF job")
         run_cmd_check_output(f"bkill {job_id}")
         print("Kill command submitted!")
 
     def kill_all_running_job_steps(self):
         print("Killing all jsrun jobs")
         run_cmd_check_output(f"jskill all")
-    
+
     def run_job(
         self,
         cmd,
         stdout=None,
         stderr=None,
         node_count=None,
         process_count=None,
         processes_per_node=None,
         cpu_cores_per_process=None,
         gpus_per_job=None,
     ):
         jsrun_command = [
-            'jsrun',
-            '--nrs', str(node_count) if node_count else '1',
-            '--tasks_per_rs', str(process_count) if process_count else '1',
-            '--tasks_per_host', str(processes_per_node) if processes_per_node else '1',
-            '--cpu_per_rs', str(cpu_cores_per_process) if cpu_cores_per_process else '1',
-            '--gpu_per_rs', str(gpu_cores_per_process) if gpu_cores_per_process else '0',
-            '--stdout', stdout,
-            '--stderr', stderr,
+            "jsrun",
+            "--nrs",
+            str(node_count) if node_count else "1",
+            "--tasks_per_rs",
+            str(process_count) if process_count else "1",
+            "--tasks_per_host",
+            str(processes_per_node) if processes_per_node else "1",
+            "--cpu_per_rs",
+            str(cpu_cores_per_process) if cpu_cores_per_process else "1",
+            "--gpu_per_rs",
+            str(gpu_cores_per_process) if gpu_cores_per_process else "0",
+            "--stdout",
+            stdout,
+            "--stderr",
+            stderr,
         ]
-    
+
         jsrun_command += cmd
         print(jsrun_command)
         process = subprocess.Popen(jsrun_command)
         return process
-    
+
     def get_job_hosts(self):
         hosts = os.getenv("LSB_HOSTS")
         if hosts is not None:
             lsb_hosts = hosts.split()
         else:
             host_file = os.getenv("LSB_DJOB_HOSTFILE")
             with open(host_file) as f:
@@ -104,8 +111,9 @@
             "lsf_avg_mem_mb": avg_mem,
             "from_host": from_host,
         }
 
     def __init__(self):
         super().__init__()
 
+
 BaseClusterUtils.register_subclass("lsf", LsfUtils)
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils/cluster_utils/slurm_utils.py` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils/cluster_utils/slurm_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,81 +13,82 @@
     def kill_job(self, job_id=None):
         if job_id is None:
             job_id = self.get_this_job_id()
         print(f"Killing job {job_id}")
         run_cmd_check_output(f"scancel {job_id}")
         print("Kill command submitted!")
         printed_sleep(2)
-        
-
 
     def kill_all_running_job_steps(self):
-        this_job = self.get_this_job_id()        
+        this_job = self.get_this_job_id()
         try:
             # Run the sacct command and capture the output
-            result = subprocess.run(['sacct', '-j', str(this_job)], capture_output=True, text=True, check=True)
+            result = subprocess.run(
+                ["sacct", "-j", str(this_job)],
+                capture_output=True,
+                text=True,
+                check=True,
+            )
             # Split the output into lines and iterate through them
-            for line in result.stdout.strip().split('\n'):
+            for line in result.stdout.strip().split("\n"):
                 # Split each line into columns
                 columns = line.split()
                 # Check if the line corresponds to a RUNNING job
                 if len(columns):
                     step_job_id = columns[0]
                     status = columns[4]
-                    if "." in step_job_id and status == 'RUNNING':                                  
+                    if "." in step_job_id and status == "RUNNING":
                         split_val = step_job_id.split(".")
                         if split_val[1].isdigit():
                             self.kill_job(step_job_id)
-                            
-    
+
         except subprocess.CalledProcessError as e:
             print(f"Error running sacct: {e}")
-    
 
     def run_job(
         self,
         cmd,
         stdout=None,
         stderr=None,
         node_count=None,
         process_count=None,
         processes_per_node=None,
         cpu_cores_per_process=None,
         gpus_per_job=None,
     ):
-        srun_command = ['srun', '--exclusive']
+        srun_command = ["srun", "--exclusive"]
 
         if node_count is not None:
-            srun_command.extend(['--nodes', str(node_count)])
-    
+            srun_command.extend(["--nodes", str(node_count)])
+
         if process_count is not None:
-            srun_command.extend(['--ntasks', str(process_count)])
-    
+            srun_command.extend(["--ntasks", str(process_count)])
+
         if processes_per_node is not None:
-            srun_command.extend(['--ntasks-per-node', str(processes_per_node)])
-    
+            srun_command.extend(["--ntasks-per-node", str(processes_per_node)])
+
         if cpu_cores_per_process is not None:
-            srun_command.extend(['--cpus-per-task', str(cpu_cores_per_process)])
-    
+            srun_command.extend(["--cpus-per-task", str(cpu_cores_per_process)])
+
         if gpus_per_job is not None:
-            srun_command.extend(['--gpus', str(gpus_per_job)])
-    
+            srun_command.extend(["--gpus", str(gpus_per_job)])
+
         if stdout is not None:
-            srun_command.extend(['--output', stdout])
-    
+            srun_command.extend(["--output", stdout])
+
         if stderr is not None:
-            srun_command.extend(['--error', stderr])
+            srun_command.extend(["--error", stderr])
 
         cmd = cmd.strip()
         srun_command_str = " ".join(srun_command)
         srun_command_str += " /bin/bash -c '" + cmd + "'"
-        #srun_command.extend(cmd.split())
+        # srun_command.extend(cmd.split())
         print(srun_command_str)
         process = subprocess.Popen(srun_command_str, shell=True)
-        
+
         return process
 
     def get_job_hosts(self):
         """
         Gets a mapping of job hosts and number of available cores per host
         :return:
         """
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils/flowcept_utils.py` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils/flowcept_utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -92,26 +92,26 @@
         run_cmd(f"{mongo_start_cmd} &")
     else:
         run_cmd(f"ssh {db_host} {mongo_start_cmd} & ")
     printed_sleep(5)
     print("Mongo UP!")
 
 
-
 def start_redis(db_host, redis_start_cmd):
     print("Starting Redis")
     run_cmd(f"ssh {db_host} {redis_start_cmd} &")
     printed_sleep(2)
     print("Done starting Redis.")
 
 
 def test_data_and_persist(rep_dir, wf_result, job_output):
     from flowcept import DBAPI
     from flowcept import WorkflowObject
     from flowcept import TaskQueryAPI
+
     api = TaskQueryAPI()
 
     wf_id = wf_result.get("workflow_id")
     docs = api.query(filter={"workflow_id": wf_id})
 
     if len(docs):
         print("Great! Found docs with the workflow_id in the tasks collection.")
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils/utils.py` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/PKG-INFO` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiment_utils
-Version: 0.0.7
+Version: 0.0.9
 Summary: Cluster Experiment Utils
 Home-page: https://github.com/renan-souza/experiment_utils
 Author: Renan Souza
 Author-email: contact@renansouza.org
 License: MIT
 Keywords: experiment-utils,experiment_utils
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cluster_experiment_utils-0.0.7/cluster_experiment_utils.egg-info/SOURCES.txt` & `cluster_experiment_utils-0.0.9/cluster_experiment_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiment_utils-0.0.7/setup.py` & `cluster_experiment_utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `cluster_experiment_utils-0.0.7/tests/test_the_utils.py` & `cluster_experiment_utils-0.0.9/tests/test_the_utils.py`

 * *Files identical despite different names*


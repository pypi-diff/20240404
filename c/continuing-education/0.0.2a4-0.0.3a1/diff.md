# Comparing `tmp/continuing_education-0.0.2a4.tar.gz` & `tmp/continuing_education-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuing_education-0.0.2a4.tar", last modified: Thu Mar 28 17:07:03 2024, max compression
+gzip compressed data, was "continuing_education-0.0.3a1.tar", last modified: Thu Apr  4 00:17:58 2024, max compression
```

## Comparing `continuing_education-0.0.2a4.tar` & `continuing_education-0.0.3a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-03-28 17:07:03.108461 continuing_education-0.0.2a4/
--rw-rw-r--   0 stevemadere   (502) staff       (20)    11357 2024-03-20 14:52:11.000000 continuing_education-0.0.2a4/LICENSE
--rw-r--r--   0 stevemadere   (502) staff       (20)    10527 2024-03-28 17:07:03.107837 continuing_education-0.0.2a4/PKG-INFO
--rw-rw-r--   0 stevemadere   (502) staff       (20)     9574 2024-03-26 15:22:29.000000 continuing_education-0.0.2a4/README.md
--rw-rw-r--   0 stevemadere   (502) staff       (20)     1001 2024-03-28 17:06:10.000000 continuing_education-0.0.2a4/pyproject.toml
--rw-rw-r--   0 stevemadere   (502) staff       (20)       38 2024-03-28 17:07:03.108538 continuing_education-0.0.2a4/setup.cfg
--rw-rw-r--   0 stevemadere   (502) staff       (20)     1309 2024-03-28 17:06:13.000000 continuing_education-0.0.2a4/setup.py
-drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-03-28 17:07:03.086801 continuing_education-0.0.2a4/src/
-drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-03-28 17:07:03.090810 continuing_education-0.0.2a4/src/continuing_education/
--rw-rw-r--   0 stevemadere   (502) staff       (20)      397 2024-03-22 22:44:09.000000 continuing_education-0.0.2a4/src/continuing_education/__init__.py
--rw-rw-r--   0 stevemadere   (502) staff       (20)     9275 2024-03-22 17:50:53.000000 continuing_education-0.0.2a4/src/continuing_education/checkpoint_manager.py
--rw-rw-r--   0 stevemadere   (502) staff       (20)    14328 2024-03-28 16:55:08.000000 continuing_education-0.0.2a4/src/continuing_education/checkpoint_registry.py
--rw-rw-r--   0 stevemadere   (502) staff       (20)    24862 2024-03-26 18:31:57.000000 continuing_education-0.0.2a4/src/continuing_education/continuing_trainer.py
-drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-03-28 17:07:03.107217 continuing_education-0.0.2a4/src/continuing_education.egg-info/
--rw-r--r--   0 stevemadere   (502) staff       (20)    10527 2024-03-28 17:07:03.000000 continuing_education-0.0.2a4/src/continuing_education.egg-info/PKG-INFO
--rw-rw-r--   0 stevemadere   (502) staff       (20)      538 2024-03-28 17:07:03.000000 continuing_education-0.0.2a4/src/continuing_education.egg-info/SOURCES.txt
--rw-rw-r--   0 stevemadere   (502) staff       (20)        1 2024-03-28 17:07:03.000000 continuing_education-0.0.2a4/src/continuing_education.egg-info/dependency_links.txt
--rw-rw-r--   0 stevemadere   (502) staff       (20)       62 2024-03-28 17:07:03.000000 continuing_education-0.0.2a4/src/continuing_education.egg-info/requires.txt
--rw-rw-r--   0 stevemadere   (502) staff       (20)       21 2024-03-28 17:07:03.000000 continuing_education-0.0.2a4/src/continuing_education.egg-info/top_level.txt
-drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-03-28 17:07:03.106780 continuing_education-0.0.2a4/tests/
--rw-rw-r--   0 stevemadere   (502) staff       (20)     5958 2024-03-26 19:20:40.000000 continuing_education-0.0.2a4/tests/test_checkpoint_registry.py
--rw-rw-r--   0 stevemadere   (502) staff       (20)     9874 2024-03-28 16:56:27.000000 continuing_education-0.0.2a4/tests/test_remote_checkpoint_synchronizer.py
+drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-04-04 00:17:58.524719 continuing_education-0.0.3a1/
+-rw-rw-r--   0 stevemadere   (502) staff       (20)    11357 2024-03-20 14:52:11.000000 continuing_education-0.0.3a1/LICENSE
+-rw-r--r--   0 stevemadere   (502) staff       (20)    10527 2024-04-04 00:17:58.524101 continuing_education-0.0.3a1/PKG-INFO
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     9574 2024-03-28 21:17:52.000000 continuing_education-0.0.3a1/README.md
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     1001 2024-04-04 00:15:59.000000 continuing_education-0.0.3a1/pyproject.toml
+-rw-rw-r--   0 stevemadere   (502) staff       (20)       38 2024-04-04 00:17:58.524814 continuing_education-0.0.3a1/setup.cfg
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     1309 2024-04-04 00:16:06.000000 continuing_education-0.0.3a1/setup.py
+drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-04-04 00:17:58.514624 continuing_education-0.0.3a1/src/
+drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-04-04 00:17:58.518740 continuing_education-0.0.3a1/src/continuing_education/
+-rw-rw-r--   0 stevemadere   (502) staff       (20)      397 2024-03-28 21:17:52.000000 continuing_education-0.0.3a1/src/continuing_education/__init__.py
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     9532 2024-04-03 21:56:23.000000 continuing_education-0.0.3a1/src/continuing_education/checkpoint_manager.py
+-rw-rw-r--   0 stevemadere   (502) staff       (20)    14328 2024-03-28 21:17:52.000000 continuing_education-0.0.3a1/src/continuing_education/checkpoint_registry.py
+-rw-rw-r--   0 stevemadere   (502) staff       (20)    24988 2024-04-03 21:56:23.000000 continuing_education-0.0.3a1/src/continuing_education/continuing_trainer.py
+drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-04-04 00:17:58.523494 continuing_education-0.0.3a1/src/continuing_education.egg-info/
+-rw-r--r--   0 stevemadere   (502) staff       (20)    10527 2024-04-04 00:17:58.000000 continuing_education-0.0.3a1/src/continuing_education.egg-info/PKG-INFO
+-rw-rw-r--   0 stevemadere   (502) staff       (20)      538 2024-04-04 00:17:58.000000 continuing_education-0.0.3a1/src/continuing_education.egg-info/SOURCES.txt
+-rw-rw-r--   0 stevemadere   (502) staff       (20)        1 2024-04-04 00:17:58.000000 continuing_education-0.0.3a1/src/continuing_education.egg-info/dependency_links.txt
+-rw-rw-r--   0 stevemadere   (502) staff       (20)       62 2024-04-04 00:17:58.000000 continuing_education-0.0.3a1/src/continuing_education.egg-info/requires.txt
+-rw-rw-r--   0 stevemadere   (502) staff       (20)       21 2024-04-04 00:17:58.000000 continuing_education-0.0.3a1/src/continuing_education.egg-info/top_level.txt
+drwxrwxr-x   0 stevemadere   (502) staff       (20)        0 2024-04-04 00:17:58.522433 continuing_education-0.0.3a1/tests/
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     5958 2024-04-03 21:27:47.000000 continuing_education-0.0.3a1/tests/test_checkpoint_registry.py
+-rw-rw-r--   0 stevemadere   (502) staff       (20)     9874 2024-04-03 21:27:47.000000 continuing_education-0.0.3a1/tests/test_remote_checkpoint_synchronizer.py
```

### Comparing `continuing_education-0.0.2a4/LICENSE` & `continuing_education-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `continuing_education-0.0.2a4/PKG-INFO` & `continuing_education-0.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuing_education
-Version: 0.0.2a4
+Version: 0.0.3a1
 Summary: System to ease incremental training of a Huggingface transformer model from a large S3-based dataset
 Author-email: Steve Madere <steve@stevemadere.com>
 Project-URL: Homepage, https://github.com/stevemadere/continuing-education
 Project-URL: Issues, https://github.com/stevemadere/continuing-education/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `continuing_education-0.0.2a4/README.md` & `continuing_education-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `continuing_education-0.0.2a4/pyproject.toml` & `continuing_education-0.0.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "continuing_education"
-version = "0.0.2a4"
+version = "0.0.3a1"
 authors = [
   { name="Steve Madere", email="steve@stevemadere.com" },
 ]
 description = "System to ease incremental training of a Huggingface transformer model from a large S3-based dataset"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `continuing_education-0.0.2a4/setup.py` & `continuing_education-0.0.3a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='s3datasets',
     python_requires='>=3.6',
     description = "System to ease incremental training of a Huggingface transformer model from a large S3-based dataset",
     long_description="This Python module provides tools to enhance Huggingface Trainer to make it feasible to train transformers on very large remote datasets that are impractical to just download en-masse for every training session or to complete all of the training on a single server instance.  It makes it practical to use cloud providers like vast.ai or salad.ai as a fine-tuning platform for large language models.",
-    version='0.0.2a4',
+    version='0.0.3a1',
     package_dir={'': 'src'},  # This tells setuptools where to find packages
     packages=find_packages(where='src'),
     install_requires=[
         's3datasets',
         'dataclasses',
         'typing; python_version<"3.5"',
         'peft'
```

### Comparing `continuing_education-0.0.2a4/src/continuing_education/checkpoint_manager.py` & `continuing_education-0.0.3a1/src/continuing_education/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
       save_on_stop: bool
       steps_seen: int
       checkpoint_registry: Union[CheckpointRegistry,None]
       starting_checkpoint_info: Union[CheckpointInfo,None]
       current_dataset_segment_number: int
       logger: logging.Logger
       trainer_state_at_save: Union[dict,None]
+      max_steps_passed: bool
 
       def __init__(self,
                    trainer: Trainer,
                    checkpoint_registry : Union[CheckpointRegistry,None] = None,
                    dataset_generator: Union[TextDS2TokensGenerator,None] = None,
                    starting_checkpoint_info: Union[CheckpointInfo,None] = None,
                    stop_after_steps: Union[int,None] = None,
@@ -54,14 +55,15 @@
           self.stop_after_steps = stop_after_steps
           self.save_on_stop = save_on_stop
           self.logger = logger
           self.steps_seen = 0
           self._last_save_was_at_step = None
           self.trainer_state_at_save = None
           self.current_dataset_segment_number = self.starting_checkpoint_info.segment_number if (self.starting_checkpoint_info and self.starting_checkpoint_info.segment_number) else 1
+          self.max_steps_passed = False
           self.trainer.add_callback(self)
 
       def on_train_begin(self,
                          args: TrainingArguments,
                          state: TrainerState, control: TrainerControl, **kwargs ):
           if args or state or control or kwargs: # silence unused var warnings
               pass
@@ -76,14 +78,17 @@
               else:
                   self.logger.warn(f"checkpoint {checkpoint} has no dataset cursor")
           if self.dataset_generator:
               self.logger.info(f"initial cursor is segment {self.current_dataset_segment_number}, {self.dataset_generator.get_cursor().to_dict()}")
           else:
               self.logger.debug(f"CheckpointManager is unaware of a dataset_generator")
 
+          if state.global_step >= args.max_steps:
+              self.max_steps_passed = True
+
       def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs ):
           if args or state or kwargs: # suppress unused param warnings
               pass
           self.logger.debug(f"about to do local step {self.steps_seen+1} and dataset cursor is segment {self.current_dataset_segment_number}, {self.dataset_generator.get_cursor().to_dict().__repr__() if self.dataset_generator else 'not defined'}")
           # Why the heck do I have to do this?  It's insane.  This should be the default behavior of Trainer anyway.
           # Instead, if it runs out of training data, it raises an error
           if self.dataset_generator and self.dataset_generator.exhausted:
@@ -99,14 +104,17 @@
               pass
           self.steps_seen += 1
           self.logger.debug(f"just did local step {self.steps_seen} and dataset cursor is segment {self.current_dataset_segment_number}, {self.dataset_generator.get_cursor().to_dict().__repr__() if self.dataset_generator else 'not defined'}")
           if self.stop_after_steps and self.steps_seen >= self.stop_after_steps:
               self.logger.debug(f"Terminating training loop after {self.stop_after_steps} steps")
               control.should_training_stop = True
 
+          if state.global_step >= args.max_steps:
+              self.max_steps_passed = True
+
           # Why the heck do I have to do this?  It's insane.  This should be the default behavior of Trainer anyway.
           # Instead, if it runs out of training data, it raises an error
           if self.dataset_generator and self.dataset_generator.exhausted:
               control.should_training_stop = True
 
           if control.should_training_stop and self.save_on_stop:
               self.logger.debug("Trying to trigger a save_on_stop")
```

### Comparing `continuing_education-0.0.2a4/src/continuing_education/checkpoint_registry.py` & `continuing_education-0.0.3a1/src/continuing_education/checkpoint_registry.py`

 * *Files identical despite different names*

### Comparing `continuing_education-0.0.2a4/src/continuing_education/continuing_trainer.py` & `continuing_education-0.0.3a1/src/continuing_education/continuing_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,17 @@
 
         logger.info(f'generator cursor after training is segment {self.dataset_segment_number()},  {self.train_tokens_generator.get_cursor().to_dict()}')
         logger.info(f'Trained for {self.checkpoint_manager.steps_seen} steps')
         logger.debug(f'post training trainer state {self.trainer.state.__repr__()}')
         # Ensure that any ongoing checkpoint uploads complete before returning
         self.checkpoint_registry.finish_up()
 
+    def reached_max_steps(self) -> bool:
+        return self.checkpoint_manager and self.checkpoint_manager.max_steps_passed
+
     def dataset_segment_number(self):
         if 'checkpoint_manager' in self.__dict__ and self.checkpoint_manager:
             return self.checkpoint_manager.current_dataset_segment_number
         elif self.starting_checkpoint_info and self.starting_checkpoint_info.segment_number:
             return self.starting_checkpoint_info.segment_number
         else:
             return 1
```

### Comparing `continuing_education-0.0.2a4/src/continuing_education.egg-info/PKG-INFO` & `continuing_education-0.0.3a1/src/continuing_education.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuing_education
-Version: 0.0.2a4
+Version: 0.0.3a1
 Summary: System to ease incremental training of a Huggingface transformer model from a large S3-based dataset
 Author-email: Steve Madere <steve@stevemadere.com>
 Project-URL: Homepage, https://github.com/stevemadere/continuing-education
 Project-URL: Issues, https://github.com/stevemadere/continuing-education/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `continuing_education-0.0.2a4/src/continuing_education.egg-info/SOURCES.txt` & `continuing_education-0.0.3a1/src/continuing_education.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `continuing_education-0.0.2a4/tests/test_checkpoint_registry.py` & `continuing_education-0.0.3a1/tests/test_checkpoint_registry.py`

 * *Files identical despite different names*

### Comparing `continuing_education-0.0.2a4/tests/test_remote_checkpoint_synchronizer.py` & `continuing_education-0.0.3a1/tests/test_remote_checkpoint_synchronizer.py`

 * *Files identical despite different names*


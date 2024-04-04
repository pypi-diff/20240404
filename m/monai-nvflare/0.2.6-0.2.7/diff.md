# Comparing `tmp/monai_nvflare-0.2.6-py3-none-any.whl.zip` & `tmp/monai_nvflare-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15080 bytes, number of entries: 11
+Zip file size: 15048 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      842 b- defN 24-Jan-19 02:23 monai_nvflare/__init__.py
--rw-rw-r--  2.0 unx    10507 b- defN 24-Jan-19 02:23 monai_nvflare/client_algo_executor.py
+-rw-rw-r--  2.0 unx    10507 b- defN 24-Feb-20 18:07 monai_nvflare/client_algo_executor.py
 -rw-rw-r--  2.0 unx     7394 b- defN 24-Jan-19 02:23 monai_nvflare/client_algo_statistics.py
--rw-rw-r--  2.0 unx     4800 b- defN 24-Jan-19 02:23 monai_nvflare/monai_bundle_persistor.py
+-rw-rw-r--  2.0 unx     4800 b- defN 24-Jan-30 21:34 monai_nvflare/monai_bundle_persistor.py
 -rw-rw-r--  2.0 unx     2145 b- defN 24-Jan-19 02:23 monai_nvflare/monai_data_stats_persistor.py
--rw-rw-r--  2.0 unx    10922 b- defN 24-Jan-19 02:23 monai_nvflare/nvflare_stats_handler.py
+-rw-rw-r--  2.0 unx    10869 b- defN 24-Feb-20 18:07 monai_nvflare/nvflare_stats_handler.py
 -rw-rw-r--  2.0 unx      747 b- defN 24-Jan-19 02:23 monai_nvflare/utils.py
--rw-rw-r--  2.0 unx     2406 b- defN 24-Jan-23 21:54 monai_nvflare-0.2.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-23 21:54 monai_nvflare-0.2.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 24-Jan-23 21:54 monai_nvflare-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      964 b- defN 24-Jan-23 21:54 monai_nvflare-0.2.6.dist-info/RECORD
-11 files, 40833 bytes uncompressed, 13432 bytes compressed:  67.1%
+-rw-rw-r--  2.0 unx     2385 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      964 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/RECORD
+11 files, 40759 bytes uncompressed, 13400 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: monai_nvflare/nvflare_stats_handler.py
 Comment: 
 
 Filename: monai_nvflare/utils.py
 Comment: 
 
-Filename: monai_nvflare-0.2.6.dist-info/METADATA
+Filename: monai_nvflare-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: monai_nvflare-0.2.6.dist-info/WHEEL
+Filename: monai_nvflare-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: monai_nvflare-0.2.6.dist-info/top_level.txt
+Filename: monai_nvflare-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_nvflare-0.2.6.dist-info/RECORD
+Filename: monai_nvflare-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai_nvflare/nvflare_stats_handler.py

```diff
@@ -167,15 +167,14 @@
         Args:
             engine: Ignite Engine, it can be a trainer, validator or evaluator.
 
         """
         current_epoch = self.global_epoch_transform(engine.state.epoch)
         summary_dict = engine.state.metrics
         for name, value in summary_dict.items():
-            print(f"\n\t{name}", type(value), value)
             self._send_stats(engine, name, value, AnalyticsDataType.SCALAR, current_epoch)
 
         if self.state_attributes is not None:
             for attr in self.state_attributes:
                 self._send_stats(
                     engine, attr, getattr(engine.state, attr, None), self.state_attributes_type, current_epoch
                 )
```

## Comparing `monai_nvflare-0.2.6.dist-info/METADATA` & `monai_nvflare-0.2.7.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: monai-nvflare
-Version: 0.2.6
+Version: 0.2.7
 Summary: MONAI NVIDIA FLARE integration
 Home-page: https://github.com/NVIDIA/NVFlare
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Requires-Dist: monai >=1.3.0
-Requires-Dist: nvflare ~=2.4.0rc6
+Requires-Dist: nvflare ~=2.4.1rc3
 
 # MONAI Integration
 
 ## Objective
 Integration with [MONAI](https://monai.io/)'s federated learning capabilities.
 
 Add `ClientAlgoExecutor` class to allow using MONAI's `ClientAlgo` class in federated scenarios.
 
 ### Goals:
 
 Allow the use of bundles from the MONAI [model zoo](https://github.com/Project-MONAI/model-zoo) or custom configurations with NVFlare.
 
-### Non-goals:
-
-n/a
-
 ## Background
 MONAI allows the definition of AI models using the "[bundle](https://docs.monai.io/en/latest/bundle.html)" concept. 
 It allows for easy experimentation and sharing of models that have been developed using MONAI.
 Using the bundle configurations, we can use MONAI's `MonaiAlgo` (the implementation of `ClientAlgo`) to execute a bundle model in a federated scenario using NVFlare.
 
 ![Federated Learning Module in MONAI (https://docs.monai.io/en/stable/modules.html#federated-learning)](https://docs.monai.io/en/stable/_images/federated.svg)
```

## Comparing `monai_nvflare-0.2.6.dist-info/RECORD` & `monai_nvflare-0.2.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 monai_nvflare/__init__.py,sha256=VdMkO_e5cO4c08OESZP_Ari647QryLIT1B2fhjCr_7E,842
 monai_nvflare/client_algo_executor.py,sha256=uiCCqCscPVsZRc2GQHggWQ-KRoh-j2WPobS-sGYq9dE,10507
 monai_nvflare/client_algo_statistics.py,sha256=tzkDATxL965tj537iwwm9e6kf1Ia9m3gCPbhdqJZfzk,7394
 monai_nvflare/monai_bundle_persistor.py,sha256=kwuYzi9umV27ON9QmKOJFW1fv2mMu_fPt9IEN9xSfuM,4800
 monai_nvflare/monai_data_stats_persistor.py,sha256=YgbMUIfUc_O5tn7y45Mqi2AEJVk6FfK8oK2OAwaCRxM,2145
-monai_nvflare/nvflare_stats_handler.py,sha256=02D0_ez2q5PofNHVCBZYhERJsdtJlky5RN9MSY42IP0,10922
+monai_nvflare/nvflare_stats_handler.py,sha256=CmYQt9zwEn7KWQoqSX-O2WvMwqZDVqKlgEAwoxTNIiU,10869
 monai_nvflare/utils.py,sha256=Nilco4ll_vsNozM3fL4KrIVFcwqWEndGgoNppF5fF70,747
-monai_nvflare-0.2.6.dist-info/METADATA,sha256=gT3dCmu85cqMhfZ-XIWkV3Lez4tHid_7C-S28N4jXYU,2406
-monai_nvflare-0.2.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-monai_nvflare-0.2.6.dist-info/top_level.txt,sha256=VDiu-tAUOUqzkR4VFFKlXWg8mx6WbUj6rIa8mrZgZWI,14
-monai_nvflare-0.2.6.dist-info/RECORD,,
+monai_nvflare-0.2.7.dist-info/METADATA,sha256=uk1VVGYtZF6l6bW_u31ox_Zh4LtJSX-g4qR-3LeiDYM,2385
+monai_nvflare-0.2.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+monai_nvflare-0.2.7.dist-info/top_level.txt,sha256=VDiu-tAUOUqzkR4VFFKlXWg8mx6WbUj6rIa8mrZgZWI,14
+monai_nvflare-0.2.7.dist-info/RECORD,,
```


# Comparing `tmp/smartboiler-0.0.3.0.0.5.8.9.tar.gz` & `tmp/smartboiler-0.0.3.0.0.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.5.8.9.tar", last modified: Tue Apr  2 20:16:27 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.5.9.2.tar", last modified: Thu Apr  4 08:33:24 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.5.8.9.tar` & `smartboiler-0.0.3.0.0.5.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 20:16:25.000000 smartboiler-0.0.3.0.0.5.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.192939 smartboiler-0.0.3.0.0.5.8.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-04 08:33:23.000000 smartboiler-0.0.3.0.0.5.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.406498 smartboiler-0.0.3.0.0.5.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-04 08:33:19.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:33:24.410498 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 08:33:24.000000 smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/PKG-INFO` & `smartboiler-0.0.3.0.0.5.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.8.9
+Version: 0.0.3.0.0.5.9.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/README.md` & `smartboiler-0.0.3.0.0.5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/setup.py` & `smartboiler-0.0.3.0.0.5.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.5.8.9',  # Required
+    version='0.0.3.0.0.5.9.2',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,20 +75,20 @@
         # self.Hass = remote.API('localhost', 'smart_boiler01')
         self.dataHandler = dataHandler
         self.boiler = boiler
         self.forecast = forecast
 
         if load_model:
             print("loading model")
+            self.forecast.build_model()
             self.forecast.load_model()
         else:
             print("training model")
-            forecast.train_model()
             self.forecast.build_model()
-            self.forecast.fit_model()
+            forecast.train_model()
 
         self.last_model_training = datetime.now()
 
         # #self.EventChecker = EventChecker()
         # #self.TimeHandler = TimeHandler()
         # #self.Boiler = Boiler(capacity=boiler_capacity,
         # #                    wattage=boiler_wattage, set_tmp=boiler_set_tmp)
@@ -108,15 +108,14 @@
 
     def _check_data(self):
         """Retrain model if the last data update is older than 7 days."""
         if self.last_model_training - datetime.now() > timedelta(days=7):
             print("actualizing data")
 
             self.forecast.train_model()
-            self.forecast.fit_model()
             self.last_model_training = datetime.now()
 
     def _learning(self):
         """After one week of only measuring the data starts heating based on historical data.
 
         Returns:
             [boolean]: [True if in learing]
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,16 @@
         freq = 1
         freq_hour = f"{freq}H"
 
         df.index = pd.to_datetime(df.index)
 
         df.loc[:, "weekday"] = df.index.weekday
         df.loc[:, "hour"] = df.index.hour
-        df.loc[:, "minute"] = df.index.minute
+        # df.loc[:, "minute"] = df.index.minute
+        df.loc[:, "minute"] = 0
 
         # delete rows with weekday nan
         df = df.dropna(subset=["weekday"])
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].fillna(0)
 
         # fill negative values with 0
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].clip(lower=0)
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,51 @@
             (self.df_train_norm.shape[0] * 0.1 - self.lookback) // self.batch_size
         )
         # This is how many steps to draw from `train_gen`
         # in order to see the whole train set:
         self.train_steps = int(
             (self.df_train_norm.shape[0] * 0.9 - self.lookback) // self.batch_size
         )
+        
+        callbacks = [
+            EarlyStopping(
+                monitor="loss",
+                min_delta=0,
+                patience=10,
+                verbose=2,
+                mode="auto",
+                restore_best_weights=True,
+            ),
+
+            ModelCheckpoint(verbose=1, filepath=self.model_path, save_best_only=True, save_weights_only=True)
+            ]
+
+        print("Start training")
+        history = self.model.fit(
+            self.train_gen,
+            steps_per_epoch=self.train_steps,
+            epochs=100,
+            shuffle=False,
+            validation_data=self.valid_gen,
+            validation_steps=self.val_steps,
+            callbacks=callbacks,
+            verbose=2,
+        )
+        
+        self.model.save(self.model_path)
+        print("End training")
 
 
     def load_model(
         self,
         left_time_interval=datetime.now() - timedelta(days=4),
         right_time_interval=datetime.now(),
     ):
         
         self.scaler = load(open(self.scaler_path, 'rb'))
-        self.build_model()
         self.model.load_weights(self.model_path)
 
 
 
     def generator(
         self,
         dataframe,
@@ -184,43 +211,16 @@
         model.add(Dense(1))
 
         self.model = model
         self.model.compile(loss="mae", optimizer="adam")
         return model
 
     def fit_model(self):
+        pass
 
-        callbacks = [
-            EarlyStopping(
-                monitor="loss",
-                min_delta=0,
-                patience=10,
-                verbose=2,
-                mode="auto",
-                restore_best_weights=True,
-            ),
-
-            ModelCheckpoint(verbose=1, filepath=self.model_path, save_best_only=True, save_weights_only=True)
-            ]
-
-        # history = model.fit(train_gen, epochs=50, batch_size=72, validation_data=valid_gen, verbose=2, shuffle=False, use_multiprocessing=True)
-        print("Start training")
-        history = self.model.fit(
-            self.train_gen,
-            steps_per_epoch=self.train_steps,
-            epochs=100,
-            shuffle=False,
-            validation_data=self.valid_gen,
-            validation_steps=self.val_steps,
-            callbacks=callbacks,
-            verbose=2,
-        )
-        
-        self.model.save(self.model_path)
-        print("End training")
         
         # self.model.save(self.model_path)
 
 
         
         
 
@@ -324,14 +324,15 @@
         right_time_interval = right_time_interval.replace(minute=0)
 
 
         df_all = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
+        
         num_targets = len(self.predicted_columns)
         len_columns = len(df_all.columns)
         
         df_all = df_all.dropna()
         df_all = df_all.reset_index(drop=True)
         
         forecast_future = pd.DataFrame()
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.8.9
+Version: 0.0.3.0.0.5.9.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.5.9.2/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


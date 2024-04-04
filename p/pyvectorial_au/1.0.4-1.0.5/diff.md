# Comparing `tmp/pyvectorial_au-1.0.4.tar.gz` & `tmp/pyvectorial_au-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvectorial_au-1.0.4.tar", max compression
+gzip compressed data, was "pyvectorial_au-1.0.5.tar", max compression
```

## Comparing `pyvectorial_au-1.0.4.tar` & `pyvectorial_au-1.0.5.tar`

### file list

```diff
@@ -1,49 +1,54 @@
--rw-r--r--   0        0        0      436 2024-03-22 18:12:40.303262 pyvectorial_au-1.0.4/README.md
--rw-r--r--   0        0        0      715 2024-03-22 20:41:25.987435 pyvectorial_au-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       80 2024-03-22 18:01:09.228542 pyvectorial_au-1.0.4/src/pyvectorial_au/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.242931 pyvectorial_au-1.0.4/src/pyvectorial_au/aperture/__init__.py
--rw-r--r--   0        0        0     4682 2024-03-22 18:00:27.662102 pyvectorial_au-1.0.4/src/pyvectorial_au/aperture/aperture.py
--rw-r--r--   0        0        0        0 2024-03-22 18:01:36.159316 pyvectorial_au-1.0.4/src/pyvectorial_au/backends/__init__.py
--rw-r--r--   0        0        0     7842 2024-03-22 18:46:16.222966 pyvectorial_au-1.0.4/src/pyvectorial_au/backends/fortran_version.py
--rw-r--r--   0        0        0     4873 2024-03-22 18:00:27.600096 pyvectorial_au-1.0.4/src/pyvectorial_au/backends/python_version.py
--rw-r--r--   0        0        0    10625 2024-03-22 18:46:07.530169 pyvectorial_au-1.0.4/src/pyvectorial_au/backends/rust_version.py
--rwxr-xr-x   0        0        0    86032 2024-03-22 17:57:51.244433 pyvectorial_au-1.0.4/src/pyvectorial_au/bin/fvm_m1
--rwxr-xr-x   0        0        0   451936 2024-03-22 17:57:51.246817 pyvectorial_au-1.0.4/src/pyvectorial_au/bin/rust_vect_m1
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.246954 pyvectorial_au-1.0.4/src/pyvectorial_au/db/__init.py__
--rw-r--r--   0        0        0     1542 2024-03-22 17:57:51.247096 pyvectorial_au-1.0.4/src/pyvectorial_au/db/vectorial_model_cache.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.247200 pyvectorial_au-1.0.4/src/pyvectorial_au/encoding/__init__.py
--rw-r--r--   0        0        0      973 2024-03-22 18:00:27.594302 pyvectorial_au-1.0.4/src/pyvectorial_au/encoding/encoding_and_hashing.py
--rw-r--r--   0        0        0        0 2024-03-22 18:21:43.426017 pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/__init__.py
--rw-r--r--   0        0        0      520 2024-03-22 18:00:27.653797 pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/haser_matplotlib.py
--rw-r--r--   0        0        0     9260 2024-03-22 18:00:27.636165 pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/vm_matplotlib.py
--rw-r--r--   0        0        0     8320 2024-03-22 18:00:27.658064 pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/vm_plotly.py
--rw-r--r--   0        0        0        0 2024-03-22 18:22:14.473305 pyvectorial_au-1.0.4/src/pyvectorial_au/haser/__init__.py
--rw-r--r--   0        0        0     6836 2024-03-22 18:00:27.581642 pyvectorial_au-1.0.4/src/pyvectorial_au/haser/haser_fits.py
--rw-r--r--   0        0        0     1629 2024-03-22 18:00:27.576817 pyvectorial_au-1.0.4/src/pyvectorial_au/haser/haser_params.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.248731 pyvectorial_au-1.0.4/src/pyvectorial_au/model_input/__init__.py
--rw-r--r--   0        0        0     6903 2024-03-22 17:57:51.248961 pyvectorial_au-1.0.4/src/pyvectorial_au/model_input/vectorial_model_config.py
--rw-r--r--   0        0        0      958 2024-03-22 18:00:27.671500 pyvectorial_au-1.0.4/src/pyvectorial_au/model_input/vectorial_model_config_reader.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.249209 pyvectorial_au-1.0.4/src/pyvectorial_au/model_output/__init__.py
--rw-r--r--   0        0        0    13879 2024-03-22 18:00:27.626791 pyvectorial_au-1.0.4/src/pyvectorial_au/model_output/vectorial_model_calculation.py
--rw-r--r--   0        0        0     4612 2024-03-22 17:57:51.249556 pyvectorial_au-1.0.4/src/pyvectorial_au/model_output/vectorial_model_result.py
--rw-r--r--   0        0        0     2288 2024-03-22 18:00:27.649176 pyvectorial_au-1.0.4/src/pyvectorial_au/model_output/vectorial_model_runner.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.249759 pyvectorial_au-1.0.4/src/pyvectorial_au/post_model_processing/__init__.py
--rw-r--r--   0        0        0     1247 2024-03-22 18:00:27.590216 pyvectorial_au-1.0.4/src/pyvectorial_au/post_model_processing/column_density_abel.py
--rw-r--r--   0        0        0     1411 2024-03-22 18:00:27.585791 pyvectorial_au-1.0.4/src/pyvectorial_au/post_model_processing/interpolation.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.250101 pyvectorial_au-1.0.4/src/pyvectorial_au/pre_model_processing/__init__.py
--rw-r--r--   0        0        0     3086 2024-03-22 18:00:27.565024 pyvectorial_au-1.0.4/src/pyvectorial_au/pre_model_processing/input_transforms.py
--rw-r--r--   0        0        0     3699 2024-03-22 18:00:27.572092 pyvectorial_au-1.0.4/src/pyvectorial_au/pre_model_processing/timedependentproduction.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:51.250419 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/__init__.py
--rw-r--r--   0        0        0   215308 2024-03-22 17:57:51.250986 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/fort.16
--rw-r--r--   0        0        0  1119685 2024-03-22 17:57:51.253752 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/rust_out.txt
--rw-r--r--   0        0        0      627 2024-03-22 17:57:51.254116 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run.yaml
--rw-r--r--   0        0        0     1002 2024-03-22 17:57:51.254214 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_binned.yaml
--rw-r--r--   0        0        0      837 2024-03-22 17:57:51.254299 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_gaussian.yaml
--rw-r--r--   0        0        0      840 2024-03-22 17:57:51.254384 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_sine.yaml
--rw-r--r--   0        0        0      847 2024-03-22 17:57:51.254467 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_square_pulse.yaml
--rw-r--r--   0        0        0     3186 2024-03-22 18:00:27.679903 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_fortran_version.py
--rw-r--r--   0        0        0     2697 2024-03-22 18:00:27.689390 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_input_transforms.py
--rw-r--r--   0        0        0     2775 2024-03-22 18:00:27.684234 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_rust_version.py
--rw-r--r--   0        0        0     5100 2024-03-22 18:00:27.694283 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_timedependentproduction.py
--rw-r--r--   0        0        0     1644 2024-03-22 18:00:27.675589 pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_vectorial_model_config_read.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 pyvectorial_au-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-03-22 18:12:40.303262 pyvectorial_au-1.0.5/README.md
+-rw-r--r--   0        0        0      715 2024-04-04 15:17:54.952326 pyvectorial_au-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-03-22 18:01:09.228542 pyvectorial_au-1.0.5/src/pyvectorial_au/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.242931 pyvectorial_au-1.0.5/src/pyvectorial_au/aperture/__init__.py
+-rw-r--r--   0        0        0     4682 2024-03-22 18:00:27.662102 pyvectorial_au-1.0.5/src/pyvectorial_au/aperture/aperture.py
+-rw-r--r--   0        0        0        0 2024-03-22 18:01:36.159316 pyvectorial_au-1.0.5/src/pyvectorial_au/backends/__init__.py
+-rw-r--r--   0        0        0     7842 2024-03-22 18:46:16.222966 pyvectorial_au-1.0.5/src/pyvectorial_au/backends/fortran_version.py
+-rw-r--r--   0        0        0     4873 2024-03-22 18:00:27.600096 pyvectorial_au-1.0.5/src/pyvectorial_au/backends/python_version.py
+-rw-r--r--   0        0        0    10625 2024-03-22 18:46:07.530169 pyvectorial_au-1.0.5/src/pyvectorial_au/backends/rust_version.py
+-rwxr-xr-x   0        0        0    86032 2024-03-22 17:57:51.244433 pyvectorial_au-1.0.5/src/pyvectorial_au/bin/fvm_m1
+-rwxr-xr-x   0        0        0   451936 2024-03-22 17:57:51.246817 pyvectorial_au-1.0.5/src/pyvectorial_au/bin/rust_vect_m1
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.246954 pyvectorial_au-1.0.5/src/pyvectorial_au/db/__init.py__
+-rw-r--r--   0        0        0      743 2024-04-03 16:03:19.207149 pyvectorial_au-1.0.5/src/pyvectorial_au/db/cache_init.py
+-rw-r--r--   0        0        0     2955 2024-04-03 16:25:03.992237 pyvectorial_au-1.0.5/src/pyvectorial_au/db/cache_io.py
+-rw-r--r--   0        0        0     1845 2024-04-03 16:37:19.687771 pyvectorial_au-1.0.5/src/pyvectorial_au/db/vectorial_model_cache.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.247200 pyvectorial_au-1.0.5/src/pyvectorial_au/encoding/__init__.py
+-rw-r--r--   0        0        0      973 2024-03-22 18:00:27.594302 pyvectorial_au-1.0.5/src/pyvectorial_au/encoding/encoding_and_hashing.py
+-rw-r--r--   0        0        0        0 2024-03-22 18:21:43.426017 pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/__init__.py
+-rw-r--r--   0        0        0      520 2024-03-22 18:00:27.653797 pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/haser_matplotlib.py
+-rw-r--r--   0        0        0     9472 2024-04-04 14:56:01.906301 pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/vm_matplotlib.py
+-rw-r--r--   0        0        0     8452 2024-04-04 14:50:45.056901 pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/vm_plotly.py
+-rw-r--r--   0        0        0        0 2024-03-22 18:22:14.473305 pyvectorial_au-1.0.5/src/pyvectorial_au/haser/__init__.py
+-rw-r--r--   0        0        0     6836 2024-03-22 18:00:27.581642 pyvectorial_au-1.0.5/src/pyvectorial_au/haser/haser_fits.py
+-rw-r--r--   0        0        0     1629 2024-03-22 18:00:27.576817 pyvectorial_au-1.0.5/src/pyvectorial_au/haser/haser_params.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.248731 pyvectorial_au-1.0.5/src/pyvectorial_au/model_input/__init__.py
+-rw-r--r--   0        0        0     6903 2024-03-22 17:57:51.248961 pyvectorial_au-1.0.5/src/pyvectorial_au/model_input/vectorial_model_config.py
+-rw-r--r--   0        0        0      958 2024-03-22 18:00:27.671500 pyvectorial_au-1.0.5/src/pyvectorial_au/model_input/vectorial_model_config_reader.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.249209 pyvectorial_au-1.0.5/src/pyvectorial_au/model_output/__init__.py
+-rw-r--r--   0        0        0     1516 2024-04-04 14:47:21.595275 pyvectorial_au-1.0.5/src/pyvectorial_au/model_output/fragment_sputter.py
+-rw-r--r--   0        0        0     4764 2024-04-04 14:32:30.753392 pyvectorial_au-1.0.5/src/pyvectorial_au/model_output/vectorial_model_calculation.py
+-rw-r--r--   0        0        0     1431 2024-04-04 14:48:31.501822 pyvectorial_au-1.0.5/src/pyvectorial_au/model_output/vectorial_model_result.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.249209 pyvectorial_au-1.0.5/src/pyvectorial_au/model_running/__init__.py
+-rw-r--r--   0        0        0     6779 2024-04-04 14:27:50.125780 pyvectorial_au-1.0.5/src/pyvectorial_au/model_running/vectorial_model_runner.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.249759 pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/__init__.py
+-rw-r--r--   0        0        0     1247 2024-03-22 18:00:27.590216 pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/column_density_abel.py
+-rw-r--r--   0        0        0     1986 2024-04-04 14:52:16.711488 pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/fragment_sputter_transform.py
+-rw-r--r--   0        0        0     1411 2024-03-22 18:00:27.585791 pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/interpolation.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.250101 pyvectorial_au-1.0.5/src/pyvectorial_au/pre_model_processing/__init__.py
+-rw-r--r--   0        0        0     3086 2024-03-22 18:00:27.565024 pyvectorial_au-1.0.5/src/pyvectorial_au/pre_model_processing/input_transforms.py
+-rw-r--r--   0        0        0     3699 2024-03-22 18:00:27.572092 pyvectorial_au-1.0.5/src/pyvectorial_au/pre_model_processing/timedependentproduction.py
+-rw-r--r--   0        0        0        0 2024-03-22 17:57:51.250419 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/__init__.py
+-rw-r--r--   0        0        0   215308 2024-03-22 17:57:51.250986 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/fort.16
+-rw-r--r--   0        0        0  1119685 2024-03-22 17:57:51.253752 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/rust_out.txt
+-rw-r--r--   0        0        0      627 2024-03-22 17:57:51.254116 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run.yaml
+-rw-r--r--   0        0        0     1002 2024-03-22 17:57:51.254214 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_binned.yaml
+-rw-r--r--   0        0        0      837 2024-03-22 17:57:51.254299 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_gaussian.yaml
+-rw-r--r--   0        0        0      840 2024-03-22 17:57:51.254384 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_sine.yaml
+-rw-r--r--   0        0        0      847 2024-03-22 17:57:51.254467 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_square_pulse.yaml
+-rw-r--r--   0        0        0     3186 2024-03-22 18:00:27.679903 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_fortran_version.py
+-rw-r--r--   0        0        0     2697 2024-03-22 18:00:27.689390 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_input_transforms.py
+-rw-r--r--   0        0        0     2775 2024-03-22 18:00:27.684234 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_rust_version.py
+-rw-r--r--   0        0        0     5100 2024-03-22 18:00:27.694283 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_timedependentproduction.py
+-rw-r--r--   0        0        0     1644 2024-03-22 18:00:27.675589 pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_vectorial_model_config_read.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 pyvectorial_au-1.0.5/PKG-INFO
```

### Comparing `pyvectorial_au-1.0.4/pyproject.toml` & `pyvectorial_au-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvectorial_au"
-version = "1.0.4"
+version = "1.0.5"
 description = "Utilities for running, saving, and interfacing with cometary vectorial models, like the one included in sbpy"
 authors = ["Shawn Oset <szo0032@auburn.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
```

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/aperture/aperture.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/aperture/aperture.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/backends/fortran_version.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/backends/fortran_version.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/backends/python_version.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/backends/python_version.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/backends/rust_version.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/backends/rust_version.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/bin/fvm_m1` & `pyvectorial_au-1.0.5/src/pyvectorial_au/bin/fvm_m1`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/bin/rust_vect_m1` & `pyvectorial_au-1.0.5/src/pyvectorial_au/bin/rust_vect_m1`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/db/vectorial_model_cache.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/db/vectorial_model_cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,20 @@
     Mapped,
     Session,
     mapped_column,
     scoped_session,
     sessionmaker,
 )
 
-# globals - there has to be a better way to do this
-vm_cache_engine: Optional[Engine] = None
-vm_cache_session = None
+"""
+From the sqlalchemy docs:
+    When using an Engine with multiple Python processes,
+    such as when using os.fork or Python multiprocessing,
+    it’s important that the engine is initialized per process.
+"""
 
 
 class VMCachedBase(DeclarativeBase):
     pass
 
 
 class VMCached(VMCachedBase):
@@ -25,29 +28,39 @@
     vmc_hash: Mapped[str] = mapped_column(primary_key=True)
     vmr_b64_enc_zip: Mapped[bytes] = mapped_column(nullable=False)
     execution_time_s: Mapped[float] = mapped_column(nullable=False)
     vectorial_model_backend: Mapped[str] = mapped_column(nullable=False)
     vectorial_model_version: Mapped[str] = mapped_column(nullable=False)
 
 
-def initialize_vectorial_model_cache(vectorial_model_cache_dir: pathlib.Path) -> None:
-    global vm_cache_engine, vm_cache_session
-
-    if vm_cache_engine is not None or vm_cache_session is not None:
-        return
-
-    full_db_path = vectorial_model_cache_dir / pathlib.Path("vmcache.sqlite3")
-    vm_cache_engine = create_engine(f"sqlite:///{full_db_path}", poolclass=NullPool)
-
-    VMCachedBase.metadata.create_all(bind=vm_cache_engine)
-
-    session_factory = sessionmaker(vm_cache_engine)
-    vm_cache_session = scoped_session(session_factory)
-
-
-def get_vm_cache_db_session() -> Optional[Session]:
-    global vm_cache_engine, vm_cache_session
-
-    if vm_cache_session:
-        return vm_cache_session()
-    else:
-        return None
+def get_vectorial_model_cache_engine(
+    vectorial_model_cache_path: pathlib.Path,
+) -> Engine:
+    """
+    Returns an engine to the db based on the given path
+    """
+
+    vm_cache_engine = create_engine(
+        f"sqlite:///{vectorial_model_cache_path}", poolclass=NullPool
+    )
+
+    return vm_cache_engine
+
+
+def get_vectorial_model_cache_session(
+    vectorial_model_cache_path: pathlib.Path,
+    cache_engine: Optional[Engine] = None,
+) -> Optional[Session]:
+    """
+    Returns a db session based on the given Engine, but if none was given we construct
+    an engine with the given path.
+    If an engine is specified, the path is ignored.
+    """
+
+    if not cache_engine:
+        cache_engine = get_vectorial_model_cache_engine(
+            vectorial_model_cache_path=vectorial_model_cache_path,
+        )
+
+    session_factory = sessionmaker(cache_engine)
+    cache_session = scoped_session(session_factory)
+    return cache_session()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/encoding/encoding_and_hashing.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/encoding/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/haser_matplotlib.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/haser_matplotlib.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/vm_matplotlib.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/vm_matplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import astropy.units as u
 import scipy.interpolate
 
 import matplotlib.pyplot as plt
 import matplotlib.cm as cmx
 from matplotlib.colors import Normalize
 
-from pyvectorial_au.model_output.vectorial_model_result import (
-    VectorialModelResult,
-    FragmentSputterPolar,
+from pyvectorial_au.model_output.vectorial_model_result import VectorialModelResult
+from pyvectorial_au.model_output.fragment_sputter import (
     FragmentSputterSpherical,
-    fragment_sputter_to_cartesian,
+    FragmentSputterPolar,
+)
+from pyvectorial_au.post_model_processing.fragment_sputter_transform import (
     mirror_fragment_sputter,
+    fragment_sputter_to_cartesian,
 )
 
 
 """
     Functions for using matplotlib to plot various data contained in VectorialModelResults
 """
 
@@ -247,37 +249,37 @@
     within_r=1000 * u.km,  # type: ignore
     mirrored: bool = False,
     show_outflow_axis: bool = True,
     **kwargs
 ) -> None:
     fragment_sputter = vmr.fragment_sputter
 
-    if mirrored:
-        fragment_sputter = mirror_fragment_sputter(fragment_sputter)
-
     if isinstance(fragment_sputter, FragmentSputterPolar) or isinstance(
         fragment_sputter, FragmentSputterSpherical
     ):
         fragment_sputter = fragment_sputter_to_cartesian(fragment_sputter)
 
-    xs = fragment_sputter.xs.to(dist_units)
-    ys = fragment_sputter.ys.to(dist_units)
-    zs = fragment_sputter.fragment_density.to(sputter_units)
+    if mirrored:
+        fragment_sputter = mirror_fragment_sputter(fragment_sputter)
+
+    xs = fragment_sputter.xs.to(dist_units)  # type: ignore
+    ys = fragment_sputter.ys.to(dist_units)  # type: ignore
+    zs = fragment_sputter.fragment_density.to(sputter_units)  # type: ignore
 
     within_limit = np.sqrt(xs**2 + ys**2) < within_r
 
     xs = xs[within_limit]
     ys = ys[within_limit]
     zs = zs[within_limit]
 
     colors_map = "viridis"
     cm = plt.get_cmap(colors_map)
     cNorm = Normalize(vmin=np.min(zs.value), vmax=np.max(zs.value))
     scalarMap = cmx.ScalarMappable(norm=cNorm, cmap=cm)
 
     # highlight the outflow axis, along positive y
     if show_outflow_axis:
-        origin = [0, 0, 0] * dist_units
-        outflow_max = [0, np.max(ys.to_value(dist_units)), 0] * dist_units
+        origin = [0, 0, 0] * dist_units  # type: ignore
+        outflow_max = [0, np.max(ys.to_value(dist_units)), 0] * dist_units  # type: ignore
         ax.plot(origin, outflow_max, color=myblue, lw=2, label="outflow axis")
 
     ax.scatter(xs, ys, zs, c=kwargs.get("color", scalarMap.to_rgba(zs.value)))
```

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/graphing/vm_plotly.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/graphing/vm_plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import copy
 import astropy.units as u
 import scipy.interpolate
 import plotly.graph_objects as go
 from typing import Tuple
 from typing import Optional
 
-from pyvectorial_au.model_output.vectorial_model_result import (
-    VectorialModelResult,
-    FragmentSputterPolar,
+from pyvectorial_au.model_output.vectorial_model_result import VectorialModelResult
+from pyvectorial_au.model_output.fragment_sputter import (
     FragmentSputterSpherical,
-    fragment_sputter_to_cartesian,
+    FragmentSputterPolar,
+)
+from pyvectorial_au.post_model_processing.fragment_sputter_transform import (
     mirror_fragment_sputter,
+    fragment_sputter_to_cartesian,
 )
 
 
 """
     Functions for using plotly to plot various data contained in VectorialModelResults
 """
```

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/haser/haser_fits.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/haser/haser_fits.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/haser/haser_params.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/haser/haser_params.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/model_input/vectorial_model_config.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/model_input/vectorial_model_config.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/model_input/vectorial_model_config_reader.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/model_input/vectorial_model_config_reader.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/post_model_processing/column_density_abel.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/column_density_abel.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/post_model_processing/interpolation.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/post_model_processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/pre_model_processing/input_transforms.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/pre_model_processing/input_transforms.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/pre_model_processing/timedependentproduction.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/pre_model_processing/timedependentproduction.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/fort.16` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/fort.16`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/rust_out.txt` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/rust_out.txt`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run.yaml` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run.yaml`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_binned.yaml` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_binned.yaml`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_gaussian.yaml` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_gaussian.yaml`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_sine.yaml` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_sine.yaml`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/input/single_run_square_pulse.yaml` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/input/single_run_square_pulse.yaml`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_fortran_version.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_fortran_version.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_input_transforms.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_input_transforms.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_rust_version.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_rust_version.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_timedependentproduction.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_timedependentproduction.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/src/pyvectorial_au/tests/test_vectorial_model_config_read.py` & `pyvectorial_au-1.0.5/src/pyvectorial_au/tests/test_vectorial_model_config_read.py`

 * *Files identical despite different names*

### Comparing `pyvectorial_au-1.0.4/PKG-INFO` & `pyvectorial_au-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvectorial_au
-Version: 1.0.4
+Version: 1.0.5
 Summary: Utilities for running, saving, and interfacing with cometary vectorial models, like the one included in sbpy
 License: MIT
 Author: Shawn Oset
 Author-email: szo0032@auburn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/Stackinator-3.0.tar.gz` & `tmp/Stackinator-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/stackinator/stackinator/dist/tmphn0ja_mu/Stackinator-3.0.tar", last modified: Tue Oct  3 06:42:37 2023, max compression
+gzip compressed data, was "/home/runner/work/stackinator/stackinator/dist/tmp0t3ilkzk/Stackinator-4.0.tar", last modified: Thu Apr  4 16:04:11 2024, max compression
```

## Comparing `Stackinator-3.0.tar` & `Stackinator-4.0.tar`

### file list

```diff
@@ -1,48 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-03 06:42:37.000000 Stackinator-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-03 06:42:21.000000 Stackinator-3.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/etc/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3531 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/etc/add-compiler-links.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/etc/bwrap-mutable-root.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/etc/Make.inc
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/schema/environments.json
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/schema/compilers.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/schema/cache.json
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/schema/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/repo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/repo/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/repo/packages/cray-mpich/
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/repo/packages/cray-mpich/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/repo/repo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/stackinator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/Makefile.environments
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/environments.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/compilers.llvm.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/Make.user
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/stack-debug.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/Makefile.compilers
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/compilers.bootstrap.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/repos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/Makefile.generate-config
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/templates/compilers.gcc.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17546 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-10-03 06:42:21.000000 Stackinator-3.0/stackinator/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-03 06:42:21.000000 Stackinator-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-03 06:42:37.000000 Stackinator-3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-03 06:42:37.000000 Stackinator-3.0/Stackinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-03 06:42:21.000000 Stackinator-3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-03 06:42:21.000000 Stackinator-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 06:42:37.000000 Stackinator-3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      350 2023-10-03 06:42:21.000000 Stackinator-3.0/bin/stack-config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      350 2024-04-04 16:03:57.000000 Stackinator-4.0/bin/stack-config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 16:04:11.000000 Stackinator-4.0/Stackinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 16:03:57.000000 Stackinator-4.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/stackinator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/stackinator/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/schema/cache.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/schema/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/schema/environments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/schema/compilers.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/stackinator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/stack-debug.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/repos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/compilers.llvm.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/Makefile.environments
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/Makefile.compilers
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/compilers.bootstrap.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/Make.user
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/compilers.gcc.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/environments.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/templates/Makefile.generate-config
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/spack_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:04:11.000000 Stackinator-4.0/stackinator/etc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/etc/bwrap-mutable-root.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/etc/Make.inc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/etc/add-compiler-links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-04 16:03:57.000000 Stackinator-4.0/stackinator/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-04 16:04:11.000000 Stackinator-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-04 16:03:57.000000 Stackinator-4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 16:03:57.000000 Stackinator-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 16:03:57.000000 Stackinator-4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 16:04:11.000000 Stackinator-4.0/PKG-INFO
```

### Comparing `Stackinator-3.0/PKG-INFO` & `Stackinator-4.0/Stackinator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stackinator
-Version: 3.0
+Version: 4.0
 Summary: Stackinator is a tool for building a scientific software stack from a recipe for vClusters on CSCS' Alps infrastructure
 Home-page: https://github.com/eth-cscs/stackinator
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich)
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Stackinator-3.0/stackinator/schema.py` & `Stackinator-4.0/stackinator/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # if they have not been provided.
 
 
 def extend_with_default(validator_class):
     validate_properties = validator_class.VALIDATORS["properties"]
 
     def set_defaults(validator, properties, instance, schema):
-        for property, subschema in properties.items():
-            if "default" in subschema:
-                instance.setdefault(property, subschema["default"])
+        # if instance is none, it's not possible to set any default for any sub-property
+        if instance is not None:
+            for property, subschema in properties.items():
+                if "default" in subschema:
+                    instance.setdefault(property, subschema["default"])
 
         for error in validate_properties(
             validator,
             properties,
             instance,
             schema,
         ):
```

### Comparing `Stackinator-3.0/stackinator/etc/add-compiler-links.py` & `Stackinator-4.0/stackinator/etc/add-compiler-links.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     print(f"error - build path '{args.build_path}' does not exist.")
     exit(2)
 
 compilers = load_compilers_yaml(args.compiler_path)
 
 paths = []
 for c in compilers:
-    local_paths = set([os.path.dirname(v) for k, v in c["paths"].items()])
+    local_paths = set([os.path.dirname(v) for k, v in c["paths"].items() if v is not None])
     paths += local_paths
     print(f'adding compiler {c["spec"]} -> {[p for p in local_paths]}')
 
 # find unique paths and concatenate them
 pathstring = ":".join(set(paths))
 
 # Parse the spack env activation script line by line.
@@ -90,17 +90,15 @@
         if is_alias(parts):
             pass
         elif is_export(parts):
             export = parse_export(line)
 
             # parse PATH to remove references to the build directory
             if export["variable"] == "PATH":
-                paths = [
-                    p for p in export["paths"] if not has_prefix(p, args.build_path)
-                ]
+                paths = [p for p in export["paths"] if not has_prefix(p, args.build_path)]
                 lines.append(f"export PATH={':'.join(paths)};\n")
 
             # drop the SPACK_ENV variable
             elif export["variable"] == "SPACK_ENV":
                 pass
 
             else:
```

### Comparing `Stackinator-3.0/stackinator/etc/Make.inc` & `Stackinator-4.0/stackinator/etc/Make.inc`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/stackinator/recipe.py` & `Stackinator-4.0/stackinator/recipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import pathlib
 
 import jinja2
 import yaml
 
-from . import cache, root_logger, schema
+from . import cache, root_logger, schema, spack_util
 
 
 class Recipe:
     valid_mpi_specs = {
         "cray-mpich": (None, None),
         "mpich": ("4.1", "device=ch4 netmod=ofi +slurm"),
         "mvapich2": (
@@ -59,44 +59,37 @@
         if not self.mount.is_dir():
             raise FileNotFoundError(f"the mount point '{self.mount}' must exist")
 
         # required compiler.yaml file
         compiler_path = self.path / "compilers.yaml"
         self._logger.debug(f"opening {compiler_path}")
         if not compiler_path.is_file():
-            raise FileNotFoundError(
-                f"The recipe path '{compiler_path}' does " f"not contain compilers.yaml"
-            )
+            raise FileNotFoundError(f"The recipe path '{compiler_path}' does " f"not contain compilers.yaml")
 
         with compiler_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
             schema.compilers_validator.validate(raw)
             self.generate_compiler_specs(raw)
 
         # required environments.yaml file
         environments_path = self.path / "environments.yaml"
         self._logger.debug(f"opening {environments_path}")
         if not environments_path.is_file():
-            raise FileNotFoundError(
-                f"The recipe path '{environments_path}' does "
-                f" not contain environments.yaml"
-            )
+            raise FileNotFoundError(f"The recipe path '{environments_path}' does " f" not contain environments.yaml")
 
         with environments_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
             schema.environments_validator.validate(raw)
             self.generate_environment_specs(raw)
 
         # optional modules.yaml file
         modules_path = self.path / "modules.yaml"
         self._logger.debug(f"opening {modules_path}")
         if not modules_path.is_file():
-            modules_path = (
-                pathlib.Path(args.build) / "spack/etc/spack/defaults/modules.yaml"
-            )
+            modules_path = pathlib.Path(args.build) / "spack/etc/spack/defaults/modules.yaml"
             self._logger.debug(f"no modules.yaml provided - using the {modules_path}")
 
         self.modules = modules_path
 
         # optional packages.yaml file
         packages_path = self.path / "packages.yaml"
         self._logger.debug(f"opening {packages_path}")
@@ -105,16 +98,15 @@
             with packages_path.open() as fid:
                 self.packages = yaml.load(fid, Loader=yaml.Loader)
 
         # optional mirror configurtion
         mirrors_path = self.path / "mirrors.yaml"
         if mirrors_path.is_file():
             self._logger.warning(
-                "mirrors.yaml have been removed from recipes,"
-                " use the --cache option on stack-config instead."
+                "mirrors.yaml have been removed from recipes," " use the --cache option on stack-config instead."
             )
             raise RuntimeError("Unsupported mirrors.yaml file in recipe.")
 
         self.mirror = (args.cache, self.mount)
 
         # optional post install hook
         if self.post_install_hook is not None:
@@ -125,14 +117,24 @@
         # optional pre install hook
         if self.pre_install_hook is not None:
             self._logger.debug(f"pre install hook {self.pre_install_hook}")
         else:
             self._logger.debug("no pre install hook provided")
 
     # Returns:
+    #   Path: if the recipe contains a spack package repository
+    #   None: if there is the recipe contains no repo
+    @property
+    def spack_repo(self):
+        repo_path = self.path / "repo"
+        if spack_util.is_repo(repo_path):
+            return repo_path
+        return None
+
+    # Returns:
     #   Path: of the recipe extra path if it exists
     #   None: if there is no user-provided extra path in the recipe
     @property
     def user_extra(self):
         extra_path = self.path / "extra"
         if extra_path.exists() and extra_path.is_dir():
             return extra_path
@@ -176,40 +178,53 @@
         self._mirror = None
 
         file, mount = configuration
 
         if file is not None:
             mirror_config_path = pathlib.Path(file)
             if not mirror_config_path.is_file():
-                raise FileNotFoundError(
-                    f"The cache configuration '{file}' is not a file"
-                )
+                raise FileNotFoundError(f"The cache configuration '{file}' is not a file")
 
-            self._mirror = cache.configuration_from_file(
-                mirror_config_path, pathlib.Path(mount)
-            )
+            self._mirror = cache.configuration_from_file(mirror_config_path, pathlib.Path(mount))
 
     @property
     def config(self):
         return self._config
 
     @config.setter
     def config(self, config_path):
         self._logger.debug(f"opening {config_path}")
         if not config_path.is_file():
-            raise FileNotFoundError(
-                f"The recipe path '{config_path}' does not contain compilers.yaml"
-            )
+            raise FileNotFoundError(f"The recipe path '{config_path}' does not contain compilers.yaml")
 
         with config_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
             schema.config_validator.validate(raw)
             self._config = raw
 
     @property
+    def spack_version(self):
+        # determine the "major" version, if it can be inferred.
+        # one of "0.20", "0.21", "develop" or "unknown".
+        commit = self.config["spack"]["commit"]
+        if commit is None or commit == "develop":
+            return "develop"
+        # currently supported
+        if commit.find("0.20") >= 0:
+            return "0.20"
+        # currently supported
+        if commit.find("0.21") >= 0:
+            return "0.21"
+        # branches that contain wip for the next v0.22 release
+        if commit.find("0.22") >= 0:
+            return "0.22"
+
+        return "unknown"
+
+    @property
     def environment_view_meta(self):
         # generate the view meta data that is presented in the squashfs image meta data
         view_meta = {}
         for _, env in self.environments.items():
             view = env["view"]
             if view is not None:
                 view_meta[view["name"]] = {
@@ -220,17 +235,15 @@
 
         return view_meta
 
     @property
     def modules_yaml(self):
         with self.modules.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
-            raw["modules"]["default"]["roots"]["tcl"] = (
-                pathlib.Path(self.mount) / "modules"
-            ).as_posix()
+            raw["modules"]["default"]["roots"]["tcl"] = (pathlib.Path(self.mount) / "modules").as_posix()
             return yaml.dump(raw)
 
     # creates the self.environments field that describes the full specifications
     # for all of the environments sets, grouped in environments, from the raw
     # environments.yaml input.
     def generate_environment_specs(self, raw):
         environments = raw
@@ -279,27 +292,28 @@
                     else:
                         # TODO: Create a custom exception type
                         raise Exception(f"Unsupported mpi: {mpi_impl}")
 
         # An awkward hack to work around spack not supporting creating activation
         # scripts for each file system view in an environment: it only generates them
         # for the "default" view.
-        # The workaround is to create multiple versions of the same environment, one for
-        # each view.
-        # TODO: remove when the minimum supported version of Spack supports generation
-        # for more than one view.
+        # The workaround is to create multiple versions of the same environment, one
+        # for each view.
+        # TODO: remove when the minimum supported version of spack is v0.21, in which
+        # this issue was fixed, see https://github.com/spack/spack/pull/40549
+        # we have a `--develop` workaround that uses the current approach of generating
+        # a separate environment for each view, with a view named "default", and uses
+        # the name default to generated the activation script.
         env_names = set()
         env_name_map = {}
         for name, config in environments.items():
             env_name_map[name] = []
             for view, vc in config["views"].items():
                 if view in env_names:
-                    raise Exception(
-                        f"An environment view with the name '{view}' already exists."
-                    )
+                    raise Exception(f"An environment view with the name '{view}' already exists.")
                 # save a copy of the view configuration
                 env_name_map[name].append((view, vc))
 
         # Iterate over each environment:
         # - creating copies of the env so that there is one copy per view.
         # - configure each view
         for name, views in env_name_map.items():
@@ -393,17 +407,15 @@
             llvm["packages"] = False
             llvm["specs"] = []
             for spec in raw["llvm"]["specs"]:
                 if spec.startswith("nvhpc"):
                     llvm["specs"].append(f"{spec}~mpi~blas~lapack")
 
                 if spec.startswith("llvm"):
-                    llvm["specs"].append(
-                        f"{spec} +clang targets=x86 ~gold ^ninja@kitware"
-                    )
+                    llvm["specs"].append(f"{spec} +clang targets=x86 ~gold ^ninja@kitware")
 
             llvm["requires"] = raw["llvm"]["requires"]
             llvm["exclude_from_cache"] = ["nvhpc"]
             compilers["llvm"] = llvm
 
         self.compilers = compilers
 
@@ -415,17 +427,15 @@
     @system_config_path.setter
     def system_config_path(self, path):
         system_path = pathlib.Path(path)
         if not system_path.is_absolute():
             system_path = pathlib.Path.cwd() / system_path
 
         if not system_path.is_dir():
-            raise FileNotFoundError(
-                f"The system configuration path '{system_path}' does not exist"
-            )
+            raise FileNotFoundError(f"The system configuration path '{system_path}' does not exist")
 
         self._system_path = system_path
 
     @property
     def mount(self):
         return pathlib.Path(self.config["store"])
 
@@ -468,17 +478,16 @@
 
         makefile_template = jenv.get_template("Makefile.environments")
         push_to_cache = self.mirror is not None
         files["makefile"] = makefile_template.render(
             environments=self.environments,
             push_to_cache=push_to_cache,
             develop=self.spack_develop,
+            spack_version=self.spack_version,
         )
 
         files["config"] = {}
         for env, config in self.environments.items():
             spack_yaml_template = jenv.get_template("environments.spack.yaml")
-            files["config"][env] = spack_yaml_template.render(
-                config=config, name=env, store=self.mount
-            )
+            files["config"][env] = spack_yaml_template.render(config=config, name=env, store=self.mount)
 
         return files
```

### Comparing `Stackinator-3.0/stackinator/schema/environments.json` & `Stackinator-4.0/stackinator/schema/environments.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992177327473959%*

 * *Differences: {"'patternProperties'": "{'\\\\w[\\\\w-]*': {'properties': {'mpi': {'oneOf': {0: {'properties': "*

 * *                        "{'gpu': {'default': None}}}}}, 'deprecated': OrderedDict([('type', "*

 * *                        "'boolean'), ('default', False)])}}}"}*

```diff
@@ -16,21 +16,26 @@
                                 "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
+                "deprecated": {
+                    "default": false,
+                    "type": "boolean"
+                },
                 "mpi": {
                     "default": null,
                     "oneOf": [
                         {
                             "additionalProperties": false,
                             "properties": {
                                 "gpu": {
+                                    "default": null,
                                     "enum": [
                                         "cuda",
                                         "rocm",
                                         null,
                                         false
                                     ]
                                 },
```

### Comparing `Stackinator-3.0/stackinator/schema/compilers.json` & `Stackinator-4.0/stackinator/schema/compilers.json`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/stackinator/schema/config.json` & `Stackinator-4.0/stackinator/schema/config.json`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/stackinator/cache.py` & `Stackinator-4.0/stackinator/cache.py`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/stackinator/templates/Makefile.environments` & `Stackinator-4.0/stackinator/templates/Makefile.environments`

 * *Files 6% similar despite different names*

```diff
@@ -14,37 +14,36 @@
 # Ensure that package yaml files are never removed as intermediate files...
 .packages.yaml:{% for env in environments %} {{ env }}/packages.yaml{% endfor %}
 
 # Push built packages to a binary cache if a key has been provided
 {% for env, config in environments.items() %}
 {{ env }}/generated/build_cache: {{ env }}/generated/view_config
 {% if push_to_cache %}
-{% if develop %}
 	$(SPACK) -e ./{{ env }} buildcache create --rebuild-index --allow-root --only=package alpscache \
-	$$($(SPACK) --color=never -e ./{{ env }} find --format '{name};{/hash}' \
+	$$($(SPACK) --color=never -e ./{{ env }} find --format '{name};{/hash};version={version}' \
 	| grep -v -E '^({% for p in config.exclude_from_cache %}{{ pipejoiner() }}{{ p }}{% endfor %});'\
+	| grep -v -E 'version=git\.'\
 	| cut -d ';' -f2)
-{% else %}
-	$(SPACK) -e ./{{ env }} buildcache create --rebuild-index --allow-root --only=package -m alpscache \
-	$$($(SPACK) --color=never -e ./{{ env }} find --format '{name};{/hash}' \
-	| grep -v -E '^({% for p in config.exclude_from_cache %}{{ pipejoiner() }}{{ p }}{% endfor %});'\
-	| cut -d ';' -f2)
-{% endif %}
 {% endif %}
 	touch $@
 
 {% endfor %}
 
 # Create environment view where requested
 {% for env, config in environments.items() %}
 {{ env }}/generated/view_config: {{ env }}/generated/env
 {% if config.view %}
+{% if develop or (spack_version>="0.21") %}
+	$(SPACK) env activate --with-view default --sh ./{{ env }} > $(STORE)/env/{{ config.view.name }}/activate.sh
+	$(SOFTWARE_STACK_PROJECT)/add-compiler-links.py  ./{{ env }}/compilers.yaml $(STORE)/env/{{ config.view.name }}/activate.sh $(SOFTWARE_STACK_PROJECT)
+{% else %}
 	$(SPACK) env activate --with-view --sh ./{{ env }} > $(STORE)/env/{{ config.view.name }}/activate.sh
 	$(SOFTWARE_STACK_PROJECT)/add-compiler-links.py  ./{{ env }}/compilers.yaml $(STORE)/env/{{ config.view.name }}/activate.sh $(SOFTWARE_STACK_PROJECT)
 {% endif %}
+{% endif %}
 	touch $@
 
 {% endfor %}
 
 
 {% for env in environments %}{{ env }}/config.yaml {% endfor %}: | store
 	$(SPACK) config --scope=user add config:install_tree:root:$(STORE)
```

### Comparing `Stackinator-3.0/stackinator/templates/environments.spack.yaml` & `Stackinator-4.0/stackinator/templates/environments.spack.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 spack:
   include:
 {% if config.packages %}
   - packages.yaml
 {% endif %}
   - compilers.yaml
   - config.yaml
+  config:
+    deprecated: {{ config.deprecated }}
   concretizer:
     unify: {{ config.unify }}
     reuse: false
   specs:
 {% for spec in config.specs %}
   - {{ spec }}
 {% endfor %}
```

### Comparing `Stackinator-3.0/stackinator/templates/Makefile` & `Stackinator-4.0/stackinator/templates/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -60,33 +60,30 @@
 post-install: generate-config environments{% if modules %} modules{% endif %}
 
 	$(SANDBOX) $(STORE)/post-install-hook
 
 # Create a squashfs file from the installed software.
 store.squashfs: environments generate-config{% if modules %} modules{% endif %}{% if post_install_hook %} post-install{% endif %}
 
+	# clean up the __pycache__ paths in the repo
+	$(SANDBOX) find $(STORE)/repo -type d -name __pycache__ -exec rm -r {} +
 	$(SANDBOX) env -u SOURCE_DATE_EPOCH "$$($(SANDBOX) $(SPACK) -e ./compilers/bootstrap find --format='{prefix}' squashfs | head -n1)/bin/mksquashfs" $(STORE) $@ -all-root -all-time $$(date +%s) -no-recovery -noappend -Xcompression-level 3
 
 # Force push all built packages to the build cache
 cache-force: mirror-setup
 {% if cache.key %}
 	$(warning ================================================================================)
 	$(warning Generate the config in order to force push partially built compiler environments)
 	$(warning if this step is performed with partially built compiler envs, you will)
 	$(warning likely have to start a fresh build (but that's okay, because build caches FTW))
 	$(warning ================================================================================)
 	$(SANDBOX) $(MAKE) -C generate-config
-{% if develop %}
 	$(SANDBOX) $(SPACK) -C $(STORE)/config buildcache create --rebuild-index --allow-root --only=package alpscache \
 	$$($(SANDBOX) $(SPACK) --color=never -C $(STORE)/config find --format '{/hash}')
 {% else %}
-	$(SANDBOX) $(SPACK) -C $(STORE)/config buildcache create --rebuild-index --allow-root --only=package -m alpscache \
-	$$($(SANDBOX) $(SPACK) --color=never -C $(STORE)/config find --format '{/hash}')
-{% endif %}
-{% else %}
 	$(warning "pushing to the build cache is not enabled. See the documentation on how to add a key: https://eth-cscs.github.io/stackinator/build-caches/")
 {% endif %}
 
 # A backup of all the generated files during the build, useful for posterity,
 # excluding the binaries themselves, since they're in the squashfs file
 build.tar.gz: spack-version Make.user Make.inc Makefile | environments
 	tar czf $@ $^ $$(find environments compilers config -maxdepth 2 -name Makefile -o -name '*.yaml')
```

### Comparing `Stackinator-3.0/stackinator/templates/Make.user` & `Stackinator-4.0/stackinator/templates/Make.user`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/stackinator/templates/Makefile.compilers` & `Stackinator-4.0/stackinator/templates/Makefile.compilers`

 * *Files 7% similar despite different names*

```diff
@@ -15,25 +15,18 @@
 # Ensure that package yaml files are never removed as intermediate files...
 .packages.yaml:{% for compiler in compilers %} {{ compiler }}/packages.yaml{% endfor %}
 
 
 {% for compiler, config in compilers.items() %}
 {{ compiler }}/generated/build_cache: {{ compiler }}/generated/env
 {% if push_to_cache %}
-{% if develop %}
 	$(SPACK) -e ./{{ compiler }} buildcache create --rebuild-index --allow-root --only=package alpscache \
 	$$($(SPACK) --color=never -e ./{{ compiler }} find --format '{name};{/hash}' \
 	| grep -v -E '^({% for p in config.exclude_from_cache %}{{ pipejoiner() }}{{ p }}{% endfor %});'\
 	| cut -d ';' -f2)
-{% else %}
-	$(SPACK) -e ./{{ compiler }} buildcache create --rebuild-index --allow-root --only=package -m alpscache \
-	$$($(SPACK) --color=never -e ./{{ compiler }} find --format '{name};{/hash}' \
-	| grep -v -E '^({% for p in config.exclude_from_cache %}{{ pipejoiner() }}{{ p }}{% endfor %});'\
-	| cut -d ';' -f2)
-{% endif %}
 {% endif %}
 	touch $@
 
 {% endfor %}
 
 # Configure the install location.
 {% for compiler in compilers %}{{ compiler }}/config.yaml {% endfor %}: | store
```

### Comparing `Stackinator-3.0/stackinator/templates/Makefile.generate-config` & `Stackinator-4.0/stackinator/templates/Makefile.generate-config`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 $(CONFIG_DIR)/upstreams.yaml:
 	$(SPACK) config --scope=user add upstreams:system:install_tree:$(STORE)
 
 # Copy the cluster-specific packages.yaml file to the configuration.
 # requires compilers.yaml to ensure that the path $(CONFIG_DIR) has been created.
 $(CONFIG_DIR)/packages.yaml: $(CONFIG_DIR)/compilers.yaml
-	cp $(SOFTWARE_STACK_PROJECT)/config/packages.yaml $(CONFIG_DIR)/packages.yaml
+	install -m 644 $(SOFTWARE_STACK_PROJECT)/config/packages.yaml $(CONFIG_DIR)/packages.yaml
 
 $(CONFIG_DIR)/repos.yaml: $(CONFIG_DIR)/compilers.yaml
-	cp $(SOFTWARE_STACK_PROJECT)/config/repos.yaml $(CONFIG_DIR)/repos.yaml
+	install -m 644 $(SOFTWARE_STACK_PROJECT)/config/repos.yaml $(CONFIG_DIR)/repos.yaml
 
 # Generate a configuration used to generate the module files
 # The configuration in CONFIG_DIR can't be used for this purpose, because a compilers.yaml
 # that includes the bootstrap compiler is required to build the modules.
 $(MODULE_DIR)/compilers.yaml:
 	$(SPACK) compiler find --scope=user $(call compiler_bin_dirs, $(ALL_COMPILER_PREFIXES))
```

### Comparing `Stackinator-3.0/stackinator/builder.py` & `Stackinator-4.0/stackinator/builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,53 @@
 import subprocess
 import sys
 from datetime import datetime
 
 import jinja2
 import yaml
 
-from . import VERSION, cache, root_logger
+from . import VERSION, cache, root_logger, spack_util
+
+
+def install(src, dst, *, ignore=None, symlinks=False):
+    """Call shutil.copytree or shutil.copy2. copy2 is used if `src` is not a directory.
+    Afterwards run the equivalent of chmod a+rX dst."""
+
+    def apply_permissions_recursive(directory):
+        """Apply permissions recursively to an entire directory."""
+
+        def set_permissions(path):
+            """Set permissions for a given path based on chmod a+rX equivalent."""
+            mode = os.stat(path).st_mode
+            # Always give read permissions for user, group, and others.
+            new_mode = mode | stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH
+            # If it's a directory or execute bit is set for owner or group,
+            # set execute bit for all.
+            if stat.S_ISDIR(mode) or mode & (stat.S_IXUSR | stat.S_IXGRP):
+                new_mode |= stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH
+            os.chmod(path, new_mode)
+
+        set_permissions(directory)
+        for dirpath, dirnames, filenames in os.walk(directory):
+            for dirname in dirnames:
+                set_permissions(os.path.join(dirpath, dirname))
+            for filename in filenames:
+                set_permissions(os.path.join(dirpath, filename))
+
+    if stat.S_ISDIR(os.stat(src).st_mode):
+        shutil.copytree(
+            src,
+            dst,
+            ignore=ignore,
+            symlinks=symlinks,
+        )
+    else:
+        shutil.copy2(src, dst, follow_symlinks=symlinks)
+    # set permissions
+    apply_permissions_recursive(dst)
 
 
 class Builder:
     def __init__(self, args):
         self._logger = root_logger
         path = pathlib.Path(args.build)
         if not path.is_absolute():
@@ -44,14 +82,17 @@
             raise IOError("build path can't be in '$HOME' or '~'")
         # if path.is_relative_to(pathlib.Path.home()):
         # raise IOError("build path can't be in '$HOME' or '~'")
 
         self.path = path
         self.root = pathlib.Path(__file__).parent.resolve()
 
+        # Optionally support breaking changes in Spack develop
+        self.spack_develop = args.develop
+
     @property
     def configuration_meta(self):
         """Meta data about the configuration and build"""
         return self._configuration_meta
 
     @configuration_meta.setter
     def configuration_meta(self, recipe):
@@ -128,14 +169,15 @@
         tmp_path = self.path / "tmp"
 
         self.path.mkdir(exist_ok=True, parents=True)
         store_path.mkdir(exist_ok=True)
         tmp_path.mkdir(exist_ok=True)
 
         # check out the version of spack
+        spack_version = recipe.spack_version
         spack = recipe.config["spack"]
         spack_path = self.path / "spack"
 
         # set general build and configuration meta data for the project
         self.configuration_meta = recipe
 
         # set the environment view meta data
@@ -151,32 +193,30 @@
                 shell=False,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
             )
             self._logger.debug(capture.stdout.decode("utf-8"))
 
             if capture.returncode != 0:
-                self._logger.debug(f'error cloning the repository {spack["repo"]}')
+                self._logger.error(f'error cloning the repository {spack["repo"]}')
                 capture.check_returncode()
 
         # Check out a branch or commit if one was specified
         if spack["commit"]:
             self._logger.info(f'spack: checkout branch/commit {spack["commit"]}')
             capture = subprocess.run(
                 ["git", "-C", spack_path, "checkout", spack["commit"]],
                 shell=False,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
             )
             self._logger.debug(capture.stdout.decode("utf-8"))
 
             if capture.returncode != 0:
-                self._logger.debug(
-                    f'unable to change to the requested commit {spack["commit"]}'
-                )
+                self._logger.debug(f'unable to change to the requested commit {spack["commit"]}')
                 capture.check_returncode()
 
         # load the jinja templating environment
         template_path = self.root / "templates"
         jinja_env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(template_path),
             trim_blocks=True,
@@ -189,26 +229,24 @@
         with (self.path / "Makefile").open("w") as f:
             f.write(
                 makefile_template.render(
                     cache=recipe.mirror,
                     modules=recipe.config["modules"],
                     post_install_hook=recipe.post_install_hook,
                     pre_install_hook=recipe.pre_install_hook,
+                    develop=self.spack_develop,
+                    spack_version=spack_version,
                     verbose=False,
                 )
             )
             f.write("\n")
 
         make_user_template = jinja_env.get_template("Make.user")
         with (self.path / "Make.user").open("w") as f:
-            f.write(
-                make_user_template.render(
-                    build_path=self.path, store=recipe.mount, verbose=False
-                )
-            )
+            f.write(make_user_template.render(build_path=self.path, store=recipe.mount, verbose=False))
             f.write("\n")
 
         etc_path = self.root / "etc"
         for f_etc in ["Make.inc", "bwrap-mutable-root.sh", "add-compiler-links.py"]:
             shutil.copy2(etc_path / f_etc, self.path / f_etc)
 
         # used to configure both pre and post install hooks, if they are provided.
@@ -219,17 +257,15 @@
             "spack": self.path / "spack",
         }
 
         # copy post install hook file, if provided
         post_hook = recipe.post_install_hook
         if post_hook is not None:
             self._logger.debug("installing post-install-hook script")
-            jinja_recipe_env = jinja2.Environment(
-                loader=jinja2.FileSystemLoader(recipe.path)
-            )
+            jinja_recipe_env = jinja2.Environment(loader=jinja2.FileSystemLoader(recipe.path))
             post_hook_template = jinja_recipe_env.get_template("post-install")
             post_hook_destination = store_path / "post-install-hook"
 
             with post_hook_destination.open("w") as f:
                 f.write(post_hook_template.render(env=hook_env, verbose=False))
                 f.write("\n")
 
@@ -238,17 +274,15 @@
                 os.stat(post_hook_destination).st_mode | stat.S_IEXEC,
             )
 
         # copy pre install hook file, if provided
         pre_hook = recipe.pre_install_hook
         if pre_hook is not None:
             self._logger.debug("installing pre-install-hook script")
-            jinja_recipe_env = jinja2.Environment(
-                loader=jinja2.FileSystemLoader(recipe.path)
-            )
+            jinja_recipe_env = jinja2.Environment(loader=jinja2.FileSystemLoader(recipe.path))
             pre_hook_template = jinja_recipe_env.get_template("pre-install")
             pre_hook_destination = store_path / "pre-install-hook"
 
             with pre_hook_destination.open("w") as f:
                 f.write(pre_hook_template.render(env=hook_env, verbose=False))
                 f.write("\n")
 
@@ -267,17 +301,15 @@
         for f_config in system_config_path.iterdir():
             # print warning if mirrors.yaml is found
             if f_config.name in ["mirrors.yaml"]:
                 self._logger.error(
                     "mirrors.yaml have been removed from cluster configurations,"
                     " use the --cache option on stack-config instead."
                 )
-                raise RuntimeError(
-                    "Unsupported mirrors.yaml file in cluster configuration."
-                )
+                raise RuntimeError("Unsupported mirrors.yaml file in cluster configuration.")
 
             # construct full file path
             src = system_config_path / f_config.name
             dst = config_path / f_config.name
             # copy only files
             if src.is_file():
                 shutil.copy(src, dst)
@@ -300,54 +332,99 @@
                     packages_data = raw["packages"]
             packages_data.update(recipe.packages["packages"])
             packages_yaml = yaml.dump({"packages": packages_data})
             packages_path = config_path / "packages.yaml"
             with packages_path.open("w") as fid:
                 fid.write(packages_yaml)
 
-        # Configure the CSCS custom spack environments.
-        # Step 1: copy the CSCS repo to store_path where, it will be used to
+        # Add custom spack package recipes, configured via Spack repos.
+        # Step 1: copy Spack repos to store_path where they will be used to
         #         build the stack, and then be part of the upstream provided
         #         to users of the stack.
-        repo_src = self.root / "repo"
+        #
+        # Packages in the recipe are prioritised over cluster specific packages,
+        # etc. The order of preference from highest to lowest is:
+        #
+        # 3. recipe/repo
+        # 2. cluster-config/repos.yaml
+        #   - if the repos.yaml file exists it will contain a list of relative paths
+        #     to search for package
+        # 1. spack/var/spack/repos/builtin
+
+        # Build a list of repos with packages to install.
+        repos = []
+
+        # check for a repo in the recipe
+        if recipe.spack_repo is not None:
+            self._logger.debug(f"adding recipe spack package repo: {recipe.spack_repo}")
+            repos.append(recipe.spack_repo)
+
+        # look for repos.yaml file in the system configuration
+        repo_yaml = system_config_path / "repos.yaml"
+        if repo_yaml.exists() and repo_yaml.is_file():
+            # open repos.yaml file and reat the list of repos
+            with repo_yaml.open() as fid:
+                raw = yaml.load(fid, Loader=yaml.Loader)
+                P = raw["repos"]
+
+            self._logger.debug(f"the system configuration has a repo file {repo_yaml} refers to {P}")
+
+            # test each path
+            for rel_path in P:
+                repo_path = (system_config_path / rel_path).resolve()
+                if spack_util.is_repo(repo_path):
+                    repos.append(repo_path)
+                    self._logger.debug(f"adding site spack package repo: {repo_path}")
+                else:
+                    self._logger.error(f"{repo_path} from {repo_yaml} is not a spack package repository")
+                    raise RuntimeError("invalid system-provided package repository")
+
+        self._logger.debug(f"full list of spack package repo: {repos}")
+
+        # Delete the store/repo path, if it already exists.
+        # Do this so that incremental builds (though not officially supported) won't break if a repo is updated.
         repo_dst = store_path / "repo"
+        self._logger.debug(f"creating the stack spack prepo in {repo_dst}")
         if repo_dst.exists():
+            self._logger.debug(f"{repo_dst} exists ... deleting")
             shutil.rmtree(repo_dst)
 
-        shutil.copytree(repo_src, repo_dst)
+        # Iterate over the source repositories copying their contents to the consolidated repo in the uenv.
+        # Do overwrite packages that have been copied from an earlier source repo, enforcing a descending
+        # order of precidence.
+        if len(repos) > 0:
+            pkg_dst = repo_dst / "packages"
+            pkg_dst.mkdir(mode=0o755, parents=True)
+            self._logger.debug(f"created the repo packages path {pkg_dst}")
+            for repo_src in repos:
+                self._logger.debug(f"installing repo {repo_src}")
+                packages_path = repo_src / "packages"
+                for pkg_path in packages_path.iterdir():
+                    dst = pkg_dst / pkg_path.name
+                    if pkg_path.is_dir() and not dst.exists():
+                        self._logger.debug(f"  installing package {pkg_path} to {pkg_dst}")
+                        install(pkg_path, dst)
+                    elif dst.exists():
+                        self._logger.debug(f"  NOT installing package {pkg_path}")
+            # create the repo.yaml file that configures the repo.
+            with (repo_dst / "repo.yaml").open("w") as f:
+                f.write(
+                    """\
+repo:
+  namespace: alps
+"""
+                )
 
-        # Step 2: Create a repos.yaml file in build_path/config
+        # Create a repos.yaml file in build_path/config
         repos_yaml_template = jinja_env.get_template("repos.yaml")
         with (config_path / "repos.yaml").open("w") as f:
             repo_path = recipe.mount / "repo"
-            f.write(
-                repos_yaml_template.render(
-                    repo_path=repo_path.as_posix(), verbose=False
-                )
-            )
+            f.write(repos_yaml_template.render(repo_path=repo_path.as_posix(), verbose=False))
             f.write("\n")
 
-        # Add user-defined repo to internal repo
-        user_repo_path = recipe.path / "repo"
-        if user_repo_path.exists() and user_repo_path.is_dir():
-            user_repo_yaml = user_repo_path / "repo.yaml"
-            if user_repo_yaml.exists():
-                self._logger.warning(f"Found 'repo.yaml' file in {user_repo_path}")
-                self._logger.warning(
-                    "'repo.yaml' is ignored, packages are added to the 'alps' repo"
-                )
-
-            # Copy user-provided recipes into repo
-            user_repo_packages = user_repo_path / "packages"
-            for user_recipe_dir in user_repo_packages.iterdir():
-                if user_recipe_dir.is_dir():  # iterdir() yelds files too
-                    shutil.copytree(
-                        user_recipe_dir, repo_dst / "packages" / user_recipe_dir.name
-                    )
-
         # Generate the makefile and spack.yaml files that describe the compilers
         compiler_files = recipe.compiler_files
         compiler_path = self.path / "compilers"
         compiler_path.mkdir(exist_ok=True)
         with (compiler_path / "Makefile").open(mode="w") as f:
             f.write(compiler_files["makefile"])
 
@@ -398,46 +475,38 @@
 
         # write the meta data
         meta_path = self.path / "store/meta"
         meta_path.mkdir(exist_ok=True)
         # write a json file with basic meta data
         with (meta_path / "configure.json").open("w") as f:
             # default serialisation is str to serialise the pathlib.PosixPath
-            f.write(
-                json.dumps(
-                    self.configuration_meta, sort_keys=True, indent=2, default=str
-                )
-            )
+            f.write(json.dumps(self.configuration_meta, sort_keys=True, indent=2, default=str))
             f.write("\n")
 
         # write a json file with the environment view meta data
         with (meta_path / "env.json").open("w") as f:
             # default serialisation is str to serialise the pathlib.PosixPath
-            f.write(
-                json.dumps(self.environment_meta, sort_keys=True, indent=2, default=str)
-            )
+            f.write(json.dumps(self.environment_meta, sort_keys=True, indent=2, default=str))
             f.write("\n")
 
         # copy the recipe to a recipe subdirectory of the meta path
         meta_recipe_path = meta_path / "recipe"
         meta_recipe_path.mkdir(exist_ok=True)
         if meta_recipe_path.exists():
             shutil.rmtree(meta_recipe_path)
-        shutil.copytree(
-            recipe.path, meta_recipe_path, ignore=shutil.ignore_patterns(".git")
-        )
+        install(recipe.path, meta_recipe_path, ignore=shutil.ignore_patterns(".git"))
 
         # create the meta/extra path and copy recipe meta data if it exists
         meta_extra_path = meta_path / "extra"
         meta_extra_path.mkdir(exist_ok=True)
         if meta_extra_path.exists():
             shutil.rmtree(meta_extra_path)
         if recipe.user_extra is not None:
             self._logger.debug(f"copying extra recipe meta data to {meta_extra_path}")
-            shutil.copytree(recipe.user_extra, meta_extra_path)
+            install(recipe.user_extra, meta_extra_path)
 
         # create debug helper script
         debug_script_path = self.path / "stack-debug.sh"
         debug_script_template = jinja_env.get_template("stack-debug.sh")
         with debug_script_path.open("w") as f:
             f.write(
                 debug_script_template.render(
```

### Comparing `Stackinator-3.0/stackinator/main.py` & `Stackinator-4.0/stackinator/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,20 @@
     root_logger.info("Stackinator")
     root_logger.info(f"  recipe path: {args.recipe}")
     root_logger.info(f"  build path : {args.build}")
     root_logger.info(f"  system     : {args.system}")
     mount = args.mount or "default"
     root_logger.info(f"  mount      : {mount}")
     root_logger.info(f"  build cache: {args.cache}")
+    root_logger.info(f"  develop    : {args.develop}")
 
 
 def make_argparser():
-    parser = argparse.ArgumentParser(
-        description=(
-            "Generate a build configuration for a spack stack from " "a recipe."
-        )
-    )
-    parser.add_argument(
-        "--version", action="version", version=f"stackinator version {VERSION}"
-    )
+    parser = argparse.ArgumentParser(description=("Generate a build configuration for a spack stack from " "a recipe."))
+    parser.add_argument("--version", action="version", version=f"stackinator version {VERSION}")
     parser.add_argument("-b", "--build", required=True, type=str)
     parser.add_argument("-r", "--recipe", required=True, type=str)
     parser.add_argument("-s", "--system", required=True, type=str)
     parser.add_argument("-d", "--debug", action="store_true")
     parser.add_argument("-m", "--mount", required=False, type=str)
     parser.add_argument("-c", "--cache", required=False, type=str)
     parser.add_argument("--develop", action="store_true", required=False)
@@ -74,21 +69,18 @@
         log_header(args)
 
         recipe = Recipe(args)
         builder = Builder(args)
 
         builder.generate(recipe)
 
-        root_logger.info(
-            "\nConfiguration finished, run the following to build the " "environment:\n"
-        )
+        root_logger.info("\nConfiguration finished, run the following to build the " "environment:\n")
         root_logger.info(f"cd {builder.path}")
         root_logger.info(
-            "env --ignore-environment PATH=/usr/bin:/bin:`pwd`"
-            "/spack/bin make store.squashfs -j32"
+            "env --ignore-environment PATH=/usr/bin:/bin:`pwd`" "/spack/bin HOME=$HOME make store.squashfs -j32"
         )
         return 0
     except Exception as e:
         root_logger.debug(traceback.format_exc())
         root_logger.error(str(e))
         root_logger.info(f"see {logfile} for more information")
         return 1
```

### Comparing `Stackinator-3.0/LICENSE` & `Stackinator-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/setup.cfg` & `Stackinator-4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Stackinator-3.0/Stackinator.egg-info/PKG-INFO` & `Stackinator-4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stackinator
-Version: 3.0
+Version: 4.0
 Summary: Stackinator is a tool for building a scientific software stack from a recipe for vClusters on CSCS' Alps infrastructure
 Home-page: https://github.com/eth-cscs/stackinator
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich)
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Stackinator-3.0/Stackinator.egg-info/SOURCES.txt` & `Stackinator-4.0/Stackinator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 bin/stack-config
 stackinator/__init__.py
 stackinator/builder.py
 stackinator/cache.py
 stackinator/main.py
 stackinator/recipe.py
 stackinator/schema.py
+stackinator/spack_util.py
 stackinator/etc/Make.inc
 stackinator/etc/add-compiler-links.py
 stackinator/etc/bwrap-mutable-root.sh
-stackinator/repo/repo.yaml
-stackinator/repo/packages/cray-mpich/package.py
 stackinator/schema/cache.json
 stackinator/schema/compilers.json
 stackinator/schema/config.json
 stackinator/schema/environments.json
 stackinator/templates/Make.user
 stackinator/templates/Makefile
 stackinator/templates/Makefile.compilers
```


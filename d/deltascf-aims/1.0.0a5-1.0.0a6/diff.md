# Comparing `tmp/deltascf_aims-1.0.0a5.tar.gz` & `tmp/deltascf_aims-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltascf_aims-1.0.0a5.tar", max compression
+gzip compressed data, was "deltascf_aims-1.0.0a6.tar", max compression
```

## Comparing `deltascf_aims-1.0.0a5.tar` & `deltascf_aims-1.0.0a6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2024-02-28 16:54:54.129180 deltascf_aims-1.0.0a5/LICENSE
--rw-r--r--   0        0        0     2264 2024-02-28 16:54:54.129263 deltascf_aims-1.0.0a5/README.md
--rw-r--r--   0        0        0        0 2024-02-28 16:54:54.129325 deltascf_aims-1.0.0a5/deltascf_aims/__init__.py
--rw-r--r--   0        0        0     4815 2024-03-28 12:47:42.144566 deltascf_aims-1.0.0a5/deltascf_aims/__main__.py
--rw-r--r--   0        0        0     1730 2024-02-28 16:54:54.129402 deltascf_aims-1.0.0a5/deltascf_aims/add_basis_functions.yml
--rw-r--r--   0        0        0      258 2024-03-28 14:55:28.230756 deltascf_aims-1.0.0a5/deltascf_aims/aims_bin_loc.txt
--rw-r--r--   0        0        0    36793 2024-03-28 20:05:12.683121 deltascf_aims-1.0.0a5/deltascf_aims/aims_dscf.py
--rw-r--r--   0        0        0     3418 2024-02-28 16:54:54.129658 deltascf_aims-1.0.0a5/deltascf_aims/calc_dscf.py
--rw-r--r--   0        0        0     9414 2024-03-28 18:01:06.045509 deltascf_aims-1.0.0a5/deltascf_aims/cli.py
--rw-r--r--   0        0        0      489 2024-02-28 16:54:54.129838 deltascf_aims-1.0.0a5/deltascf_aims/elements.yml
--rw-r--r--   0        0        0    31988 2024-03-28 20:48:44.941052 deltascf_aims-1.0.0a5/deltascf_aims/force_occupation.py
--rw-r--r--   0        0        0     4827 2024-03-28 19:16:31.531133 deltascf_aims-1.0.0a5/deltascf_aims/main.py
--rw-r--r--   0        0        0    10872 2024-03-28 12:50:18.347558 deltascf_aims-1.0.0a5/deltascf_aims/new_cli.py
--rw-r--r--   0        0        0     6288 2024-03-25 17:01:31.881657 deltascf_aims-1.0.0a5/deltascf_aims/plot.py
--rw-r--r--   0        0        0     3170 2024-03-28 17:59:23.205869 deltascf_aims-1.0.0a5/deltascf_aims/schmid_pseudo_voigt.py
--rw-r--r--   0        0        0        0 2024-03-28 11:17:32.904374 deltascf_aims-1.0.0a5/deltascf_aims/utils/__init__.py
--rw-r--r--   0        0        0     3524 2024-03-28 11:17:32.904669 deltascf_aims-1.0.0a5/deltascf_aims/utils/click_extras.py
--rw-r--r--   0        0        0      265 2024-03-28 11:17:32.905007 deltascf_aims-1.0.0a5/deltascf_aims/utils/hints.py
--rw-r--r--   0        0        0    35347 2024-03-28 19:11:12.815643 deltascf_aims-1.0.0a5/deltascf_aims/utils/utils.py
--rw-r--r--   0        0        0      827 2024-03-28 19:13:36.000967 deltascf_aims-1.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 deltascf_aims-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-28 16:54:54.129180 deltascf_aims-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0     2264 2024-02-28 16:54:54.129263 deltascf_aims-1.0.0a6/README.md
+-rw-r--r--   0        0        0        0 2024-02-28 16:54:54.129325 deltascf_aims-1.0.0a6/deltascf_aims/__init__.py
+-rw-r--r--   0        0        0     4815 2024-03-28 21:21:00.987494 deltascf_aims-1.0.0a6/deltascf_aims/__main__.py
+-rw-r--r--   0        0        0     1730 2024-02-28 16:54:54.129402 deltascf_aims-1.0.0a6/deltascf_aims/add_basis_functions.yml
+-rw-r--r--   0        0        0      258 2024-03-28 14:55:28.230756 deltascf_aims-1.0.0a6/deltascf_aims/aims_bin_loc.txt
+-rw-r--r--   0        0        0    36853 2024-04-04 16:45:42.280517 deltascf_aims-1.0.0a6/deltascf_aims/aims_dscf.py
+-rw-r--r--   0        0        0     3418 2024-02-28 16:54:54.129658 deltascf_aims-1.0.0a6/deltascf_aims/calc_dscf.py
+-rw-r--r--   0        0        0     9573 2024-04-04 16:45:42.281129 deltascf_aims-1.0.0a6/deltascf_aims/cli.py
+-rw-r--r--   0        0        0      489 2024-02-28 16:54:54.129838 deltascf_aims-1.0.0a6/deltascf_aims/elements.yml
+-rw-r--r--   0        0        0    31988 2024-03-28 21:21:00.988561 deltascf_aims-1.0.0a6/deltascf_aims/force_occupation.py
+-rw-r--r--   0        0        0     4827 2024-03-28 21:21:00.988790 deltascf_aims-1.0.0a6/deltascf_aims/main.py
+-rw-r--r--   0        0        0    10872 2024-03-28 21:21:00.989053 deltascf_aims-1.0.0a6/deltascf_aims/new_cli.py
+-rw-r--r--   0        0        0     6288 2024-03-25 17:01:31.881657 deltascf_aims-1.0.0a6/deltascf_aims/plot.py
+-rw-r--r--   0        0        0     3170 2024-03-28 21:21:00.989294 deltascf_aims-1.0.0a6/deltascf_aims/schmid_pseudo_voigt.py
+-rw-r--r--   0        0        0        0 2024-03-28 21:21:00.989342 deltascf_aims-1.0.0a6/deltascf_aims/utils/__init__.py
+-rw-r--r--   0        0        0     3524 2024-03-28 21:21:00.989486 deltascf_aims-1.0.0a6/deltascf_aims/utils/click_extras.py
+-rw-r--r--   0        0        0      265 2024-03-28 21:21:00.989578 deltascf_aims-1.0.0a6/deltascf_aims/utils/hints.py
+-rw-r--r--   0        0        0    35372 2024-04-04 16:45:42.281634 deltascf_aims-1.0.0a6/deltascf_aims/utils/utils.py
+-rw-r--r--   0        0        0      827 2024-04-04 16:48:02.120622 deltascf_aims-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 deltascf_aims-1.0.0a6/PKG-INFO
```

### Comparing `deltascf_aims-1.0.0a5/LICENSE` & `deltascf_aims-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/README.md` & `deltascf_aims-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/__main__.py` & `deltascf_aims-1.0.0a6/deltascf_aims/__main__.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/add_basis_functions.yml` & `deltascf_aims-1.0.0a6/deltascf_aims/add_basis_functions.yml`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/aims_dscf.py` & `deltascf_aims-1.0.0a6/deltascf_aims/aims_dscf.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,14 +655,15 @@
         utils.check_curr_prev_run(
             self.run_type,
             self.start.run_loc,
             self.constr_atoms,
             self.atom_specifier,
             "projector",
             self.start.hpc,
+            self.start.force,
         )
 
         # Check that the restart files exist from the previous calculation
         if check_restart:
             for i_atom in self.atom_specifier:
                 self.check_restart_files(self.constr_atoms, prev_calc, i_atom)
 
@@ -1082,14 +1083,15 @@
         utils.check_curr_prev_run(
             self.run_type,
             self.start.run_loc,
             self.constr_atoms,
             self.atom_specifier,
             "basis",
             self.start.hpc,
+            self.start.force,
         )
 
         # Check that the constrained atoms have been given
         utils.check_params(self.start)
 
         # Check that the required arguments have been given
         utils.check_args(
```

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/calc_dscf.py` & `deltascf_aims-1.0.0a6/deltascf_aims/calc_dscf.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/cli.py` & `deltascf_aims-1.0.0a6/deltascf_aims/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,20 @@
 @click.option(
     "-p",
     "--print_output",
     is_flag=True,
     help="print the live output of the calculation",
 )
 @click.option(
+    "-f",
+    "--force",
+    is_flag=True,
+    help="force the calculation to run even if it has already been run",
+)
+@click.option(
     "-n",
     "--nprocs",
     default=4,
     show_default=True,
     type=int,
     help="number of processors to use",
 )
@@ -134,14 +140,15 @@
     constr_atom,
     spec_at_constr,
     occupation,
     n_atoms,
     basis_set,
     use_extra_basis,
     print_output,
+    force,
     nprocs,
 ):
     """
     An interface to automate core-hole constrained occupation methods in
     FHI-aims.
 
     There is functionality to use both the older and soon-to-be deprecated
@@ -175,14 +182,15 @@
         constr_atom,
         spec_at_constr,
         occupation,
         n_atoms,
         basis_set,
         use_extra_basis,
         print_output,
+        force,
         nprocs,
     )
 
 
 @initialise.command()
 @click.option(
     "-r",
```

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/force_occupation.py` & `deltascf_aims-1.0.0a6/deltascf_aims/force_occupation.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/main.py` & `deltascf_aims-1.0.0a6/deltascf_aims/main.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/new_cli.py` & `deltascf_aims-1.0.0a6/deltascf_aims/new_cli.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/plot.py` & `deltascf_aims-1.0.0a6/deltascf_aims/plot.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/schmid_pseudo_voigt.py` & `deltascf_aims-1.0.0a6/deltascf_aims/schmid_pseudo_voigt.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/utils/click_extras.py` & `deltascf_aims-1.0.0a6/deltascf_aims/utils/click_extras.py`

 * *Files identical despite different names*

### Comparing `deltascf_aims-1.0.0a5/deltascf_aims/utils/utils.py` & `deltascf_aims-1.0.0a6/deltascf_aims/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 def check_curr_prev_run(
     run_type: Literal["ground", "hole", "init_1", "init_2"],
     run_loc,
     constr_atoms,
     atom_specifier,
     constr_method: Literal["projector", "basis"],
     hpc,
+    force,
 ) -> None:
     """
 
     Check if the current calculation has previously been run.
 
     Parameters
     ----------
@@ -238,15 +239,15 @@
     elif constr_method == "projector":
         search_path = (
             f"{run_loc}/{constr_atoms[0]}{atom_specifier[0]}/{run_type}/aims.out"
         )
     elif constr_method == "basis":
         search_path = f"{run_loc}/{constr_atoms[0]}{atom_specifier[0]}/aims.out"
 
-    if os.path.isfile(search_path) and not hpc:
+    if os.path.isfile(search_path) and not hpc and not force:
         warnings.warn("Calculation has already been completed")
         cont = None
         while cont != "y":
             cont = str(input("Do you want to continue? (y/n) ")).lower()
 
             if cont == "n":
                 print("aborting...")
```

### Comparing `deltascf_aims-1.0.0a5/pyproject.toml` & `deltascf_aims-1.0.0a6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltascf-aims"
-version = "1.0.0a5"
+version = "1.0.0a6"
 description = "Application to test calculation of core holes in FHI-aims"
 authors = ["Dylan Morgan <dylan.morgan@warwick.ac.uk>"]
 license = "GPL 3"
 readme = "README.md"
 repository = "https://github.com/maurergroup/deltascf-aims"
 packages = [
     { include = "deltascf_aims" }
```

### Comparing `deltascf_aims-1.0.0a5/PKG-INFO` & `deltascf_aims-1.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltascf-aims
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Application to test calculation of core holes in FHI-aims
 Home-page: https://github.com/maurergroup/deltascf-aims
 License: GPL 3
 Author: Dylan Morgan
 Author-email: dylan.morgan@warwick.ac.uk
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
```


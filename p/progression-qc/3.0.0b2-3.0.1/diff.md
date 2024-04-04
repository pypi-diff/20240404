# Comparing `tmp/progression_qc-3.0.0b2.tar.gz` & `tmp/progression_qc-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progression_qc-3.0.0b2.tar", last modified: Thu Sep  7 18:15:56 2023, max compression
+gzip compressed data, was "progression_qc-3.0.1.tar", last modified: Thu Apr  4 21:19:46 2024, max compression
```

## Comparing `progression_qc-3.0.0b2.tar` & `progression_qc-3.0.1.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 18:15:56.836176 progression_qc-3.0.0b2/
--rw-rw-rw-   0 root         (0) root         (0)    35074 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      572 2023-09-07 18:15:56.836176 progression_qc-3.0.0b2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 18:15:56.832176 progression_qc-3.0.0b2/progression_qc/
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-09-07 17:19:15.000000 progression_qc-3.0.0b2/progression_qc/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7946 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/progression_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 18:15:56.836176 progression_qc-3.0.0b2/progression_qc/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-07 18:15:45.000000 progression_qc-3.0.0b2/progression_qc/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/question_base.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/question_bd.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/question_prog.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-09-07 17:19:15.000000 progression_qc-3.0.0b2/progression_qc/schemas/question_sys.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/question_vcs.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/rétroactions.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-08-29 19:59:51.000000 progression_qc-3.0.0b2/progression_qc/schemas/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/test_prog.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/progression_qc/schemas/test_sys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 18:15:56.832176 progression_qc-3.0.0b2/progression_qc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      572 2023-09-07 18:15:56.000000 progression_qc-3.0.0b2/progression_qc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      722 2023-09-07 18:15:56.000000 progression_qc-3.0.0b2/progression_qc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-07 18:15:56.000000 progression_qc-3.0.0b2/progression_qc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-09-07 18:15:56.000000 progression_qc-3.0.0b2/progression_qc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-07 18:15:56.000000 progression_qc-3.0.0b2/progression_qc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-07 18:15:56.840175 progression_qc-3.0.0b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-08-29 19:44:57.000000 progression_qc-3.0.0b2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 18:15:56.836176 progression_qc-3.0.0b2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8625 2023-08-29 19:59:51.000000 progression_qc-3.0.0b2/tests/test_progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.041484 progression_qc-3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35074 2024-01-22 02:39:15.000000 progression_qc-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-04 21:19:46.041484 progression_qc-3.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/progression_qc/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-04 21:19:33.000000 progression_qc-3.0.1/progression_qc/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7377 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/progression_qc/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:19:34.000000 progression_qc-3.0.1/progression_qc/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_sys.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/rétroactions.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_sys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.041484 progression_qc-3.0.1/progression_qc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      645 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:19:46.041484 progression_qc-3.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-04 21:19:14.000000 progression_qc-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2024-01-22 02:39:15.000000 progression_qc-3.0.1/tests/test_progression_qc.py
```

### Comparing `progression_qc-3.0.0b2/LICENSE` & `progression_qc-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.0b2/progression_qc/__main__.py` & `progression_qc-3.0.1/progression_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.0b2/progression_qc/progression_qc.py` & `progression_qc-3.0.1/progression_qc/progression_qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,35 +55,19 @@
         "question_prog",
         eval(pkg_resources.read_text(schemas, "question_prog.py")),
     )
     schema_registry.add(
         "question_sys",
         eval(pkg_resources.read_text(schemas, "question_sys.py")),
     )
-    schema_registry.add(
-        "question_vcs",
-        eval(pkg_resources.read_text(schemas, "question_vcs.py")),
-    )
-
-    schema_registry.add(
-        "question_bd",
-        {
-            **schema_registry.get("question_sys"),
-            **eval(pkg_resources.read_text(schemas, "question_bd.py")),
-        },
-    )
 
     if "type" in contenu_fichier and contenu_fichier["type"].lower() == "prog":
         schemas_à_valider = "question_prog"
-    elif "type" in contenu_fichier and contenu_fichier["type"].lower() == "vcs":
-        schemas_à_valider = "question_vcs"
     elif "type" in contenu_fichier and contenu_fichier["type"].lower() == "sys":
         schemas_à_valider = "question_sys"
-    elif "type" in contenu_fichier and contenu_fichier["type"].lower() == "bd":
-        schemas_à_valider = "question_bd"
     else:
         schemas_à_valider = "question_base"
 
     return traiter_validation_question_yaml(contenu_fichier, schemas_à_valider)
 
 
 def get_readers():
```

### Comparing `progression_qc-3.0.0b2/progression_qc/schemas/question_base.py` & `progression_qc-3.0.1/progression_qc/schemas/question_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {
-    "type": {"required": True, "type": "string", "regex": "(?i)^(prog|sys|bd|vcs)$"},
+    "type": {"required": True, "type": "string", "regex": "(?i)^(prog|sys)$"},
     "niveau": {"required": False, "type": "string"},
     "titre": {"required": False, "type": "string"},
     "objectif": {"required": False, "type": "string"},
     "description": {"required": False, "type": "string"},
     "énoncé": {
         "required": False,
         "type": ["string", "list"],
```

### Comparing `progression_qc-3.0.0b2/progression_qc/schemas/question_sys.py` & `progression_qc-3.0.1/progression_qc/schemas/question_sys.py`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.0b2/progression_qc.egg-info/SOURCES.txt` & `progression_qc-3.0.1/progression_qc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 progression_qc.egg-info/PKG-INFO
 progression_qc.egg-info/SOURCES.txt
 progression_qc.egg-info/dependency_links.txt
 progression_qc.egg-info/requires.txt
 progression_qc.egg-info/top_level.txt
 progression_qc/schemas/__init__.py
 progression_qc/schemas/question_base.py
-progression_qc/schemas/question_bd.py
 progression_qc/schemas/question_prog.py
 progression_qc/schemas/question_sys.py
-progression_qc/schemas/question_vcs.py
 progression_qc/schemas/rétroactions.py
 progression_qc/schemas/test_base.py
 progression_qc/schemas/test_prog.py
 progression_qc/schemas/test_sys.py
 tests/test_progression_qc.py
```

### Comparing `progression_qc-3.0.0b2/setup.py` & `progression_qc-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     description="progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.",
     url="https://git.dti.crosemont.quebec/progression/validateur",
     author="Patrick Lafrance",
     author_email="plafrance@crosemont.qc.ca",
     license='GPLv3+',
     packages=["progression_qc", "progression_qc/schemas"],
     package_data={"progression_qc": ["VERSION"]},
-    install_requires=["cerberus", "pyyaml-include", "werkzeug"],
+    install_requires=["cerberus", "pyyaml-include==1.4.1", "werkzeug"],
     classifiers=['Programming Language :: Python :: 3'],
 )
```

### Comparing `progression_qc-3.0.0b2/tests/test_progression_qc.py` & `progression_qc-3.0.1/tests/test_progression_qc.py`

 * *Files 15% similar despite different names*

```diff
@@ -154,64 +154,7 @@
     from question_prog_avec_ébauches_et_tests_vides import question
 
     résultat = progression_qc.valider_schema_yaml_infos_question(question)
 
     assert résultat == {"avertissements": {},
                         'erreurs': {'tests': ['empty values not allowed'],
                                     'ébauches': ['empty values not allowed']}}
-
-def test_valider_question_vcs_minimale():
-    from question_vcs_minimale import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements": {}, "erreurs": {}}
-
-def test_valider_question_vsc_sans_champ_vcs():
-    from question_vcs_sans_champ_vcs import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements": {}, "erreurs": {'vcs': ['required field']}}
-
-def test_valider_question_vsc_avec_champ_vcs_null():
-    from question_vcs_avec_champ_vcs_null import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements": {}, "erreurs": {'vcs': ['null value not allowed']}}
-    
-def test_valider_question_vsc_avec_champ_vcs_vide():
-    from question_vcs_avec_champ_vcs_vide import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-    print (résultat)
-    assert résultat == {'erreurs': {'vcs': ['empty values not allowed']}, 'avertissements': {}}
-
-def test_valider_question_bd_sans_sgbd():
-    from question_bd_sans_sgbd import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements":{},
-                        'erreurs': {'sgbd': ['required field']}}
-
-def test_valider_question_bd_avec_sgbd_vide():
-    from question_bd_avec_sgbd_vide import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements":{}, "erreurs": {'sgbd': ['empty values not allowed']}}
-
-def test_valider_question_bd_avec_sgbd_valide():
-    from question_bd_avec_sgbd_valide import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements":{}, "erreurs":{}}
-
-def test_valider_question_bd_avec_sgbd_null():
-    from question_bd_avec_sgbd_null import question
-
-    résultat = progression_qc.valider_schema_yaml_infos_question(question)
-
-    assert résultat == {"avertissements":{}, "erreurs": {"sgbd": ["null value not allowed"]}}
```


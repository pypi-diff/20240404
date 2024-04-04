# Comparing `tmp/mahdi_env-0.0.0.tar.gz` & `tmp/mahdi_env-0.0.1.tar.gz`

## Comparing `mahdi_env-0.0.0.tar` & `mahdi_env-0.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/.gitattributes
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/src/mahdi_env/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/src/mahdi_env/env.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/.gitignore
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/README.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 mahdi_env-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/.gitattributes
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/src/mahdi_env/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/src/mahdi_env/env.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/.gitignore
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/README.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 mahdi_env-0.0.1/PKG-INFO
```

### Comparing `mahdi_env-0.0.0/.github/workflows/python-publish.yml` & `mahdi_env-0.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mahdi_env-0.0.0/src/mahdi_env/env.py` & `mahdi_env-0.0.1/src/mahdi_env/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,13 @@
     with subprocess.Popen(['sh'] ,
                           stdin = subprocess.PIPE ,
                           stdout = subprocess.PIPE) as p :
         result = p.communicate(script)
 
     for line in result[0].decode().splitlines() :
         var , _ , value = line.partition('=')
-        print(var , value)
         environ[var] = value
 
     if not 'DB' in environ :
         raise Exception('DB is not set')
 
     return dotsi.fy(dict(environ))
```

### Comparing `mahdi_env-0.0.0/.gitignore` & `mahdi_env-0.0.1/.gitignore`

 * *Files identical despite different names*


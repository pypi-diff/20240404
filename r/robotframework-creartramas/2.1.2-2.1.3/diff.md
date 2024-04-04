# Comparing `tmp/robotframework_creartramas-2.1.2.tar.gz` & `tmp/robotframework_creartramas-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.2.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.3.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.2.tar` & `robotframework_creartramas-2.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.2/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.2/LICENSE
--rw-r--r--   0        0        0      670 2024-04-04 06:48:24.827057 robotframework_creartramas-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.2/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2488 2024-04-04 06:48:08.907625 robotframework_creartramas-2.1.2/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.3/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.3/LICENSE
+-rw-r--r--   0        0        0      670 2024-04-04 07:58:59.260954 robotframework_creartramas-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.3/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2483 2024-04-04 07:58:38.538339 robotframework_creartramas-2.1.3/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.3/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.2/docs/README.md` & `robotframework_creartramas-2.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.2/LICENSE` & `robotframework_creartramas-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.2/pyproject.toml` & `robotframework_creartramas-2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.2"
+version = "2.1.3"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.2/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.3/TRAMAS/creartramas.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
         direccion_origen_hex = int(direccion_origen, 16)
         comando_hex = int(comando, 16)
         datos_hex = [int(dato, 16) for dato in datos]
 
          # Construye la trama en hexadecimal según la estructura proporcionada
         trama = " ".join([f"{direccion_destino_hex:02X}", f"{numero_bits_hex:02X}", f"{direccion_origen_hex:02X}", f"{comando_hex:02X}"]) 
         # Agregar cada elemento de la lista datos a la trama en formato hexadecimal
-        trama +=" " + " ".join([f"{datos_hex:02X}" for dato in datos_hex]) + " "
+        trama +=" " + " ".join([f"{dato:02X}" for dato in datos_hex]) + " "
         # Calcula el checksum de la trama
         checksum = calcular_checksum(trama)
         # Agrega el checksum a la trama
         trama += f"{checksum:02X}\n"  # Asegura que el checksum esté representado por dos caracteres hexadecimales
         return trama
```

### Comparing `robotframework_creartramas-2.1.2/PKG-INFO` & `robotframework_creartramas-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.2
+Version: 2.1.3
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


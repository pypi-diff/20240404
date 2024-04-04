# Comparing `tmp/robotframework_creartramas-2.1.0.tar.gz` & `tmp/robotframework_creartramas-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.0.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.2.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.0.tar` & `robotframework_creartramas-2.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.0/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.0/LICENSE
--rw-r--r--   0        0        0      670 2024-04-03 07:10:09.864255 robotframework_creartramas-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.0/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2133 2024-04-03 07:08:04.373140 robotframework_creartramas-2.1.0/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.2/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.2/LICENSE
+-rw-r--r--   0        0        0      670 2024-04-04 06:48:24.827057 robotframework_creartramas-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.2/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-04 06:48:08.907625 robotframework_creartramas-2.1.2/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.2/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.0/docs/README.md` & `robotframework_creartramas-2.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.0/LICENSE` & `robotframework_creartramas-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.0/pyproject.toml` & `robotframework_creartramas-2.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.0"
+version = "2.1.2"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.0/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.2/TRAMAS/creartramas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 class   TRAMAS:
     """
     Dicha Librería implementa diferentes funciones que permiten calcular el checksum
-    de una trama y crear una nueva trama, que posteriormente se podra enviar
+    de una trama y crear una nueva trama, que posteriormente se podrá enviar.
     """
     def __init__(self) -> None:
         pass
     def calcular_checksum(self,trama):
         """
         Esta función toma una trama en hexadecimal como entrada y calcula 
-        el checksum para esa trama. Devuelve el valor de checksum
+        el checksum para esa trama. Devuelve el valor del checksum.
         """
         # Convierto trama en hexadecimal a trama en bytes para sumarla
         trama_byte = bytes.fromhex(trama)
         # Suma todos los valores ASCII de los caracteres en la trama convertida
         check = sum(trama_byte)
         # Devuelve el checksum módulo 256, comprobando que si check > 256 , el cheksum es 256 menos la diferencia que hay entre ambos
         if check >= 256:
             checksum = 256 - (abs(256-check))
         else:
             checksum = abs(256-check)
         return checksum # valor absoluto por si checksum es mayor que 256
         
     def crear_trama(self,direccion_destino, numero_bits, direccion_origen, comando, datos):
         """
-        Esta funcion construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
+        Esta función construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
         Hay que tener en cuenta que los datos que se introducen deben estar en formate hexadecimal 0XAB.
         También a la hora de introducir datos, estso deben estar en forma de lista datos=[0x00,0x00,..]
         Finalmente, se devuelve la trama creada.
         """
-         # Construye la trama según la estructura proporcionada
-        trama = " ".join([f"{direccion_destino:02X}", f"{numero_bits:02X}", f"{direccion_origen:02X}", f"{comando:02X}"]) 
+        # Convertir los valores a hexadecimal
+        direccion_destino_hex = int(direccion_destino, 16)
+        numero_bits_hex = int(numero_bits, 16)
+        direccion_origen_hex = int(direccion_origen, 16)
+        comando_hex = int(comando, 16)
+        datos_hex = [int(dato, 16) for dato in datos]
+
+         # Construye la trama en hexadecimal según la estructura proporcionada
+        trama = " ".join([f"{direccion_destino_hex:02X}", f"{numero_bits_hex:02X}", f"{direccion_origen_hex:02X}", f"{comando_hex:02X}"]) 
         # Agregar cada elemento de la lista datos a la trama en formato hexadecimal
-        trama +=" " + " ".join([f"{dato:02X}" for dato in datos]) + " "
+        trama +=" " + " ".join([f"{datos_hex:02X}" for dato in datos_hex]) + " "
         # Calcula el checksum de la trama
         checksum = calcular_checksum(trama)
         # Agrega el checksum a la trama
         trama += f"{checksum:02X}\n"  # Asegura que el checksum esté representado por dos caracteres hexadecimales
         return trama
```

### Comparing `robotframework_creartramas-2.1.0/PKG-INFO` & `robotframework_creartramas-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.0
+Version: 2.1.2
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


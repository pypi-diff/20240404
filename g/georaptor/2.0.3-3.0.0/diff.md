# Comparing `tmp/georaptor-2.0.3.tar.gz` & `tmp/georaptor-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/georaptor-2.0.3.tar", last modified: Wed Jun  7 09:26:33 2017, max compression
+gzip compressed data, was "georaptor-3.0.0.tar", last modified: Thu Apr  4 05:51:15 2024, max compression
```

## Comparing `georaptor-2.0.3.tar` & `georaptor-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-07 09:26:33.000000 georaptor-2.0.3/
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/
--rw-r--r--   0 Ashwin     (501) staff       (20)        1 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/dependency_links.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)       48 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/entry_points.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)     3843 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/PKG-INFO
--rw-r--r--   0 Ashwin     (501) staff       (20)       15 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/requires.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)      262 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/SOURCES.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)       10 2017-06-07 09:26:33.000000 georaptor-2.0.3/georaptor.egg-info/top_level.txt
--rwxr-xr-x   0 Ashwin     (501) staff       (20)     4472 2017-06-07 06:49:22.000000 georaptor-2.0.3/georaptor.py
--rw-r--r--   0 Ashwin     (501) staff       (20)     3843 2017-06-07 09:26:33.000000 georaptor-2.0.3/PKG-INFO
--rw-r--r--   0 Ashwin     (501) staff       (20)     2517 2017-06-07 06:47:44.000000 georaptor-2.0.3/README.rst
--rw-r--r--   0 Ashwin     (501) staff       (20)      101 2017-06-07 09:26:33.000000 georaptor-2.0.3/setup.cfg
--rw-r--r--   0 Ashwin     (501) staff       (20)      964 2017-06-07 09:24:53.000000 georaptor-2.0.3/setup.py
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-07 09:26:33.000000 georaptor-2.0.3/test/
--rw-r--r--   0 Ashwin     (501) staff       (20)     1414 2017-06-07 06:48:26.000000 georaptor-2.0.3/test/test_raptor.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-04-04 05:51:15.036431 georaptor-3.0.0/
+-rw-r--r--   0 ashwin     (501) staff       (20)    11383 2023-12-01 16:15:31.000000 georaptor-3.0.0/LICENSE
+-rw-r--r--   0 ashwin     (501) staff       (20)     3113 2024-04-04 05:51:15.036390 georaptor-3.0.0/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)     2367 2024-04-04 05:37:02.000000 georaptor-3.0.0/README.rst
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-04-04 05:51:15.036092 georaptor-3.0.0/georaptor.egg-info/
+-rw-r--r--   0 ashwin     (501) staff       (20)     3113 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)      270 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/SOURCES.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)        1 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/dependency_links.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       45 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/entry_points.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       15 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/requires.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       10 2024-04-04 05:51:14.000000 georaptor-3.0.0/georaptor.egg-info/top_level.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)     4421 2024-04-04 05:20:04.000000 georaptor-3.0.0/georaptor.py
+-rw-r--r--   0 ashwin     (501) staff       (20)       80 2024-04-04 05:51:15.036589 georaptor-3.0.0/setup.cfg
+-rw-r--r--   0 ashwin     (501) staff       (20)      965 2024-04-04 05:33:02.000000 georaptor-3.0.0/setup.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-04-04 05:51:15.035823 georaptor-3.0.0/test/
+-rw-r--r--   0 ashwin     (501) staff       (20)     1414 2023-12-01 16:15:31.000000 georaptor-3.0.0/test/test_raptor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `georaptor-2.0.3/georaptor.egg-info/PKG-INFO` & `georaptor-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: georaptor
-Version: 2.0.3
+Version: 3.0.0
 Summary: A Python Geohash Compression Tool
 Home-page: https://github.com/ashwin711/georaptor
+Download-URL: https://github.com/ashwin711/georaptor/tarball/3.0.0
 Author: Ashwin Nair
 Author-email: ashwinnair.ua@gmail.com
 License: MIT
-Download-URL: https://github.com/ashwin711/georaptor/tarball/2.0.3
-Description: .. image:: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b.svg
-           :target: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b
-        
-        GeoRaptor: Python Geohash Compression Tool
-        ===========================================
-        
-        Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of what is known as a Z-order curve, and generally space-filling curves.
-        
-        Geohash creation for a polygon at a given precision level could result in a huge set of geohashes.
-        
-        **GeoRaptor** creates the best combination of geohashes across various levels to represent a polygon, by starting from the highest level and iterating till the optimal blend is brewed. Result accuracy remains the same as that of the starting geohash level, but data size reduces considerably for large polygons, thereby improving speed and performance.
-        
-        Following is a sample of what georaptor does
-        
-        .. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_input.png
-           :width: 480
-           :height: 320
-        .. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_output.png
-           :width: 480
-           :height: 320
-        
-        
-        *Input:* 1096 geohashes at precision 6 for Singapore.
-        
-        *Output:* 414 geohashes with a mix of precision 5 and 6.
-        
-        Performance
-        -----------
-        
-        **Input sample size:** 18,992,425
-        
-        **Output:** 220,375
-        
-        **Total execution time:** 35.8013219833 seconds
-        
-        Usage
-        -----
-        
-        $ georaptor <input> --output <output> --minlevel <minlevel> --maxlevel <maxlevel>
-        
-        
-        Example
-        -------
-        
-        $ georaptor sample.csv
-        
-        OR
-        
-        $ georaptor sample.csv --output sample_out.csv --minlevel 3 --maxlevel 4
-        
-        
-        Installation
-        ------------
-        
-        To install georaptor, simply: ::
-        
-            $ pip install georaptor
-        
-        
-        License:
-        --------
-        
-        
-        Licensed under the Apache License, Version 2.0. ::
-        
-            Copyright 2017 Ashwin Nair <https://www.linkedin.com/in/nairashwin7>
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
 Keywords: geohash,optimizer,compression,location
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+License-File: LICENSE
+Requires-Dist: clint
+Requires-Dist: argparse
+
+GeoRaptor: Python Geohash Compression Tool
+===========================================
+
+Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of what is known as a Z-order curve, and generally space-filling curves.
+
+Geohash creation for a polygon at a given precision level could result in a huge set of geohashes.
+
+**GeoRaptor** creates the best combination of geohashes across various levels to represent a polygon, by starting from the highest level and iterating till the optimal blend is brewed. Result accuracy remains the same as that of the starting geohash level, but data size reduces considerably for large polygons, thereby improving speed and performance.
+
+Following is a sample of what georaptor does
+
+.. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_input.png
+   :width: 480
+   :height: 320
+.. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_output.png
+   :width: 480
+   :height: 320
+
+
+*Input:* 1096 geohashes at precision 6 for Singapore.
+
+*Output:* 414 geohashes with a mix of precision 5 and 6.
+
+Performance
+-----------
+
+**Input sample size:** 18,992,425
+
+**Output:** 220,375
+
+**Total execution time:** 35.8013219833 seconds
+
+Usage
+-----
+
+$ georaptor <input> --output <output> --minlevel <minlevel> --maxlevel <maxlevel>
+
+
+Example
+-------
+
+$ georaptor sample.csv
+
+OR
+
+$ georaptor sample.csv --output sample_out.csv --minlevel 3 --maxlevel 4
+
+
+Installation
+------------
+
+To install georaptor, simply: ::
+
+    $ pip install georaptor
+
+
+License:
+--------
+
+
+Licensed under the Apache License, Version 2.0. ::
+
+    Copyright 2024 Ashwin Nair <https://www.linkedin.com/in/ashwin-nair7>
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `georaptor-2.0.3/georaptor.py` & `georaptor-3.0.0/georaptor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,149 +1,128 @@
-#!/usr/bin/python
+#!/usr/bin/python3
 
 import time
 import argparse
 from clint.textui import puts, indent, colored
 
-
 def read_file(filename):
     # Read file by lines into a set
     with open(filename) as f:
         geohashes = set(f.read().splitlines())
-
     return geohashes
 
-
 # Combination generator for a given geohash at the next level
 def get_combinations(string):
     base32 = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'j', 'k', 'm',
               'n', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
     return [string + '{0}'.format(i) for i in base32]
 
-
 # Recursive optimization of the geohash set
 def compress(geohashes, minlevel, maxlevel):
     deletegh = set()
     final_geohashes = set()
     flag = True
     final_geohashes_size = 0
-    
+
     # Input size less than 32
     if len(geohashes) == 0:
         puts(colored.red('No geohashes found!\n'))
         return False
 
-
-    while flag == True:
-
+    while flag:
         final_geohashes.clear()
         deletegh.clear()
 
         for geohash in geohashes:
-
             geohash_length = len(geohash)
 
             # Compress only if geohash length is greater than the min level
             if geohash_length >= minlevel:
                 # Get geohash to generate combinations for
                 part = geohash[:-1]
 
                 # Proceed only if not already processed
                 if part not in deletegh and geohash not in deletegh:
-
                     # Generate combinations
                     combinations = set(get_combinations(part))
 
                     # If all generated combinations exist in the input set
                     if combinations.issubset(geohashes):
                         # Add part to temporary output
                         final_geohashes.add(part)
                         # Add part to deleted geohash set
                         deletegh.add(part)
 
                     # Else add the geohash to the temp out and deleted set
                     else:
-
                         deletegh.add(geohash)
 
                         # Forced compression if geohash length is greater than max level after combination check failure
                         if geohash_length >= maxlevel:
                             final_geohashes.add(geohash[:maxlevel])
                         else:
                             final_geohashes.add(geohash)
 
                     # Break if compressed output size same as the last iteration
                     if final_geohashes_size == len(final_geohashes):
                         flag = False
 
         final_geohashes_size = len(final_geohashes)
-
         geohashes.clear()
 
         # Temp output moved to the primary geohash set
         geohashes = geohashes.union(final_geohashes)
 
     return geohashes
 
-
 def main():
-
     start_time = time.time()
     output_file = 'output.csv'
     minlevel = 1
     maxlevel = 12
 
     # Fetch input arguments
     parser = argparse.ArgumentParser()
     parser.add_argument('input', help='input filename containing list of geohashes')
     parser.add_argument('--output', default='output.csv',
                         help='output filename containing a optimized list of geohashes (default: output.csv)')
-    parser.add_argument('--minlevel', default=1,
+    parser.add_argument('--minlevel', type=int, default=1,
                         help='minimum level of geohash (default: 1)')
-    parser.add_argument('--maxlevel', default=12,
+    parser.add_argument('--maxlevel', type=int, default=12,
                         help='maximum level of geohash  (default: 12)')
 
     args = parser.parse_args()
 
     filename = args.input
-
-    if 'output' in args:
-        output_file  = args.output
-
-    if 'minlevel' in args:
-        minlevel = args.minlevel
-
-    if 'maxlevel' in args:
-        maxlevel = args.maxlevel
-
-    fp = open(output_file, "a");
+    output_file = args.output
+    minlevel = args.minlevel
+    maxlevel = args.maxlevel
 
     puts(colored.green('\nReading the file'))
 
     geohashes = read_file(filename)
 
     puts(colored.green(str("{:,}".format(len(geohashes))) + ' geohashes read\n'))
 
-    time.sleep(1);
+    time.sleep(1)
 
     puts(colored.red('Starting compression\n'))
 
-    georaptor_out = compress(geohashes, int(minlevel), int(maxlevel))
+    georaptor_out = compress(geohashes, minlevel, maxlevel)
 
     puts(colored.red('Compressed to: ' + str("{:,}".format(len(georaptor_out)))))
 
     if georaptor_out != False:
-
         # Output to file
-        for geohash in georaptor_out:
-            fp.write(geohash+'\n')
+        with open(output_file, 'a') as fp:
+            for geohash in georaptor_out:
+                fp.write(geohash + '\n')
 
         puts(colored.red('\nCompression complete!'))
-
         time.sleep(1)
-
         puts(colored.white('\nOutput available at ' + output_file + '\n'))
 
-
     et = time.time() - start_time
+    puts(colored.green('Total execution time: ' + str(et) + ' seconds\n'))
 
-    puts(colored.green('Total execution time: '+str(et)+' seconds\n'))
+if __name__ == "__main__":
+    main()
```

### Comparing `georaptor-2.0.3/PKG-INFO` & `georaptor-3.0.0/georaptor.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: georaptor
-Version: 2.0.3
+Version: 3.0.0
 Summary: A Python Geohash Compression Tool
 Home-page: https://github.com/ashwin711/georaptor
+Download-URL: https://github.com/ashwin711/georaptor/tarball/3.0.0
 Author: Ashwin Nair
 Author-email: ashwinnair.ua@gmail.com
 License: MIT
-Download-URL: https://github.com/ashwin711/georaptor/tarball/2.0.3
-Description: .. image:: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b.svg
-           :target: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b
-        
-        GeoRaptor: Python Geohash Compression Tool
-        ===========================================
-        
-        Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of what is known as a Z-order curve, and generally space-filling curves.
-        
-        Geohash creation for a polygon at a given precision level could result in a huge set of geohashes.
-        
-        **GeoRaptor** creates the best combination of geohashes across various levels to represent a polygon, by starting from the highest level and iterating till the optimal blend is brewed. Result accuracy remains the same as that of the starting geohash level, but data size reduces considerably for large polygons, thereby improving speed and performance.
-        
-        Following is a sample of what georaptor does
-        
-        .. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_input.png
-           :width: 480
-           :height: 320
-        .. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_output.png
-           :width: 480
-           :height: 320
-        
-        
-        *Input:* 1096 geohashes at precision 6 for Singapore.
-        
-        *Output:* 414 geohashes with a mix of precision 5 and 6.
-        
-        Performance
-        -----------
-        
-        **Input sample size:** 18,992,425
-        
-        **Output:** 220,375
-        
-        **Total execution time:** 35.8013219833 seconds
-        
-        Usage
-        -----
-        
-        $ georaptor <input> --output <output> --minlevel <minlevel> --maxlevel <maxlevel>
-        
-        
-        Example
-        -------
-        
-        $ georaptor sample.csv
-        
-        OR
-        
-        $ georaptor sample.csv --output sample_out.csv --minlevel 3 --maxlevel 4
-        
-        
-        Installation
-        ------------
-        
-        To install georaptor, simply: ::
-        
-            $ pip install georaptor
-        
-        
-        License:
-        --------
-        
-        
-        Licensed under the Apache License, Version 2.0. ::
-        
-            Copyright 2017 Ashwin Nair <https://www.linkedin.com/in/nairashwin7>
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
 Keywords: geohash,optimizer,compression,location
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+License-File: LICENSE
+Requires-Dist: clint
+Requires-Dist: argparse
+
+GeoRaptor: Python Geohash Compression Tool
+===========================================
+
+Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of what is known as a Z-order curve, and generally space-filling curves.
+
+Geohash creation for a polygon at a given precision level could result in a huge set of geohashes.
+
+**GeoRaptor** creates the best combination of geohashes across various levels to represent a polygon, by starting from the highest level and iterating till the optimal blend is brewed. Result accuracy remains the same as that of the starting geohash level, but data size reduces considerably for large polygons, thereby improving speed and performance.
+
+Following is a sample of what georaptor does
+
+.. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_input.png
+   :width: 480
+   :height: 320
+.. image:: https://raw.github.com/ashwin711/georaptor/master/images/sgp_output.png
+   :width: 480
+   :height: 320
+
+
+*Input:* 1096 geohashes at precision 6 for Singapore.
+
+*Output:* 414 geohashes with a mix of precision 5 and 6.
+
+Performance
+-----------
+
+**Input sample size:** 18,992,425
+
+**Output:** 220,375
+
+**Total execution time:** 35.8013219833 seconds
+
+Usage
+-----
+
+$ georaptor <input> --output <output> --minlevel <minlevel> --maxlevel <maxlevel>
+
+
+Example
+-------
+
+$ georaptor sample.csv
+
+OR
+
+$ georaptor sample.csv --output sample_out.csv --minlevel 3 --maxlevel 4
+
+
+Installation
+------------
+
+To install georaptor, simply: ::
+
+    $ pip install georaptor
+
+
+License:
+--------
+
+
+Licensed under the Apache License, Version 2.0. ::
+
+    Copyright 2024 Ashwin Nair <https://www.linkedin.com/in/ashwin-nair7>
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `georaptor-2.0.3/README.rst` & `georaptor-3.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.. image:: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b.svg
-   :target: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b
-
 GeoRaptor: Python Geohash Compression Tool
 ===========================================
 
 Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of what is known as a Z-order curve, and generally space-filling curves.
 
 Geohash creation for a polygon at a given precision level could result in a huge set of geohashes.
 
@@ -59,20 +56,20 @@
 
 License:
 --------
 
 
 Licensed under the Apache License, Version 2.0. ::
 
-    Copyright 2017 Ashwin Nair <https://www.linkedin.com/in/nairashwin7>
+    Copyright 2024 Ashwin Nair <https://www.linkedin.com/in/ashwin-nair7>
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `georaptor-2.0.3/setup.py` & `georaptor-3.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 import setuptools
 
 setup(
   name = 'georaptor',
   py_modules = ['georaptor'],
-  version = '2.0.3',
+  version = '3.0.0',
   description = 'A Python Geohash Compression Tool',
   long_description = open('README.rst').read(),
   author = 'Ashwin Nair',
   author_email = 'ashwinnair.ua@gmail.com',
   license = "MIT",
   url = 'https://github.com/ashwin711/georaptor',
-  download_url = 'https://github.com/ashwin711/georaptor/tarball/2.0.3',
+  download_url = 'https://github.com/ashwin711/georaptor/tarball/3.0.0',
   keywords = ['geohash', 'optimizer', 'compression', 'location'],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
@@ -26,8 +26,8 @@
 	'clint',
 	'argparse'
   ],
   entry_points='''
 	[console_scripts]
 	georaptor=georaptor:main
   '''
-)
+)
```

### Comparing `georaptor-2.0.3/test/test_raptor.py` & `georaptor-3.0.0/test/test_raptor.py`

 * *Files identical despite different names*


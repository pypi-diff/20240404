# Comparing `tmp/automation_tools-1.0.3.tar.gz` & `tmp/automation_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/automation_tools-1.0.3.tar", last modified: Thu Feb 29 20:51:42 2024, max compression
+gzip compressed data, was "dist/automation_tools-1.0.4.tar", last modified: Thu Apr  4 05:21:32 2024, max compression
```

## Comparing `automation_tools-1.0.3.tar` & `automation_tools-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-02-29 20:51:42.070264 automation_tools-1.0.3/
--rw-r--r--   0 sporty     (501) staff       (20)        0 2024-02-29 20:50:12.000000 automation_tools-1.0.3/LICENSE
--rw-r--r--   0 sporty     (501) staff       (20)     2124 2024-02-29 20:51:42.070047 automation_tools-1.0.3/PKG-INFO
--rw-r--r--   0 sporty     (501) staff       (20)     1773 2024-02-29 19:33:55.000000 automation_tools-1.0.3/README.md
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-02-29 20:51:42.069085 automation_tools-1.0.3/automation_tools/
--rw-r--r--   0 sporty     (501) staff       (20)       14 2024-02-29 20:27:09.000000 automation_tools-1.0.3/automation_tools/__init__.py
--rw-r--r--   0 sporty     (501) staff       (20)     4757 2024-02-29 20:12:22.000000 automation_tools-1.0.3/automation_tools/excel_to_csv_converter.py
-drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-02-29 20:51:42.069831 automation_tools-1.0.3/automation_tools.egg-info/
--rw-r--r--   0 sporty     (501) staff       (20)     2124 2024-02-29 20:51:42.000000 automation_tools-1.0.3/automation_tools.egg-info/PKG-INFO
--rw-r--r--   0 sporty     (501) staff       (20)      297 2024-02-29 20:51:42.000000 automation_tools-1.0.3/automation_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sporty     (501) staff       (20)        1 2024-02-29 20:51:42.000000 automation_tools-1.0.3/automation_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sporty     (501) staff       (20)        9 2024-02-29 20:51:42.000000 automation_tools-1.0.3/automation_tools.egg-info/requires.txt
--rw-r--r--   0 sporty     (501) staff       (20)       17 2024-02-29 20:51:42.000000 automation_tools-1.0.3/automation_tools.egg-info/top_level.txt
--rw-r--r--   0 sporty     (501) staff       (20)       38 2024-02-29 20:51:42.070308 automation_tools-1.0.3/setup.cfg
--rw-r--r--   0 sporty     (501) staff       (20)      524 2024-02-29 20:49:04.000000 automation_tools-1.0.3/setup.py
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:21:32.599050 automation_tools-1.0.4/
+-rw-r--r--   0 sporty     (501) staff       (20)        0 2024-02-29 20:50:12.000000 automation_tools-1.0.4/LICENSE
+-rw-r--r--   0 sporty     (501) staff       (20)     2459 2024-04-04 05:21:32.598830 automation_tools-1.0.4/PKG-INFO
+-rw-r--r--   0 sporty     (501) staff       (20)     2108 2024-04-04 05:01:22.000000 automation_tools-1.0.4/README.md
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:21:32.597859 automation_tools-1.0.4/automation_tools/
+-rw-r--r--   0 sporty     (501) staff       (20)       14 2024-02-29 20:27:09.000000 automation_tools-1.0.4/automation_tools/__init__.py
+-rw-r--r--   0 sporty     (501) staff       (20)     4757 2024-02-29 20:12:22.000000 automation_tools-1.0.4/automation_tools/excel_to_csv_converter.py
+drwxr-xr-x   0 sporty     (501) staff       (20)        0 2024-04-04 05:21:32.598631 automation_tools-1.0.4/automation_tools.egg-info/
+-rw-r--r--   0 sporty     (501) staff       (20)     2459 2024-04-04 05:21:32.000000 automation_tools-1.0.4/automation_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sporty     (501) staff       (20)      297 2024-04-04 05:21:32.000000 automation_tools-1.0.4/automation_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sporty     (501) staff       (20)        1 2024-04-04 05:21:32.000000 automation_tools-1.0.4/automation_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sporty     (501) staff       (20)        9 2024-04-04 05:21:32.000000 automation_tools-1.0.4/automation_tools.egg-info/requires.txt
+-rw-r--r--   0 sporty     (501) staff       (20)       17 2024-04-04 05:21:32.000000 automation_tools-1.0.4/automation_tools.egg-info/top_level.txt
+-rw-r--r--   0 sporty     (501) staff       (20)       38 2024-04-04 05:21:32.599094 automation_tools-1.0.4/setup.cfg
+-rw-r--r--   0 sporty     (501) staff       (20)      528 2024-04-04 05:15:08.000000 automation_tools-1.0.4/setup.py
```

### Comparing `automation_tools-1.0.3/PKG-INFO` & `automation_tools-1.0.4/automation_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 Metadata-Version: 2.1
-Name: automation_tools
-Version: 1.0.3
+Name: automation-tools
+Version: 1.0.4
 Summary: A suite of automation tools for various tasks.
 Home-page: https://github.com/sportyomar/automation_tools
 Author: Omar Lydale Morrison
 Author-email: omar.morrison@sportyventures.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openpyxl
 
-Excel to CSV Converter
+# Excel to CSV Converter
 The Excel to CSV Converter is a Python script that allows you to convert Excel files (.xlsx) into CSV (Comma-Separated Values) format. It provides a graphical user interface (GUI) built with Tkinter for easy file selection and conversion.
 
-Features
-Convert multiple Excel files into CSV format simultaneously.
-Graphical user interface (GUI) for intuitive operation.
-Displays sheet names of loaded Excel files.
-Handles error cases gracefully with informative error messages.
-Dependencies
-Python 3.x
-openpyxl (Python library for reading and writing Excel files)
-Installation
-Make sure you have Python 3.x installed on your system. If not, download and install it from python.org.
-Install the required Python library using pip:
-pip install openpyxl
-Usage
-Clone the repository or download the source code.
-Navigate to the project directory in your terminal.
-Run the script using Python:
-python excel_to_csv_converter.py
-Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
-Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
-Click on "Convert to CSV" to start the conversion process.
-Once the conversion is complete, the script will display the number of CSV files generated.
-Examples
-# Example usage of the ExcelToCsvConverter class
+### Features
+* Convert multiple Excel files into CSV format simultaneously. 
+* Graphical user interface (GUI) for intuitive operation.
+* Displays sheet names of loaded Excel files.
+* Handles error cases gracefully with informative error messages.
+### Dependencies
+* Python 3.x
+* openpyxl (Python library for reading and writing Excel files)
 
+### Installation
+* Make sure you have Python 3.x installed on your system. (If not, download and install it from python.org).
+* Install the required Python library using pip:
+  * pip install openpyxl
+  
+
+### Usage
+  1. Clone the repository or download the source code.
+  2. Navigate to the project directory in your terminal.
+  3. Run the script using Python:
+     * python excel_to_csv_converter.py
+     * Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
+     * Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
+     * Click on "Convert to CSV" to start the conversion process.
+       * Once the conversion is complete, the script will display the number of CSV files generated.
+       
+### Quickstart
+
+```python
 import tkinter as tk
-from excel_to_csv_converter import ExcelToCsvConverter
+from automation_tools.excel_to_csv_converter import ExcelToCsvConverter
+
+
+def main():
+    root = tk.Tk()
+    root.title("Excel to CSV Converter")
+
+    app = ExcelToCsvConverter(root)
+
+    root.mainloop()
 
-root = tk.Tk()
-app = ExcelToCsvConverter(root)
-root.mainloop()
-How to Contribute
+
+if __name__ == "__main__":
+    main()
+```
+
+The code produces the following graphical user interface for converting Excel files to csv files.
+
+![Alt text](image.png)
+
+### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
-License
+
+### License
 This project is licensed under the MIT License.
```

### Comparing `automation_tools-1.0.3/README.md` & `automation_tools-1.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,61 @@
-Excel to CSV Converter
+# Excel to CSV Converter
 The Excel to CSV Converter is a Python script that allows you to convert Excel files (.xlsx) into CSV (Comma-Separated Values) format. It provides a graphical user interface (GUI) built with Tkinter for easy file selection and conversion.
 
-Features
-Convert multiple Excel files into CSV format simultaneously.
-Graphical user interface (GUI) for intuitive operation.
-Displays sheet names of loaded Excel files.
-Handles error cases gracefully with informative error messages.
-Dependencies
-Python 3.x
-openpyxl (Python library for reading and writing Excel files)
-Installation
-Make sure you have Python 3.x installed on your system. If not, download and install it from python.org.
-Install the required Python library using pip:
-pip install openpyxl
-Usage
-Clone the repository or download the source code.
-Navigate to the project directory in your terminal.
-Run the script using Python:
-python excel_to_csv_converter.py
-Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
-Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
-Click on "Convert to CSV" to start the conversion process.
-Once the conversion is complete, the script will display the number of CSV files generated.
-Examples
-# Example usage of the ExcelToCsvConverter class
+### Features
+* Convert multiple Excel files into CSV format simultaneously. 
+* Graphical user interface (GUI) for intuitive operation.
+* Displays sheet names of loaded Excel files.
+* Handles error cases gracefully with informative error messages.
+### Dependencies
+* Python 3.x
+* openpyxl (Python library for reading and writing Excel files)
 
+### Installation
+* Make sure you have Python 3.x installed on your system. (If not, download and install it from python.org).
+* Install the required Python library using pip:
+  * pip install openpyxl
+  
+
+### Usage
+  1. Clone the repository or download the source code.
+  2. Navigate to the project directory in your terminal.
+  3. Run the script using Python:
+     * python excel_to_csv_converter.py
+     * Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
+     * Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
+     * Click on "Convert to CSV" to start the conversion process.
+       * Once the conversion is complete, the script will display the number of CSV files generated.
+       
+### Quickstart
+
+```python
 import tkinter as tk
-from excel_to_csv_converter import ExcelToCsvConverter
+from automation_tools.excel_to_csv_converter import ExcelToCsvConverter
+
+
+def main():
+    root = tk.Tk()
+    root.title("Excel to CSV Converter")
+
+    app = ExcelToCsvConverter(root)
+
+    root.mainloop()
 
-root = tk.Tk()
-app = ExcelToCsvConverter(root)
-root.mainloop()
-How to Contribute
+
+if __name__ == "__main__":
+    main()
+```
+
+The code produces the following graphical user interface for converting Excel files to csv files.
+
+![Alt text](image.png)
+
+### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
-License
+
+### License
 This project is licensed under the MIT License.
```

### Comparing `automation_tools-1.0.3/automation_tools/excel_to_csv_converter.py` & `automation_tools-1.0.4/automation_tools/excel_to_csv_converter.py`

 * *Files identical despite different names*

### Comparing `automation_tools-1.0.3/automation_tools.egg-info/PKG-INFO` & `automation_tools-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 Metadata-Version: 2.1
-Name: automation-tools
-Version: 1.0.3
+Name: automation_tools
+Version: 1.0.4
 Summary: A suite of automation tools for various tasks.
 Home-page: https://github.com/sportyomar/automation_tools
 Author: Omar Lydale Morrison
 Author-email: omar.morrison@sportyventures.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openpyxl
 
-Excel to CSV Converter
+# Excel to CSV Converter
 The Excel to CSV Converter is a Python script that allows you to convert Excel files (.xlsx) into CSV (Comma-Separated Values) format. It provides a graphical user interface (GUI) built with Tkinter for easy file selection and conversion.
 
-Features
-Convert multiple Excel files into CSV format simultaneously.
-Graphical user interface (GUI) for intuitive operation.
-Displays sheet names of loaded Excel files.
-Handles error cases gracefully with informative error messages.
-Dependencies
-Python 3.x
-openpyxl (Python library for reading and writing Excel files)
-Installation
-Make sure you have Python 3.x installed on your system. If not, download and install it from python.org.
-Install the required Python library using pip:
-pip install openpyxl
-Usage
-Clone the repository or download the source code.
-Navigate to the project directory in your terminal.
-Run the script using Python:
-python excel_to_csv_converter.py
-Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
-Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
-Click on "Convert to CSV" to start the conversion process.
-Once the conversion is complete, the script will display the number of CSV files generated.
-Examples
-# Example usage of the ExcelToCsvConverter class
+### Features
+* Convert multiple Excel files into CSV format simultaneously. 
+* Graphical user interface (GUI) for intuitive operation.
+* Displays sheet names of loaded Excel files.
+* Handles error cases gracefully with informative error messages.
+### Dependencies
+* Python 3.x
+* openpyxl (Python library for reading and writing Excel files)
 
+### Installation
+* Make sure you have Python 3.x installed on your system. (If not, download and install it from python.org).
+* Install the required Python library using pip:
+  * pip install openpyxl
+  
+
+### Usage
+  1. Clone the repository or download the source code.
+  2. Navigate to the project directory in your terminal.
+  3. Run the script using Python:
+     * python excel_to_csv_converter.py
+     * Click on "Load XLSX Files" to select one or more Excel files (.xlsx) you want to convert.
+     * Click on "Select Output Directory" to choose the directory where you want to save the converted CSV files.
+     * Click on "Convert to CSV" to start the conversion process.
+       * Once the conversion is complete, the script will display the number of CSV files generated.
+       
+### Quickstart
+
+```python
 import tkinter as tk
-from excel_to_csv_converter import ExcelToCsvConverter
+from automation_tools.excel_to_csv_converter import ExcelToCsvConverter
+
+
+def main():
+    root = tk.Tk()
+    root.title("Excel to CSV Converter")
+
+    app = ExcelToCsvConverter(root)
+
+    root.mainloop()
 
-root = tk.Tk()
-app = ExcelToCsvConverter(root)
-root.mainloop()
-How to Contribute
+
+if __name__ == "__main__":
+    main()
+```
+
+The code produces the following graphical user interface for converting Excel files to csv files.
+
+![Alt text](image.png)
+
+### How to Contribute
 Contributions to improve Excel to CSV Converter are welcome! Here's how you can contribute:
 
 Fork the repository.
 Make your changes and enhancements.
 Submit a pull request with a clear description of your changes.
-License
+
+### License
 This project is licensed under the MIT License.
```

### Comparing `automation_tools-1.0.3/setup.py` & `automation_tools-1.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='automation_tools',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     install_requires=[
         'openpyxl',
     ],
     author='Omar Lydale Morrison',
     author_email='omar.morrison@sportyventures.com',
     description='A suite of automation tools for various tasks.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sportyomar/automation_tools',
     license='MIT',
 )
+
+
+
+
```


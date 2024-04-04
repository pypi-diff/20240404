# Comparing `tmp/generic_configuration_builder-1.2.1.tar.gz` & `tmp/generic_configuration_builder-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "generic_configuration_builder-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `generic_configuration_builder-1.2.1.tar` & `generic_configuration_builder-1.2.2.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/.gitattributes
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/src/generic_configuration_builder/__init__.py
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/src/generic_configuration_builder/configuration_builder.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/LICENSE
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 generic_configuration_builder-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-03-28 14:08:56.553994 generic_configuration_builder-1.2.2/LICENSE
+-rw-r--r--   0        0        0     7197 2023-09-14 15:51:58.191307 generic_configuration_builder-1.2.2/README.md
+-rw-r--r--   0        0        0     1016 2024-04-04 10:27:39.385458 generic_configuration_builder-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-02-07 11:22:01.872881 generic_configuration_builder-1.2.2/src/generic_configuration_builder/__init__.py
+-rw-r--r--   0        0        0    15477 2024-04-04 09:58:56.444586 generic_configuration_builder-1.2.2/src/generic_configuration_builder/configuration_builder.py
+-rw-r--r--   0        0        0     8060 1970-01-01 00:00:00.000000 generic_configuration_builder-1.2.2/PKG-INFO
```

### Comparing `generic_configuration_builder-1.2.1/src/generic_configuration_builder/configuration_builder.py` & `generic_configuration_builder-1.2.2/src/generic_configuration_builder/configuration_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 import configparser
 from collections import OrderedDict
 import os
 import ast
 from typing import Union, Dict, Callable
 import re
+import warnings
 
-### Optional Imports
+# Optional Imports
 
 SPECIAL_TYPES = []
 
 try:
     import torch
     HAS_TORCH = True
     SPECIAL_TYPES.append(torch.tensor)
@@ -20,24 +21,24 @@
 try:
     import numpy as np
     HAS_NUMPY = True
     SPECIAL_TYPES.append(np.ndarray)
 except ImportError:
     HAS_NUMPY = False
 
-### Keywords
+# Keywords
 
 MODULE_MARKER = "~MODULE"
 CLASS_MARKER = "~CLASS"
 INSTANCE_INDICATOR = "*"
 RETURN_SECTION = "~RETURN"
 DEFAULT_SECTION = "~DEFAULT"
 RETURN_ATTRIBUTE = "RETURN"
 
-### Code
+# Code
 
 
 def gcb_build(configuration_path: str, **input_instances) -> Union[Dict[str, object], object]:
     """ Build class and dependencies construct according to configuration file.
 
     Args:
         configuration_path (str): Path to configuration file
@@ -54,63 +55,102 @@
 
     input_dict = OrderedDict(**input_instances)
 
     variables_dict = _load_defaults(configuration=configuration)
 
     variables_dict.update(input_dict)
 
-    _check_necessary_arguments(configuration=configuration, variables_dict=variables_dict)
+    used_variables = set()
+
+    _check_necessary_arguments(
+        configuration=configuration, variables_dict=variables_dict)
 
     for section in configuration.sections():
-        if(section == RETURN_SECTION):
-            return_variable_names = _parse_unmarked_string_list(configuration[RETURN_SECTION][RETURN_ATTRIBUTE])
+        if (section == RETURN_SECTION):
+            return_variable_names = _parse_unmarked_string_list(
+                configuration[RETURN_SECTION][RETURN_ATTRIBUTE])
             return_dict = {}
             for variable_name in return_variable_names:
-                return_dict[variable_name] = _get_attribute(argument_string=variable_name, variables_dict=variables_dict)
+                return_dict[variable_name] = _get_attribute(
+                    argument_string=variable_name, variables_dict=variables_dict)
+                used_variables.add(variable_name)
             return return_dict
 
         try:
             module_name = configuration[section].pop(MODULE_MARKER)
         except KeyError as key_error:
-            raise Exception(f'Instance "{section}" is missing the "{MODULE_MARKER}" keyword') from key_error
-        
+            raise Exception(
+                f'Instance "{section}" is missing the "{MODULE_MARKER}" keyword')
+
         try:
             class_name = configuration[section].pop(CLASS_MARKER)
         except KeyError as key_error:
-            raise Exception(f'Instance "{section}" is missing the "{CLASS_MARKER}" keyword') from key_error
-        
+            raise Exception(
+                f'Instance "{section}" is missing the "{CLASS_MARKER}" keyword')
+
         try:
-            instance = _initialize_class(module_name, class_name, configuration[section], variables_dict)
+            instance = _initialize_class(
+                module_name, class_name, configuration[section], variables_dict)
         except Exception as exception:
-            raise Exception(f'An error occurred while trying to initialize "{section}".') from exception
+            raise Exception(
+                f'An error occurred while trying to initialize "{section}".') from exception
         variables_dict[section] = instance
 
     return variables_dict.popitem()[1]
 
+
+def gcb_get_default_dictionary(configuration_path: str) -> Dict[str, object]:
+    """Returns the default dictionary that would be used to initialize the classes according to the configuration.
+
+    Args:
+        configuration_path (str): Path to the configuration file.
+
+    Returns:
+        Dict[str, object]: Dictionary of default values.
+    """
+    configuration = _read_configuration(configuration_path)
+    return dict(_load_defaults(configuration=configuration))
+
+
 def _check_necessary_arguments(configuration: list[str], variables_dict: Dict[str, object]) -> None:
     """Checks if all necessary keywords have been passed according to the configuration.
 
     Args:
         configuration (list[str]): The parsed ini configuration file.
         variables_dict (Dict[str, object]): All passed keyword arguments.
 
     Raises:
         Exception: This exception occurs if not all keyword arguments have been passed.
     """
+    defined_variables = set(variables_dict.keys())
+    used_variables = set()
+
     instances_so_far = []
     for section in configuration.sections():
         for arg_name, arg_string in configuration[section].items():
-            if(arg_string.startswith(INSTANCE_INDICATOR)):
-                instance_name = arg_string[len(INSTANCE_INDICATOR):].split(".")[0]
-                if not (instance_name in variables_dict or instance_name in instances_so_far):
-                    raise Exception(f'The given configuration expects to be given a value for the keyword "{instance_name}" ' +
+            matches = _match_instances(arg_string)
+            for match in matches:
+                variable_name = match[len(
+                    INSTANCE_INDICATOR):].split(".")[0]
+                used_variables.add(variable_name)
+            # if (arg_string.startswith(INSTANCE_INDICATOR)):
+            #     instance_name = arg_string[len(
+            #         INSTANCE_INDICATOR):].split(".")[0]
+                if not (variable_name in variables_dict or variable_name in instances_so_far):
+                    raise Exception(f'The given configuration expects to be given a value for the keyword "{variable_name}" ' +
                                     f'which is used as an argument for "{arg_name}" to initialize the instance "{section}". ' +
-                                    f'However this value is not passed. Please pass "{instance_name}" as a keyword to {gcb_build.__name__}.')
+                                    f'However this value is not passed. Please pass "{variable_name}" as a keyword to {gcb_build.__name__}.')
         instances_so_far.append(section)
 
+    unused_variables = defined_variables - used_variables
+    if len(unused_variables) > 0:
+        warnings.warn(
+            f'The following variables are defined but not used in the configuration: {unused_variables}')
+
+
 def _load_defaults(configuration: list[str]) -> Dict[str, object]:
     """Loads defaults values given in the configuration. These values may be overwritten with values passed to the gcb_build function.
 
     Args:
         configuration (list[str]): The parsed configuration.
 
     Raises:
@@ -121,38 +161,41 @@
     """
     variables_dict = OrderedDict()
     if DEFAULT_SECTION in configuration.sections():
         for arg_name, arg_string in configuration[DEFAULT_SECTION].items():
             try:
                 variables_dict[arg_name] = ast.literal_eval(arg_string)
             except Exception as exception:
-                raise Exception(f'An Error occurred while trying to parse the default value for "{arg_name}" in the "{DEFAULT_SECTION}" section'+
-                               f' of the document. The given value "{arg_string}" could not be parsed as a literal.') from exception          
+                raise Exception(f'An Error occurred while trying to parse the default value for "{arg_name}" in the "{DEFAULT_SECTION}" section' +
+                                f' of the document. The given value "{arg_string}" could not be parsed as a literal.') from exception
     configuration.pop(DEFAULT_SECTION, None)
     return variables_dict
 
+
 def _read_configuration(configuration_path: str) -> list[str]:
     """Read the ini configuration given the path.
 
     Args:
         configuration_path (str): Path to the configuration
 
     Raises:
         Exception: The file could not be found.
 
     Returns:
         list[str]: The parsed ini config.
     """
     absolute_configuration_path = os.path.abspath(configuration_path)
     if not os.path.isfile(absolute_configuration_path):
-        raise Exception(f'Configuration: {absolute_configuration_path} was not found.')
+        raise Exception(
+            f'Configuration: {absolute_configuration_path} was not found.')
     configuration = configparser.ConfigParser()
     configuration.read(absolute_configuration_path)
     return configuration
 
+
 def _initialize_class(module_name: str, class_name: str, init_args_string_dict: Dict[str, str], variables_dict: Dict[str, object]) -> object:
     """initialized a class given all information as strings
 
     Args:
         module_name (str): String that leads to the module of the class
         class_name (str): Name of the class
         init_args_string_dict (Dict[str, str]): Arguments of the __init__ function as strings with their according keywords.
@@ -162,45 +205,53 @@
         object: Initialized instance of class.
     """
     _class = _load_class(module_name, class_name)
 
     full_arg_spec = inspect.getfullargspec(_class.__init__)
 
     init_args = full_arg_spec.args
-    if "self" in init_args: init_args.remove("self")
+    if "self" in init_args:
+        init_args.remove("self")
     init_args_types = dict.fromkeys(init_args)
 
     annotations_dict = full_arg_spec.annotations
     annotations_dict.pop("return", None)
 
     init_args_types.update(annotations_dict)
 
     init_args_instances = {}
     for arg_name, arg_string in init_args_string_dict.items():
         if arg_name in init_args_types:
-            init_args_instances[arg_name] = _parse_value(string=arg_string, variables_dict=variables_dict, dtype=init_args_types[arg_name])
+            init_args_instances[arg_name] = _parse_value(
+                string=arg_string, variables_dict=variables_dict, dtype=init_args_types[arg_name])
         elif full_arg_spec.varkw != None:
-            init_args_instances[arg_name] = _parse_value(string=arg_string, variables_dict=variables_dict, dtype=None)
+            init_args_instances[arg_name] = _parse_value(
+                string=arg_string, variables_dict=variables_dict, dtype=None)
+        else:
+            raise Exception(
+                f'The initialization function of the class "{class_name}" does not accept a keyword argument of name "{arg_name}".')
 
     return _class(**init_args_instances)
 
+
 def _load_class(module_name: str, class_name: str) -> type:
     """Loads a class type given its location by strings.
 
     Args:
         module_name (str): String that leads to the module of the class
         class_name (str): Name of the class
 
     Returns:
         type: According python class type object
     """
-    module = __import__(module_name, fromlist = class_name)
+    module = __import__(module_name, fromlist=class_name)
     _class = getattr(module, class_name)
     return _class
 
+
 def _get_attribute(argument_string: str, variables_dict: Dict[str, object]) -> object:
     """Gets an attribute of an instance.
 
     Args:
         argument_string (str): String that describes path to the Attribute. E.g. "parent.child.subchild"
         variables_dict (Dict[str, object]): A dictionary of already initialized classes. This is where the attributes are in.
 
@@ -210,21 +261,23 @@
     Returns:
         object: Python object of the attribute
     """
     argument_attributes = argument_string.split(".")
     try:
         base_instance = variables_dict[argument_attributes[0]]
     except KeyError as key_error:
-        raise Exception(f'"{argument_attributes[0]}" has not been assigned a value yet.') from key_error
+        raise Exception(
+            f'"{argument_attributes[0]}" has not been assigned a value yet.')
     instance = base_instance
     for attribute_name in argument_attributes[1:]:
         instance = getattr(instance, attribute_name)
 
     return instance
 
+
 def _parse_value(string: str, variables_dict: Dict[str, any], dtype: type = None) -> any:
     """Parse Python base datatypes from a string.
 
     Args:
         dtype (type): type to cast to.
         variables_dict (Dict[str, any]):  Dictionary of already initialized classes.
         string (str): String to cast.
@@ -236,57 +289,74 @@
         object: Parsed string as Python object
     """
     try:
         if dtype != None and dtype in SPECIAL_TYPES:
             parse_function = _parse_function_of(dtype=dtype)
             return parse_function(string)
         else:
-            parsed = _parse_literal_with_instance_markers(value_string = string, variables_dict = variables_dict)
+            parsed = _parse_literal_with_instance_markers(
+                value_string=string, variables_dict=variables_dict)
     except Exception as error:
-        raise Exception(f"Error while trying to parse: {string}") from error
+        raise Exception(
+            f'An error occurred while trying to parse the string "{string}" as a value.') from error
     return parsed
 
+
 def _parse_function_of(dtype: type) -> Callable:
     """Returns function to parse a string to dtype.
     Args:
         dtype (type): Type for which the parse function is needed.
     Returns:
         Callable: According parse function
     """
-    if( HAS_TORCH and dtype == torch.Tensor):
+    if (HAS_TORCH and dtype == torch.Tensor):
         return _parse_torch_tensor
-    if( HAS_NUMPY and dtype == np.ndarray):
+    if (HAS_NUMPY and dtype == np.ndarray):
         return _parse_numpy_array
 
-    raise Exception(f'No special parse function implemented for dtype: "{dtype}"')
+    raise Exception(
+        f'No special parse function implemented for dtype "{dtype}".')
+
+
+def _match_instances(string: str) -> list[str]:
+    """Matches all instances in a string.
+
+    Args:
+        string (str): String to match
+
+    Returns:
+        list[str]: List of strings that represent instances.
+    """
+    regex = f'([{INSTANCE_INDICATOR}][\w.]+)'
+    prog = re.compile(regex)
+    return re.findall(prog, string)
+
 
 def _parse_literal_with_instance_markers(value_string: str, variables_dict: Dict[str, any]) -> any:
     """Parses a string to a python object. 
     If string contain INSTANCE_INDICATOR than replace that string with the according instance.
 
     Args:
         value_string (str): String to parse
         variables_dict (Dict[str, any]): Already initialized instances.
 
     Returns:
         any: _description_
     """
-      
-    regex = f'([{INSTANCE_INDICATOR}][\w.]+)'
-    prog = re.compile(regex)
-    matches = re.findall(prog, value_string)
+
+    matches = _match_instances(value_string)
     if len(matches) == 0:
         return ast.literal_eval(value_string)
     else:
         for match in set(matches):
             value_string = value_string.replace(match, f"'{match}'")
 
         parsed_with_placeholders = ast.literal_eval(value_string)
         return replace_strings(data=parsed_with_placeholders, to_replace=matches, variables_dict=variables_dict)
-        
+
 
 def replace_strings(data: any, to_replace: list[str], variables_dict: Dict[str, any]) -> any:
     """Recursively iterates over a nested collection and replaces strings 
         that are part of to_replace with instances.
 
     Args:
         data (any): A construct of nested collections containing list, tuples and dictionaries
@@ -304,55 +374,55 @@
     elif isinstance(data, dict):
         return {replace_strings(key, to_replace, variables_dict): replace_strings(value, to_replace, variables_dict) for key, value in data.items()}
     elif isinstance(data, str):
         if data in to_replace:
             return _get_attribute(argument_string=data[len(INSTANCE_INDICATOR):], variables_dict=variables_dict)
     return data
 
+
 def _parse_unmarked_string_list(list_string: str) -> list[str]:
     """ Converts a string that represents a list without INSTANCE_INDICATOR to a list of strings. 
         Each entry is assumed to be a variable.
 
     Args:
         list_string (str): String that represents a list.
 
     Returns:
         list[str]: List of strings where each string represents an instance.
     """
     list_string = list_string[1:-1].split(",")
     list_string = list(map(lambda item: item.strip(" "), list_string))
     return list_string
 
+
 def _parse_torch_tensor(tensor_string: str) -> object:
     """Parses a string to a torch tensor.
 
     Args:
         tensor_string (str): String to parse
 
     Returns:
         torch.Tensor: Parsed tensor
     """
-    if(tensor_string.startswith("tensor")):
+    if (tensor_string.startswith("tensor")):
         tensor_string = tensor_string[7:-1]
 
     parsed_list = ast.literal_eval(tensor_string)
     tensor = torch.tensor(parsed_list, dtype=torch.float32)
     return tensor
 
+
 def _parse_numpy_array(array_string: str) -> object:
     """Parses a string to a numpy array.
 
     Args:
         array_string (str): String to parse
 
     Returns:
         np.ndarray: Parsed array
     """
-    if(array_string.startswith("array")):
+    if (array_string.startswith("array")):
         tensor_string = array_string[6:-1]
 
     parsed_list = ast.literal_eval(tensor_string)
     array = np.array(parsed_list, dtype=np.float32)
     return array
-
-
-
```

### Comparing `generic_configuration_builder-1.2.1/LICENSE` & `generic_configuration_builder-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `generic_configuration_builder-1.2.1/README.md` & `generic_configuration_builder-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `generic_configuration_builder-1.2.1/pyproject.toml` & `generic_configuration_builder-1.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "generic_configuration_builder"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Sebastian Griesbach", email="sebastian.griesbach@zoho.eu" },
 ]
 description = "A simple library for parsing a configuration file format which is intended to build dependencies and hold parameters - well suited for experimentaton settings in which different experiments use different clases."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `generic_configuration_builder-1.2.1/PKG-INFO` & `generic_configuration_builder-1.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,21 @@
 Metadata-Version: 2.1
 Name: generic_configuration_builder
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple library for parsing a configuration file format which is intended to build dependencies and hold parameters - well suited for experimentaton settings in which different experiments use different clases.
-Project-URL: Homepage, https://github.com/Sebastian-Griesbach/Generic-Configuration-Builder
-Project-URL: Bug Tracker, https://github.com/Sebastian-Griesbach/Generic-Configuration-Builder/issues
+Keywords: configuration,config,experiment,dependencies,setup,parameters
 Author-email: Sebastian Griesbach <sebastian.griesbach@zoho.eu>
-License: MIT License
-        
-        Copyright (c) 2022 Sebastian Griesbach
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-License-File: LICENSE
-Keywords: config,configuration,dependencies,experiment,parameters,setup
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
 Requires-Dist: configparser
-Description-Content-Type: text/markdown
+Project-URL: Bug Tracker, https://github.com/Sebastian-Griesbach/Generic-Configuration-Builder/issues
+Project-URL: Homepage, https://github.com/Sebastian-Griesbach/Generic-Configuration-Builder
 
 # Generic-Configuration-Builder
 This library intends to help separate the setup and execution of experiments. If you need a bunch of different main classes to store the setup of your experiments, then this tiny library can help!
 The library parses a file format that can be used to set up any kind of class dependencies including all parameters, while also leaving the option to input additional parameters into the setup.
 
 ## Installation
 ```
@@ -211,7 +189,8 @@
     'parent_instance': <classes.ParentClass object at 0x7fd91416ec50>,
     'parent_instance.combined_string': 'blub3.141'
 }
 ```
 Which now can be used in whatever way these objects are intended to be used.
 
 Some extensive examples using a complex class structure can be found [here](https://github.com/Sebastian-Griesbach/Improving-Policy-Conditioned-Value-Functions/tree/main/experiments).
+
```


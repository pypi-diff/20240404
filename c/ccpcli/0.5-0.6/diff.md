# Comparing `tmp/ccpcli-0.5.tar.gz` & `tmp/ccpcli-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpcli-0.5.tar", last modified: Thu Apr  4 07:57:27 2024, max compression
+gzip compressed data, was "ccpcli-0.6.tar", last modified: Thu Apr  4 16:21:48 2024, max compression
```

## Comparing `ccpcli-0.5.tar` & `ccpcli-0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 07:57:27.884288 ccpcli-0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/ccpcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:57:27.884288 ccpcli-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-04 07:57:16.000000 ccpcli-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-04 07:57:16.000000 ccpcli-0.5/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-04 07:57:16.000000 ccpcli-0.5/src/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/resource_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/service/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/compute/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/security_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/service/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/volume/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/http_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 16:21:48.756492 ccpcli-0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/ccpcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.752493 ccpcli-0.6/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:21:48.760492 ccpcli-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-04 16:21:36.000000 ccpcli-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.752493 ccpcli-0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-04 16:21:36.000000 ccpcli-0.6/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-04 16:21:36.000000 ccpcli-0.6/src/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/resource_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/compute/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/security_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/volume/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/http_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/utils.py
```

### Comparing `ccpcli-0.5/ccpcli.egg-info/SOURCES.txt` & `ccpcli-0.6/ccpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/setup.py` & `ccpcli-0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='ccpcli',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     author='Mani Keshari',
     author_email='mani@coredge.io',
     description='CCP cli',
     install_requires=['click', 'halo', 'tabulate'],
     entry_points={
         'console_scripts': [
```

### Comparing `ccpcli-0.5/src/cli.py` & `ccpcli-0.6/src/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import urllib3
 from click import echo
 from click import style
 from src.project import project
 from src.service.network.network import networks
 from src.service.volume.volume import volumes
 from src.service.network.security_group import security_groups
-from src.service.compute.instance import instances
+from src.service.compute.instance import instances, flavors, images
 from src.util.constants import Constants, HttpStatus, YntraaCreds
 from src.util.http_helper import get_assert
 from src.util.utils import print_error, convert_unix_timestamp
 from src.util.utils import print_info
 from src.util.utils import save_context, clear_context
 
 urllib3.disable_warnings()
@@ -161,7 +161,9 @@
 
 # Add commands to the cli group
 cli.add_command(project)
 cli.add_command(networks)
 cli.add_command(volumes)
 cli.add_command(security_groups)
 cli.add_command(instances)
+cli.add_command(flavors)
+cli.add_command(images)
```

### Comparing `ccpcli-0.5/src/project.py` & `ccpcli-0.6/src/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/resource_schemas/network.py` & `ccpcli-0.6/src/resource_schemas/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/resource_schemas/project.py` & `ccpcli-0.6/src/resource_schemas/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/resource_schemas/volume.py` & `ccpcli-0.6/src/resource_schemas/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/service/compute/instance.py` & `ccpcli-0.6/src/service/volume/volume.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,79 @@
 ###############################################################################
 # Copyright (c) 2024-present CorEdge India Pvt. Ltd - All Rights Reserved     #
 # Unauthorized copying of this file, via any medium is strictly prohibited    #
 # Proprietary and confidential                                                #
-# Written by Mani Keshari <mani@coredge.io>, April 2024                       #
+# Written by Deepak Pant <deepakpant@coredge.io>, April 2023                  #
+# Modified by Aman Kadhala <aman@coredge.io>, April 2023                      #
 ###############################################################################
 import os
 
 import click
 from src.util.constants import Constants
+from src.util.http_helper import delete_assert
 from src.util.http_helper import get_assert
-from src.util.utils import print_cli
+from src.util.utils import print_cli, print_info
 from src.util.utils import set_context
-from src.resource_schemas.compute import instance_list_response
+from src.resource_schemas.volume import volume_list_response
 
 
-@click.group(name=Constants.COMMAND_GROUP_INSTANCE)
+@click.group(name=Constants.COMMAND_GROUP_VOLUME)
 @click.pass_context
-def instances(ctx):
-    """This command will do all the operations on instances"""
+def volumes(ctx):
+    """This command will do all the operations on volumes"""
     pass
 
 
-@instances.command(name=Constants.COMMAND_GET)
+@volumes.command(name=Constants.COMMAND_GET)
 @click.pass_context
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def get_instance(ctx, output):
-    """This command will provide the list of Instances"""
+def get_volume(ctx, output):
+    """This command will provide the list of Volume"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes/'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes'
+    params = {'include_bootable': False}
 
-    res = get_assert(ctx, url=url)
+    res = get_assert(ctx, url=url, params=params)
 
     if output == Constants.TABULAR_OUTPUT:
-        instance_list = instance_list_response(res)
+        volumes = volume_list_response(res)
     else:
-        instance_list = res
-    print_cli(msg=instance_list, output_format=output, headers=Constants.INSTANCE_TABLE_HEADERS)
+        volumes = res
+
+    print_cli(msg=volumes, output_format=output,
+              headers=Constants.TABLE_HEADER_VOLUME)
 
 
-@instances.command(name=Constants.COMMAND_DESCRIBE)
+@volumes.command(name=Constants.COMMAND_DESCRIBE)
 @click.pass_context
-@click.argument('instance')
+@click.argument('volume')
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def describe_instance(ctx, instance, output):
-    """This command will describe instance"""
+def describe_volume(ctx, volume, output):
+    """This command will describe volume"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes{os.sep}{instance}'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
     res = get_assert(ctx, url=url)
 
     print_cli(msg=[res], output_format=output)
+
+
+@volumes.command(name=Constants.COMMAND_DELETE)
+@click.pass_context
+@click.argument('volume')
+def delete_volume(ctx, volume):
+    """This command will delete network"""
+
+    # set up the configuration details into ctx object
+    set_context(ctx)
+
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
+
+    delete_assert(ctx, url=url, expected_response_code=202)
+
+    print_info("Volume deleting in progress.")
+
```

### Comparing `ccpcli-0.5/src/service/network/network.py` & `ccpcli-0.6/src/service/network/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/service/network/security_group.py` & `ccpcli-0.6/src/service/network/security_group.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/service/volume/volume.py` & `ccpcli-0.6/src/service/compute/instance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,107 @@
 ###############################################################################
 # Copyright (c) 2024-present CorEdge India Pvt. Ltd - All Rights Reserved     #
 # Unauthorized copying of this file, via any medium is strictly prohibited    #
 # Proprietary and confidential                                                #
-# Written by Deepak Pant <deepakpant@coredge.io>, April 2023                  #
-# Modified by Aman Kadhala <aman@coredge.io>, April 2023                      #
+# Written by Mani Keshari <mani@coredge.io>, April 2024                       #
 ###############################################################################
 import os
 
 import click
 from src.util.constants import Constants
-from src.util.http_helper import delete_assert
 from src.util.http_helper import get_assert
-from src.util.utils import print_cli, print_info
+from src.util.utils import print_cli
 from src.util.utils import set_context
-from src.resource_schemas.volume import volume_list_response
+from src.resource_schemas.compute import instance_list_response, flavors_list_response, images_list_response
 
 
-@click.group(name=Constants.COMMAND_GROUP_VOLUME)
+@click.group(name=Constants.COMMAND_GROUP_INSTANCE)
 @click.pass_context
-def volumes(ctx):
-    """This command will do all the operations on volumes"""
+def instances(ctx):
+    """This command will do all the operations on instances"""
     pass
 
 
-@volumes.command(name=Constants.COMMAND_GET)
+@instances.command(name=Constants.COMMAND_GET)
 @click.pass_context
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def get_volume(ctx, output):
-    """This command will provide the list of Volume"""
+def get_instance(ctx, output):
+    """This command will provide the list of Instances"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes'
-    params = {'include_bootable': False}
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes/'
 
-    res = get_assert(ctx, url=url, params=params)
+    res = get_assert(ctx, url=url)
 
     if output == Constants.TABULAR_OUTPUT:
-        volumes = volume_list_response(res)
+        instance_list = instance_list_response(res)
     else:
-        volumes = res
-
-    print_cli(msg=volumes, output_format=output,
-              headers=Constants.TABLE_HEADER_VOLUME)
+        instance_list = res
+    print_cli(msg=instance_list, output_format=output, headers=Constants.INSTANCE_TABLE_HEADERS)
 
 
-@volumes.command(name=Constants.COMMAND_DESCRIBE)
+@instances.command(name=Constants.COMMAND_DESCRIBE)
 @click.pass_context
-@click.argument('volume')
+@click.argument('instance')
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def describe_volume(ctx, volume, output):
-    """This command will describe volume"""
+def describe_instance(ctx, instance, output):
+    """This command will describe instance"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes{os.sep}{instance}'
     res = get_assert(ctx, url=url)
 
     print_cli(msg=[res], output_format=output)
 
 
-@volumes.command(name=Constants.COMMAND_DELETE)
+@click.group()
 @click.pass_context
-@click.argument('volume')
-def delete_volume(ctx, volume):
-    """This command will delete network"""
+def flavors(ctx):
+    """This command will do all the operations on flavours"""
+    pass
+
+
+@flavors.command(name=Constants.COMMAND_GET)
+@click.pass_context
+@click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
+def get_flavors(ctx, output):
+    """This will list flavors"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes{os.sep}flavors/'
+    res = get_assert(ctx, url=url)
+    if output == Constants.TABULAR_OUTPUT:
+        flavors_list = flavors_list_response(res)
+    else:
+        flavors_list = res
+    print_cli(msg=flavors_list, output_format=output, headers=Constants.FLAVOUR_TABLE_HEADERS)
+
+
+@click.group()
+@click.pass_context
+def images(ctx):
+    """This command will do all the operations on flavours"""
+    pass
 
-    delete_assert(ctx, url=url, expected_response_code=202)
 
-    print_info("Volume deleting in progress.")
+@images.command(name=Constants.COMMAND_GET)
+@click.pass_context
+@click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
+def get_images(ctx, output):
+    """This will list images"""
 
+    # set up the configuration details into ctx object
+    set_context(ctx)
+
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}computes{os.sep}images/'
+    res = get_assert(ctx, url=url)
+    if output == Constants.TABULAR_OUTPUT:
+        images_list = images_list_response(res)
+    else:
+        images_list = res
+    print_cli(msg=images_list, output_format=output, headers=Constants.IMAGE_TABLE_HEADERS)
```

### Comparing `ccpcli-0.5/src/util/constants.py` & `ccpcli-0.6/src/util/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,14 +91,22 @@
     SECURITY_GROUP_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "SECURITY_GROUP_NAME") + [
         "TYPE", "MANAGED_BY", "LAST_UPDATED_AT"]
 
     # Instance Table Headers
     INSTANCE_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "INSTANCE_NAME") + [
         "ACTION", "PRIVATE_IP", "PUBLIC_IP", "UPDATED_AT" ]
 
+    # Flavors Table Headers
+    FLAVOUR_TABLE_HEADERS = ["ID", "NAME", "RAM(MB)", "VCPUS", "FLAVOR_GROUP", "HOURLY_PRICE(INR)", "MONTHLY_PRICE("
+                                                                                                    "INR)"]
+
+    # Images Table Headers
+    IMAGE_TABLE_HEADERS = ["ID", "NAME",  "DISTRIBUTION", "IMAGE_TYPE", "OS", "OS_VERSION", "OS_ARCHITECTURE",
+                            "MONTHLY_PRICE(INR)", "HOURLY_PRICE(INR)"]
+
     TABLE_HEADER_INSTANCE = ["ID", "NAME", " PUBLIC_V4", "AVAILABILITY_ZONE", "STATUS", "TAGS",
                              "CREATED_BY", "CREATED_AT"]
 
     # properties = read_properties(ENV_DEV_FILE_PATH)
     GRANT_TYPE = 'password'
 
     # Cloud CLI Group Command
@@ -120,14 +128,19 @@
     COMMAND_CREATE = 'create'
     COMMAND_DELETE = 'delete'
     COMMAND_CURRENT = 'current'
     COMMAND_SWITCH_PROJECT = 'switch-project'
     COMMAND_SET_DEFAULT_PROJECT = 'set-default-project'
 
 
+    # Billing unit
+    HOURLY_BILLING_UNIT = "HRC"
+    MONTHLY_BILLING_UNIT = "MRC"
+
+
 class HttpStatus:
     # Status Codes
     OK: int = 200
     CREATED: int = 201
     BAD_REQUEST: int = 400
     UNAUTHORIZED: int = 401
     NO_CONTENT: int = 204
```

### Comparing `ccpcli-0.5/src/util/file_utils.py` & `ccpcli-0.6/src/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/util/http_helper.py` & `ccpcli-0.6/src/util/http_helper.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.5/src/util/utils.py` & `ccpcli-0.6/src/util/utils.py`

 * *Files identical despite different names*


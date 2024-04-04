# Comparing `tmp/ccpcli-0.4.tar.gz` & `tmp/ccpcli-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpcli-0.4.tar", last modified: Wed Apr  3 08:12:14 2024, max compression
+gzip compressed data, was "ccpcli-0.5.tar", last modified: Thu Apr  4 07:57:27 2024, max compression
```

## Comparing `ccpcli-0.4.tar` & `ccpcli-0.5.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.858460 ccpcli-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 08:12:14.858460 ccpcli-0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.858460 ccpcli-0.4/ccpcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 08:12:14.000000 ccpcli-0.4/ccpcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:12:14.858460 ccpcli-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 08:11:58.000000 ccpcli-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-03 08:11:58.000000 ccpcli-0.4/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-03 08:11:58.000000 ccpcli-0.4/src/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/src/resource_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/resource_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-03 08:11:58.000000 ccpcli-0.4/src/resource_schemas/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 08:11:58.000000 ccpcli-0.4/src/resource_schemas/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-03 08:11:58.000000 ccpcli-0.4/src/resource_schemas/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/src/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/src/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/network/security_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.854460 ccpcli-0.4/src/service/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-03 08:11:58.000000 ccpcli-0.4/src/service/volume/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:12:14.858460 ccpcli-0.4/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:11:58.000000 ccpcli-0.4/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-03 08:11:58.000000 ccpcli-0.4/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 08:11:58.000000 ccpcli-0.4/src/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 08:11:58.000000 ccpcli-0.4/src/util/http_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-03 08:11:58.000000 ccpcli-0.4/src/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 07:57:27.884288 ccpcli-0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/ccpcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 07:57:27.000000 ccpcli-0.5/ccpcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:57:27.884288 ccpcli-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-04 07:57:16.000000 ccpcli-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-04 07:57:16.000000 ccpcli-0.5/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-04 07:57:16.000000 ccpcli-0.5/src/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/resource_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-04 07:57:16.000000 ccpcli-0.5/src/resource_schemas/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.880288 ccpcli-0.5/src/service/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/compute/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/network/security_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/service/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 07:57:16.000000 ccpcli-0.5/src/service/volume/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:27.884288 ccpcli-0.5/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/http_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-04 07:57:16.000000 ccpcli-0.5/src/util/utils.py
```

### Comparing `ccpcli-0.4/ccpcli.egg-info/SOURCES.txt` & `ccpcli-0.5/ccpcli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 ccpcli.egg-info/requires.txt
 ccpcli.egg-info/top_level.txt
 resources/__init__.py
 src/__init__.py
 src/cli.py
 src/project.py
 src/resource_schemas/__init__.py
+src/resource_schemas/compute.py
 src/resource_schemas/network.py
 src/resource_schemas/project.py
 src/resource_schemas/volume.py
 src/service/__init__.py
+src/service/compute/__init__.py
+src/service/compute/instance.py
 src/service/network/__init__.py
 src/service/network/network.py
 src/service/network/security_group.py
 src/service/volume/__init__.py
 src/service/volume/volume.py
 src/util/__init__.py
 src/util/constants.py
```

### Comparing `ccpcli-0.4/setup.py` & `ccpcli-0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='ccpcli',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     author='Mani Keshari',
     author_email='mani@coredge.io',
     description='CCP cli',
     install_requires=['click', 'halo', 'tabulate'],
     entry_points={
         'console_scripts': [
```

### Comparing `ccpcli-0.4/src/cli.py` & `ccpcli-0.5/src/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import urllib3
 from click import echo
 from click import style
 from src.project import project
 from src.service.network.network import networks
 from src.service.volume.volume import volumes
 from src.service.network.security_group import security_groups
+from src.service.compute.instance import instances
 from src.util.constants import Constants, HttpStatus, YntraaCreds
 from src.util.http_helper import get_assert
 from src.util.utils import print_error, convert_unix_timestamp
 from src.util.utils import print_info
 from src.util.utils import save_context, clear_context
 
 urllib3.disable_warnings()
@@ -159,7 +160,8 @@
 
 
 # Add commands to the cli group
 cli.add_command(project)
 cli.add_command(networks)
 cli.add_command(volumes)
 cli.add_command(security_groups)
+cli.add_command(instances)
```

### Comparing `ccpcli-0.4/src/project.py` & `ccpcli-0.5/src/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/resource_schemas/network.py` & `ccpcli-0.5/src/resource_schemas/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/resource_schemas/project.py` & `ccpcli-0.5/src/resource_schemas/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/resource_schemas/volume.py` & `ccpcli-0.5/src/resource_schemas/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/service/network/network.py` & `ccpcli-0.5/src/service/volume/volume.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 ###############################################################################
 # Copyright (c) 2024-present CorEdge India Pvt. Ltd - All Rights Reserved     #
 # Unauthorized copying of this file, via any medium is strictly prohibited    #
 # Proprietary and confidential                                                #
-# Written by Mani Keshari <mani@coredge.io>, March 2024                       #
+# Written by Deepak Pant <deepakpant@coredge.io>, April 2023                  #
+# Modified by Aman Kadhala <aman@coredge.io>, April 2023                      #
 ###############################################################################
 import os
 
 import click
 from src.util.constants import Constants
 from src.util.http_helper import delete_assert
 from src.util.http_helper import get_assert
 from src.util.utils import print_cli, print_info
 from src.util.utils import set_context
-from src.resource_schemas.network import network_list_response, network_describe_response
+from src.resource_schemas.volume import volume_list_response
 
 
-@click.group(name=Constants.COMMAND_GROUP_NETWORK)
+@click.group(name=Constants.COMMAND_GROUP_VOLUME)
 @click.pass_context
-def networks(ctx):
-    """This command will do all the operations on networks"""
+def volumes(ctx):
+    """This command will do all the operations on volumes"""
     pass
 
 
-@networks.command(name=Constants.COMMAND_GET)
+@volumes.command(name=Constants.COMMAND_GET)
 @click.pass_context
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def get_network(ctx, output):
-    """This command will provide the list of Network"""
+def get_volume(ctx, output):
+    """This command will provide the list of Volume"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    params = {'external': False}
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}networks'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes'
+    params = {'include_bootable': False}
+
     res = get_assert(ctx, url=url, params=params)
 
     if output == Constants.TABULAR_OUTPUT:
-        network_list = network_list_response(res)
+        volumes = volume_list_response(res)
     else:
-        network_list = res
-    print_cli(msg=network_list, output_format=output, headers=Constants.TABLE_HEADER_NETWORKS)
+        volumes = res
+
+    print_cli(msg=volumes, output_format=output,
+              headers=Constants.TABLE_HEADER_VOLUME)
 
 
-@networks.command(name=Constants.COMMAND_DESCRIBE)
+@volumes.command(name=Constants.COMMAND_DESCRIBE)
 @click.pass_context
-@click.argument('network')
+@click.argument('volume')
 @click.option('--output', '-o', help='Supported formats are json,tabular,yaml', required=False)
-def describe_network(ctx, network, output):
-    """This command will describe network"""
+def describe_volume(ctx, volume, output):
+    """This command will describe volume"""
+
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}networks{os.sep}{network}/'
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
     res = get_assert(ctx, url=url)
 
-    if output == Constants.TABULAR_OUTPUT:
-        network_get = network_describe_response(res)
-    else:
-        network_get = res
-    print_cli(msg=[network_get], output_format=output, headers=Constants.TABLE_HEADER_NETWORK_DESCRIBE)
+    print_cli(msg=[res], output_format=output)
 
 
-@networks.command(name=Constants.COMMAND_DELETE)
+@volumes.command(name=Constants.COMMAND_DELETE)
 @click.pass_context
-@click.argument('network')
-def delete_network(ctx, network):
-    """This command will delete instance"""
+@click.argument('volume')
+def delete_volume(ctx, volume):
+    """This command will delete network"""
 
     # set up the configuration details into ctx object
     set_context(ctx)
 
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}networks{os.sep}{network}/'
-
-    delete_assert(ctx, url=url, expected_response_code=200)
+    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
 
-    print_info(msg="Network deleted successfully")
+    delete_assert(ctx, url=url, expected_response_code=202)
 
+    print_info("Volume deleting in progress.")
```

### Comparing `ccpcli-0.4/src/service/network/security_group.py` & `ccpcli-0.5/src/service/network/security_group.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/service/volume/volume.py` & `ccpcli-0.5/src/service/compute/instance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,57 @@
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
+from src.resource_schemas.compute import instance_list_response
 
 
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
-
-
-@volumes.command(name=Constants.COMMAND_DELETE)
-@click.pass_context
-@click.argument('volume')
-def delete_volume(ctx, volume):
-    """This command will delete network"""
-
-    # set up the configuration details into ctx object
-    set_context(ctx)
-
-    url = f'{ctx.obj.get(Constants.CLOUD_BASE_URL)}{os.sep}volumes{os.sep}{volume}/'
-
-    delete_assert(ctx, url=url, expected_response_code=202)
-
-    print_info("Volume deleting in progress.")
-
```

### Comparing `ccpcli-0.4/src/util/constants.py` & `ccpcli-0.5/src/util/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     # Volume Table Headers
     TABLE_HEADER_VOLUME = replace_field(COMMON_TABLE_HEADERS, "NAME", "VOLUME_NAME") + ["VOLUME_TYPE"]
 
     # Security Group Table Headers
     SECURITY_GROUP_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "SECURITY_GROUP_NAME") + [
         "TYPE", "MANAGED_BY", "LAST_UPDATED_AT"]
 
-
+    # Instance Table Headers
+    INSTANCE_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "INSTANCE_NAME") + [
+        "ACTION", "PRIVATE_IP", "PUBLIC_IP", "UPDATED_AT" ]
 
     TABLE_HEADER_INSTANCE = ["ID", "NAME", " PUBLIC_V4", "AVAILABILITY_ZONE", "STATUS", "TAGS",
                              "CREATED_BY", "CREATED_AT"]
 
     # properties = read_properties(ENV_DEV_FILE_PATH)
     GRANT_TYPE = 'password'
```

### Comparing `ccpcli-0.4/src/util/file_utils.py` & `ccpcli-0.5/src/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.4/src/util/http_helper.py` & `ccpcli-0.5/src/util/http_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from halo import Halo
 from src.util.constants import Constants
 from src.util.utils import print_error
 
 CONNECTION_TIMEOUT_IN_SEC = 300
 
 
-def populate_headers(ctx):
+def populate_headers(ctx, content_type=None):
     # Read the default user creds from the context
 
     headers = {
-        Constants.CONTENT_TYPE: Constants.APPLICATION_JSON_TYPE,
+        Constants.CONTENT_TYPE: Constants.APPLICATION_FORM_TYPE if content_type is None else content_type,
     }
 
     access_token = ctx.obj.get(Constants.ACCESS_TOKEN)
     org_id = str(ctx.obj.get(Constants.ORG_ID))
     project_id = str(ctx.obj.get(Constants.PROJECT_ID))
 
     if access_token:
@@ -31,25 +31,27 @@
         print_error(f"You are either not logged in or logged out out already.")
         raise click.exceptions.Exit()
 
     if project_id:
         headers[Constants.PROJECT_ID] = project_id
     if org_id:
         headers[Constants.ORG_ID] = org_id
+
     return headers
 
 
-def call_assert(ctx, method, url, expected_response_code, headers=None, data=None, json=None, params=None):
+def call_assert(ctx, method, url, expected_response_code, headers=None, data=None, json=None, params=None,
+                content_type=None):
     _spinner = Halo(text='Loading...', spinner='dots',
                     text_color='green', color='blue')
     _spinner.start()
     try:
         if not headers:
             # auto-populate headers based on context values
-            headers = populate_headers(ctx)
+            headers = populate_headers(ctx, content_type)
 
         response = requests.request(method=method, url=url, headers=headers, verify=False,
                                     timeout=CONNECTION_TIMEOUT_IN_SEC, data=data, json=json, params=params)
 
         if expected_response_code == response.status_code:
             if response.text:
                 return response.json()
@@ -61,29 +63,29 @@
     except Exception as e:
         print_error(str(e))
         raise click.exceptions.Exit()
     finally:
         _spinner.stop()
 
 
-def get_assert(ctx, url, headers=None, params=None, expected_response_code=200):
+def get_assert(ctx, url, headers=None, params=None, expected_response_code=200, content_type=None):
     return call_assert(ctx, 'get', url=url, headers=headers, params=params,
-                       expected_response_code=expected_response_code)
+                       expected_response_code=expected_response_code, content_type=content_type)
 
 
-def post_assert(ctx, url, headers=None, data=None, json=None, expected_response_code=201):
+def post_assert(ctx, url, headers=None, data=None, json=None, expected_response_code=201, content_type=None):
 
     return call_assert(ctx, 'post', url=url, headers=headers, data=data, json=json,
-                       expected_response_code=expected_response_code)
+                       expected_response_code=expected_response_code, content_type=content_type)
 
 
 def put_assert():
     pass
 
 
-def patch_assert(ctx, url, headers=None, expected_response_code=200):
-    return call_assert(ctx, 'patch', url=url, headers=headers, expected_response_code=expected_response_code)
+def patch_assert(ctx, url, headers=None, expected_response_code=200, content_type=None):
+    return call_assert(ctx, 'patch', url=url, headers=headers, expected_response_code=expected_response_code, content_type=content_type)
 
 
+def delete_assert(ctx, url, headers=None, expected_response_code=204, content_type=None):
+    return call_assert(ctx, 'delete', url=url, headers=headers, expected_response_code=expected_response_code, content_type=content_type)
 
-def delete_assert(ctx, url, headers=None, expected_response_code=204):
-    return call_assert(ctx, 'delete', url=url, headers=headers, expected_response_code=expected_response_code)
```

### Comparing `ccpcli-0.4/src/util/utils.py` & `ccpcli-0.5/src/util/utils.py`

 * *Files identical despite different names*


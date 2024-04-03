# Comparing `tmp/smpmgr-0.5.0.tar.gz` & `tmp/smpmgr-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpmgr-0.5.0.tar", max compression
+gzip compressed data, was "smpmgr-0.6.0.tar", max compression
```

## Comparing `smpmgr-0.5.0.tar` & `smpmgr-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    11366 2024-03-11 23:05:00.769865 smpmgr-0.5.0/LICENSE
--rw-r--r--   0        0        0     2556 2024-03-11 23:05:00.769865 smpmgr-0.5.0/README.md
--rw-r--r--   0        0        0     1083 2024-03-11 23:05:00.769865 smpmgr-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/__init__.py
--rw-r--r--   0        0        0       92 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/__main__.py
--rw-r--r--   0        0        0     3705 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/common.py
--rw-r--r--   0        0        0     3531 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/image_management.py
--rw-r--r--   0        0        0     3373 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/logging.py
--rw-r--r--   0        0        0     5190 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/main.py
--rw-r--r--   0        0        0     1086 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/os_management.py
--rw-r--r--   0        0        0        0 2024-03-11 23:05:00.769865 smpmgr-0.5.0/smpmgr/py.typed
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 smpmgr-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11366 2024-04-03 23:41:22.394472 smpmgr-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2556 2024-04-03 23:41:22.394472 smpmgr-0.6.0/README.md
+-rw-r--r--   0        0        0     1083 2024-04-03 23:41:22.394472 smpmgr-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/__main__.py
+-rw-r--r--   0        0        0     4041 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/common.py
+-rw-r--r--   0        0        0     3531 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/image_management.py
+-rw-r--r--   0        0        0     3373 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/logging.py
+-rw-r--r--   0        0        0     5257 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/main.py
+-rw-r--r--   0        0        0     1086 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/os_management.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/py.typed
+-rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/user/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/user/intercreate.py
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 smpmgr-0.6.0/PKG-INFO
```

### Comparing `smpmgr-0.5.0/LICENSE` & `smpmgr-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpmgr-0.5.0/README.md` & `smpmgr-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `smpmgr-0.5.0/pyproject.toml` & `smpmgr-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 smpmgr = "smpmgr.main:app"
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
-smpclient = "^1.0.1"
+smpclient = "^1.3.1"
 typer = {extras = ["all"], version = "^0.9.0"}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 black = "^23.11.0"
```

### Comparing `smpmgr-0.5.0/smpmgr/common.py` & `smpmgr-0.6.0/smpmgr/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 """Common CLI helpers from rich, typer, click, etc."""
 
 import asyncio
 import logging
 from dataclasses import dataclass, fields
+from typing import Type, TypeVar
 
 import typer
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from serial import SerialException
 from smp.exceptions import SMPBadStartDelimiter
 from smpclient import SMPClient
 from smpclient.generics import SMPRequest, TEr0, TEr1, TErr, TRep
 from smpclient.transport.serial import SMPSerialTransport
 
 logger = logging.getLogger(__name__)
 
+TSMPClient = TypeVar(
+    "TSMPClient",
+    bound=SMPClient,
+)
+
 
 @dataclass(frozen=True)
 class TransportDefinition:
     port: str | None
 
 
 @dataclass(frozen=True)
 class Options:
     timeout: float
     transport: TransportDefinition
     mtu: int
 
 
-def get_smpclient(options: Options) -> SMPClient:
-    """Return an `SMPClient` to the chosen transport or raise `typer.Exit`."""
+def get_custom_smpclient(options: Options, smp_client_cls: Type[TSMPClient]) -> TSMPClient:
+    """Return an `SMPClient` subclass to the chosen transport or raise `typer.Exit`."""
     if options.transport.port is not None:
         logger.info(
             f"Initializing SMPClient with the SMPSerialTransport, {options.transport.port=}"
         )
-        return SMPClient(SMPSerialTransport(mtu=options.mtu), options.transport.port)
+        return smp_client_cls(SMPSerialTransport(mtu=options.mtu), options.transport.port)
     else:
         typer.echo(
             f"A transport option is required; "
             f"one of [{', '.join(map(lambda x: '--' + x.name, fields(options.transport)))}]."
         )
         typer.echo("See smpmgr --help.")
         raise typer.Exit(code=1)
 
 
+def get_smpclient(options: Options) -> SMPClient:
+    """Return an `SMPClient` to the chosen transport or raise `typer.Exit`."""
+    return get_custom_smpclient(options, SMPClient)
+
+
 async def connect_with_spinner(smpclient: SMPClient) -> None:
     """Spin while connecting to the SMP Server; raises `typer.Exit` if connection fails."""
     with Progress(
         SpinnerColumn(), TextColumn("[progress.description]{task.description}")
     ) as progress:
         connect_task_description = f"Connecting to {smpclient._address}..."
         connect_task = progress.add_task(description=connect_task_description, total=None)
```

### Comparing `smpmgr-0.5.0/smpmgr/image_management.py` & `smpmgr-0.6.0/smpmgr/image_management.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.5.0/smpmgr/logging.py` & `smpmgr-0.6.0/smpmgr/logging.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.5.0/smpmgr/main.py` & `smpmgr-0.6.0/smpmgr/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,27 @@
     TransportDefinition,
     connect_with_spinner,
     get_smpclient,
     smp_request,
 )
 from smpmgr.image_management import upload_with_progress_bar
 from smpmgr.logging import LogLevel, setup_logging
+from smpmgr.user import intercreate
 
 logger = logging.getLogger(__name__)
 
 HELP_LINES: Final = (
     f"Simple Management Protocol (SMP) Manager Version {get_version(__package__)}\n",
     "Copyright (c) 2023-2024 Intercreate, Inc. and Contributors\n",
 )
 
 app: Final = typer.Typer(help="\n".join(HELP_LINES))
 app.add_typer(os_management.app)
 app.add_typer(image_management.app)
+app.add_typer(intercreate.app)
 
 
 @app.callback(invoke_without_command=True)
 def options(
     ctx: typer.Context,
     port: str = typer.Option(
         None, help="The serial port to connect to, e.g. COM1, /dev/ttyACM0, etc."
```

### Comparing `smpmgr-0.5.0/smpmgr/os_management.py` & `smpmgr-0.6.0/smpmgr/os_management.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.5.0/PKG-INFO` & `smpmgr-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: smpmgr
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple Management Protocol (SMP) Manager for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jp@intercreate.io
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: smpclient (>=1.0.1,<2.0.0)
+Requires-Dist: smpclient (>=1.3.1,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP) Manager
 
 `smpmgr` is a CLI application for interacting with device firmware over a
 **serial (UART or USB)**, **Bluetooth (BLE)**, or **UDP**, connection.  It can be used as a
```


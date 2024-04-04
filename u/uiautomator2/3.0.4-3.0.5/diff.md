# Comparing `tmp/uiautomator2-3.0.4.tar.gz` & `tmp/uiautomator2-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautomator2-3.0.4.tar", max compression
+gzip compressed data, was "uiautomator2-3.0.5.tar", max compression
```

## Comparing `uiautomator2-3.0.4.tar` & `uiautomator2-3.0.5.tar`

### file list

```diff
@@ -1,45 +1,43 @@
--rw-r--r--   0        0        0     1064 2024-03-30 16:28:40.099037 uiautomator2-3.0.4/LICENSE
--rw-r--r--   0        0        0    53131 2024-03-30 16:28:40.099037 uiautomator2-3.0.4/README.md
--rw-r--r--   0        0        0     1045 2024-03-30 16:28:57.443193 uiautomator2-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    69426 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/__init__.py
--rw-r--r--   0        0        0     8106 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/__main__.py
--rw-r--r--   0        0        0      289 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/_proto.py
--rw-r--r--   0        0        0    21287 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/_selector.py
--rw-r--r--   0        0        0      647 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/abcd.py
--rw-r--r--   0        0        0  1061950 2024-03-30 16:28:56.407184 uiautomator2-3.0.4/uiautomator2/assets/app-uiautomator-test.apk
--rw-r--r--   0        0        0  2191186 2024-03-30 16:28:55.767179 uiautomator2-3.0.4/uiautomator2/assets/app-uiautomator.apk
--rwxr-xr-x   0        0        0      570 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/assets/sync.sh
--rw-r--r--   0        0        0     2602 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/__init__.py
--rw-r--r--   0        0        0      405 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/README.md
--rw-r--r--   0        0        0     5574 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/__init__.py
--rw-r--r--   0        0        0     4802 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/index.html
--rw-r--r--   0        0        0    61137 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/pig.jpg
--rw-r--r--   0        0        0     1100 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
--rw-r--r--   0        0        0       29 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/start.bat
--rw-r--r--   0        0        0     2645 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/info/__init__.py
--rw-r--r--   0        0        0    28515 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/info/conf.py
--rw-r--r--   0        0        0     2852 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext/perf/README.md
--rw-r--r--   0        0        0    12384 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/ext/perf/__init__.py
--rw-r--r--   0        0        0    41467 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/ext/perf/net.png
--rw-r--r--   0        0        0    26928 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/ext/perf/summary.png
--rw-r--r--   0        0        0       88 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/ext/xpath/README.md
--rw-r--r--   0        0        0      228 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/ext/xpath/__init__.py
--rw-r--r--   0        0        0     4180 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext-archived/aircv/README.md
--rw-r--r--   0        0        0    18456 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext-archived/aircv/__init__.py
--rw-r--r--   0        0        0      947 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/README.md
--rw-r--r--   0        0        0     2495 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/__init__.py
--rw-r--r--   0        0        0     3308 2024-03-30 16:28:40.103037 uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/baiduOCR.py
--rw-r--r--   0        0        0    10564 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/image.py
--rw-r--r--   0        0        0    15077 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/init.py
--rw-r--r--   0        0        0     1801 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/messagebox.py
--rw-r--r--   0        0        0     3776 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/screenrecord.py
--rw-r--r--   0        0        0     3342 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/settings.py
--rw-r--r--   0        0        0     1762 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/swipe.py
--rw-r--r--   0        0        0     5856 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/utils.py
--rw-r--r--   0        0        0     4780 2024-03-30 16:28:57.443193 uiautomator2-3.0.4/uiautomator2/version.py
--rw-r--r--   0        0        0     9885 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/watcher.py
--rw-r--r--   0        0        0     6704 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/webview.py
--rw-r--r--   0        0        0    14506 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/widget.py
--rw-r--r--   0        0        0    28935 2024-03-30 16:28:40.107037 uiautomator2-3.0.4/uiautomator2/xpath.py
--rw-r--r--   0        0        0    54047 1970-01-01 00:00:00.000000 uiautomator2-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-04 14:51:55.415653 uiautomator2-3.0.5/LICENSE
+-rw-r--r--   0        0        0    53306 2024-04-04 14:51:55.419653 uiautomator2-3.0.5/README.md
+-rw-r--r--   0        0        0     1032 2024-04-04 14:52:09.127554 uiautomator2-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0    68753 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/__init__.py
+-rw-r--r--   0        0        0     7964 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/__main__.py
+-rw-r--r--   0        0        0      289 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/_proto.py
+-rw-r--r--   0        0        0    21287 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/_selector.py
+-rw-r--r--   0        0        0      647 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/abcd.py
+-rw-r--r--   0        0        0  1061950 2024-04-04 14:52:08.183558 uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator-test.apk
+-rw-r--r--   0        0        0  2191186 2024-04-04 14:52:08.011560 uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator.apk
+-rwxr-xr-x   0        0        0      570 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/assets/sync.sh
+-rw-r--r--   0        0        0     2602 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/README.md
+-rw-r--r--   0        0        0     5574 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/__init__.py
+-rw-r--r--   0        0        0     4802 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/index.html
+-rw-r--r--   0        0        0    61137 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/pig.jpg
+-rw-r--r--   0        0        0     1100 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
+-rw-r--r--   0        0        0       29 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/start.bat
+-rw-r--r--   0        0        0     2645 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/info/__init__.py
+-rw-r--r--   0        0        0    28515 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/info/conf.py
+-rw-r--r--   0        0        0     2852 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/README.md
+-rw-r--r--   0        0        0    12384 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/__init__.py
+-rw-r--r--   0        0        0    41467 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/net.png
+-rw-r--r--   0        0        0    26928 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/summary.png
+-rw-r--r--   0        0        0     4180 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/README.md
+-rw-r--r--   0        0        0    18456 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/README.md
+-rw-r--r--   0        0        0     2495 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/baiduOCR.py
+-rw-r--r--   0        0        0    10476 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/image.py
+-rw-r--r--   0        0        0    14731 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/init.py
+-rw-r--r--   0        0        0     1801 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/messagebox.py
+-rw-r--r--   0        0        0     3776 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/screenrecord.py
+-rw-r--r--   0        0        0     3342 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/settings.py
+-rw-r--r--   0        0        0     1762 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/swipe.py
+-rw-r--r--   0        0        0     5856 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/utils.py
+-rw-r--r--   0        0        0     4780 2024-04-04 14:52:09.131554 uiautomator2-3.0.5/uiautomator2/version.py
+-rw-r--r--   0        0        0     9456 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/watcher.py
+-rw-r--r--   0        0        0     6710 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/webview.py
+-rw-r--r--   0        0        0    14389 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/widget.py
+-rw-r--r--   0        0        0    23845 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/xpath.py
+-rw-r--r--   0        0        0    54208 1970-01-01 00:00:00.000000 uiautomator2-3.0.5/PKG-INFO
```

### Comparing `uiautomator2-3.0.4/LICENSE` & `uiautomator2-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/README.md` & `uiautomator2-3.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# uiautomator2 [![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg)](https://pypi.python.org/pypi/uiautomator2) ![PyPI](https://img.shields.io/pypi/pyversions/uiautomator2.svg)
+# uiautomator2
+[![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg)](https://pypi.python.org/pypi/uiautomator2)
+![PyPI](https://img.shields.io/pypi/pyversions/uiautomator2.svg)
+[![codecov](https://codecov.io/gh/openatx/uiautomator2/graph/badge.svg?token=d0ZLkqorBu)](https://codecov.io/gh/openatx/uiautomator2)
 
 QQ交流群: **815453846**
 
 > 有段时间没有维护这个项目了（可能有两年了），但是最近工作需要又重新研究一下Android原生自动化，当然又调研了Appium，对比下来一看，发现uiautomator2这个项目的运行速度是真的好快，从检测元素到点击，都是毫秒级的，代码也比较好理解。真是没想到以前竟然写出了这么神奇的项目，这么好的项目怎么能让它落灰呢，得好好整一整，一些垃圾代码清理清理。所以项目版本从2.x.x升级到了3.x.x
 
 还在用2.x.x版本的用户，可以先看一下[2to3](docs/2to3.md) 再决定是否要升级3.x.x （我个人还是非常建议升级的）
 
@@ -75,15 +78,15 @@
 - [py-uiautomator2通过悬浮窗让服务长时间可用](https://zhuanlan.zhihu.com/p/688009468) 这个**强烈推荐**看一下
 - [termux里如何部署uiautomator2简介](https://www.cnblogs.com/ze-yan/p/12242383.html) by `成都-测试只会一点点`
 
 ## 相关项目
 - 基于adb协议与Android进行交互的库 [adbutils](https://github.com/openatx/adbutils)
 - 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
 - [atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务
-- 类似于uiautomatorviewer，用于查看UI层级结构 https://appinspector.devsleep.com
+- [uiauto.dev](https://uiauto.dev) 用于查看UI层级结构，类似于uiautomatorviewer(用于替代之前写的weditor），用于查看UI层级结构 
 - ~~[weditor](https://github.com/openatx/weditor) 类似于uiautomatorviewer，专门为本项目开发的辅助编辑器(这个暂不维护了~~
 
 **[Installation](#installation)**
 
 **[Connect to a device](#connect-to-a-device)**
 
 **[Command line](#command-line)**
@@ -146,24 +149,24 @@
     ```
     
     测试是否安装成功 `uiautomator2 --help`
     
 2. UI Inspector
 
     ```bash
-    pip install appinspector
+    pip install uiauto-dev
     # 启动
-    appinspector
+    uiauto.dev
     ```
 
-    浏览器打开 https://appinspector.devsleep.com 查看当前设备的界面结构。
+    浏览器打开 https://uiauto.dev 查看当前设备的界面结构。
 
     **appinspector介绍**
 
-    [appinspector](https://github.com/codeskyblue/appinspector) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
+    [uiauto.dev](https://github.com/codeskyblue/uiauto.dev) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
 
 # Connect to a device
 There are two ways to connect to the device. 
 
 1. **Through WiFi**
 
 Suppose device IP is `10.0.0.1` and your PC is in the same network.
```

### Comparing `uiautomator2-3.0.4/pyproject.toml` & `uiautomator2-3.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "uiautomator2"
-version = "3.0.4"
+version = "3.0.5"
 description = "automator for anroid device"
 homepage = "https://github.com/openatx/uiautomator2"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["*/assets/*.apk"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "*"
 lxml = "*"
-adbutils = ">=2.2"
+adbutils = "^2.2.3"
 retry = ">=0,<1"
 packaging = ">=20.3"
+pillow = "*"
 
 # TODO: remove later
 Deprecated = "*"
-logzero = "*"
 filelock = ">=3,<4"
 progress = "^1.6"
-pillow = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 isort = "^5.13.2"
 pytest-cov = "^4.1.0"
 ipython = "*"
```

### Comparing `uiautomator2-3.0.4/uiautomator2/__init__.py` & `uiautomator2-3.0.5/uiautomator2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,47 +35,50 @@
 from functools import cached_property
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 # import progress.bar
 import adbutils
 import filelock
-import logzero
 import requests
 from deprecated import deprecated
-from logzero import setup_logger
 from packaging import version as packaging_version
 from PIL import Image
 from retry import retry
-from urllib3.util.retry import Retry
 
 from . import xpath
 from ._proto import HTTP_TIMEOUT, SCROLL_STEPS, Direction
 from ._selector import Selector, UiObject
 from .exceptions import BaseError, ConnectError, GatewayError, JSONRPCError, NullObjectExceptionError, \
     NullPointerExceptionError, RetryError, ServerError, SessionBrokenError, StaleObjectExceptionError, \
     UiAutomationNotConnectedError, UiObjectNotFoundError
-from .init import Initer
 # from .session import Session  # noqa: F401
 from .settings import Settings
 from .swipe import SwipeExt
-from .utils import list2cmdline, process_safe_wrapper, thread_safe_wrapper
+from .utils import list2cmdline
 from .version import __apk_version__, __atx_agent_version__
 from .watcher import WatchContext, Watcher
 
 DEBUG = False
 WAIT_FOR_DEVICE_TIMEOUT = int(os.getenv("WAIT_FOR_DEVICE_TIMEOUT", 20))
 
-
-log_format = '%(color)s[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d]%(end_color)s [pid:%(process)d] %(message)s'
-formatter = logzero.LogFormatter(fmt=log_format)
-logger = setup_logger("uiautomator2", level=logging.DEBUG, formatter=formatter)
 _mswindows = (os.name == "nt")
 
 
+logger = logging.getLogger(__name__)
+
+def enable_pretty_logging(level=logging.DEBUG):
+    if not logger.handlers:
+        # Configure handler
+        handler = logging.StreamHandler()
+        formatter = logging.Formatter('[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d pid:%(process)d] %(message)s')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+    logger.setLevel(level)
+
 class AppInstaller(abc.ABC):
     """ 解决手机安装apk弹窗问题 """
     @abc.abstractmethod
     def install(self, url: str):
         """ install app to device """
 
 
@@ -203,15 +206,15 @@
                 raise
 
 
         if not self.__client._serial:
             raise OSError(
                 "http-request to atx-agent error, can only recover from USB")
 
-        logger.warning("atx-agent has something wrong, auto recovering")
+        logger.info("atx-agent has something wrong, auto recovering")
         # ReadTimeout: sometime means atx-agent is running but not responsing
         # one reason is futex_wait_queue: https://stackoverflow.com/questions/9801256/app-hangs-on-futex-wait-queue-me-every-a-couple-of-minutes
 
         # fix atx-agent and request again
         self.__client._prepare_atx_agent()
         url = self.__client.path2url(url)
         return super().request(method, url, **kwargs)
@@ -240,30 +243,21 @@
             # WIFI 连接
             self._serial = serial_or_url
             self._atx_agent_url = serial_or_url
         else:
             # USB 连接
             self._serial = serial_or_url
             self._atx_agent_url = None
-
-        # setup logger
-        log_format = f'%(color)s[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d]%(end_color)s [pid:%(process)d] [{self._serial}] %(message)s'
-        formatter = logzero.LogFormatter(fmt=log_format)
-        self._logger = setup_logger(name="uiautomator2.client", level=logging.DEBUG, formatter=formatter)
         
         filelock_path = os.path.expanduser("~/.uiautomator2/filelocks/") + base64.urlsafe_b64encode(self._serial.encode('utf-8')).decode('utf-8') + ".lock"
         os.makedirs(os.path.dirname(filelock_path), exist_ok=True)
         self._filelock = filelock.FileLock(filelock_path, timeout=200)
 
         self._app_installer: AppInstaller = None
 
-    @property
-    def logger(self) -> logging.Logger:
-        return self._logger
-
     def set_app_installer(self, app_installer: AppInstaller):
         """ set uiautomator.apk installer """
         assert isinstance(app_installer, AppInstaller)
         self._app_installer = app_installer
 
     def _get_atx_agent_url(self) -> str:
         """ get url for python client to connect """
@@ -273,15 +267,15 @@
         try:
             lport = self._adb_device.forward_port(
                 7912)  # this method is so fast, only take 0.2ms
             return f"http://{self._adb_device._client.host}:{lport}"
         except adbutils.AdbError as e:
             if not _is_tmq_production() and self._atx_agent_url:
                 # when device offline, use atx-agent-url
-                self.logger.info(
+                logger.info(
                     "USB disconnected, fallback to WiFi, ATX_AGENT_URL=%s",
                     self._atx_agent_url)
                 return self._atx_agent_url
             raise
 
     def _get_atx_agent_path(self) -> str:
         return "/data/local/tmp/atx-agent"
@@ -302,15 +296,15 @@
         """
         check running -> push binary -> launch
         """
         assert self._serial, "Device serialno is required"
         _d = self._wait_for_device()
         if not _d:
             raise RuntimeError("USB device %s is offline" % self._serial)
-        self.logger.debug("device %s is online", self._serial)
+        logger.debug("device %s is online", self._serial)
         version_url = self.path2url("/version")
         try:
             version = requests.get(version_url, timeout=3).text
             if version != __atx_agent_version__:
                 raise EnvironmentError("atx-agent need upgrade")
         except (requests.RequestException, EnvironmentError):
             self._setup_atx_agent()
@@ -342,21 +336,21 @@
         _RE_remote_adb = re.compile(r"^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}:\d+$")
         _is_remote = _RE_remote_adb.match(self._serial) is not None
 
         adb = adbutils.adb
         deadline = time.time() + timeout
         while time.time() < deadline:
             title = "device reconnecting" if _is_remote else "wait-for-device"
-            self.logger.info("%s, time left(%.1fs)", title, deadline - time.time())
+            logger.info("%s, time left(%.1fs)", title, deadline - time.time())
             if _is_remote:
                 try:
                     adb.disconnect(self._serial)
                     adb.connect(self._serial, timeout=1)
                 except (adbutils.AdbError, adbutils.AdbTimeout) as e:
-                    self.logger.debug("adb reconnect error: %s", str(e))
+                    logger.debug("adb reconnect error: %s", str(e))
                     time.sleep(1.0)
                     continue
             try:
                 adb.wait_for(self._serial, timeout=1)
             except (adbutils.AdbError, adbutils.AdbTimeout):
                 continue
             
@@ -376,15 +370,15 @@
 
         for name in ("app-uiautomator.apk", "app-uiautomator-test.apk"):
             apk_path = assets_dir.joinpath(name).as_posix()
             cwd_apk_path = cwd_assets_dir.joinpath(name).as_posix()
             if not os.path.exists(apk_path) and os.path.exists(cwd_apk_path):
                 apk_path = cwd_apk_path
             target_path = "/data/local/tmp/" + name
-            self.logger.debug("Install %s", name)
+            logger.debug("Install %s", name)
             self.push(apk_path, target_path)
             self.shell(['pm', 'install', '-r', '-t', target_path])
 
     def sleep(self, seconds: float):
         """ same as time.sleep """
         time.sleep(seconds)
 
@@ -477,15 +471,15 @@
         try:
             return self._jsonrpc_call(*args, **kwargs)
         except (requests.ReadTimeout, ServerError) as e:
             self.reset_uiautomator(str(e))  # uiautomator可能出问题了，强制重启一下
         except (NullObjectExceptionError,
                 NullPointerExceptionError,
                 StaleObjectExceptionError) as e:
-            self.logger.warning("jsonrpc call got: %s", str(e))
+            logger.warning("jsonrpc call got: %s", str(e))
             self.reset_uiautomator(str(e))  # added to fix strange fatal jsonrpc NullPointerException
         return self._jsonrpc_call(*args, **kwargs)
 
     def _jsonrpc_call(self, method, params=[], http_timeout=60):
         """ jsonrpc2 call
         Refs:
             - http://www.jsonrpc.org/specification
@@ -614,15 +608,15 @@
                     "Uiautomator started failed.",
                     reason,
                     "https://github.com/openatx/uiautomator2/wiki/Common-issues",
                     "adb shell am instrument -w -r -e debug false -e class com.github.uiautomator.stub.Stub com.github.uiautomator.test/android.support.test.runner.AndroidJUnitRunner",
                 )
 
             if depth > 0:
-                self.logger.info("restart-uiautomator since \"%s\"", reason)
+                logger.info("restart-uiautomator since \"%s\"", reason)
 
             # Note:
             # atx-agent check has moved to _AgentRequestSession
             # If code goes here, it means atx-agent is fine.
 
             if self._is_alive():
                 return
@@ -631,33 +625,32 @@
             if self._is_agent_outdated():
                 if self._serial: # update atx-agent will not work on WiFi
                     self._prepare_atx_agent()
 
             ok = self._force_reset_uiautomator_v2(
                 launch_test_app=depth > 0)  # uiautomator 2.0
             if ok:
-                self.logger.info("uiautomator back to normal")
+                logger.info("uiautomator back to normal")
                 return
 
             output = self._test_run_instrument()
             if "does not have a signature matching the target" in output:
                 self._setup_uiautomator()
                 reason = "signature not match, reinstall uiautomator apks"
 
         return self.reset_uiautomator(reason=reason,
                                     depth=depth + 1)
 
     def _force_reset_uiautomator_v2(self, launch_test_app=False):
         brand = self.shell("getprop ro.product.brand").output.strip()
-        # self.logger.debug("Device: %s, %s", brand, self.serial)
         package_name = "com.github.uiautomator"
 
         self.uiautomator.stop()
 
-        self.logger.debug("kill process(ps): uiautomator")
+        logger.debug("kill process(ps): uiautomator")
         self._kill_process_by_name("uiautomator")
 
         ## Note: Here do not reinstall apks, since vivo and oppo reinstall need password
         # if self._is_apk_outdated():
         #     self._setup_uiautomator()
         if self._is_apk_required():
             self._setup_uiautomator()
@@ -669,29 +662,29 @@
         self.uiautomator.start()
 
         # wait until uiautomator2 service is working
         time.sleep(.5)
         deadline = time.time() + 40.0  # in vivo-Y67, launch timeout 24s
         flow_window_showed = False
         while time.time() < deadline:
-            self.logger.debug("uiautomator-v2 is starting ... left: %.1fs",
+            logger.debug("uiautomator-v2 is starting ... left: %.1fs",
                          deadline - time.time())
 
             if not self.uiautomator.running():
                 break
 
             if self._is_alive():
                 # 显示悬浮窗，增加稳定性
                 # 可能会带来悬浮窗对话框
                 # 利大于弊，先加了
                 # show Float window 在华为手机上，还需要再次等待
                 if not flow_window_showed:
                     flow_window_showed = True
                     self.show_float_window(True)
-                    self.logger.debug("show float window")
+                    logger.debug("show float window")
                     time.sleep(1.0)
                     continue
                 return True
             time.sleep(1.0)
 
         self.uiautomator.stop()
         return False
@@ -731,15 +724,15 @@
             return None
         try:
             return packaging_version.parse(m.group('name'))
         except packaging_version.InvalidVersion:
             return None
 
     def _grant_app_permissions(self):
-        self.logger.debug("grant permissions")
+        logger.debug("grant permissions")
         for permission in [
                 "android.permission.SYSTEM_ALERT_WINDOW",
                 "android.permission.ACCESS_FINE_LOCATION",
                 "android.permission.READ_PHONE_STATE",
         ]:
             self.shell(['pm', 'grant', "com.github.uiautomator", permission])
 
@@ -748,15 +741,15 @@
             "am instrument -w -r -e debug false -e class com.github.uiautomator.stub.Stub com.github.uiautomator.test/android.support.test.runner.AndroidJUnitRunner",
             timeout=3)
         return shret.output
 
     def _kill_process_by_name(self, name, use_adb=False):
         for p in self._iter_process(use_adb=use_adb):
             if p.name == name and p.user == "shell":
-                self.logger.debug("kill %s", name)
+                logger.debug("kill %s", name)
                 kill_cmd = ["kill", "-9", str(p.pid)]
                 if use_adb:
                     self._adb_device.shell(kill_cmd)
                 else:
                     self.shell(kill_cmd)
 
     def _iter_process(self, use_adb=False):
@@ -872,15 +865,15 @@
         """ default 3 minutes
         Args:
             timeout (int): seconds
         """
         r = self.http.post("/newCommandTimeout", data=str(int(timeout)))
         data = r.json()
         assert data['success'], data['description']
-        self.logger.info("%s", data['description'])
+        logger.info("%s", data['description'])
 
     @cached_property
     def device_info(self):
         return self.http.get("/info").json()
 
     def window_size(self):
         """ return (width, height) """
@@ -1026,19 +1019,19 @@
     def _operation_delay(self, operation_name: str = None):
         before, after = self.settings['operation_delay']
         # 排除不要求延迟的方法
         if operation_name not in self.settings['operation_delay_methods']:
             before, after = 0, 0
 
         if before:
-            self.logger.debug(f"operation [{operation_name}] pre-delay {before}s")
+            logger.debug(f"operation [{operation_name}] pre-delay {before}s")
             time.sleep(before)
         yield
         if after:
-            self.logger.debug(f"operation [{operation_name}] post-delay {after}s")
+            logger.debug(f"operation [{operation_name}] post-delay {after}s")
             time.sleep(after)
 
     @property
     def touch(self):
         """
         ACTION_DOWN: 0 ACTION_MOVE: 2
         touch.down(x, y)
@@ -1949,28 +1942,25 @@
         subprocess.call([adbutils.adb_path(), "-s", addr, "wait-for-device"],
                         timeout=2)
     except subprocess.TimeoutExpired:
         raise ConnectError("Fail execute", "adb connect " + addr)
     return connect_usb(addr)
 
 
-def connect_usb(serial: Optional[str] = None, init: bool = False) -> Device:
+def connect_usb(serial: Optional[str] = None) -> Device:
     """
     Args:
         serial (str): android device serial
 
     Returns:
         Device
 
     Raises:
         ConnectError
     """
-    if init:
-        logger.warning("connect_usb, args init=True is deprecated since 2.8.0")
-
     if not serial:
         device = adbutils.adb.device()
         serial = device.serial
     return Device(serial)
 
 
 def connect_wifi(addr: str) -> Device:
```

### Comparing `uiautomator2-3.0.4/uiautomator2/__main__.py` & `uiautomator2-3.0.5/uiautomator2/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # coding: utf-8
 #
 
 from __future__ import absolute_import, print_function
 
 import argparse
-import hashlib
 import json
 import logging
-import os
-import re
 
 import adbutils
-import progress.bar
-import requests
-from logzero import logger
-from retry import retry
 
 import uiautomator2 as u2
 
 from .init import Initer
 from .version import __version__
 
 
+logger = logging.getLogger(__name__)
+
 def cmd_init(args):
     serial = args.serial or args.serial_optional
     if serial:
         device = adbutils.adb.device(serial)
         init = Initer(device)
         init.install()
     else:
@@ -280,10 +275,8 @@
         return
 
     parser.print_help()
     # yapf: enable
 
 
 if __name__ == '__main__':
-    # import logzero
-    # logzero.loglevel(logging.INFO)
     main()
```

### Comparing `uiautomator2-3.0.4/uiautomator2/_selector.py` & `uiautomator2-3.0.5/uiautomator2/_selector.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/abcd.py` & `uiautomator2-3.0.5/uiautomator2/abcd.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/assets/app-uiautomator-test.apk` & `uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator-test.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/assets/app-uiautomator.apk` & `uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/assets/sync.sh` & `uiautomator2-3.0.5/uiautomator2/assets/sync.sh`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/exceptions.py` & `uiautomator2-3.0.5/uiautomator2/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/htmlreport/__init__.py` & `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/index.html` & `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/index.html`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/pig.jpg` & `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/pig.jpg`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/htmlreport/assets/simplehttpserver.py` & `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/simplehttpserver.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/info/__init__.py` & `uiautomator2-3.0.5/uiautomator2/ext/info/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/info/conf.py` & `uiautomator2-3.0.5/uiautomator2/ext/info/conf.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/perf/README.md` & `uiautomator2-3.0.5/uiautomator2/ext/perf/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/perf/__init__.py` & `uiautomator2-3.0.5/uiautomator2/ext/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/perf/net.png` & `uiautomator2-3.0.5/uiautomator2/ext/perf/net.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext/perf/summary.png` & `uiautomator2-3.0.5/uiautomator2/ext/perf/summary.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext-archived/aircv/README.md` & `uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext-archived/aircv/__init__.py` & `uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/README.md` & `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/__init__.py` & `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/ext-archived/ocr/baiduOCR.py` & `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/baiduOCR.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/image.py` & `uiautomator2-3.0.5/uiautomator2/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from typing import Union
 
 import cv2
 import findit
 import imutils
 import numpy as np
 import requests
-from logzero import setup_logger
 from PIL import Image, ImageDraw
 from skimage.metrics import structural_similarity
 
 import uiautomator2
 
 ImageType = typing.Union[np.ndarray, Image.Image]
 
 compare_ssim = structural_similarity
+logger = logging.getLogger(__name__)
 
 
 def color_bgr2gray(image: ImageType):
     """ change color image to gray
     Returns:
         opencv-image
     """
@@ -219,21 +219,18 @@
 
 class ImageX(object):
     def __init__(self, d: "uiautomator2.Device"):
         """
         Args:
             d (uiautomator2 instance)
         """
-        self.logger = setup_logger()
         self._d = d
         assert hasattr(d, 'click')
         assert hasattr(d, 'screenshot')
 
-        self.logger.setLevel(logging.DEBUG)
-
     def send_click(self, x, y):
         return self._d.click(x, y)
     
     def getpixel(self, x, y):
         """
         Returns:
             (r, g, b)
@@ -270,21 +267,21 @@
         return {"similarity": target_sim, "point": [x, y]}
 
     def __wait(self, imdata, timeout=30.0, threshold=0.8):
         deadline = time.time() + timeout
         while time.time() < deadline:
             m = self.match(imdata)
             sim = m['similarity']
-            self.logger.debug("similarity %.2f [~%.2f], left time: %.1fs", sim,
+            logger.debug("similarity %.2f [~%.2f], left time: %.1fs", sim,
                               threshold, deadline - time.time())
             if sim < threshold:
                 continue
             time.sleep(.1)
             return m
-        self.logger.debug("image not found")
+        logger.debug("image not found")
 
     def wait(self, imdata, timeout=30.0, threshold=0.9):
         """ wait until image show up """
         m = self.__wait(imdata, timeout=timeout, threshold=threshold)
         return m
 
     def click(self, imdata, timeout=30.0, threshold=0.9):
```

### Comparing `uiautomator2-3.0.4/uiautomator2/init.py` & `uiautomator2-3.0.5/uiautomator2/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 import os
 import shutil
 import tarfile
 
 import adbutils
 import progress.bar
 import requests
-from logzero import logger, setup_logger
 from retry import retry
 
 from uiautomator2.utils import natualsize
 from uiautomator2.version import __apk_version__, __atx_agent_version__, __jar_version__, __version__
 
 appdir = os.path.join(os.path.expanduser("~"), '.uiautomator2')
 
 GITHUB_BASEURL = "https://github.com/openatx"
 
 
+logger = logging.getLogger(__name__)
+
 class DownloadBar(progress.bar.PixelBar):
     message = "Downloading"
     suffix = '%(current_size)s/%(total_size)s'
     width = 10
 
     @property
     def total_size(self):
@@ -84,15 +85,15 @@
         bar.finish()
 
     assert file_size == os.path.getsize(storepath +
                                         ".part")  # may raise FileNotFoundError
     shutil.move(storepath + '.part', storepath)
     return storepath
 
-def mirror_download(url: str, filename=None, logger: logging.Logger = logger):
+def mirror_download(url: str, filename=None):
     """
     Download from mirror, then fallback to origin url
     """
     storepath = gen_cachepath(url)
     if not filename:
         filename = os.path.basename(url)
     github_host = "https://github.com"
@@ -146,28 +147,26 @@
         self.abi = d.getprop('ro.product.cpu.abi')
         self.pre = d.getprop('ro.build.version.preview_sdk')
         self.arch = d.getprop('ro.arch')
         self.abis = (d.getprop('ro.product.cpu.abilist').strip()
                      or self.abi).split(",")
         
         self.__atx_listen_addr = "127.0.0.1:7912"
-        self.logger = setup_logger(level=loglevel)
-        # self.logger.debug("Initial device %s", device)
-        self.logger.info("uiautomator2 version: %s", __version__)
+        logger.info("uiautomator2 version: %s", __version__)
 
     def set_atx_agent_addr(self, addr: str):
         assert ":" in addr
         self.__atx_listen_addr = addr
 
     @property
     def atx_agent_path(self):
         return "/data/local/tmp/atx-agent"
 
     def shell(self, *args, timeout=60):
-        self.logger.debug("Shell: %s", args)
+        logger.debug("Shell: %s", args)
         return self._device.shell(args, timeout=60)
 
     @property
     def jar_urls(self):
         """
         Returns:
             iter([name, url], [name, url])
@@ -218,27 +217,25 @@
             GITHUB_BASEURL + "/stf-binaries",
             "/raw/0.3.0/node_modules/@devicefarmer/minitouch-prebuilt/prebuilt/",
             self.abi + "/bin/minitouch"
         ])
 
     @retry(tries=2, logger=logger)
     def push_url(self, url, dest=None, mode=0o755, tgz=False, extract_name=None):  # yapf: disable
-        path = mirror_download(url,
-                               filename=os.path.basename(url),
-                               logger=self.logger)
+        path = mirror_download(url, filename=os.path.basename(url))
         if tgz:
             tar = tarfile.open(path, 'r:gz')
             path = os.path.join(os.path.dirname(path), extract_name)
             tar.extract(extract_name,
                         os.path.dirname(path))  # zlib.error may raise
 
         if not dest:
             dest = "/data/local/tmp/" + os.path.basename(path)
 
-        self.logger.debug("Push to %s:0%o", dest, mode)
+        logger.debug("Push to %s:0%o", dest, mode)
         self._device.sync.push(path, dest, mode=mode)
         return dest
 
     def is_apk_outdated(self):
         """
         If apk signature mismatch, the uiautomator test will fail to start
         command: am instrument -w -r -e debug false \
@@ -248,54 +245,54 @@
             starting instrumentation ComponentInfo{com.github.uiautomator.test/android.support.test.runner.AndroidJUnitRunner} \
             from pid=7877, uid=7877 not allowed \
             because package com.github.uiautomator.test does not have a signature matching the target com.github.uiautomator
         """
         apk_debug = self._device.package_info("com.github.uiautomator")
         apk_debug_test = self._device.package_info(
             "com.github.uiautomator.test")
-        self.logger.debug("apk-debug package-info: %s", apk_debug)
-        self.logger.debug("apk-debug-test package-info: %s", apk_debug_test)
+        logger.debug("apk-debug package-info: %s", apk_debug)
+        logger.debug("apk-debug-test package-info: %s", apk_debug_test)
         if not apk_debug or not apk_debug_test:
             return True
         if apk_debug['version_name'] != __apk_version__:
-            self.logger.info(
+            logger.info(
                 "package com.github.uiautomator version %s, latest %s",
                 apk_debug['version_name'], __apk_version__)
             return True
 
         if apk_debug['signature'] != apk_debug_test['signature']:
             # On vivo-Y67 signature might not same, but signature matched.
             # So here need to check first_install_time again
             max_delta = datetime.timedelta(minutes=3)
             if abs(apk_debug['first_install_time'] -
                    apk_debug_test['first_install_time']) > max_delta:
-                self.logger.debug(
+                logger.debug(
                     "package com.github.uiautomator does not have a signature matching the target com.github.uiautomator"
                 )
                 return True
         return False
 
     def is_atx_agent_outdated(self):
         """
         Returns:
             bool
         """
         agent_version = self._device.shell([self.atx_agent_path, "version"]).strip()
         if agent_version == "dev":
-            self.logger.info("skip version check for atx-agent dev")
+            logger.info("skip version check for atx-agent dev")
             return False
 
         # semver major.minor.patch
         try:
             real_ver = list(map(int, agent_version.split(".")))
             want_ver = list(map(int, __atx_agent_version__.split(".")))
         except ValueError:
             return True
 
-        self.logger.debug("Real version: %s, Expect version: %s", real_ver,
+        logger.debug("Real version: %s, Expect version: %s", real_ver,
                           want_ver)
 
         if real_ver[:2] != want_ver[:2]:
             return True
 
         return real_ver[2] < want_ver[2]
 
@@ -323,90 +320,90 @@
         通常在连接USB数据线的情况下调用
         """
         self.shell("pm", "uninstall", "com.github.uiautomator")
         self.shell("pm", "uninstall", "com.github.uiautomator.test")
         for filename, url in app_uiautomator_apk_urls():
             path = self.push_url(url, mode=0o644)
             self.shell("pm", "install", "-r", "-t", path)
-            self.logger.info("- %s installed", filename)
+            logger.info("- %s installed", filename)
 
     def _install_jars(self):
         """ use uiautomator 1.0 to run uiautomator test """
         for (name, url) in self.jar_urls:
             self.push_url(url, "/data/local/tmp/" + name, mode=0o644)
 
     def _install_atx_agent(self):
-        self.logger.info("Install atx-agent %s", __atx_agent_version__)
+        logger.info("Install atx-agent %s", __atx_agent_version__)
         self.push_url(self.atx_agent_url, tgz=True, extract_name="atx-agent")
 
     def setup_atx_agent(self):
         # stop atx-agent first
         self.shell(self.atx_agent_path, "server", "--stop")
         if self.is_atx_agent_outdated():
-            self.logger.info("Install atx-agent %s", __atx_agent_version__)
+            logger.info("Install atx-agent %s", __atx_agent_version__)
             self.push_url(self.atx_agent_url, tgz=True, extract_name="atx-agent")
         
         self.shell(self.atx_agent_path, 'server', '--nouia', '-d', "--addr", self.__atx_listen_addr)
-        self.logger.info("Check atx-agent version")
+        logger.info("Check atx-agent version")
         self.check_atx_agent_version()
 
     @retry(
         (requests.ConnectionError, requests.ReadTimeout, requests.HTTPError),
         delay=.5,
         tries=10)
     def check_atx_agent_version(self):
         port = self._device.forward_port(7912)
-        self.logger.debug("Forward: local:tcp:%d -> remote:tcp:%d", port, 7912)
+        logger.debug("Forward: local:tcp:%d -> remote:tcp:%d", port, 7912)
         version = requests.get("http://%s:%d/version" %
                                (self._device._client.host, port)).text.strip()
-        self.logger.debug("atx-agent version %s", version)
+        logger.debug("atx-agent version %s", version)
 
         wlan_ip = requests.get("http://%s:%d/wlan/ip" %
                                (self._device._client.host, port)).text.strip()
-        self.logger.debug("device wlan ip: %s", wlan_ip)
+        logger.debug("device wlan ip: %s", wlan_ip)
         return version
 
     def install(self):
         """
         TODO: push minicap and minitouch from tgz file
         """
-        self.logger.info("Install minicap, minitouch")
+        logger.info("Install minicap, minitouch")
         self.push_url(self.minitouch_url)
         if self.abi == "x86":
-            self.logger.info(
+            logger.info(
                 "abi:x86 not supported well, skip install minicap")
         elif int(self.sdk) > 30:
-            self.logger.info("Android R (sdk:30) has no minicap resource")
+            logger.info("Android R (sdk:30) has no minicap resource")
         else:
             for url in self.minicap_urls:
                 self.push_url(url)
 
         # self._install_jars() # disable jars
         if self.is_apk_outdated():
-            self.logger.info(
+            logger.info(
                 "Install com.github.uiautomator, com.github.uiautomator.test %s",
                 __apk_version__)
             self._install_uiautomator_apks()
         else:
-            self.logger.info("Already installed com.github.uiautomator apks")
+            logger.info("Already installed com.github.uiautomator apks")
 
         self.setup_atx_agent()
         print("Successfully init %s" % self._device)
 
     def uninstall(self):
         self._device.shell([self.atx_agent_path, "server", "--stop"])
         self._device.shell(["rm", self.atx_agent_path])
-        self.logger.info("atx-agent stopped and removed")
+        logger.info("atx-agent stopped and removed")
         self._device.shell(["rm", "/data/local/tmp/minicap"])
         self._device.shell(["rm", "/data/local/tmp/minicap.so"])
         self._device.shell(["rm", "/data/local/tmp/minitouch"])
-        self.logger.info("minicap, minitouch removed")
+        logger.info("minicap, minitouch removed")
         self._device.shell(["pm", "uninstall", "com.github.uiautomator"])
         self._device.shell(["pm", "uninstall", "com.github.uiautomator.test"])
-        self.logger.info("com.github.uiautomator uninstalled, all done !!!")
+        logger.info("com.github.uiautomator uninstalled, all done !!!")
 
 
 if __name__ == "__main__":
     import adbutils
 
     serial = None
     device = adbutils.adb.device(serial)
```

### Comparing `uiautomator2-3.0.4/uiautomator2/messagebox.py` & `uiautomator2-3.0.5/uiautomator2/messagebox.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/screenrecord.py` & `uiautomator2-3.0.5/uiautomator2/screenrecord.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/settings.py` & `uiautomator2-3.0.5/uiautomator2/settings.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/swipe.py` & `uiautomator2-3.0.5/uiautomator2/swipe.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/utils.py` & `uiautomator2-3.0.5/uiautomator2/utils.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.4/uiautomator2/version.py` & `uiautomator2-3.0.5/uiautomator2/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 #
 
 # version managed by poetry
-__version__ = "3.0.4"
+__version__ = "3.0.5"
 
 # See ChangeLog for details
 
 __apk_version__ = '2.3.3'
 # 2.3.3 make float windows smaller
 # 2.3.2 merge pull requests # require atx-agent>=0.10.0
 # 2.3.1 support minicapagent, rotationagent, minitouchagent
```

### Comparing `uiautomator2-3.0.4/uiautomator2/watcher.py` & `uiautomator2-3.0.5/uiautomator2/watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 import logging
 import threading
 import time
 import typing
 from collections import OrderedDict
 from typing import Optional
 
-from logzero import setup_logger
-
 import uiautomator2
 from uiautomator2.xpath import XPath
+from uiautomator2.utils import inject_call
 
-from .utils import inject_call
-
-logger = logging.getLogger("uiautomator2")
+logger = logging.getLogger(__name__)
 
 
 def _callback_click(el):
-    # print("callback", threading.current_thread())
     el.click()
 
 
 class WatchContext:
     def __init__(self, d: "uiautomator2.Device", builtin: bool = False):
         self._d = d
         self._callbacks = OrderedDict()
@@ -151,53 +147,41 @@
         self._watchers = []
 
         self._watch_stop_event = threading.Event()
         self._watch_stopped = threading.Event()
         self._watching = False  # func start is calling
         self._triggering = False
 
-        self.logger = setup_logger()
-        self.logger.setLevel(logging.INFO)
-
-    @property
-    def debug(self):
-        return self.logger.level == logging.DEBUG
-
-    @debug.setter
-    def debug(self, v: bool):
-        assert isinstance(v, bool)
-        self.logger.setLevel(logging.DEBUG if v else logging.INFO)
-
     @property
     def _xpath(self) -> XPath:
         return self._d.xpath
 
     def _dump_hierarchy(self):
         return self._d.dump_hierarchy()
 
     def when(self, xpath=None):
         return XPathWatcher(self, xpath)
 
     def start(self, interval: float = 2.0):
         """ stop watcher """
         if self._watching:
-            self.logger.warning("already started")
+            logger.warning("already started")
             return
         self._watching = True
         th = threading.Thread(name="watcher",
                               target=self._watch_forever,
                               args=(interval, ))
         th.daemon = True
         th.start()
         return th
 
     def stop(self):
         """ stop watcher """
         if not self._watching:
-            self.logger.warning("watch already stopped")
+            logger.warning("watch already stopped")
             return
 
         if self._watch_stopped.is_set():
             return
 
         self._watch_stopped.set()
         self._watch_stop_event.wait(timeout=10)
@@ -235,15 +219,15 @@
             source: hierarchy content
         """
         if self.triggering:  # avoid to run watcher when run watcher
             return False
         try:
             return self._run_watchers(source=source)
         except Exception as e:
-            self.logger.warning("_run_watchers exception: %s", e)
+            logger.warning("_run_watchers exception: %s", e)
             return False
 
     def _run_watchers(self, source=None) -> bool:
         """
         Returns:
             bool (watched or not)
         """
@@ -254,15 +238,15 @@
             for xpath in h['xpaths']:
                 last_selector = self._xpath(xpath, source)
                 if not last_selector.exists:
                     last_selector = None
                     break
 
             if last_selector:
-                self.logger.info("XPath(hook:%s): %s", h['name'], h['xpaths'])
+                logger.info("XPath(hook:%s): %s", h['name'], h['xpaths'])
                 self._triggering = True
                 cb = h['callback']
                 defaults = {
                     "selector": last_selector,
                     "d": self._d,
                     "source": source,
                 }
@@ -272,15 +256,15 @@
                     for key in st.parameters.keys() if key in defaults
                 }
                 ba = st.bind(**kwargs)
                 ba.apply_defaults()
                 try:
                     cb(*ba.args, **ba.kwargs)
                 except Exception as e:
-                    self.logger.warning("watchers exception: %s", e)
+                    logger.warning("watchers exception: %s", e)
                 finally:
                     self._triggering = False
                 return True
         return False
 
     def __call__(self, name: str) -> "XPathWatcher":
         return XPathWatcher(self, None, name)
@@ -288,15 +272,15 @@
     def remove(self, name=None):
         """ remove watcher """
         if name is None:
             self._watchers = []
             return
         for w in self._watchers[:]:
             if w['name'] == name:
-                self.logger.debug("remove(%s) %s", name, w['xpaths'])
+                logger.debug("remove(%s) %s", name, w['xpaths'])
                 self._watchers.remove(w)
 
 
 class XPathWatcher():
     def __init__(self, parent: Watcher, xpath: str, name: str = ''):
         self._name = name
         self._parent = parent
```

### Comparing `uiautomator2-3.0.4/uiautomator2/webview.py` & `uiautomator2-3.0.5/uiautomator2/webview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # coding: utf-8
 #
 # Not implemented yet.
 #
-
-import contextlib
 import json
+import logging
 import string
 from pprint import pprint
 
 import adbutils
 import pychrome
 import requests
-from logzero import logger
 
+logger = logging.getLogger(__name__)
 
 class WebviewDriver():
     def __init__(self, url):
         self._url = url
         self._browser = pychrome.Browser(self._url)
 
     @property
```

### Comparing `uiautomator2-3.0.4/uiautomator2/widget.py` & `uiautomator2-3.0.5/uiautomator2/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import time
 from collections import defaultdict, namedtuple
 from functools import partial
 from pprint import pprint
 from typing import Union
 
 import requests
-from logzero import logger, setup_logger
 from lxml import etree
 
 import uiautomator2 as u2
-import uiautomator2.image as uim
 from uiautomator2.image import compare_ssim, draw_point, imread
 
+logger = logging.getLogger(__name__)
+
 
 def xml2nodes(xml_content: Union[str, bytes]):
     if isinstance(xml_content, str):
         xml_content = xml_content.encode("utf-8")
 
     root = etree.fromstring(xml_content)
     nodes = []
@@ -88,17 +88,14 @@
     def __init__(self, d: "u2.Device"):
         self._d = d
         self._widgets = {}
         self._compare_results = {}
 
         self.popups = []
 
-        self.logger = setup_logger()
-        self.logger.setLevel(logging.INFO)
-
     @property
     def wait_timeout(self):
         return self._d.settings['wait_timeout']
 
     def _get_widget(self, id: str):
         if id in self._widgets:
             return self._widgets[id]
```

### Comparing `uiautomator2-3.0.4/uiautomator2/xpath.py` & `uiautomator2-3.0.5/uiautomator2/xpath.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # coding: utf-8
 #
 
 from __future__ import absolute_import
 
-import abc
 import functools
-import io
-import json
 import logging
 import re
 import threading
 import time
 from collections import defaultdict
-from types import ModuleType
-from typing import Callable, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
-import adbutils
 from deprecated import deprecated
-from logzero import logger, setup_logger
 from PIL import Image
 from lxml import etree
 
 from uiautomator2._proto import Direction
 from uiautomator2.abcd import DeviceInterface
 from uiautomator2.exceptions import XPathElementNotFoundError
 from uiautomator2.utils import inject_call, swipe_in_bounds
 
 
+logger = logging.getLogger(__name__)
+
 def safe_xmlstr(s):
     return s.replace("$", "-")
 
 
 def string_quote(s):
     """quick way to quote string"""
     return "{!r}".format(s)
@@ -38,23 +34,23 @@
 
 def str2bytes(v: Union[str, bytes]) -> bytes:
     if isinstance(v, bytes):
         return v
     return v.encode("utf-8")
 
 
-def is_xpath_syntax_ok(xpath_expression) -> bool:
+def is_xpath_syntax_ok(xpath_expression: str) -> bool:
     try:
         etree.XPath(xpath_expression)
         return True  # No error means the XPath syntax is likely okay
     except etree.XPathSyntaxError:
         return False  # Indicates a syntax error in the XPath expression
 
 
-def strict_xpath(xpath: str, logger=logger) -> str:
+def strict_xpath(xpath: str) -> str:
     """make xpath to be computer recognized xpath"""
     orig_xpath = xpath
 
     if xpath.startswith("/"):
         pass
     elif xpath.startswith("@"):
         xpath = "//*[@resource-id={!r}]".format(xpath[1:])
@@ -115,19 +111,14 @@
         self._event_callbacks = defaultdict(list)
 
         # used for click("#back") and back is the key
         self._alias = {}
         self._alias_strict = False
         self._dump_lock = threading.Lock()
 
-        # 这里setup_logger不可以通过level参数传入logging.INFO
-        # 不然其StreamHandler都要重新setLevel，没看懂也没关系，反正就是不要这么干. 特此备注
-        self._logger = setup_logger()
-        self._logger.setLevel(logging.INFO)
-
     def global_set(self, key, value):
         valid_keys = {
             "timeout",
             "alias",
             "alias_strict",
             "click_after_delay",
             "click_before_delay",
@@ -140,23 +131,14 @@
             setattr(self, "_" + key, value)
 
     def implicitly_wait(self, timeout):
         """set default timeout when click"""
         self._d.wait_timeout = timeout
 
     @property
-    def logger(self):
-        expect_level = (
-            logging.DEBUG if self._d.settings["xpath_debug"] else logging.INFO
-        )  # yapf: disable
-        if expect_level != self._logger.level:
-            self._logger.setLevel(expect_level)
-        return self._logger
-
-    @property
     def wait_timeout(self):
         return self._d.wait_timeout
 
     @property
     def _watcher(self):
         return self._d.watcher
 
@@ -172,28 +154,28 @@
         self._event_callbacks[event_name] += [callback]
 
     # def register_callback(action: str, callback):
     #     pass
 
     def send_click(self, x, y):
         if self._click_before_delay:
-            self.logger.debug(
+            logger.debug(
                 "click before delay %.1f seconds", self._click_after_delay
             )
             time.sleep(self._click_before_delay)
 
         # TODO(ssx): should use a better way
         # event callbacks for report generate
         for callback_func in self._event_callbacks["send_click"]:
             callback_func(x, y)
 
         self._d.click(x, y)
 
         if self._click_after_delay:
-            self.logger.debug("click after delay %.1f seconds", self._click_after_delay)
+            logger.debug("click after delay %.1f seconds", self._click_after_delay)
             time.sleep(self._click_after_delay)
 
     def send_longclick(self, x, y):
         self._d.long_click(x, y)
 
     def send_swipe(self, sx, sy, tx, ty):
         self._d.swipe(sx, sy, tx, ty)
@@ -210,52 +192,14 @@
     def match(self, xpath, source=None):
         return len(self(xpath, source).all()) > 0
 
     @deprecated(version="3.0.0", reason="use d.watcher.when(..) instead")
     def when(self, xquery: str):
         return self._watcher.when(xquery)
 
-    @deprecated(version="3.0.0", reason="deprecated")
-    def apply_watch_from_yaml(self, data):
-        """
-        Examples of argument data
-
-            ---
-            - when: "@com.example.app/popup"
-            then: >
-                def callback(d):
-                    d.click(0.5, 0.5)
-            - when: 继续
-            then: click
-        """
-        try:
-            import yaml
-        except ImportError:
-            self.logger.warning("missing lib pyyaml")
-
-        data = yaml.load(data, Loader=yaml.SafeLoader)
-        for item in data:
-            when, then = item["when"], item["then"]
-
-            trigger = lambda: None
-            self.logger.info("%s, %s", when, then)
-            if then == "click":
-                trigger = lambda selector: selector.get_last_match().click()
-                trigger.__doc__ = "click"
-            elif then.lstrip().startswith("def callback"):
-                mod = ModuleType("_inner_module")
-                exec(then, mod.__dict__)
-                trigger = mod.callback
-                trigger.__doc__ = then
-            else:
-                self.logger.warning("Unknown then: %r", then)
-
-            self.logger.debug("When: %r, Trigger: %r", when, trigger.__doc__)
-            self.when(when).call(trigger)
-
     @deprecated(version="3.0.0", reason="use d.watcher.run() instead")
     def run_watchers(self, source=None):
         self._watcher.run()
 
     @deprecated(version="3.0.0", reason="use d.watcher.start(..) instead")
     def watch_background(self, interval: float = 4.0):
         return self._watcher.start(interval)
@@ -278,15 +222,15 @@
             left_time = max(0, deadline - time.time())
             time.sleep(min(0.5, left_time))
 
     def _get_after_watch(self, xpath: Union[str, list], timeout=None):
         if timeout == 0:
             timeout = 0.01
         timeout = timeout or self.wait_timeout
-        self.logger.info("XPath(timeout %.1f) %s", timeout, xpath)
+        logger.info("XPath(timeout %.1f) %s", timeout, xpath)
         deadline = time.time() + timeout
         while True:
             source = self.dump_hierarchy()
 
             selector = self(xpath, source)
             if selector.exists:
                 return selector.get_last_match()
@@ -352,29 +296,26 @@
         if value is None:
             if self._alias_strict:
                 raise XPathError("alias have not found key", key)
             value = key
         return value
 
     def __call__(self, xpath: str, source=None):
-        print("XPATH:", xpath)
         return XPathSelector(self, xpath, source)
 
 
 class XPathSelector(object):
     def __init__(self, parent: XPath, xpath: str = None, source: str = None):
-        self.logger = parent.logger
-
         self._parent = parent
         self._d = parent._d
         self._source = source
         self._last_source = None
         self._position = None
         self._fallback = None
-        self._xpath_list = (strict_xpath(xpath, self.logger),) if xpath else ()
+        self._xpath_list = (strict_xpath(xpath),) if xpath else ()
 
     def __str__(self):
         return f"XPathSelector={'|'.join(self._xpath_list)}"
 
     def copy(self) -> "XPathSelector":
         """copy self"""
         new = XPathSelector(self._parent)
@@ -391,15 +332,15 @@
         the element should match all conditions
         """
         new = self.copy()
         if isinstance(_xpath, (list, tuple)):
             for xp in _xpath:
                 new = new.xpath(xp)
         else:
-            new._xpath_list = new._xpath_list + (strict_xpath(_xpath, self.logger),)
+            new._xpath_list = new._xpath_list + (strict_xpath(_xpath),)
         return new
 
     def child(self, _xpath: str) -> "XPathSelector":
         """
         add child xpath
         """
         if not _xpath.startswith("/"):
@@ -430,37 +371,36 @@
 
         assert callable(func)
         new = self.copy()
         new._fallback = func
         return new
 
     @property
-    def _global_timeout(self):
-        return self._parent.wait_timeout
+    def _global_timeout(self) -> float:
+        if hasattr(self._parent, "wait_timeout") and isinstance(self._parent.wait_timeout, (int, float)):
+            return self._parent.wait_timeout
+        return 20.0
 
-    def all(self, source=None):
-        """
-        Returns:
-            list of XMLElement
-        """
+    def all(self, source=None) -> List["XMLElement"]:
+        """find all matched elements"""
         xml_content = source or self._source or self._parent.dump_hierarchy()
         self._last_source = xml_content
 
         # run-watchers
         hierarchy = source or self._source
         if not hierarchy:
             trigger_count = 0
             for _ in range(5):  # trigger for most 5 times
                 triggered = self._parent._watcher.run(xml_content)
                 if not triggered:
                     break
                 trigger_count += 1
                 xml_content = self._parent.dump_hierarchy()
             if trigger_count:
-                self.logger.debug("watcher triggered %d times", trigger_count)
+                logger.debug("watcher triggered %d times", trigger_count)
 
         if hierarchy is None:
             root = etree.fromstring(str2bytes(xml_content))
         elif isinstance(hierarchy, (str, bytes)):
             root = etree.fromstring(str2bytes(hierarchy))
         elif isinstance(hierarchy, etree._Element):
             root = hierarchy
@@ -518,47 +458,41 @@
         if not self.wait(timeout or self._global_timeout):
             raise XPathElementNotFoundError(self._xpath_list)
         return self.get_last_match()
 
     def get_last_match(self):
         return self.all(self._last_source)[0]
 
-    def get_text(self):
+    def get_text(self) -> Optional[str]:
         """
         get element text
 
         Returns:
             string of node text
 
         Raises:
             XPathElementNotFoundError
         """
-        return self.get().attrib.get("text", "")
+        return self.get().text
 
     def set_text(self, text: str = ""):
         el = self.get()
         self._d.set_fastinput_ime()  # switch ime
         el.click()  # focus input-area
         self._parent.send_text(text)
 
     def wait(self, timeout=None) -> bool:
-        """
-        Args:
-            timeout (float): seconds
-
-        Returns:
-            None or XMLElement
-        """
+        """ wait until element found """
         deadline = time.time() + (timeout or self._global_timeout)
-        while time.time() < deadline:
-            # self.logger.debug("wait %s left %.1fs", self, deadline-time.time())
+        while True:
             if self.exists:
                 return True
+            if time.time() > deadline:
+                return False
             time.sleep(0.2)
-        return False
 
     def match(self) -> Optional["XMLElement"]:
         """
         Returns:
             None or matched XMLElement
         """
         if self.exists:
@@ -577,26 +511,26 @@
             if not self.exists:
                 return True
             time.sleep(0.2)
         return False
 
     def click_nowait(self):
         x, y = self.all()[0].center()
-        self.logger.info("click %d, %d", x, y)
+        logger.info("click %d, %d", x, y)
         self._parent.send_click(x, y)
 
     def click(self, timeout=None):
         """find element and perform click"""
         try:
             el = self.get(timeout=timeout)
             el.click()
         except XPathElementNotFoundError:
             if not self._fallback:
                 raise
-            self.logger.info("element not found, run fallback")
+            logger.info("element not found, run fallback")
             return inject_call(self._fallback, d=self._d)
 
     def click_exists(self, timeout=None) -> bool:
         """return if clicked"""
         try:
             el = self.get(timeout=timeout)
             el.click()
@@ -657,32 +591,14 @@
         """get element full xpath"""
         root = self.elem.getroottree()
         path = root.getpath(self.elem)
         if strip_index:
             path = re.sub(r"\[\d+\]", "", path)  # remove indexes
         return path
 
-    # 模糊对比方法，后来发现直接对比XPath似乎更好一些
-    # def fuzzy_equal(self, xml_element) -> bool:
-    #     root = self.elem.getroottree()
-    #     fullpath = root.getpath(self.elem)
-    #     fullpath = re.sub(r'\[\d+\]', '', fullpath)  # remove indexes
-
-    #     compared_attrs = ("text", "resource-id", "package", "content-desc")
-    #     for name in compared_attrs:
-    #         if self.elem.attrib[name] != xml_element.attrib[name]:
-    #             return False
-
-    #     def _elem2fullpath(el):
-    #         root = el.getroottree()
-    #         fullpath = root.getpath(el)
-    #         return re.sub(r'\[\d+\]', '', fullpath)  # remove indexes
-
-    #     return _elem2fullpath(self.elem) == _elem2fullpath(xml_element.elem)
-
     def center(self):
         """
         Returns:
             (x, y)
         """
         return self.offset(0.5, 0.5)
 
@@ -835,15 +751,15 @@
         return self.elem.attrib.get("text")
 
     @property
     def attrib(self):
         return self.elem.attrib
 
     @property
-    def info(self):
+    def info(self) -> Dict[str, Any]:
         ret = {}
         for key in (
             "text",
             "focusable",
             "enabled",
             "focused",
             "scrollable",
@@ -858,91 +774,8 @@
         ret["longClickable"] = self.attrib.get("long-clickable")
         ret["packageName"] = self.attrib.get("package")
         ret["resourceName"] = self.attrib.get("resource-id")
         ret["resourceId"] = self.attrib.get(
             "resource-id"
         )  # this is better than resourceName
         ret["childCount"] = len(self.elem.getchildren())
-        return ret
-
-
-class AdbUI(DeviceInterface):
-    """
-    Use adb command to run ui test
-    """
-
-    def __init__(self, d: adbutils.AdbDevice):
-        self._d = d
-
-    def click(self, x, y):
-        self._d.click(x, y)
-
-    def swipe(self, sx, sy, ex, ey, duration):
-        self._d.swipe(sx, sy, ex, ey, duration)
-
-    def window_size(self):
-        w, h = self._d.window_size()
-        return w, h
-
-    def dump_hierarchy(self):
-        return self._d.dump_hierarchy()
-
-    def screenshot(self):
-        d = self._d
-        json_output = d.shell(
-            [
-                "LD_LIBRARY_PATH=/data/local/tmp",
-                "/data/local/tmp/minicap",
-                "-i",
-                "2&>/dev/null",
-            ]
-        ).strip()
-        data = json.loads(json_output)
-        w, h, r = data["width"], data["height"], data["rotation"]
-        remote_image_path = "/sdcard/minicap.jpg"
-        d.shell(["rm", remote_image_path])
-        d.shell(
-            [
-                "LD_LIBRARY_PATH=/data/local/tmp",
-                "/data/local/tmp/minicap",
-                "-P",
-                "{0}x{1}@{0}x{1}/{2}".format(w, h, r),
-                "-s",
-                ">" + remote_image_path,
-            ]
-        )  # yapf: disable
-
-        if d.sync.stat(remote_image_path).size == 0:
-            raise RuntimeError("screenshot using minicap error")
-
-        buf = io.BytesIO()
-        for data in d.sync.iter_content(remote_image_path):
-            buf.write(data)
-        return Image.open(buf)
-
-
-if __name__ == "__main__":
-    d = AdbUI(adbutils.adb.device())
-    xpath = XPath(d)
-    # print(d.screenshot())
-    # print(d.dump_hierarchy()[:20])
-    xpath("App").click()
-    xpath("Alarm").click()
-    # init()
-    # import uiautomator2.ext.htmlreport as htmlreport
-
-    # d = uiautomator2.connect()
-    # hrp = htmlreport.HTMLReport(d)
-
-    # # take screenshot before each click
-    # hrp.patch_click()
-    # d.app_start("com.netease.cloudmusic", stop=True)
-
-    # # watchers
-    # d.ext_xpath.when("跳过").click()
-    # # d.ext_xpath.when("知道了").click()
-
-    # # steps
-    # d.ext_xpath("//*[@text='私人FM']/../android.widget.ImageView").click()
-    # d.ext_xpath("下一首").click()
-    # d.ext_xpath.sleep_watch(2)
-    # d.ext_xpath("转到上一层级").click()
+        return ret
```

### Comparing `uiautomator2-3.0.4/PKG-INFO` & `uiautomator2-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: uiautomator2
-Version: 3.0.4
+Version: 3.0.5
 Summary: automator for anroid device
 Home-page: https://github.com/openatx/uiautomator2
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Deprecated
-Requires-Dist: adbutils (>=2.2)
+Requires-Dist: adbutils (>=2.2.3,<3.0.0)
 Requires-Dist: filelock (>=3,<4)
-Requires-Dist: logzero
 Requires-Dist: lxml
 Requires-Dist: packaging (>=20.3)
 Requires-Dist: pillow
 Requires-Dist: progress (>=1.6,<2.0)
 Requires-Dist: requests
 Requires-Dist: retry (>=0,<1)
 Description-Content-Type: text/markdown
 
-# uiautomator2 [![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg)](https://pypi.python.org/pypi/uiautomator2) ![PyPI](https://img.shields.io/pypi/pyversions/uiautomator2.svg)
+# uiautomator2
+[![PyPI](https://img.shields.io/pypi/v/uiautomator2.svg)](https://pypi.python.org/pypi/uiautomator2)
+![PyPI](https://img.shields.io/pypi/pyversions/uiautomator2.svg)
+[![codecov](https://codecov.io/gh/openatx/uiautomator2/graph/badge.svg?token=d0ZLkqorBu)](https://codecov.io/gh/openatx/uiautomator2)
 
 QQ交流群: **815453846**
 
 > 有段时间没有维护这个项目了（可能有两年了），但是最近工作需要又重新研究一下Android原生自动化，当然又调研了Appium，对比下来一看，发现uiautomator2这个项目的运行速度是真的好快，从检测元素到点击，都是毫秒级的，代码也比较好理解。真是没想到以前竟然写出了这么神奇的项目，这么好的项目怎么能让它落灰呢，得好好整一整，一些垃圾代码清理清理。所以项目版本从2.x.x升级到了3.x.x
 
 还在用2.x.x版本的用户，可以先看一下[2to3](docs/2to3.md) 再决定是否要升级3.x.x （我个人还是非常建议升级的）
 
@@ -103,15 +105,15 @@
 - [py-uiautomator2通过悬浮窗让服务长时间可用](https://zhuanlan.zhihu.com/p/688009468) 这个**强烈推荐**看一下
 - [termux里如何部署uiautomator2简介](https://www.cnblogs.com/ze-yan/p/12242383.html) by `成都-测试只会一点点`
 
 ## 相关项目
 - 基于adb协议与Android进行交互的库 [adbutils](https://github.com/openatx/adbutils)
 - 设备管理平台，设备多了就会用到 [atxserver2](https://github.com/openatx/atxserver2) （寻找项目维护人员）
 - [atx-agent](https://github.com/openatx/atx-agent) 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务
-- 类似于uiautomatorviewer，用于查看UI层级结构 https://appinspector.devsleep.com
+- [uiauto.dev](https://uiauto.dev) 用于查看UI层级结构，类似于uiautomatorviewer(用于替代之前写的weditor），用于查看UI层级结构 
 - ~~[weditor](https://github.com/openatx/weditor) 类似于uiautomatorviewer，专门为本项目开发的辅助编辑器(这个暂不维护了~~
 
 **[Installation](#installation)**
 
 **[Connect to a device](#connect-to-a-device)**
 
 **[Command line](#command-line)**
@@ -174,24 +176,24 @@
     ```
     
     测试是否安装成功 `uiautomator2 --help`
     
 2. UI Inspector
 
     ```bash
-    pip install appinspector
+    pip install uiauto-dev
     # 启动
-    appinspector
+    uiauto.dev
     ```
 
-    浏览器打开 https://appinspector.devsleep.com 查看当前设备的界面结构。
+    浏览器打开 https://uiauto.dev 查看当前设备的界面结构。
 
     **appinspector介绍**
 
-    [appinspector](https://github.com/codeskyblue/appinspector) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
+    [uiauto.dev](https://github.com/codeskyblue/uiauto.dev) 是一个独立与uiautomator2之外的一个项目，用于查看图层结构的。属于旧版项目[weditor的重构版本](https://github.com/openatx/weditor)，后续也许会收费（价格肯定物超所值），来支持当前这个项目继续维护下去。感兴趣的可以加群讨论(也包含提需求) QQ群 536481989
 
 # Connect to a device
 There are two ways to connect to the device. 
 
 1. **Through WiFi**
 
 Suppose device IP is `10.0.0.1` and your PC is in the same network.
```


# Comparing `tmp/ceasylog-1.1.1.tar.gz` & `tmp/ceasylog-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceasylog-1.1.1.tar", last modified: Sun Mar 31 06:01:48 2024, max compression
+gzip compressed data, was "ceasylog-1.2.1.tar", last modified: Thu Apr  4 12:26:29 2024, max compression
```

## Comparing `ceasylog-1.1.1.tar` & `ceasylog-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-03-31 06:01:48.326024 ceasylog-1.1.1/
--rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.1.1/LICENSE
--rw-r--r--   0 adminhuang   (501) staff       (20)      230 2024-03-31 06:01:48.325657 ceasylog-1.1.1/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)     4422 2024-03-31 05:40:55.000000 ceasylog-1.1.1/README.md
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-03-31 06:01:48.321750 ceasylog-1.1.1/ceasylog/
--rw-r--r--   0 adminhuang   (501) staff       (20)     4815 2024-03-31 03:39:23.000000 ceasylog-1.1.1/ceasylog/Logger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)     8624 2024-03-31 05:56:39.000000 ceasylog-1.1.1/ceasylog/LoggerConfiger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.1.1/ceasylog/LoggerLevel.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      129 2024-03-27 14:42:18.000000 ceasylog-1.1.1/ceasylog/__init__.py
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-03-31 06:01:48.325050 ceasylog-1.1.1/ceasylog.egg-info/
--rw-r--r--   0 adminhuang   (501) staff       (20)      230 2024-03-31 06:01:48.000000 ceasylog-1.1.1/ceasylog.egg-info/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)      276 2024-03-31 06:01:48.000000 ceasylog-1.1.1/ceasylog.egg-info/SOURCES.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-03-31 06:01:48.000000 ceasylog-1.1.1/ceasylog.egg-info/dependency_links.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-03-31 06:01:48.000000 ceasylog-1.1.1/ceasylog.egg-info/requires.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-03-31 06:01:48.000000 ceasylog-1.1.1/ceasylog.egg-info/top_level.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-03-31 06:01:48.326138 ceasylog-1.1.1/setup.cfg
--rw-r--r--   0 adminhuang   (501) staff       (20)      359 2024-03-31 05:41:53.000000 ceasylog-1.1.1/setup.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.645442 ceasylog-1.2.1/
+-rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.2.1/LICENSE
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-04 12:26:29.645079 ceasylog-1.2.1/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)     6079 2024-04-04 12:26:11.000000 ceasylog-1.2.1/README.md
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.642202 ceasylog-1.2.1/ceasylog/
+-rw-r--r--   0 adminhuang   (501) staff       (20)     7239 2024-04-04 12:22:40.000000 ceasylog-1.2.1/ceasylog/Logger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)    11433 2024-04-04 12:19:51.000000 ceasylog-1.2.1/ceasylog/LoggerConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.2.1/ceasylog/LoggerLevel.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      633 2024-04-04 11:52:17.000000 ceasylog-1.2.1/ceasylog/LoggerNetworkConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      213 2024-04-04 11:52:17.000000 ceasylog-1.2.1/ceasylog/__init__.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.644731 ceasylog-1.2.1/ceasylog.egg-info/
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)      310 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/SOURCES.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/dependency_links.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       18 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/requires.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/top_level.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-04-04 12:26:29.645510 ceasylog-1.2.1/setup.cfg
+-rw-r--r--   0 adminhuang   (501) staff       (20)      371 2024-04-04 05:48:58.000000 ceasylog-1.2.1/setup.py
```

### Comparing `ceasylog-1.1.1/LICENSE` & `ceasylog-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ceasylog-1.1.1/README.md` & `ceasylog-1.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # CEasyLog
 
 一个简单的日志记录工具
 
-更新时间 2024-03-31 
+更新时间 2024-04-04 
 
 ## 介绍
 
 您可以使用CEasyLog来优雅的记录和打印程序运行过程中的日志信息
 
 ## 安装
 
@@ -97,14 +97,16 @@
 logger.warn("这是一条警告日志")
 logger.error("这是一条错误日志")
 logger.critical("这是一条严重错误日志")
 ```
 
 ## 更多功能
 
+**注：所有的相关demo都在项目/demo文件夹中**
+
 ### 配置继承
 
 不同的日志记录器之间的配置可以进行继承
 
 ```python
 """
 配置继承的使用
@@ -124,18 +126,18 @@
 # 修改一下继承的内容
 loggerCfgChild.setName("child")
 
 loggerFather = Logger(loggerCfgFather)
 loggerChild = Logger(loggerCfgChild)
 
 # 这父子两除了名字外其他都一样
-loggerFather.info("俺是他爹er")
-loggerChild.info("俺是他崽er")
+loggerFather.info("俺是他爹")
+loggerChild.info("俺是他崽")
 
-# 另外继承是可以不断连续的 (子可以有孙 孙可以有曾孙.....子子孙孙无穷匮也)
+# 另外继承是可以不断继续的 (子可以有孙 孙可以有曾孙.....子子孙孙无穷匮也)
 
 ```
 
 ### 配置文件
 
 配置文件可以更加方便的设置日志记录
 
@@ -186,12 +188,74 @@
 logger.error("错误信息")
 logger.critical("严重错误信息")
 
 ```
 
 其中配置文件路径可以为绝对路径 或者是相对于主脚本运行目录的相对路径
 
+#### 推送至网络服务器
+
+ceasylog支持把日志信息推送到您自建的日志服务器上
+
+```python
+"""
+向网络服务器发送日志信息
+
+注意：ceasylog仅提供一个接口请求门面 具体的服务端请您手动实现
+请求的方式使用POST 发送的数据为json
+服务端接收到的内容：
+{
+        "uid": 日志uid, string
+        "msg": 日志内容, string
+        "level": 日志等级 INFO | DEBUG | WARN | ERROR | CRITICAL, enum(string)
+        "time": 记录时间，string(timestamp)
+}
+请求头默认带Content-Type: application/json, 您可以结合自身业务需要自定义 也可及结合服务端实现鉴权需求
+"""
+
+from ceasylog import *
+
+loggerCfg = LoggerConfiger()
+loggerCfg.setName(__name__)
+
+# 创建网络配置器
+loggerNetworkCfg = LoggerNetworkConfiger()
+# 指定目标服务器
+loggerNetworkCfg.setEndpoint("http://127.0.0.1:8080/log")
+# 可以使用setHeader设置请求头 默认带Content-Type: application/json
+# loggerNetworkCfg.setHeader()
+
+# 设置使用网络日志服务器
+loggerCfg.setNetwork(loggerNetworkCfg)
+
+logger = Logger(loggerCfg)
+
+logger.debug("调试信息")
+logger.info("一般信息")
+logger.warn("警告信息")
+logger.error("错误信息")
+logger.critical("严重错误信息")
+
+
+# 服务端可参考下面 flask实现
+
+# from flask import Flask, request
+# from flask_cors import CORS
+#
+# app = Flask(__name__)
+# CORS(app)
+#
+# @app.route("/log", methods=['POST'])
+# def log():
+#     # print(request.headers)
+#     print(request.json)
+#     return "ok."
+#
+# if __name__ == '__main__':
+#     app.run(port=8080)
+```
+
 ## 作者
 
 糖星科技@黄旭东
 
 CandyStar@HuangXudong
```

### Comparing `ceasylog-1.1.1/ceasylog/LoggerConfiger.py` & `ceasylog-1.2.1/ceasylog/LoggerConfiger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import ceasylog
 import ceasylog.LoggerLevel as LoggerLevel
+from ceasylog.LoggerNetworkConfiger import LoggerNetworkConfiger
 
 
 class LoggerConfiger(object):
 
     def __init__(self):
         self.__name = "default"
 
@@ -14,14 +16,17 @@
         self.__printTimeFormat = "%Y-%m-%d %H:%M:%S.%f"
         self.__recordTimeFormat = "%Y-%m-%d %H:%M:%S.%f"
         self.__recordPathNameFormat = "%Y-%m-%d"
 
         self.__isRecordB = False
         self.__recordPath = "./"
 
+        self.__isRecordNetworkB = False
+        self.__networkRecordCfg: LoggerNetworkConfiger = LoggerNetworkConfiger()
+
     @property
     def name(self):
         return self.__name
 
     @property
     def maxPrintLevel(self):
         return self.__maxPrintLevel
@@ -54,14 +59,22 @@
     def isRecordB(self):
         return self.__isRecordB
 
     @property
     def recordPath(self):
         return self.__recordPath
 
+    @property
+    def isRecordNetworkB(self):
+        return self.__isRecordNetworkB
+
+    @property
+    def networkRecordCfg(self):
+        return self.__networkRecordCfg
+
     def loadFromFile(self, path: str):
         import os
         import json
         if not os.path.isabs(path):
             # 拼接解释器运行路径作为绝对路径
             path = os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
         if not os.path.exists(path):
@@ -72,14 +85,20 @@
             configObject: dict = json.loads(fileContent)
         except Exception as e:
             raise Exception(f"Could not read LoggerConfiger config file: {path} because {str(e)}")
         for key in configObject.keys():
             value = configObject[key]
             if key == "name":
                 self.setName(value)
+            elif key == "version":
+                fileVersion = float(str(value).split(".")[0] + "." + str(value).split(".")[1])
+                version = float(str(ceasylog.VERSION).split(".")[0] + "." + str(ceasylog.VERSION).split(".")[1])
+                if fileVersion > version:
+                    raise Exception(f"LoggerConfiger file version {fileVersion} is higher than ceasylog "
+                                    f"version {version}")
             elif key == "maxPrintLevel":
                 if value == "CRITICAL":
                     value = LoggerLevel.CRITICAL
                 elif value == "ERROR":
                     value = LoggerLevel.ERROR
                 elif value == "WARN":
                     value = LoggerLevel.WARN
@@ -136,35 +155,75 @@
                 self.setPrintTimeFormat(value)
             elif key == "recordTimeFormat":
                 self.setRecordTimeFormat(value)
             elif key == "recordPathNameFormat":
                 self.setRecordPathNameFormat(value)
             elif key == "isRecord":
                 self.isRecord(value)
+            elif key == "network":
+                endpoint = value["endpoint"]
+                header = value["header"]
+                networkCfg = LoggerNetworkConfiger()
+                networkCfg.setEndpoint(endpoint)
+                networkCfg.setHeader(header)
+                self.setNetwork(networkCfg)
             else:
                 raise KeyError(f"Paser LoggerConfiger failed: Unknown key {key}")
 
     def saveToFile(self, path: str):
         import os
         import json
         # 存储为配置文件的内容
-        if self.isRecordB:
+        if self.__isRecordB and self.__isRecordNetworkB:
+            configObject = {
+                "version": ceasylog.VERSION,
+                "name": self.name,
+                "maxPrintLevel": self.maxPrintLevel.des,
+                "minPrintLevel": self.minPrintLevel.des,
+                "maxRecordLevel": self.maxRecordLevel.des,
+                "minRecordLevel": self.minRecordLevel.des,
+                "printTimeFormat": self.printTimeFormat,
+                "network": {
+                    "endpoint": self.__networkRecordCfg.endpoint,
+                    "header": self.__networkRecordCfg.header
+                },
+                "recordTimeFormat": self.recordTimeFormat,
+                "recordPathNameFormat": self.recordPathNameFormat,
+                "isRecord": self.recordPath
+            }
+        elif self.isRecordB:
             configObject = {
+                "version": ceasylog.VERSION,
                 "name": self.name,
                 "maxPrintLevel": self.maxPrintLevel.des,
                 "minPrintLevel": self.minPrintLevel.des,
                 "maxRecordLevel": self.maxRecordLevel.des,
                 "minRecordLevel": self.minRecordLevel.des,
                 "printTimeFormat": self.printTimeFormat,
                 "recordTimeFormat": self.recordTimeFormat,
                 "recordPathNameFormat": self.recordPathNameFormat,
                 "isRecord": self.recordPath
             }
+        elif self.__isRecordNetworkB:
+            configObject = {
+                "version": ceasylog.VERSION,
+                "name": self.name,
+                "maxPrintLevel": self.maxPrintLevel.des,
+                "minPrintLevel": self.minPrintLevel.des,
+                "maxRecordLevel": self.maxRecordLevel.des,
+                "minRecordLevel": self.minRecordLevel.des,
+                "printTimeFormat": self.printTimeFormat,
+                "network": {
+                    "endpoint": self.__networkRecordCfg.endpoint,
+                    "header": self.__networkRecordCfg.header
+                }
+            }
         else:
             configObject = {
+                "version": ceasylog.VERSION,
                 "name": self.name,
                 "maxPrintLevel": self.maxPrintLevel.des,
                 "minPrintLevel": self.minPrintLevel.des,
                 "maxRecordLevel": self.maxRecordLevel.des,
                 "minRecordLevel": self.minRecordLevel.des,
                 "printTimeFormat": self.printTimeFormat,
             }
@@ -216,15 +275,19 @@
     def setPrintTimeFormat(self, printTimeFormat: str):
         self.__printTimeFormat = printTimeFormat
 
     def setRecordTimeFormat(self, recordTimeFormat: str):
         self.__recordTimeFormat = recordTimeFormat
 
     def setRecordPathNameFormat(self, printTimeFormat: str):
-        self.__printTimeFormat = printTimeFormat
+        self.__recordPathNameFormat = printTimeFormat
 
     def isRecord(self, path: str):
         self.__isRecordB = True
         self.__recordPath = path
 
     def setRecordPath(self, recordPath: str):
         self.__recordPath = recordPath
+
+    def setNetwork(self, config: LoggerNetworkConfiger):
+        self.__isRecordNetworkB = True
+        self.__networkRecordCfg = config
```

### Comparing `ceasylog-1.1.1/ceasylog/LoggerLevel.py` & `ceasylog-1.2.1/ceasylog/LoggerLevel.py`

 * *Files identical despite different names*


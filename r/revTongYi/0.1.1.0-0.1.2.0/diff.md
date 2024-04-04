# Comparing `tmp/revtongyi-0.1.1.0.tar.gz` & `tmp/revtongyi-0.1.2.0.tar.gz`

## Comparing `revtongyi-0.1.1.0.tar` & `revtongyi-0.1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/revTongYi/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/revTongYi/entity.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/revTongYi/errors.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/revTongYi/qianwen.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/revTongYi/wanxiang.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/tests/qianwen.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/LICENSE
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 revtongyi-0.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/entity.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/errors.py
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/qianwen.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/wanxiang.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/tests/qianwen.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/LICENSE
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/PKG-INFO
```

### Comparing `revtongyi-0.1.1.0/.github/workflows/publish-pypi.yaml` & `revtongyi-0.1.2.0/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/revTongYi/__init__.py` & `revtongyi-0.1.2.0/revTongYi/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from fake_useragent import UserAgent
 
 from . import qianwen
 
 
 def cli():
     cookies_file_content = []
+    sessionId = ""
     with open("cookies.json", encoding="utf-8") as f:
         cookies_file_content = json.load(f)
 
     cookies_dict = {}
     for it in cookies_file_content:
         cookies_dict[it['name']] = it['value']
 
@@ -25,26 +26,28 @@
 
     lastId = "0"
     while True:
 
         reply_iter = session.ask(
             prompt=question,
             parentId=lastId,
+            sessionId=sessionId,
             stream=True
         )
 
         last_out = ""
 
         print("AI  > ", end="")
 
         for resp in reply_iter:
             lastId = resp.msgId
             if 'contents' in resp:
                 resp_text = resp.contents[-1].content
                 print(resp_text.replace(last_out, ""), end="")
                 last_out = resp_text
+                sessionId = resp.sessionId
         
         question = input("\nYou > ")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `revtongyi-0.1.1.0/revTongYi/entity.py` & `revtongyi-0.1.2.0/revTongYi/entity.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/revTongYi/qianwen.py` & `revtongyi-0.1.2.0/revTongYi/qianwen.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     """Parent msg id"""
 
     def __init__(
             self,
             cookies: dict = None,
             cookies_str: str = "",
     ):
-        self.sessionId = ""
 
         if cookies and cookies_str:
             raise ValueError("cookies和cookies_str不能同时存在")
 
         if cookies:
             self.cookies = cookies
             self.cookies_str = ""
@@ -117,15 +116,15 @@
                     "role": "user"
                 }
             ],
             "mode": "chat",
             "model": "",
             "requestId": gen_request_id(),
             "parentMsgId": parentId,
-            "sessionId": sessionId if sessionId else self.sessionId,
+            "sessionId": sessionId,
             "sessionType": "text_chat" if not image else "image_chat",
             "userAction": "chat"
         }
 
         if image:
             image_link = self.upload_image(image)
             data["contents"].append({
@@ -162,22 +161,26 @@
                     # chunk完整
                     try:
                         pending = pending.split("\n")[-1]
                         pending = pending[6:]
 
                         resp_json = json.loads(pending)
 
+                        if resp_json.get("errorCode"):
+                            raise errors.TongYiProtocolError("unexpected response: {}".format(resp_json))
+
                         pending = ""
 
                         self.parentId = resp_json["msgId"]
-                        self.sessionId = resp_json["sessionId"]
 
                         result = QianWenChatResponse(resp_json)
 
                         yield result
+                    except errors.TongYiProtocolError as e:
+                        raise e
                     except Exception as e:
                         pass
 
         logging.debug("done: {}".format(result))
 
     def _non_stream_ask(
             self,
```

### Comparing `revtongyi-0.1.1.0/revTongYi/wanxiang.py` & `revtongyi-0.1.2.0/revTongYi/wanxiang.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/tests/qianwen.py` & `revtongyi-0.1.2.0/tests/qianwen.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/.gitignore` & `revtongyi-0.1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/LICENSE` & `revtongyi-0.1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.1.0/README.md` & `revtongyi-0.1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 [![PyPi](https://img.shields.io/pypi/v/revTongYi.svg)](https://pypi.python.org/pypi/revTongYi)
 [![Downloads](https://static.pepy.tech/badge/revTongYi)](https://pypi.python.org/pypi/revTongYi)
 
 阿里通义千问、通义万相 Python逆向API
 
 > **近期更改**
 >
-> ### 2024/03/39
+> ### 2024/04/03
+>  - 修改sessionId判断，优化报错
+>
+> ### 2024/03/29
 > - 以对象封装响应数据，方便使用 
 >
 > ### 2024/03/11
 > - 添加识图功能。
 > - 响应数据格式有变动，请尽快适配。
 
 ```bash
@@ -67,14 +70,18 @@
 )
 ```
 
 ### 连续对话
 
 返回值中有`msgId`和`sessionId`，下一次调用`ask`时以`parentId`和`sessionId`传入这两个值，即可继续对话。
 
+### 新建对话
+
+调用`ask`时不传入`sessionId`参数或传入空字符串即可。
+
 ### 列出会话列表
 
 ```python
 sessions = chatbot.list_session()
 ```
 
 ### 删除指定会话
```

### Comparing `revtongyi-0.1.1.0/pyproject.toml` & `revtongyi-0.1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revTongYi"
-version = "0.1.1.0"
+version = "0.1.2.0"
 authors = [
   { name="xw5xr6", email="xw5xr6@hotmail.com" },
   { name="leeeduke", email="dukelee652@gmail.com" }
 ]
 description = "阿里通义千问逆向工程API"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `revtongyi-0.1.1.0/PKG-INFO` & `revtongyi-0.1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: revTongYi
-Version: 0.1.1.0
+Version: 0.1.2.0
 Summary: 阿里通义千问逆向工程API
 Project-URL: Homepage, https://github.com/leeeduke/revTongYi
 Project-URL: Bug Tracker, https://github.com/leeeduke/revTongYi/issues
 Author-email: xw5xr6 <xw5xr6@hotmail.com>, leeeduke <dukelee652@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,18 @@
 [![PyPi](https://img.shields.io/pypi/v/revTongYi.svg)](https://pypi.python.org/pypi/revTongYi)
 [![Downloads](https://static.pepy.tech/badge/revTongYi)](https://pypi.python.org/pypi/revTongYi)
 
 阿里通义千问、通义万相 Python逆向API
 
 > **近期更改**
 >
-> ### 2024/03/39
+> ### 2024/04/03
+>  - 修改sessionId判断，优化报错
+>
+> ### 2024/03/29
 > - 以对象封装响应数据，方便使用 
 >
 > ### 2024/03/11
 > - 添加识图功能。
 > - 响应数据格式有变动，请尽快适配。
 
 ```bash
@@ -84,14 +87,18 @@
 )
 ```
 
 ### 连续对话
 
 返回值中有`msgId`和`sessionId`，下一次调用`ask`时以`parentId`和`sessionId`传入这两个值，即可继续对话。
 
+### 新建对话
+
+调用`ask`时不传入`sessionId`参数或传入空字符串即可。
+
 ### 列出会话列表
 
 ```python
 sessions = chatbot.list_session()
 ```
 
 ### 删除指定会话
```


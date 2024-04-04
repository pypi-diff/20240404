# Comparing `tmp/lyytext-1.8.tar.gz` & `tmp/lyytext-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyytext-1.8.tar", last modified: Thu Mar 21 06:37:54 2024, max compression
+gzip compressed data, was "lyytext-1.9.tar", last modified: Thu Apr  4 15:35:39 2024, max compression
```

## Comparing `lyytext-1.8.tar` & `lyytext-1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 06:37:54.285313 lyytext-1.8/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytext-1.8/LICENSE
--rw-rw-rw-   0        0        0      158 2024-03-21 06:37:54.284312 lyytext-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytext-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 06:37:54.282312 lyytext-1.8/lyytext.egg-info/
--rw-rw-rw-   0        0        0      158 2024-03-21 06:37:54.000000 lyytext-1.8/lyytext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-03-21 06:37:54.000000 lyytext-1.8/lyytext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 06:37:54.000000 lyytext-1.8/lyytext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-21 06:37:54.000000 lyytext-1.8/lyytext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8447 2024-03-21 06:37:47.000000 lyytext-1.8/lyytext.py
--rw-rw-rw-   0        0        0       42 2024-03-21 06:37:54.285313 lyytext-1.8/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-03-21 06:37:52.000000 lyytext-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:35:39.859460 lyytext-1.9/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytext-1.9/LICENSE
+-rw-rw-rw-   0        0        0      158 2024-04-04 15:35:39.859460 lyytext-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytext-1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 15:35:39.857462 lyytext-1.9/lyytext.egg-info/
+-rw-rw-rw-   0        0        0      158 2024-04-04 15:35:39.000000 lyytext-1.9/lyytext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-04-04 15:35:39.000000 lyytext-1.9/lyytext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:35:39.000000 lyytext-1.9/lyytext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 15:35:39.000000 lyytext-1.9/lyytext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10526 2024-04-04 15:34:58.000000 lyytext-1.9/lyytext.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:35:39.860462 lyytext-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-04-04 15:35:37.000000 lyytext-1.9/setup.py
```

### Comparing `lyytext-1.8/LICENSE` & `lyytext-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lyytext-1.8/lyytext.py` & `lyytext-1.9/lyytext.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,75 @@
 import re
 import json
 from lyylog import log
 import xml.etree.ElementTree as ET
 
+characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_"
+
+def dingding_extract_packet_size(message,deub=False):
+    # 使用正则表达式定义两个捕获组，提取图片包和尺寸2部分
+    pattern = r'http.*\/(.*)_(\d{2,4}_\d{2,4})'
+    
+    # 使用正则表达式匹配并提取两个分组
+    match = re.search(pattern, message)
+    if match:
+        group1 = match.group(1)
+        group2 = match.group(2)
+        print("group1=",group1,"group2=",group2)
+        return [group1, group2]
+    else:
+        return []
+    
+    
+def encode_number(number,debug=False):
+    """
+    钉钉图片，把尺寸数字转换成字符作为图片包的一部分
+    """
+    # 计算1024的倍数
+    thousands = number // 1024
+    # 获取剩余的数值
+    remainder = number % 1024
+    if debug:print("remainder:",remainder)
+    # 计算16的倍数
+    sixteens = remainder // 16
+    # 获取个位数值（每增加4代表字符集中的下一个字符）
+    units = remainder % 16
+    if debug: print("units:",units)
+    # 将数值转换为对应的字符
+    encoded = characters[thousands] + characters[sixteens] + characters[units * 4+1]
+    return encoded
+
+# 解码函数
+def decode_number(encoded):
+    """
+        钉钉图片，从图片包字符提取尺寸数字
+    """
+    # 将字符转换为对应的数值
+    thousands = characters.index(encoded[0])
+    sixteens = characters.index(encoded[1])
+    units = int(characters.index(encoded[2])/4)
+    
+    # 根据编码规则重建原始的数字
+    number = (thousands * 1024) + (sixteens * 16) + units
+    return number
+
+def txt_to_jd_jsontext(msgtype, chinesename, msg_time, txt, return_json=False):
+    """
+    生成适合在jd控件中显示的json格式文本
+    """
+    msg_json = {}
+    msg_json["msgtype"] = msgtype
+    msg_json["chinesename"] = chinesename
+    msg_json["time"] = msg_time
+    msg_json["message"] = txt
+    if return_json:
+        return msg_json
+    else:
+        return json.dumps(msg_json)
+
 
 def read_xml_branch_value(xml_file=r"D:\Soft\_Stock\KTPro\User\BlockInfo\UserBlockInfo6633458850865152.data", branch_name="BC", attribute_name="ToTDX.", option="Stock"):
     """
     # 解析XML文件,交易师的xml文件是UTF-16编码的，分支名是BC
 
     """
```


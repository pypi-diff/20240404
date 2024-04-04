# Comparing `tmp/py3office-0.2.0.tar.gz` & `tmp/py3office-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3office-0.2.0.tar", last modified: Wed Feb  7 14:14:56 2024, max compression
+gzip compressed data, was "py3office-0.3.0.tar", last modified: Thu Apr  4 02:02:55 2024, max compression
```

## Comparing `py3office-0.2.0.tar` & `py3office-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 14:14:56.606502 py3office-0.2.0/
--rw-rw-rw-   0        0        0       31 2024-01-18 12:56:57.000000 py3office-0.2.0/.mailmap
--rw-rw-rw-   0        0        0      212 2024-01-18 12:56:57.000000 py3office-0.2.0/AUTHORS.txt
--rw-rw-rw-   0        0        0      798 2024-02-07 14:14:37.000000 py3office-0.2.0/CHANGELOG
--rw-rw-rw-   0        0        0     1107 2024-01-18 12:56:57.000000 py3office-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      122 2024-01-18 13:24:39.000000 py3office-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1447 2024-02-07 14:14:56.604505 py3office-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-01-31 11:11:44.000000 py3office-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-07 14:14:56.557347 py3office-0.2.0/docs/
--rw-rw-rw-   0        0        0     1827 2024-02-05 10:49:08.000000 py3office-0.2.0/docs/handler.md
--rw-rw-rw-   0        0        0     1022 2024-02-05 10:49:08.000000 py3office-0.2.0/docs/pdf.md
--rw-rw-rw-   0        0        0     8294 2024-01-18 12:56:57.000000 py3office-0.2.0/logo.jpeg
--rw-rw-rw-   0        0        0       42 2024-02-07 14:14:56.606502 py3office-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1070 2024-02-07 14:14:51.000000 py3office-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-07 14:14:56.513483 py3office-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-07 14:14:56.568799 py3office-0.2.0/src/py3office/
--rw-rw-rw-   0        0        0       20 2024-02-01 12:15:55.000000 py3office-0.2.0/src/py3office/__init__.py
--rw-rw-rw-   0        0        0     3002 2024-02-05 10:49:08.000000 py3office-0.2.0/src/py3office/handler.py
--rw-rw-rw-   0        0        0     3427 2024-02-05 10:49:08.000000 py3office-0.2.0/src/py3office/pdf.py
-drwxrwxrwx   0        0        0        0 2024-02-07 14:14:56.601589 py3office-0.2.0/src/py3office.egg-info/
--rw-rw-rw-   0        0        0     1447 2024-02-07 14:14:55.000000 py3office-0.2.0/src/py3office.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-02-07 14:14:56.000000 py3office-0.2.0/src/py3office.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 14:14:55.000000 py3office-0.2.0/src/py3office.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-02-07 14:14:56.000000 py3office-0.2.0/src/py3office.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-07 14:14:56.000000 py3office-0.2.0/src/py3office.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 02:02:55.550177 py3office-0.3.0/
+-rw-rw-rw-   0        0        0       31 2024-03-22 11:26:22.000000 py3office-0.3.0/.mailmap
+-rw-rw-rw-   0        0        0      212 2024-03-22 11:26:22.000000 py3office-0.3.0/AUTHORS.txt
+-rw-rw-rw-   0        0        0      927 2024-04-04 02:01:50.000000 py3office-0.3.0/CHANGELOG
+-rw-rw-rw-   0        0        0     1107 2024-03-22 11:26:22.000000 py3office-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-03-22 11:26:22.000000 py3office-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1498 2024-04-04 02:02:55.548181 py3office-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-03-22 11:26:22.000000 py3office-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 02:02:55.474379 py3office-0.3.0/docs/
+-rw-rw-rw-   0        0        0     1827 2024-03-22 11:26:22.000000 py3office-0.3.0/docs/handler.md
+-rw-rw-rw-   0        0        0      267 2024-03-22 11:26:23.000000 py3office-0.3.0/docs/ocr.md
+-rw-rw-rw-   0        0        0     1022 2024-03-22 11:26:23.000000 py3office-0.3.0/docs/pdf.md
+-rw-rw-rw-   0        0        0     8294 2024-03-22 11:26:23.000000 py3office-0.3.0/logo.jpeg
+-rw-rw-rw-   0        0        0       42 2024-04-04 02:02:55.550177 py3office-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-04 02:02:03.000000 py3office-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:02:55.414539 py3office-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 02:02:55.492331 py3office-0.3.0/src/py3office/
+-rw-rw-rw-   0        0        0       20 2024-03-22 11:26:23.000000 py3office-0.3.0/src/py3office/__init__.py
+-rw-rw-rw-   0        0        0     3002 2024-03-22 11:26:23.000000 py3office-0.3.0/src/py3office/handler.py
+-rw-rw-rw-   0        0        0      269 2024-03-22 11:26:23.000000 py3office-0.3.0/src/py3office/ocr.py
+-rw-rw-rw-   0        0        0     3427 2024-03-22 11:26:23.000000 py3office-0.3.0/src/py3office/pdf.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:02:55.544193 py3office-0.3.0/src/py3office.egg-info/
+-rw-rw-rw-   0        0        0     1498 2024-04-04 02:02:54.000000 py3office-0.3.0/src/py3office.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-04 02:02:54.000000 py3office-0.3.0/src/py3office.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 02:02:54.000000 py3office-0.3.0/src/py3office.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-04 02:02:54.000000 py3office-0.3.0/src/py3office.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 02:02:54.000000 py3office-0.3.0/src/py3office.egg-info/top_level.txt
```

### Comparing `py3office-0.2.0/CHANGELOG` & `py3office-0.3.0/CHANGELOG`

 * *Files 17% similar despite different names*

```diff
@@ -19,7 +19,13 @@
             * listFolder 遍历所有文件夹
             * getFiles 获取所有子文件
             * copy 复制文件或文件夹
             * write 文本写入文件
         2、py3office.pdf
             * toWord 把pdf转成word
             * logInfo 打印pdf内容
+v0.3.0:
+    date:2024-04-04
+    changes:
+      - 新增功能
+        1、py3office.ocr
+            * toTexts 图片变成列表
```

### Comparing `py3office-0.2.0/LICENSE` & `py3office-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3office-0.2.0/README.md` & `py3office-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <img src="./logo.jpeg" />
 
-# [py3office](https://github.com/fragement-contrib/py3office)
+# [py3office](https://github.com/zxl20070701/py3office)
 ⏰ 提供python3版本的自动化办公常用处理方法
 
 <p>
-    <a href="https://github.com/fragement-contrib/py3office" target='_blank'>
-        <img alt="GitHub repo stars" src="https://img.shields.io/github/stars/fragement-contrib/py3office?style=social">
+    <a href="https://github.com/zxl20070701/py3office" target='_blank'>
+        <img alt="GitHub repo stars" src="https://img.shields.io/github/stars/zxl20070701/py3office?style=social">
     </a>
 </p>
 
 ## 使用
 
 首先需要进行安装：
 
@@ -17,13 +17,14 @@
 pip3 install py3office
 ```
 
 然后就可以使用了，下面列出所有可用内容：
 
 - [handler 基本辅助相关](./docs/handler.md)
 - [PDF文件相关操作](./docs/pdf.md)
+- [OCR相关操作](./docs/ocr.md)
 
 ## 版权
 
 MIT License
 
 Copyright (c) [zxl20070701](https://zxl20070701.github.io/notebook/home.html) 走一步，再走一步
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-[./logo.jpeg]# [py3office](https://github.com/fragement-contrib/py3office) â°
+[./logo.jpeg]# [py3office](https://github.com/zxl20070701/py3office) â°
 æä¾python3çæ¬çèªå¨ååå¬å¸¸ç¨å¤çæ¹æ³
 _[_G_i_t_H_u_b_ _r_e_p_o_ _s_t_a_r_s_]
 ## ä½¿ç¨ é¦åéè¦è¿è¡å®è£ï¼ ``` pip3 install py3office ```
 ç¶åå°±å¯ä»¥ä½¿ç¨äºï¼ä¸é¢ååºææå¯ç¨åå®¹ï¼ - [handler
 åºæ¬è¾å©ç¸å³](./docs/handler.md) - [PDFæä»¶ç¸å³æä½](./docs/pdf.md)
-## çæ MIT License Copyright (c) [zxl20070701](https://
-zxl20070701.github.io/notebook/home.html) èµ°ä¸æ­¥ï¼åèµ°ä¸æ­¥
+- [OCRç¸å³æä½](./docs/ocr.md) ## çæ MIT License Copyright (c)
+[zxl20070701](https://zxl20070701.github.io/notebook/home.html)
+èµ°ä¸æ­¥ï¼åèµ°ä¸æ­¥
```

### Comparing `py3office-0.2.0/docs/handler.md` & `py3office-0.3.0/docs/handler.md`

 * *Files identical despite different names*

### Comparing `py3office-0.2.0/docs/pdf.md` & `py3office-0.3.0/docs/pdf.md`

 * *Files identical despite different names*

### Comparing `py3office-0.2.0/logo.jpeg` & `py3office-0.3.0/logo.jpeg`

 * *Files identical despite different names*

### Comparing `py3office-0.2.0/setup.py` & `py3office-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 #!/usr/bin/python3
 
 from setuptools import setup
 
 readmeFile = open("README.md", "r", encoding="utf-8")
 long_description = readmeFile.read().replace(
-    "./docs/", "https://github.com/fragement-contrib/py3office/blob/master/docs/"
+    "./docs/", "https://github.com/zxl20070701/py3office/blob/master/docs/"
 )
 readmeFile.close()
 
 # https://setuptools.pypa.io/en/latest/setuptools.html
 
 setup(
     name="py3office",
-    version="0.2.0",
+    version="0.3.0",
     description="提供python3版本的自动化办公常用处理方法",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zxl20070701",
     author_email="1904314465@qq.com",
     maintainer="zxl20070701",
     maintainer_email="1904314465@qq.com",
     package_dir={"": "src"},
     packages=["py3office"],
-    url="https://github.com/fragement-contrib/py3office",
+    url="https://github.com/zxl20070701/py3office",
     license="MIT",
     keywords=["pdf", "office", "python3"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["PyMuPDF>=1.23.16", "pdf2docx>=0.5.8"],
+    install_requires=[
+        "PyMuPDF>=1.23.16",
+        "pdf2docx>=0.5.8",
+        "cnocr>=2.3.0.1",
+        "onnxruntime>=1.17.1",
+    ],
 )
```

### Comparing `py3office-0.2.0/src/py3office/handler.py` & `py3office-0.3.0/src/py3office/handler.py`

 * *Files identical despite different names*

### Comparing `py3office-0.2.0/src/py3office/pdf.py` & `py3office-0.3.0/src/py3office/pdf.py`

 * *Files identical despite different names*


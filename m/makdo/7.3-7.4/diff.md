# Comparing `tmp/makdo-7.3.tar.gz` & `tmp/makdo-7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makdo-7.3.tar", last modified: Tue Apr  2 04:27:52 2024, max compression
+gzip compressed data, was "makdo-7.4.tar", last modified: Wed Apr  3 23:53:31 2024, max compression
```

## Comparing `makdo-7.3.tar` & `makdo-7.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 say       (1000) say       (1000)        0 2024-04-02 04:27:52.796294 makdo-7.3/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-02 04:27:52.796294 makdo-7.3/PKG-INFO
--rw-------   0 say       (1000) say       (1000)    17888 2024-04-02 04:27:44.000000 makdo-7.3/README.txt
-drwx------   0 say       (1000) say       (1000)        0 2024-04-02 04:27:52.792294 makdo-7.3/makdo/
--rw-------   0 say       (1000) say       (1000)      137 2024-04-02 04:27:44.000000 makdo-7.3/makdo/__init__.py
--rwx------   0 say       (1000) say       (1000)   262576 2024-04-02 04:27:44.000000 makdo-7.3/makdo/makdo_docx2md.py
--rwx------   0 say       (1000) say       (1000)     4201 2024-04-02 04:27:44.000000 makdo-7.3/makdo/makdo_gui.py
--rwx------   0 say       (1000) say       (1000)   237761 2024-04-02 04:27:44.000000 makdo-7.3/makdo/makdo_md2docx.py
-drwx------   0 say       (1000) say       (1000)        0 2024-04-02 04:27:52.796294 makdo-7.3/makdo.egg-info/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-02 04:27:52.000000 makdo-7.3/makdo.egg-info/PKG-INFO
--rw-------   0 say       (1000) say       (1000)      246 2024-04-02 04:27:52.000000 makdo-7.3/makdo.egg-info/SOURCES.txt
--rw-------   0 say       (1000) say       (1000)        1 2024-04-02 04:27:52.000000 makdo-7.3/makdo.egg-info/dependency_links.txt
--rw-------   0 say       (1000) say       (1000)       32 2024-04-02 04:27:52.000000 makdo-7.3/makdo.egg-info/requires.txt
--rw-------   0 say       (1000) say       (1000)        6 2024-04-02 04:27:52.000000 makdo-7.3/makdo.egg-info/top_level.txt
--rw-------   0 say       (1000) say       (1000)       38 2024-04-02 04:27:52.796294 makdo-7.3/setup.cfg
--rw-------   0 say       (1000) say       (1000)      567 2024-04-02 04:27:44.000000 makdo-7.3/setup.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.155840 makdo-7.4/
+-rw-------   0 say       (1000) say       (1000)    22533 2024-04-03 23:53:31.155840 makdo-7.4/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)    18501 2024-04-03 23:53:23.000000 makdo-7.4/README.txt
+drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.151840 makdo-7.4/makdo/
+-rw-------   0 say       (1000) say       (1000)      137 2024-04-03 23:53:23.000000 makdo-7.4/makdo/__init__.py
+-rwx------   0 say       (1000) say       (1000)   262582 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_docx2md.py
+-rwx------   0 say       (1000) say       (1000)     4201 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_gui.py
+-rwx------   0 say       (1000) say       (1000)   237761 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_md2docx.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.155840 makdo-7.4/makdo.egg-info/
+-rw-------   0 say       (1000) say       (1000)    22533 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)      246 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/SOURCES.txt
+-rw-------   0 say       (1000) say       (1000)        1 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/dependency_links.txt
+-rw-------   0 say       (1000) say       (1000)       32 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/requires.txt
+-rw-------   0 say       (1000) say       (1000)        6 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/top_level.txt
+-rw-------   0 say       (1000) say       (1000)       38 2024-04-03 23:53:31.155840 makdo-7.4/setup.cfg
+-rw-------   0 say       (1000) say       (1000)      567 2024-04-03 23:53:23.000000 makdo-7.4/setup.py
```

### Comparing `makdo-7.3/PKG-INFO` & `makdo-7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.3
+Version: 7.4
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
-Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
+Description: <!-- Time-stamp:   <2024.04.03-09:00:13-JST> -->
         
-        # MAKDO（魔苦怒）
+        # MAKDO（MS Wordの互換アプリ）
         
         ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
         
         〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
         
         〜〜 MS Wordがなくても、MS Word形式のファイルを読み書きできます 〜〜
         
         〜〜 わずらわしいナンバリング（番号付け）やインデント（字下げ）から、あなたを解放します 〜〜
         
         ## 注意事項
         
+        ### Python3について
+        
+        簡易実行ファイルは単独で実行できますので不要ですが、
         このアプリ（ライブラリ）は、Python3（Pythonのバージョン3）以上を想定しています。
         
         以下の説明では`python`という表記は、システムによっては`python3`等を意味する場合があります。
         
         `python`をうまく実行できない場合には、`python`の実行ファイルをフルパスで指定するか、
         環境変数PATHの設定をお願いします。
         
+        ### MS Wordの機能の実装状況について
+        
+        MS Wordの機能のうち、
+        日常使用する機能のかなりの部分は実装できていますが、
+        実装できていない機能もたくさんあります。
+        
         ## とりあえず使いたい方へ
         
         ※ 現在、macOSの開発環境がないため、macOS用の簡易実行ファイルはありません。
         どなたかご協力いただけますと助かります。
         
         こんな感じで、Markdown形式のファイルからMS Word形式のファイルを作ったり、その逆ができたりします。
         
@@ -69,15 +78,17 @@
         公用文書書式のMS Word形式のファイルからMarkdown形式のファイルを作成できます。
         
         Markdown形式のファイルから公用文書書式のMS Word形式のファイルを作成することで、
         次のような恩恵があります。
         
         - 「第1、第2…」や「ア、イ…」などのナンバリングを自動でやってくれるようになります
         - インデント（字下げ）を自動でやってくれるようになり、手作業で設定する必要がなくなります
-        - 草冠が「十十」の花などの異字体を「花6;」などと書くことで簡単に使えます
+        - 草冠が「十十」の花などの異字体（人名漢字）を「花6;」などと書くことで簡単に使えます
+        - 簡単なスクリプトが使えるので、金額などを自動で計算してくれるようになります（超便利！）
+        - 簡単なスクリプトが使えるので、1か所を変更したら、他の所にも反映するようにできます
         - `grep`コマンドを使って、過去に作成した書面に検索をかけられるようになります
         - `diff`コマンドを使って、原稿間の違いを確認できるようになります
         - 定型文書をコンピューターで自動で作成できるようになります
         - LinuxやFreeBSDで弁護士の仕事ができるようになります
         
         **見出し機能などのMS Wordの特別な機能は、あえて使っていません。
         これは、見出し機能などの特別な機能を使わなくても公用文書書式を実現できる一方で、
```

### Comparing `makdo-7.3/README.txt` & `makdo-7.4/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-<!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
+<!-- Time-stamp:   <2024.04.03-09:00:13-JST> -->
 
-# MAKDO（魔苦怒）
+# MAKDO（MS Wordの互換アプリ）
 
 ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
 
 〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
 
 〜〜 MS Wordがなくても、MS Word形式のファイルを読み書きできます 〜〜
 
 〜〜 わずらわしいナンバリング（番号付け）やインデント（字下げ）から、あなたを解放します 〜〜
 
 ## 注意事項
 
+### Python3について
+
+簡易実行ファイルは単独で実行できますので不要ですが、
 このアプリ（ライブラリ）は、Python3（Pythonのバージョン3）以上を想定しています。
 
 以下の説明では`python`という表記は、システムによっては`python3`等を意味する場合があります。
 
 `python`をうまく実行できない場合には、`python`の実行ファイルをフルパスで指定するか、
 環境変数PATHの設定をお願いします。
 
+### MS Wordの機能の実装状況について
+
+MS Wordの機能のうち、
+日常使用する機能のかなりの部分は実装できていますが、
+実装できていない機能もたくさんあります。
+
 ## とりあえず使いたい方へ
 
 ※ 現在、macOSの開発環境がないため、macOS用の簡易実行ファイルはありません。
 どなたかご協力いただけますと助かります。
 
 こんな感じで、Markdown形式のファイルからMS Word形式のファイルを作ったり、その逆ができたりします。
 
@@ -61,15 +70,17 @@
 公用文書書式のMS Word形式のファイルからMarkdown形式のファイルを作成できます。
 
 Markdown形式のファイルから公用文書書式のMS Word形式のファイルを作成することで、
 次のような恩恵があります。
 
 - 「第1、第2…」や「ア、イ…」などのナンバリングを自動でやってくれるようになります
 - インデント（字下げ）を自動でやってくれるようになり、手作業で設定する必要がなくなります
-- 草冠が「十十」の花などの異字体を「花6;」などと書くことで簡単に使えます
+- 草冠が「十十」の花などの異字体（人名漢字）を「花6;」などと書くことで簡単に使えます
+- 簡単なスクリプトが使えるので、金額などを自動で計算してくれるようになります（超便利！）
+- 簡単なスクリプトが使えるので、1か所を変更したら、他の所にも反映するようにできます
 - `grep`コマンドを使って、過去に作成した書面に検索をかけられるようになります
 - `diff`コマンドを使って、原稿間の違いを確認できるようになります
 - 定型文書をコンピューターで自動で作成できるようになります
 - LinuxやFreeBSDで弁護士の仕事ができるようになります
 
 **見出し機能などのMS Wordの特別な機能は、あえて使っていません。
 これは、見出し機能などの特別な機能を使わなくても公用文書書式を実現できる一方で、
```

### Comparing `makdo-7.3/makdo/makdo_docx2md.py` & `makdo-7.4/makdo/makdo_docx2md.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         docx2md.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-03:19:19-JST>
+# Time-stamp:   <2024.04.04-08:36:04-JST>
 
 # docx2md.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -5767,15 +5767,15 @@
                     = self._decompose_text(res, raw_text, beg_num, end_num)
                 ydepth = len(state) - 1
                 if head_tc != '->':
                     self._step_states(xdepth, ydepth)
                     numbering_revisers \
                         = self._get_numbering_revisers(xdepth, state)
                 head_symbol += '#' * (xdepth + 1) + '-#' * ydepth + ' '
-        raw_text = re.sub(ParagraphSection.r9, '', raw_text)
+        raw_text = re.sub('^' + ParagraphSection.r9, '', raw_text)
         # raw_text = re.sub('^(?:  ?|\t|\u3000|\\. ?|．)', '', raw_text)
         if head_symbol == '':
             self._step_states(0, 0)
             if '+++' in head_font_revisers:
                 head_font_revisers.remove('+++')
             if '+++' in tail_font_revisers:
                 tail_font_revisers.remove('+++')
```

### Comparing `makdo-7.3/makdo/makdo_gui.py` & `makdo-7.4/makdo/makdo_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         makdo-gui.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-13:25:14-JST>
+# Time-stamp:   <2024.04.04-08:49:47-JST>
 
 # makdo-gui.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -44,15 +44,15 @@
 import importlib
 import makdo.makdo_md2docx
 import makdo.makdo_docx2md
 
 
 __version__ = 'v07 Furuichibashi'
 
-VERSION = 'v07.03'
+VERSION = 'v07.04'
 
 WINDOW_SIZE = "601x276"
 
 
 class Makdo:
 
     receipt_number = 0
```

### Comparing `makdo-7.3/makdo/makdo_md2docx.py` & `makdo-7.4/makdo/makdo_md2docx.py`

 * *Files identical despite different names*

### Comparing `makdo-7.3/makdo.egg-info/PKG-INFO` & `makdo-7.4/makdo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.3
+Version: 7.4
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
-Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
+Description: <!-- Time-stamp:   <2024.04.03-09:00:13-JST> -->
         
-        # MAKDO（魔苦怒）
+        # MAKDO（MS Wordの互換アプリ）
         
         ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
         
         〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
         
         〜〜 MS Wordがなくても、MS Word形式のファイルを読み書きできます 〜〜
         
         〜〜 わずらわしいナンバリング（番号付け）やインデント（字下げ）から、あなたを解放します 〜〜
         
         ## 注意事項
         
+        ### Python3について
+        
+        簡易実行ファイルは単独で実行できますので不要ですが、
         このアプリ（ライブラリ）は、Python3（Pythonのバージョン3）以上を想定しています。
         
         以下の説明では`python`という表記は、システムによっては`python3`等を意味する場合があります。
         
         `python`をうまく実行できない場合には、`python`の実行ファイルをフルパスで指定するか、
         環境変数PATHの設定をお願いします。
         
+        ### MS Wordの機能の実装状況について
+        
+        MS Wordの機能のうち、
+        日常使用する機能のかなりの部分は実装できていますが、
+        実装できていない機能もたくさんあります。
+        
         ## とりあえず使いたい方へ
         
         ※ 現在、macOSの開発環境がないため、macOS用の簡易実行ファイルはありません。
         どなたかご協力いただけますと助かります。
         
         こんな感じで、Markdown形式のファイルからMS Word形式のファイルを作ったり、その逆ができたりします。
         
@@ -69,15 +78,17 @@
         公用文書書式のMS Word形式のファイルからMarkdown形式のファイルを作成できます。
         
         Markdown形式のファイルから公用文書書式のMS Word形式のファイルを作成することで、
         次のような恩恵があります。
         
         - 「第1、第2…」や「ア、イ…」などのナンバリングを自動でやってくれるようになります
         - インデント（字下げ）を自動でやってくれるようになり、手作業で設定する必要がなくなります
-        - 草冠が「十十」の花などの異字体を「花6;」などと書くことで簡単に使えます
+        - 草冠が「十十」の花などの異字体（人名漢字）を「花6;」などと書くことで簡単に使えます
+        - 簡単なスクリプトが使えるので、金額などを自動で計算してくれるようになります（超便利！）
+        - 簡単なスクリプトが使えるので、1か所を変更したら、他の所にも反映するようにできます
         - `grep`コマンドを使って、過去に作成した書面に検索をかけられるようになります
         - `diff`コマンドを使って、原稿間の違いを確認できるようになります
         - 定型文書をコンピューターで自動で作成できるようになります
         - LinuxやFreeBSDで弁護士の仕事ができるようになります
         
         **見出し機能などのMS Wordの特別な機能は、あえて使っていません。
         これは、見出し機能などの特別な機能を使わなくても公用文書書式を実現できる一方で、
```

### Comparing `makdo-7.3/setup.py` & `makdo-7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='makdo',
-    version='07.03',
+    version='07.04',
     description='日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Seiichiro HATA',
     author_email='hata48915b@post.nifty.jp',
     url='https://github.com/hata48915b/makdo/',
     license='GPLv3+',
```


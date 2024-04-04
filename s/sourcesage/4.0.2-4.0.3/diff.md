# Comparing `tmp/sourcesage-4.0.2.tar.gz` & `tmp/sourcesage-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.0.2.tar", last modified: Thu Apr  4 15:35:06 2024, max compression
+gzip compressed data, was "sourcesage-4.0.3.tar", last modified: Thu Apr  4 15:45:56 2024, max compression
```

## Comparing `sourcesage-4.0.2.tar` & `sourcesage-4.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:35:06.617576 sourcesage-4.0.2/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.2/LICENSE
--rw-rw-rw-   0        0        0    11085 2024-04-04 15:35:06.615567 sourcesage-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10828 2024-04-04 15:34:49.000000 sourcesage-4.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 15:35:06.618443 sourcesage-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-04-04 15:35:03.000000 sourcesage-4.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:35:06.549863 sourcesage-4.0.2/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 07:25:42.000000 sourcesage-4.0.2/sourcesage/__init__.py
--rw-rw-rw-   0        0        0      856 2024-04-04 14:57:00.000000 sourcesage-4.0.2/sourcesage/cli.py
--rw-rw-rw-   0        0        0     4768 2024-04-04 14:54:29.000000 sourcesage-4.0.2/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:35:06.610055 sourcesage-4.0.2/sourcesage/modules/
--rw-rw-rw-   0        0        0     3885 2024-04-04 13:12:45.000000 sourcesage-4.0.2/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 12:17:15.000000 sourcesage-4.0.2/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 12:17:05.000000 sourcesage-4.0.2/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 13:12:58.000000 sourcesage-4.0.2/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 07:13:56.000000 sourcesage-4.0.2/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 12:15:04.000000 sourcesage-4.0.2/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 12:14:07.000000 sourcesage-4.0.2/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:35:06.577387 sourcesage-4.0.2/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    11085 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 15:35:06.000000 sourcesage-4.0.2/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 15:35:06.613052 sourcesage-4.0.2/tests/
--rw-rw-rw-   0        0        0     2577 2024-04-04 13:09:04.000000 sourcesage-4.0.2/tests/test_sourcesage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.505641 sourcesage-4.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10147 2024-04-04 15:45:56.505641 sourcesage-4.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9890 2024-04-04 15:45:36.000000 sourcesage-4.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:45:56.505641 sourcesage-4.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-04-04 15:45:53.000000 sourcesage-4.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.434631 sourcesage-4.0.3/sourcesage/
+-rw-rw-rw-   0        0        0        0 2024-04-04 07:25:42.000000 sourcesage-4.0.3/sourcesage/__init__.py
+-rw-rw-rw-   0        0        0      856 2024-04-04 14:57:00.000000 sourcesage-4.0.3/sourcesage/cli.py
+-rw-rw-rw-   0        0        0     4768 2024-04-04 14:54:29.000000 sourcesage-4.0.3/sourcesage/core.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.501215 sourcesage-4.0.3/sourcesage/modules/
+-rw-rw-rw-   0        0        0     3885 2024-04-04 13:12:45.000000 sourcesage-4.0.3/sourcesage/modules/ChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1440 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/ChangelogUtils.py
+-rw-rw-rw-   0        0        0     4171 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/DiffChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/EnvFileHandler.py
+-rw-rw-rw-   0        0        0      836 2024-04-04 12:17:15.000000 sourcesage-4.0.3/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-rw-rw-   0        0        0     1291 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/GitHubUtils.py
+-rw-rw-rw-   0        0        0     2227 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/IssuesToMarkdown.py
+-rw-rw-rw-   0        0        0     3036 2024-04-04 12:17:05.000000 sourcesage-4.0.3/sourcesage/modules/StageInfoGenerator.py
+-rw-rw-rw-   0        0        0     2778 2024-04-04 13:12:58.000000 sourcesage-4.0.3/sourcesage/modules/StagedDiffGenerator.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/file_utils.py
+-rw-rw-rw-   0        0        0     3261 2024-04-04 12:15:04.000000 sourcesage-4.0.3/sourcesage/modules/markdown_utils.py
+-rw-rw-rw-   0        0        0     1115 2024-04-04 12:14:07.000000 sourcesage-4.0.3/sourcesage/modules/source_sage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.458994 sourcesage-4.0.3/sourcesage.egg-info/
+-rw-rw-rw-   0        0        0    10147 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.503569 sourcesage-4.0.3/tests/
+-rw-rw-rw-   0        0        0     2577 2024-04-04 13:09:04.000000 sourcesage-4.0.3/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.0.2/LICENSE` & `sourcesage-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/PKG-INFO` & `sourcesage-4.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.2
+Version: 4.0.3
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 
@@ -48,63 +48,36 @@
 ### [DocuMind（リリース後のドキュメント化）](#3-documindリリース後のドキュメント化)
 - プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
-### 設定
-
-1. `SourceSage.py`ファイルと`modules`フォルダを、分析対象のプロジェクトのルートディレクトリにコピーします。
-
-2. 必要に応じて、`config/.SourceSageignore`ファイルを作成し、除外したいファイルやフォルダのパターンを記述します。
-
-3. `config/language_map.json`ファイルを編集し、必要なプログラミング言語とそれに対応するシンタックスハイライトの識別子を設定します。
-
-4. 必要に応じて、`.env`内の以下の設定を変更します：
+### セットアップ
 
 ```bash
-
-REPO_PATH=./
-SOURCE_SAGE_ASSETS_DIR=SourceSageAssets
-CONFIG_DIR=config
-DOCS_DIR=docs
-FOLDERS=./
-IGNORE_FILE=.SourceSageignore
-OUTPUT_FILE=SourceSage.md
-LANGUAGE_MAP_FILE=config/language_map.json
-ISSUE_LOG_DIR=ISSUE_LOG
-
-OWNER=Sunwood-ai-labs
-REPOSITORY=SourceSage
-ISSUES_FILE_NAME=open_issues_filtered.json
-
-ISSUES_RESOLVE_DIR=ISSUES_RESOLVE
-STAGE_INFO_DIR=STAGE_INFO
+pip install sourcesage
 ```
 
-
 ### 実行
 
 ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
 
 ```bash
-python SourceSage.py
+sourcesage
 ```
 
 これにより、以下のファイルが生成されます：
 
 - `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
 - `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
 - `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
 - `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
 
 
-
-
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
 
 IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
```

### Comparing `sourcesage-4.0.2/README.md` & `sourcesage-4.0.3/sourcesage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: sourcesage
+Version: 4.0.3
+Home-page: https://github.com/Sunwood-ai-labs/SourceSage
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: GitPython
+Requires-Dist: requests
+
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">～Transforming code for AI～</h2>
 </p>
 
@@ -38,63 +48,36 @@
 ### [DocuMind（リリース後のドキュメント化）](#3-documindリリース後のドキュメント化)
 - プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
-### 設定
-
-1. `SourceSage.py`ファイルと`modules`フォルダを、分析対象のプロジェクトのルートディレクトリにコピーします。
-
-2. 必要に応じて、`config/.SourceSageignore`ファイルを作成し、除外したいファイルやフォルダのパターンを記述します。
-
-3. `config/language_map.json`ファイルを編集し、必要なプログラミング言語とそれに対応するシンタックスハイライトの識別子を設定します。
-
-4. 必要に応じて、`.env`内の以下の設定を変更します：
+### セットアップ
 
 ```bash
-
-REPO_PATH=./
-SOURCE_SAGE_ASSETS_DIR=SourceSageAssets
-CONFIG_DIR=config
-DOCS_DIR=docs
-FOLDERS=./
-IGNORE_FILE=.SourceSageignore
-OUTPUT_FILE=SourceSage.md
-LANGUAGE_MAP_FILE=config/language_map.json
-ISSUE_LOG_DIR=ISSUE_LOG
-
-OWNER=Sunwood-ai-labs
-REPOSITORY=SourceSage
-ISSUES_FILE_NAME=open_issues_filtered.json
-
-ISSUES_RESOLVE_DIR=ISSUES_RESOLVE
-STAGE_INFO_DIR=STAGE_INFO
+pip install sourcesage
 ```
 
-
 ### 実行
 
 ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
 
 ```bash
-python SourceSage.py
+sourcesage
 ```
 
 これにより、以下のファイルが生成されます：
 
 - `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
 - `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
 - `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
 - `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
 
 
-
-
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
 
 IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
@@ -242,8 +225,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

### Comparing `sourcesage-4.0.2/setup.py` & `sourcesage-4.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sourcesage',
-    version='4.0.2',
+    version='4.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'sourcesage=sourcesage.cli:main',
         ],
     },
     long_description=long_description,
```

### Comparing `sourcesage-4.0.2/sourcesage/cli.py` & `sourcesage-4.0.3/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/core.py` & `sourcesage-4.0.3/sourcesage/core.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.0.3/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.0.3/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.0.3/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.0.3/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.0.3/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.0.3/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.0.3/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.0.3/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.0.3/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/file_utils.py` & `sourcesage-4.0.3/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/markdown_utils.py` & `sourcesage-4.0.3/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage/modules/source_sage.py` & `sourcesage-4.0.3/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: sourcesage
-Version: 4.0.2
-Home-page: https://github.com/Sunwood-ai-labs/SourceSage
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: GitPython
-Requires-Dist: requests
-
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">～Transforming code for AI～</h2>
 </p>
 
@@ -48,63 +38,36 @@
 ### [DocuMind（リリース後のドキュメント化）](#3-documindリリース後のドキュメント化)
 - プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
-### 設定
-
-1. `SourceSage.py`ファイルと`modules`フォルダを、分析対象のプロジェクトのルートディレクトリにコピーします。
-
-2. 必要に応じて、`config/.SourceSageignore`ファイルを作成し、除外したいファイルやフォルダのパターンを記述します。
-
-3. `config/language_map.json`ファイルを編集し、必要なプログラミング言語とそれに対応するシンタックスハイライトの識別子を設定します。
-
-4. 必要に応じて、`.env`内の以下の設定を変更します：
+### セットアップ
 
 ```bash
-
-REPO_PATH=./
-SOURCE_SAGE_ASSETS_DIR=SourceSageAssets
-CONFIG_DIR=config
-DOCS_DIR=docs
-FOLDERS=./
-IGNORE_FILE=.SourceSageignore
-OUTPUT_FILE=SourceSage.md
-LANGUAGE_MAP_FILE=config/language_map.json
-ISSUE_LOG_DIR=ISSUE_LOG
-
-OWNER=Sunwood-ai-labs
-REPOSITORY=SourceSage
-ISSUES_FILE_NAME=open_issues_filtered.json
-
-ISSUES_RESOLVE_DIR=ISSUES_RESOLVE
-STAGE_INFO_DIR=STAGE_INFO
+pip install sourcesage
 ```
 
-
 ### 実行
 
 ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
 
 ```bash
-python SourceSage.py
+sourcesage
 ```
 
 これにより、以下のファイルが生成されます：
 
 - `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
 - `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
 - `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
 - `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
 
 
-
-
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
 
 IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
@@ -252,8 +215,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

### Comparing `sourcesage-4.0.2/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.0.3/sourcesage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.2/tests/test_sourcesage.py` & `sourcesage-4.0.3/tests/test_sourcesage.py`

 * *Files identical despite different names*


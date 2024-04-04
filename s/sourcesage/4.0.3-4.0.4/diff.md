# Comparing `tmp/sourcesage-4.0.3.tar.gz` & `tmp/sourcesage-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.0.3.tar", last modified: Thu Apr  4 15:45:56 2024, max compression
+gzip compressed data, was "sourcesage-4.0.4.tar", last modified: Thu Apr  4 16:09:09 2024, max compression
```

## Comparing `sourcesage-4.0.3.tar` & `sourcesage-4.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.505641 sourcesage-4.0.3/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.3/LICENSE
--rw-rw-rw-   0        0        0    10147 2024-04-04 15:45:56.505641 sourcesage-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9890 2024-04-04 15:45:36.000000 sourcesage-4.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 15:45:56.505641 sourcesage-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-04-04 15:45:53.000000 sourcesage-4.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.434631 sourcesage-4.0.3/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 07:25:42.000000 sourcesage-4.0.3/sourcesage/__init__.py
--rw-rw-rw-   0        0        0      856 2024-04-04 14:57:00.000000 sourcesage-4.0.3/sourcesage/cli.py
--rw-rw-rw-   0        0        0     4768 2024-04-04 14:54:29.000000 sourcesage-4.0.3/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.501215 sourcesage-4.0.3/sourcesage/modules/
--rw-rw-rw-   0        0        0     3885 2024-04-04 13:12:45.000000 sourcesage-4.0.3/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 12:17:15.000000 sourcesage-4.0.3/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 12:17:05.000000 sourcesage-4.0.3/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 13:12:58.000000 sourcesage-4.0.3/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 07:13:56.000000 sourcesage-4.0.3/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 12:15:04.000000 sourcesage-4.0.3/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 12:14:07.000000 sourcesage-4.0.3/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.458994 sourcesage-4.0.3/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    10147 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 15:45:56.000000 sourcesage-4.0.3/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 15:45:56.503569 sourcesage-4.0.3/tests/
--rw-rw-rw-   0        0        0     2577 2024-04-04 13:09:04.000000 sourcesage-4.0.3/tests/test_sourcesage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:09:09.863521 sourcesage-4.0.4/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12430 2024-04-04 16:09:09.861522 sourcesage-4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12173 2024-04-04 16:07:12.000000 sourcesage-4.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 16:09:09.864520 sourcesage-4.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-04-04 16:08:00.000000 sourcesage-4.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:09:09.726520 sourcesage-4.0.4/sourcesage/
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/__init__.py
+-rw-rw-rw-   0        0        0      856 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/cli.py
+-rw-rw-rw-   0        0        0     4768 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/core.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:09:09.857519 sourcesage-4.0.4/sourcesage/modules/
+-rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/ChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/ChangelogUtils.py
+-rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/DiffChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/EnvFileHandler.py
+-rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/GitHubUtils.py
+-rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/IssuesToMarkdown.py
+-rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/StageInfoGenerator.py
+-rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/StagedDiffGenerator.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/file_utils.py
+-rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/markdown_utils.py
+-rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.4/sourcesage/modules/source_sage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:09:09.813526 sourcesage-4.0.4/sourcesage.egg-info/
+-rw-rw-rw-   0        0        0    12430 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 16:09:09.000000 sourcesage-4.0.4/sourcesage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 16:09:09.859522 sourcesage-4.0.4/tests/
+-rw-rw-rw-   0        0        0     2577 2024-04-04 15:59:17.000000 sourcesage-4.0.4/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.0.3/LICENSE` & `sourcesage-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/PKG-INFO` & `sourcesage-4.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.3
+Version: 4.0.4
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 
@@ -13,22 +13,27 @@
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">～Transforming code for AI～</h2>
 </p>
 
 SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
 
+
 ## 更新内容
 
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
 - [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
   - コードの品質と保守性を向上させるためのリファクタリングと機能改善
   - コミットメッセージのフォーマットとタイプの説明を追加
   - コマンドラインからソースコードのリポジトリパスを取得するように修正
   - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0) 
   - [IssueWise](#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
   - [CommitCraft](#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
   - [DocuMind](#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
@@ -50,32 +55,57 @@
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
 ### セットアップ
 
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
 ```bash
 pip install sourcesage
 ```
 
-### 実行
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash
+   cd ~/my_project
+   ```
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
 
-ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
 
 ```bash
-sourcesage
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
-これにより、以下のファイルが生成されます：
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-- `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
-- `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
-- `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
-- `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
```

### Comparing `sourcesage-4.0.3/README.md` & `sourcesage-4.0.4/sourcesage.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,39 @@
+Metadata-Version: 2.1
+Name: sourcesage
+Version: 4.0.4
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
 
 SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
 
+
 ## 更新内容
 
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
 - [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
   - コードの品質と保守性を向上させるためのリファクタリングと機能改善
   - コミットメッセージのフォーマットとタイプの説明を追加
   - コマンドラインからソースコードのリポジトリパスを取得するように修正
   - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0) 
   - [IssueWise](#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
   - [CommitCraft](#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
   - [DocuMind](#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
@@ -40,32 +55,57 @@
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
 ### セットアップ
 
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
 ```bash
 pip install sourcesage
 ```
 
-### 実行
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash
+   cd ~/my_project
+   ```
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
 
-ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
 
 ```bash
-sourcesage
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
-これにより、以下のファイルが生成されます：
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-- `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
-- `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
-- `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
-- `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
@@ -215,8 +255,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

### Comparing `sourcesage-4.0.3/setup.py` & `sourcesage-4.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sourcesage',
-    version='4.0.3',
+    version='4.0.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'sourcesage=sourcesage.cli:main',
         ],
     },
     long_description=long_description,
```

### Comparing `sourcesage-4.0.3/sourcesage/cli.py` & `sourcesage-4.0.4/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/core.py` & `sourcesage-4.0.4/sourcesage/core.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.0.4/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.0.4/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.0.4/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.0.4/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.0.4/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.0.4/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.0.4/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.0.4/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.0.4/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/file_utils.py` & `sourcesage-4.0.4/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/markdown_utils.py` & `sourcesage-4.0.4/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage/modules/source_sage.py` & `sourcesage-4.0.4/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-Metadata-Version: 2.1
-Name: sourcesage
-Version: 4.0.3
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
 
 SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
 
+
 ## 更新内容
 
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
 - [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
   - コードの品質と保守性を向上させるためのリファクタリングと機能改善
   - コミットメッセージのフォーマットとタイプの説明を追加
   - コマンドラインからソースコードのリポジトリパスを取得するように修正
   - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0) 
   - [IssueWise](#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
   - [CommitCraft](#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
   - [DocuMind](#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
@@ -50,32 +45,57 @@
 - プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
 
 
 ## 使用方法
 
 ### セットアップ
 
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
 ```bash
 pip install sourcesage
 ```
 
-### 実行
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash
+   cd ~/my_project
+   ```
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
 
-ターミナルまたはコマンドプロンプトで、プロジェクトのルートディレクトリに移動し、以下のコマンドを実行します：
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
 
 ```bash
-sourcesage
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
-これにより、以下のファイルが生成されます：
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-- `SourceSageAssets/SourceSage.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイル
-- `SourceSageAssets/Changelog`：Gitの変更履歴を保存するディレクトリ
-- `SourceSageAssets/open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイル
-- `SourceSageAssets/STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイル
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 
 ## 1. IssueWise：開発前の課題解決
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
 </p>
@@ -225,8 +245,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

### Comparing `sourcesage-4.0.3/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.0.4/sourcesage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.3/tests/test_sourcesage.py` & `sourcesage-4.0.4/tests/test_sourcesage.py`

 * *Files identical despite different names*


# Comparing `tmp/PAGETools-0.5.1.tar.gz` & `tmp/PAGETools-0.5.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PAGETools-0.5.1.tar", last modified: Tue Nov 21 11:19:10 2023, max compression
+gzip compressed data, was "PAGETools-0.5.2a0.tar", last modified: Thu Apr  4 09:14:39 2024, max compression
```

## Comparing `PAGETools-0.5.1.tar` & `PAGETools-0.5.2a0.tar`

### file list

```diff
@@ -1,80 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.677582 PAGETools-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-21 11:19:00.000000 PAGETools-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-21 11:19:00.000000 PAGETools-0.5.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-11-21 11:19:00.000000 PAGETools-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-21 11:19:00.000000 PAGETools-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-21 11:19:00.000000 PAGETools-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-21 11:19:00.000000 PAGETools-0.5.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/PAGETools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-21 11:19:10.000000 PAGETools-0.5.1/PAGETools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2023-11-21 11:19:10.689582 PAGETools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2023-11-21 11:19:00.000000 PAGETools-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    63816 2023-11-21 11:19:00.000000 PAGETools-0.5.1/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/pagetools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/pagetools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/pagetools/cli/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/analytics/get_char_occurence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/analytics/get_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/analytics/get_text_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.681582 PAGETools-0.5.1/pagetools/cli/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/management/cull.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/cli/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/transformations/change_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/transformations/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/transformations/line2page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/cli/transformations/regularize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/resources/rulesets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/ligatures_consonantal.json
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/ligatures_vocal.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/punctuation.json
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/quotes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/roman_digits.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/spaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/uvius.json
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/resources/rulesets/various.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/Image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/Page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/src/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/extraction/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/src/line2page/
--rw-r--r--   0 runner    (1001) docker     (127)    11511 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/line2page/Line2Page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/line2page/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.685582 PAGETools-0.5.1/pagetools/src/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/regularization/Regularizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/regularization/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/regularization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/pagetools/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/utils/img_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/src/utils/page_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/pagetools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/pagetools/tests/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/tests/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:10.689582 PAGETools-0.5.1/pagetools/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/tests/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pagetools/tests/src/utils/test_page_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-21 11:19:00.000000 PAGETools-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 11:19:10.689582 PAGETools-0.5.1/setup.cfg
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.962539 PAGETools-0.5.2a0/
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.951367 PAGETools-0.5.2a0/.github/
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.953587 PAGETools-0.5.2a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      595 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.953959 PAGETools-0.5.2a0/.github/workflows/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1874 2023-11-21 13:38:58.000000 PAGETools-0.5.2a0/.github/workflows/deploy_docs.yml
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1420 2023-11-21 13:37:46.000000 PAGETools-0.5.2a0/.github/workflows/python-package.yml
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1060 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/.github/workflows/python-publish.yml
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      111 2023-11-21 13:03:39.000000 PAGETools-0.5.2a0/.gitignore
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1073 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/LICENSE.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)       68 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/MANIFEST.in
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.961892 PAGETools-0.5.2a0/PAGETools.egg-info/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     2989 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/PKG-INFO
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     2437 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/SOURCES.txt
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        1 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/dependency_links.txt
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)       48 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/entry_points.txt
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      105 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/requires.txt
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)       10 2024-04-04 09:14:39.000000 PAGETools-0.5.2a0/PAGETools.egg-info/top_level.txt
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     2989 2024-04-04 09:14:39.962285 PAGETools-0.5.2a0/PKG-INFO
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      953 2023-11-21 13:42:27.000000 PAGETools-0.5.2a0/README.md
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.954752 PAGETools-0.5.2a0/assets/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)    63816 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/assets/logo.png
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.955280 PAGETools-0.5.2a0/docs/
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.955448 PAGETools-0.5.2a0/docs/.vitepress/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1731 2023-11-21 13:30:20.000000 PAGETools-0.5.2a0/docs/.vitepress/config.mts
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.955670 PAGETools-0.5.2a0/docs/.vitepress/theme/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      435 2023-11-21 11:31:58.000000 PAGETools-0.5.2a0/docs/.vitepress/theme/index.ts
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     4286 2023-11-21 11:31:58.000000 PAGETools-0.5.2a0/docs/.vitepress/theme/style.css
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      617 2024-04-04 06:54:04.000000 PAGETools-0.5.2a0/docs/index.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      455 2023-11-21 11:44:23.000000 PAGETools-0.5.2a0/docs/installation.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      292 2024-04-04 06:54:04.000000 PAGETools-0.5.2a0/docs/package.json
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.955802 PAGETools-0.5.2a0/docs/tools/
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.956037 PAGETools-0.5.2a0/docs/tools/analytics/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1265 2023-11-21 12:42:21.000000 PAGETools-0.5.2a0/docs/tools/analytics/get_codec.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      476 2023-11-21 12:42:17.000000 PAGETools-0.5.2a0/docs/tools/analytics/get_text_count.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      677 2023-11-21 12:56:31.000000 PAGETools-0.5.2a0/docs/tools/index.md
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.956530 PAGETools-0.5.2a0/docs/tools/transformation/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      343 2023-11-21 12:42:07.000000 PAGETools-0.5.2a0/docs/tools/transformation/change_index.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3115 2023-11-21 12:38:19.000000 PAGETools-0.5.2a0/docs/tools/transformation/extraction.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1911 2023-11-21 12:42:07.000000 PAGETools-0.5.2a0/docs/tools/transformation/line2page.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1112 2023-11-21 12:42:12.000000 PAGETools-0.5.2a0/docs/tools/transformation/regularization.md
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)    96225 2024-04-04 06:54:04.000000 PAGETools-0.5.2a0/docs/yarn.lock
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.956647 PAGETools-0.5.2a0/pagetools/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.956742 PAGETools-0.5.2a0/pagetools/cli/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      721 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.957210 PAGETools-0.5.2a0/pagetools/cli/analytics/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/analytics/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      206 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/analytics/get_char_occurence.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     4768 2024-04-04 08:56:33.000000 PAGETools-0.5.2a0/pagetools/cli/analytics/get_codec.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3251 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/analytics/get_text_count.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.957420 PAGETools-0.5.2a0/pagetools/cli/management/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/management/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1569 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/management/cull.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.958072 PAGETools-0.5.2a0/pagetools/cli/transformations/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/transformations/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1742 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/transformations/change_index.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3963 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/transformations/extract.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     5183 2023-11-21 09:53:20.000000 PAGETools-0.5.2a0/pagetools/cli/transformations/line2page.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     4020 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/cli/transformations/regularize.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.958204 PAGETools-0.5.2a0/pagetools/resources/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.959364 PAGETools-0.5.2a0/pagetools/resources/rulesets/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      762 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/ligatures_consonantal.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      570 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/ligatures_vocal.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)       80 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/punctuation.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      668 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/quotes.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1342 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/roman_digits.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      201 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/spaces.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     5661 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/uvius.json
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      167 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/resources/rulesets/various.json
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.959754 PAGETools-0.5.2a0/pagetools/src/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3242 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/Image.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3354 2023-11-21 07:41:53.000000 PAGETools-0.5.2a0/pagetools/src/Page.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.959994 PAGETools-0.5.2a0/pagetools/src/extraction/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3743 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/extraction/Extractor.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/extraction/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.960250 PAGETools-0.5.2a0/pagetools/src/line2page/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)    11511 2023-11-21 09:27:57.000000 PAGETools-0.5.2a0/pagetools/src/line2page/Line2Page.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/line2page/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.960615 PAGETools-0.5.2a0/pagetools/src/regularization/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      767 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/regularization/Regularizer.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     2778 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/regularization/Rules.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/regularization/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.961209 PAGETools-0.5.2a0/pagetools/src/utils/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/utils/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      720 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/utils/constants.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     3076 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/utils/filesystem.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1432 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/utils/img_processing.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      451 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/src/utils/page_processing.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.961341 PAGETools-0.5.2a0/pagetools/tests/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/tests/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.961456 PAGETools-0.5.2a0/pagetools/tests/src/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/tests/src/__init__.py
+drwxr-xr-x   0 maximiliannoth   (501) staff       (20)        0 2024-04-04 09:14:39.961690 PAGETools-0.5.2a0/pagetools/tests/src/utils/
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)        0 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/tests/src/utils/__init__.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)      321 2023-05-17 13:58:44.000000 PAGETools-0.5.2a0/pagetools/tests/src/utils/test_page_processing.py
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)     1057 2024-04-04 09:14:34.000000 PAGETools-0.5.2a0/pyproject.toml
+-rw-r--r--   0 maximiliannoth   (501) staff       (20)       38 2024-04-04 09:14:39.962586 PAGETools-0.5.2a0/setup.cfg
```

### Comparing `PAGETools-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `PAGETools-0.5.2a0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/.github/workflows/python-package.yml` & `PAGETools-0.5.2a0/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Python package
 
 on:
   push:
     branches: [ main ]
+    paths-ignore:
+      - './README.md'
+      - 'docs/**'
+      - '.github/workflows/deploy_docs.md'
   pull_request:
     branches: [ main ]
+    paths-ignore:
+      - './README.md'
+      - 'docs/**'
+      - '.github/workflows/deploy_docs.md'
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
```

### Comparing `PAGETools-0.5.1/.github/workflows/python-publish.yml` & `PAGETools-0.5.2a0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/LICENSE.md` & `PAGETools-0.5.2a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/PAGETools.egg-info/SOURCES.txt` & `PAGETools-0.5.2a0/PAGETools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 .gitignore
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/deploy_docs.yml
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 PAGETools.egg-info/PKG-INFO
 PAGETools.egg-info/SOURCES.txt
 PAGETools.egg-info/dependency_links.txt
 PAGETools.egg-info/entry_points.txt
 PAGETools.egg-info/requires.txt
 PAGETools.egg-info/top_level.txt
 assets/logo.png
+docs/index.md
+docs/installation.md
+docs/package.json
+docs/yarn.lock
+docs/.vitepress/config.mts
+docs/.vitepress/theme/index.ts
+docs/.vitepress/theme/style.css
+docs/tools/index.md
+docs/tools/analytics/get_codec.md
+docs/tools/analytics/get_text_count.md
+docs/tools/transformation/change_index.md
+docs/tools/transformation/extraction.md
+docs/tools/transformation/line2page.md
+docs/tools/transformation/regularization.md
 pagetools/__init__.py
 pagetools/cli/__init__.py
 pagetools/cli/analytics/__init__.py
 pagetools/cli/analytics/get_char_occurence.py
 pagetools/cli/analytics/get_codec.py
 pagetools/cli/analytics/get_text_count.py
 pagetools/cli/management/__init__.py
```

### Comparing `PAGETools-0.5.1/assets/logo.png` & `PAGETools-0.5.2a0/assets/logo.png`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/__init__.py` & `PAGETools-0.5.2a0/pagetools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/analytics/get_codec.py` & `PAGETools-0.5.2a0/pagetools/cli/analytics/get_codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             json_dicts.append({"character": key, "frequency": value})
 
         with open(output, "w", encoding="utf-8") as outfile:
             json.dump(json_dicts, outfile, indent=4)
     elif out_format == "csv":
         header = ["character", "frequency"]
 
-        with open(output, "w") as outfile:
+        with open(output, "w", encoding="utf-8") as outfile:
             csv_writer = csv.writer(outfile, delimiter=",", quotechar='"', quoting=csv.QUOTE_ALL)
             csv_writer.writerow(header)
             for row in codec:
                 csv_writer.writerow([row, codec[row]])
 
     elif out_format == "txt":
         with open(output, "w", encoding="utf-8") as outfile:
```

### Comparing `PAGETools-0.5.1/pagetools/cli/analytics/get_text_count.py` & `PAGETools-0.5.2a0/pagetools/cli/analytics/get_text_count.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/management/cull.py` & `PAGETools-0.5.2a0/pagetools/cli/management/cull.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/transformations/change_index.py` & `PAGETools-0.5.2a0/pagetools/cli/transformations/change_index.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/transformations/extract.py` & `PAGETools-0.5.2a0/pagetools/cli/transformations/extract.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/transformations/line2page.py` & `PAGETools-0.5.2a0/pagetools/cli/transformations/line2page.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/cli/transformations/regularize.py` & `PAGETools-0.5.2a0/pagetools/cli/transformations/regularize.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/resources/rulesets/ligatures_consonantal.json` & `PAGETools-0.5.2a0/pagetools/resources/rulesets/ligatures_consonantal.json`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/resources/rulesets/ligatures_vocal.json` & `PAGETools-0.5.2a0/pagetools/resources/rulesets/ligatures_vocal.json`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/resources/rulesets/quotes.json` & `PAGETools-0.5.2a0/pagetools/resources/rulesets/quotes.json`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/resources/rulesets/roman_digits.json` & `PAGETools-0.5.2a0/pagetools/resources/rulesets/roman_digits.json`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/resources/rulesets/uvius.json` & `PAGETools-0.5.2a0/pagetools/resources/rulesets/uvius.json`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/Image.py` & `PAGETools-0.5.2a0/pagetools/src/Image.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/Page.py` & `PAGETools-0.5.2a0/pagetools/src/Page.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/extraction/Extractor.py` & `PAGETools-0.5.2a0/pagetools/src/extraction/Extractor.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/line2page/Line2Page.py` & `PAGETools-0.5.2a0/pagetools/src/line2page/Line2Page.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/regularization/Regularizer.py` & `PAGETools-0.5.2a0/pagetools/src/regularization/Regularizer.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/regularization/Rules.py` & `PAGETools-0.5.2a0/pagetools/src/regularization/Rules.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/utils/constants.py` & `PAGETools-0.5.2a0/pagetools/src/utils/constants.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/utils/filesystem.py` & `PAGETools-0.5.2a0/pagetools/src/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pagetools/src/utils/img_processing.py` & `PAGETools-0.5.2a0/pagetools/src/utils/img_processing.py`

 * *Files identical despite different names*

### Comparing `PAGETools-0.5.1/pyproject.toml` & `PAGETools-0.5.2a0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PAGETools"
 description = "Toolset for performing various operations on PAGE XML datasets."
+version="0.5.2a"
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     {name = "Maximilian Nöth", email="maximilian.noeth@uni-wuerzburg.de"}
 ]
 keywords = ["PAGE XML", "OCR", "optical character recognition"]
 license = {file = "LICENSE.md"}
@@ -24,23 +25,22 @@
     "click",
     "flake8",
     "deskew",
     "regex",
     "pytest",
     "importlib_resources ; python_version<'3.7'",
 ]
-dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/uniwuezpd/PAGETools"
 
 [project.scripts]
 pagetools = "pagetools.cli:cli"
 
 [options]
 include_package_data = true
 
 [tool.setuptools.packages.find]
 include = ["pagetools"]
-exclude = ["assets"]
+exclude = ["assets", "docs"]
 
 [tool.setuptools_scm]
```


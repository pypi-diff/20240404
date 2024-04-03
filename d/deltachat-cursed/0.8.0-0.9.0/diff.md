# Comparing `tmp/deltachat_cursed-0.8.0.tar.gz` & `tmp/deltachat-cursed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_cursed-0.8.0.tar", last modified: Fri Dec  2 10:04:48 2022, max compression
+gzip compressed data, was "deltachat-cursed-0.9.0.tar", last modified: Wed Apr  3 23:07:42 2024, max compression
```

## Comparing `deltachat_cursed-0.8.0.tar` & `deltachat-cursed-0.9.0.tar`

### file list

```diff
@@ -1,48 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.099411 deltachat_cursed-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-02 10:04:48.099411 deltachat_cursed-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/docs/user-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/pylama.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/requirements/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   238874 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/screenshots/e1.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 10:04:48.099411 deltachat_cursed-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/src/deltachat_cursed/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/scli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.099411 deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/chatlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2022-12-02 10:04:35.000000 deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:04:48.095411 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-02 10:04:48.000000 deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.082669 deltachat-cursed-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.074669 deltachat-cursed-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.074669 deltachat-cursed-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-03 23:07:42.082669 deltachat-cursed-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.078669 deltachat-cursed-0.9.0/deltachat_cursed/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 23:07:41.000000 deltachat-cursed-0.9.0/deltachat_cursed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/cards_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/chatlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/eventcenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/lazylistwaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/deltachat_cursed/welcome_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.082669 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 23:07:42.000000 deltachat-cursed-0.9.0/deltachat_cursed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.078669 deltachat-cursed-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/docs/user-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:07:42.082669 deltachat-cursed-0.9.0/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    74016 2024-04-03 23:07:29.000000 deltachat-cursed-0.9.0/screenshots/e1.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:07:42.082669 deltachat-cursed-0.9.0/setup.cfg
```

### Comparing `deltachat_cursed-0.8.0/.github/workflows/python-ci.yml` & `deltachat-cursed-0.9.0/.github/workflows/python-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 name: CI
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main, master ]
     tags:
       - 'v*.*.*'
   pull_request:
-    branches: [ master ]
+    branches: [ main, master ]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.9]
+        python-version: ["3.8", "3.12"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
-        python -m pip install --upgrade pip
+        python -m pip install --upgrade pip setuptools
         python -m pip install '.[dev]'
-    - name: Check code with isort
-      run: |
-        isort --check .
     - name: Check code with black
       run: |
         black --check .
     - name: Lint code with pylama
       run: |
         pylama
     - name: Test with pytest
@@ -53,15 +50,7 @@
       - name: Create PyPI release
         uses: casperdcl/deploy-pypi@v2
         with:
           password: ${{ secrets.PYPI_TOKEN }}
           build: true
           # only upload if a tag is pushed (otherwise just build & check)
           upload: ${{ github.event_name == 'push' && steps.check-tag.outputs.match == 'true' }}
-      - name: Create GitHub release
-        if: ${{ github.event_name == 'push' && steps.check-tag.outputs.match == 'true' }}
-        uses: Roang-zero1/github-create-release-action@master
-        with:
-          version_regex: ^v[[:digit:]]+\.[[:digit:]]+\.[[:digit:]]+
-          changelog_file: "CHANGELOG.md"
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `deltachat_cursed-0.8.0/LICENSE` & `deltachat-cursed-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_cursed-0.8.0/PKG-INFO` & `deltachat-cursed-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,75 @@
 Metadata-Version: 2.1
-Name: deltachat_cursed
-Version: 0.8.0
+Name: deltachat-cursed
+Version: 0.9.0
 Summary: Delta Chat client for the command line
-Home-page: https://github.com/adbenitez/deltachat-cursed
-Author: The Cursed Delta Contributors
-Author-email: adbenitez@nauta.cu
-Keywords: deltachat tui client ncurses
+Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/adbenitez/deltachat-cursed
+Project-URL: Issues, https://github.com/adbenitez/deltachat-cursed/issues
+Keywords: deltachat,ncurses,tui
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: deltachat2>=0.2.0
+Requires-Dist: urwid>=2.6.10
+Requires-Dist: urwid-readline>=0.14
+Requires-Dist: appdirs>=1.4.4
+Provides-Extra: full
+Requires-Dist: deltachat-rpc-server>=1.136.6; extra == "full"
+Provides-Extra: dev
+Requires-Dist: deltachat-rpc-server; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pylama; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Cursed Delta
 
 ncurses Delta Chat client developed in Python with the urwid library.
 
 <p align="center">
   <img src="https://github.com/adbenitez/deltachat-cursed/blob/master/screenshots/e1.png" alt="screenshot of Cursed Delta"/>
 </p>
 
 [![Latest Release](https://img.shields.io/pypi/v/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
-[![Supported Versions](https://img.shields.io/pypi/pyversions/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
 [![Downloads](https://pepy.tech/badge/deltachat-cursed)](https://pepy.tech/project/deltachat-cursed)
 [![License](https://img.shields.io/pypi/l/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
 [![CI](https://github.com/adbenitez/deltachat-cursed/actions/workflows/python-ci.yml/badge.svg)](https://github.com/adbenitez/deltachat-cursed/actions/workflows/python-ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 #### Features
 
+- [X] Create accounts
+- [X] Tweak account configuration (ex. set display name and status)
 - [X] Ability to send text messages :)
-- [X] Ability to send files
-- [X] Notifications
 - [X] Read receipts ✓✓
-- [X] Create and open encrypted accounts
-- [X] Import/export keys and backups (including password-protected backups)
-- [X] Emoji support and auto-completion
-- [X] @Mentions support and auto-completion
-- [X] Display message replies
-- [X] themes/skins and keyboard shortcuts customization
-- [X] Chat operations: delete, pin/unpin, mute/unmute, add/remove members, change chat name, clear chat messages
-- [ ] Proxy support
+- [X] Display quoted messages
+- [ ] Account switcher
+- [ ] Chat operations: delete, pin/unpin, mute/unmute, archive/unarchive, add/remove members, etc.
+- [ ] Message operations: reply, delete, open attachment/links, see info, jump to quote
+- [ ] Import/export keys and backups
+- [ ] Ability to send files
+- [ ] Notifications
 - [ ] Support for contact verification and group invitations links
 - [ ] Block/unblock contacts and see the list of blocked contacts
-- [ ] Ability to send stickers
-- [ ] Jump to quoted messages
-- [ ] Record and send voice messages
-- [ ] Message operations: reply, delete, open attachment/links, see info
-- [ ] List contacts
-- [ ] Search
-- [ ] Set disappearing messages timer
+- [ ] See contact list
+- [ ] Search messages and chats
 - [ ] Open HTML messages
-- [ ] Open webxdc documents
-- [ ] View archived chats and allow to archive/Unarchive
-- [ ] Multi-language support
+- [ ] View archived chats
 
 ## Installation
 
 Install Cursed Delta with pip:
 
 ```
 $ pip install -U deltachat-cursed
 ```
 
 After installation the command `delta` should be available.
-For more tips and info check [the user guide](https://github.com/adbenitez/deltachat-cursed/blob/master/docs/user-guide.md)
-
-
-## Credits
-
-The user interface was initially based on [ncTelegram](https://github.com/Nanoseb/ncTelegram)
-
-Some code and ideas were taken from [scli](https://github.com/isamert/scli/)
-
-## License
-
-Licensed GPLv3+, see the LICENSE file for details.
-
-Copyright © 2020-2022 Cursed Delta contributors.
+For more tips and info check [the user guide](./docs/user-guide.md)
```

### Comparing `deltachat_cursed-0.8.0/src/deltachat_cursed/widgets/chatlist.py` & `deltachat-cursed-0.9.0/deltachat_cursed/chatlist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,104 @@
-from logging import Logger
-from typing import Callable, List, Optional
+"""Chat list widget"""
+
+from typing import Any, Callable, Optional, Tuple
 
 import urwid
-from deltachat import Chat, const
-from emoji import demojize
+from deltachat2 import ChatlistFlag, Client
+
+from .lazylistwaker import LazyListWalker
+from .util import shorten_text
 
-from ..scli import LazyEvalListWalker, ListBoxPlus
-from ..util import is_pinned, shorten_text
+CHAT_SELECTED = "chat_selected"
 
 
 class ChatListItem(urwid.Button):
-    def __init__(self, caption: list, callback: Callable, chat: Chat) -> None:
-        super().__init__("")
-        urwid.connect_signal(self, "click", callback, chat)
-        self._w = urwid.AttrMap(
-            urwid.SelectableIcon(caption, 3), None, focus_map="focused_item"
-        )
-
-
-class ChatListWidget(ListBoxPlus):
-    signals = ["chat_selected"]
-
-    def __init__(self, keymap: dict, display_emoji: bool, logger: Logger) -> None:
-        self.keymap = keymap
-        self.display_emoji = display_emoji
-        self.selected_chat: Optional[Chat] = None
-        self.logger = logger
-        super().__init__(
-            LazyEvalListWalker(urwid.MonitoredList(), self._get_chat_widget, 0)
-        )
-
-    def _item_clicked(self, _button, chat: Chat) -> None:
-        self.select_chat(chat)
-
-    def _get_chat(self, position) -> Optional[Chat]:
-        if 0 <= position < len(self.contents):
-            return self.contents[position]
-        return None
-
-    def set_chats(self, chats: List[Chat]) -> None:
-        prev_position = self.get_focus()[1]
-        self.contents = chats
-        if prev_position is not None:
-            self.try_set_focus(prev_position)
-        if self.selected_chat and self.selected_chat not in self.contents:
-            self.select_chat(None)
+    """A single chatlist item"""
 
-    def select_chat(self, chat: Chat) -> None:
-        self.logger.debug("Chat selected: %s", chat)
-        self.selected_chat = chat
-        urwid.emit_signal(self, "chat_selected", chat)
+    def __init__(
+        self,
+        accid: int,
+        item: Any,
+        selected: bool,
+        callback: Callable[["ChatListItem"], None],
+    ) -> None:
+        super().__init__("", callback)
+        self.accid = accid
+        self.id = item.id
+        elements: list = []
 
-    def select_next_chat(self) -> None:
-        if self.selected_chat:
-            i = self.contents.index(self.selected_chat)
-            if i < 0:  # no chat selected, skip
-                return
-            i -= 1
-            if i < 0:
-                i = len(self.contents) - 1
-            self.try_set_focus(i)
-            self.select_chat(self.contents[i])
-
-    def select_previous_chat(self) -> None:
-        if self.selected_chat:
-            i = self.contents.index(self.selected_chat)
-            if i < 0:  # no chat selected, skip
-                return
-            i += 1
-            if i >= len(self.contents):
-                i = 0
-            self.try_set_focus(i)
-            self.select_chat(self.contents[i])
-
-    def keypress(self, size: list, key: str) -> Optional[str]:
-        key = super().keypress(size, key)
-        if key == self.keymap["down"]:
-            self.keypress(size, "down")
-        elif key == self.keymap["up"]:
-            self.keypress(size, "up")
+        if item.is_self_talk:
+            color = "#0af"
+            icon = "*"
+        elif item.is_device_talk:
+            color = "#888"
+            icon = "i"
         else:
-            return key
-        return None
+            color = item.color
+            icon = "@" if item.dm_chat_contact else "#"
+        elements.append((urwid.AttrSpec("#fff", color), f" {icon} "))
 
-    def _get_chat_widget(self, chat: Chat, position: int) -> urwid.Widget:
-        elements: list = []
+        if item.is_pinned:
+            elements.append("*")
+        else:
+            elements.append(" ")
 
-        chat_color = urwid.AttrSpec(
-            "#fff",
-            f"#{chat.get_color():06X}",
-        )
-        elements.append(
-            (
-                chat_color,
-                " @ " if chat.get_type() == const.DC_CHAT_TYPE_SINGLE else " # ",
-            )
-        )
-
-        elements.append(" ")
-
-        name = shorten_text(chat.get_name(), 40)
-        label = f"{name if self.display_emoji else demojize(name)}"
-        if self.selected_chat and chat == self.selected_chat:
-            label = ("cur_chat", label)  # type: ignore
-        elements.append(label)
+        name = shorten_text(item.name, 40)
+        elements.append(("selected_chat", name) if selected else name)
 
-        new_messages = chat.count_fresh_messages()
-        if new_messages > 0:
+        if item.fresh_message_counter > 0:
             elements.append(" ")
-            if chat.is_muted():
-                elements.append(f"({new_messages})")
-            else:
-                elements.append(("unread_chat", f"({new_messages})"))
+            style = "unread_badge_muted" if item.is_muted else "unread_badge"
+            elements.append((style, f"({item.fresh_message_counter})"))
+
+        self._w = urwid.AttrMap(urwid.SelectableIcon(elements, 3), None, focus_map="focused_item")
+
 
-        widget = ChatListItem(elements, self._item_clicked, chat)
+class ChatListWidget(urwid.ListBox):
+    """Display a list of chats"""
 
-        if is_pinned(chat):
-            next_chat = self._get_chat(position + 1)
-            if next_chat and not is_pinned(next_chat):
-                divider = urwid.AttrMap(urwid.Divider("─"), "pinned_marker")
-                widget = urwid.Pile([widget, divider])
+    signals = [CHAT_SELECTED]
+
+    def __init__(self, client: Client) -> None:
+        self.client = client
+        self.accid: Optional[int] = None
+        self.selected_chat: Optional[Tuple[int, int]] = None
+        super().__init__(LazyListWalker([], self._create_chatlist_item))
+
+    def set_account(self, accid: Optional[int]) -> None:
+        self.accid = accid
+        if self.selected_chat and accid != self.selected_chat[0]:
+            self._select_chat(None)
+        self.chatlist_changed(self.client, accid)
+
+    def select_chat(self, chat: Optional[Tuple[int, int]]) -> None:
+        self._select_chat(chat)
+        self.chatlist_changed(self.client, self.accid)
+
+    def chatlist_changed(self, client: Client, accid: Optional[int]) -> None:
+        if not self.accid:
+            self.body.clear_cache()
+            self.body.clear()
+        elif accid == self.accid:
+            entries = client.rpc.get_chatlist_entries(accid, ChatlistFlag.NO_SPECIALS, None, None)
+            item = self.focus
+            self.body.clear_cache()
+            self.body[:] = [(accid, chatid) for chatid in entries]
+            try:
+                index = max(entries.index(item.id), 0) if item else 0
+            except ValueError:
+                pass
+            else:
+                if entries:
+                    self.set_focus(index)
+
+    def _create_chatlist_item(self, chat: Tuple[int, int]) -> urwid.Widget:
+        item = self.client.rpc.get_chatlist_items_by_entries(chat[0], [chat[1]])[str(chat[1])]
+        return ChatListItem(chat[0], item, self.selected_chat == chat, self._on_item_clicked)
+
+    def _on_item_clicked(self, item: ChatListItem) -> None:
+        self._select_chat((item.accid, item.id))
+        self.chatlist_changed(self.client, self.accid)  # so the selected chat widget is updated
 
-        return widget
+    def _select_chat(self, chat: Optional[Tuple[int, int]]) -> None:
+        self.selected_chat = chat
+        urwid.emit_signal(self, CHAT_SELECTED, self.selected_chat)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deltachat_cursed-0.8.0/src/deltachat_cursed.egg-info/PKG-INFO` & `deltachat-cursed-0.9.0/deltachat_cursed.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,75 @@
 Metadata-Version: 2.1
 Name: deltachat-cursed
-Version: 0.8.0
+Version: 0.9.0
 Summary: Delta Chat client for the command line
-Home-page: https://github.com/adbenitez/deltachat-cursed
-Author: The Cursed Delta Contributors
-Author-email: adbenitez@nauta.cu
-Keywords: deltachat tui client ncurses
+Author-email: adbenitez <adb@merlinux.eu>
+Project-URL: Homepage, https://github.com/adbenitez/deltachat-cursed
+Project-URL: Issues, https://github.com/adbenitez/deltachat-cursed/issues
+Keywords: deltachat,ncurses,tui
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: deltachat2>=0.2.0
+Requires-Dist: urwid>=2.6.10
+Requires-Dist: urwid-readline>=0.14
+Requires-Dist: appdirs>=1.4.4
+Provides-Extra: full
+Requires-Dist: deltachat-rpc-server>=1.136.6; extra == "full"
+Provides-Extra: dev
+Requires-Dist: deltachat-rpc-server; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pylama; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Cursed Delta
 
 ncurses Delta Chat client developed in Python with the urwid library.
 
 <p align="center">
   <img src="https://github.com/adbenitez/deltachat-cursed/blob/master/screenshots/e1.png" alt="screenshot of Cursed Delta"/>
 </p>
 
 [![Latest Release](https://img.shields.io/pypi/v/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
-[![Supported Versions](https://img.shields.io/pypi/pyversions/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
 [![Downloads](https://pepy.tech/badge/deltachat-cursed)](https://pepy.tech/project/deltachat-cursed)
 [![License](https://img.shields.io/pypi/l/deltachat-cursed.svg)](https://pypi.org/project/deltachat-cursed)
 [![CI](https://github.com/adbenitez/deltachat-cursed/actions/workflows/python-ci.yml/badge.svg)](https://github.com/adbenitez/deltachat-cursed/actions/workflows/python-ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 #### Features
 
+- [X] Create accounts
+- [X] Tweak account configuration (ex. set display name and status)
 - [X] Ability to send text messages :)
-- [X] Ability to send files
-- [X] Notifications
 - [X] Read receipts ✓✓
-- [X] Create and open encrypted accounts
-- [X] Import/export keys and backups (including password-protected backups)
-- [X] Emoji support and auto-completion
-- [X] @Mentions support and auto-completion
-- [X] Display message replies
-- [X] themes/skins and keyboard shortcuts customization
-- [X] Chat operations: delete, pin/unpin, mute/unmute, add/remove members, change chat name, clear chat messages
-- [ ] Proxy support
+- [X] Display quoted messages
+- [ ] Account switcher
+- [ ] Chat operations: delete, pin/unpin, mute/unmute, archive/unarchive, add/remove members, etc.
+- [ ] Message operations: reply, delete, open attachment/links, see info, jump to quote
+- [ ] Import/export keys and backups
+- [ ] Ability to send files
+- [ ] Notifications
 - [ ] Support for contact verification and group invitations links
 - [ ] Block/unblock contacts and see the list of blocked contacts
-- [ ] Ability to send stickers
-- [ ] Jump to quoted messages
-- [ ] Record and send voice messages
-- [ ] Message operations: reply, delete, open attachment/links, see info
-- [ ] List contacts
-- [ ] Search
-- [ ] Set disappearing messages timer
+- [ ] See contact list
+- [ ] Search messages and chats
 - [ ] Open HTML messages
-- [ ] Open webxdc documents
-- [ ] View archived chats and allow to archive/Unarchive
-- [ ] Multi-language support
+- [ ] View archived chats
 
 ## Installation
 
 Install Cursed Delta with pip:
 
 ```
 $ pip install -U deltachat-cursed
 ```
 
 After installation the command `delta` should be available.
-For more tips and info check [the user guide](https://github.com/adbenitez/deltachat-cursed/blob/master/docs/user-guide.md)
-
-
-## Credits
-
-The user interface was initially based on [ncTelegram](https://github.com/Nanoseb/ncTelegram)
-
-Some code and ideas were taken from [scli](https://github.com/isamert/scli/)
-
-## License
-
-Licensed GPLv3+, see the LICENSE file for details.
-
-Copyright © 2020-2022 Cursed Delta contributors.
+For more tips and info check [the user guide](./docs/user-guide.md)
```


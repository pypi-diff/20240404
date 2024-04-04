# Comparing `tmp/pipxu-1.6.tar.gz` & `tmp/pipxu-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipxu-1.6.tar", last modified: Tue Apr  2 23:42:46 2024, max compression
+gzip compressed data, was "pipxu-1.7.tar", last modified: Thu Apr  4 00:18:34 2024, max compression
```

## Comparing `pipxu-1.6.tar` & `pipxu-1.7.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 23:42:46.517512 pipxu-1.6/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pipxu-1.6/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-02-24 11:57:27.000000 pipxu-1.6/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      471 2024-04-02 22:48:31.000000 pipxu-1.6/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    15658 2024-04-02 23:42:46.517512 pipxu-1.6/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    15135 2024-04-02 23:34:26.000000 pipxu-1.6/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 23:42:46.517512 pipxu-1.6/pipxu/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-03-29 00:15:14.000000 pipxu-1.6/pipxu/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-03-29 00:15:14.000000 pipxu-1.6/pipxu/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 23:42:46.517512 pipxu-1.6/pipxu/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     1718 2024-04-02 23:31:10.000000 pipxu-1.6/pipxu/commands/debug.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1176 2024-04-02 23:29:01.000000 pipxu-1.6/pipxu/commands/inject.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4314 2024-04-02 23:28:43.000000 pipxu-1.6/pipxu/commands/install.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1369 2024-04-02 01:11:56.000000 pipxu-1.6/pipxu/commands/list.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1097 2024-04-02 01:12:02.000000 pipxu-1.6/pipxu/commands/reinstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2178 2024-04-02 03:40:36.000000 pipxu-1.6/pipxu/commands/reinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      958 2024-04-02 23:29:13.000000 pipxu-1.6/pipxu/commands/runpip.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1176 2024-04-02 23:28:17.000000 pipxu-1.6/pipxu/commands/uninject.py
--rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-02 01:12:29.000000 pipxu-1.6/pipxu/commands/uninstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)      875 2024-04-02 01:12:35.000000 pipxu-1.6/pipxu/commands/uninstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-02 01:12:41.000000 pipxu-1.6/pipxu/commands/upgrade-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1357 2024-04-02 03:44:39.000000 pipxu-1.6/pipxu/commands/upgrade.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-02 01:12:52.000000 pipxu-1.6/pipxu/commands/version.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5786 2024-04-02 04:45:36.000000 pipxu-1.6/pipxu/pipxu.py
--rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-02 01:13:16.000000 pipxu-1.6/pipxu/run.py
--rw-r--r--   0 mark      (1000) mark      (1000)    10004 2024-04-02 12:23:49.000000 pipxu-1.6/pipxu/utils.py
--rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-02 11:28:31.000000 pipxu-1.6/pipxu-bootstrap
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 23:42:46.517512 pipxu-1.6/pipxu.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    15658 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      675 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-02 23:42:46.000000 pipxu-1.6/pipxu.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-02 22:45:17.000000 pipxu-1.6/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-02 23:42:46.517512 pipxu-1.6/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2024-04-04 00:13:06.000000 pipxu-1.7/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-04-04 00:13:06.000000 pipxu-1.7/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      472 2024-04-04 00:13:57.000000 pipxu-1.7/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    16994 2024-04-04 00:18:34.375951 pipxu-1.7/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    16471 2024-04-04 00:14:10.000000 pipxu-1.7/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/doc/
+-rw-r--r--   0 mark      (1000) mark      (1000)     2539 2024-04-04 00:13:06.000000 pipxu-1.7/doc/debug.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1729 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/debug.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1186 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/inject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4696 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/install.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1442 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/list.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1515 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/reinstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2953 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/reinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      958 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/runpip.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1176 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      938 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/upgrade-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1407 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/upgrade.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/version.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5786 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/pipxu.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/run.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    10070 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/utils.py
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu-bootstrap
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    16994 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      688 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-04 00:13:06.000000 pipxu-1.7/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-04 00:18:34.375951 pipxu-1.7/setup.cfg
```

### Comparing `pipxu-1.6/PKG-INFO` & `pipxu-1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pipxu
-Version: 1.6
-Summary: Install and Run Python Applications in Isolated Environments using UV
-Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
-License: GPLv3
-Project-URL: Homepage, https://github.com/bulletmark/pipxu
-Keywords: pipx,pip,uv,venv,virtualenv
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: filelock
-Requires-Dist: platformdirs
-Requires-Dist: importlib-metadata; python_version < "3.8"
-
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
 [`pipxu`][pipxu] installs Python applications, i.e. a Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
@@ -93,17 +78,17 @@
 ### Command `debug`
 
 ```
 usage: pipxu debug [-h] [-e EXECUTABLE] [-d DEBUGGER] package [args ...]
 
 Run an installed application using a debugger.
 
-Tries to work out your preferred debugger from the PYTHONBREAKPOINT
-environment variable. If not set, defaults to pdb. Or you can set it
-explicitly with the -d/--debugger option.
+Tries to work out your preferred debugger from the standard
+PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
+you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
   args                  options and arguments to pass to application. should
                         start with "--".
 
 options:
@@ -129,15 +114,16 @@
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
-usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
+usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
+                           [--system-site-packages] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
@@ -147,14 +133,16 @@
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
+  --system-site-packages
+                        allow venv access to system packages
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -168,49 +156,65 @@
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
-usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV]
+                                 [--system-site-packages]
+                                 [--no-system-site-packages] [-v]
                                  [-s [SKIP ...]]
 
 Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
-usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV]
+                             [--system-site-packages]
+                             [--no-system-site-packages] [-v]
                              package [package ...]
 
 Reinstall an application.
 
 positional arguments:
   package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
@@ -329,36 +333,45 @@
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
 script](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
-```
+```sh
 $ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/pipxu-bootstrap | sh
 ```
 
-:warning: Note that the `pipxu` package also installs the
-`pipxu-bootstrap` script on your system so you can always recover easily
-from a broken `pipxu` installation by running that script.
-
 To upgrade:
 
-```
+```sh
 $ pipxu upgrade pipxu
 ```
 
 To uninstall all `pipxu` installed applications, and then uninstall
 `pipxu` itself:
 
-```
+```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
+## Recovery
+
+The `pipxu` package also installs the `pipxu-bootstrap` shell script on
+your system so you can always recover easily from a broken `pipxu`
+installation by manually running that script. E.g. The following may be
+needed after a major or incompatible Python version upgrade where
+`pipxu` may have stopped working:
+
+```sh
+$ pipxu-bootstrap
+$ pipxu reinstall-all --skip pipxu
+```
+
 ## Comparison to pipx
 
 Why would you use [`pipxu`][pipxu] instead of [`pipx`][pipx]? The main
 reason is to gain a massive speed improvement. `pipx` uses [`python -m
 venv`][venv] to create and install virtual environments and `pip` to
 install packages whereas `pipxu` uses `uv` for these operations.
 [`uv`][uv] is [a new project](https://astral.sh/blog/uv) written in
@@ -384,16 +397,18 @@
 2. You can do `pipxu` commands on an editable projects (as often used by
    developers) in the current directory by simply typing "`.`" as the
    package name and this works for all commands. E.g. `pipxu uninstall
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
-3. `pipxu` adds a `debug` command to run an installed application using a
-   Python debugger.
+3. For Python developers,`pipxu` adds a [`debug`](#command-debug)
+   command to conveniently run an installed application using a
+   debugger. `pipx` does not have this command. Read more about the
+   `debug` command [here](doc/debug.md).
 
 4. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
@@ -452,16 +467,16 @@
 General Public License as published by the Free Software Foundation,
 either version 3 of the License, or any later version. This program is
 distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or
 FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at
 <http://www.gnu.org/licenses/> for more details.
 
-[pip]: https://pip.pypa.io/en/stable/
-[pipx]: https://github.com/pypa/pipx
 [pipxu]: https://github.com/bulletmark/pipxu
+[pipx]: https://github.com/pypa/pipx
 [uv]: https://github.com/astral-sh/uv
 [venv]: https://docs.python.org/3/library/venv.html
+[pip]: https://pip.pypa.io/en/stable/
 [pypi]: https://pypi.org/
 [path]: https://www.baeldung.com/linux/path-variable
 
 <!-- vim: se ai syn=markdown: -->
```

### Comparing `pipxu-1.6/README.md` & `pipxu-1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pipxu
+Version: 1.7
+Summary: Install and Run Python Applications in Isolated Environments using UV
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
+License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/pipxu
+Keywords: pipx,pip,uv,venv,virtualenv
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: filelock
+Requires-Dist: platformdirs
+Requires-Dist: importlib-metadata; python_version < "3.8"
+
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
 [`pipxu`][pipxu] installs Python applications, i.e. a Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
@@ -78,17 +93,17 @@
 ### Command `debug`
 
 ```
 usage: pipxu debug [-h] [-e EXECUTABLE] [-d DEBUGGER] package [args ...]
 
 Run an installed application using a debugger.
 
-Tries to work out your preferred debugger from the PYTHONBREAKPOINT
-environment variable. If not set, defaults to pdb. Or you can set it
-explicitly with the -d/--debugger option.
+Tries to work out your preferred debugger from the standard
+PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
+you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
   args                  options and arguments to pass to application. should
                         start with "--".
 
 options:
@@ -114,15 +129,16 @@
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
-usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
+usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
+                           [--system-site-packages] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
@@ -132,14 +148,16 @@
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
+  --system-site-packages
+                        allow venv access to system packages
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -153,49 +171,65 @@
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
-usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV]
+                                 [--system-site-packages]
+                                 [--no-system-site-packages] [-v]
                                  [-s [SKIP ...]]
 
 Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
-usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV]
+                             [--system-site-packages]
+                             [--no-system-site-packages] [-v]
                              package [package ...]
 
 Reinstall an application.
 
 positional arguments:
   package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
@@ -314,36 +348,45 @@
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
 script](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
-```
+```sh
 $ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/pipxu-bootstrap | sh
 ```
 
-:warning: Note that the `pipxu` package also installs the
-`pipxu-bootstrap` script on your system so you can always recover easily
-from a broken `pipxu` installation by running that script.
-
 To upgrade:
 
-```
+```sh
 $ pipxu upgrade pipxu
 ```
 
 To uninstall all `pipxu` installed applications, and then uninstall
 `pipxu` itself:
 
-```
+```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
+## Recovery
+
+The `pipxu` package also installs the `pipxu-bootstrap` shell script on
+your system so you can always recover easily from a broken `pipxu`
+installation by manually running that script. E.g. The following may be
+needed after a major or incompatible Python version upgrade where
+`pipxu` may have stopped working:
+
+```sh
+$ pipxu-bootstrap
+$ pipxu reinstall-all --skip pipxu
+```
+
 ## Comparison to pipx
 
 Why would you use [`pipxu`][pipxu] instead of [`pipx`][pipx]? The main
 reason is to gain a massive speed improvement. `pipx` uses [`python -m
 venv`][venv] to create and install virtual environments and `pip` to
 install packages whereas `pipxu` uses `uv` for these operations.
 [`uv`][uv] is [a new project](https://astral.sh/blog/uv) written in
@@ -369,16 +412,18 @@
 2. You can do `pipxu` commands on an editable projects (as often used by
    developers) in the current directory by simply typing "`.`" as the
    package name and this works for all commands. E.g. `pipxu uninstall
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
-3. `pipxu` adds a `debug` command to run an installed application using a
-   Python debugger.
+3. For Python developers,`pipxu` adds a [`debug`](#command-debug)
+   command to conveniently run an installed application using a
+   debugger. `pipx` does not have this command. Read more about the
+   `debug` command [here](doc/debug.md).
 
 4. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
@@ -437,16 +482,16 @@
 General Public License as published by the Free Software Foundation,
 either version 3 of the License, or any later version. This program is
 distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or
 FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at
 <http://www.gnu.org/licenses/> for more details.
 
-[pip]: https://pip.pypa.io/en/stable/
-[pipx]: https://github.com/pypa/pipx
 [pipxu]: https://github.com/bulletmark/pipxu
+[pipx]: https://github.com/pypa/pipx
 [uv]: https://github.com/astral-sh/uv
 [venv]: https://docs.python.org/3/library/venv.html
+[pip]: https://pip.pypa.io/en/stable/
 [pypi]: https://pypi.org/
 [path]: https://www.baeldung.com/linux/path-variable
 
 <!-- vim: se ai syn=markdown: -->
```

### Comparing `pipxu-1.6/pipxu/commands/debug.py` & `pipxu-1.7/pipxu/commands/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Author: Mark Blakeney, Feb 2024.
 '''
 Run an installed application using a debugger.
 
-Tries to work out your preferred debugger from the PYTHONBREAKPOINT
-environment variable. If not set, defaults to pdb. Or you can set it
-explicitly with the -d/--debugger option.
+Tries to work out your preferred debugger from the standard
+PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
+you can set it explicitly with the -d/--debugger option.
 '''
 
 from __future__ import annotations
 
 import os
 import re
 from argparse import ArgumentParser, Namespace
```

### Comparing `pipxu-1.6/pipxu/commands/inject.py` & `pipxu-1.7/pipxu/commands/inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
 
     pip_args = utils.make_args((args.verbose, '-v'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
-    if not utils.piprun(vdir, f'install{pip_args} {extras}'):
+    if not utils.piprun(vdir, f'install{pip_args} --compile {extras}'):
         return f'Error: failed to install "{extras}" to {pkgname}'
 
     return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=True)
```

### Comparing `pipxu-1.6/pipxu/commands/install.py` & `pipxu-1.7/pipxu/commands/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,27 @@
                         'i.e. from `pyenv versions`, e.g. "3.9".')
     parser.add_argument('-f', '--force', action='store_true',
                         help='recreate any already installed venv')
     parser.add_argument('-e', '--editable', action='store_true',
                         help='install application[s] in editable mode')
     parser.add_argument('-d', '--include-deps', action='store_true',
                         help='include executables from dependencies')
+    parser.add_argument('--system-site-packages', action='store_true',
+                        help='allow venv access to system packages')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to install')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
+                                (args.system_site_packages,
+                                 '--system-site-packages'),
                                 (bool(pyexe), f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'), (args.editable, '-e'))
 
     lockfile = user_runtime_path() / f'{args._prog}.lock'
     vdirbase = args._venvs_dir
     for pkg in args.package:
         # Use a lock file in case we are running multiple installs in parallel
@@ -65,15 +69,16 @@
 
         python_exe = (vdir / 'bin' / 'python').resolve()
         python_ver = run(f'{python_exe} -V', capture=True)
         python_ver = python_ver.strip().split()[1] if python_ver else '?ver?'
         print(f'Created {vdir} using {python_exe} ({python_ver})')
 
         # Install the package
-        if not utils.piprun(vdir, f'install --no-deps{pip_args} "{pkg}"'):
+        if not utils.piprun(vdir, f'install --compile --no-deps{pip_args} '
+                            f'"{pkg}"'):
             utils.rm_vdir(vdir, args)
             return f'Error: failed to preinstall "{pkg}".'
 
         versions = utils.get_versions(vdir)
         if not versions:
             utils.rm_vdir(vdir, args)
             return f'Error: failed to get versions for {pkg}.'
@@ -88,27 +93,30 @@
             if not args.force:
                 utils.rm_vdir(vdir, args)
                 return f'Error: venv for {pkgname} exists. Use -f to force.'
             print(f'Removing pre-existing {pkgname} venv dir.')
             utils.rm_vdir(pdir, args)
             pdir.unlink()
 
-        if not utils.piprun(vdir, f'install{pip_args} "{pkg}"'):
+        if not utils.piprun(vdir, f'install --compile{pip_args} "{pkg}"'):
             utils.rm_vdir(vdir, args)
             return f'Error: failed to install "{pkg}".'
 
         pdir.symlink_to(vdir)
 
         data: dict = {'name': pkgname}
         if editpath:
             data['editpath'] = editpath
 
         if args.include_deps:
             data['deps'] = True
 
+        if args.system_site_packages:
+            data['sys'] = True
+
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             pdir.unlink()
             utils.rm_vdir(vdir, args)
             return err
 
     return None
```

### Comparing `pipxu-1.6/pipxu/commands/list.py` & `pipxu-1.7/pipxu/commands/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,25 @@
     parser.add_argument('--json', action='store_true',
                         help='output json instead')
     parser.add_argument('package', nargs='*',
                         help='list the given application[s] only')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
-    pkgs = set(utils.get_package_from_arg(p, args)[0] for p in args.package)
+    if args.package:
+        pkgs = [utils.get_package_from_arg(p, args) for p in args.package]
+    else:
+        pkgs = sorted((p.name, p) for p in args._packages_dir.iterdir())
+
     json_out = {}
-    for pdir in sorted(args._packages_dir.iterdir()):
-        pkgname = pdir.name
-        if pkgs and pkgname not in pkgs:
-            continue
+    for pkgname, vdir in pkgs:
+        if not vdir:
+            return f'Application {pkgname} is not installed.'
 
-        data = utils.get_json(pdir, args)
+        data = utils.get_json(vdir, args)
         if data:
             data.pop('name', None)
             if args.json:
                 json_out[pkgname] = data
             else:
                 d = ', '.join(f'{k}={show(data[k])}' for k in sorted(data))
                 print(f'{pkgname}: {d}')
```

### Comparing `pipxu-1.6/pipxu/commands/reinstall.py` & `pipxu-1.7/pipxu/commands/reinstall.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     'Called to add command arguments to parser at init'
     xgroup = parser.add_mutually_exclusive_group()
     xgroup.add_argument('-p', '--python',
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
                         'i.e. from `pyenv versions`, e.g. "3.9".')
+    parser.add_argument('--system-site-packages', action='store_true',
+                        help='allow venv access to system packages. '
+                        'Overrides the per-application setting.')
+    parser.add_argument('--no-system-site-packages', action='store_true',
+                        help='remove venv access to system packages. '
+                        'Overrides the per-application setting.')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to reinstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
@@ -31,26 +37,35 @@
                                 (bool(pyexe), f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
+        print(f'Reinstalling {pkgname} ..')
         data = utils.get_json(vdir, args) or {}
 
+        if args.system_site_packages or (
+                not args.no_system_site_packages and data.get('sys')):
+            data['sys'] = True
+        else:
+            data.pop('sys', None)
+
+        sysp = ' --system-site-packages' if data.get('sys') else ''
         with tempfile.TemporaryDirectory() as tdir:
             tfile = Path(tdir, args._freeze_file)
             shutil.copyfile(vdir / args._freeze_file, tfile)
 
             # Recreate the vdir
-            if not run(f'uv venv{venv_args} {vdir}'):
+            if not run(f'uv venv{venv_args}{sysp} {vdir}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to recreate {vdir} for {pkgname}.'
 
-            if not utils.piprun(vdir, f'sync{pip_args} --reinstall {tfile}'):
+            if not utils.piprun(vdir, f'sync{pip_args} --compile --reinstall '
+                                f'{tfile}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to resync {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
```

### Comparing `pipxu-1.6/pipxu/commands/runpip.py` & `pipxu-1.7/pipxu/commands/runpip.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/commands/uninject.py` & `pipxu-1.7/pipxu/commands/uninject.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/commands/uninstall-all.py` & `pipxu-1.7/pipxu/commands/uninstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/commands/uninstall.py` & `pipxu-1.7/pipxu/commands/uninstall.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,13 +14,16 @@
     parser.add_argument('package', nargs='+',
                         help='application[s] to uninstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
-        if not vdir or not utils.rm_package(pkgname, args):
+        if not vdir:
             return f'Application {pkgname} is not installed.'
 
+        if not utils.rm_package(pkgname, args):
+            return f'Failed to uninstall {pkgname}.'
+
         print(f'{pkgname} uninstalled.')
 
     return None
```

### Comparing `pipxu-1.6/pipxu/commands/upgrade-all.py` & `pipxu-1.7/pipxu/commands/upgrade-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/commands/upgrade.py` & `pipxu-1.7/pipxu/commands/upgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,19 +18,20 @@
     'Called to action this command'
     pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
+        print(f'Upgrading {pkgname} ..')
         data = utils.get_json(vdir, args) or {}
         editpath = data.get('editpath')
         pkg = f'-e {editpath}' if editpath else pkgname
         extras = ' '.join(data.get('injected', []))
-        if not utils.piprun(vdir, f'install --reinstall -U'
+        if not utils.piprun(vdir, 'install --compile --reinstall -U'
                             f'{pip_args} {pkg} {extras}'):
             return f'Error: failed to {args.name} {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
```

### Comparing `pipxu-1.6/pipxu/commands/version.py` & `pipxu-1.7/pipxu/commands/version.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/pipxu.py` & `pipxu-1.7/pipxu/pipxu.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/run.py` & `pipxu-1.7/pipxu/run.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.6/pipxu/utils.py` & `pipxu-1.7/pipxu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,19 @@
 def rm_package(pkgname: str, args: Namespace) -> bool:
     'Remove this package'
     pdir = args._packages_dir / pkgname
     if not pdir.exists():
         return False
 
     vdir = pdir.resolve()
+
+    if args.verbose:
+        print(f'Removing link {pdir}')
     pdir.unlink()
+
     rm_vdir(vdir, args)
     return True
 
 def get_all_pkg_venvs(args: Namespace) -> Iterable[tuple[Path, dict]]:
     'Return a list of all virtual environments and their JSON data'
     for pdir in sorted(args._packages_dir.iterdir()):
         data = get_json(pdir, args)
@@ -224,15 +228,15 @@
                 break
         else:
             return name, None
 
     path = (args._packages_dir / name).resolve()
     return name, (path if path.exists() else None)
 
-def rm_path(path: Path) -> None:
+def _rm_path(path: Path) -> None:
     'Remove the given path'
     print(f'Purging stray {path}', file=sys.stderr)
     if path.is_dir():
         shutil.rmtree(path)
     else:
         path.unlink()
 
@@ -240,28 +244,28 @@
     'Clean out any old virtual environments, packages, and executables'
     # Remove any packages that do not point to a dir in the venvs directory
     valids_venvs = set()
     for pkg in args._packages_dir.iterdir():
         vdir = pkg.resolve()
         if vdir.parent != args._venvs_dir or not vdir.is_dir() \
                 or not vdir.name.isdigit():
-            rm_path(pkg)
+            _rm_path(pkg)
         else:
             valids_venvs.add(vdir.name)
 
     # Remove any venvs that are not in the packages directory
     for vdir in args._venvs_dir.iterdir():
         if vdir.name not in valids_venvs:
-            rm_path(vdir)
+            _rm_path(vdir)
 
     # Remove any executables that point to a non-existent path
     for exe in args._bin_dir.iterdir():
         rexe = exe.resolve()
         if args._venvs_dir in rexe.parents and not rexe.exists():
-            rm_path(exe)
+            _rm_path(exe)
 
 def get_all_package_names(args: Namespace) -> list[str]:
     'Return a sorted list of all package names'
     return sorted(set(f.name for f in args._packages_dir.iterdir())
                   - set(args.skip or []))
 
 def get_python(args: Namespace) -> str:
```

### Comparing `pipxu-1.6/pipxu.egg-info/PKG-INFO` & `pipxu-1.7/pipxu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.6
+Version: 1.7
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -93,17 +93,17 @@
 ### Command `debug`
 
 ```
 usage: pipxu debug [-h] [-e EXECUTABLE] [-d DEBUGGER] package [args ...]
 
 Run an installed application using a debugger.
 
-Tries to work out your preferred debugger from the PYTHONBREAKPOINT
-environment variable. If not set, defaults to pdb. Or you can set it
-explicitly with the -d/--debugger option.
+Tries to work out your preferred debugger from the standard
+PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
+you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
   args                  options and arguments to pass to application. should
                         start with "--".
 
 options:
@@ -129,15 +129,16 @@
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
-usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
+usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
+                           [--system-site-packages] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
@@ -147,14 +148,16 @@
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
+  --system-site-packages
+                        allow venv access to system packages
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -168,49 +171,65 @@
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
-usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV]
+                                 [--system-site-packages]
+                                 [--no-system-site-packages] [-v]
                                  [-s [SKIP ...]]
 
 Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
-usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
+usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV]
+                             [--system-site-packages]
+                             [--no-system-site-packages] [-v]
                              package [package ...]
 
 Reinstall an application.
 
 positional arguments:
   package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
+  --system-site-packages
+                        allow venv access to system packages. Overrides the
+                        per-application setting.
+  --no-system-site-packages
+                        remove venv access to system packages. Overrides the
+                        per-application setting.
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
@@ -329,36 +348,45 @@
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
 script](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
-```
+```sh
 $ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/pipxu-bootstrap | sh
 ```
 
-:warning: Note that the `pipxu` package also installs the
-`pipxu-bootstrap` script on your system so you can always recover easily
-from a broken `pipxu` installation by running that script.
-
 To upgrade:
 
-```
+```sh
 $ pipxu upgrade pipxu
 ```
 
 To uninstall all `pipxu` installed applications, and then uninstall
 `pipxu` itself:
 
-```
+```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
+## Recovery
+
+The `pipxu` package also installs the `pipxu-bootstrap` shell script on
+your system so you can always recover easily from a broken `pipxu`
+installation by manually running that script. E.g. The following may be
+needed after a major or incompatible Python version upgrade where
+`pipxu` may have stopped working:
+
+```sh
+$ pipxu-bootstrap
+$ pipxu reinstall-all --skip pipxu
+```
+
 ## Comparison to pipx
 
 Why would you use [`pipxu`][pipxu] instead of [`pipx`][pipx]? The main
 reason is to gain a massive speed improvement. `pipx` uses [`python -m
 venv`][venv] to create and install virtual environments and `pip` to
 install packages whereas `pipxu` uses `uv` for these operations.
 [`uv`][uv] is [a new project](https://astral.sh/blog/uv) written in
@@ -384,16 +412,18 @@
 2. You can do `pipxu` commands on an editable projects (as often used by
    developers) in the current directory by simply typing "`.`" as the
    package name and this works for all commands. E.g. `pipxu uninstall
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
-3. `pipxu` adds a `debug` command to run an installed application using a
-   Python debugger.
+3. For Python developers,`pipxu` adds a [`debug`](#command-debug)
+   command to conveniently run an installed application using a
+   debugger. `pipx` does not have this command. Read more about the
+   `debug` command [here](doc/debug.md).
 
 4. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
@@ -452,16 +482,16 @@
 General Public License as published by the Free Software Foundation,
 either version 3 of the License, or any later version. This program is
 distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or
 FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at
 <http://www.gnu.org/licenses/> for more details.
 
-[pip]: https://pip.pypa.io/en/stable/
-[pipx]: https://github.com/pypa/pipx
 [pipxu]: https://github.com/bulletmark/pipxu
+[pipx]: https://github.com/pypa/pipx
 [uv]: https://github.com/astral-sh/uv
 [venv]: https://docs.python.org/3/library/venv.html
+[pip]: https://pip.pypa.io/en/stable/
 [pypi]: https://pypi.org/
 [path]: https://www.baeldung.com/linux/path-variable
 
 <!-- vim: se ai syn=markdown: -->
```

### Comparing `pipxu-1.6/pyproject.toml` & `pipxu-1.7/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/django_typer-1.0.9.tar.gz` & `tmp/django_typer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_typer-1.0.9.tar", max compression
+gzip compressed data, was "django_typer-1.1.0.tar", max compression
```

## Comparing `django_typer-1.0.9.tar` & `django_typer-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-10-24 04:20:22.142156 django_typer-1.0.9/LICENSE
--rw-r--r--   0        0        0     9070 2024-03-02 06:59:26.726709 django_typer-1.0.9/README.rst
--rw-r--r--   0        0        0    81834 2024-03-31 05:13:34.030192 django_typer-1.0.9/django_typer/__init__.py
--rw-r--r--   0        0        0     3268 2024-03-08 09:32:29.828059 django_typer-1.0.9/django_typer/apps.py
--rw-r--r--   0        0        0    16547 2024-03-04 21:09:02.016028 django_typer-1.0.9/django_typer/completers.py
--rw-r--r--   0        0        0        0 2024-01-14 22:24:15.916200 django_typer-1.0.9/django_typer/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-14 22:25:15.612846 django_typer-1.0.9/django_typer/management/commands/__init__.py
--rw-r--r--   0        0        0    26891 2024-03-27 02:22:06.591732 django_typer-1.0.9/django_typer/management/commands/shellcompletion.py
--rw-r--r--   0        0        0     7195 2024-03-13 20:15:02.250115 django_typer-1.0.9/django_typer/parsers.py
--rw-r--r--   0        0        0     5659 2024-03-31 05:12:13.792951 django_typer-1.0.9/django_typer/patch.py
--rw-r--r--   0        0        0        0 2024-03-04 21:09:02.017478 django_typer-1.0.9/django_typer/py.typed
--rw-r--r--   0        0        0     6055 2024-03-04 21:09:02.017884 django_typer-1.0.9/django_typer/types.py
--rw-r--r--   0        0        0     2828 2024-03-18 05:32:54.389828 django_typer-1.0.9/django_typer/utils.py
--rw-r--r--   0        0        0     5601 2024-03-31 05:13:49.659384 django_typer-1.0.9/pyproject.toml
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 django_typer-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-14 23:09:15.471852 django_typer-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8172 2024-04-03 22:32:47.609362 django_typer-1.1.0/README.md
+-rw-r--r--   0        0        0    81834 2024-04-03 22:32:47.610140 django_typer-1.1.0/django_typer/__init__.py
+-rw-r--r--   0        0        0     3268 2024-03-14 23:09:15.472335 django_typer-1.1.0/django_typer/apps.py
+-rw-r--r--   0        0        0    16547 2024-03-14 23:09:15.472439 django_typer-1.1.0/django_typer/completers.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474628 django_typer-1.1.0/django_typer/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474707 django_typer-1.1.0/django_typer/management/commands/__init__.py
+-rw-r--r--   0        0        0    26891 2024-04-03 18:21:16.067895 django_typer-1.1.0/django_typer/management/commands/shellcompletion.py
+-rw-r--r--   0        0        0     7195 2024-03-14 23:09:15.474929 django_typer-1.1.0/django_typer/parsers.py
+-rw-r--r--   0        0        0     5659 2024-04-03 18:21:16.068517 django_typer-1.1.0/django_typer/patch.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.475040 django_typer-1.1.0/django_typer/py.typed
+-rw-r--r--   0        0        0     6055 2024-03-14 23:09:15.487659 django_typer-1.1.0/django_typer/types.py
+-rw-r--r--   0        0        0     2828 2024-03-18 04:57:08.074572 django_typer-1.1.0/django_typer/utils.py
+-rw-r--r--   0        0        0     5605 2024-04-03 22:32:47.614956 django_typer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9976 1970-01-01 00:00:00.000000 django_typer-1.1.0/PKG-INFO
```

### Comparing `django_typer-1.0.9/LICENSE` & `django_typer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/README.rst` & `django_typer-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,86 @@
-|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPi djversions| |PyPI status| |Documentation Status|
-|Code Cov| |Test Status| |Lint Status| |Code Style|
+# django-typer
 
-.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-   :target: https://lbesson.mit-license.org/
 
-.. |PyPI version fury.io| image:: https://badge.fury.io/py/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer/
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
+[![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
+[![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
+[![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
+[![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
+[![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
+[![Lint Status](https://github.com/bckohan/django-typer/workflows/lint/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/lint.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer/
-
-.. |PyPI djversions| image:: https://img.shields.io/pypi/djversions/django-typer.svg
-   :target: https://pypi.org/project/django-typer/
-
-.. |PyPI status| image:: https://img.shields.io/pypi/status/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer
-
-.. |Documentation Status| image:: https://readthedocs.org/projects/django-typer/badge/?version=latest
-   :target: http://django-typer.readthedocs.io/?badge=latest/
-
-.. |Code Cov| image:: https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL
-   :target: https://codecov.io/gh/bckohan/django-typer
-
-.. |Test Status| image:: https://github.com/bckohan/django-typer/workflows/test/badge.svg
-   :target: https://github.com/bckohan/django-typer/actions/workflows/test.yml
-
-.. |Lint Status| image:: https://github.com/bckohan/django-typer/workflows/lint/badge.svg
-   :target: https://github.com/bckohan/django-typer/actions/workflows/lint.yml
-
-.. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-.. _powershell: https://learn.microsoft.com/en-us/powershell/scripting/overview
-.. _fish: https://fishshell.com/
-.. _zsh: https://www.zsh.org/
-.. _bash: https://www.gnu.org/software/bash/
-.. _Django: https://www.djangoproject.com/
-
-django-typer
-############
-
-Use `Typer <https://typer.tiangolo.com/>`_ to define the CLI for your Django_ management commands. 
-Provides a TyperCommand class that inherits from `BaseCommand <https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand>`_
-and allows typer-style annotated parameter types. All of the BaseCommand functionality is
-preserved, so that TyperCommand can be a drop in replacement.
+Use [Typer](https://typer.tiangolo.com/) to define the CLI for your [Django](https://www.djangoproject.com/) management commands. Provides a TyperCommand class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) and allows typer-style annotated parameter types. All of the BaseCommand functionality is preserved, so that TyperCommand can be a drop-in replacement.
 
 **django-typer makes it easy to:**
 
-   * Define your command CLI interface in a clear, DRY and safe way using type hints
-   * Create subcommand and group command hierarchies.
-   * Use the full power of Typer's parameter types to validate and parse command line inputs.
-   * Create beautiful and information dense help outputs.
-   * Configure the rendering of exception stack traces using rich.
-   * `Install shell tab-completion support <https://django-typer.readthedocs.io/en/latest/shell_completion.html>`_
-     for TyperCommands and normal Django commands for bash_, zsh_, fish_ and powershell_.
-   * `Create custom and portable shell tab-completions for your CLI parameters <https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions>`_.
-   * Refactor existing management commands into TyperCommands because TyperCommand is interface
-     compatible with BaseCommand.
-
-Please refer to the `full documentation <https://django-typer.readthedocs.io/>`_ for more information.
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif
-   :width: 100%
-   :align: center
-
-Installation
-------------
-
-1. Clone django-typer from GitHub or install a release off `PyPI <https://pypi.org/project/django-typer/>`_:
-
-    .. code:: bash
-
-        pip install django-typer
+- Define your command CLI interface in a clear, DRY, and safe way using type hints.
+- Create subcommand and group command hierarchies.
+- Use the full power of Typer's parameter types to validate and parse command line inputs.
+- Create beautiful and information dense help outputs.
+- Configure the rendering of exception stack traces using rich.
+- [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for TyperCommands and normal Django commands for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
+- [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
+- Refactor existing management commands into TyperCommands because TyperCommand is interface compatible with BaseCommand.
 
-    `rich <https://rich.readthedocs.io/en/latest/>`_ is a powerful library for rich text and
-    beautiful formatting in the terminal. It is not required, but highly recommended for the
-    best experience:
+Please refer to the [full documentation](https://django-typer.readthedocs.io/) for more information.
 
-    .. code:: bash
+![django-typer example](https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif)
 
-        pip install "django-typer[rich]"
+## Installation
 
+1. Clone django-typer from GitHub or install a release off [PyPI](https://pypi.org/project/django-typer/):
 
-2. Add ``django_typer`` to your ``INSTALLED_APPS`` setting:
+   ```bash
+   pip install django-typer
+   ```
 
-    .. code:: python
+   [rich](https://rich.readthedocs.io/en/latest/) is a powerful library for rich text and beautiful formatting in the terminal. It is not required but highly recommended for the best experience:
 
-        INSTALLED_APPS = [
-            ...
-            'django_typer',
-        ]
+   ```bash
+   pip install "django-typer[rich]"
+   ```
 
-   *You only need to install django_typer as an app if you want to use the shellcompletion command
-   to enable tab-completion or if you would like django-typer to install `rich traceback rendering 
-   <https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces>`_
-   for you - which it does by default if rich is also installed.*
+2. Add `django_typer` to your `INSTALLED_APPS` setting:
 
-Basic Example
--------------
+   ```python
+   INSTALLED_APPS = [
+       ...
+       'django_typer',
+   ]
+   ```
 
-For example TyperCommands can be a very simple drop in replacement for BaseCommands. All of the
-documented features of
-`BaseCommand <https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand>`_
-work!
+*You only need to install django_typer as an app if you want to use the shell completion command to enable tab-completion or if you would like django-typer to install [rich traceback rendering](https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces) for you - which it does by default if rich is also installed.*
 
+## Basic Example
 
-.. code-block:: python
+For example, TyperCommands can be a very simple drop-in replacement for BaseCommands. All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work!
 
-   from django_typer import TyperCommand
+```python
+from django_typer import TyperCommand
 
+class Command(TyperCommand):
+    def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
+        """
+        A basic command that uses Typer
+        """
+```
 
-   class Command(TyperCommand):
-
-      def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
-         """
-         A basic command that uses Typer
-         """
-
-
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg
-   :width: 100%
-   :align: center
-
+![Basic Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg)
 
-|
+## Multiple Subcommands Example
 
-Multiple Subcommands Example
------------------------------
 
-Or commands with multiple subcommands can be defined:
 
-.. code-block:: python
+Commands with multiple subcommands can be defined:
 
+```python
    import typing as t
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument
 
    from django_typer import TyperCommand, command
 
@@ -159,50 +103,30 @@
       def delete(
          self, id: t.Annotated[int, Argument(help=_("The id of the object to delete."))]
       ):
          """
          Delete an object.
          """
 
+```
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg
-   :width: 100%
-   :align: center
+![Multiple Subcommands Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg)
+![Multiple Subcommands Example - create](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg)
+![Multiple Subcommands Example - delete](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg)
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg
-   :width: 100%
-   :align: center
+## Grouping and Hierarchies Example
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg
-   :width: 100%
-   :align: center
+More complex groups and subcommand hierarchies can be defined. For example, this command defines a group of commands called math, with subcommands divide and multiply. The group has a common initializer that optionally sets a float precision value. We would invoke this command like so:
 
-|
-
-
-Grouping and Hierarchies Example
---------------------------------
-
-Or more complex groups and subcommand hierarchies can be defined. For example this command
-defines a group of commands called math, with subcommands divide and multiply. The group
-has a common initializer that optionally sets a float precision value. We would invoke this
-command like so:
-
-.. code:: bash
-
-    ./manage.py hierarchy math --precision 5 divide 10 2.1
-    4.76190
-    ./manage.py hierarchy math multiply 10 2
-    20.00
-
-Any number of groups and subcommands and subgroups of other groups can be defined allowing
-for arbitrarily complex command hierarchies.
-
-.. code-block:: python
+```bash
+./manage.py hierarchy math --precision 5 divide 10 2.1
+./manage.py hierarchy math multiply 10 2
+```
 
+```python
    import typing as t
    from functools import reduce
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument, Option
 
    from django_typer import TyperCommand, group
@@ -242,25 +166,13 @@
          """
          Divide the given numbers.
          """
          if floor:
                return str(numerator // denominator)
          return f"{numerator / denominator:.{self.precision}f}"
 
+```
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg
-   :width: 100%
-   :align: center
-
-|
+![Grouping and Hierarchies Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg)
+![Grouping and Hierarchies Example - math](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg)
+![Grouping and Hierarchies Example - math multiply](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg)
+![Grouping and Hierarchies Example - math divide](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg)
```

### Comparing `django_typer-1.0.9/django_typer/__init__.py` & `django_typer-1.1.0/django_typer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
 
-VERSION = (1, 0, 9)
+VERSION = (1, 1, 0)
 
 __title__ = "Django Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-2024 Brian Kohan"
```

### Comparing `django_typer-1.0.9/django_typer/apps.py` & `django_typer-1.1.0/django_typer/apps.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/completers.py` & `django_typer-1.1.0/django_typer/completers.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/management/commands/shellcompletion.py` & `django_typer-1.1.0/django_typer/management/commands/shellcompletion.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/parsers.py` & `django_typer-1.1.0/django_typer/parsers.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/patch.py` & `django_typer-1.1.0/django_typer/patch.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/types.py` & `django_typer-1.1.0/django_typer/types.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/django_typer/utils.py` & `django_typer-1.1.0/django_typer/utils.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.0.9/pyproject.toml` & `django_typer-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "django-typer"
-version = "1.0.9"
+version = "1.1.0"
 description = "Use Typer to define the CLI for your Django management commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/bckohan/django-typer"
 homepage = "https://django-typer.readthedocs.io"
 keywords = ["django", "CLI", "management", "Typer", "commands"]
 classifiers = [
     "Environment :: Console",
     "Framework :: Django",
     "Operating System :: OS Independent",
@@ -43,15 +43,15 @@
 python = ">=3.8,<4.0"
 Django = ">=3.2,<6.0"
 click = "^8.1.0"
 
 # typer's release history is full of breaking changes for minor versions
 # given the reliance on some of its private internals we peg the typer
 # version very strictly to bug fix releases for specific minor lines.
-typer = ">=0.9.0,<0.13.0"
+typer-slim = ">=0.12.0,<0.13.0"
 
 # this should track typer's rich dependency, so long as our console
 # patches still work - so be sure to test on the low end of the range
 rich = { version = ">=10.11.0,<14.0.0", optional = true }
 
 shellingham = ">=1.5.4"
 
@@ -71,15 +71,15 @@
 sphinx-rtd-theme = "^2.0.0"
 mypy = "^1.0"
 pylint = "^3.0"
 black = ">=23.12"
 doc8 = "^1.1.1"
 aiohttp = "^3.9.1"
 readme-renderer = {extras = ["md"], version = ">=42,<44"}
-sphinxcontrib-typer = {extras = ["html", "pdf", "png"], version = "^0.1.11"}
+sphinxcontrib-typer = {extras = ["html", "pdf", "png"], version = "^0.2.0"}
 scikit-learn = "^1.0.0"
 pytest-env = "^1.0.0"
 numpy = [
     { version = ">=1.26", markers = "python_version > '3.8'" },
     { version = "<=1.24", markers = "python_version <= '3.8'" },
 ]
 scipy = [
```

### Comparing `django_typer-1.0.9/PKG-INFO` & `django_typer-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typer
-Version: 1.0.9
+Version: 1.1.0
 Summary: Use Typer to define the CLI for your Django management commands.
 Home-page: https://django-typer.readthedocs.io
 License: MIT
 Keywords: django,CLI,management,Typer,commands
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -32,154 +32,98 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: rich
 Requires-Dist: Django (>=3.2,<6.0)
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: rich (>=10.11.0,<14.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.4)
-Requires-Dist: typer (>=0.9.0,<0.13.0)
+Requires-Dist: typer-slim (>=0.12.0,<0.13.0)
 Requires-Dist: typing-extensions (>=3.7.4.3) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/bckohan/django-typer
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPi djversions| |PyPI status| |Documentation Status|
-|Code Cov| |Test Status| |Lint Status| |Code Style|
+# django-typer
 
-.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-   :target: https://lbesson.mit-license.org/
 
-.. |PyPI version fury.io| image:: https://badge.fury.io/py/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer/
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
+[![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
+[![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
+[![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
+[![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
+[![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
+[![Lint Status](https://github.com/bckohan/django-typer/workflows/lint/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/lint.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer/
-
-.. |PyPI djversions| image:: https://img.shields.io/pypi/djversions/django-typer.svg
-   :target: https://pypi.org/project/django-typer/
-
-.. |PyPI status| image:: https://img.shields.io/pypi/status/django-typer.svg
-   :target: https://pypi.python.org/pypi/django-typer
-
-.. |Documentation Status| image:: https://readthedocs.org/projects/django-typer/badge/?version=latest
-   :target: http://django-typer.readthedocs.io/?badge=latest/
-
-.. |Code Cov| image:: https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL
-   :target: https://codecov.io/gh/bckohan/django-typer
-
-.. |Test Status| image:: https://github.com/bckohan/django-typer/workflows/test/badge.svg
-   :target: https://github.com/bckohan/django-typer/actions/workflows/test.yml
-
-.. |Lint Status| image:: https://github.com/bckohan/django-typer/workflows/lint/badge.svg
-   :target: https://github.com/bckohan/django-typer/actions/workflows/lint.yml
-
-.. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-.. _powershell: https://learn.microsoft.com/en-us/powershell/scripting/overview
-.. _fish: https://fishshell.com/
-.. _zsh: https://www.zsh.org/
-.. _bash: https://www.gnu.org/software/bash/
-.. _Django: https://www.djangoproject.com/
-
-django-typer
-############
-
-Use `Typer <https://typer.tiangolo.com/>`_ to define the CLI for your Django_ management commands. 
-Provides a TyperCommand class that inherits from `BaseCommand <https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand>`_
-and allows typer-style annotated parameter types. All of the BaseCommand functionality is
-preserved, so that TyperCommand can be a drop in replacement.
+Use [Typer](https://typer.tiangolo.com/) to define the CLI for your [Django](https://www.djangoproject.com/) management commands. Provides a TyperCommand class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) and allows typer-style annotated parameter types. All of the BaseCommand functionality is preserved, so that TyperCommand can be a drop-in replacement.
 
 **django-typer makes it easy to:**
 
-   * Define your command CLI interface in a clear, DRY and safe way using type hints
-   * Create subcommand and group command hierarchies.
-   * Use the full power of Typer's parameter types to validate and parse command line inputs.
-   * Create beautiful and information dense help outputs.
-   * Configure the rendering of exception stack traces using rich.
-   * `Install shell tab-completion support <https://django-typer.readthedocs.io/en/latest/shell_completion.html>`_
-     for TyperCommands and normal Django commands for bash_, zsh_, fish_ and powershell_.
-   * `Create custom and portable shell tab-completions for your CLI parameters <https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions>`_.
-   * Refactor existing management commands into TyperCommands because TyperCommand is interface
-     compatible with BaseCommand.
-
-Please refer to the `full documentation <https://django-typer.readthedocs.io/>`_ for more information.
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif
-   :width: 100%
-   :align: center
-
-Installation
-------------
-
-1. Clone django-typer from GitHub or install a release off `PyPI <https://pypi.org/project/django-typer/>`_:
-
-    .. code:: bash
-
-        pip install django-typer
+- Define your command CLI interface in a clear, DRY, and safe way using type hints.
+- Create subcommand and group command hierarchies.
+- Use the full power of Typer's parameter types to validate and parse command line inputs.
+- Create beautiful and information dense help outputs.
+- Configure the rendering of exception stack traces using rich.
+- [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for TyperCommands and normal Django commands for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
+- [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
+- Refactor existing management commands into TyperCommands because TyperCommand is interface compatible with BaseCommand.
 
-    `rich <https://rich.readthedocs.io/en/latest/>`_ is a powerful library for rich text and
-    beautiful formatting in the terminal. It is not required, but highly recommended for the
-    best experience:
+Please refer to the [full documentation](https://django-typer.readthedocs.io/) for more information.
 
-    .. code:: bash
+![django-typer example](https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif)
 
-        pip install "django-typer[rich]"
+## Installation
 
+1. Clone django-typer from GitHub or install a release off [PyPI](https://pypi.org/project/django-typer/):
 
-2. Add ``django_typer`` to your ``INSTALLED_APPS`` setting:
+   ```bash
+   pip install django-typer
+   ```
 
-    .. code:: python
+   [rich](https://rich.readthedocs.io/en/latest/) is a powerful library for rich text and beautiful formatting in the terminal. It is not required but highly recommended for the best experience:
 
-        INSTALLED_APPS = [
-            ...
-            'django_typer',
-        ]
+   ```bash
+   pip install "django-typer[rich]"
+   ```
 
-   *You only need to install django_typer as an app if you want to use the shellcompletion command
-   to enable tab-completion or if you would like django-typer to install `rich traceback rendering 
-   <https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces>`_
-   for you - which it does by default if rich is also installed.*
+2. Add `django_typer` to your `INSTALLED_APPS` setting:
 
-Basic Example
--------------
+   ```python
+   INSTALLED_APPS = [
+       ...
+       'django_typer',
+   ]
+   ```
 
-For example TyperCommands can be a very simple drop in replacement for BaseCommands. All of the
-documented features of
-`BaseCommand <https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand>`_
-work!
+*You only need to install django_typer as an app if you want to use the shell completion command to enable tab-completion or if you would like django-typer to install [rich traceback rendering](https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces) for you - which it does by default if rich is also installed.*
 
+## Basic Example
 
-.. code-block:: python
+For example, TyperCommands can be a very simple drop-in replacement for BaseCommands. All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work!
 
-   from django_typer import TyperCommand
+```python
+from django_typer import TyperCommand
 
+class Command(TyperCommand):
+    def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
+        """
+        A basic command that uses Typer
+        """
+```
 
-   class Command(TyperCommand):
-
-      def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
-         """
-         A basic command that uses Typer
-         """
-
-
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg
-   :width: 100%
-   :align: center
-
+![Basic Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg)
 
-|
+## Multiple Subcommands Example
 
-Multiple Subcommands Example
------------------------------
 
-Or commands with multiple subcommands can be defined:
 
-.. code-block:: python
+Commands with multiple subcommands can be defined:
 
+```python
    import typing as t
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument
 
    from django_typer import TyperCommand, command
 
@@ -202,50 +146,30 @@
       def delete(
          self, id: t.Annotated[int, Argument(help=_("The id of the object to delete."))]
       ):
          """
          Delete an object.
          """
 
+```
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg
-   :width: 100%
-   :align: center
+![Multiple Subcommands Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg)
+![Multiple Subcommands Example - create](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg)
+![Multiple Subcommands Example - delete](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg)
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg
-   :width: 100%
-   :align: center
+## Grouping and Hierarchies Example
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg
-   :width: 100%
-   :align: center
+More complex groups and subcommand hierarchies can be defined. For example, this command defines a group of commands called math, with subcommands divide and multiply. The group has a common initializer that optionally sets a float precision value. We would invoke this command like so:
 
-|
-
-
-Grouping and Hierarchies Example
---------------------------------
-
-Or more complex groups and subcommand hierarchies can be defined. For example this command
-defines a group of commands called math, with subcommands divide and multiply. The group
-has a common initializer that optionally sets a float precision value. We would invoke this
-command like so:
-
-.. code:: bash
-
-    ./manage.py hierarchy math --precision 5 divide 10 2.1
-    4.76190
-    ./manage.py hierarchy math multiply 10 2
-    20.00
-
-Any number of groups and subcommands and subgroups of other groups can be defined allowing
-for arbitrarily complex command hierarchies.
-
-.. code-block:: python
+```bash
+./manage.py hierarchy math --precision 5 divide 10 2.1
+./manage.py hierarchy math multiply 10 2
+```
 
+```python
    import typing as t
    from functools import reduce
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument, Option
 
    from django_typer import TyperCommand, group
@@ -285,26 +209,14 @@
          """
          Divide the given numbers.
          """
          if floor:
                return str(numerator // denominator)
          return f"{numerator / denominator:.{self.precision}f}"
 
+```
 
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg
-   :width: 100%
-   :align: center
-
-.. image:: https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg
-   :width: 100%
-   :align: center
-
-|
+![Grouping and Hierarchies Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg)
+![Grouping and Hierarchies Example - math](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg)
+![Grouping and Hierarchies Example - math multiply](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg)
+![Grouping and Hierarchies Example - math divide](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg)
```


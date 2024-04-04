# Comparing `tmp/tinta-0.1.7b3.tar.gz` & `tmp/tinta-0.1.7b4.tar.gz`

## Comparing `tinta-0.1.7b3.tar` & `tinta-0.1.7b4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b3/DESCRIPTION.rst
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b3/HIPPOCRATIC_LICENSE.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b3/MANIFEST.in
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tinta-0.1.7b3/Pipfile
--rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b3/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b3/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b3/requirements-dev.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tinta-0.1.7b3/requirements.txt
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b3/setup.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/launch.json
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/settings.json
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/tasks.json
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/basic_example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/colors.ini
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/complete_example.py
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/tinta-discover.png
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b3/junit/test-results.xml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/conftest.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_colors_invalid.ini
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_discover.py
--rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_tinta.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/__main__.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/ansi.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/colorize.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/colors.ini
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/constants.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/discover.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/multi_version_imports.py
--rw-r--r--   0        0        0    25608 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/tinta.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/typ.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/utils.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b3/LICENSE
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 tinta-0.1.7b3/README.md
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tinta-0.1.7b3/pyproject.toml
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 tinta-0.1.7b3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b4/DESCRIPTION.rst
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b4/HIPPOCRATIC_LICENSE.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b4/MANIFEST.in
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinta-0.1.7b4/Pipfile
+-rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b4/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b4/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b4/requirements-dev.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tinta-0.1.7b4/requirements.txt
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b4/setup.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.vscode/launch.json
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.vscode/settings.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.vscode/tasks.json
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b4/examples/basic_example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b4/examples/colors.ini
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tinta-0.1.7b4/examples/complete_example.py
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b4/examples/tinta-discover.png
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b4/junit/test-results.xml
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tests/conftest.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tests/test_colors_invalid.ini
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tests/test_discover.py
+-rw-r--r--   0        0        0    24946 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tests/test_tinta.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/__main__.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/ansi.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/colorize.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/colors.ini
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/constants.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/discover.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/multi_version_imports.py
+-rw-r--r--   0        0        0    25619 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/tinta.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/typ.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b4/tinta/utils.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b4/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b4/LICENSE
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 tinta-0.1.7b4/README.md
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tinta-0.1.7b4/pyproject.toml
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 tinta-0.1.7b4/PKG-INFO
```

### Comparing `tinta-0.1.7b3/CODE_OF_CONDUCT.md` & `tinta-0.1.7b4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/HIPPOCRATIC_LICENSE.md` & `tinta-0.1.7b4/HIPPOCRATIC_LICENSE.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/Pipfile` & `tinta-0.1.7b4/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-deprecated = "*"
+deprecated = "^1.2.14"
 
 [dev-packages]
 pipenv = "*"
 pylint = "*"
 autopep8 = "*"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `tinta-0.1.7b3/Pipfile.lock` & `tinta-0.1.7b4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/setup.py` & `tinta-0.1.7b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from setuptools import setup
 
 with Path("README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="tinta",
-    version="0.1.7b3",
+    version="0.1.7b4",
     description="Tinta, a magical console output tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brandonscript/tinta",
     author="Brandon Shelley",
     author_email="brandon@pacificaviator.co",
     install_requires=[],
```

### Comparing `tinta-0.1.7b3/.github/workflows/publish-test.yml` & `tinta-0.1.7b4/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.github/workflows/publish.yml` & `tinta-0.1.7b4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.github/workflows/run-tests.yml` & `tinta-0.1.7b4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.vscode/launch.json` & `tinta-0.1.7b4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.vscode/settings.json` & `tinta-0.1.7b4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.vscode/tasks.json` & `tinta-0.1.7b4/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/examples/basic_example.py` & `tinta-0.1.7b4/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/examples/complete_example.py` & `tinta-0.1.7b4/examples/complete_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/examples/tinta-discover.png` & `tinta-0.1.7b4/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/junit/test-results.xml` & `tinta-0.1.7b4/junit/test-results.xml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tests/conftest.py` & `tinta-0.1.7b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tests/test_discover.py` & `tinta-0.1.7b4/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tests/test_tinta.py` & `tinta-0.1.7b4/tests/test_tinta.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 # to whom the Software is furnished to do so, subject to the conditions layed
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 
+import os
 import re
+from contextlib import contextmanager
 from typing import Any, Callable, Dict, List, Tuple
 
 import pytest
 from pytest import CaptureFixture
 
 # pylint: disable=import-error
 from tinta import Tinta
@@ -45,14 +47,22 @@
 PINK = "\x1b[38;5;197m"
 GRAY = "\x1b[38;5;243m"
 D_GRAY = "\x1b[38;5;235m"
 L_GRAY = "\x1b[38;5;248m"
 WHITE = "\x1b[38;5;255m"
 
 
+@contextmanager
+def skip_on_github_actions():
+    gh = bool(os.getenv("GITHUB_ACTIONS") == "true")
+    if gh:
+        pytest.mark.skipif(True, reason="Function skipped on GitHub Actions")
+    yield gh
+
+
 class TestInit:
 
     def test_init(self):
         assert len(Tinta("initialized").parts) == 1
 
 
 class TestBasicColorizing:
@@ -109,16 +119,18 @@
         kwargs: Dict[str, Any],
         expected: str,
         capfd: CaptureFixture[str],
     ):
         s = Testa().to_str(**kwargs)
         Testa().print(**kwargs)
         assert s == expected
-        out = capfd.readouterr().out
-        assert out == f"{expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         [
             (
                 lambda: Tinta().mint("Mint\nice cream"),
                 f"{MINT}Mint\nice cream{O}",
@@ -275,29 +287,33 @@
     )
     def test_uncolored_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
     ):
         s = Testa().to_str()
         assert s == expected
         Testa().print()
-        out = capfd.readouterr().out
-        assert out == f"{expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         whitespace_cases,
     )
     def test_uncolored_plaintext_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
     ):
         p = Testa().to_str(plaintext=True)
         assert p == expected
         Testa().print(plaintext=True)
-        out = capfd.readouterr().out
-        assert out == f"{expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         whitespace_cases,
     )
     def test_proxy_color_to_str_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
@@ -306,29 +322,33 @@
         found = re.search(r"\s+$", expected)
         trail_ws = found.group() if found else ""
         _expected = f"{PURPLE}{expected.rstrip()}{O}{trail_ws}"
         #                                         ^^^^^^^^^^^^^
         # Reset ANSI char is always placed before trailing whitespace
         assert Tinta().purple(s).to_str() == _expected
         Tinta().purple(s).print()
-        out = capfd.readouterr().out
-        assert out == f"{_expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{_expected}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         whitespace_cases,
     )
     def test_proxy_color_to_plaintext_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
     ):
         p = Testa().to_str(plaintext=True)
         assert Tinta().purple(p).to_str(plaintext=True) == expected
         Tinta().purple(p).print(plaintext=True)
-        out = capfd.readouterr().out
-        assert out == f"{expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         whitespace_cases,
     )
     def test_proxy_color_chain_to_str_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
@@ -343,16 +363,18 @@
         # ^ If there is a newline at the end of the current or start of the next segment,
         #   Tinta will ignore the separator
         assert (
             Tinta().purple(s).pink(s).to_str()
             == f"{expected_purple}{sep}{expected_pink}"
         )
         Tinta().purple(s).pink(s).print()
-        out = capfd.readouterr().out
-        assert out == f"{expected_purple}{sep}{expected_pink}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected_purple}{sep}{expected_pink}\n"
 
     @pytest.mark.parametrize(
         "Testa,expected",
         whitespace_cases,
     )
     def test_proxy_color_chain_to_plaintext_respects_whitespace(
         self, Testa: Callable[[], Tinta], expected: str, capfd: CaptureFixture[str]
@@ -363,16 +385,18 @@
         # ^ If there is a newline at the end of the current or start of the next segment,
         #   Tinta will ignore the separator
         assert (
             Tinta().purple(p).pink(p).to_str(plaintext=True)
             == f"{expected}{sep}{expected}"
         )
         Tinta().purple(p).pink(p).print(plaintext=True)
-        out = capfd.readouterr().out
-        assert out == f"{expected}{sep}{expected}\n"
+        with skip_on_github_actions() as skip:
+            if not skip:
+                out = capfd.readouterr().out
+                assert out == f"{expected}{sep}{expected}\n"
 
     def test_sep_inherits_prev_part_color(self):
         assert (
             Tinta().red("Red").green("Green").blue("Blue").to_str(sep=";")
             == f"{RED}Red;{GREEN}Green;{BLUE}Blue{O}"
         )
```

### Comparing `tinta-0.1.7b3/tinta/__init__.py` & `tinta-0.1.7b4/tinta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.7b3"
+__version__ = "0.1.7b4"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 
     assert bool(Tinta)
```

### Comparing `tinta-0.1.7b3/tinta/__main__.py` & `tinta-0.1.7b4/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tinta/ansi.py` & `tinta-0.1.7b4/tinta/ansi.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tinta/colorize.py` & `tinta-0.1.7b4/tinta/colorize.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tinta/constants.py` & `tinta-0.1.7b4/tinta/constants.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tinta/discover.py` & `tinta-0.1.7b4/tinta/discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/tinta/multi_version_imports.py` & `tinta-0.1.7b4/tinta/multi_version_imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     GenericCallable = Any
 
 # Deprecated
 try:
     from warnings import deprecated
 except ImportError:
     from deprecated import deprecated
+deprecated = deprecated
 
 
 all = [
     deprecated,
     GenericCallable,
     Literal,
     T,
```

### Comparing `tinta-0.1.7b3/tinta/tinta.py` & `tinta-0.1.7b4/tinta/tinta.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,27 +21,26 @@
 import os
 import re
 import sys
 from itertools import zip_longest
 from pathlib import Path
 from typing import Any, cast, Dict, List, Optional, overload, Union
 
-from deprecated import deprecated
-
 from .ansi import AnsiColors
 from .colorize import colorize, ensure_reset, tint, was_reset
 from .constants import (
     CURSOR_UP_ONE,
     ERASE_LINE,
     PREFER_PLAINTEXT,
     SEP,
     SMART_FIX_PUNCTUATION,
     STEALTH,
 )
 from .discover import discover as _discover
+from .multi_version_imports import deprecated
 from .typ import copy_kwargs, MissingColorError, StringType
 
 config = configparser.ConfigParser()
 
 
 class _MetaTinta(type):
```

### Comparing `tinta-0.1.7b3/tinta/typ.py` & `tinta-0.1.7b4/tinta/typ.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/.gitignore` & `tinta-0.1.7b4/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/LICENSE` & `tinta-0.1.7b4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b3/README.md` & `tinta-0.1.7b4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b3-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b4-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -189,15 +189,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b3 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b4 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -224,15 +224,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b3 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b4 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```

### Comparing `tinta-0.1.7b3/pyproject.toml` & `tinta-0.1.7b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.7b3"
+version = "0.1.7b4"
 description = "Tinta, a magical console output tool."
 authors = [{ name = "Brandon Shelley", email = "brandon@pacificaviator.co" }]
 license = "MIT"
 readme = "README.md"
 keywords = [
   "console",
   "colors",
```

### Comparing `tinta-0.1.7b3/PKG-INFO` & `tinta-0.1.7b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinta
-Version: 0.1.7b3
+Version: 0.1.7b4
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,cli,colors,console,development,print,term,terminal
@@ -25,15 +25,15 @@
 
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b3-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b4-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -214,15 +214,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b3 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b4 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -249,15 +249,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b3 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b4 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```


# Comparing `tmp/attr_utils-0.9.0.tar.gz` & `tmp/attr_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attr_utils-0.9.0.tar", last modified: Mon Jul 31 14:53:10 2023, max compression
+gzip compressed data, was "attr_utils-1.0.0.tar", last modified: Thu Apr  4 17:00:09 2024, max compression
```

## Comparing `attr_utils-0.9.0.tar` & `attr_utils-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-31 14:53:10.092008 attr_utils-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-31 14:53:10.100008 attr_utils-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-31 14:53:10.100008 attr_utils-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-07-31 14:53:10.104008 attr_utils-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-07-31 14:53:10.100008 attr_utils-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-31 14:52:34.031780 attr_utils-0.9.0/attr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/mypy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-07-31 14:52:34.031780 attr_utils-0.9.0/attr_utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/pprinter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12736 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/autoattrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-04 17:00:09.480480 attr_utils-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 17:00:09.476480 attr_utils-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 17:00:09.480480 attr_utils-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-04 17:00:09.480480 attr_utils-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-04 17:00:09.484480 attr_utils-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/pprinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/mypy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 16:59:44.736285 attr_utils-1.0.0/attr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-04 16:59:44.740285 attr_utils-1.0.0/attr_utils/autoattrs.py
```

### Comparing `attr_utils-0.9.0/LICENSE` & `attr_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/README.rst` & `attr_utils-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v1.0.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/attr_utils
 	:target: https://pypi.org/project/attr_utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `attr_utils-0.9.0/PKG-INFO` & `attr_utils-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: attr-utils
-Version: 0.9.0
+Version: 1.0.0
 Summary: Utilities to augment attrs.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: attrs,documentation,serde,sphinx
 Home-page: https://github.com/domdfcoding/attr_utils
 Project-URL: Issue Tracker, https://github.com/domdfcoding/attr_utils/issues
 Project-URL: Source Code, https://github.com/domdfcoding/attr_utils
@@ -13,36 +13,36 @@
 Platform: macOS
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Requires-Dist: attrs>=21.2.0
+Requires-Python: >=3.7
+Requires-Dist: attrs<23.2.0,>=21.2.0
 Requires-Dist: domdf-python-tools>=3.6.1
 Requires-Dist: toolz>=0.11.1
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: typing-inspect>=0.6.0; python_version == "3.6"
 Requires-Dist: prettyprinter==0.18.0; extra == 'pprint'
-Requires-Dist: sphinx<5,>=3.2.0; extra == 'sphinx'
-Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'sphinx'
+Requires-Dist: sphinx<7,>=3.2.0; extra == 'sphinx'
+Requires-Dist: sphinx-toolbox>=3.3.0; extra == 'sphinx'
 Requires-Dist: prettyprinter==0.18.0; extra == 'all'
-Requires-Dist: sphinx<5,>=3.2.0; extra == 'all'
-Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'all'
+Requires-Dist: sphinx<7,>=3.2.0; extra == 'all'
+Requires-Dist: sphinx-toolbox>=3.3.0; extra == 'all'
 Provides-Extra: pprint
 Provides-Extra: sphinx
 Provides-Extra: all
 Description-Content-Type: text/x-rst
 
 
 ###########
@@ -144,23 +144,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v1.0.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/attr_utils
 	:target: https://pypi.org/project/attr_utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `attr_utils-0.9.0/pyproject.toml` & `attr_utils-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "attr_utils"
-version = "0.9.0"
+version = "1.0.0"
 description = "Utilities to augment attrs."
 readme = "README.rst"
 keywords = [ "attrs", "documentation", "serde", "sphinx",]
 dynamic = []
 dependencies = [
-    "attrs>=21.2.0",
+    "attrs<23.2.0,>=21.2.0",
     "domdf-python-tools>=3.6.1",
     "toolz>=0.11.1",
     "typing-extensions>=4.0.0",
     'typing-inspect>=0.6.0; python_version == "3.6"',
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
 
 [project.license]
@@ -47,16 +47,16 @@
 Homepage = "https://github.com/domdfcoding/attr_utils"
 "Issue Tracker" = "https://github.com/domdfcoding/attr_utils/issues"
 "Source Code" = "https://github.com/domdfcoding/attr_utils"
 Documentation = "https://attr-utils.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 pprint = [ "prettyprinter==0.18.0",]
-sphinx = [ "sphinx<5,>=3.2.0", "sphinx-toolbox>=2.16.0",]
-all = [ "prettyprinter==0.18.0", "sphinx<5,>=3.2.0", "sphinx-toolbox>=2.16.0",]
+sphinx = [ "sphinx<7,>=3.2.0", "sphinx-toolbox>=3.3.0",]
+all = [ "prettyprinter==0.18.0", "sphinx<7,>=3.2.0", "sphinx-toolbox>=3.3.0",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
@@ -146,21 +146,21 @@
 
 [tool.whey]
 base-classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 plugins = [ "attr_utils.mypy_plugin",]
 incremental = false
```

### Comparing `attr_utils-0.9.0/attr_utils/docstrings.py` & `attr_utils-1.0.0/attr_utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/attr_utils/serialise.py` & `attr_utils-1.0.0/attr_utils/serialise.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/attr_utils/__init__.py` & `attr_utils-1.0.0/attr_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.9.0"
+__version__: str = "1.0.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 _docs = False
```

### Comparing `attr_utils-0.9.0/attr_utils/mypy_plugin.py` & `attr_utils-1.0.0/attr_utils/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/attr_utils/annotations.py` & `attr_utils-1.0.0/attr_utils/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,17 @@
 import attr_utils
 
 if sys.version_info > (3, 7):  # pragma: no cover (<py37)
 	# 3rd party
 	from typing_extensions import get_origin
 else:  # pragma: no cover (py37+)
 	# 3rd party
-	from typing_inspect import get_origin  # type: ignore
+	from typing_inspect import get_origin
 
-if TYPE_CHECKING or attr_utils._docs:
+if TYPE_CHECKING or attr_utils._docs:  # pragma: no cover
 	# 3rd party
 	from sphinx.application import Sphinx
 	from sphinx_toolbox.utils import SphinxExtMetadata
 
 __all__ = ["attrib", "_A", "_C", "add_init_annotations", "attr_docstring_hook", "setup"]
 
 _A = TypeVar("_A", bound=Any)
@@ -297,17 +297,15 @@
 
 
 ################################
 # Demo
 ################################
 
 
-def parse_occupations(  # pragma: no cover
-		occupations: Iterable[str],
-		) -> Iterable[str]:
+def parse_occupations(occupations: Iterable[str]) -> Iterable[str]:  # pragma: no cover
 
 	if isinstance(occupations, str):
 		return [x.strip() for x in occupations.split(',')]
 	else:
 		return [str(x) for x in occupations]
```

### Comparing `attr_utils-0.9.0/attr_utils/pprinter.py` & `attr_utils-1.0.0/attr_utils/pprinter.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/attr_utils/utils.py` & `attr_utils-1.0.0/attr_utils/utils.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.9.0/attr_utils/autoattrs.py` & `attr_utils-1.0.0/attr_utils/autoattrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,34 +93,57 @@
 #  |  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  |  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  |  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  |  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
-import warnings
 from textwrap import dedent
-from typing import Any, Dict, List, MutableMapping, Optional, Tuple, Type
+from typing import TYPE_CHECKING, Any, Dict, List, MutableMapping, Optional, Tuple, Type
 
 # 3rd party
 import attr
 from sphinx.application import Sphinx  # nodep
-from sphinx.deprecation import RemovedInSphinx50Warning  # nodep
 from sphinx.ext.autodoc import ClassDocumenter, Documenter  # nodep
 from sphinx.pycode import ModuleAnalyzer  # nodep
 from sphinx_toolbox import __version__  # nodep
 from sphinx_toolbox.more_autosummary import PatchedAutoSummClassDocumenter  # nodep
 from sphinx_toolbox.utils import Param, SphinxExtMetadata, flag, parse_parameters, unknown_module_warning  # nodep
 
 # this package
 from attr_utils.docstrings import add_attrs_doc
 from attr_utils.utils import AttrsClass
 
 __all__ = ["AttrsDocumenter", "setup"]
 
+if TYPE_CHECKING:
+	# 3rd party
+	from docutils.statemachine import StringList  # type: ignore[import]
+
+
+def _documenter_add_content(
+		self: Documenter,
+		more_content: Optional["StringList"],
+		) -> None:
+
+	# set sourcename and add content from attribute documentation
+	sourcename = self.get_sourcename()
+	if self.analyzer:
+		if self.objpath:
+			key = ('.'.join(self.objpath[:-1]), self.objpath[-1])
+			attr_docs = self.analyzer.find_attr_docs()
+			if key in attr_docs:
+				for i, line in enumerate(self.process_doc([list(attr_docs[key])])):
+					self.add_line(line, sourcename, i)
+
+	# add additional content (e.g. from document), if present
+	if more_content:
+		for line, src in zip(more_content.data, more_content.items):
+			self.add_line(line, src[0], src[1])
+
 
 class AttrsDocumenter(PatchedAutoSummClassDocumenter):
 	r"""
 	Sphinx autodoc :class:`~sphinx.ext.autodoc.Documenter`
 	for documenting `attrs <https://www.attrs.org/>`__ classes.
 
 	.. versionchanged:: 0.3.0
@@ -164,18 +187,15 @@
 		"""
 		Add extra content (from docstrings, attribute docs etc.), but not the class docstring.
 
 		:param more_content:
 		:param no_docstring:
 		"""
 
-		with warnings.catch_warnings():
-			# TODO: work out what to do about this
-			warnings.simplefilter("ignore", RemovedInSphinx50Warning)
-			Documenter.add_content(self, more_content, True)
+		_documenter_add_content(self, more_content)
 
 		# set sourcename and add content from attribute documentation
 		sourcename = self.get_sourcename()
 
 		self.add_line('', sourcename)
 
 		if hasattr(self.object, "__attrs_init__"):
```


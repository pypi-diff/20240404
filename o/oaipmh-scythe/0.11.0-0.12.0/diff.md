# Comparing `tmp/oaipmh_scythe-0.11.0.tar.gz` & `tmp/oaipmh_scythe-0.12.0.tar.gz`

## Comparing `oaipmh_scythe-0.11.0.tar` & `oaipmh_scythe-0.12.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/CHANGELOG.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/__about__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/__init__.py
--rw-r--r--   0        0        0    17979 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/client.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/exceptions.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/iterator.py
--rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/py.typed
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/response.py
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/src/oaipmh_scythe/utils.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/AUTHORS.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/LICENSE
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/README.md
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/pyproject.toml
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 oaipmh_scythe-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/CHANGELOG.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/__about__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/__init__.py
+-rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/client.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/exceptions.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/iterator.py
+-rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/py.typed
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/response.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/utils.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/.gitignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/AUTHORS.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/LICENSE
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/README.md
+-rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/PKG-INFO
```

### Comparing `oaipmh_scythe-0.11.0/CHANGELOG.md` & `oaipmh_scythe-0.12.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,34 @@
 
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). See
 [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit guidelines.
 
 
-## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.11.0...main)
+## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.0...main)
 
 
 
+## [0.12.0](https://github.com/afuetterer/oaipmh-scythe/compare/0.11.0...0.12.0) (2024-04-04)
+
+### Features
+
+- **client:** add authentication parameter (#316) ([`035c0fe`](https://github.com/afuetterer/oaipmh-scythe/commit/035c0fe4af20c1a749ce3dc02d1f5174aa13c57c))
+
+### Documentation
+
+- **readme:** add download badges to readme (#294) ([`c375ea9`](https://github.com/afuetterer/oaipmh-scythe/commit/c375ea935e226b3fc8a16ae9e2e023b7713c32b5))
+- add pypi project version to release notes template (#282) ([`c9d37ea`](https://github.com/afuetterer/oaipmh-scythe/commit/c9d37ea6e698f2706ac6cf893e9e97f4f2cd1c3c))
+- update environment section in bug report template (#281) ([`a2c225a`](https://github.com/afuetterer/oaipmh-scythe/commit/a2c225a3fc38ada61386a6abd8310bec79c6e482))
+- add ci to types of changes in pr template (#272) ([`f2745e7`](https://github.com/afuetterer/oaipmh-scythe/commit/f2745e74eaf2714eee8b6133924d15b050cc9ac9))
+- rename code of conduct (#270) ([`1994bf3`](https://github.com/afuetterer/oaipmh-scythe/commit/1994bf39cf76321dad509c189d1b7757f7bd21fb))
+- add license headers to documentation (#258) ([`63aa318`](https://github.com/afuetterer/oaipmh-scythe/commit/63aa318d94607571e4852315c310c71593257791))
+
+
 ## [0.11.0](https://github.com/afuetterer/oaipmh-scythe/compare/0.10.0...0.11.0) (2024-01-25)
 
 ### Features
 
 - set up logging of http requests (#250) ([`3df5ba1`](https://github.com/afuetterer/oaipmh-scythe/commit/3df5ba1c3247b38bc8fa0414b070296fc309a5ef))
 
 ### Documentation
```

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/client.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from oaipmh_scythe.response import OAIResponse
 from oaipmh_scythe.utils import filter_dict_except_resumption_token, log_response, remove_none_values
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, Iterator
     from types import TracebackType
 
+    from httpx._types import AuthTypes
+
 logger = logging.getLogger(__name__)
 
 USER_AGENT: str = f"oaipmh-scythe/{__version__}"
 OAI_NAMESPACE: str = "{http://www.openarchives.org/OAI/2.0/}"
 
 
 # Map OAI verbs to class representations
@@ -57,14 +59,15 @@
         http_method: The HTTP method to use for requests (either 'GET' or 'POST').
         iterator: The iterator class to be used for iterating over responses.
         max_retries: The maximum number of retries for a request in case of failures.
         retry_status_codes: The HTTP status codes on which to retry the request.
         default_retry_after: The default wait time (in seconds) between retries if no 'retry-after' header is present.
         class_mapping: A mapping from OAI verbs to classes representing OAI items.
         encoding: The character encoding for decoding responses. Defaults to the server's specified encoding.
+        auth: Optional authentication credentials for accessing the OAI-PMH interface.
         timeout: The timeout (in seconds) for HTTP requests.
 
     Examples:
         >>> with Scythe("https://zenodo.org/oai2d") as scythe:
         >>>     records = scythe.list_records()
         >>>     for record in records:
         >>>         print(record)
@@ -77,14 +80,15 @@
         http_method: str = "GET",
         iterator: type[BaseOAIIterator] = OAIItemIterator,
         max_retries: int = 0,
         retry_status_codes: Iterable[int] | None = None,
         default_retry_after: int = 60,
         class_mapping: dict[str, type[OAIItem]] | None = None,
         encoding: str | None = None,
+        auth: AuthTypes | None = None,
         timeout: int = 60,
     ):
         self.endpoint = endpoint
         if http_method not in ("GET", "POST"):
             raise ValueError("Invalid HTTP method: %s! Must be GET or POST.")
         self.http_method = http_method
         if inspect.isclass(iterator) and issubclass(iterator, BaseOAIIterator):
@@ -93,14 +97,15 @@
             raise TypeError("Argument 'iterator' must be subclass of %s" % BaseOAIIterator.__name__)
         self.max_retries = max_retries
         self.retry_status_codes = retry_status_codes or (503,)
         self.default_retry_after = default_retry_after
         self.oai_namespace = OAI_NAMESPACE
         self.class_mapping = class_mapping or DEFAULT_CLASS_MAP
         self.encoding = encoding
+        self.auth = auth
         self.timeout = timeout
         self._client: httpx.Client | None = None
 
     @property
     def client(self) -> httpx.Client:
         """Provide a reusable HTTP client instance for making requests.
 
@@ -109,15 +114,17 @@
         ensures that a new client is created if the existing one is closed.
 
         Returns:
             A reusable HTTP client instance for making HTTP requests.
         """
         if self._client is None or self._client.is_closed:
             headers = {"Accept": "text/xml; charset=utf-8", "user-agent": USER_AGENT}
-            self._client = httpx.Client(headers=headers, timeout=self.timeout, event_hooks={"response": [log_response]})
+            self._client = httpx.Client(
+                headers=headers, timeout=self.timeout, auth=self.auth, event_hooks={"response": [log_response]}
+            )
         return self._client
 
     def close(self) -> None:
         """Close the internal HTTP client if it exists and is open.
 
         This method is responsible for explicitly closing the `httpx.Client` instance used
         by the `Scythe` class. It should be called when the client is no longer needed, to
@@ -153,15 +160,15 @@
         Raises:
             HTTPError: If the HTTP request fails after the maximum number of retries.
         """
         http_response = self._request(query)
         for _ in range(self.max_retries):
             if httpx.codes.is_error(http_response.status_code) and http_response.status_code in self.retry_status_codes:
                 retry_after = self.get_retry_after(http_response)
-                logger.warning("HTTP %d! Retrying after %d seconds..." % (http_response.status_code, retry_after))
+                logger.warning("HTTP %d! Retrying after %d seconds...", http_response.status_code, retry_after)
                 time.sleep(retry_after)
                 http_response = self._request(query)
         http_response.raise_for_status()
         if self.encoding:
             http_response.encoding = self.encoding
         return OAIResponse(http_response, params=query)
```

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/exceptions.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/exceptions.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/iterator.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/iterator.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/models.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/models.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/response.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/response.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/src/oaipmh_scythe/utils.py` & `oaipmh_scythe-0.12.0/src/oaipmh_scythe/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         dict[str, Any]: A filtered dictionary based on the defined criteria.
     """
     allowed_keys = ("verb", "resumptionToken")
     resumption_token_present = d["resumptionToken"] is not None
     non_empty_keys = [k for k, v in d.items() if v is not None and k not in allowed_keys]
     if resumption_token_present and resumption_token_present:
         logger.warning(
-            f"`resumption_token` should not be used in combination with other parameters. Dropping {non_empty_keys}"
+            "`resumption_token` should not be used in combination with other parameters. Dropping %s", non_empty_keys
         )
         return {k: v for k, v in d.items() if k in allowed_keys}
     return d
 
 
 def get_namespace(element: etree._Element) -> str | None:
     """Return the namespace URI of an XML element.
```

### Comparing `oaipmh_scythe-0.11.0/.gitignore` & `oaipmh_scythe-0.12.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/LICENSE` & `oaipmh_scythe-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.11.0/pyproject.toml` & `oaipmh_scythe-0.12.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "A Scythe for harvesting OAI-PMH repositories."
 readme = "README.md"
 keywords = [
   "metadata",
   "oai-pmh",
   "oai-pmh-client",
 ]
-license = "BSD-3-Clause"
+license = {text = "BSD-3-Clause"}
 authors = [
   { name = "Heinz-Alexander Fütterer" },
 ]
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
@@ -34,33 +34,28 @@
 ]
 dependencies = [
   "httpx>=0.25",
   "lxml>=5.1",
 ]
 [project.optional-dependencies]
 dev = [
-  "oaipmh-scythe[lint]",
-  "oaipmh-scythe[test]",
-  "pipdeptree~=2.13",
+  "pre-commit~=3.6",
 ]
 docs = [
   "mkdocs~=1.5",
   "mkdocs-include-markdown-plugin~=6.0",
   "mkdocs-material~=9.5",
   "mkdocstrings[python]~=0.24",
 ]
-lint = [
-  "pre-commit~=3.6",
-]
 release = [
-  "python-semantic-release~=8.7",
+  "python-semantic-release~=9.1",
 ]
 test = [
-  "pytest~=7.4",
-  "pytest-cov~=4.1",
+  "pytest~=8.0",
+  "pytest-cov~=5.0",
   "pytest-mock~=3.12",
   "pytest-randomly~=3.15",
   "pytest-recording~=0.13",
   "pytest-xdist~=3.5",
   "respx~=0.20",
 ]
 [project.urls]
@@ -84,71 +79,68 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src/oaipmh_scythe"]
 
 [tool.hatch.version]
 path = "src/oaipmh_scythe/__about__.py"
 
 [tool.hatch.envs.default]
-features = [
-  "test",
-]
+features = ["dev", "test"]
+post-install-commands = ["pre-commit install"]
 [tool.hatch.envs.default.scripts]
+check = ["lint", "typecheck"]
+lint = "SKIP=mypy pre-commit run --all-files --color=always --show-diff-on-failure"
+typecheck = "pre-commit run --all-files --color=always --show-diff-on-failure mypy"
 test = "pytest {args:tests}"
 cov = "pytest --cov {args:src}"
-cov-report-markdown = "python -m coverage report --format=markdown > coverage.md"
-cov-summary-json = "python -m coverage json"
+cov-report-markdown = "python -m coverage report --format=markdown {args:>coverage.md}"
 cov-total = """
-python -c "import json;print(json.load(open('coverage.json'))['totals']['percent_covered_display'])"
+  python -m coverage json --quiet
+  python -c "import json;print(json.load(open('coverage.json'))['totals']['percent_covered_display'])"
 """
 
-[tool.hatch.envs.lint]
-features = [ "lint"]
-[tool.hatch.envs.lint.scripts]
-style = "SKIP=mypy pre-commit run --all-files --color=always"
-typing = "pre-commit run --all-files --color=always mypy"
-all = [
-  "style",
-  "typing",
-]
-
 [tool.hatch.envs.docs]
 features = ["docs"]
+template = "docs"
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --strict --config-file=docs/mkdocs.yml"
 serve = "mkdocs serve --strict --config-file=docs/mkdocs.yml"
 deploy = "mkdocs gh-deploy --force --config-file=docs/mkdocs.yml"
 
 [tool.hatch.envs.release]
 features = ["release"]
+template = "release"
 [tool.hatch.envs.release.scripts]
 next-version = "semantic-release version --print"
 update-citation = """
   sed -i "s/^version: .*/version: $(semantic-release version --print)/" CITATION.cff
   sed -i "s/^date-released: .*/date-released: $(date "+%Y-%m-%d")/" CITATION.cff
   cat CITATION.cff
 """
 
 # ruff
 # Ref: https://docs.astral.sh/ruff/configuration/
 # ------------------------------------------------------------------------------
 
 [tool.ruff]
 line-length = 120
-src = ["src"]
-target-version = "py310"
+src = ["src", "tests"]
+
+[tool.ruff.format]
+# Ref: https://docs.astral.sh/ruff/settings/#format
+docstring-code-format = true
 
 [tool.ruff.lint]
 # Ref: https://docs.astral.sh/ruff/rules/
 extend-select = [
   "A",    # flake8-builtins
   "B",    # flake8-bugbear
   "C4",   # flake8-comprehensions
   "D",    # pydocstyle
-  "FURB", # refurb
   "I",    # isort
+  "G",    # flake8-logging-format
   "PERF", # perflint-perf
   "PGH",  # pygrep-hooks
   "PIE",  # flake8-pie
   "PL",   # pylint
   "PT",   # flake8-pytest-style
   "RUF",  # ruff
   "TCH",  # flake8-type-checking
@@ -160,34 +152,30 @@
 ignore = [
   "D105", # undocumented-magic-method
   "D107", # undocumented-public-init
 ]
 unfixable = [
   "F401", # unused-import
 ]
+isort.known-first-party = ["oaipmh_scythe"]
+pydocstyle.convention = "google"
 
 [tool.ruff.lint.per-file-ignores]
 "src/oaipmh_scythe/__about__.py" = [
   "D100", # undocumented-public-module
 ]
 "src/oaipmh_scythe/client.py" = [
   "PLR0913", # too-many-arguments
 ]
 "tests/*" = [
   "D100",     # undocumented-public-module
   "D103",     # undocumented-public-function
   "PLR2004",  # magic-value-comparison
 ]
 
-[tool.ruff.lint.isort]
-known-first-party = ["oaipmh_scythe"]
-
-[tool.ruff.lint.pydocstyle]
-convention = "google"
-
 # sp-repo-review
 # Ref: https://github.com/scientific-python/cookie/tree/main#list-of-checks
 # ------------------------------------------------------------------------------
 
 [tool.repo-review]
 ignore = [
   # Pre-commit
@@ -200,15 +188,15 @@
 ]
 
 # pytest
 # Ref: https://docs.pytest.org/en/stable/customize.html
 # ------------------------------------------------------------------------------
 
 [tool.pytest.ini_options]
-minversion = "7.0"
+minversion = "8.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 filterwarnings = ["error"]
 log_cli_level = "INFO"
 xfail_strict = true
 testpaths = "tests"
 
 # coverage.py
@@ -237,16 +225,17 @@
 # Ref: https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 # ------------------------------------------------------------------------------
 
 [tool.mypy]
 python_version = "3.10"
 pretty = true
 show_column_numbers = true
-show_error_codes = true
 show_error_context = true
+enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
+warn_unreachable = true
 
 # licensecheck
 # Ref: https://github.com/FHPythonUtils/LicenseCheck/#example-1-pyprojecttoml
 # ------------------------------------------------------------------------------
 
 [tool.licensecheck]
 using = "PEP631"
@@ -264,20 +253,16 @@
 version_variables = [
   "src/oaipmh_scythe/__about__.py:__version__",
 ]
 build_command = """
 python -m pip install build
 python -m build
 """
-
-[tool.semantic_release.changelog]
-template_dir = ".github/templates"
-
-[tool.semantic_release.changelog.environment]
-keep_trailing_newline = true
+changelog.template_dir = ".github/templates"
+changelog.environment.keep_trailing_newline = true
 
 # typos
 # Ref: https://github.com/crate-ci/typos/blob/master/docs/reference.md
 # ------------------------------------------------------------------------------
 
 [tool.typos]
 # add "spellchecker:disable-line" to ignore specific lines
```


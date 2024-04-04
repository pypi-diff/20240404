# Comparing `tmp/git_changelog-2.5.1.tar.gz` & `tmp/git_changelog-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_changelog-2.5.1.tar", last modified: Mon Apr  1 22:55:04 2024, max compression
+gzip compressed data, was "git_changelog-2.5.2.tar", last modified: Thu Apr  4 15:35:49 2024, max compression
```

## Comparing `git_changelog-2.5.1.tar` & `git_changelog-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      754 2024-03-31 19:47:09.968170 git_changelog-2.5.1/LICENSE
--rw-r--r--   0        0        0     3702 2024-03-31 19:47:09.968170 git_changelog-2.5.1/README.md
--rw-r--r--   0        0        0     1853 2024-04-01 22:55:04.151203 git_changelog-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      278 2024-03-31 19:47:09.968170 git_changelog-2.5.1/src/git_changelog/__init__.py
--rw-r--r--   0        0        0      387 2024-03-31 19:47:09.968170 git_changelog-2.5.1/src/git_changelog/__main__.py
--rw-r--r--   0        0        0    20209 2024-04-01 11:49:17.580819 git_changelog-2.5.1/src/git_changelog/build.py
--rw-r--r--   0        0        0    27496 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/cli.py
--rw-r--r--   0        0        0    14008 2024-04-01 11:45:41.037014 git_changelog-2.5.1/src/git_changelog/commit.py
--rw-r--r--   0        0        0     2840 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/debug.py
--rw-r--r--   0        0        0    13417 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/providers.py
--rw-r--r--   0        0        0        0 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/py.typed
--rw-r--r--   0        0        0     1122 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/templates/__init__.py
--rw-r--r--   0        0        0     1588 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/templates/angular.md.jinja
--rw-r--r--   0        0        0     2213 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/templates/keepachangelog.md.jinja
--rw-r--r--   0        0        0    27786 2024-03-31 19:47:09.971503 git_changelog-2.5.1/src/git_changelog/versioning.py
--rw-r--r--   0        0        0      166 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/__init__.py
--rw-r--r--   0        0        0      850 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/conftest.py
--rw-r--r--   0        0        0     3243 2024-03-31 19:52:40.640087 git_changelog-2.5.1/tests/helpers.py
--rw-r--r--   0        0        0     2361 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_angular_style.py
--rw-r--r--   0        0        0     2308 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_basic_style.py
--rw-r--r--   0        0        0     8744 2024-04-01 11:46:08.991345 git_changelog-2.5.1/tests/test_build.py
--rw-r--r--   0        0        0     8550 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_cli.py
--rw-r--r--   0        0        0     1079 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_commit.py
--rw-r--r--   0        0        0     5483 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_conventional_commit_style.py
--rw-r--r--   0        0        0     6546 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_end_to_end.py
--rw-r--r--   0        0        0     1505 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_providers.py
--rw-r--r--   0        0        0      897 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_release_notes.py
--rw-r--r--   0        0        0    11631 2024-03-31 19:47:09.971503 git_changelog-2.5.1/tests/test_versioning.py
--rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 git_changelog-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-31 19:47:09.968170 git_changelog-2.5.2/LICENSE
+-rw-r--r--   0        0        0     3702 2024-03-31 19:47:09.968170 git_changelog-2.5.2/README.md
+-rw-r--r--   0        0        0     1853 2024-04-04 15:35:49.424775 git_changelog-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      278 2024-03-31 19:47:09.968170 git_changelog-2.5.2/src/git_changelog/__init__.py
+-rw-r--r--   0        0        0      387 2024-03-31 19:47:09.968170 git_changelog-2.5.2/src/git_changelog/__main__.py
+-rw-r--r--   0        0        0    19760 2024-04-04 15:32:39.799052 git_changelog-2.5.2/src/git_changelog/build.py
+-rw-r--r--   0        0        0    27496 2024-04-04 15:32:29.639101 git_changelog-2.5.2/src/git_changelog/cli.py
+-rw-r--r--   0        0        0    14008 2024-04-01 11:45:41.037014 git_changelog-2.5.2/src/git_changelog/commit.py
+-rw-r--r--   0        0        0     2840 2024-03-31 19:47:09.971503 git_changelog-2.5.2/src/git_changelog/debug.py
+-rw-r--r--   0        0        0    13417 2024-03-31 19:47:09.971503 git_changelog-2.5.2/src/git_changelog/providers.py
+-rw-r--r--   0        0        0        0 2024-03-31 19:47:09.971503 git_changelog-2.5.2/src/git_changelog/py.typed
+-rw-r--r--   0        0        0     1122 2024-03-31 19:47:09.971503 git_changelog-2.5.2/src/git_changelog/templates/__init__.py
+-rw-r--r--   0        0        0     1588 2024-03-31 19:47:09.971503 git_changelog-2.5.2/src/git_changelog/templates/angular.md.jinja
+-rw-r--r--   0        0        0     2213 2024-04-04 15:32:29.639101 git_changelog-2.5.2/src/git_changelog/templates/keepachangelog.md.jinja
+-rw-r--r--   0        0        0    27860 2024-04-04 15:32:39.799052 git_changelog-2.5.2/src/git_changelog/versioning.py
+-rw-r--r--   0        0        0      166 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      850 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     3243 2024-03-31 19:52:40.640087 git_changelog-2.5.2/tests/helpers.py
+-rw-r--r--   0        0        0     2361 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_angular_style.py
+-rw-r--r--   0        0        0     2308 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_basic_style.py
+-rw-r--r--   0        0        0     9246 2024-04-04 15:32:39.799052 git_changelog-2.5.2/tests/test_build.py
+-rw-r--r--   0        0        0     8550 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1079 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_commit.py
+-rw-r--r--   0        0        0     5483 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_conventional_commit_style.py
+-rw-r--r--   0        0        0     6546 2024-04-04 15:32:29.639101 git_changelog-2.5.2/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     1505 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_providers.py
+-rw-r--r--   0        0        0      897 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_release_notes.py
+-rw-r--r--   0        0        0    11631 2024-03-31 19:47:09.971503 git_changelog-2.5.2/tests/test_versioning.py
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 git_changelog-2.5.2/PKG-INFO
```

### Comparing `git_changelog-2.5.1/LICENSE` & `git_changelog-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/README.md` & `git_changelog-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/pyproject.toml` & `git_changelog-2.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 dependencies = [
     "appdirs>=1.4",
     "Jinja2>=2.10",
     "packaging>=24.0",
     "semver>=2.13",
     "tomli>=2.0; python_version < '3.11'",
 ]
-version = "2.5.1"
+version = "2.5.2"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/git-changelog"
 Documentation = "https://pawamoy.github.io/git-changelog"
```

### Comparing `git_changelog-2.5.1/src/git_changelog/build.py` & `git_changelog-2.5.2/src/git_changelog/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,17 +291,14 @@
                 stacklevel=1,
             )
             if bump is None:
                 bump = "auto"
         if bump:
             self._bump(bump)
 
-        # fix a single, initial version to the user specified version or 0.1.0 if none is specified
-        self._fix_single_version(bump)
-
     def run_git(self, *args: str) -> str:
         """Run a git command in the chosen repository.
 
         Arguments:
             *args: Arguments passed to the git command.
 
         Returns:
@@ -476,16 +473,19 @@
                 version.compare_url = self.provider.get_compare_url(
                     base=previous_version,
                     target=version.tag or "HEAD",
                 )
 
     def _bump(self, version: str) -> None:
         last_version = self.versions_list[0]
-        if not last_version.tag and last_version.previous_version:
-            last_tag = last_version.previous_version.tag
+        if not last_version.tag:
+            if last_version.previous_version:
+                last_tag = last_version.previous_version.tag
+            else:
+                last_tag = self.version_bumper.initial
             version, *plus = version.split("+")
             if version == "auto":
                 # guess the next version number based on last version and recent commits
                 version = "patch"
                 for commit in last_version.commits:
                     if commit.convention["is_major"]:
                         version = "major"
@@ -503,18 +503,12 @@
                 except ValueError as error:
                     raise ValueError(f"{error}; typo in bumping strategy? Check the CLI help and our docs") from error
                 last_version.planned_tag = version
             # update URLs
             if self.provider:
                 last_version.url = self.provider.get_tag_url(tag=last_version.planned_tag)
                 last_version.compare_url = self.provider.get_compare_url(
-                    base=last_version.previous_version.tag,
+                    base=last_version.previous_version.tag
+                    if last_version.previous_version
+                    else last_version.commits[-1].hash,
                     target=last_version.planned_tag,
                 )
-
-    def _fix_single_version(self, version: str | None) -> None:
-        last_version = self.versions_list[0]
-        if len(self.versions_list) == 1 and last_version.planned_tag is None and not last_version.tag:
-            planned_tag = version if version and version not in {"auto", "major", "minor", "patch"} else "0.1.0"
-            last_version.tag = planned_tag
-            last_version.url += planned_tag
-            last_version.compare_url = last_version.compare_url.replace("HEAD", planned_tag)
```

### Comparing `git_changelog-2.5.1/src/git_changelog/cli.py` & `git_changelog-2.5.2/src/git_changelog/cli.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/commit.py` & `git_changelog-2.5.2/src/git_changelog/commit.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/debug.py` & `git_changelog-2.5.2/src/git_changelog/debug.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/providers.py` & `git_changelog-2.5.2/src/git_changelog/providers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/templates/__init__.py` & `git_changelog-2.5.2/src/git_changelog/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/templates/angular.md.jinja` & `git_changelog-2.5.2/src/git_changelog/templates/angular.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/templates/keepachangelog.md.jinja` & `git_changelog-2.5.2/src/git_changelog/templates/keepachangelog.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/src/git_changelog/versioning.py` & `git_changelog-2.5.2/src/git_changelog/versioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,14 +641,16 @@
     version, prefix = version_prefix(version)
     return PEP440Version(version), prefix
 
 
 class VersionBumper:
     """Base class for version bumpers."""
 
+    initial: str
+
     def __init__(self, strategies: tuple[str, ...]) -> None:
         """Initialize the bumper.
 
         Parameters:
             strategies: The supported bumping strategies.
         """
         self.strategies = strategies
@@ -666,14 +668,16 @@
         """
         raise NotImplementedError
 
 
 class PEP440Bumper(VersionBumper):
     """PEP 440 version bumper."""
 
+    initial: str = "0.0.0"
+
     def __call__(  # type: ignore[override]
         self,
         version: str,
         strategy: PEP440Strategy = "micro",
         *,
         zerover: bool = False,
         trim: bool = False,
@@ -740,14 +744,16 @@
         # Return new version with preserved prefix.
         return prefix + str(pep440_version)
 
 
 class SemVerBumper(VersionBumper):
     """SemVer version bumper."""
 
+    initial: str = "0.0.0"
+
     def __call__(  # type: ignore[override]
         self,
         version: str,
         strategy: SemVerStrategy = "patch",
         *,
         zerover: bool = True,
     ) -> str:
```

### Comparing `git_changelog-2.5.1/tests/conftest.py` & `git_changelog-2.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/helpers.py` & `git_changelog-2.5.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_angular_style.py` & `git_changelog-2.5.2/tests/test_angular_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_basic_style.py` & `git_changelog-2.5.2/tests/test_basic_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_build.py` & `git_changelog-2.5.2/tests/test_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 """Tests for the `build` module."""
 
 from __future__ import annotations
 
 from time import sleep
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import pytest
 
 from git_changelog import Changelog
 from git_changelog.commit import AngularConvention
 
 if TYPE_CHECKING:
     from git_changelog.build import Version
     from tests.helpers import GitRepo
 
 
 @pytest.mark.parametrize(
-    ("bump", "expected"),
-    [("auto", "0.1.0"), ("major", "0.1.0"), ("minor", "0.1.0"), ("1.1.1", "1.1.1")],
+    ("versioning", "bump", "expected"),
+    [
+        ("semver", "auto", "0.0.1"),  # chore commit
+        ("semver", "major", "1.0.0"),
+        ("semver", "minor", "0.1.0"),
+        ("semver", "patch", "0.0.1"),
+        ("semver", "1.1.1", "1.1.1"),
+        ("pep440", "auto", "0.0.1"),  # chore commit
+        ("pep440", "major", "1.0.0"),
+        ("pep440", "minor+dev", "0.1.0.dev0"),
+        ("pep440", "micro+alpha+dev", "0.0.1a0.dev0"),
+        ("pep440", "1.1.1", "1.1.1"),
+    ],
 )
-def test_bump_with_semver_on_new_repo(repo: GitRepo, bump: str, expected: str) -> None:
-    """Bump to user specified version (SemVer) on new git repo.
+def test_bump_with_semver_on_new_repo(
+    repo: GitRepo,
+    versioning: Literal["pep440", "semver"],
+    bump: str,
+    expected: str,
+) -> None:
+    """Bump to user specified version on new Git repo.
 
     Parameters:
         repo: GitRepo to a temporary repository.
         bump: The bump parameter value.
         expected: Expected version for the new changelog entry.
     """
-    changelog = Changelog(repo.path, convention=AngularConvention, bump=bump)
+    changelog = Changelog(repo.path, convention=AngularConvention, bump=bump, versioning=versioning, zerover=False)
     assert len(changelog.versions_list) == 1
-    assert changelog.versions_list[0].tag == expected
+    assert changelog.versions_list[0].planned_tag == expected
 
 
 @pytest.mark.parametrize("bump", ["auto", "major", "minor", "2.0.0"])
 def test_no_bump_on_first_tag(repo: GitRepo, bump: str) -> None:
     """Ignore bump on new git repo without unreleased commits.
 
     Parameters:
@@ -185,15 +201,15 @@
 
 def _assert_version(
     version: Version,
     expected_tag: str,
     expected_prev_tag: str | None,
     expected_commits: list[str],
 ) -> None:
-    assert version.tag == expected_tag
+    assert expected_tag in (version.tag, version.planned_tag)
     if expected_prev_tag:
         assert version.previous_version is not None, f"Expected previous version '{expected_prev_tag}', but was None"
         assert version.previous_version.tag == expected_prev_tag
     else:
         assert version.previous_version is None
     hashes = [commit.hash for commit in version.commits]
     assert hashes == expected_commits
@@ -248,15 +264,15 @@
 
     changelog = Changelog(repo.path, convention=AngularConvention)
 
     assert len(changelog.versions_list) == 1
     version = changelog.versions_list[0]
     _assert_version(
         version,
-        expected_tag="0.1.0",
+        expected_tag="",
         expected_prev_tag=None,
         expected_commits=[commit_e, commit_c, commit_d, commit_a, commit_b],
     )
 
 
 def test_build_changelog_with_pep440_versions(repo: GitRepo) -> None:
     """Test parsing and grouping commits to PEP440 versions.
```

### Comparing `git_changelog-2.5.1/tests/test_cli.py` & `git_changelog-2.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_commit.py` & `git_changelog-2.5.2/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_conventional_commit_style.py` & `git_changelog-2.5.2/tests/test_conventional_commit_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_end_to_end.py` & `git_changelog-2.5.2/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_providers.py` & `git_changelog-2.5.2/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_release_notes.py` & `git_changelog-2.5.2/tests/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/tests/test_versioning.py` & `git_changelog-2.5.2/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.5.1/PKG-INFO` & `git_changelog-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-changelog
-Version: 2.5.1
+Version: 2.5.2
 Summary: Automatic Changelog generator using Jinja2 templates.
 Keywords: git changelog changelog-generator commit-style commit-convention
 Author-Email: Timothée Mazzucotelli <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```


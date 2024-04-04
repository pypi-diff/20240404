# Comparing `tmp/sitreps_client-1.1.1-py2.py3-none-any.whl.zip` & `tmp/sitreps_client-1.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21305 bytes, number of entries: 18
+Zip file size: 21485 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 sitreps_client/__init__.py
--rw-r--r--  2.0 unx     5495 b- defN 20-Feb-02 00:00 sitreps_client/cloc.py
--rw-r--r--  2.0 unx     4921 b- defN 20-Feb-02 00:00 sitreps_client/code_coverage.py
+-rw-r--r--  2.0 unx     5496 b- defN 20-Feb-02 00:00 sitreps_client/cloc.py
+-rw-r--r--  2.0 unx     4922 b- defN 20-Feb-02 00:00 sitreps_client/code_coverage.py
 -rw-r--r--  2.0 unx      425 b- defN 20-Feb-02 00:00 sitreps_client/exceptions.py
--rw-r--r--  2.0 unx     3719 b- defN 20-Feb-02 00:00 sitreps_client/issues.py
+-rw-r--r--  2.0 unx     3720 b- defN 20-Feb-02 00:00 sitreps_client/issues.py
 -rw-r--r--  2.0 unx     7634 b- defN 20-Feb-02 00:00 sitreps_client/project.py
 -rw-r--r--  2.0 unx     3233 b- defN 20-Feb-02 00:00 sitreps_client/sonarqube.py
--rw-r--r--  2.0 unx    17351 b- defN 20-Feb-02 00:00 sitreps_client/unit_tests.py
+-rw-r--r--  2.0 unx    17626 b- defN 20-Feb-02 00:00 sitreps_client/unit_tests.py
 -rw-r--r--  2.0 unx     2632 b- defN 20-Feb-02 00:00 sitreps_client/conf/config.py
 -rw-r--r--  2.0 unx     1712 b- defN 20-Feb-02 00:00 sitreps_client/conf/default_settings.yaml
--rw-r--r--  2.0 unx     1525 b- defN 20-Feb-02 00:00 sitreps_client/utils/ci_downloader.py
+-rw-r--r--  2.0 unx     1526 b- defN 20-Feb-02 00:00 sitreps_client/utils/ci_downloader.py
 -rw-r--r--  2.0 unx     2576 b- defN 20-Feb-02 00:00 sitreps_client/utils/helpers.py
 -rw-r--r--  2.0 unx      162 b- defN 20-Feb-02 00:00 sitreps_client/utils/path.py
 -rw-r--r--  2.0 unx     3531 b- defN 20-Feb-02 00:00 sitreps_client/utils/repository.py
-?rw-r--r--  2.0 unx     1371 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1537 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/RECORD
-18 files, 59000 bytes uncompressed, 18775 bytes compressed:  68.2%
+?rw-r--r--  2.0 unx     1345 b- defN 20-Feb-02 00:00 sitreps_client-1.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sitreps_client-1.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 sitreps_client-1.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1537 b- defN 20-Feb-02 00:00 sitreps_client-1.1.2.dist-info/RECORD
+18 files, 59253 bytes uncompressed, 18955 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: sitreps_client/utils/path.py
 Comment: 
 
 Filename: sitreps_client/utils/repository.py
 Comment: 
 
-Filename: sitreps_client-1.1.1.dist-info/METADATA
+Filename: sitreps_client-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sitreps_client-1.1.1.dist-info/WHEEL
+Filename: sitreps_client-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sitreps_client-1.1.1.dist-info/licenses/LICENSE
+Filename: sitreps_client-1.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sitreps_client-1.1.1.dist-info/RECORD
+Filename: sitreps_client-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sitreps_client/cloc.py

```diff
@@ -1,8 +1,9 @@
 """Count cloc for project and tests repositories."""
+
 import io
 import logging
 from contextlib import redirect_stdout
 from pathlib import Path
 from typing import Dict
 from typing import Optional
```

## sitreps_client/code_coverage.py

```diff
@@ -1,8 +1,9 @@
 """Code coverage for repositories."""
+
 import logging
 import re
 from typing import Optional
 
 import requests
 
 from sitreps_client.exceptions import CodeCoverageError
```

## sitreps_client/issues.py

```diff
@@ -1,8 +1,9 @@
 """Jira/Bugzilla issues."""
+
 import logging
 from typing import Optional
 from typing import Union
 
 from cached_property import cached_property
 from jira import JIRA
```

## sitreps_client/unit_tests.py

```diff
@@ -1,30 +1,30 @@
 """Numbers of unit tests for repositories."""
+
 import logging
 import re
 from pathlib import Path
-from typing import Generator
 from typing import Optional
 from uuid import uuid4
 from zipfile import ZipFile
 
 import requests
-from cached_property import cached_property
-from PyTravisCI import TravisCI
-from PyTravisCI.defaults.access_points import OPEN
-from PyTravisCI.defaults.access_points import PRIVATE
-from PyTravisCI.exceptions import TravisCIError
 from requests.auth import AuthBase
 
 from sitreps_client.exceptions import SitrepsError
 from sitreps_client.utils.ci_downloader import CIDownloader
 from sitreps_client.utils.ci_downloader import JenkinsDownloader
 from sitreps_client.utils.helpers import escape_ansi
 from sitreps_client.utils.helpers import wait_for
 
+# from PyTravisCI import TravisCI
+# from PyTravisCI.defaults.access_points import OPEN
+# from PyTravisCI.defaults.access_points import PRIVATE
+# from PyTravisCI.exceptions import TravisCIError
+
 LOGGER = logging.getLogger(__name__)
 
 KNOWN_TESTING_TOOLS = (
     "gotest",
     "pytest",
     "pyunittest",
     "npm",
@@ -327,90 +327,94 @@
                 return num_of_tests
         return 0
 
     def __repr__(self):
         return f"<GHActionUnitTests(repo_slug={self.repo_slug})>"
 
 
-class TravisUnitTests(BaseUnitTests):
-    """Number of unit tests from Travis."""
-
-    def __init__(
-        self,
-        repo_slug: str,
-        access_token: str = None,
-        branch: str = "master",
-        is_private: bool = True,
-        test_tool: str = None,
-    ):
-        self.repo_slug = repo_slug
-        self.access_token = access_token
-        self.branch = branch
-        self.is_private = is_private
-        self.test_tool = test_tool
-
-    @cached_property
-    def client(self):
-        """Travis client.
+# Travis not supported by app-sre and PyTravisCI not properly maintain.
 
-        Returns: TravisCI object
-        """
-        if self.access_token:
-            access_point = PRIVATE if self.is_private else OPEN
-            return TravisCI(access_token=self.access_token, access_point=access_point)
-        return TravisCI()
-
-    def get_logs(self) -> Generator[str, None, None]:
-        try:
-            repo = self.client.get_repository(repository_id_or_slug=self.repo_slug)
-        except Exception as e:
-            msg = f"[Travis-{self.repo_slug}]: is it using private travis? is repo used travis?"
-            LOGGER.warning(msg)
-            raise SitrepsError(f"{msg}, Error:{e}")
-
-        builds = repo.get_builds(params={"branch.name": self.branch, "state": "passed", "limit": 1})
-
-        if not builds:
-            raise SitrepsError(
-                f"[Travis-{self.repo_slug}]: Build for branch '{self.branch}' with passed status "
-                f"not found."
-            )
-        build = builds[0]  # Select first build i.e. latest one.
-        LOGGER.info(f"[Travis-{self.repo_slug}]: Latest build: {build.id}")
-        jobs = build.get_jobs().jobs
-        test_jobs = [job for job in jobs if job.stage and "test" in job.stage.name.lower()]
-        if test_jobs:
-            LOGGER.info(f"[Travis-{self.repo_slug}]: Test jobs detected. Limiting scan.")
-            jobs = test_jobs
-
-        for job in jobs:
-            try:
-                log = job.get_log()
-            except TravisCIError as e:
-                raise SitrepsError(f"[Travis-{self.repo_slug}]: {e}")
-            yield log.content
-
-    def get_num_of_tests(self) -> Optional[int]:
-        """Return number of unit tests."""
-        try:
-            log_generator = self.get_logs()
-        # pylint: disable=broad-except
-        except Exception as exc:
-            msg = f"[Travis-{self.repo_slug}]: {exc}"
-            LOGGER.error(msg)
-            return None
-
-        for ci_log in log_generator:
-            num_of_tests = self._get_tests_count(ci_log, test_tool=self.test_tool)
-            if num_of_tests > 0:
-                return num_of_tests
-        return 0
-
-    def __repr__(self):
-        return f"<TravisUnitTests(repo_slug={self.repo_slug})>"
+# class TravisUnitTests(BaseUnitTests):
+#     """Number of unit tests from Travis."""
+#
+#     def __init__(
+#         self,
+#         repo_slug: str,
+#         access_token: str = None,
+#         branch: str = "master",
+#         is_private: bool = True,
+#         test_tool: str = None,
+#     ):
+#         self.repo_slug = repo_slug
+#         self.access_token = access_token
+#         self.branch = branch
+#         self.is_private = is_private
+#         self.test_tool = test_tool
+#
+#     @cached_property
+#     def client(self):
+#         """Travis client.
+#
+#         Returns: TravisCI object
+#         """
+#         if self.access_token:
+#             access_point = PRIVATE if self.is_private else OPEN
+#             return TravisCI(access_token=self.access_token, access_point=access_point)
+#         return TravisCI()
+#
+#     def get_logs(self) -> Generator[str, None, None]:
+#         try:
+#             repo = self.client.get_repository(repository_id_or_slug=self.repo_slug)
+#         except Exception as e:
+#             msg = f"[Travis-{self.repo_slug}]: is it using private travis? is repo used travis?"
+#             LOGGER.warning(msg)
+#             raise SitrepsError(f"{msg}, Error:{e}")
+#
+#         builds = repo.get_builds(
+#         params={"branch.name": self.branch, "state": "passed", "limit": 1}
+#         )
+#
+#         if not builds:
+#             raise SitrepsError(
+#                 f"[Travis-{self.repo_slug}]: Build for branch '{self.branch}' with passed status "
+#                 f"not found."
+#             )
+#         build = builds[0]  # Select first build i.e. latest one.
+#         LOGGER.info(f"[Travis-{self.repo_slug}]: Latest build: {build.id}")
+#         jobs = build.get_jobs().jobs
+#         test_jobs = [job for job in jobs if job.stage and "test" in job.stage.name.lower()]
+#         if test_jobs:
+#             LOGGER.info(f"[Travis-{self.repo_slug}]: Test jobs detected. Limiting scan.")
+#             jobs = test_jobs
+#
+#         for job in jobs:
+#             try:
+#                 log = job.get_log()
+#             except TravisCIError as e:
+#                 raise SitrepsError(f"[Travis-{self.repo_slug}]: {e}")
+#             yield log.content
+#
+#     def get_num_of_tests(self) -> Optional[int]:
+#         """Return number of unit tests."""
+#         try:
+#             log_generator = self.get_logs()
+#         # pylint: disable=broad-except
+#         except Exception as exc:
+#             msg = f"[Travis-{self.repo_slug}]: {exc}"
+#             LOGGER.error(msg)
+#             return None
+#
+#         for ci_log in log_generator:
+#             num_of_tests = self._get_tests_count(ci_log, test_tool=self.test_tool)
+#             if num_of_tests > 0:
+#                 return num_of_tests
+#         return 0
+#
+#     def __repr__(self):
+#         return f"<TravisUnitTests(repo_slug={self.repo_slug})>"
 
 
 class CIUnitTests(BaseUnitTests):
     """Number of unit tests from CI."""
 
     def __init__(self, url: str, ci_downloader: CIDownloader, test_tool: str = None):
         self.url = url
@@ -432,21 +436,23 @@
         return f"<CIUnitTests(url={self.url})>"
 
 
 def get_unit_tests(travis=None, gh_action=None, jenkins=None):
     unit_tests = {}
 
     if travis:
-        LOGGER.info(f"[UnitTests-{travis.get('repo_slug')}]: Collecting with 'travis'.")
-        unit_tests["travis"] = TravisUnitTests(
-            repo_slug=travis.get("repo_slug"),
-            branch=travis.get("branch"),
-            access_token=travis.get("access_token"),
-            test_tool=travis.get("test_tool"),
-        )
+        LOGGER.error("Travis not supported by app-sre.")
+        return dict(travis=0)
+        # LOGGER.info(f"[UnitTests-{travis.get('repo_slug')}]: Collecting with 'travis'.")
+        # unit_tests["travis"] = TravisUnitTests(
+        #     repo_slug=travis.get("repo_slug"),
+        #     branch=travis.get("branch"),
+        #     access_token=travis.get("access_token"),
+        #     test_tool=travis.get("test_tool"),
+        # )
 
     if gh_action:
         LOGGER.info(f"[UnitTests-{gh_action.get('repo_slug')}]: Collecting with 'gh_actions'.")
         unit_tests["gh_action"] = GHActionUnitTests(
             repo_slug=gh_action.get("repo_slug"),
             branch=gh_action.get("branch"),
             github_token=gh_action.get("token"),
```

## sitreps_client/utils/ci_downloader.py

```diff
@@ -1,8 +1,9 @@
 """Downloader for files on CI (Jenkins, ...)."""
+
 import logging
 
 import requests
 
 from sitreps_client.exceptions import SitrepsError
 from sitreps_client.utils.helpers import wait_for
```

## Comparing `sitreps_client-1.1.1.dist-info/METADATA` & `sitreps_client-1.1.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sitreps-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: A client help to collect different metrics.
 Project-URL: Source, https://github.com/digitronik/sitreps-client
 Maintainer-email: Nikhil Dhandare <ndhandre@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,14 @@
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: cached-property
 Requires-Dist: jira
 Requires-Dist: pygount
 Requires-Dist: python-box
 Requires-Dist: python-dotenv
 Requires-Dist: python-sonarqube-api
-Requires-Dist: pytravisci
 Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: ipython; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
```

## Comparing `sitreps_client-1.1.1.dist-info/licenses/LICENSE` & `sitreps_client-1.1.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `sitreps_client-1.1.1.dist-info/RECORD` & `sitreps_client-1.1.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sitreps_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sitreps_client/cloc.py,sha256=iN_4lw6q7py3oKvsxIS45l__wGBtsVnAAOdvVPnmByU,5495
-sitreps_client/code_coverage.py,sha256=kB3I1rgBwZqvQffJs8E3JlipXZWx50G5bLfM_oyEJns,4921
+sitreps_client/cloc.py,sha256=bODn1_Wt-Fu_RyedPZuyg5-FYBWS54_a7sscAVHf_pQ,5496
+sitreps_client/code_coverage.py,sha256=eqsJkkbi0FzVmqG8qCP7wS66zoMK6-_MfaQvUrrq3UE,4922
 sitreps_client/exceptions.py,sha256=ey9fBW9t8sckaWM6vFeU1sxQpVj4ohJFgQg3vI6rR58,425
-sitreps_client/issues.py,sha256=S6k_n82QWpIN0der5kpHYqFrZhTpgqk3a08dVG1DKQI,3719
+sitreps_client/issues.py,sha256=VYBiuVV-jZWMyt2i1iP5uYUsAZw6isx4ceH5WxtNygQ,3720
 sitreps_client/project.py,sha256=5UupPEDBFNZFumRsZMD_JmTitY3BtPELHqSbzkC9J4Q,7634
 sitreps_client/sonarqube.py,sha256=-iJTdu6tBNlOdULyOStk0XwUOxTkNZzz5JOgASXt9h0,3233
-sitreps_client/unit_tests.py,sha256=bqf9v6xi9tq7D6WuzBjNiS5AC9jryR0FlqEA6C8OHvc,17351
+sitreps_client/unit_tests.py,sha256=DPoQ25kb6sqJ0sC-VaVYXRrvsw8iLt5J4_ojCbgD4vM,17626
 sitreps_client/conf/config.py,sha256=NatSvY0sxWKdM1gOKJTblwQ964MTkI1thXbdznNWCr0,2632
 sitreps_client/conf/default_settings.yaml,sha256=AlRHe5awZRANMFBhePYtIC75u1ClYz2jnt-Y-rW0onc,1712
-sitreps_client/utils/ci_downloader.py,sha256=atzPrA-coOLrDvCyq9Ot4tbFbsdEB8FnMt5BlTrQ-Js,1525
+sitreps_client/utils/ci_downloader.py,sha256=Bs6DhJA2bMeWqCHWYQY3EUAfZQ6U4BGjVKCY3XAjp5c,1526
 sitreps_client/utils/helpers.py,sha256=ayjxyyFFNI2tyKzsq1SlElyvsAZsZfstI10fqzfpyFk,2576
 sitreps_client/utils/path.py,sha256=eOwe26HwN_WYaw28Kae-ZYtHT5reb0l4nEfK5K6LVbk,162
 sitreps_client/utils/repository.py,sha256=E7XblcUkEN0X-WO0NOa9WAHxodqYpqGnG3NinQJ1H7Q,3531
-sitreps_client-1.1.1.dist-info/METADATA,sha256=115RDbrnhr1iPN_ZyKa940VQ9KoczXMtPLDZjZ4_QL4,1371
-sitreps_client-1.1.1.dist-info/WHEEL,sha256=BnTM96A0yHS39SE-waRX_LK6xllJtQJhpP4G4cCnPIA,105
-sitreps_client-1.1.1.dist-info/licenses/LICENSE,sha256=O5tfZlESkbOf5s8Fbq8KW3MHGZgX5XCS6FT2ZQuOUbI,1071
-sitreps_client-1.1.1.dist-info/RECORD,,
+sitreps_client-1.1.2.dist-info/METADATA,sha256=ev2Q4FBEPD57PxoOjOGVUW1mZ6PodghC0VLLTNhNodU,1345
+sitreps_client-1.1.2.dist-info/WHEEL,sha256=q6Ejfpj4HRnt7o1XWgEOo5g7W0PKmxxzhdMpcVNBe68,105
+sitreps_client-1.1.2.dist-info/licenses/LICENSE,sha256=O5tfZlESkbOf5s8Fbq8KW3MHGZgX5XCS6FT2ZQuOUbI,1071
+sitreps_client-1.1.2.dist-info/RECORD,,
```


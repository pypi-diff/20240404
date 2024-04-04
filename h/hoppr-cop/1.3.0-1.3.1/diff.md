# Comparing `tmp/hoppr_cop-1.3.0.tar.gz` & `tmp/hoppr_cop-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.3.0.tar", max compression
+gzip compressed data, was "hoppr_cop-1.3.1.tar", max compression
```

## Comparing `hoppr_cop-1.3.0.tar` & `hoppr_cop-1.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1084 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/LICENSE.md
--rw-r--r--   0        0        0       94 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0    14286 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/combined/analysis_assessment.py
--rw-r--r--   0        0        0     7692 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     5996 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/combined/py.typed
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0    11453 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1974 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/gemnasium/models.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/gemnasium/py.typed
--rwxr-xr-x   0        0        0      113 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     8912 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     8363 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/grype/models.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/grype/py.typed
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/hoppr_plugin/__init__.py
--rw-r--r--   0        0        0     9128 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/hoppr_plugin/py.typed
--rw-r--r--   0        0        0      478 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1048 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9278 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    10293 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     2997 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     6179 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/ossindex/py.typed
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/py.typed
--rw-r--r--   0        0        0    14093 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/gitlab/__init__.py
--rw-r--r--   0        0        0    21389 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/gitlab/models.py
--rw-r--r--   0        0        0     1703 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/models.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/py.typed
--rw-r--r--   0        0        0    13776 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/assets/vulnerabilities.css
--rw-r--r--   0        0        0    62168 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/package-lock.json
--rw-r--r--   0        0        0       56 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/package.json
--rw-r--r--   0        0        0      135 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/tailwind.config.js
--rw-r--r--   0        0        0     3241 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/vulnerabilities.html
--rw-r--r--   0        0        0       58 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/vulnerability.css
--rw-r--r--   0        0        0    10820 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/reporting/templates/vulnerability_details.html
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/trivy/py.typed
--rw-r--r--   0        0        0     7703 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0     7459 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/utils.py
--rw-r--r--   0        0        0     3423 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/vulnerability_combiner.py
--rw-r--r--   0        0        0     5971 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/hopprcop/vulnerability_scanner.py
--rw-r--r--   0        0        0     6311 2024-02-05 18:06:08.000000 hoppr_cop-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/LICENSE.md
+-rw-r--r--   0        0        0       94 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0    14286 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/combined/analysis_assessment.py
+-rw-r--r--   0        0        0     7692 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     5996 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/combined/py.typed
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0    11453 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1974 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/gemnasium/models.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/gemnasium/py.typed
+-rwxr-xr-x   0        0        0      113 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     8912 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     8363 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/grype/models.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/grype/py.typed
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/hoppr_plugin/__init__.py
+-rw-r--r--   0        0        0     9128 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/hoppr_plugin/py.typed
+-rw-r--r--   0        0        0      478 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1048 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9278 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    10293 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     2997 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     6179 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/ossindex/py.typed
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/py.typed
+-rw-r--r--   0        0        0    14603 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/gitlab/__init__.py
+-rw-r--r--   0        0        0    21389 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/gitlab/models.py
+-rw-r--r--   0        0        0     1703 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/models.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/py.typed
+-rw-r--r--   0        0        0    13776 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/assets/vulnerabilities.css
+-rw-r--r--   0        0        0    62168 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/package-lock.json
+-rw-r--r--   0        0        0       56 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/package.json
+-rw-r--r--   0        0        0      135 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/tailwind.config.js
+-rw-r--r--   0        0        0     3241 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/vulnerabilities.html
+-rw-r--r--   0        0        0       58 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/vulnerability.css
+-rw-r--r--   0        0        0    10820 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/reporting/templates/vulnerability_details.html
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/trivy/py.typed
+-rw-r--r--   0        0        0     7703 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0     7459 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/utils.py
+-rw-r--r--   0        0        0     3423 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/vulnerability_combiner.py
+-rw-r--r--   0        0        0     5971 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/hopprcop/vulnerability_scanner.py
+-rw-r--r--   0        0        0     6311 2024-02-13 18:21:00.000000 hoppr_cop-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.3.1/PKG-INFO
```

### Comparing `hoppr_cop-1.3.0/LICENSE.md` & `hoppr_cop-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/combined/analysis_assessment.py` & `hoppr_cop-1.3.1/hopprcop/combined/analysis_assessment.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/combined/cli.py` & `hoppr_cop-1.3.1/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.3.1/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.3.1/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/gemnasium/models.py` & `hoppr_cop-1.3.1/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.3.1/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/grype/models.py` & `hoppr_cop-1.3.1/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.3.1/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.3.1/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/__init__.py` & `hoppr_cop-1.3.1/hopprcop/reporting/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from rich.box import Box
 from rich.table import Table
 
 import hopprcop
 
 from hopprcop.reporting.gitlab.models import (
     Analyzer,
+    CvssVectors,
     CvssVectors3x,
     Dependency,
     DependencyFile,
     Identifier,
     Link,
     Location,
     Package,
@@ -312,36 +313,46 @@
         elif "CVSSv3" in methods:
             preferred_method = "CVSSv3"
         elif "CVSSv2" in methods:
             preferred_method = "CVSSv2"
 
         return next((rating for rating in ratings if str(rating.method) == preferred_method), default_rating)
 
+    def _get_cvss_vectors(self, ratings: list[cdx.Rating] | None) -> list[CvssVectors3x | CvssVectors]:
+        result: list[CvssVectors3x | CvssVectors] = []
+        for rating in ratings or []:
+            match rating.method:
+                case "CVSSv31" | "CVSSv3":
+                    result.append(
+                        CvssVectors3x(vendor=rating.source.name if rating.source else "unknown", vector=rating.vector)
+                    )
+                case "CVSSv2":
+                    result.append(
+                        CvssVectors(vendor=rating.source.name if rating.source else "unknown", vector=rating.vector)
+                    )
+
+        return result
+
     def _generate_gitlab_row(self, vuln: Vulnerability) -> GitlabVulnerability | None:
         """Generates a report row."""
         # Ensure `affects` and `tools` are non-empty lists
         if not (vuln.id and vuln.affects and vuln.tools):
             return None
 
         purl = PackageURL.from_string(vuln.affects[0].ref)
         severity = self._get_severity(vuln.ratings).title()
 
         return GitlabVulnerability(
             id=vuln.id,
             name=vuln.id,
             description=vuln.description,
-            severity=severity if severity != "none" else "Info",  # type: ignore[arg-type]
+            severity=severity if severity != "None" else "Info",  # type: ignore[arg-type]
             solution=vuln.recommendation or "",
             identifiers=[Identifier(type=vuln.id.split("-")[0].lower(), name=vuln.id, value=vuln.id)],
-            cvss_vectors=[
-                CvssVectors3x(vendor=rating.source.name if rating.source else "unknown", vector=rating.vector)
-                for rating in vuln.ratings or []
-                if rating.vector
-            ]
-            or None,
+            cvss_vectors=self._get_cvss_vectors(vuln.ratings) or None,
             links=[Link(url=advisory.url) for advisory in vuln.advisories or []],
             location=Location(
                 file="cyclonedx.bom",
                 dependency=Dependency(
                     package=Package(name=purl.name),
                     version=purl.version or "",
                 ),
```

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/gitlab/models.py` & `hoppr_cop-1.3.1/hopprcop/reporting/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/models.py` & `hoppr_cop-1.3.1/hopprcop/reporting/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/templates/assets/vulnerabilities.css` & `hoppr_cop-1.3.1/hopprcop/reporting/templates/assets/vulnerabilities.css`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/templates/package-lock.json` & `hoppr_cop-1.3.1/hopprcop/reporting/templates/package-lock.json`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/templates/vulnerabilities.html` & `hoppr_cop-1.3.1/hopprcop/reporting/templates/vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/reporting/templates/vulnerability_details.html` & `hoppr_cop-1.3.1/hopprcop/reporting/templates/vulnerability_details.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.3.1/hopprcop/trivy/trivy_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/utils.py` & `hoppr_cop-1.3.1/hopprcop/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/vulnerability_combiner.py` & `hoppr_cop-1.3.1/hopprcop/vulnerability_combiner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/hopprcop/vulnerability_scanner.py` & `hoppr_cop-1.3.1/hopprcop/vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.3.0/pyproject.toml` & `hoppr_cop-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.3.0"
+version = "1.3.1"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `hoppr_cop-1.3.0/PKG-INFO` & `hoppr_cop-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


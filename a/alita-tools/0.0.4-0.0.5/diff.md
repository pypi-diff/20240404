# Comparing `tmp/alita_tools-0.0.4.tar.gz` & `tmp/alita_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_tools-0.0.4.tar", last modified: Tue Apr  2 16:32:09 2024, max compression
+gzip compressed data, was "alita_tools-0.0.5.tar", last modified: Thu Apr  4 06:35:27 2024, max compression
```

## Comparing `alita_tools-0.0.4.tar` & `alita_tools-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/
--rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.4/LICENSE
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 16:32:09.520000 alita_tools-0.0.4/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.4/README.md
--rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-02 16:31:29.000000 alita_tools-0.0.4/pyproject.toml
--rwx------   0 arozumenko   (501) staff       (20)      138 2024-04-01 06:54:04.000000 alita_tools-0.0.4/requirements.txt
--rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-02 16:32:09.520000 alita_tools-0.0.4/setup.cfg
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.4/src/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/alita_tools/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.4/src/alita_tools/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/alita_tools/base/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.4/src/alita_tools/base/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.4/src/alita_tools/base/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/alita_tools/confluence/
--rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.4/src/alita_tools/confluence/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.4/src/alita_tools/confluence/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/alita_tools/github/
--rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.4/src/alita_tools/github/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    14849 2024-04-02 14:45:38.000000 alita_tools-0.0.4/src/alita_tools/github/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.4/src/alita_tools/github/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.490000 alita_tools-0.0.4/src/alita_tools/jira/
--rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.4/src/alita_tools/jira/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    11399 2024-04-02 16:05:32.000000 alita_tools-0.0.4/src/alita_tools/jira/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 16:32:09.480000 alita_tools-0.0.4/src/alita_tools.egg-info/
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 16:32:09.000000 alita_tools-0.0.4/src/alita_tools.egg-info/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      603 2024-04-02 16:32:09.000000 alita_tools-0.0.4/src/alita_tools.egg-info/SOURCES.txt
--rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-02 16:32:09.000000 alita_tools-0.0.4/src/alita_tools.egg-info/dependency_links.txt
--rwx------   0 arozumenko   (501) staff       (20)      139 2024-04-02 16:32:09.000000 alita_tools-0.0.4/src/alita_tools.egg-info/requires.txt
--rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-02 16:32:09.000000 alita_tools-0.0.4/src/alita_tools.egg-info/top_level.txt
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/
+-rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.5/LICENSE
+-rwx------   0 arozumenko   (501) staff       (20)      993 2024-04-04 06:35:27.780000 alita_tools-0.0.5/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.5/README.md
+-rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-03 08:00:02.000000 alita_tools-0.0.5/pyproject.toml
+-rwx------   0 arozumenko   (501) staff       (20)      148 2024-04-03 06:36:12.000000 alita_tools-0.0.5/requirements.txt
+-rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-04 06:35:27.790000 alita_tools-0.0.5/setup.cfg
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.5/src/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.5/src/alita_tools/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/base/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.5/src/alita_tools/base/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.5/src/alita_tools/base/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/confluence/
+-rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.5/src/alita_tools/confluence/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.5/src/alita_tools/confluence/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/datasources/
+-rwx------   0 arozumenko   (501) staff       (20)     1773 2024-04-03 08:43:31.000000 alita_tools-0.0.5/src/alita_tools/datasources/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/github/
+-rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.5/src/alita_tools/github/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    15406 2024-04-04 06:35:17.000000 alita_tools-0.0.5/src/alita_tools/github/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.5/src/alita_tools/github/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.740000 alita_tools-0.0.5/src/alita_tools/jira/
+-rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.5/src/alita_tools/jira/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    11399 2024-04-02 16:05:32.000000 alita_tools-0.0.5/src/alita_tools/jira/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools.egg-info/
+-rwx------   0 arozumenko   (501) staff       (20)      993 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      643 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/SOURCES.txt
+-rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/dependency_links.txt
+-rwx------   0 arozumenko   (501) staff       (20)      149 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/requires.txt
+-rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/top_level.txt
```

### Comparing `alita_tools-0.0.4/LICENSE` & `alita_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/PKG-INFO` & `alita_tools-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,10 +14,11 @@
 Requires-Dist: pydantic==1.10.9
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: pygithub==2.3.0
 Requires-Dist: atlassian_python_api==3.41.11
 Requires-Dist: markdownify==0.12.1
 Requires-Dist: pillow==10.2.0
+Requires-Dist: alita_sdk
 
 # application-tools
 Default set of tools available in ProjectAlita and CodeMie application interfaces
```

### Comparing `alita_tools-0.0.4/pyproject.toml` & `alita_tools-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_tools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Artem Rozumenko", email="support@projectalita.ai" },
   { name="Vadym Vlasenko", email="vadym_vlasenko@epam.com"}
 ]
 description = "Default set of tools and toolkits available within ProjectAlita and CodeMie applications."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `alita_tools-0.0.4/src/alita_tools/base/tool.py` & `alita_tools-0.0.5/src/alita_tools/base/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/confluence/__init__.py` & `alita_tools-0.0.5/src/alita_tools/confluence/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/confluence/api_wrapper.py` & `alita_tools-0.0.5/src/alita_tools/confluence/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/github/__init__.py` & `alita_tools-0.0.5/src/alita_tools/github/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/github/api_wrapper.py` & `alita_tools-0.0.5/src/alita_tools/github/api_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,21 +19,19 @@
     OVERVIEW_EXISTING_FILES_IN_MAIN,
     READ_FILE_PROMPT,
     SET_ACTIVE_BRANCH_PROMPT,
     UPDATE_FILE_PROMPT,
 )
 
 from langchain_community.agent_toolkits.github.toolkit import (
-    BranchName, CreatePR, DeleteFile,
-    GetIssue, GetPR, CommentOnIssue, BaseModel, Field
+    BranchName, CreatePR, GetIssue, GetPR, BaseModel, Field
 )
 
 from langchain_community.utilities.github import GitHubAPIWrapper
 
-
 CREATE_FILE_PROMPT = """Create new file in your github repository."""
 
 class SearchCode(BaseModel):
     """Schema for operations that require a search query as input."""
 
     query: str = Field(
         ...,
@@ -90,14 +88,33 @@
 
 class CreateFile(BaseModel):
     """Schema for operations that require a file path and content as input."""
 
     file_path: str = Field(..., description="Path of a file to be created.")
     file_contents: str = Field(..., description="Content of a file to be put into chat.")
 
+class CommentOnIssue(BaseModel):
+    """Schema for operations that require a comment as input."""
+
+    comment_query: str = Field(..., description="Follow the required formatting.")
+
+
+class DeleteFile(BaseModel):
+    """Schema for operations that require a file path as input."""
+
+    file_path: str = Field(
+        ...,
+        description=(
+            "The full file path of the file you would like to delete"
+            " where the path must NOT start with a slash, e.g."
+            " `some_dir/my_file.py`. Only input a string,"
+            " not the param name."
+        ),
+    )
+
 
 class AlitaGitHubAPIWrapper(GitHubAPIWrapper):
     github: Any  #: :meta private:
     github_repo_instance: Any  #: :meta private:
     github_repository: Optional[str] = None
     active_branch: Optional[str] = None
     github_base_branch: Optional[str] = None
```

### Comparing `alita_tools-0.0.4/src/alita_tools/github/tool.py` & `alita_tools-0.0.5/src/alita_tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/jira/__init__.py` & `alita_tools-0.0.5/src/alita_tools/jira/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools/jira/api_wrapper.py` & `alita_tools-0.0.5/src/alita_tools/jira/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.4/src/alita_tools.egg-info/PKG-INFO` & `alita_tools-0.0.5/src/alita_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,10 +14,11 @@
 Requires-Dist: pydantic==1.10.9
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: pygithub==2.3.0
 Requires-Dist: atlassian_python_api==3.41.11
 Requires-Dist: markdownify==0.12.1
 Requires-Dist: pillow==10.2.0
+Requires-Dist: alita_sdk
 
 # application-tools
 Default set of tools available in ProjectAlita and CodeMie application interfaces
```

### Comparing `alita_tools-0.0.4/src/alita_tools.egg-info/SOURCES.txt` & `alita_tools-0.0.5/src/alita_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 src/alita_tools.egg-info/dependency_links.txt
 src/alita_tools.egg-info/requires.txt
 src/alita_tools.egg-info/top_level.txt
 src/alita_tools/base/__init__.py
 src/alita_tools/base/tool.py
 src/alita_tools/confluence/__init__.py
 src/alita_tools/confluence/api_wrapper.py
+src/alita_tools/datasources/__init__.py
 src/alita_tools/github/__init__.py
 src/alita_tools/github/api_wrapper.py
 src/alita_tools/github/tool.py
 src/alita_tools/jira/__init__.py
 src/alita_tools/jira/api_wrapper.py
```


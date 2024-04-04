# Comparing `tmp/exposed_github_user_emails_scanner-1.0.6.tar.gz` & `tmp/exposed_github_user_emails_scanner-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Florian\Documents\gits\showExposedGitHubEmails\dist\.tmp-3k9diogz\exposed_github_user_emails_scanner-1.0.6.tar", last modified: Fri Feb 17 20:56:50 2023, max compression
+gzip compressed data, was "exposed_github_user_emails_scanner-1.0.7.tar", last modified: Thu Apr  4 14:28:46 2024, max compression
```

## Comparing `exposed_github_user_emails_scanner-1.0.6.tar` & `exposed_github_user_emails_scanner-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 20:56:50.158902 exposed_github_user_emails_scanner-1.0.6/
--rw-rw-rw-   0        0        0     1090 2021-03-16 14:52:29.000000 exposed_github_user_emails_scanner-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2411 2023-02-17 20:56:50.158389 exposed_github_user_emails_scanner-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2023-02-17 20:55:45.000000 exposed_github_user_emails_scanner-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 20:56:50.155684 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-02-17 20:56:50.000000 exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-17 20:56:50.157359 exposed_github_user_emails_scanner-1.0.6/github_exposed_email_crawler/
--rw-rw-rw-   0        0        0        0 2021-03-16 14:52:29.000000 exposed_github_user_emails_scanner-1.0.6/github_exposed_email_crawler/__init__.py
--rw-rw-rw-   0        0        0     7942 2023-02-17 20:54:33.000000 exposed_github_user_emails_scanner-1.0.6/github_exposed_email_crawler/script.py
--rw-rw-rw-   0        0        0       42 2023-02-17 20:56:50.159421 exposed_github_user_emails_scanner-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-02-17 20:54:33.000000 exposed_github_user_emails_scanner-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:28:46.506069 exposed_github_user_emails_scanner-1.0.7/
+-rw-rw-rw-   0        0        0     1090 2024-04-04 14:26:46.000000 exposed_github_user_emails_scanner-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2473 2024-04-04 14:28:46.505053 exposed_github_user_emails_scanner-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1873 2024-04-04 14:26:46.000000 exposed_github_user_emails_scanner-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 14:28:46.504046 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/
+-rw-rw-rw-   0        0        0     2473 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-04 14:28:46.000000 exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 14:28:46.503525 exposed_github_user_emails_scanner-1.0.7/github_exposed_email_crawler/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:26:46.000000 exposed_github_user_emails_scanner-1.0.7/github_exposed_email_crawler/__init__.py
+-rw-rw-rw-   0        0        0     7940 2024-04-04 14:26:46.000000 exposed_github_user_emails_scanner-1.0.7/github_exposed_email_crawler/script.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:28:46.506069 exposed_github_user_emails_scanner-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2024-04-04 14:27:24.000000 exposed_github_user_emails_scanner-1.0.7/setup.py
```

### Comparing `exposed_github_user_emails_scanner-1.0.6/LICENSE` & `exposed_github_user_emails_scanner-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exposed_github_user_emails_scanner-1.0.6/PKG-INFO` & `exposed_github_user_emails_scanner-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: exposed_github_user_emails_scanner
-Version: 1.0.6
+Version: 1.0.7
 Summary: A cli script to find exposed email addresses of one GitHub user in his or her public repositories.
 Home-page: https://github.com/wahlflo/showExposedGitHubEmails
 Author: Florian Wahl
 Author-email: florian.wahl.developer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cli-formatter>=1.1.0
+Requires-Dist: requests
 
 # showExposedGitHubEmails
 Is a crawler which lists all email addresses used in commits of a specific GitHub user using the GitHub API.
 
 It iterates through all public respositories owned by the user and all commits in each of these repositories.
```

### Comparing `exposed_github_user_emails_scanner-1.0.6/README.md` & `exposed_github_user_emails_scanner-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `exposed_github_user_emails_scanner-1.0.6/exposed_github_user_emails_scanner.egg-info/PKG-INFO` & `exposed_github_user_emails_scanner-1.0.7/exposed_github_user_emails_scanner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: exposed-github-user-emails-scanner
-Version: 1.0.6
+Name: exposed_github_user_emails_scanner
+Version: 1.0.7
 Summary: A cli script to find exposed email addresses of one GitHub user in his or her public repositories.
 Home-page: https://github.com/wahlflo/showExposedGitHubEmails
 Author: Florian Wahl
 Author-email: florian.wahl.developer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cli-formatter>=1.1.0
+Requires-Dist: requests
 
 # showExposedGitHubEmails
 Is a crawler which lists all email addresses used in commits of a specific GitHub user using the GitHub API.
 
 It iterates through all public respositories owned by the user and all commits in each of these repositories.
```

### Comparing `exposed_github_user_emails_scanner-1.0.6/github_exposed_email_crawler/script.py` & `exposed_github_user_emails_scanner-1.0.7/github_exposed_email_crawler/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         continue_loop = True
         url = '{}/repos/{}/{}/commits?per_page=100&page={}'.format(API_URL, username, repo_name, page_counter)
         result_dict = __api_call(url=url)
 
         if 'message' in result_dict:
             if result_dict['message'] == 'Git Repository is empty.':
                 info('Git repository is empty', verbosity_level=5)
-                continue
+                break 
 
             if 'API rate limit exceeded for ' in result_dict['message']:
                 warning('API rate limit exceeded - not all repos where fetched')
                 return emails_to_name
 
             if result_dict['message'] == 'Not Found':
                 warning('There is no repository with the name "{}"'.format(repo_name))
```

### Comparing `exposed_github_user_emails_scanner-1.0.6/setup.py` & `exposed_github_user_emails_scanner-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', mode='r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 
 setuptools.setup(
     name="exposed_github_user_emails_scanner",
-    version="1.0.6",
+    version="1.0.7",
     author="Florian Wahl",
     author_email="florian.wahl.developer@gmail.com",
     description="A cli script to find exposed email addresses of one GitHub user in his or her public repositories.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wahlflo/showExposedGitHubEmails",
     packages=setuptools.find_packages(),
```


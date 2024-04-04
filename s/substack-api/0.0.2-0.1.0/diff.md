# Comparing `tmp/substack_api-0.0.2.tar.gz` & `tmp/substack_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "substack_api-0.1.0.tar", max compression
```

## Comparing `substack_api-0.0.2.tar` & `substack_api-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substack_api-0.0.2/src/substack_api/__init__.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 substack_api-0.0.2/src/substack_api/substack_api.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 substack_api-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 substack_api-0.0.2/LICENSE
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 substack_api-0.0.2/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 substack_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 substack_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 00:13:09.763913 substack_api-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1191 2024-04-04 00:13:09.763913 substack_api-0.1.0/README.md
+-rw-r--r--   0        0        0      388 2024-04-04 00:13:09.763913 substack_api-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 00:13:09.763913 substack_api-0.1.0/substack_api/__init__.py
+-rw-r--r--   0        0        0     5439 2024-04-04 00:13:09.763913 substack_api-0.1.0/substack_api/newsletter.py
+-rw-r--r--   0        0        0     2014 2024-04-04 00:13:09.763913 substack_api-0.1.0/substack_api/user.py
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 substack_api-0.1.0/PKG-INFO
```

### Comparing `substack_api-0.0.2/src/substack_api/substack_api.py` & `substack_api-0.1.0/substack_api/newsletter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,178 @@
-import math
-from time import sleep
-from typing import Dict, List, Tuple, Union
-
-import requests
-
-HEADERS = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36"
-}
-
-def list_all_categories() -> List[Tuple[str, int]]:
-    """
-    Get name / id representations of all newsletter categories
-    """
-    endpoint_cat = "https://substack.com/api/v1/categories"
-    r = requests.get(endpoint_cat, headers=HEADERS)
-    categories = [(i['name'], i['id']) for i in r.json()]
-    return categories
-
-
-def category_id_to_name(id: int) -> str:
-    """
-    Map a numerical category id to a name
-
-    Parameters
-    ----------
-    id : Numerical category identifier
-    """
-    categories = list_all_categories()
-    category_name = [i[0] for i in categories if i[1] == id]
-    if len(category_name) > 0:
-        return category_name[0]
-    else:
-        raise ValueError(f"{id} is not in Substack's list of categories")
-
-
-def category_name_to_id(name: str) -> int:
-    """
-    Map a category name to a numerical id
-
-    Parameters
-    ----------
-    name : Category name
-    """
-    categories = list_all_categories()
-    category_id = [i[1] for i in categories if i[0] == name]
-    if len(category_id) > 0:
-        return category_id[0]
-    else:
-        raise ValueError(f"{name} is not in Substack's list of categories")
-
-
-def get_newsletters_in_category(category_id: int, subdomains_only: bool = False, start_page: int = None, end_page: int = None) -> List:
-    """
-    Collects newsletter objects listed under specified category
-
-    Parameters
-    ----------
-    category_id : Numerical category identifier
-    subdomains_only : Whether to return only newsletter subdomains (needed for post collection), or to return all metadata
-    start_page : Start page for paginated API results
-    end_page : End page for paginated API results
-    """
-    page_num = 0 if start_page is None else start_page
-    page_num_end = math.inf if end_page is None else end_page
-
-    base_url = f"https://substack.com/api/v1/category/public/{category_id}/all?page="
-    page_num = 0
-    more = True
-    all_pubs = []
-    while more and page_num < page_num_end:
-        full_url = base_url + str(page_num)
-        pubs = requests.get(full_url, headers=HEADERS).json()
-        more = pubs["more"]
-        if subdomains_only:
-            pubs = [i["id"] for i in pubs["publications"]]
-        else:
-            pubs = pubs["publications"]
-        all_pubs.extend(pubs)
-        page_num += 1
-        print(f"page {page_num} done")
-        sleep(1)
-
-    return all_pubs
-
-
-def get_newsletter_post_metadata(newsletter_subdomain: str, slugs_only: bool = False, start_offset: int = None, end_offset: int = None) -> List:
-    """
-    Get available post metadata for newsletter
-
-    Parameters
-    ----------
-    newsletter_subdomain : Substack subdomain of newsletter (can be retrieved from `get_newsletters_in_category`)
-    slugs_only : Whether to return only post slugs (needed for post content collection), or to return all metadata
-    start_page : Start page for paginated API results
-    end_page : End page for paginated API results
-    """
-    offset_start = 0 if start_offset is None else start_offset
-    offset_end = math.inf if end_offset is None else end_offset
-
-    last_id_ref = 0
-    all_posts = []
-    while offset_start < offset_end:
-        full_url = f"https://{newsletter_subdomain}.substack.com/api/v1/archive?sort=new&search=&offset={offset_start}&limit=10"
-        posts = requests.get(full_url, headers=HEADERS).json()
-
-        last_id = posts[-1]["id"]
-        if last_id == last_id_ref:
-            break
-        else:
-            last_id_ref = last_id
-
-        if slugs_only:
-            all_posts.extend([i["slug"] for i in posts])
-        else:
-            all_posts.extend(posts)
-
-        offset_start += 10
-        sleep(1)
-
-    return all_posts
-
-
-def get_post_contents(newsletter_subdomain: str, slug: str, html_only: bool = False) -> Union[Dict, str]:
-    """
-    Gets individual post metadata and contents
-
-    Parameters
-    ----------
-    newsletter_subdomain : Substack subdomain of newsletter (can be retrieved from `get_newsletters_in_category`)
-    slug : Slug of post to retrieve (can be retrieved from `get_newsletter_post_metadata`)
-    html_only : Whether to get only HTML of body text, or all metadata/content
-    """
-    endpoint = f"https://{newsletter_subdomain}.substack.com/api/v1/posts/{slug}"
-    post_info = requests.get(endpoint, headers=HEADERS).json()
-    if html_only:
-        return post_info["body_html"]
-    else:
-        return post_info
+import math
+from time import sleep
+from typing import Dict, List, Tuple, Union
+
+from bs4 import BeautifulSoup
+import requests
+
+
+HEADERS = {
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36"
+}
+
+
+def list_all_categories() -> List[Tuple[str, int]]:
+    """
+    Get name / id representations of all newsletter categories
+    """
+    endpoint_cat = "https://substack.com/api/v1/categories"
+    r = requests.get(endpoint_cat, headers=HEADERS, timeout=30)
+    categories = [(i["name"], i["id"]) for i in r.json()]
+    return categories
+
+
+def category_id_to_name(user_id: int) -> str:
+    """
+    Map a numerical category id to a name
+
+    Parameters
+    ----------
+    id : Numerical category identifier
+    """
+    categories = list_all_categories()
+    category_name = [i[0] for i in categories if i[1] == user_id]
+    if len(category_name) > 0:
+        return category_name[0]
+
+    raise ValueError(f"{user_id} is not in Substack's list of categories")
+
+
+def category_name_to_id(name: str) -> int:
+    """
+    Map a category name to a numerical id
+
+    Parameters
+    ----------
+    name : Category name
+    """
+    categories = list_all_categories()
+    category_id = [i[1] for i in categories if i[0] == name]
+    if len(category_id) > 0:
+        return category_id[0]
+    else:
+        raise ValueError(f"{name} is not in Substack's list of categories")
+
+
+def get_newsletters_in_category(
+    category_id: int,
+    subdomains_only: bool = False,
+    start_page: int = None,
+    end_page: int = None,
+) -> List:
+    """
+    Collects newsletter objects listed under specified category
+
+    Parameters
+    ----------
+    category_id : Numerical category identifier
+    subdomains_only : Whether to return only newsletter subdomains (needed for post collection)
+    start_page : Start page for paginated API results
+    end_page : End page for paginated API results
+    """
+    page_num = 0 if start_page is None else start_page
+    page_num_end = math.inf if end_page is None else end_page
+
+    base_url = f"https://substack.com/api/v1/category/public/{category_id}/all?page="
+    page_num = 0
+    more = True
+    all_pubs = []
+    while more and page_num < page_num_end:
+        full_url = base_url + str(page_num)
+        pubs = requests.get(full_url, headers=HEADERS, timeout=30).json()
+        more = pubs["more"]
+        if subdomains_only:
+            pubs = [i["id"] for i in pubs["publications"]]
+        else:
+            pubs = pubs["publications"]
+        all_pubs.extend(pubs)
+        page_num += 1
+        print(f"page {page_num} done")
+        sleep(1)
+
+    return all_pubs
+
+
+def get_newsletter_post_metadata(
+    newsletter_subdomain: str,
+    slugs_only: bool = False,
+    start_offset: int = None,
+    end_offset: int = None,
+) -> List:
+    """
+    Get available post metadata for newsletter
+
+    Parameters
+    ----------
+    newsletter_subdomain : Substack subdomain of newsletter
+    slugs_only : Whether to return only post slugs (needed for post content collection)
+    start_page : Start page for paginated API results
+    end_page : End page for paginated API results
+    """
+    offset_start = 0 if start_offset is None else start_offset
+    offset_end = math.inf if end_offset is None else end_offset
+
+    last_id_ref = 0
+    all_posts = []
+    while offset_start < offset_end:
+        full_url = f"https://{newsletter_subdomain}.substack.com/api/v1/archive?sort=new&search=&offset={offset_start}&limit=10"
+        posts = requests.get(full_url, headers=HEADERS, timeout=30).json()
+
+        if len(posts) == 0:
+            break
+
+        last_id = posts[-1]["id"]
+        if last_id == last_id_ref:
+            break
+
+        last_id_ref = last_id
+
+        if slugs_only:
+            all_posts.extend([i["slug"] for i in posts])
+        else:
+            all_posts.extend(posts)
+
+        offset_start += 10
+        sleep(1)
+
+    return all_posts
+
+
+def get_post_contents(
+    newsletter_subdomain: str, slug: str, html_only: bool = False
+) -> Union[Dict, str]:
+    """
+    Gets individual post metadata and contents
+
+    Parameters
+    ----------
+    newsletter_subdomain : Substack subdomain of newsletter
+    slug : Slug of post to retrieve (can be retrieved from `get_newsletter_post_metadata`)
+    html_only : Whether to get only HTML of body text, or all metadata/content
+    """
+    endpoint = f"https://{newsletter_subdomain}.substack.com/api/v1/posts/{slug}"
+    post_info = requests.get(endpoint, headers=HEADERS, timeout=30).json()
+    if html_only:
+        return post_info["body_html"]
+
+    return post_info
+
+
+def get_newsletter_recommendations(newsletter_subdomain: str) -> List[Dict[str, str]]:
+    """
+    Gets recommended newsletters for a given newsletter
+
+    Parameters
+    ----------
+    newsletter_subdomain : Substack subdomain of newsletter
+    """
+    endpoint = f"https://{newsletter_subdomain}.substack.com/recommendations"
+    r = requests.get(endpoint, headers=HEADERS, timeout=30)
+    recs = r.text
+    soup = BeautifulSoup(recs, "html.parser")
+    div_elements = soup.find_all("div", class_="publication-content")
+    a_elements = [div.find("a") for div in div_elements]
+    titles = [i.text for i in soup.find_all("div", {"class": "publication-title"})]
+    links = [i["href"].split("?")[0] for i in a_elements]
+    results = [{"title": t, "url": u} for t, u in zip(titles, links)]
+
+    return results
```

### Comparing `substack_api-0.0.2/README.md` & `substack_api-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Substack-api
-
-**An unofficial Python wrapper around Substack's API.**
-
-I developed this package as a lightweight tool to help researchers collect data about Substack newsletters, and to help writers archive their work off-platform. This is not a tool designed for bulk text extraction/web scraping. It supports the following functionality:
-
-* Download full JSON metadata about newsletters by category
-* Download full JSON metadata about posts by newsletter
-* Download text of individual, publicly-available posts
-* List newsletter categories
-
-## Installation
-
-`pip install substack-api`
-
-## Usage
-
-```from substack_api import substack_api```
-
-List all categories on Substack:
-
-```
-substack_api.list_all_categories()
-```
-
-Get metadata for the first 2 pages of Technology newsletters:
-
-```
-substack_api.get_newsletters_in_category(4, start_page=0, end_page=2)
-```
-
-Get post metadata for the most recent 30 posts from a newsletter:
-
-```
-substack_api.get_newsletter_post_metadata("platformer", start_offset=0, end_offset=30)
-```
-
-Get post contents (HTML only) from one newsletter post:
-
-```
-substack_api.get_post_contents("platformer", "how-a-single-engineer-brought-down", html_only=True)
+# Substack-api
+
+**An unofficial Python wrapper around Substack's API.**
+
+I developed this package as a lightweight tool to help researchers collect data about Substack newsletters, and to help writers archive their work off-platform. This is not a tool designed for bulk text extraction/web scraping. It supports the following functionality:
+
+* Download full JSON metadata about newsletters by category
+* Download full JSON metadata about posts by newsletter
+* Download text of individual, publicly-available posts
+* List newsletter categories
+
+## Installation
+
+`pip install substack-api`
+
+## Usage
+
+```from substack_api import substack_api```
+
+List all categories on Substack:
+
+```
+substack_api.list_all_categories()
+```
+
+Get metadata for the first 2 pages of Technology newsletters:
+
+```
+substack_api.get_newsletters_in_category(4, start_page=0, end_page=2)
+```
+
+Get post metadata for the most recent 30 posts from a newsletter:
+
+```
+substack_api.get_newsletter_post_metadata("platformer", start_offset=0, end_offset=30)
+```
+
+Get post contents (HTML only) from one newsletter post:
+
+```
+substack_api.get_post_contents("platformer", "how-a-single-engineer-brought-down", html_only=True)
 ```
```

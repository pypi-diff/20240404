# Comparing `tmp/crewai_tools-0.1.2.tar.gz` & `tmp/crewai_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.1.2.tar", max compression
+gzip compressed data, was "crewai_tools-0.1.3.tar", max compression
```

## Comparing `crewai_tools-0.1.2.tar` & `crewai_tools-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.2/README.md
--rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.2/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.2/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.2/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.2/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.2/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1541 2024-03-27 18:04:45.820264 crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.821112 crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1598 2024-03-27 18:04:45.822270 crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1460 2024-03-27 18:04:45.823331 crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     1854 2024-03-27 18:04:45.824045 crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1495 2024-03-27 18:04:45.824458 crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.825044 crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1246 2024-03-27 18:04:45.827249 crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.2/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.2/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.2/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.2/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1445 2024-03-27 18:04:45.828786 crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.2/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1531 2024-03-27 18:04:45.829385 crewai_tools-0.1.2/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.829923 crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     1889 2024-03-27 18:04:45.830546 crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1663 2024-03-27 18:04:45.830891 crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-04-03 09:02:15.231634 crewai_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.3/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.3/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.3/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.3/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.3/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.3/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1541 2024-03-27 18:04:45.820264 crewai_tools-0.1.3/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.3/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.821112 crewai_tools-0.1.3/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.3/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.3/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.3/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1598 2024-03-27 18:04:45.822270 crewai_tools-0.1.3/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.3/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1460 2024-03-27 18:04:45.823331 crewai_tools-0.1.3/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.3/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.3/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.3/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     1854 2024-03-27 18:04:45.824045 crewai_tools-0.1.3/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.3/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1495 2024-03-27 18:04:45.824458 crewai_tools-0.1.3/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.3/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.825044 crewai_tools-0.1.3/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.3/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.3/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.3/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1246 2024-03-27 18:04:45.827249 crewai_tools-0.1.3/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.3/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.3/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.3/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.3/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.3/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.3/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.3/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.3/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.3/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.3/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.3/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1445 2024-03-27 18:04:45.828786 crewai_tools-0.1.3/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.3/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1531 2024-03-27 18:04:45.829385 crewai_tools-0.1.3/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.3/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.829923 crewai_tools-0.1.3/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.3/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     1889 2024-03-27 18:04:45.830546 crewai_tools-0.1.3/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.3/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1663 2024-03-27 18:04:45.830891 crewai_tools-0.1.3/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      730 2024-04-04 16:16:10.201900 crewai_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.3/PKG-INFO
```

### Comparing `crewai_tools-0.1.2/LICENSE` & `crewai_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/README.md` & `crewai_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.1.3/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.1.3/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/__init__.py` & `crewai_tools-0.1.3/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/base_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/docx_search_tool/docx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/github_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/rag/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.1.3/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/xml_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.1.3/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.1.3/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.2/pyproject.toml` & `crewai_tools-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.1.2/PKG-INFO` & `crewai_tools-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


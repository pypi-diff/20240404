# Comparing `tmp/tcia_utils-2.0.1.tar.gz` & `tmp/tcia_utils-2.1.0.tar.gz`

## Comparing `tcia_utils-2.0.1.tar` & `tcia_utils-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/curation.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    87608 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/utils.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/src/tcia_utils/wordpress.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/LICENSE
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/README.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 tcia_utils-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    87232 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/wordpress.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/PKG-INFO
```

### Comparing `tcia_utils-2.0.1/src/tcia_utils/datacite.py` & `tcia_utils-2.1.0/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.0.1/src/tcia_utils/nbia.py` & `tcia_utils-2.1.0/src/tcia_utils/nbia.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,23 @@
 from datetime import datetime
 from datetime import timedelta
 from enum import Enum
 import matplotlib
 import matplotlib.pyplot as plt
 import plotly.express as px
 import pydicom
+import pydicom_seg
+import rt_utils
+import tkinter
+from tkinter import filedialog
 import numpy as np
 from ipywidgets import interact
 from tcia_utils.utils import searchDf
+from tcia_utils.utils import format_disk_space
+from tcia_utils.utils import remove_html_tags
 from tcia_utils.datacite import getDoi
 
 
 class StopExecution(Exception):
     def _render_traceback_(self):
         pass
 
@@ -538,21 +544,24 @@
 
 def getUpdatedSeries(date,
                      api_url = "",
                      format = ""):
     """
     Gets "new" series metadata from a specified api_url.
     The date format is YYYY/MM/DD.
-    NOTE: Unlike other API endpoints, this one expects MM/DD/YYYY, 
-      but we convert from YYYY/MM/DD so tcia-utils date inputs are consistent.
+    NOTE: Unlike other API endpoints, this one expects DD/MM/YYYY, 
+      but we convert to YYYY/MM/DD so tcia-utils date inputs are consistent.
     """
     endpoint = "getUpdatedSeries"
 
     # convert to NBIA's expected date format
-    nbiaDate = datetime.strptime(date, "%Y/%m/%d").strftime("%m/%d/%Y")
+    # It appears there is likely a bug in the API here.  
+    # Date format for the API is currently DD/MM/YYYY so we'll convert it.
+    nbiaDate = datetime.strptime(date, "%Y/%m/%d").strftime("%d/%m/%Y")
+
 
     # create options dict to construct URL
     options = {}
     options['fromDate'] = nbiaDate
 
     data = queryData(endpoint, options, api_url, format)
     return data
@@ -867,23 +876,27 @@
         _log.error(err)
 
 ##########################
 ##########################
 # Advanced API Endpoints
 
 
-def getCollectionDescriptions(api_url = "", format = ""):
+def getCollectionDescriptions(api_url = "", format = "", removeHtml = None):
     """
     Gets HTML-formatted descriptions of collections and their DOIs
     """
     endpoint = "getCollectionDescriptions"
     options = {}
 
     data = queryData(endpoint, options, api_url, format)
-    return data
+    if format == "df" and removeHtml == "yes":
+        data['description'] = data['description'].apply(remove_html_tags)
+        return data
+    else:
+        return data
 
 
 def getCollectionPatientCounts(api_url = "", format = ""):
     """
     Gets counts of Patient by collection from Advanced API
     """
     endpoint = "getCollectionValuesAndCounts"
@@ -1409,16 +1422,15 @@
                 Helper functions reportCollectionSummary() and reportDoiSummary() are
                 the expected way to deal with this, which pass this parameter accordingly.
     api_url: Only necessary if input_type = list or manifest.
             Set to 'restricted' for limited-access collections or 
             'nlst' for National Lung Screening trial.
             
     See reportDataSummary() for more details.
-    """
-    
+    """    
     df = reportDataSummary(series_data, input_type, report_type = "doi", api_url = api_url, format = format)   
     return df
 
 
 def reportCollectionSummary(series_data, input_type="", api_url = "", format=""):
     """
     Generate a summary report about Collections from series metadata created by the
@@ -1636,49 +1648,15 @@
     fig = px.pie(df, names='Labels', values='Values', title=f'{metric_name} Distribution Across Datasets')
     fig.update_traces(textposition='inside', textinfo='percent+label')
     fig.update_layout(showlegend=True, legend_title_text='Datasets', width=width, height=height)
 
     # Show the pie chart
     fig.show()
 
-
-def format_disk_space_binary(size_in_bytes):
-    """
-    Helper function for reportCollections() to format bytes to other binary units.
-    I.e. Mebibytes (MiB) reported in Windows.
-    """
-    if size_in_bytes < 1024 ** 2:
-        return f'{size_in_bytes / 1024:.2f} KB'
-    elif size_in_bytes < 1024 ** 3:
-        return f'{size_in_bytes / (1024 ** 2):.2f} MB'
-    elif size_in_bytes < 1024 ** 4:
-        return f'{size_in_bytes / (1024 ** 3):.2f} GB'
-    elif size_in_bytes < 1024 ** 5:
-        return f'{size_in_bytes / (1024 ** 4):.2f} TB'
-    else:
-        return f'{size_in_bytes / (1024 ** 5):.2f} PB'
-        
-def format_disk_space(size_in_bytes):
-    """
-    Helper function for reportCollections() to format bytes to other units.
-    I.e. Megabytes (MB) reported in Mac/Linux.
-    """
-    if size_in_bytes < 1000:
-        return f'{size_in_bytes:.2f} B'
-    elif size_in_bytes < 1000 ** 2:
-        return f'{size_in_bytes / 1000:.2f} kB'
-    elif size_in_bytes < 1000 ** 3:
-        return f'{size_in_bytes / (1000 ** 2):.2f} MB'
-    elif size_in_bytes < 1000 ** 4:
-        return f'{size_in_bytes / (1000 ** 3):.2f} GB'
-    elif size_in_bytes < 1000 ** 5:
-        return f'{size_in_bytes / (1000 ** 4):.2f} TB'
-    else:
-        return f'{size_in_bytes / (1000 ** 5):.2f} PB'
-        
+    
 def reportSeriesReleaseDate(series_data, chart_width = 1024, chart_height = 768):
     """
     Ingests the results of getSeries() as df or JSON and visualizes the 
     submission timeline of the series in it by collection.
     
     Currently this only supports getSeries(), but feature requests have been submitted
     to the NBIA team to make it possible to use this with the other series API endpoints.
@@ -1937,22 +1915,34 @@
         return df
     else:
         return df
 
 
 def viewSeries(seriesUid = "", path = ""):
     """
-    Visualizes a Series (scan) you've downloaded in the notebook
-    Requires EITHER a seriesUid or path parameter
-    Leave seriesUid empty if you want to provide a custom path.
+    Visualizes a Series (scan) you've downloaded.
+    If neither seriesUid nor path is specified, the user will be 
+    prompted to select a directory using a GUI.
     The function assumes "tciaDownload/<seriesUid>/" as path if
     seriesUid is provided since this is where downloadSeries() saves data.
+    Leave seriesUid empty if you want to provide a custom path.
     """
     # set path where downloadSeries() saves the data if seriesUid is provided
-    if seriesUid != "":
+    if seriesUid == "" and path == "":
+        try:
+            tkinter.Tk().withdraw()
+            folder_path = filedialog.askdirectory()
+            path = folder_path
+        except Exception:
+            _log.error(
+                f"\nYou are executing the function with unspecified parameters in an unsupported enviroment,"
+                "\nor with an unsupported modality. Please specify the reference series UID or the folder path instead."
+            )
+            return
+    elif seriesUid != "":
         path = "tciaDownload/" + seriesUid
 
     # error message function for when series doesn't exist or is invalid data
     def seriesInvalid(uid):
         if seriesUid:
             link = f"https://nbia.cancerimagingarchive.net/viewer/?series={seriesUID}"
         else:
@@ -2012,15 +2002,14 @@
     Visualizes a Series (scan) you've downloaded and
     adds an overlay from the SEG series.
     Requires a path parameter for the reference series.
     Requires the file path for the annotation series.
     Used by the viewSeriesAnnotation() function.
     Not recommended to be used as a standalone function.
     """
-    import pydicom_seg 
     slices = [pydicom.dcmread(seriesPath + '/' + s) for s in os.listdir(seriesPath) if s.endswith(".dcm")]
     slices.sort(key = lambda x: int(x.InstanceNumber), reverse = True)
 
     try:
         modality = slices[0].Modality
     except IndexError:
         seriesInvalid(seriesUid)
@@ -2096,15 +2085,14 @@
     adds an overlay from the RTSTRUCT series.
     Requires a path parameter for the reference series.
     Requires the file path for the annotation series.
     Currenly not able to visualize seed points.
     Used by the viewSeriesAnnotation() function.
     Not recommended to be used as a standalone function.
     """
-    import rt_utils 
     rtstruct = rt_utils.RTStructBuilder.create_from(seriesPath, RTPath)
     roi_names = rtstruct.get_roi_names()
 
     slices = rtstruct.series_data
     try:
         modality = slices[0].Modality
     except IndexError:
@@ -2175,16 +2163,14 @@
     the required parameters are not specified.
     Leave seriesUid and/or annotationUid empty if
     you want to provide a custom path.
     The function assumes "tciaDownload/<UID>/" as path if seriesUid and/or
     annotationUid is provided since this is where downloadSeries() saves data.
     Note that non-axial images might not be correctly displayed.
     """
-    import tkinter
-    from tkinter import filedialog
     def seriesInvalid(uid, path):
         if uid:
             link = f"https://nbia.cancerimagingarchive.net/viewer/?series={uid}"
         else:
             link = "https://nbia.cancerimagingarchive.net/viewer/?series=YOUR_SERIES_UID"
         _log.error(
             f"Cannot find a valid DICOM series at: {path}\n"
```

### Comparing `tcia_utils-2.0.1/src/tcia_utils/pathdb.py` & `tcia_utils-2.1.0/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.0.1/src/tcia_utils/wordpress.py` & `tcia_utils-2.1.0/src/tcia_utils/wordpress.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pandas as pd
 import json
 import requests
 from datetime import datetime
 import logging
 from tcia_utils.utils import searchDf
+from tcia_utils.utils import remove_html_tags
 
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
 base_url = "https://cancerimagingarchive.net/api/v1/"
 
-def getQuery(endpoint, per_page, format="", file_name=None, fields=None, ids=None, query=None):
+def getQuery(endpoint, per_page, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Handle query basics that are common to all endpoints such as
     paging results, setting output formats, and file names.
 
     Args:
         endpoint (str): The API endpoint to query.
         per_page (int, optional): Number of results per page (default is 250).
@@ -79,25 +80,53 @@
             if file_name:
                 with open(file_name, "w") as f:
                     json.dump(data, f)
             return data
         elif format == "df":
             # Convert to DataFrame
             df = pd.DataFrame(data)
+            # optionally remove HTML formatting for relevant columns
+            if removeHtml == "yes":
+                if "collections" in endpoint:
+                    for column in ["collection_summary", "detailed_description", "publications_using", 
+                                   "additional_resources", "collection_download_info", "publications_related",
+                                   "version_change_log", "collection_acknowledgements"]:
+                        if column in df:
+                            df[column] = df[column].apply(remove_html_tags)
+                elif "analysis" in endpoint:
+                    for column in ["result_summary", "detailed_description", "publications_using", 
+                                   "additional_resources", "collection_download_info", "publications_related",
+                                   "version_change_log", "result_acknowledgements"]:
+                        if column in df:
+                            df[column] = df[column].apply(remove_html_tags)
+                elif "downloads" in endpoint:
+                    for column in ["description"]:
+                        if column in df:
+                            df[column] = df[column].apply(remove_html_tags)
+                elif "citations" in endpoint:
+                    for column in ["tcia_citation_text, tcia_citation_statement"]:
+                        if column in df:
+                            df[column] = df[column].apply(remove_html_tags)
+                elif "versions" in endpoint:
+                    for column in ["version_text"]:
+                        if column in df:
+                            df[column] = df[column].apply(remove_html_tags)
+
+            # save csv if file name provided
             if file_name:
                 df.to_csv(file_name, index=False)
             return df
         else:
             raise ValueError("Invalid format. Please choose 'json', 'df', or 'csv'.")
     else:
         _log.error('Error accessing the API: %s', response.status_code)
         return None
 
 
-def getCollections(per_page=100, format="", file_name=None, fields=None, ids=None, query=None):
+def getCollections(per_page=100, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Retrieve collections from the API.
 
     Args:
         per_page (int, optional): Number of collections per page (default is 100).
         format (str, optional): Output format ('json' or 'df') (default is JSON if not populated).
         file_name (str, optional): File name to save the output as JSON or CSV if format = "df".
@@ -117,19 +146,19 @@
         list or DataFrame: Retrieved collections based on the specified parameters and format.
 
     """
     # set the endpoint for Collections query
     endpoint = "collections/"
     
     # call getQuery to retrieve the data
-    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query)
+    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query, removeHtml)
     return data
 
 
-def getAnalyses(per_page=100, format="", file_name=None, fields=None, ids=None, query=None):
+def getAnalyses(per_page=100, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Retrieve Analysis Results from the API.
 
     Args:
         per_page (int, optional): Number of analysis results per page (default is 100).
         format (str, optional): Output format ('json' or 'df') (default is JSON if not populated).
         file_name (str, optional): File name to save the output as JSON or CSV if format = "df".
@@ -149,19 +178,19 @@
         list or DataFrame: Retrieved analysis results based on the specified parameters and format.
 
     """
     # set the endpoint for an Analysis Result query
     endpoint = "analysis-results/"
     
     # call getQuery to retrieve the data
-    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query)
+    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query, removeHtml)
     return data
 
 
-def getDownloads(per_page=200, format="", file_name=None, fields=None, ids=None, query=None):
+def getDownloads(per_page=200, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Retrieve Download metadata from the API.
 
     Args:
         per_page (int, optional): Number of downloads per page (default is 200).
         format (str, optional): Output format ('json' or 'df') (default is JSON if not populated).
         file_name (str, optional): File name to save the output as JSON or CSV if format = "df".
@@ -180,19 +209,19 @@
         list or DataFrame: Retrieved download metadata based on the specified parameters and format.
 
     """
     # Set the endpoint for a Download query
     endpoint = "downloads/"
     
     # Call getQuery to retrieve the data
-    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query)
+    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query, removeHtml)
     return data
 
 
-def getCitations(per_page=200, format="", file_name=None, fields=None, ids=None, query=None):
+def getCitations(per_page=200, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Retrieve Citation metadata from the API.
 
     Args:
         per_page (int, optional): Number of citations per page (default is 200).
         format (str, optional): Output format ('json' or 'df') (default is JSON if not populated).
         file_name (str, optional): File name to save the output as JSON or CSV if format = "df".
@@ -201,25 +230,24 @@
                                  type, link, title, template, yoast_head, yoast_head_json, tcia_citation_type,
                                  tcia_citation_text, tcia_citation_statement, tcia_citation_doi, _links.
         ids (list, optional): List of IDs to include in the request (default is None).
         query (str, optional): Search criteria to filter results (default is None).
 
     Returns:
         list or DataFrame: Retrieved citation metadata based on the specified parameters and format.
-
     """
     # Set the endpoint for a Citation query
     endpoint = "citations/"
     
     # Call getQuery to retrieve the data
-    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query)
+    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query, removeHtml)
     return data
 
 
-def getVersions(per_page=200, format="", file_name=None, fields=None, ids=None, query=None):
+def getVersions(per_page=200, format="", file_name=None, fields=None, ids=None, query=None, removeHtml=None):
     """
     Retrieve Version metadata from the API.
 
     Args:
         per_page (int, optional): Number of citations per page (default is 200).
         format (str, optional): Output format ('json' or 'df') (default is JSON if not populated).
         file_name (str, optional): File name to save the output as JSON or CSV if format = "df".
@@ -236,9 +264,9 @@
         list or DataFrame: Retrieved citation metadata based on the specified parameters and format.
 
     """
     # Set the endpoint for a Citation query
     endpoint = "versions/"
     
     # Call getQuery to retrieve the data
-    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query)
+    data = getQuery(endpoint, per_page, format, file_name, fields, ids, query, removeHtml)
     return data
```

### Comparing `tcia_utils-2.0.1/.gitignore` & `tcia_utils-2.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -124,7 +124,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 *.bak
+.DS_Store
```

### Comparing `tcia_utils-2.0.1/LICENSE` & `tcia_utils-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.0.1/README.md` & `tcia_utils-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.0.1/pyproject.toml` & `tcia_utils-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "2.0.1"
+version = "2.1.0"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "pydicom",
+  "unidecode",
   "requests",
   "pandas",
   "matplotlib",
   "plotly",
   "numpy",
   "ipywidgets", 
   "pydicom-seg", 
-  "rt-utils",
-  "nibabel",
-  "nilearn"
+  "rt-utils"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kirbyju/tcia_utils"
 "Bug Tracker" = "https://github.com/kirbyju/tcia_utils/issues"
```

### Comparing `tcia_utils-2.0.1/PKG-INFO` & `tcia_utils-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tcia_utils
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: ipywidgets
 Requires-Dist: matplotlib
-Requires-Dist: nibabel
-Requires-Dist: nilearn
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pydicom
 Requires-Dist: pydicom-seg
 Requires-Dist: requests
 Requires-Dist: rt-utils
+Requires-Dist: unidecode
 Description-Content-Type: text/markdown
 
 # Overview
 The [tcia_utils](https://pypi.org/project/tcia-utils/) package contains functions to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python. Learn more about TCIA and its open-access datasets at https://www.cancerimagingarchive.net/.  Please be sure to comply with the [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF).
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tcia-utils?period=month&units=international_system&left_color=blue&right_color=grey&left_text=Downloads%20/%20Month)](https://pepy.tech/project/tcia-utils)
```


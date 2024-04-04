# Comparing `tmp/themoviedb-lib-0.0.1.tar.gz` & `tmp/themoviedb-lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themoviedb-lib-0.0.1.tar", last modified: Tue Mar 26 17:26:07 2024, max compression
+gzip compressed data, was "themoviedb-lib-0.0.2.tar", last modified: Thu Apr  4 14:37:31 2024, max compression
```

## Comparing `themoviedb-lib-0.0.1.tar` & `themoviedb-lib-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-03-26 17:26:07.561818 themoviedb-lib-0.0.1/
--rw-r--r--   0 mark      (1000) mark      (1000)     1063 2024-01-14 12:53:54.000000 themoviedb-lib-0.0.1/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)      712 2024-03-26 17:26:07.560818 themoviedb-lib-0.0.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-03-26 15:58:41.000000 themoviedb-lib-0.0.1/README.md
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-03-26 17:26:07.561818 themoviedb-lib-0.0.1/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1188 2024-03-26 17:06:07.000000 themoviedb-lib-0.0.1/setup.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-03-26 17:26:07.560818 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      712 2024-03-26 17:26:07.000000 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      345 2024-03-26 17:26:07.000000 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-03-26 17:26:07.000000 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       39 2024-03-26 17:26:07.000000 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        5 2024-03-26 17:26:07.000000 themoviedb-lib-0.0.1/themoviedb_lib.egg-info/top_level.txt
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-03-26 17:26:07.559817 themoviedb-lib-0.0.1/tmdb/
--rw-r--r--   0 mark      (1000) mark      (1000)    16863 2024-03-26 15:52:08.000000 themoviedb-lib-0.0.1/tmdb/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-03-26 17:26:07.560818 themoviedb-lib-0.0.1/tmdb/tests/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-12-12 21:04:09.000000 themoviedb-lib-0.0.1/tmdb/tests/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3770 2024-03-26 15:52:08.000000 themoviedb-lib-0.0.1/tmdb/tests/test_tmdb_api.py
--rw-r--r--   0 mark      (1000) mark      (1000)    11503 2024-03-26 15:52:08.000000 themoviedb-lib-0.0.1/tmdb/tests/test_tmdb_entry.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-03-26 15:52:08.000000 themoviedb-lib-0.0.1/tmdb/tests/test_tmdb_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.498574 themoviedb-lib-0.0.2/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/tmdb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_request.py
```

### Comparing `themoviedb-lib-0.0.1/LICENSE` & `themoviedb-lib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `themoviedb-lib-0.0.1/tmdb/__init__.py` & `themoviedb-lib-0.0.2/tmdb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,20 +121,35 @@
         for a_search_tab in html_page.find_all("a", {"class": "search_tab"}):
             if a_search_tab.get("id") is not None:
                 categories.append(a_search_tab.get("id"))
 
         return categories
 
     @classmethod
-    def find(cls):
+    def poster_path(cls, poster_id: str, original_resolution: bool = True,
+                    width: int = None, height: int = None) -> str:
         """
-        TODO: method to find a specific movie or tv series
+        Returns the TMDb URL path for a poster image. Allowed sizes: 94x141, 188x282, 150x225, 300x450, 600x900.
+
+        :param poster_id: The poster ID.
+        :param original_resolution: Whether to return the path for the original resolution of the image.
+        :param width: The width of the image.
+        :param height: The height of the image.
+        :return: Poster path as string.
         """
 
-        raise NotImplementedError()
+        if original_resolution and width is None and height is None:
+            return f"/t/p/original/{poster_id}.jpg"
+
+        if not any([width == 94 and height == 141, width == 188 and height == 282, width == 150 and height == 225,
+                    width == 300 and height == 450, width == 600 and height == 900]):
+
+            raise ValueError("Image size not supported.")
+
+        return f"/t/p/w{width}_and_h{height}_bestv2/{poster_id}.jpg"
 
     @classmethod
     def __search_results(cls, html_page: BeautifulSoup, language: str) -> list:
         search_results = []
         for div_card in html_page.find_all('div', {'class': 'card v4 tight'}):
             tmdb_entry = TMDbEntry(language=language)
 
@@ -190,26 +205,42 @@
                 search_results += cls.search(query=query, page=page + 1, language=language,
                                              recursive=True, max_pages=max_pages - 1)
 
         return search_results
 
     class Movie:
         @classmethod
-        def poster_path(cls):
+        def details(cls):
+            """
+            TODO: method to get information for a specific movie
+            """
+
+            raise NotImplementedError()
+
+        @classmethod
+        def poster_id(cls):
             """
-            TODO: method to get the poster_path for a specific movie
+            TODO: method to get the poster_id for a specific movie
             """
 
             raise NotImplementedError()
 
     class TV:
         @classmethod
-        def poster_path(cls):
+        def details(cls):
             """
-            TODO: method to get the poster_path for a specific tv series
+            TODO: method to get information for a specific tv series
+            """
+
+            raise NotImplementedError()
+
+        @classmethod
+        def poster_id(cls):
+            """
+            TODO: method to get the poster_id for a specific tv series
             """
 
             raise NotImplementedError()
 
         @classmethod
         @cache
         def seasons(cls, series_id: str) -> list:
@@ -228,16 +259,24 @@
                 season_number = (re.search(r"season/(\d+)", season.find("h2").find("a").get("href")).group()
                                  .replace("season/", ""))
                 seasons.append(season_number)
 
             return seasons
 
         @classmethod
-        def number_of_seasons(cls):
-            raise NotImplementedError()
+        def number_of_seasons(cls, series_id: str) -> int:
+            # get seasons for the tv show
+            seasons = API.TV.seasons(series_id=series_id)
+
+            # remove season '0'
+            if "0" in seasons:
+                seasons.remove("0")
+
+            # return season count
+            return len(seasons)
 
         @classmethod
         @cache
         def episodes(cls, series_id: str, season_id: str, language: str = "en") -> list:
             # build a request for TMDb
             path = f"/tv/{series_id}/season/{season_id}"
             query = f"language={language}"
@@ -413,55 +452,40 @@
         :return: Is (not) a TV show.
         """
         if self.category is None:
             return False
 
         return self.category == "tv"
 
-    def __poster_path(self, width: int, height: int) -> str:
-        return f"/t/p/w{width}_and_h{height}_bestv2/{self.poster_id}.jpg"
-
-    def poster(self, resolution: str = "low", high_resolution: bool = False) -> Optional[io.BytesIO]:
+    def poster(self, resolution: str = "original", high_resolution: bool = False) -> Optional[io.BytesIO]:
         """
         Returns the poster of this TMDbEntry. By default, with a resolution of 94x141.
 
-        :param resolution: Specify the desired resolution for the image (e.g. 'low', 'medium', 'high').
+        :param resolution: Specify the desired resolution for the image (e.g. 'original', 'low', 'medium' or 'high').
         :parameter high_resolution: Specify whether the image should be returned in a higher resolution (600x900).
         :return: Poster image.
         """
 
         if self.poster_id is None:
             return None
 
-        if resolution != "low" and resolution != "medium" and resolution != "high":
-            raise ValueError("Specified resolution must be 'low', 'medium' or 'high'.")
-
         if high_resolution:
             resolution = "high"
 
-        if resolution == "low":
-            return Request.image(file_path=self.__poster_path(width=94, height=141))
-
-        if resolution == "medium":
-            return Request.image(file_path=self.__poster_path(width=188, height=282))
-
-        if resolution == "high":
-            return Request.image(file_path=self.__poster_path(width=600, height=900))
-
-    def get_poster(self, high_resolution: bool = False):
-        """
-        TODO: REMOVE THIS METHOD. NOW CALLABLE AS TMDbEntry.poster().\n
-
-        Returns the poster of this TMDbEntry. By default, with a resolution of 94x141.
-
-        :parameter high_resolution: Specify whether the image should be returned in a higher resolution (600x900).
-        :return: Poster image.
-        """
-
-        raise Exception("get_poster() HAS BEEN REMOVED. PLEASE USE TMDbEntry.poster().")
+        match resolution:
+            case "original":
+                return Request.image(file_path=API.poster_path(poster_id=self.poster_id, original_resolution=True))
+            case "low":
+                return Request.image(file_path=API.poster_path(poster_id=self.poster_id, width=150, height=225))
+            case "medium":
+                return Request.image(file_path=API.poster_path(poster_id=self.poster_id, width=300, height=450))
+            case "high":
+                return Request.image(file_path=API.poster_path(poster_id=self.poster_id, width=600, height=900))
+            case _:
+                raise ValueError("Specified resolution must be 'low', 'medium', 'high' or 'original'.")
 
     def seasons(self) -> list:
         """
         Returns a list of all seasons for a TV series.
 
         :return: List of seasons.
         """
@@ -481,19 +505,7 @@
         """
 
         # raise exception if TMDbEntry is not a TV series
         if not self.is_tv():
             raise Exception(f"TMDbEntry is not a TV series. Category: {self.category}")
 
         return API.TV.episodes(series_id=self.tmdb_id, season_id=season_id, language=self.language)
-
-    def season(self, season_id: str) -> dict:
-        """
-        TODO: REMOVE THIS METHOD. NOW CALLABLE AS TMDbEntry.episodes().\n
-
-        Returns a dictionary mapping all the episodes for a specific season.
-
-        :param season_id: The season id.
-        :return: Dictionary mapping the season´s episodes.
-        """
-
-        raise Exception("season() HAS BEEN REMOVED. PLEASE USE TMDbEntry.episodes().")
```

### Comparing `themoviedb-lib-0.0.1/tmdb/tests/test_tmdb_entry.py` & `themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,19 @@
         self.assertIsInstance(tmdb_entry.poster(resolution="medium"), io.BytesIO)
 
     def test_poster_high_resolution(self):
         tmdb_entry = TMDbEntry(poster_id="mqGTDn6c5wy4Bwf6DR7eZeO7c5d")
 
         self.assertIsInstance(tmdb_entry.poster(resolution="high"), io.BytesIO)
 
+    def test_poster_original_resolution(self):
+        tmdb_entry = TMDbEntry(poster_id="mqGTDn6c5wy4Bwf6DR7eZeO7c5d")
+
+        self.assertIsInstance(tmdb_entry.poster(resolution="original"), io.BytesIO)
+
     def test_poster_poster_id_is_none(self):
         tmdb_entry = TMDbEntry(poster_id=None)
 
         self.assertIsNone(tmdb_entry.poster())
 
     def test_poster_invalid_resolution(self):
         tmdb_entry = TMDbEntry(poster_id="mqGTDn6c5wy4Bwf6DR7eZeO7c5d")
```

### Comparing `themoviedb-lib-0.0.1/tmdb/tests/test_tmdb_request.py` & `themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_request.py`

 * *Files identical despite different names*


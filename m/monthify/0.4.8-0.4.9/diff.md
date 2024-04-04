# Comparing `tmp/monthify-0.4.8.tar.gz` & `tmp/monthify-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.4.8.tar", max compression
+gzip compressed data, was "monthify-0.4.9.tar", max compression
```

## Comparing `monthify-0.4.8.tar` & `monthify-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.4.8/README.md
--rw-r--r--   0        0        0      735 2023-07-02 01:29:05.096437 monthify-0.4.8/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.4.8/monthify/__main__.py
--rw-r--r--   0        0        0     1739 2023-08-01 19:57:31.582312 monthify-0.4.8/monthify/args.py
--rw-r--r--   0        0        0     1103 2023-07-02 01:14:09.885599 monthify-0.4.8/monthify/auth.py
--rw-r--r--   0        0        0      811 2023-07-02 01:14:09.885599 monthify-0.4.8/monthify/config.py
--rw-r--r--   0        0        0     3273 2023-08-06 09:37:33.569263 monthify-0.4.8/monthify/main.py
--rw-r--r--   0        0        0    18572 2023-08-07 07:51:37.815320 monthify-0.4.8/monthify/script.py
--rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.4.8/monthify/track.py
--rw-r--r--   0        0        0     1980 2023-08-01 19:57:31.582312 monthify-0.4.8/monthify/utils.py
--rw-r--r--   0        0        0      815 2023-08-07 07:51:37.815320 monthify-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.4.9/README.md
+-rw-r--r--   0        0        0      735 2023-07-02 01:29:05.096437 monthify-0.4.9/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.4.9/monthify/__main__.py
+-rw-r--r--   0        0        0     1739 2023-08-01 19:57:31.582312 monthify-0.4.9/monthify/args.py
+-rw-r--r--   0        0        0     1045 2024-04-04 10:11:34.029819 monthify-0.4.9/monthify/auth.py
+-rw-r--r--   0        0        0      811 2023-07-02 01:14:09.885599 monthify-0.4.9/monthify/config.py
+-rw-r--r--   0        0        0     3273 2024-02-13 21:36:44.207609 monthify-0.4.9/monthify/main.py
+-rw-r--r--   0        0        0    18671 2024-04-04 10:11:34.029819 monthify-0.4.9/monthify/script.py
+-rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.4.9/monthify/track.py
+-rw-r--r--   0        0        0     1428 2024-04-04 10:11:34.029819 monthify-0.4.9/monthify/utils.py
+-rw-r--r--   0        0        0      863 2024-04-04 10:11:34.029819 monthify-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 monthify-0.4.9/PKG-INFO
```

### Comparing `monthify-0.4.8/README.md` & `monthify-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/__init__.py` & `monthify-0.4.9/monthify/__init__.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/args.py` & `monthify-0.4.9/monthify/args.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/auth.py` & `monthify-0.4.9/monthify/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,12 +28,11 @@
         return spotipy.Spotify(
             retries=self.retries,
             requests_timeout=self.timeout,
             auth_manager=SpotifyOAuth(
                 client_id=self.client_id,
                 client_secret=self.client_secret,
                 redirect_uri=self.redirect_uri,
-                # scope=[str(scope) for scope in scopes],
                 scope=self.scopes,
                 cache_path=f"{self.location}/.cache",
             ),
         )
```

### Comparing `monthify-0.4.8/monthify/config.py` & `monthify-0.4.9/monthify/config.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/main.py` & `monthify-0.4.9/monthify/main.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/script.py` & `monthify-0.4.9/monthify/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Displays project name and current username
         """
 
         logger.info("Starting script execution")
         console.print(self.name, style="green")
         with console.status("Retrieving user information"):
             self.current_display_name = self.get_username()["display_name"]
-            self.current_username = self.get_username()["uri"][13:]
+            self.current_username = self.get_username()["id"]
         console.print(f"Username: [cyan]{self.current_display_name}[/cyan]\n")
 
     def update_last_run(self) -> None:
         """
         Updates last run time to current time
         """
 
@@ -170,36 +170,36 @@
         """
         Creates playlist with name var checking if the playlist already exists in the user's library,
         if it does the user is informed
         """
 
         sp = self.sp
         playlists = self.get_user_saved_playlists()
+        playlists = [normalize_text(item["name"]) for item in playlists]
         created_playlists = []
         logger.info(f"Playlist creation called {name}")
         t0 = perf_counter()
         log = ""
 
         for item in playlists:
-            if normalize_text(item["name"]) == normalize_text(name):
+            if item == normalize_text(name):
                 log += f"Playlist {name} already exists"
                 self.already_created_playlists.add(name)
                 logger.info(f"Playlist already exists {name}")
                 logger.debug(f"Playlist creation took {perf_counter() - t0} s")
                 return log
 
         logger.debug(f"Playlist creation took {perf_counter() - t0} s")
-        log += "\n" f"Creating playlist {name}"
+        log += f"\nCreating playlist {name}"
         logger.info(f"Creating playlist {name}")
         playlist = sp.user_playlist_create(
             user=self.current_username, name=name, public=self.MAKE_PUBLIC, collaborative=False, description=f"{name}"
         )
         created_playlists.append(playlist)
-        log += "\n" f"Added {name} playlist"
-        log += "\n"
+        log += f"\nAdded {name} playlist\n"
         logger.info(f"Added {name} playlist")
         self.has_created_playlists = len(created_playlists) > 0
         return log
 
     def get_saved_track_info(self) -> None:
         """
         Calls the get_saved_track_gen function at program's start to cache the user's saved tracks
@@ -248,14 +248,15 @@
             for month, year in self.playlist_names:
                 for item in playlists:
                     if normalize_text((month + " '" + year[2:])) == normalize_text(item["name"]):
                         self.playlist_names_with_id.append((month, year, item["id"]))
                         logger.info(
                             "Playlist name: {name} id: {id}", name=str(month + " '" + year[2:]), id=str(item["id"])
                         )
+        self.playlist_names_with_id = [*set(self.playlist_names_with_id)]
 
     def skip(self, status: bool, playlists: Optional[Iterable] = None) -> None:
         """
         Skips playlist generation if status is True
         """
 
         if status is True:
@@ -292,15 +293,15 @@
         if has_month_passed and self.already_created_playlists_exists is False:
             self.skip(False, spotify_playlists)
         elif not has_month_passed and self.already_created_playlists_exists:
             monthly_ran = True
 
         if self.CREATE_PLAYLIST is False:
             if self.SKIP_PLAYLIST_CREATION is False and monthly_ran is False:
-                console.print("Playlist generation has not occured this month, Generating Playlists...")
+                console.print("Playlist generation has not occurred this month, Generating Playlists...")
                 logger.info("Requesting playlist creation")
                 self.skip(False, spotify_playlists)
 
             elif self.SKIP_PLAYLIST_CREATION is False and monthly_ran is True:
                 console.print(
                     "Playlist generation has already occurred this month, do you still want to generate "
                     "playlists? (yes/no)"
@@ -378,20 +379,20 @@
                 self.sp.playlist_add_items(playlist_id=playlist_id, items=chunk)
             log += "\n"
             self.total_tracks_added += len(to_be_added_uris)
 
         logger.info("Ended track addition")
         return log
 
-    def sort_tracks_by_month(self, playlist: List[Tuple[str, str, str]]) -> List[str]:
+    def sort_tracks_by_month(self, playlist: Tuple[str, str, str]) -> List[str]:
         month, year, playlist_id = playlist
         playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
         playlist_name = f"{month} '{year[2:]}"
         logger.info("Sorting into playlist: {playlist}", playlist=playlist_name)
-        log = []
+        log: list[str] = []
 
         tracks = tuple(track for track in self.get_saved_track_gen() if track.track_month == (month, year))
         if not tracks:
             return log
         else:
             log.append(f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]")
             log.append("\t\n")
```

### Comparing `monthify-0.4.8/monthify/track.py` & `monthify-0.4.9/monthify/track.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.8/monthify/utils.py` & `monthify-0.4.9/monthify/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,30 +46,7 @@
 def strIsGreater(a: str, b: str) -> bool:
     """
     Compare two strings by summing their ascii values
     """
     if sum(ord(c) for c in a.lower()) > sum(ord(c) for c in b.lower()):
         return True
     return False
-
-
-def search_normalized(dataset: Iterable[str], target: str) -> bool:
-    """
-    Binary search for target in dataset
-    """
-    low = 0
-    high = len(dataset) - 1
-    sorted_dataset = sorted(dataset, key=lambda a: sum(ord(c) for c in a.lower()))
-
-    while low <= high:
-        mid = (high + low) // 2
-        guess = sorted_dataset[mid]
-
-        if normalize_text(guess) == normalize_text(target):
-            return True
-
-        if strIsGreater(guess, target):
-            high = mid - 1
-        else:
-            low = mid + 1
-
-    return False
```

### Comparing `monthify-0.4.8/pyproject.toml` & `monthify-0.4.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "monthify"
-version = "0.4.8"
+version = "0.4.9"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
 cachetools = "^5.2.1"
 rich = "^13.1.0"
 spotipy = "^2.22.0"
 appdirs = "^1.4.4"
 toml = "^0.10.2"
+algorithms = "^0.1.4"
 
 [tool.poetry.group.dev.dependencies]
 icecream = "^2.1.3"
 pynvim = "^0.4.3"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 types-requests = "^2.31.0.0"
 types-toml = "^0.10.8.6"
 types-appdirs = "^1.4.3.5"
 mypy = "^1.3.0"
 types-cachetools = "^5.3.0.5"
+pytest-mypy = "^0.10.3"
 
 [tool.poetry.scripts]
 monthify = "monthify.main:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `monthify-0.4.8/PKG-INFO` & `monthify-0.4.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.4.8
+Version: 0.4.9
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: algorithms (>=0.1.4,<0.2.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: cachetools (>=5.2.1,<6.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: rich (>=13.1.0,<14.0.0)
 Requires-Dist: spotipy (>=2.22.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
```


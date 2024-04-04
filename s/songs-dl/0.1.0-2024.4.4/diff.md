# Comparing `tmp/songs-dl-0.1.0.tar.gz` & `tmp/songs-dl-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songs-dl-0.1.0.tar", last modified: Fri Jun  9 11:43:40 2023, max compression
+gzip compressed data, was "songs-dl-2024.4.4.tar", last modified: Thu Apr  4 13:28:19 2024, max compression
```

## Comparing `songs-dl-0.1.0.tar` & `songs-dl-2024.4.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 11:43:40.322092 songs-dl-0.1.0/
--rw-rw-rw-   0        0        0     1235 2023-03-26 16:13:26.000000 songs-dl-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2397 2023-06-09 11:43:40.318684 songs-dl-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-09 11:43:10.000000 songs-dl-0.1.0/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-09 11:40:26.000000 songs-dl-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 11:43:40.323095 songs-dl-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 11:43:40.285172 songs-dl-0.1.0/songs_dl/
--rw-rw-rw-   0        0        0     8053 2023-06-09 11:33:15.000000 songs-dl-0.1.0/songs_dl/__init__.py
--rw-rw-rw-   0        0        0      332 2023-06-08 14:06:52.000000 songs-dl-0.1.0/songs_dl/__main__.py
--rw-rw-rw-   0        0        0     7024 2023-06-09 11:32:56.000000 songs-dl-0.1.0/songs_dl/deezer.py
--rw-rw-rw-   0        0        0     2537 2023-06-09 11:37:15.000000 songs-dl-0.1.0/songs_dl/itunes.py
--rw-rw-rw-   0        0        0      556 2023-06-09 11:37:42.000000 songs-dl-0.1.0/songs_dl/monkeypatch_requests.py
--rw-rw-rw-   0        0        0     4383 2023-06-09 11:33:15.000000 songs-dl-0.1.0/songs_dl/spotify.py
--rw-rw-rw-   0        0        0    18081 2023-06-09 11:34:55.000000 songs-dl-0.1.0/songs_dl/utils.py
--rw-rw-rw-   0        0        0     6008 2023-06-09 11:33:15.000000 songs-dl-0.1.0/songs_dl/youtube.py
--rw-rw-rw-   0        0        0     1584 2023-06-09 11:36:54.000000 songs-dl-0.1.0/songs_dl/youtube_dl.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:43:40.313662 songs-dl-0.1.0/songs_dl.egg-info/
--rw-rw-rw-   0        0        0     2397 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 11:43:40.000000 songs-dl-0.1.0/songs_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:28:19.143123 songs-dl-2024.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-04 13:28:19.143123 songs-dl-2024.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:28:19.143123 songs-dl-2024.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:28:19.139124 songs-dl-2024.4.4/songs_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/deezer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/itunes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/monkeypatch_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/musixmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/print_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20953 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-04 13:27:07.000000 songs-dl-2024.4.4/songs_dl/youtube_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:28:19.139124 songs-dl-2024.4.4/songs_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 13:28:19.000000 songs-dl-2024.4.4/songs_dl.egg-info/top_level.txt
```

### Comparing `songs-dl-0.1.0/LICENSE` & `songs-dl-2024.4.4/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org>
```

### Comparing `songs-dl-0.1.0/songs_dl/itunes.py` & `songs-dl-2024.4.4/songs_dl/itunes.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import logging
-from threading import Lock
-from typing import Any
-
-import requests
-
-from .utils import Picture, PictureProvider, Song, format_query, get, locked
-
-logger = logging.getLogger(__name__)
-itunes_lock = Lock()
-
-
-class ItunesPictureProvider(PictureProvider):
-    def get_sure_pictures(self, result: dict[str, Any]):
-        # TODO add debug information
-        pictures: list[Picture] = []
-
-        for key, value in result.items():
-            if key.startswith("artworkUrl"):
-                try:
-                    pictures.append(Picture(value, int(key.removeprefix("artworkUrl"))))
-                except ValueError:  # invalid number
-                    pass
-
-        return pictures
-
-
-def download_itunes(song: str, artist: str | None = None, market: str | None = None):
-    """
-    Fetch the iTunes search results.
-    """
-    logger.info("Searching %s on iTunes...", format_query(song, artist, market))
-    if artist:
-        query = song + " " + artist
-    else:
-        query = song
-    params = {"term": query, "entity": "song"}
-    if market:
-        params["country"] = market
-    req = locked(itunes_lock)(requests.get)("https://itunes.apple.com/search", params=params)
-    try:
-        # decode the JSON data
-        search = req.json()
-        logger.debug("JSON decoding OK")
-    except requests.exceptions.JSONDecodeError as err:
-        # we skip iTunes
-        logger.debug("JSON decoding error: %s", err)
-        return []
-
-    results = get(search, "results", list[dict[str, Any]])
-    if len(results) == 0:
-        logger.debug("No 'results' index")
-        return []  # same thing
-
-    ret: list[Song] = []
-
-    for result in results:
-        ret.append(
-            Song(
-                title=get(result, "trackName", str),
-                artists=[get(result, "artistName", str)],
-                album=get(result, "collectionName", str),
-                duration=get(result, "trackTimeMillis", int) / 1000,
-                language=get(result, "country", str).lower(),
-                genre=get(result, "primaryGenreName", str),
-                track_number=(
-                    get(result, "trackNumber", int),
-                    get(result, "trackCount", int),
-                ),
-                release_date=get(result, "releaseDate", str),
-                # picture = Picture(image, taille) if image and taille else None,
-                picture=ItunesPictureProvider(result),
-            )
-        )
-
-    return ret
+import logging
+from threading import Lock
+from typing import Any
+
+import requests
+
+from .utils import Picture, PictureProvider, Song, format_query, get, locked
+
+logger = logging.getLogger(__name__)
+itunes_lock = Lock()
+
+
+class ItunesPictureProvider(PictureProvider):
+    def get_sure_pictures(self, result: dict[str, Any]):
+        # TODO add debug information
+        pictures: list[Picture] = []
+
+        for key, value in result.items():
+            if key.startswith("artworkUrl"):
+                try:
+                    pictures.append(Picture(value, int(key.removeprefix("artworkUrl"))))
+                except ValueError:  # invalid number
+                    pass
+
+        return pictures
+
+
+def download_itunes(song: str, artist: str | None = None, market: str | None = None):
+    """
+    Fetch the iTunes search results.
+    """
+    logger.info("Searching %s on iTunes...", format_query(song, artist, market))
+    if artist:
+        query = song + " " + artist
+    else:
+        query = song
+    params = {"term": query, "entity": "song"}
+    if market:
+        params["country"] = market
+    req = locked(itunes_lock)(requests.get)("https://itunes.apple.com/search", params=params)
+    try:
+        # decode the JSON data
+        search = req.json()
+        logger.debug("JSON decoding OK")
+    except requests.exceptions.JSONDecodeError as err:
+        # we skip iTunes
+        logger.debug("JSON decoding error: %s", err)
+        return []
+
+    results = get(search, "results", list[dict[str, Any]])
+    if len(results) == 0:
+        logger.debug("No 'results' index")
+        return []  # same thing
+
+    ret: list[Song] = []
+
+    for result in results:
+        ret.append(
+            Song(
+                title=get(result, "trackName", str),
+                artists=[get(result, "artistName", str)],
+                album=get(result, "collectionName", str),
+                duration=get(result, "trackTimeMillis", int) / 1000,
+                language=get(result, "country", str).lower(),
+                genre=get(result, "primaryGenreName", str),
+                track_number=(
+                    get(result, "trackNumber", int),
+                    get(result, "trackCount", int),
+                ),
+                release_date=get(result, "releaseDate", str),
+                # picture = Picture(image, taille) if image and taille else None,
+                picture=ItunesPictureProvider(result),
+            )
+        )
+
+    return ret
```

### Comparing `songs-dl-0.1.0/songs_dl/spotify.py` & `songs-dl-2024.4.4/songs_dl/spotify.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import logging
-from pprint import pformat
-from threading import Lock
-from time import time
-from typing import TypedDict
-
-import requests
-
-from .utils import Picture, PictureProvider, Song, format_query, get, locked
-
-logger = logging.getLogger(__name__)
-spotify_lock = Lock()
-
-
-class SpotifyAccessToken(TypedDict):
-    """
-    Spotify access token (on Spotify).
-    """
-
-    accessToken: str
-    accessTokenExpirationTimestampMs: int
-
-
-class AccessToken(TypedDict):
-    """
-    Spotify access token for the `get_access_token` function
-    """
-
-    token: str
-    expiration: int
-
-
-class SpotifyArtist(TypedDict):
-    name: str
-
-
-class SpotifyImage(TypedDict):
-    width: int
-    height: int
-    url: str
-
-
-class SpotifyAlbum(TypedDict):
-    name: str
-    images: list[SpotifyImage]
-
-
-class SpotifyTrack(TypedDict):
-    name: str
-    artists: list[SpotifyArtist]
-    album: SpotifyAlbum
-    duration_ms: int
-
-
-class SpotifyTracks(TypedDict):
-    items: list[SpotifyTrack]
-
-
-class SpotifyData(TypedDict):
-    tracks: SpotifyTracks
-
-
-ACCESS_TOKEN = ""
-ACCESS_TOKEN_EXPIRATION = 0
-
-
-def get_access_token():
-    """
-    Get the Spofity access token
-    """
-    global ACCESS_TOKEN, ACCESS_TOKEN_EXPIRATION
-    # we don't need "global" statement (we edit the keys)
-    if not ACCESS_TOKEN_EXPIRATION or ACCESS_TOKEN_EXPIRATION < time():
-        logger.info("Getting Spotify access token...")
-        req = locked(spotify_lock)(requests.get)("https://open.spotify.com/get_access_token")
-
-        try:
-            result = req.json()
-            logger.debug("JSON decoding OK")
-        except requests.JSONDecodeError as err:
-            logger.debug("JSON decoding error: %s", err)
-            return ""
-
-        if not result["accessToken"]:
-            logger.error("Can't get the Spotify access token!")
-            return ""
-
-        ACCESS_TOKEN_EXPIRATION = get(result, "accessTokenExpirationTimestampMs", int) or int(
-            time() + 30 * 60
-        )  # 30 minutes
-
-        ACCESS_TOKEN = result["accessToken"]
-
-    return ACCESS_TOKEN
-
-
-class SpotifyPictureProvider(PictureProvider):
-    """
-    Picture provider for Spotify.
-    """
-
-    def get_sure_pictures(self, result):
-        pictures = get(result, ("album", "images"), list)
-        return [
-            Picture(
-                get(picture, "url", str),
-                get(picture, "width", int),
-                get(picture, "height", int),
-            )
-            for picture in pictures
-        ]
-
-    def get_url_for_size(self, size):
-        return None  # the Spotify URLs are hash-based
-
-
-def download_spotify(song: str, artist: str | None = None, market: str | None = None):
-    """
-    Fetch the Spotify search results.
-    """
-    access_token = get_access_token()
-    if not access_token:
-        logger.error("No access token: stop Spotify search")
-        return []
-
-    logger.info("Searching %s on Spotify...", format_query(song, artist, market))
-    params = {
-        "q": f"track:{song}" + (f" artist:{artist}" if artist else ""),
-        "type": "track",
-    }
-    if market:
-        params["market"] = market
-    req = locked(spotify_lock)(requests.get)(
-        "https://api.spotify.com/v1/search",
-        params=params,
-        headers={"Authorization": f"Bearer {access_token}"},
-    )
-
-    try:
-        result = req.json()
-        logger.debug("JSON decoding OK")
-    except requests.exceptions.JSONDecodeError as err:
-        # we skip Spotify
-        logger.debug("JSON decoding error: %s", err)
-        return []
-
-    # result = validate_schema(SpotifyData, result)
-
-    ret: list[Song] = []
-    for element in result.get("tracks", {}).get("items", []):
-        ret.append(
-            Song(
-                title=get(element, "name", str),
-                artists=[get(artist, "name", str) for artist in element.get("artists", {})],
-                album=get(element.get("album", {}), "name", str),
-                duration=get(element, "duration_ms", int) / 1000,
-                isrc=get(element, ("external_ids", "isrc"), str),
-                picture=SpotifyPictureProvider(element),
-                # TODO add other elements?
-            )
-        )
-
-    logger.debug("Results:\n%s", pformat(ret))
-
-    return ret
+import logging
+from pprint import pformat
+from threading import Lock
+from time import time
+from typing import TypedDict
+
+import requests
+
+from .utils import Picture, PictureProvider, Song, format_query, get, locked
+
+logger = logging.getLogger(__name__)
+spotify_lock = Lock()
+
+
+class SpotifyAccessToken(TypedDict):
+    """
+    Spotify access token (on Spotify).
+    """
+
+    accessToken: str
+    accessTokenExpirationTimestampMs: int
+
+
+class AccessToken(TypedDict):
+    """
+    Spotify access token for the `get_access_token` function
+    """
+
+    token: str
+    expiration: int
+
+
+class SpotifyArtist(TypedDict):
+    name: str
+
+
+class SpotifyImage(TypedDict):
+    width: int
+    height: int
+    url: str
+
+
+class SpotifyAlbum(TypedDict):
+    name: str
+    images: list[SpotifyImage]
+
+
+class SpotifyTrack(TypedDict):
+    name: str
+    artists: list[SpotifyArtist]
+    album: SpotifyAlbum
+    duration_ms: int
+
+
+class SpotifyTracks(TypedDict):
+    items: list[SpotifyTrack]
+
+
+class SpotifyData(TypedDict):
+    tracks: SpotifyTracks
+
+
+ACCESS_TOKEN = ""
+ACCESS_TOKEN_EXPIRATION = 0
+
+
+def get_access_token():
+    """
+    Get the Spofity access token
+    """
+    global ACCESS_TOKEN, ACCESS_TOKEN_EXPIRATION
+    # we don't need "global" statement (we edit the keys)
+    if not ACCESS_TOKEN_EXPIRATION or ACCESS_TOKEN_EXPIRATION < time():
+        logger.info("Getting Spotify access token...")
+        req = locked(spotify_lock)(requests.get)("https://open.spotify.com/get_access_token")
+
+        try:
+            result = req.json()
+            logger.debug("JSON decoding OK")
+        except requests.JSONDecodeError as err:
+            logger.debug("JSON decoding error: %s", err)
+            return ""
+
+        if not result["accessToken"]:
+            logger.error("Can't get the Spotify access token!")
+            return ""
+
+        ACCESS_TOKEN_EXPIRATION = get(result, "accessTokenExpirationTimestampMs", int) or int(
+            time() + 30 * 60
+        )  # 30 minutes
+
+        ACCESS_TOKEN = result["accessToken"]
+
+    return ACCESS_TOKEN
+
+
+class SpotifyPictureProvider(PictureProvider):
+    """
+    Picture provider for Spotify.
+    """
+
+    def get_sure_pictures(self, result):
+        pictures = get(result, ("album", "images"), list)
+        return [
+            Picture(
+                get(picture, "url", str),
+                get(picture, "width", int),
+                get(picture, "height", int),
+            )
+            for picture in pictures
+        ]
+
+    def get_url_for_size(self, size):
+        return None  # the Spotify URLs are hash-based
+
+
+def download_spotify(song: str, artist: str | None = None, market: str | None = None):
+    """
+    Fetch the Spotify search results.
+    """
+    access_token = get_access_token()
+    if not access_token:
+        logger.error("No access token: stop Spotify search")
+        return []
+
+    logger.info("Searching %s on Spotify...", format_query(song, artist, market))
+    params = {
+        "q": f"track:{song}" + (f" artist:{artist}" if artist else ""),
+        "type": "track",
+    }
+    if market:
+        params["market"] = market
+    req = locked(spotify_lock)(requests.get)(
+        "https://api.spotify.com/v1/search",
+        params=params,
+        headers={"Authorization": f"Bearer {access_token}"},
+    )
+
+    try:
+        result = req.json()
+        logger.debug("JSON decoding OK")
+    except requests.exceptions.JSONDecodeError as err:
+        # we skip Spotify
+        logger.debug("JSON decoding error: %s", err)
+        return []
+
+    # result = validate_schema(SpotifyData, result)
+
+    ret: list[Song] = []
+    for element in result.get("tracks", {}).get("items", []):
+        ret.append(
+            Song(
+                title=get(element, "name", str),
+                artists=[get(artist, "name", str) for artist in element.get("artists", {})],
+                album=get(element.get("album", {}), "name", str),
+                duration=get(element, "duration_ms", int) / 1000,
+                isrc=get(element, ("external_ids", "isrc"), str),
+                picture=SpotifyPictureProvider(element),
+                # TODO add other elements?
+            )
+        )
+
+    logger.debug("Results:\n%s", pformat(ret))
+
+    return ret
```

### Comparing `songs-dl-0.1.0/songs_dl/utils.py` & `songs-dl-2024.4.4/songs_dl/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,584 +1,704 @@
-"""
-Utilitary functions.
-"""
-import datetime as dt
-import functools
-import logging
-import re
-from threading import Lock
-from typing import Any, Callable, Literal, Required, Sequence, Type, TypedDict, TypeVar, Union, get_origin, overload
-
-import requests
-from rapidfuzz import fuzz
-from unidecode import unidecode as unidecode_py
-from yt_dlp.utils import traverse_obj
-
-Self = TypeVar("Self")
-
-logger = logging.getLogger(__name__)
-
-AnyDictKey = TypeVar("AnyDictKey")
-AnyT = TypeVar("AnyT")
-
-
-def merge_dicts(
-    *args: Union[dict[AnyDictKey, AnyT], TypedDict], merge_lists: bool | None = False
-) -> dict[AnyDictKey, list[AnyT]]:
-    """
-    Merge many dicts and return a dict with arrays containing all values.
-
-    `merge_list` :
-    - `True` -> all the elements must be lists (list/tuple) and are concatenated
-    - `False` -> all the elements are added as is
-    - `None` -> `True` for the element that are lists and `False` for the other elements
-
-    >>> merge_dicts({"a": "b"}, {"x": "y"}, {"a": "c"}, {"x": ["z", "Z"]}, merge_lists = None)
-    {"a": ["b", "c"], "x": ["y", "z", "Z"]}
-    """
-    ret = {}
-    for arg in args:
-        for key, value in arg.items():
-            if value:
-                if ret.get(key) is None:
-                    ret[key] = []
-                if merge_lists is None:
-                    if not isinstance(value, list) and not isinstance(value, tuple):
-                        value = [value]
-                elif merge_lists is False:
-                    value = [value]
-                else:
-                    if not isinstance(value, list) and not isinstance(value, tuple):
-                        raise ValueError(f"The value {key!r}: {value!r} is not a list")
-                ret[key].append(*value)
-    return ret
-
-
-ExpectedT = TypeVar("ExpectedT")
-
-
-def get_base_type(candidate):
-    """
-    Return the base type of a type.
-
-    >>> get_base_type(list)
-    <class 'list'>
-    >>> get_base_type(list[str])
-    <class 'list'>
-    """
-    origin = get_origin(candidate)
-    if origin:
-        return origin
-    if not isinstance(candidate, type):
-        return type(candidate)
-    return candidate
-
-
-@overload
-def get(obj: Any, paths: Any, expected: Callable[[Any], ExpectedT]) -> ExpectedT:
-    ...
-
-
-@overload
-def get(obj: Any, paths: Any, expected: Type[ExpectedT]) -> ExpectedT:
-    ...
-
-
-@overload
-def get(obj: Any, paths: Any, expected: ExpectedT) -> ExpectedT:
-    ...
-
-
-@overload
-def get(
-    obj: dict[str, Any] | Sequence[Any],
-    *paths: Any,
-    expected: Callable[[Any], ExpectedT],
-) -> ExpectedT:
-    ...
-
-
-@overload
-def get(obj: dict[str, Any] | Sequence[Any], *paths: Any, expected: Type[ExpectedT]) -> ExpectedT:
-    ...
-
-
-@overload
-def get(obj: dict[str, Any] | Sequence[Any], *paths: Any, expected: ExpectedT) -> ExpectedT:
-    ...
-
-
-@overload
-def get(obj: dict[str, Any] | Sequence[Any], *paths: Any, expected: None = ...) -> Any:
-    ...
-
-
-def get(obj, *paths, expected=None, **kwargs):
-    """
-    Safely traverse nested `dict`s and `Sequence`s.
-
-    Work around to force the return value to have the correct type.
-
-    See `yt_dlp.utils.traverse_obj` docstring for more information.
-    """
-    expected_type = kwargs.pop("expected_type", None)
-    expected = expected or expected_type
-    if not expected and (get_base_type(paths[-1]) or callable(paths[:-1])):
-        expected = paths[-1]
-        paths = paths[:-1]
-    if expected:
-        expected = get_base_type(expected)
-    ret = traverse_obj(
-        obj,
-        *paths,
-        expected_type=lambda val: expected(val) if expected else None,  # pylint: disable=W0108
-        **kwargs,
-    )
-    if ret is None and expected:
-        return instantiate(expected)
-    return ret
-
-
-def instantiate(target_type: Type[ExpectedT] | Callable[[Any], ExpectedT]) -> ExpectedT | None:
-    """
-    Return an empty instance of the given type/function or `None` if it's not possible.
-    """
-    if target_type is dt.date:
-        target_type = dt.date.fromisoformat  # type: ignore
-
-    target_type = get_base_type(target_type)
-
-    for args in [
-        (),
-        (""),
-        (0),
-    ]:
-        try:
-            return target_type(*args)  # type: ignore
-        except:  # noqa
-            pass
-
-    return None
-
-
-def fuzz_wrapper(func):
-    """
-    Decorator for `rapidfuzz` functions: work around emojis that cause bugs.
-    """
-
-    @functools.wraps(func)
-    def wrapper(str1: str, str2: str, score_cutoff: float = 0):
-        try:
-            return func(str1, str2, score_cutoff)
-        except:  # noqa
-            # we build new strings that contain only alphanumerical characters and spaces
-            # and return the partial_ratio of that
-            new_str1 = "".join(each_letter for each_letter in str1 if each_letter.isalnum() or each_letter.isspace())
-            new_str2 = "".join(each_letter for each_letter in str2 if each_letter.isalnum() or each_letter.isspace())
-            return func(new_str1, new_str2, score_cutoff=score_cutoff)
-
-    return wrapper
-
-
-_ratio = fuzz_wrapper(fuzz.ratio)
-_partial_ratio = fuzz_wrapper(fuzz.partial_ratio)
-
-
-class Picture:
-    """
-    A picture (album art) on a website.
-    """
-
-    CHUNK_SIZE = 64 * 1024
-
-    def __init__(self, url: str, width: int, height: int = 0, sure=True):
-        self.url = url
-        self.width = width
-        self.height = height or width
-        self.data: Literal[False] | bytes | None = None
-        self.sure = sure
-        self.req: requests.Response | None = None
-
-    @property
-    def size(self):
-        """
-        Size of the image (smallest dimension).
-        """
-        return min(self.width, self.height)
-
-    def check(self):
-        """
-        Check if the picture exists (without downloading it, if possible).
-        """
-        if self.sure:
-            return True
-        logger.debug("Checking picture '%s'...", self.url)
-        # don't download the picture, just the headers
-        req = requests.head(self.url, stream=True)
-        try:
-            req.raise_for_status()
-            self.sure = True
-        except requests.exceptions.HTTPError as err:
-            logger.debug("HTTP error: %s...", err)
-            self.sure = False
-        return self.sure
-
-    def download(self) -> Literal[False] | bytes:
-        """
-        Download the picture.
-        """
-        if self.data is not None:
-            return self.data
-
-        # download the picture
-        logger.debug("Downloading picture '%s'...", self.url)
-
-        self.data = b""
-
-        try:
-            # don't download the page if there is an error
-            self.req = requests.get(self.url, stream=True)
-            self.req.raise_for_status()
-            self.data = self.req.content
-        except requests.exceptions.HTTPError as err:
-            logger.debug("HTTP error: %s...", err)
-            self.data = False
-
-        logger.debug("Picture downloaded")
-        return self.data
-
-    def __repr__(self):
-        return f"<Picture {self.size}x{self.size} {'sure' if self.sure else 'not sure'} at {self.url}>"
-
-
-class PictureProvider:
-    """
-    Class for listing and downloading the images of a website.
-    """
-
-    pictures: list[Picture]
-
-    def __init__(self, result: dict[str, Any]):
-        self.provider_urls = {pic.size: pic for pic in self.get_sure_pictures(result)}
-
-        self.pictures = self.get_sure_pictures(result)
-
-        if not self.pictures:
-            return
-
-        sizes_to_try = [1200, 1000, 800, 500, 300]
-
-        for size in sizes_to_try:
-            if not any(pic.size == size for pic in self.pictures):
-                url = self.get_url_for_size(size)
-                if url:
-                    self.pictures.append(Picture(url, size, sure=False))
-
-        self.pictures.sort(key=lambda pic: pic.size, reverse=True)
-
-    def get_sure_pictures(self, result: dict[str, Any]) -> list[Picture]:
-        """
-        Return a list of all the sure pictures.
-        """
-        raise NotImplementedError
-
-    def get_url_for_size(self, size: int) -> str | None:
-        """
-        Return a probably valid URL for the given size.
-        """
-        first = self.pictures[0]
-        first_size = first.size
-        picture = first.url
-
-        url_parts = picture.split("/")
-        url_parts[-1] = url_parts[-1].replace(str(first_size), str(size))
-        return "/".join(url_parts)
-
-    def get_pictures(self):
-        return self.pictures
-
-    def get_best_picture(self):
-        return self.pictures[0]
-
-
-class TagsList(TypedDict, total=False):
-    TIT2: Required[str]
-    TPE1: Required[str]
-    TALB: str
-    TLEN: str
-    TCOM: str
-    TYER: str
-    TDAT: str
-    TIME: str
-    COMM: str
-    TSRC: str
-    TRCK: str
-    TCOP: str
-    TLAN: str
-    TCON: str
-    USLT: str
-    SYLT: list[tuple[str, int]]
-    APIC: Picture | None
-
-
-class Song:
-    """
-    A song.
-    """
-
-    def __init__(
-        self,
-        *,
-        title: str = "",
-        artists: list[str] | tuple[str, ...] = (),
-        album: str | None = None,
-        duration: float = 0,
-        language: str | None = None,
-        genre: str | None = None,
-        composers: list[str] | None = None,
-        release_date: str | dt.date | None = None,
-        isrc: str | None = None,
-        track_number: int | tuple[int, int | None] | None = None,
-        copyright: str | None = None,  # pylint: disable=W0622
-        lyrics: str | list[tuple[str, float]] | None = None,
-        picture: Picture | PictureProvider | None = None,
-        comments: str | None = None,
-    ):
-        self.title = title
-        self.artists = list(artists)
-        self.album = album
-        self.duration = duration
-        self.language = language
-        self.genre = genre
-        self.composers = composers
-        if isinstance(release_date, str):
-            try:
-                self.release_date = dt.datetime.fromisoformat(release_date)
-            except ValueError:
-                self.release_date = None
-        else:
-            self.release_date = release_date
-        self.isrc = isrc
-        self.track_number = (track_number, None) if isinstance(track_number, int) else track_number
-        self.copyright = copyright
-        self.lyrics = lyrics
-        self.picture = picture
-        self.comments = comments
-
-    @classmethod
-    def empty(cls):
-        """
-        Return an empty song for placeholder purposes.
-        """
-        return cls()
-
-    def __not__(self):
-        return not self.title and not self.artists
-
-    def to_id3(self) -> TagsList:
-        """
-        Return the ID3 tags for a song.
-        """
-        if not self:
-            return {"TIT2": "", "TPE1": ""}
-        r_date = self.release_date
-        if not r_date:
-            year = date = time = ""
-        else:
-
-            def test_value(value: str):
-                return "" if not int(value) else value  # avoid "0000" for example...
-
-            year = test_value(f"{r_date:%Y}")  # YYYY
-            date = test_value(f"{r_date:%d%m}")  # DDMM
-            time = test_value(f"{r_date:%H%M}")  # HHMM
-
-        def format_lrc_timestamp(timestamp: float):
-            return f"[{int(timestamp // 60):02d}:{timestamp % 60:05.2f}]"
-
-        ret: TagsList = {
-            "TIT2": self.title,
-            "TPE1": ", ".join(self.artists),
-            "TALB": self.album or "",
-            "TLEN": str(self.duration * 1000) if self.duration is not None else "",
-            "TCOM": ", ".join(self.composers) if self.composers else "",
-            "TYER": year,
-            "TDAT": date,
-            "TIME": time,
-            "TSRC": self.isrc or "",
-            "TRCK": (
-                "/".join(str(n) for n in self.track_number)
-                if isinstance(self.track_number, tuple)
-                else str(self.track_number)
-            )
-            if self.track_number
-            else "",
-            "TCOP": self.copyright or "",
-            "TLAN": self.language or "",
-            "TCON": self.genre or "",
-            "USLT": "\n".join((format_lrc_timestamp(ts) + line if line else "") for line, ts in self.lyrics)
-            if isinstance(self.lyrics, list)
-            else (self.lyrics or ""),
-            "SYLT": [(line[0], int(line[1] * 1000)) for line in self.lyrics] if isinstance(self.lyrics, list) else [],
-            "APIC": self.picture.get_best_picture() if isinstance(self.picture, PictureProvider) else self.picture,
-            "COMM": self.comments or "",
-        }
-        return ret
-
-    def __repr__(self):
-        return f"<Song '{self.title}' by {', '.join(self.artists)} album {self.album} {self.duration} s>"
-
-
-def _get_sentence_words(string: str):
-    """
-    Get all the words in a sentence.
-    """
-    return re.findall(r"\w+", unidecode(string.lower()))
-
-
-def _normalize_sentence(string: str):
-    """
-    Return a sentence without punctuation, without brackets and lowercased.
-    """
-    return " ".join(_get_sentence_words(re.sub(r"(?i)\(.*?\)|-.*|feat", "", string)))
-
-
-def get_provider_name(provider: str):
-    """
-    Return the human name of a provider.
-    """
-    return {"itunes": "iTunes", "youtube": "YouTube"}.get(provider, provider.title())
-
-
-def order_results(provider: str, results: list[Song], other_results: dict[str, list[Song]] | None):
-    """
-    Order the results: choose the result that is the most similar to the Spotify / Deezer song.
-    """
-    if not other_results:
-        return results
-
-    spotify_song = other_results["spotify"][0]
-    deezer_song = other_results["spotify"][0]
-
-    ret: list[tuple[Song, float, list[float]]] = []
-
-    for result in results:
-        # check for common word
-        sp_title_words = _get_sentence_words(spotify_song.title)
-
-        if not any(word in _get_sentence_words(result.title) for word in sp_title_words):
-            # if there are no common words, skip result
-            continue
-
-        # Find artist match
-        # match = (no of artist names in result) / (no of artist names on spotify) * 100
-        artist_match_number = 0
-
-        all_r_artists = _normalize_sentence(" ".join(result.artists))
-
-        artist_match_number = sum(
-            1 if _partial_ratio(_normalize_sentence(sp_artist), all_r_artists, 85) else 0
-            for sp_artist in spotify_song.artists
-        )
-
-        artist_match = (artist_match_number / len(spotify_song.artists)) * 100
-
-        # Skip if there are no artists in common
-        if artist_match_number == 0:
-            continue
-
-        name_match = _ratio(
-            str(unidecode(spotify_song.title.lower())),
-            str(unidecode(result.title.lower())),
-            60,
-        )
-
-        official_match = (
-            len(
-                re.findall(
-                    r"(?i)(\b[ou]ffi[cz]i[ae]l|_off\b|\btopic\b)",
-                    result.title + " " + all_r_artists,
-                )
-            )
-            * 50
-        )
-        if not official_match and hasattr(result, "youtube_video"):
-            official_match += (
-                100 if "BADGE_STYLE_TYPE_VERIFIED_ARTIST" in result.youtube_video["badges"] else 0  # type: ignore
-            )
-        if official_match:
-            official_match += len(re.findall(r"(?i)\baudio\b", result.title)) * 100
-
-        if deezer_song.copyright:
-            copyright_match = 80 + (_normalize_sentence(deezer_song.copyright) in all_r_artists) * 20
-        else:
-            copyright_match = 100
-
-        delta = max(abs(result.duration - spotify_song.duration) - 4, 0)
-        non_match_value = delta**2 / spotify_song.duration * 100
-
-        time_match = max(100 - non_match_value, 0)
-
-        discard_match = len(re.findall(r"(?i)\d+ h(?:our)\b|\b8d audio\b", result.title)) * -100
-
-        # the average match is rounded for debugging
-        average_match = round(
-            (artist_match + name_match + official_match * 2 + copyright_match * 2 + time_match * 3 + discard_match * 2)
-            / 9,
-            ndigits=3,
-        )
-
-        # the results along with the average match
-        ret.append(
-            (
-                result,
-                average_match,
-                [artist_match, name_match, official_match, copyright_match, time_match],
-            )
-        )
-
-    ret = sorted(ret, key=lambda el: el[1], reverse=True)
-    logger.debug(
-        "%s sorted results:\n%s",
-        get_provider_name(provider),
-        "\n".join([f"{el[1]} ({' '.join(str(round(e, 3)) for e in el[2])}): {el[0]}" for el in ret]),
-    )
-    return [el[0] for el in ret]
-
-
-# for type checking
-def unidecode(string: str) -> str:
-    """
-    Transliterate an Unicode object into an ASCII string.
-    """
-    return unidecode_py(string)  # type: ignore
-
-
-AnyFunction = TypeVar("AnyFunction", bound=Callable)
-
-
-def locked(lock: Lock):
-    """
-    Acquire a lock before executing the function and release it after
-    (if the lock has already been released, don't do anything).
-    """
-
-    def decorator(f: AnyFunction) -> AnyFunction:
-        @functools.wraps(f)
-        def wrapper(*args, **kwargs):
-            lock.acquire()
-            try:
-                return f(*args, **kwargs)
-            finally:
-                if lock.locked():
-                    lock.release()
-
-        return wrapper  # type: ignore
-
-    return decorator
-
-
-def format_query(song: str, artist: str | None = None, market: str | None = None):
-    """
-    Return a formatted version of `song`, `artist` and `market` (for logging).
-    """
-    return f"'{song}'" + (f" - '{artist}'" if artist else "") + (f" on '{market}' market" if market else "")
+"""
+Utilitary functions.
+"""
+
+import datetime as dt
+import functools
+import logging
+import re
+from io import BytesIO
+from threading import Lock
+from typing import Any, Callable, Literal, Required, Sequence, Type, TypedDict, TypeVar, Union, get_origin, overload
+
+import mutagen.id3
+import requests
+from rapidfuzz import fuzz
+from unidecode import unidecode as unidecode_py
+from yt_dlp.utils import traverse_obj
+
+Self = TypeVar("Self")
+
+logger = logging.getLogger(__name__)
+
+AnyDictKey = TypeVar("AnyDictKey")
+AnyT = TypeVar("AnyT")
+
+
+def merge_dicts(
+    *args: Union[dict[AnyDictKey, AnyT], TypedDict], merge_lists: bool | None = False
+) -> dict[AnyDictKey, list[AnyT]]:
+    """
+    Merge many dicts and return a dict with arrays containing all values.
+
+    `merge_list` :
+    - `True` -> all the elements must be lists (list/tuple) and are concatenated
+    - `False` -> all the elements are added as is
+    - `None` -> `True` for the element that are lists and `False` for the other elements
+
+    >>> merge_dicts({"a": "b"}, {"x": "y"}, {"a": "c"}, {"x": ["z", "Z"]}, merge_lists = None)
+    {"a": ["b", "c"], "x": ["y", "z", "Z"]}
+    """
+    ret = {}
+    for arg in args:
+        for key, value in arg.items():
+            if value:
+                if ret.get(key) is None:
+                    ret[key] = []
+                if merge_lists is None:
+                    if not isinstance(value, list) and not isinstance(value, tuple):
+                        value = [value]
+                elif merge_lists is False:
+                    value = [value]
+                else:
+                    if not isinstance(value, list) and not isinstance(value, tuple):
+                        raise ValueError(f"The value {key!r}: {value!r} is not a list")
+                ret[key].append(*value)
+    return ret
+
+
+ExpectedT = TypeVar("ExpectedT")
+
+
+def get_base_type(candidate):
+    """
+    Return the base type of a type.
+
+    >>> get_base_type(list)
+    <class 'list'>
+    >>> get_base_type(list[str])
+    <class 'list'>
+    """
+    origin = get_origin(candidate)
+    if origin:
+        return origin
+    if not isinstance(candidate, type):
+        return type(candidate)
+    return candidate
+
+
+@overload
+def get(obj: Any, paths: Any, expected: Callable[[Any], ExpectedT]) -> ExpectedT: ...
+
+
+@overload
+def get(obj: Any, paths: Any, expected: Type[ExpectedT]) -> ExpectedT: ...
+
+
+@overload
+def get(obj: Any, paths: Any, expected: ExpectedT) -> ExpectedT: ...
+
+
+@overload
+def get(
+    obj: dict[str, Any] | Sequence[Any],
+    *paths: Any,
+    expected: Callable[[Any], ExpectedT],
+) -> ExpectedT: ...
+
+
+@overload
+def get(obj: dict[str, Any] | Sequence[Any], *paths: Any, expected: Type[ExpectedT]) -> ExpectedT: ...
+
+
+@overload
+def get(obj: dict[str, Any] | Sequence[Any], *paths: Any, expected: ExpectedT) -> ExpectedT: ...
+
+
+@overload
+def get(obj: Any, *paths: Any, expected: None = ...) -> Any: ...
+
+
+def get(obj, *paths, expected=None, **kwargs):
+    """
+    Safely traverse nested `dict`s and `Sequence`s.
+
+    Work around to force the return value to have the correct type.
+
+    See `yt_dlp.utils.traverse_obj` docstring for more information.
+    """
+    expected_type = kwargs.pop("expected_type", None)
+    expected = expected or expected_type
+    if not expected and (get_base_type(paths[-1]) or callable(paths[:-1])):
+        expected = paths[-1]
+        paths = paths[:-1]
+    if expected:
+        expected = get_base_type(expected)
+    ret = traverse_obj(
+        obj,
+        *paths,
+        expected_type=lambda val: expected(val) if expected else None,  # pylint: disable=W0108
+        **kwargs,
+    )
+    if ret is None and expected:
+        return instantiate(expected)
+    return ret
+
+
+def instantiate(target_type: Type[ExpectedT] | Callable[[Any], ExpectedT]) -> ExpectedT | None:
+    """
+    Return an empty instance of the given type/function or `None` if it's not possible.
+    """
+    if target_type is dt.date:
+        target_type = dt.date.fromisoformat  # type: ignore
+
+    target_type = get_base_type(target_type)
+
+    for args in [
+        (),
+        (""),
+        (0),
+    ]:
+        try:
+            return target_type(*args)  # type: ignore
+        except:  # noqa
+            pass
+
+    return None
+
+
+def fuzz_wrapper(func):
+    """
+    Decorator for `rapidfuzz` functions: work around emojis that cause bugs.
+    """
+
+    @functools.wraps(func)
+    def wrapper(str1: str, str2: str, score_cutoff: float = 0):
+        try:
+            return func(str1, str2, score_cutoff)
+        except:  # noqa
+            # we build new strings that contain only alphanumerical characters and spaces
+            # and return the partial_ratio of that
+            new_str1 = "".join(each_letter for each_letter in str1 if each_letter.isalnum() or each_letter.isspace())
+            new_str2 = "".join(each_letter for each_letter in str2 if each_letter.isalnum() or each_letter.isspace())
+            return func(new_str1, new_str2, score_cutoff=score_cutoff)
+
+    return wrapper
+
+
+_ratio = fuzz_wrapper(fuzz.ratio)
+_partial_ratio = fuzz_wrapper(fuzz.partial_ratio)
+
+
+class Picture:
+    """
+    A picture (album art) on a website.
+    """
+
+    CHUNK_SIZE = 64 * 1024
+
+    def __init__(
+        self,
+        url: str = "",
+        width: int = 0,
+        height: int = 0,
+        sure=True,
+        data: Literal[False] | bytes | None = None,
+    ):
+        self.url = url
+        self.width = width
+        self.height = height or width
+        self.data: Literal[False] | bytes | None = data
+        self.sure = sure
+        self.req: requests.Response | None = None
+        self._pillow = None
+        self._load_metadata()
+
+    def _load_metadata(self):
+        if self.data:
+            self.sure = True
+            try:
+                from PIL import Image
+
+                img = Image.open(BytesIO(self.data))
+                self._pillow = img
+                self.width, self.height = img.size
+            except (ImportError, OSError):
+                pass
+
+    @property
+    def pillow(self):
+        if self._pillow is not None:
+            return self._pillow
+
+        if not isinstance(self.data, bytes):
+            return None
+
+        from PIL import Image
+
+        self._pillow = Image.open(BytesIO(self.data))
+        return self._pillow
+
+    @property
+    def size(self):
+        """
+        Size of the image (smallest dimension).
+        """
+        return min(self.width, self.height)
+
+    def check(self):
+        """
+        Check if the picture exists (without downloading it, if possible).
+        """
+        if self.sure:
+            return True
+        logger.debug("Checking picture '%s'...", self.url)
+        # don't download the picture, just the headers
+        req = requests.head(self.url, stream=True)
+        try:
+            req.raise_for_status()
+            self.sure = True
+        except requests.exceptions.HTTPError as err:
+            logger.debug("HTTP error: %s...", err)
+            self.sure = False
+        return self.sure
+
+    def download(self) -> Literal[False] | bytes:
+        """
+        Download the picture.
+        """
+        if self.data is not None:
+            return self.data
+
+        # download the picture
+        logger.debug("Downloading picture '%s'...", self.url)
+
+        self.data = b""
+
+        try:
+            # don't download the page if there is an error
+            self.req = requests.get(self.url, stream=True)
+            self.req.raise_for_status()
+            self.data = self.req.content
+        except requests.exceptions.HTTPError as err:
+            logger.debug("HTTP error: %s...", err)
+            self.data = False
+
+        logger.debug("Picture downloaded")
+        return self.data
+
+    def __repr__(self):
+        return f"<Picture {self.size}x{self.size} {'sure' if self.sure else 'not sure'} at {self.url}>"
+
+
+class PictureProvider:
+    """
+    Class for listing and downloading the images of a website.
+    """
+
+    pictures: list[Picture]
+
+    def __init__(self, result: dict[str, Any]):
+        self.provider_urls = {pic.size: pic for pic in self.get_sure_pictures(result)}
+
+        self.pictures = self.get_sure_pictures(result)
+
+        if not self.pictures:
+            return
+
+        sizes_to_try = [1200, 1000, 800, 500, 300]
+
+        for size in sizes_to_try:
+            if not any(pic.size == size for pic in self.pictures):
+                url = self.get_url_for_size(size)
+                if url:
+                    self.pictures.append(Picture(url, size, sure=False))
+
+        self.pictures.sort(key=lambda pic: pic.size, reverse=True)
+
+    def get_sure_pictures(self, result: dict[str, Any]) -> list[Picture]:
+        """
+        Return a list of all the sure pictures.
+        """
+        raise NotImplementedError
+
+    def get_url_for_size(self, size: int) -> str | None:
+        """
+        Return a probably valid URL for the given size.
+        """
+        first = self.pictures[0]
+        first_size = first.size
+        picture = first.url
+
+        url_parts = picture.split("/")
+        url_parts[-1] = url_parts[-1].replace(str(first_size), str(size))
+        return "/".join(url_parts)
+
+    def get_pictures(self):
+        return self.pictures
+
+    def get_best_picture(self):
+        return self.pictures[0]
+
+    @property
+    def pillow(self):
+        return self.get_best_picture().pillow
+
+
+class TagsList(TypedDict, total=False):
+    TIT2: Required[str]
+    TPE1: Required[str]
+    TALB: str
+    TLEN: str
+    TCOM: str
+    TYER: str
+    TDAT: str
+    TIME: str
+    COMM: str
+    TSRC: str
+    TRCK: str
+    TCOP: str
+    TLAN: str
+    TCON: str
+    USLT: str
+    SYLT: list[tuple[str, int]]
+    APIC: Picture | None
+
+
+class Song:
+    """
+    A song.
+    """
+
+    def __init__(
+        self,
+        *,
+        title: str = "",
+        artists: list[str] | tuple[str, ...] = (),
+        album: str | None = None,
+        duration: float = 0,
+        language: str | None = None,
+        genre: str | None = None,
+        composers: list[str] | None = None,
+        release_date: str | dt.date | None = None,
+        isrc: str | None = None,
+        track_number: int | tuple[int, int | None] | None = None,
+        copyright: str | None = None,  # pylint: disable=W0622
+        lyrics: str | list[tuple[str, float]] | None = None,
+        picture: Picture | PictureProvider | None = None,
+        comments: str | None = None,
+    ):
+        self.title = title
+        self.artists = list(artists)
+        self.album = album
+        self.duration = duration
+        self.language = language
+        self.genre = genre
+        self.composers = composers
+        if isinstance(release_date, str):
+            try:
+                self.release_date = dt.datetime.fromisoformat(release_date)
+            except ValueError:
+                self.release_date = None
+        else:
+            self.release_date = release_date
+        self.isrc = isrc
+        self.track_number = (track_number, None) if isinstance(track_number, int) else track_number
+        self.copyright = copyright
+        self.lyrics = lyrics.rstrip() if isinstance(lyrics, str) else lyrics
+        self.picture = picture
+        self.comments = comments
+
+    @classmethod
+    def empty(cls):
+        """
+        Return an empty song for placeholder purposes.
+        """
+        return cls()
+
+    def __not__(self):
+        return not self.title and not self.artists
+
+    def to_id3(self) -> TagsList:
+        """
+        Return the ID3 tags for a song.
+        """
+        if not self:
+            return {"TIT2": "", "TPE1": ""}
+        r_date = self.release_date
+        if not r_date:
+            year = date = time = ""
+        else:
+
+            def test_value(value: str):
+                return "" if not int(value) else value  # avoid "0000" for example...
+
+            year = test_value(f"{r_date:%Y}")  # YYYY
+            date = test_value(f"{r_date:%d%m}")  # DDMM
+            time = test_value(f"{r_date:%H%M}")  # HHMM
+
+        def format_lrc_timestamp(timestamp: float):
+            return f"[{int(timestamp // 60):02d}:{timestamp % 60:05.2f}]"
+
+        ret: TagsList = {
+            "TIT2": self.title,
+            "TPE1": ", ".join(self.artists),
+            "TALB": self.album or "",
+            "TLEN": str(int(self.duration * 1000)) if self.duration is not None else "",
+            "TCOM": ", ".join(self.composers) if self.composers else "",
+            "TYER": year,
+            "TDAT": date,
+            "TIME": time,
+            "TSRC": self.isrc or "",
+            "TRCK": (
+                (
+                    "/".join(str(n) for n in self.track_number)
+                    if isinstance(self.track_number, tuple)
+                    else str(self.track_number)
+                )
+                if self.track_number
+                else ""
+            ),
+            "TCOP": self.copyright or "",
+            "TLAN": self.language or "",
+            "TCON": self.genre or "",
+            "USLT": (
+                "\n".join((format_lrc_timestamp(ts) + line if line else "") for line, ts in self.lyrics)
+                if isinstance(self.lyrics, list)
+                else (self.lyrics or "")
+            ),
+            "SYLT": [(line[0], int(line[1] * 1000)) for line in self.lyrics] if isinstance(self.lyrics, list) else [],
+            "APIC": self.picture.get_best_picture() if isinstance(self.picture, PictureProvider) else self.picture,
+            "COMM": self.comments or "",
+        }
+        return ret
+
+    @classmethod
+    def from_id3(cls, file):
+        id3 = mutagen.id3.ID3(file)
+
+        @overload
+        def get_tag(tag: str, integer: Literal[False] = False) -> str: ...
+
+        @overload
+        def get_tag(tag: str, integer: Literal[True] = True) -> int: ...
+
+        def get_tag(tag, integer=False):
+            item = id3.getall(tag)
+            if not item:
+                return ""
+
+            text = item[0].text
+            if not text:
+                return ""
+            if isinstance(text, list):
+                text = text[0]
+
+            if integer:
+                try:
+                    return int(float(text))
+                except ValueError:
+                    return 0
+            return text
+
+        try:
+            date = get_tag("TDAT")
+            year = get_tag("TYER", True)
+            release_date = dt.date(year, int(date[2:4]), int(date[0:2]))
+        except (ValueError, IndexError):
+            release_date = None
+
+        track_n = get_tag("TRCK").split("/")
+        if len(track_n) < 2:
+            track_n.append("")
+        track_n = (int(track_n[0]), int(track_n[1])) if track_n[1] else int(track_n[0]) if track_n[0] else None
+
+        pictures = id3.getall("APIC")
+
+        return Song(
+            title=get_tag("TIT2"),
+            artists=[get_tag("TPE1")],
+            album=get_tag("TALB"),
+            duration=get_tag("TLEN", True),
+            language=get_tag("TLAN"),
+            genre=get_tag("TCON"),
+            composers=[get_tag("TCOM")],
+            release_date=release_date,
+            isrc=get_tag("TSRC"),
+            track_number=track_n,
+            copyright=get_tag("TCOP"),
+            lyrics=get_tag("USLT"),
+            picture=Picture(data=pictures[0].data, url=pictures[0].desc) if pictures else None,
+            comments=get_tag("COMM"),
+        )
+
+    def __repr__(self):
+        return f"<Song '{self.title}' by {', '.join(self.artists)} album {self.album} {self.duration} s>"
+
+
+def _get_sentence_words(string: str):
+    """
+    Get all the words in a sentence.
+    """
+    return re.findall(r"\w+", unidecode(string.lower()))
+
+
+def _normalize_sentence(string: str):
+    """
+    Return a sentence without punctuation, without brackets and lowercased.
+    """
+    return " ".join(_get_sentence_words(re.sub(r"(?i)\(.*?\)|-\s+.*|feat", "", string)))
+
+
+def get_provider_name(provider: str):
+    """
+    Return the human name of a provider.
+    """
+    return {"itunes": "iTunes", "youtube": "YouTube"}.get(provider, provider.title())
+
+
+def order_results(provider: str, results: list[Song], other_results: dict[str, list[Song]] | None):
+    """
+    Order the results: choose the result that is the most similar to the Spotify / Deezer song.
+    """
+    if not other_results:
+        return results
+
+    spotify_song = other_results["spotify"][0]
+    deezer_song = other_results["deezer"][0]
+
+    ret: list[tuple[Song, float, list[float]]] = []
+
+    def normalize_title(title: str):
+        return re.sub(r"\bst(e?s?)\.?(\s+|$)", r"saint\1\2", title)
+
+    for result in results:
+        # check for common word
+        song_title = normalize_title(result.title)
+        sp_title = normalize_title(spotify_song.title)
+        sp_title_words = _get_sentence_words(sp_title)
+
+        if not any(word in _get_sentence_words(song_title) for word in sp_title_words):
+            # if there are no common words, skip result
+            continue
+
+        # Find artist match
+        # match = (no of artist names in result) / (no of artist names on spotify) * 100
+        artist_match_number = 0
+
+        all_r_artists = _normalize_sentence(" ".join(result.artists))
+
+        artist_match_number = sum(
+            1 if _partial_ratio(_normalize_sentence(sp_artist), all_r_artists, 85) else 0
+            for sp_artist in spotify_song.artists
+        )
+
+        artist_match = (artist_match_number / len(spotify_song.artists)) * 100
+
+        # Skip if there are no artists in common
+        if artist_match_number == 0:
+            continue
+
+        name_match = _ratio(
+            str(unidecode(sp_title.lower())),
+            str(unidecode(song_title.lower())),
+            60,
+        )
+
+        official_match = (
+            len(
+                re.findall(
+                    r"(?i)(\b[ou]ffi[cz]i[ae]l|_off\b|\btopic\b)",
+                    song_title + " " + all_r_artists,
+                )
+            )
+            * 50
+        )
+        if not official_match and hasattr(result, "youtube_video"):
+            official_match += (
+                100 if "BADGE_STYLE_TYPE_VERIFIED_ARTIST" in result.youtube_video["badges"] else 0  # type: ignore
+            )
+        if official_match:
+            official_match += len(re.findall(r"(?i)\baudio\b", song_title)) * 100
+
+        if deezer_song.copyright:
+            copyright_match = 80 + (_normalize_sentence(deezer_song.copyright) in all_r_artists) * 20
+        else:
+            copyright_match = 100
+
+        delta = max(abs(result.duration - spotify_song.duration) - 4, 0)
+        non_match_value = delta**2 / spotify_song.duration * 100
+
+        time_match = max(100 - non_match_value, 0)
+
+        discard_match = (
+            len(
+                re.findall(
+                    r"""(?xi)
+                    \d+ h(?:our)\b
+                    |\b8d audio\b
+                    |\bspee?d up\b
+                    |\baco?usti
+                    |\blive\b
+                    |\bdire[ct]ta?\b
+                    |\bremix
+                    |\bversion
+                    |\brecord
+                    """,
+                    song_title,
+                )
+            )
+            * -100
+        )
+
+        # the average match is rounded for debugging
+        average_match = round(
+            (artist_match + name_match + official_match * 2 + copyright_match * 2 + time_match * 3 + discard_match * 2)
+            / 11,
+            ndigits=3,
+        )
+
+        # the results along with the average match
+        ret.append(
+            (
+                result,
+                average_match,
+                [artist_match, name_match, official_match, copyright_match, time_match],
+            )
+        )
+
+    ret = sorted(ret, key=lambda el: el[1], reverse=True)
+    logger.debug(
+        "%s sorted results:\n%s",
+        get_provider_name(provider),
+        "\n".join([f"{el[1]} ({' '.join(str(round(e, 3)) for e in el[2])}): {el[0]}" for el in ret]),
+    )
+    return [el[0] for el in ret]
+
+
+# for type checking
+def unidecode(string: str) -> str:
+    """
+    Transliterate an Unicode object into an ASCII string.
+    """
+    return unidecode_py(string)  # type: ignore
+
+
+AnyFunction = TypeVar("AnyFunction", bound=Callable)
+
+
+def locked(lock: Lock):
+    """
+    Acquire a lock before executing the function and release it after
+    (if the lock has already been released, don't do anything).
+    """
+
+    def decorator(f: AnyFunction) -> AnyFunction:
+        @functools.wraps(f)
+        def wrapper(*args, **kwargs):
+            lock.acquire()
+            try:
+                return f(*args, **kwargs)
+            finally:
+                if lock.locked():
+                    lock.release()
+
+        return wrapper  # type: ignore
+
+    return decorator
+
+
+def format_query(song: str, artist: str | None = None, market: str | None = None):
+    """
+    Return a formatted version of `song`, `artist` and `market` (for logging).
+    """
+    return f"'{song}'" + (f" - '{artist}'" if artist else "") + (f" on '{market}' market" if market else "")
```

### Comparing `songs-dl-0.1.0/songs_dl/youtube.py` & `songs-dl-2024.4.4/songs_dl/youtube.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import json
-import logging
-import re
-import sys
-from pprint import pformat
-from threading import Lock
-from typing import Any, TypedDict
-
-import requests
-
-from .utils import Song, format_query, get, locked
-
-youtube_lock = Lock()
-logger = logging.getLogger(__name__)
-
-
-class YoutubeVideo(TypedDict):
-    id: str
-    thumbnail: str
-    title: str
-    channel: str
-    length: int
-    views: int
-    badges: list[str]
-    match_value: int | None
-
-
-class Thumbnail(TypedDict):
-    width: int
-    size: int
-    url: str
-
-
-class YtThumbnailObject(TypedDict):
-    thumbnails: list[Thumbnail]
-
-
-class YtText(TypedDict):
-    text: str
-
-
-class YtRunsText(TypedDict):
-    runs: list[YtText]
-
-
-class YtSimpleText(TypedDict):
-    simpleText: str
-
-
-class YtBadge(TypedDict):
-    style: str
-
-
-class YtBadgeObject(TypedDict):
-    metadataBadgeRenderer: YtBadge
-
-
-class YtInitialData(TypedDict):
-    videoId: str
-    thumbnail: YtThumbnailObject
-    title: YtRunsText
-    longBylineText: YtRunsText
-    publishedTimeText: YtSimpleText
-    lengthText: YtSimpleText
-    viewCountText: YtSimpleText
-    ownerBadges: list[YtBadgeObject]
-    ownerText: YtRunsText
-    shortBylineText: YtRunsText
-    shortViewCountText: YtSimpleText
-    isWatched: bool
-
-
-class YoutubeSong(Song):
-    def __init__(self, *args, youtube_video: YoutubeVideo, **kwargs):
-        self.youtube_video = youtube_video
-        super().__init__(*args, **kwargs)
-
-
-def download_youtube(song: str, artist: str | None = None, _market: str | None = None):
-    """
-    Get the YouTube search results.
-    """
-    logger.info("Searching %s on YouTube...", format_query(song, artist))
-    if artist:
-        query = song + " " + artist
-    else:
-        query = song
-    song = f"allintitle:{song}"
-    req = locked(youtube_lock)(requests.get)("https://www.youtube.com/results", params={"search_query": query})
-    logger.debug("Page size: %d", len(req.text))
-    if not (match := re.search(r"var ytInitialData = (.*?);</script>", req.text)):
-        # no YouTube video = no song => stop
-        logger.error("Search failed: can't get the results in the YouTube page!")
-        sys.exit()
-
-    logger.info("Results have been found")
-    try:
-        result = json.loads(match.group(1))
-        logger.debug("JSON decoding OK")
-    except json.decoder.JSONDecodeError as err:
-        logger.critical("JSON decoding error: %s", err)  # same thing
-        sys.exit()
-
-    main_contents = get(
-        result,
-        (
-            "contents",
-            "twoColumnSearchResultsRenderer",
-            "primaryContents",
-            "sectionListRenderer",
-            "contents",
-        ),
-        list,
-    )
-
-    videos_list = []
-    for content in main_contents:
-        contents = get(content, ("itemSectionRenderer", "contents"), list)
-        for video in contents:
-            # there is other information like
-            # promotedSparklesTextSearchRenderer...
-            # but it's not useful
-            if "videoRenderer" in video:
-                videos_list.append(video)
-
-    if len(videos_list) == 0:
-        logger.critical("No results!")  # same thing
-        sys.exit()
-
-    logger.debug("%d videos", len(videos_list))
-
-    def map_video(video_data: dict[str, Any]):
-        video = get(video_data, "videoRenderer", dict[str, Any])
-        length = sum(
-            # 0 = 1 (seconds); 1 = 60 (minutes); 2 = 3600 (hours); ...
-            int(value or 0) * (60**index)
-            for index, value in enumerate(
-                get(video, ("lengthText", "simpleText"), str).split(":")[::-1]
-            )  # from the end
-        )
-        thumbnail: str = ""
-        size = 0
-        for f in get(video, ("thumbnail", "thumbnails"), list[dict[str, Any]]):
-            if get(f, "width", int) >= size:
-                size = get(f, "width", int)
-                thumbnail = get(f, "url", str)
-
-        def get_int(value: str):
-            """
-            Helper function for view count.
-
-            >>> get_int("12 345 views")s
-            12345
-            """
-            value = "".join(c for c in value if c.isnumeric())
-            try:
-                return int(value)
-            except ValueError:
-                return 0
-
-        ret: YoutubeVideo = {
-            "id": get(video, "videoId", str),
-            "thumbnail": thumbnail,
-            "title": get(video, ("title", "runs", 0, "text"), str),
-            "channel": get(video, ("ownerText", "runs", 0, "text"), str),
-            "length": length,
-            "views": get(video, ("viewCountText", "simpleText"), get_int),
-            "badges": [
-                get(badge, ("metadataBadgeRenderer", "style"), str)
-                for badge in get(video, "ownerBadges", list[dict[str, Any]])
-            ],
-            "match_value": None,
-        }
-
-        artists = []
-
-        if "-" in ret["title"]:
-            parts = ret["title"].split("-", 1)
-            title = parts[1].strip("-").strip()
-            artists.append(parts[0].strip("-").strip())
-        else:
-            title = ret["title"]
-
-        match = re.search(
-            r"""(?x)
-        ^ (?P<title_first>.*) # first part of title
-        \(? \b f(?:ea)?t \b \.? (?P<artist>.*?) \)? # feat. / ft. with parens
-        (?P<title_second> \( .*)? \)? $ # second part of title (begins with paren), remove trailing ")"
-        """,
-            title,
-        )
-        if match:
-            title = (match.group("title_first").strip() + " " + (match.group("title_second") or "")[1:].strip()).strip()
-            artists.append(match.group("artist").strip())
-
-        artists.append(ret["channel"])
-
-        return YoutubeSong(title=title, artists=artists, duration=ret["length"], youtube_video=ret)
-
-    ret = [map_video(v) for v in videos_list]
-
-    logger.debug("Results:\n%s", pformat(ret))
-
-    return ret
+import json
+import logging
+import re
+import sys
+from pprint import pformat
+from threading import Lock
+from typing import Any, TypedDict
+
+import requests
+
+from .utils import Song, format_query, get, locked
+
+youtube_lock = Lock()
+logger = logging.getLogger(__name__)
+
+
+class YoutubeVideo(TypedDict):
+    id: str
+    thumbnail: str
+    title: str
+    channel: str
+    length: int
+    views: int
+    badges: list[str]
+    match_value: int | None
+
+
+class Thumbnail(TypedDict):
+    width: int
+    size: int
+    url: str
+
+
+class YtThumbnailObject(TypedDict):
+    thumbnails: list[Thumbnail]
+
+
+class YtText(TypedDict):
+    text: str
+
+
+class YtRunsText(TypedDict):
+    runs: list[YtText]
+
+
+class YtSimpleText(TypedDict):
+    simpleText: str
+
+
+class YtBadge(TypedDict):
+    style: str
+
+
+class YtBadgeObject(TypedDict):
+    metadataBadgeRenderer: YtBadge
+
+
+class YtInitialData(TypedDict):
+    videoId: str
+    thumbnail: YtThumbnailObject
+    title: YtRunsText
+    longBylineText: YtRunsText
+    publishedTimeText: YtSimpleText
+    lengthText: YtSimpleText
+    viewCountText: YtSimpleText
+    ownerBadges: list[YtBadgeObject]
+    ownerText: YtRunsText
+    shortBylineText: YtRunsText
+    shortViewCountText: YtSimpleText
+    isWatched: bool
+
+
+class YoutubeSong(Song):
+    def __init__(self, *args, youtube_video: YoutubeVideo, **kwargs):
+        self.youtube_video = youtube_video
+        super().__init__(*args, **kwargs)
+
+
+def download_youtube(song: str, artist: str | None = None, _market: str | None = None):
+    """
+    Get the YouTube search results.
+    """
+    logger.info("Searching %s on YouTube...", format_query(song, artist))
+    if artist:
+        query = song + " " + artist
+    else:
+        query = song
+    song = f"allintitle:{song}"
+    req = locked(youtube_lock)(requests.get)("https://www.youtube.com/results", params={"search_query": query})
+    logger.debug("Page size: %d", len(req.text))
+    if not (match := re.search(r"var ytInitialData = (.*?);</script>", req.text)):
+        # no YouTube video = no song => stop
+        logger.error("Search failed: can't get the results in the YouTube page!")
+        sys.exit()
+
+    logger.info("Results have been found")
+    try:
+        result = json.loads(match.group(1))
+        logger.debug("JSON decoding OK")
+    except json.decoder.JSONDecodeError as err:
+        logger.critical("JSON decoding error: %s", err)  # same thing
+        sys.exit()
+
+    main_contents = get(
+        result,
+        (
+            "contents",
+            "twoColumnSearchResultsRenderer",
+            "primaryContents",
+            "sectionListRenderer",
+            "contents",
+        ),
+        list,
+    )
+
+    videos_list = []
+    for content in main_contents:
+        contents = get(content, ("itemSectionRenderer", "contents"), list)
+        for video in contents:
+            # there is other information like
+            # promotedSparklesTextSearchRenderer...
+            # but it's not useful
+            if "videoRenderer" in video:
+                videos_list.append(video)
+
+    if len(videos_list) == 0:
+        logger.critical("No results!")  # same thing
+        sys.exit()
+
+    logger.debug("%d videos", len(videos_list))
+
+    def map_video(video_data: dict[str, Any]):
+        video = get(video_data, "videoRenderer", dict[str, Any])
+        length = sum(
+            # 0 = 1 (seconds); 1 = 60 (minutes); 2 = 3600 (hours); ...
+            int(value or 0) * (60**index)
+            for index, value in enumerate(
+                get(video, ("lengthText", "simpleText"), str).split(":")[::-1]
+            )  # from the end
+        )
+        thumbnail: str = ""
+        size = 0
+        for f in get(video, ("thumbnail", "thumbnails"), list[dict[str, Any]]):
+            if get(f, "width", int) >= size:
+                size = get(f, "width", int)
+                thumbnail = get(f, "url", str)
+
+        def get_int(value: str):
+            """
+            Helper function for view count.
+
+            >>> get_int("12 345 views")s
+            12345
+            """
+            value = "".join(c for c in value if c.isnumeric())
+            try:
+                return int(value)
+            except ValueError:
+                return 0
+
+        ret: YoutubeVideo = {
+            "id": get(video, "videoId", str),
+            "thumbnail": thumbnail,
+            "title": get(video, ("title", "runs", 0, "text"), str),
+            "channel": get(video, ("ownerText", "runs", 0, "text"), str),
+            "length": length,
+            "views": get(video, ("viewCountText", "simpleText"), get_int),
+            "badges": [
+                get(badge, ("metadataBadgeRenderer", "style"), str)
+                for badge in get(video, "ownerBadges", list[dict[str, Any]])
+            ],
+            "match_value": None,
+        }
+
+        artists = []
+
+        if " - " in ret["title"]:
+            parts = ret["title"].split(" - ", 1)
+            title = parts[1].strip().strip("-").strip()
+            artists.append(parts[0].strip().strip("-").strip())
+        else:
+            title = ret["title"]
+
+        match = re.search(
+            r"""(?x)
+        ^ (?P<title_first>.*) # first part of title
+        [(\[]? \b f(?:ea)?t \b \.? (?P<artist>.*?) [)\]]? # feat. / ft. with parens or brackets
+        (?P<title_second> [(\[] .*)? [)\]]? $ # second part of title (begins with paren), remove trailing ")"
+        """,
+            title,
+        )
+        if match:
+            title = (match.group("title_first").strip() + " " + (match.group("title_second") or "")[1:].strip()).strip()
+            artists.append(match.group("artist").strip())
+
+        artists.append(ret["channel"])
+
+        return YoutubeSong(title=title, artists=artists, duration=ret["length"], youtube_video=ret)
+
+    ret = [map_video(v) for v in videos_list]
+
+    logger.debug("Results:\n%s", pformat(ret))
+
+    return ret
```


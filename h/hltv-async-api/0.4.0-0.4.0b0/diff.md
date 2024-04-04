# Comparing `tmp/hltv_async_api-0.4.0.tar.gz` & `tmp/hltv_async_api-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.0.tar", last modified: Thu Apr  4 14:25:46 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.0b0.tar", last modified: Thu Apr  4 03:01:57 2024, max compression
```

## Comparing `hltv_async_api-0.4.0.tar` & `hltv_async_api-0.4.0b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:25:46.439440 hltv_async_api-0.4.0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     5751 2024-04-04 14:25:46.438030 hltv_async_api-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5128 2024-04-04 03:09:51.000000 hltv_async_api-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 14:25:46.380654 hltv_async_api-0.4.0/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-04 14:24:27.000000 hltv_async_api-0.4.0/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    30303 2024-04-04 14:25:41.000000 hltv_async_api-0.4.0/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:25:46.434424 hltv_async_api-0.4.0/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     5751 2024-04-04 14:25:46.000000 hltv_async_api-0.4.0/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-04 14:25:46.000000 hltv_async_api-0.4.0/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:25:46.000000 hltv_async_api-0.4.0/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 14:25:46.000000 hltv_async_api-0.4.0/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-04 14:24:27.000000 hltv_async_api-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 14:25:46.440452 hltv_async_api-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-04 14:24:27.000000 hltv_async_api-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:01:57.269712 hltv_async_api-0.4.0b0/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.0b0/LICENSE
+-rw-rw-rw-   0        0        0     4955 2024-04-04 03:01:57.268712 hltv_async_api-0.4.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4330 2024-04-03 13:07:43.000000 hltv_async_api-0.4.0b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 03:01:57.236716 hltv_async_api-0.4.0b0/hltv_async_api/
+-rw-rw-rw-   0        0        0      126 2024-04-04 03:01:47.000000 hltv_async_api-0.4.0b0/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    30071 2024-04-04 03:01:16.000000 hltv_async_api-0.4.0b0/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:01:57.266715 hltv_async_api-0.4.0b0/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     4955 2024-04-04 03:01:57.000000 hltv_async_api-0.4.0b0/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-04 03:01:57.000000 hltv_async_api-0.4.0b0/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 03:01:57.000000 hltv_async_api-0.4.0b0/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 03:01:57.000000 hltv_async_api-0.4.0b0/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      539 2024-04-04 03:01:47.000000 hltv_async_api-0.4.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 03:01:57.270716 hltv_async_api-0.4.0b0/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-04-04 03:01:47.000000 hltv_async_api-0.4.0b0/setup.py
```

### Comparing `hltv_async_api-0.4.0/LICENSE` & `hltv_async_api-0.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.0/PKG-INFO` & `hltv_async_api-0.4.0b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,20 @@
-Metadata-Version: 2.1
-Name: hltv_async_api
-Version: 0.4.0
-Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
-Home-page: https://github.com/akimerslys/aiohltv
-Author: akimerslys
-Author-email: Akim Slys <akimslys2003@gmail.com>
-Project-URL: Homepage, https://github.com/akimerslys/aiohltv
-Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
 **This page not completed, not all methods and configs are written**
 
 
 # Features
 
+* New and modern fully async library
 
-* **Simple Usage** (its realy simple)
-
-
-* **New and modern fully async library**
-
+* Supports proxy usage for rate-limiting and privacy
 
-* **Supports proxy usage with huge amount of options**
+* Automatically changes proxy if access is denied
 
 
 ---
 
 # Installation
 
 ```
@@ -84,94 +65,77 @@
 
 hltv = Hltv(use_proxy=True, proxy_list=proxy_list, proxy_protocol='http')
 ```
 
 ---
 # Methods
 
-* **get_upcoming_matches(days: int = 7, min_star_rating: int = 1)**
+* get_upcoming_matches(days: int = 7, min_star_rating: int = 1)
 
     -days (the number of days into the future to fetch matches for)
   
     -min_star_rating (the minimum star rating for matches to include)
   
 ```
 await hltv.get_upcoming_matches(1, 5)
 
->>> ['date': '11-11', 'matches': [id: '1111', team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
+>>> ['date': '11/11/2024', 'matches': [team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
 
 ```
-* **get_events(outgoing=True, future=True, max_events=10) -> [('id', 'title', 'startdate', 'enddate')]**
 
-```
-await hltv.get_events(future=False)
-
->>>[{'id': '7620', 'name': 'ESL Challenger League Season 47 Europe', 'start_date': '26-2', 'end_date': '16-6'}, {'id': '7749', 'name': 'Thunderpick World Championship 2024 EU Closed Qualifier 1', 'start_date': '1-4', 'end_date': '22-4'}]
-
-```
-
-* **get_event_results(event_id: int | str)**
+* get_event_results(event_id: int | str)
 
   
 ```
 await get_event_results(7148)
 
->>> ['date': '31-3', 'matches': ['id': '1111', team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']]
+>>> ['date': '31-3', 'team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']
 
 ```
 
-* **get_event_matches(event_id: str | int):**
+* get_event_matches(event_id: str | int):
   
 ```
 await hltv.get_event_matches(7148)
 
->>>['date': '1-1' | 'LIVE, 'matches': ['id': '1111', team1': 'Natus Vincere', 'team2': 'FaZe']
+>>>['team1': 'Natus Vincere', 'team2': 'FaZe', 'date': '11-11' | 'LIVE']
 ```
 
-* **get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)**
+* get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)
 
 ```
 await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024')
 
 (7148, 'PGL CS2 Major Copenhagen2024', '21-3', '31-3', '$1,250,000', '16', 'Copenhagen, Denmark', [])
 ```
 
 
-* **get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']**
+get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']
 
 ```
 await hltv.get_top_teams(2)
 
->>>[{'id': '1111', 'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'id': '1111', 'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
+>>>[{'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
 ```
 
-* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
+get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)
 
 ```
 await hltv.get_team_info(6667, 'faze')
 
 >>>(6667, 'faze', '1', ['karrigan', 'rain', 'frozen', 'ropz', 'broky'], 'NEO', '26.5', '256', 'CS Asia Championships 2023', 21)
 ```
 
-* **get_last_news(max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]**
+get_last_news(self, max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]
 
 ```
 await hltv.get_last_news(only_today=True, max_reg_news=1)
 
 >>>[{'date': '02-04', 'f_news': [{'f_id': '38682', 'f_title': 'NIP confirm r1nkle signing', 'f_desc': "Ninjas in Pyjamas only have an anchor player left to sign following the young Ukrainian AWPer's addition."}], 'news': [{'id': '38685', 'title': 'Rounds add sLowi, p3kko', 'posted': 'an hour ago'}, {'id': '38690', 'title': 'n1ssim returns to Sharks after paiN loan deal expires', 'posted': 'an hour ago'}]}]
 ```
-
-* **get_best_players(top=40) -> ('rank', 'name', 'team', 'maps', 'rating')**
-
-```
-await hltv.get_best_players(2)
-
->>>[{'rank': 1, 'name': 'donk', 'team': 'Spirit', 'maps': '33', 'rating': '1.52'}, {'rank': 2, 'name': 'm0NESY', 'team': 'G2', 'maps': '34', 'rating': '1.38'}]
-```
-
 ---
 # Examples
 
 ****Simple Example****
 
 ```
 from hltv_async_api import Hltv
```

### Comparing `hltv_async_api-0.4.0/README.md` & `hltv_async_api-0.4.0b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+Metadata-Version: 2.1
+Name: hltv_async_api
+Version: 0.4.0b0
+Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
+Home-page: https://github.com/akimerslys/aiohltv
+Author: akimerslys
+Author-email: Akim Slys <akimslys2003@gmail.com>
+Project-URL: Homepage, https://github.com/akimerslys/aiohltv
+Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
 **This page not completed, not all methods and configs are written**
 
 
 # Features
 
+* New and modern fully async library
 
-* **Simple Usage** (its realy simple)
-
-
-* **New and modern fully async library**
-
+* Supports proxy usage for rate-limiting and privacy
 
-* **Supports proxy usage with huge amount of options**
+* Automatically changes proxy if access is denied
 
 
 ---
 
 # Installation
 
 ```
@@ -68,94 +81,77 @@
 
 hltv = Hltv(use_proxy=True, proxy_list=proxy_list, proxy_protocol='http')
 ```
 
 ---
 # Methods
 
-* **get_upcoming_matches(days: int = 7, min_star_rating: int = 1)**
+* get_upcoming_matches(days: int = 7, min_star_rating: int = 1)
 
     -days (the number of days into the future to fetch matches for)
   
     -min_star_rating (the minimum star rating for matches to include)
   
 ```
 await hltv.get_upcoming_matches(1, 5)
 
->>> ['date': '11-11', 'matches': [id: '1111', team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
+>>> ['date': '11/11/2024', 'matches': [team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
 
 ```
-* **get_events(outgoing=True, future=True, max_events=10) -> [('id', 'title', 'startdate', 'enddate')]**
 
-```
-await hltv.get_events(future=False)
-
->>>[{'id': '7620', 'name': 'ESL Challenger League Season 47 Europe', 'start_date': '26-2', 'end_date': '16-6'}, {'id': '7749', 'name': 'Thunderpick World Championship 2024 EU Closed Qualifier 1', 'start_date': '1-4', 'end_date': '22-4'}]
-
-```
-
-* **get_event_results(event_id: int | str)**
+* get_event_results(event_id: int | str)
 
   
 ```
 await get_event_results(7148)
 
->>> ['date': '31-3', 'matches': ['id': '1111', team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']]
+>>> ['date': '31-3', 'team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']
 
 ```
 
-* **get_event_matches(event_id: str | int):**
+* get_event_matches(event_id: str | int):
   
 ```
 await hltv.get_event_matches(7148)
 
->>>['date': '1-1' | 'LIVE, 'matches': ['id': '1111', team1': 'Natus Vincere', 'team2': 'FaZe']
+>>>['team1': 'Natus Vincere', 'team2': 'FaZe', 'date': '11-11' | 'LIVE']
 ```
 
-* **get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)**
+* get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)
 
 ```
 await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024')
 
 (7148, 'PGL CS2 Major Copenhagen2024', '21-3', '31-3', '$1,250,000', '16', 'Copenhagen, Denmark', [])
 ```
 
 
-* **get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']**
+get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']
 
 ```
 await hltv.get_top_teams(2)
 
->>>[{'id': '1111', 'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'id': '1111', 'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
+>>>[{'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
 ```
 
-* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
+get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)
 
 ```
 await hltv.get_team_info(6667, 'faze')
 
 >>>(6667, 'faze', '1', ['karrigan', 'rain', 'frozen', 'ropz', 'broky'], 'NEO', '26.5', '256', 'CS Asia Championships 2023', 21)
 ```
 
-* **get_last_news(max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]**
+get_last_news(self, max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]
 
 ```
 await hltv.get_last_news(only_today=True, max_reg_news=1)
 
 >>>[{'date': '02-04', 'f_news': [{'f_id': '38682', 'f_title': 'NIP confirm r1nkle signing', 'f_desc': "Ninjas in Pyjamas only have an anchor player left to sign following the young Ukrainian AWPer's addition."}], 'news': [{'id': '38685', 'title': 'Rounds add sLowi, p3kko', 'posted': 'an hour ago'}, {'id': '38690', 'title': 'n1ssim returns to Sharks after paiN loan deal expires', 'posted': 'an hour ago'}]}]
 ```
-
-* **get_best_players(top=40) -> ('rank', 'name', 'team', 'maps', 'rating')**
-
-```
-await hltv.get_best_players(2)
-
->>>[{'rank': 1, 'name': 'donk', 'team': 'Spirit', 'maps': '33', 'rating': '1.52'}, {'rank': 2, 'name': 'm0NESY', 'team': 'G2', 'maps': '34', 'rating': '1.38'}]
-```
-
 ---
 # Examples
 
 ****Simple Example****
 
 ```
 from hltv_async_api import Hltv
```

### Comparing `hltv_async_api-0.4.0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.0b0/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
                  timeout: int = 5,
                  use_proxy: bool = False,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
-                 proxy_one_time: bool = False,
-                 true_session: bool = False,
+                 proxy_one_time: bool = False
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "UTC"
         }
         self.MAX_DELAY = max_delay
@@ -45,15 +44,14 @@
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
-        self.TRUE_SESSION = true_session
         self.session = None
 
     def _configure_logging(self):
         level = logging.DEBUG if self.DEBUG else logging.INFO
         logging.basicConfig(level=level, format="%(message)s")
 
     async def _create_session(self):
@@ -105,27 +103,27 @@
         return proxy
 
     async def _switch_proxy(self):
         if self.PROXY_ONCE:
             self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
             self.PROXY_LIST = self.PROXY_LIST[1:]
         else:
-            self.logger.debug(f"Switching proxy {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
-            self.PROXY_LIST = self.PROXY_LIST[1:] + [(self.PROXY_LIST[0])]
-            self.logger.info(f"New proxy: {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
+            self.logger.debug(f"Switching proxy {self.PROXY_LIST[0]}")
+            self.PROXY_LIST = self.PROXY_LIST[1:] + self.PROXY_LIST[0]
+            self.logger.info(f"New proxy: {self.PROXY_LIST[0]}")
 
     def _f(self, result):
         return BeautifulSoup(result, "lxml")
 
     async def _cloudflare_check(self, result) -> bool:
         page = self._f(result)
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text():
-                self.logger.debug("Got cloudflare challenge page")
+                self.logger.debug("Got cloudflare challange page")
                 return True
         return False
 
     async def _parse_error_handler(self, delay: int = 0) -> int:
         if self.USE_PROXY:
             await self._switch_proxy()
         else:
@@ -165,32 +163,26 @@
 
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             await self._create_session()
 
         status = False
         try_ = 1
-        result = None
         while not status and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
 
             # if status = True, result = page,
             # if status = False result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
-        # After Parse
-        if not self.TRUE_SESSION:
-            # Automaticaly close session after parse
-            await self.close_session()
-
-        if status:
+        if status == True:
             loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
             return None
 
@@ -749,12 +741,13 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv(debug=True)
+    #hltv = Hltv(use_proxy=True, proxy_path='proxies.txt', debug=True, proxy_one_time=True, proxy_protocol='http')
+    hltv = Hltv()
     print(await hltv.get_match_info('2370727', 'faze', 'natus-vincere', 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.4.0/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.4.0b0/hltv_async_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.0
+Version: 0.4.0b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
@@ -18,22 +18,19 @@
 
 
 **This page not completed, not all methods and configs are written**
 
 
 # Features
 
+* New and modern fully async library
 
-* **Simple Usage** (its realy simple)
+* Supports proxy usage for rate-limiting and privacy
 
-
-* **New and modern fully async library**
-
-
-* **Supports proxy usage with huge amount of options**
+* Automatically changes proxy if access is denied
 
 
 ---
 
 # Installation
 
 ```
@@ -84,94 +81,77 @@
 
 hltv = Hltv(use_proxy=True, proxy_list=proxy_list, proxy_protocol='http')
 ```
 
 ---
 # Methods
 
-* **get_upcoming_matches(days: int = 7, min_star_rating: int = 1)**
+* get_upcoming_matches(days: int = 7, min_star_rating: int = 1)
 
     -days (the number of days into the future to fetch matches for)
   
     -min_star_rating (the minimum star rating for matches to include)
   
 ```
 await hltv.get_upcoming_matches(1, 5)
 
->>> ['date': '11-11', 'matches': [id: '1111', team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
-
-```
-* **get_events(outgoing=True, future=True, max_events=10) -> [('id', 'title', 'startdate', 'enddate')]**
-
-```
-await hltv.get_events(future=False)
-
->>>[{'id': '7620', 'name': 'ESL Challenger League Season 47 Europe', 'start_date': '26-2', 'end_date': '16-6'}, {'id': '7749', 'name': 'Thunderpick World Championship 2024 EU Closed Qualifier 1', 'start_date': '1-4', 'end_date': '22-4'}]
+>>> ['date': '11/11/2024', 'matches': [team1: 'Natus Vincere' | 'TBD', team2: 'FaZe' | 'TBD', time: '14:15', maps: '3', stars: 5, 'PGL CS2 Major Copenhagen 2024' | None]]```
 
 ```
 
-* **get_event_results(event_id: int | str)**
+* get_event_results(event_id: int | str)
 
   
 ```
 await get_event_results(7148)
 
->>> ['date': '31-3', 'matches': ['id': '1111', team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']]
+>>> ['date': '31-3', 'team1': 'FaZe', 'team2': 'Natus Vincere', 'score1': '1', 'score2': '2']
 
 ```
 
-* **get_event_matches(event_id: str | int):**
+* get_event_matches(event_id: str | int):
   
 ```
 await hltv.get_event_matches(7148)
 
->>>['date': '1-1' | 'LIVE, 'matches': ['id': '1111', team1': 'Natus Vincere', 'team2': 'FaZe']
+>>>['team1': 'Natus Vincere', 'team2': 'FaZe', 'date': '11-11' | 'LIVE']
 ```
 
-* **get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)**
+* get_event_info(event_id: str | int, event_title: str) -> (event_id, event_title, event_start, event_end, prize, team_num, location, groups)
 
 ```
 await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024')
 
 (7148, 'PGL CS2 Major Copenhagen2024', '21-3', '31-3', '$1,250,000', '16', 'Copenhagen, Denmark', [])
 ```
 
 
-* **get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']**
+get_top_teams(max_teams=30) -> ['rank', 'title', 'points', 'change', 'id']
 
 ```
 await hltv.get_top_teams(2)
 
->>>[{'id': '1111', 'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'id': '1111', 'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
+>>>[{'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
 ```
 
-* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
+get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)
 
 ```
 await hltv.get_team_info(6667, 'faze')
 
 >>>(6667, 'faze', '1', ['karrigan', 'rain', 'frozen', 'ropz', 'broky'], 'NEO', '26.5', '256', 'CS Asia Championships 2023', 21)
 ```
 
-* **get_last_news(max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]**
+get_last_news(self, max_reg_news=2, only_today=True, only_featured=False) -> [date, [featured_id, featured_title, featured_desciption], [regular_id, reg_title, reg_time]]
 
 ```
 await hltv.get_last_news(only_today=True, max_reg_news=1)
 
 >>>[{'date': '02-04', 'f_news': [{'f_id': '38682', 'f_title': 'NIP confirm r1nkle signing', 'f_desc': "Ninjas in Pyjamas only have an anchor player left to sign following the young Ukrainian AWPer's addition."}], 'news': [{'id': '38685', 'title': 'Rounds add sLowi, p3kko', 'posted': 'an hour ago'}, {'id': '38690', 'title': 'n1ssim returns to Sharks after paiN loan deal expires', 'posted': 'an hour ago'}]}]
 ```
-
-* **get_best_players(top=40) -> ('rank', 'name', 'team', 'maps', 'rating')**
-
-```
-await hltv.get_best_players(2)
-
->>>[{'rank': 1, 'name': 'donk', 'team': 'Spirit', 'maps': '33', 'rating': '1.52'}, {'rank': 2, 'name': 'm0NESY', 'team': 'G2', 'maps': '34', 'rating': '1.38'}]
-```
-
 ---
 # Examples
 
 ****Simple Example****
 
 ```
 from hltv_async_api import Hltv
```

### Comparing `hltv_async_api-0.4.0/pyproject.toml` & `hltv_async_api-0.4.0b0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.0"
+version = "0.4.0b0"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.4.0/setup.py` & `hltv_async_api-0.4.0b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.0',
+    version='0.4.0b0',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```


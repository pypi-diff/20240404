# Comparing `tmp/hltv_async_api-0.3.1.tar.gz` & `tmp/hltv_async_api-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.3.1.tar", last modified: Wed Apr  3 13:08:38 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.0b0.tar", last modified: Thu Apr  4 03:01:57 2024, max compression
```

## Comparing `hltv_async_api-0.3.1.tar` & `hltv_async_api-0.4.0b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:08:38.167167 hltv_async_api-0.3.1/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     4953 2024-04-03 13:08:38.166165 hltv_async_api-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4330 2024-04-03 13:07:43.000000 hltv_async_api-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:08:38.143166 hltv_async_api-0.3.1/hltv_async_api/
--rw-rw-rw-   0        0        0      125 2024-04-02 22:43:58.000000 hltv_async_api-0.3.1/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    28116 2024-04-03 13:05:13.000000 hltv_async_api-0.3.1/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:08:38.165170 hltv_async_api-0.3.1/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     4953 2024-04-03 13:08:38.000000 hltv_async_api-0.3.1/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-03 13:08:38.000000 hltv_async_api-0.3.1/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:08:38.000000 hltv_async_api-0.3.1/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-03 13:08:38.000000 hltv_async_api-0.3.1/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-03 13:08:36.000000 hltv_async_api-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 13:08:38.168171 hltv_async_api-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-03 13:08:36.000000 hltv_async_api-0.3.1/setup.py
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

### Comparing `hltv_async_api-0.3.1/LICENSE` & `hltv_async_api-0.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.3.1/PKG-INFO` & `hltv_async_api-0.4.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.3.1
+Version: 0.4.0b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.3.1/README.md` & `hltv_async_api-0.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.3.1/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.0b0/hltv_async_api/aiohltv.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import asyncio
 from asyncio import get_running_loop
 from functools import partial
 
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
     ServerDisconnectedError, ClientHttpProxyError
+import re
+
 
 import logging
 
 
 class Hltv:
     def __init__(self, max_delay: int = 15,
                  timeout: int = 5,
@@ -42,18 +44,29 @@
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
+        self.session = None
+
     def _configure_logging(self):
         level = logging.DEBUG if self.DEBUG else logging.INFO
         logging.basicConfig(level=level, format="%(message)s")
 
+    async def _create_session(self):
+        self.logger.debug('Creating Session')
+        self.session = ClientSession()
+
+    async def close_session(self):
+        if self.session:
+            self.logger.debug('Closing Session')
+            await self.session.close()
+
     def config(self, max_delay: int | None = None,
                timeout: int | None = None,
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
                max_retries: int | None = None,
@@ -77,139 +90,142 @@
         if debug:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
-    async def get_proxy(self):
+    async def _get_proxy(self):
         proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
             proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
 
-    async def switch_proxy(self):
+    async def _switch_proxy(self):
         if self.PROXY_ONCE:
             self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
             self.PROXY_LIST = self.PROXY_LIST[1:]
         else:
             self.logger.debug(f"Switching proxy {self.PROXY_LIST[0]}")
             self.PROXY_LIST = self.PROXY_LIST[1:] + self.PROXY_LIST[0]
             self.logger.info(f"New proxy: {self.PROXY_LIST[0]}")
 
-    def f(self, result):
+    def _f(self, result):
         return BeautifulSoup(result, "lxml")
 
-    async def cloudflare_check(self, result) -> bool:
-        page = self.f(result)
+    async def _cloudflare_check(self, result) -> bool:
+        page = self._f(result)
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text():
                 self.logger.debug("Got cloudflare challange page")
                 return True
         return False
 
-    async def parse_error_handler(self, proxy, delay: int = 0) -> int:
+    async def _parse_error_handler(self, delay: int = 0) -> int:
         if self.USE_PROXY:
-            await self.switch_proxy()
+            await self._switch_proxy()
         else:
             if delay < self.MAX_DELAY:
                 delay += 1
             else:
                 self.logger.debug("Reached max delay limit, try to use proxy")
             self.logger.info(f"Calling again, increasing delay to {delay}s")
 
         return delay
 
-    async def parse(self, session, url, delay):
+    async def _parse(self, url, delay):
         proxy = ''
         # setup new proxy, cuz old one was switched
         if self.USE_PROXY:
-            proxy = await self.get_proxy()
+            proxy = await self._get_proxy()
         else:
             # delay, only for non proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
-            async with session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
+            async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 403 or response.status == 404:
                     self.logger.debug("Got 403 forbitten")
-                    return False, await self.parse_error_handler(proxy, delay)
+                    return False, await self._parse_error_handler(delay)
 
                 # checking for challenge page.
                 result = await response.text()
-                if await self.cloudflare_check(result):
-                    return False, await self.parse_error_handler(proxy, delay)
+                if await self._cloudflare_check(result):
+                    return False, await self._parse_error_handler(delay)
 
                 return True, result
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
-            delay = await self.parse_error_handler(proxy, delay)
+            delay = await self._parse_error_handler(delay)
             return False, delay
 
-    async def fetch(self, url, delay: int = 0):
-        async with ClientSession() as session:
-            status = False
-            try_ = 1
-            while not status and (try_ != self.max_retries):
-                self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
-
-                # if status = True, result = page,
-                # if status = False result = delay (default=0)
-                status, result = await self.parse(session, url, delay)
-
-                if not status and result:
-                    delay = result
-                try_ += 1
-
-            if status == True:
-                loop = get_running_loop()
-                parsed = await loop.run_in_executor(None, partial(self.f, result))
-                return parsed
-            else:
-                self.logger.error('Connection failed')
-                return None
+    async def _fetch(self, url, delay: int = 0):
+        if not self.session:
+            await self._create_session()
+
+        status = False
+        try_ = 1
+        while not status and (try_ != self.max_retries):
+            self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
+
+            # if status = True, result = page,
+            # if status = False result = delay (default=0)
+            status, result = await self._parse(url, delay)
+
+            if not status and result:
+                delay = result
+            try_ += 1
+
+        if status == True:
+            loop = get_running_loop()
+            parsed = await loop.run_in_executor(None, partial(self._f, result))
+            return parsed
+        else:
+            self.logger.error('Connection failed')
+            return None
 
     def save_error(self, page):
         with open("error.html", "w") as file:
             file.write(page.prettify())
 
     @staticmethod
-    def normalize_date(parts) -> str:
+    def _normalize_date(parts) -> str:
         month_abbreviations = {
             'Jan': '1', 'Feb': '2', 'Mar': '3', 'Apr': '4',
             'May': '5', 'Jun': '6', 'Jul': '7', 'Aug': '8',
             'Sep': '9', 'Oct': '10', 'Nov': '11', 'Dec': '12'
         }
         month = month_abbreviations[parts[0]]
         day = parts[1][:-2]
         return day + '-' + month
 
+    # TODO rewrite
     async def get_live_matches(self):
         """returns a list of all LIVE matches on HLTV along with the maps being played and the star ratings"""
-        r = await self.fetch("https://www.hltv.org/matches")
+        r = await self._fetch("https://www.hltv.org/matches")
         if not r:
             return
 
         live_matches = r.find("div", {'class', "liveMatchesContainer"})
         if live_matches is None:
             return []
         else:
             teams = [line.getText() for line in live_matches.find_all("div", {'class', "matchTeamName text-ellipsis"})]
             matches = [(team1, team2) for team1, team2 in tuple(zip(teams, teams[1:]))[::2]]
             liveMatchContainer = live_matches.find_all("div", {'class', "liveMatch-container"})
             maps = [str(line.get('data-maps')).split(',') for line in liveMatchContainer]
             stars = [line.get('stars') for line in liveMatchContainer]
             return [{'teams': teams, 'maps': maps, 'stars': stars} for teams, maps, stars in zip(matches, maps, stars)]
 
-    async def get_upcoming_matches(self, days: int = 7, star_rating: int = 1):
+    async def get_upcoming_matches(self, days: int = 7, min_rating: int = 1):
         """returns a list of all upcoming matches on HLTV"""
-        r = await self.fetch("https://www.hltv.org/matches")
+        r = await self._fetch("https://www.hltv.org/matches")
         if not r:return
 
         matches = []
         try:
 
 
             for i, date_div in enumerate(r.find_all('div', {'class': 'upcomingMatchesSection'}), start=1):
@@ -217,15 +233,17 @@
                     break
                 date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
                 matches_today = []
 
                 for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
                     time_ = match.find('div', {'class': 'matchTime'}).text
                     rating = int(match['stars'])
-                    if rating >= star_rating:
+                    if rating >= min_rating:
+                        match_id_ = match.find('a')['href'].split('/')[2]
+
                         maps = match.find('div', {'class': 'matchMeta'}).text[-1:]
                         try:
                             teams = match.find_all('div', {'class': 'matchTeamName text-ellipsis'})
 
                             team1 = teams[0].text
                             team2 = teams[1].text
                         except (IndexError, AttributeError):
@@ -238,14 +256,15 @@
 
                             try:
                                 event = match.find('span', {'class': 'line-clamp-3'}).text
                             except AttributeError:
                                 event = ''
 
                         matches_today.append({
+                            'match_id': match_id_,
                             'team1': team1,
                             'team2': team2,
                             'time': time_,
                             'maps': maps,
                             'rating': rating,
                             'event': event
                     })
@@ -254,35 +273,70 @@
                     'date': date_,
                     'matches': matches_today
                 })
         except AttributeError:
             return None
         return matches
 
-    async def get_important_upcoming_matches(self, star_rating=1):
-        """returns a list of all upcoming matches on HLTV with the star rating argument (should be between 0 and 5)"""
-        r = await self.fetch("https://www.hltv.org/matches")
-        if not r:
-            return
 
-        teams = [line.getText() for line in r.find("div",
-                                                   {'class', "upcomingMatchesContainer"}).find_all(
-            class_=lambda v: v is not None and (v == "team text-ellipsis" or v == "matchTeamName text-ellipsis"))]
-        stars = [int(line.get('stars')) for line in r.find("div",
-                                                           {'class', "upcomingMatchesContainer"}).find_all("div",
-                                                                                                           {"class",
-                                                                                                            "upcomingMatch "})
-                 if line.get('team1') is not None]
-        matches = [(team1, team2) for team1, team2 in tuple(zip(teams, teams[1:]))[::2]]
-        # assert len(matches) == len(stars), "Internal Exception :: get_important_upcoming_matches() :: misMatches detected"
-        return [match for match, star in zip(matches, stars) if star == star_rating]
+    async def get_match_info(self, match_id: str, team1: str, team2: str, event_title: str, stats: bool = True):
+        r = await self._fetch(f"https://www.hltv.org/matches/{match_id}/"
+                             f"{team1.replace(' ', '-')}-vs-"
+                             f"{team2.replace(' ', '-')}-"
+                             f"{event_title.replace(' ', '-')}")
+
+
+        status = r.find('div', {'class': 'countdown'}).text
+
+        score1, score2 = 0, 0
+
+        if status == 'Match over':
+            scores = r.find_all('div', class_='team')
+            score1 = scores[0].get_text().replace('\n', '')[-1]
+            score2 = scores[1].get_text().replace('\n', '')[-1]
+
+
+        maps = []
+        for map_div in r.find_all('div', {'class': 'mapholder'}):
+
+                mapname = map_div.find('div', {'class': 'mapname'}).text
+                try:
+                    r_teams = map_div.find_all('div', {'class': 'results-team-score'})
+                    r_team1 = r_teams[0].text
+                    r_team2 = r_teams[1].text
+                except AttributeError:
+                    r_team1 = '0'
+                    r_team2 = '0'
+                maps.append({'mapname': mapname, 'r_team1': r_team1, 'r_team2': r_team2})
+
+        stats_ = []
+        if stats and status == 'Match over':
+            for table_div in r.find_all('table', {'class': 'table totalstats'})[:2]:
+                for player in table_div.find_all('tr')[1:]:
+                    player_id = player.find('a', class_='flagAlign')['href'].split('/')[2]
+                    player_name = player.find('div', class_='statsPlayerName').text.strip()
+                    nickname = re.findall(r"'(.*?)'", player_name)[0]
+
+                    kd = player.find('td', class_='kd').text.strip()
+                    adr = player.find('td', class_='adr').text.strip()
+                    rating = player.find('td', class_='rating').text.strip()
+                    stats_.append({
+                        'id': player_id,
+                        'name': nickname,
+                        'kd': kd,
+                        'adr': adr,
+                        'rating': rating
+                    })
+
+        return match_id, score1, score2, status, maps, stats
+
 
     async def get_big_results(self, offset=0) -> list[dict[str, Any]] | None:
-        """returns a list of results from past 100 matches on HLTV starting from the offset param"""
-        r = await self.fetch("https://www.hltv.org/results?offset=" + str(offset))
+        """returns a list of big event matches results"""
+        r = await self._fetch("https://www.hltv.org/results?offset=" + str(offset))
         if not r:
             return
 
         big_results = []
         big_res = r.find("div", {'class', "big-results"}).find_all("div", {"class", "result-con"})
         if not big_res:
             return None
@@ -300,87 +354,97 @@
                 'score1': s_t1,
                 'score2': s_t2,
             })
 
         return big_results
 
     async def get_event_results(self, event: int | str) -> list[dict[str, Any]] | None:
-        r = await self.fetch("https://www.hltv.org/results?event=" + str(event))
+        r = await self._fetch("https://www.hltv.org/results?event=" + str(event))
         if not r:
             return
 
         match_results = []
 
         for result in r.find("div", {'class', 'results-holder'}).find_all("div", {'class', 'results-sublist'}):
             date = result.find("span", class_="standard-headline").text.strip()
-            matches = result.find_all("div", class_="result-con")
-
-            for match in matches:
+            match_date = []
+            for match in result.find_all("a", class_="a-reset"):
+                id_ = match['href'].split('/')[2]
                 teams = match.find_all("div", class_="team")
                 team1 = teams[0].text.strip()
                 team2 = teams[1].text.strip()
 
                 scores = match.find("td", class_="result-score").text.strip().split('-')
                 score_t1 = scores[0].strip()
                 score_t2 = scores[1].strip()
 
-                match_results.append({
-                    'date': date,
+                match_date.append({
+                    'id': id_,
                     'team1': team1,
                     'team2': team2,
                     'score1': score_t1,
                     'score2': score_t2,
                 })
-
+            match_results.append({
+                'date': date,
+                'matches': match_date,
+            })
         return match_results
 
     async def get_event_matches(self, event_id: str | int):
-        r = await self.fetch("https://www.hltv.org/events/" + str(event_id) + "/matches")
+        r = await self._fetch("https://www.hltv.org/events/" + str(event_id) + "/matches")
         if not r:
             return
 
         live_matches: List | Any
         matches = []
         try:
             live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div", {'class', 'liveMatch'})
         except AttributeError:
             live_matches = []
-
+        live_mat = []
         for live in live_matches:
+            id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
 
             # TODO FIX SCORES
             try:
                 scores = live.find("td", class_="matchTeamScore").text.strip().split('-')
                 score_team1 = scores[0].strip()
                 score_team2 = scores[1].strip()
             except AttributeError:
                 score_team1 = 0
                 score_team2 = 0
 
-            matches.append({
+            live_mat.append({
+                'id': id_,
                 'team1': team1,
                 'team2': team2,
-                'date': 'LIVE'
             })
 
+        matches.append({
+            'date': 'LIVE',
+            'matches': live_mat,
+        })
+
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
             date_ = date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1]
-            for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
+            for match in date_sect.find_all('div', {'class': 'match a-reset'}):
                 teams = match.find_all("div", class_="matchTeamName text-ellipsis")
                 if teams or len(teams) > 1:
-
+                    id_ = match['href'].split('/')[2]
                     team1 = teams[0].text.strip()
                     team2 = teams[1].text.strip()
 
                     time_ = match.find('div', {'class', 'matchTime'}).text
 
                     matches.append({
+                        'id': id_,
                         'team1': team1,
                         'team2': team2,
                         'date': date_ + " " + time_
                     })
                 else:
                     break
 
@@ -392,27 +456,27 @@
         outgoing - include live tournaments
         future - include future tournamets
         max_events - use only if future=True
         :return:
         [('id', 'title', 'startdate', 'enddate')]
         """
 
-        r = await self.fetch('https://www.hltv.org/events')
+        r = await self._fetch('https://www.hltv.org/events')
         if not r:
             return
 
         events = []
         if outgoing:
             for event in r.find('div', {'class': 'tab-content', 'id': 'TODAY'}).find_all('a', {
                                 'class': 'a-reset ongoing-event'}):
                 event_name = event.find('div', {'class': 'text-ellipsis'}).text.strip()
-                event_start_date = self.normalize_date(
+                event_start_date = self._normalize_date(
                     event.find('span', {'data-time-format': 'MMM do'}).text.strip().split())
 
-                event_end_date = self.normalize_date(
+                event_end_date = self._normalize_date(
                     event.find_all('span', {'data-time-format': 'MMM do'})[1].text.strip().split())
                 event_id = event['href'].split('/')[-2]
 
                 events.append({
                     'id': event_id,
                     'name': event_name,
                     'start_date': event_start_date,
@@ -425,35 +489,35 @@
 
                     if i >= max_events:
                         break
 
                     event_id = event['href'].split('/')[-2]
                     event_name = event.find('div', {'class': 'big-event-name'}).text.strip()
                     # event_location = event.find('span', {'class': 'big-event-location'}).text.strip()
-                    event_start_date = self.normalize_date(event.find('span', {'class': ''}).text.strip().split())
-                    event_end_date = self.normalize_date(event.find('span', {'class': ''}).text.strip().split())
+                    event_start_date = self._normalize_date(event.find('span', {'class': ''}).text.strip().split())
+                    event_end_date = self._normalize_date(event.find('span', {'class': ''}).text.strip().split())
 
                     events.append({
                         'id': event_id,
                         'title': event_name,
                         'start_date': event_start_date,
                         'end_date': event_end_date
                     })
 
         return events
 
     async def get_event_info(self, event_id: str | int, event_title: str):
-        r = await self.fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
+        r = await self._fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
         if not r:
             return
 
         event_date_div = r.find('td', {'class', 'eventdate'}).find_all('span')
 
-        event_start = self.normalize_date(event_date_div[0].text.split())
-        event_end = self.normalize_date(event_date_div[1].text.split()[1:-1])
+        event_start = self._normalize_date(event_date_div[0].text.split())
+        event_end = self._normalize_date(event_date_div[1].text.split()[1:-1])
 
         prize = r.find('td', {'class', 'prizepool text-ellipsis'}).text
 
         team_num = r.find('td', {'class', 'teamsNumber'}).text
 
         location = r.find('td', {'class', 'location gtSmartphone-only'}).get_text().replace('\n', '')
 
@@ -482,15 +546,15 @@
         """
         today = date.today()
         current_weekday = today.weekday()
         last_monday = today - timedelta(days=current_weekday)
 
         teams = []
 
-        r = await self.fetch("https://www.hltv.org/ranking/teams/" + last_monday.strftime('%Y/%B/%d').lower())
+        r = await self._fetch("https://www.hltv.org/ranking/teams/" + last_monday.strftime('%Y/%B/%d').lower())
 
         if not r:
             return
 
         try:
             for i, team in enumerate(r.find_all("div", {'class': "ranked-team standard-box"}), start=1):
                 if i > max_teams:
@@ -502,31 +566,31 @@
                     title_div = team.find('div', {'class': 'teamLine sectionTeamPlayers'})
                 else:
                     title_div = team.find('div', {'class': 'teamLine sectionTeamPlayers teamLineExpanded'})
 
                 title = title_div.find('span', {'class': 'name'}).text
                 points = title_div.find('span', {'class': 'points'}).text.split(' ', 1)[0][1:]
 
-                id = team.find('a', {'class': 'details moreLink'})['href'].split('/')[-1]
+                id_ = team.find('a', {'class': 'details moreLink'})['href'].split('/')[-1]
 
                 changes = {'change positive', 'change neutral', 'change negative'}
                 change = ''
                 for change_ in changes:
                     try:
                         change = team.find('div', {'class', change_}).text
                         break
                     except AttributeError:
                         pass
 
                 teams.append({
+                    'id': id_,
                     'rank': rank,
                     'title': title,
                     'points': points,
                     'change': change,
-                    'id': id
                 })
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
         return teams
 
     async def get_team_info(self, team_id: int | str, title: str) -> tuple | None:
@@ -535,15 +599,15 @@
         :params:
         team_id: int | str
         title: str
         :returns:
         (team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys) | None
         weeks - weeks in top 20
         """
-        r = await self.fetch("https://www.hltv.org/team/" + str(team_id) + '/' + title.replace(' ', '-'))
+        r = await self._fetch("https://www.hltv.org/team/" + str(team_id) + '/' + title.replace(' ', '-'))
         players = []
         try:
             for player in r.find_all('span', {'class': 'text-ellipsis bold'}):
                 players.append(player.text)
 
             rank = '0'
             weeks = '0'
@@ -578,25 +642,27 @@
         :params:
         top: int = 40
         :returns:
         ('rank', 'name', 'team', 'maps', 'rating')
         maps - maps played
         """
         year = datetime.strftime(datetime.utcnow(), '%Y')
-        r = await self.fetch(
+        r = await self._fetch(
             f"https://www.hltv.org/stats/players?startDate={year}-01-01&endDate={year}-12-31&rankingFilter=Top20")
 
         if not r:
             return
 
         players = []
         rank = 1
         try:
             for player in r.find('tbody').find_all('tr'):
-                name = player.find('td', {'class', 'playerCol'}).find('a').text
+                name_div = player.find('td', {'class', 'playerCol'}).find('a')
+                id_ = name_div['href'].split('/')[3]
+                name = name_div.text
                 team = player.find('td', {'class', 'teamCol'})['data-sort']
 
                 maps = player.find('td', {'class', 'statsDetail'}).text
 
                 ratings = {'ratingCol ratingPositive', 'ratingCol ratingNeutral', 'ratingCol ratingNegative'}
                 rating = 'ERROR'
                 for rat in ratings:
@@ -604,14 +670,15 @@
                         rating = player.find('td', {'class', rat}).text
 
                         break
                     except AttributeError:
                         pass
 
                 players.append({
+                    'id': id_,
                     'rank': rank,
                     'name': name,
                     'team': team,
                     'maps': maps,
                     'rating': rating,
                 })
                 rank += 1
@@ -619,15 +686,15 @@
                     break
         except AttributeError:
             raise AttributeError("Top players parsing error, probably page not fully loaded")
 
         return players
 
     async def get_last_news(self, max_reg_news=2, only_today=True, only_featured=False):
-        r = await self.fetch('https://www.hltv.org/')
+        r = await self._fetch('https://www.hltv.org/')
 
         today = datetime.now(tz=pytz.timezone('Europe/Copenhagen'))
         article_days = {
             1: today.strftime('%d-%m'),
             2: (today - timedelta(days=1)).strftime('%d-%m'),
             3: 'old'
         }
@@ -674,13 +741,13 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv(use_proxy=True, proxy_path='proxies.txt', debug=True, one_time_proxy=True, proxy_protocol='http')
-
-    print(await hltv.get_last_news(only_today=True, max_reg_news=1))
+    #hltv = Hltv(use_proxy=True, proxy_path='proxies.txt', debug=True, proxy_one_time=True, proxy_protocol='http')
+    hltv = Hltv()
+    print(await hltv.get_match_info('2370727', 'faze', 'natus-vincere', 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.3.1/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.4.0b0/hltv_async_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.3.1
+Version: 0.4.0b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.3.1/pyproject.toml` & `hltv_async_api-0.4.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.3.1"
+version = "0.4.0b0"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.3.1/setup.py` & `hltv_async_api-0.4.0b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.3.1',
+    version='0.4.0b0',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```


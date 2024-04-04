# Comparing `tmp/nonebot_plugin_cnrail-0.2.0.tar.gz` & `tmp/nonebot_plugin_cnrail-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cnrail-0.2.0.tar", last modified: Sun Mar 10 10:16:45 2024, max compression
+gzip compressed data, was "nonebot_plugin_cnrail-0.2.1.tar", last modified: Thu Apr  4 09:04:51 2024, max compression
```

## Comparing `nonebot_plugin_cnrail-0.2.0.tar` & `nonebot_plugin_cnrail-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/LICENSE
--rw-r--r--   0        0        0     4166 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/README.md
--rw-r--r--   0        0        0      681 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/__init__.py
--rw-r--r--   0        0        0     3633 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/__main__.py
--rw-r--r--   0        0        0      152 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/config.py
--rw-r--r--   0        0        0     6146 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/data_source.py
--rw-r--r--   0        0        0     3146 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/models.py
--rw-r--r--   0        0        0    16091 2024-03-10 10:16:33.573932 nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/templates/train_table.html.jinja
--rw-r--r--   0        0        0      811 2024-03-10 10:16:45.329911 nonebot_plugin_cnrail-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4601 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/README.md
+-rw-r--r--   0        0        0      681 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__init__.py
+-rw-r--r--   0        0        0     3938 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__main__.py
+-rw-r--r--   0        0        0      308 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/config.py
+-rw-r--r--   0        0        0     5526 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/data_source.py
+-rw-r--r--   0        0        0     5038 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/models.py
+-rw-r--r--   0        0        0    15513 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/templates/train_table.html.jinja
+-rw-r--r--   0        0        0      808 2024-04-04 09:04:51.320196 nonebot_plugin_cnrail-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_cnrail-0.2.0/LICENSE` & `nonebot_plugin_cnrail-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.0/README.md` & `nonebot_plugin_cnrail-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -100,15 +100,17 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-暂无
+|         配置项         | 必填 |              默认值               |              说明              |
+| :--------------------: | :--: | :-------------------------------: | :----------------------------: |
+| `CNRAIL_ACG_IMAGE_URL` |  否  | `https://www.loliapi.com/acg/pe/` | 用于指令返回图片背景的图片 URL |
 
 ## 🎉 使用
 
 使用指令 `train -h` 查看帮助
 
 ### 效果图
 
@@ -141,14 +143,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.1
+
+- 适配 [MoeFactory API](https://train.moefactory.com)
+- 新增配置项 `CNRAIL_ACG_IMAGE_URL`
+
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 样式微调
 
 ### 0.1.7
```

#### html2text {}

```diff
@@ -9,28 +9,32 @@
 ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-cnrail ``` pdm ```bash pdm add nonebot-
 plugin-cnrail ``` poetry ```bash poetry add nonebot-plugin-cnrail ``` conda
 ```bash conda install nonebot-plugin-cnrail ``` æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® ææ  ## ð ä½¿ç¨
-ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾](https://
-raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ## ð
-èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+"nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
+| è¯´æ | | :--------------------: | :--: | :-------------------------------:
+| :----------------------------: | | `CNRAIL_ACG_IMAGE_URL` | å¦ | `https://
+www.loliapi.com/acg/pe/` | ç¨äºæä»¤è¿åå¾çèæ¯çå¾ç URL | ##
+ð ä½¿ç¨ ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ##
+ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
 robot/qunshare?robot_uin=3889001607) & [Train-QQbot æä»¶](https://github.com/
 staytomorrow/FindTrain) çµææ¥æº ### [12306](https://www.12306.cn)
 æ°æ®æ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ ·å¼å¾®è° ### 0.1.7 -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.1 - éé [MoeFactory API]
+(https://train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ###
+0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
 æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
 ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
 h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
 fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
 ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
 Create this project
```

### Comparing `nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/__init__.py` & `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __plugin_meta__ = PluginMetadata(
     name="CNRail",
     description="查询 12306 列车时刻表",
     usage="使用指令 train -h 查看帮助",
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/__main__.py` & `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,34 @@
 from arclet.alconna import Alconna, Args, Arparma, CommandMeta
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from httpx import TimeoutException
 from nonebot import logger
 from nonebot_plugin_alconna import AlconnaMatcher, CommandResult, on_alconna
 from nonebot_plugin_alconna.uniseg import UniMessage
 
-from .data_source import MultipleTrainFoundError, query_train_info, render_train_info
+from .data_source import (
+    MultipleTrainFoundError,
+    generate_word,
+    query_train_info,
+    render_train_info,
+)
 
 
 def parse_date(date_str: str) -> date:
     # use local timezone
     for x in string.whitespace:
         date_str = date_str.replace(x, "")
     today_date = date.today()  # noqa: DTZ011
 
     def parse(df: str) -> Optional[date]:
         with suppress(ValueError):
             parsed = (
-                datetime.strptime(date_str, df).replace(year=today_date.year).date()  # noqa: DTZ007
+                datetime.strptime(date_str, df)
+                .replace(year=today_date.year)
+                .date()  # noqa: DTZ007
             )
             if parsed < today_date:
                 parsed = parsed.replace(year=today_date.year + 1)
             return parsed
         return None
 
     date_formats = ("%m/%d", "%m-%d", "%m月%d日", "%m月%d号", "%m月%d")
@@ -63,23 +70,30 @@
 @search_train_info.handle()
 async def _(matcher: AlconnaMatcher, parma: Arparma):
     train_no: str = parma["train"]
     train_date: Optional[str] = parma["date"]
 
     try:
         # use local timezone
-        date_obj = parse_date(train_date) if train_date else date.today()  # noqa: DTZ011
+        date_obj = (
+            parse_date(train_date) if train_date else date.today()
+        )  # noqa: DTZ011
     except ValueError:
         await matcher.finish("日期格式不正确")
 
     try:
         train_info = await query_train_info(train_no, date_obj.isoformat())
     except MultipleTrainFoundError as e:
         much_text = "\n结果过多，仅显示前五个" if len(e.trains) > 5 else ""
-        info_text = "\n".join(x.word for x in e.trains[:5])
+        info_text = "\n".join(
+            [
+                await generate_word(train_code=i, train_date=date_obj.isoformat())
+                for i in e.trains[:5]
+            ],
+        )
         await matcher.finish(
             f"查询到多个车次，请检查您的车次是否正确\n{info_text}{much_text}",
         )
     except TimeoutException:
         await matcher.finish("查询超时，请稍后重试")
     except Exception:
         logger.exception("Failed to query train info")
@@ -90,13 +104,16 @@
             "\n（可查询日期范围一般为前二日 ~ 后十四日）" if train_date else ""
         )
         await matcher.finish(
             f"未查询到车次，可能是当日未开行，请检查您的车次是否正确{with_date_tip}",
         )
 
     try:
-        img_bytes = await render_train_info(train_info)
+        img_bytes = await render_train_info(
+            return_data=train_info,
+            train_date=date_obj.isoformat(),
+        )
     except Exception:
         logger.exception("Failed to render train info")
         await matcher.finish("渲染图片时出现错误，请检查后台输出")
 
     await matcher.finish(UniMessage.image(raw=img_bytes))
```

### Comparing `nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/data_source.py` & `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/data_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,181 +1,156 @@
-from datetime import datetime
 from pathlib import Path
 from typing import List, Optional
 
 import httpx
 import jinja2
 import pytz
 from nonebot import logger
 from nonebot.compat import type_validate_python
 from nonebot_plugin_htmlrender import get_new_page
 from playwright.async_api import Request, Route
 
-from .models import TrainInfo, TrainStation, TrainSummary
+from .config import config
+from .models import ReturnData, TrainDetailData, TrainSearchResult, TrainSNData
 
-CHINA_RAIL_SEARCH_API = "https://search.12306.cn/search/v1/train/search"
-CHINA_RAIL_DETAIL_API = "https://kyfw.12306.cn/otn/queryTrainInfo/query"
-RAIL_RE_API = "https://api.rail.re/"
-
-CNRAIL_DATA_BASE_URL = "https://cnrail-data.baka.pub/data/"
-
-ACG_IMAGE_URL = "https://www.loliapi.com/acg/pe/"
+MOERAIL_API_BASE = "https://train.moefactory.com/api/"
 
 TEMPLATE_PATH = Path(__file__).parent / "templates" / "train_table.html.jinja"
 
 ROUTE_BASE_URL = "https://cnrail.nonebot/"
 ROUTE_IMAGE_URL = f"{ROUTE_BASE_URL}image"
 
 TZ_SHANGHAI = pytz.timezone("Asia/Shanghai")
 
 
 class MultipleTrainFoundError(Exception):
-    def __init__(self, trains: List[TrainSummary]) -> None:
+    def __init__(self, trains: List[str]) -> None:
         self.trains = trains
         super().__init__(trains)
 
 
-async def query_emu_from_train_code(train_code: str) -> Optional[List]:
-    async with httpx.AsyncClient(base_url=RAIL_RE_API, follow_redirects=True) as client:
-        resp = await client.get(f"/train/{train_code}")
+async def generate_word(train_code: str, train_date: str) -> str:
+    async with httpx.AsyncClient(
+        base_url=MOERAIL_API_BASE,
+        follow_redirects=True,
+    ) as client:
+        resp = await client.post(
+            url="/trainNumber/query",
+            data={
+                "date": train_date.replace("-", ""),
+                "trainNumber": train_code,
+            },
+        )
         resp.raise_for_status()
-
-    data = resp.json()
-    if not data:
-        return None
-
-    return data
+        result = type_validate_python(TrainSearchResult, resp.json()["data"])
+    return f"{result.data[0].train_number} | {result.data[0].begin_station_name} - {result.data[0].end_station_name} | 耗时 {result.data[0].duration_minutes} 分钟"
 
 
-async def query_emu_from_emu_no(emu_no: str) -> Optional[List]:
-    async with httpx.AsyncClient(base_url=RAIL_RE_API, follow_redirects=True) as client:
-        resp = await client.get(f"/emu/{emu_no}")
+async def get_train_sn(train_code: str) -> Optional[List[TrainSNData]]:
+    async with httpx.AsyncClient(
+        base_url=MOERAIL_API_BASE,
+        follow_redirects=True,
+    ) as client:
+        resp = await client.post(
+            url="/crTrainSN/query",
+            data={
+                "keyword": train_code,
+            },
+        )
         resp.raise_for_status()
+    return (
+        type_validate_python(List[TrainSNData], resp.json()["data"])
+        if resp.json()["data"]
+        else None
+    )
 
-    data = resp.json()
-    if not data:
-        return None
-
-    return data
-
-
-async def query_train_info(train_code: str, train_date: str) -> Optional[TrainInfo]:
-    train_code = train_code.upper()
-
-    async def get_search_data(train_code: str, train_date: str) -> Optional[List]:
-        async with httpx.AsyncClient(follow_redirects=True) as client:
-            resp = await client.get(
-                CHINA_RAIL_SEARCH_API,
-                params={
-                    "keyword": train_code,
-                    "date": train_date.replace("-", ""),
-                },
-            )
-            resp.raise_for_status()
 
-        return resp.json()["data"]
+async def query_train_info(
+    train_code: str,
+    train_date: str,
+) -> Optional[ReturnData]:
+    async with httpx.AsyncClient(
+        base_url=MOERAIL_API_BASE,
+        follow_redirects=True,
+    ) as client:
+        resp = await client.post(
+            url="/trainNumber/query",
+            data={
+                "date": train_date.replace("-", ""),
+                "trainNumber": train_code,
+            },
+        )
+        resp.raise_for_status()
+        result = type_validate_python(TrainSearchResult, resp.json()["data"])
 
-    raw_data = await get_search_data(train_code=train_code, train_date=train_date)
-    if not raw_data:
+    if result.total_count != 1 and result.data[0].train_number != train_code:
         async with httpx.AsyncClient(
-            base_url=CNRAIL_DATA_BASE_URL,
+            base_url=MOERAIL_API_BASE,
             follow_redirects=True,
         ) as client:
-            resp = await client.get("/alias.json")
+            resp = await client.post(
+                url="/search/getTrainCandidates",
+                data={
+                    "keywords": train_code,
+                },
+            )
             resp.raise_for_status()
+            result = resp.json()["data"]
+            if not result:
+                return None
+            raise MultipleTrainFoundError(result)
 
-        try:
-            train_code = resp.json()[train_code]
-        except KeyError:
-            return None
-
-        raw_data = await get_search_data(train_code=train_code, train_date=train_date)
-        if not raw_data:
-            return None
-
-    data = type_validate_python(List[TrainSummary], raw_data)
-    if len(data) > 1:
-        summary = next(
-            (train for train in data if train.station_train_code == train_code),
-            None,
-        )
-        if not summary:
-            raise MultipleTrainFoundError(data)
-    else:
-        summary = data[0]
-
-    if summary.station_train_code != train_code:
-        return None
-
-    async with httpx.AsyncClient(follow_redirects=True) as client:
-        resp = await client.get(
-            CHINA_RAIL_DETAIL_API,
-            params={
-                "leftTicketDTO.train_no": summary.train_no,
-                "leftTicketDTO.train_date": train_date,
-                "rand_code": "",
-            },
-        )
-        resp.raise_for_status()
-
-    raw_data = resp.json()["data"]["data"]
-    if not raw_data:
-        return None
-
-    stations = type_validate_python(List[TrainStation], raw_data)
+    search_data = result.data[0]
 
     async with httpx.AsyncClient(
-        base_url=CNRAIL_DATA_BASE_URL,
+        base_url=MOERAIL_API_BASE,
         follow_redirects=True,
     ) as client:
-        resp = await client.get("/maintance.json")
+        resp = await client.post(
+            url="/trainDetails/query",
+            data={
+                "date": train_date.replace("-", ""),
+                "trainIndex": search_data.train_index,
+            },
+        )
         resp.raise_for_status()
 
-    maintancer = resp.json()[train_code]
-
-    today_date = datetime.now(TZ_SHANGHAI).date()
-    train_date_obj = (
-        datetime.strptime(train_date, "%Y-%m-%d").replace(tzinfo=TZ_SHANGHAI).date()
-    )
+    datail_data = type_validate_python(TrainDetailData, resp.json()["data"])
 
-    emu_no = None
+    sn_data = await get_train_sn(train_code)
 
-    if (train_date_obj <= today_date) and (
-        emu_data := await query_emu_from_train_code(train_code)
-    ):
-        for i in emu_data:
-            date_data = (
-                datetime.strptime(i["date"], "%Y-%m-%d %H:%M")
-                .replace(tzinfo=TZ_SHANGHAI)
-                .date()
-            )
-            if date_data == train_date_obj:
-                emu_no = i["emu_no"]
-                break
-
-    return TrainInfo(
-        summary=summary,
-        stations=stations,
-        maintancer=maintancer,
-        emu_no=emu_no,
+    return ReturnData(
+        search=search_data,
+        datail=datail_data,
+        sn=sn_data,
+        train_date=train_date,
     )
 
 
-async def render_train_info(info: TrainInfo) -> bytes:
+async def render_train_info(return_data: ReturnData, train_date: str) -> bytes:
     template = jinja2.Template(
         TEMPLATE_PATH.read_text(encoding="u8"),
         enable_async=True,
     )
-    html = await template.render_async(info=info)
+    html = await template.render_async(
+        summary=return_data.search,
+        detail=return_data.datail,
+        sn=(
+            next((i.train_sn for i in return_data.sn if i.date == train_date), None)
+            if return_data.sn
+            else None
+        ),
+        train_date=return_data.train_date,
+    )
     if (dbg := Path.cwd() / "cnrail-debug.html").exists():
         dbg.write_text(html, encoding="u8")
 
     async def bg_router(route: Route, _: Request):
         async with httpx.AsyncClient(follow_redirects=True) as client:
-            resp = await client.get(ACG_IMAGE_URL)
+            resp = await client.get(config.CNRAIL_ACG_IMAGE_URL, follow_redirects=True)
         try:
             resp.raise_for_status()
         except Exception:
             logger.exception("Failed to fetch image")
             await route.abort()
         else:
             await route.fulfill(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_cnrail-0.2.0/nonebot_plugin_cnrail/templates/train_table.html.jinja` & `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/templates/train_table.html.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -176,23 +176,22 @@
       align-items: center;
     }
 
     .station-bottom {
       border-top: 1px solid var(--split-line-color);
       margin: 10px 20px;
       padding-top: 10px;
-      display: flex;
-      justify-content: space-between;
+      line-height: 1.7;
     }
 
     .admin,
     .emu_no {
-        font-size: 12px;
-        color: var(--top-sub-color);
-        text-align: left;
+      font-size: 12px;
+      color: var(--top-sub-color);
+      text-align: left;
     }
 
     .card-bottom {
       background-color: var(--bottom-bg-color);
     }
 
     .bottom-title {
@@ -285,54 +284,46 @@
 </head>
 
 <body>
   <div class="bg-wrapper">
     <div class="main">
       <div class="card-top">
         <div class="card-title">
-          {{ " / ".join(info.station_train_codes) }}
+          {{ summary.train_number }}
         </div>
         <div class="station">
           <div class="station-top">
             <div class="departure-station">
-              <div class="place">{{ info.summary.from_station }}</div>
+              <div class="place">{{ summary.begin_station_name }}</div>
               <div class="time">
                 <div class="departure-mark">始</div>
-                {{ info.stations[0].start_time }}
+                {{ summary.departure_time }}
               </div>
             </div>
             <div class="arrow-box">
-              {% set total_time = info.total_time -%}
-              {%- if info.arrive_next_day -%}
-              <div class="duration">历时 {{ total_time[0] }} 时 {{ total_time[1] }} 分</div>
-              <div class="arrow-icon">
-                <div class="line"></div>
-                <div class="triangle"></div>
-              </div>
-              {%- else -%}
-              <div class="date">{{ info.date_summary }}</div>
+              <div class="duration">历时 {{ summary.pass_time }}</div>
               <div class="arrow-icon">
                 <div class="line"></div>
                 <div class="triangle"></div>
               </div>
-              <div class="duration">历时 {{ total_time[0] }} 时 {{ total_time[1] }} 分</div>
-              {%- endif %}
             </div>
             <div class="terminal-station">
-              <div class="place">{{ info.summary.to_station }}</div>
+              <div class="place">{{ summary.end_station_name }}</div>
               <div class="time">
-                {{ info.stations[-1].arrive_time }}
+                {{ summary.arrival_time }}
                 <div class="terminal-mark">终</div>
               </div>
             </div>
           </div>
           <div class="station-bottom">
-            <div class="admin">担当路局：{{ info.maintancer }}</div>
-            {%- if info.emu_no -%}
-            <div class="emu_no">车组号：{{ info.emu_no }}</div>
+            <div class="admin">担当路局：{{ detail.company_name }}</div>
+            {%- if sn -%}
+            <div class="emu_no">车组号：{{ sn }}</div>
+            {%- else -%}
+            <div class="emu_no">列车型号：{{ detail.routing.train_model }}</div>
             {%- endif %}
           </div>
         </div>
       </div>
 
       <div class="card-bottom">
         <div class="bottom-title">经停站</div>
@@ -345,30 +336,29 @@
                 <th>开点</th>
                 <th>到点</th>
                 <th>停留</th>
                 <th>车次</th>
               </tr>
             </thead>
             <tbody>
-              {% for station in info.stations -%}
+              {% for station in detail.via_stations -%}
               <tr>
                 <td>
-                  <div class="station-point{% if info.arrived(loop.index0) %} arrived{% endif %}"></div>
+
+                  <div class="station-point{% if detail.arrived(loop.index0, train_date) %} arrived{% endif %}"></div>
                 </td>
                 <td>{{ station.station_name }}</td>
                 <td>
-                  {%- if station.start_time.startswith("-") %}{{ station.arrive_time }}
-                  {%- else %}{{ station.start_time }}{% endif -%}
+                  {% if loop.first %}-{% else %}{{ station.arrival_time}}{% endif %}
                 </td>
                 <td>
-                  {%- if station.arrive_time.startswith("-") %}{{ station.start_time }}
-                  {%- else %}{{ station.arrive_time }}{% endif -%}
+                  {% if loop.last %}-{% else %}{{ station.departure_time }}{% endif %}
                 </td>
-                <td>{% if loop.first %}始发站{% elif loop.last %}终点站{% else %}{{ station.stay_minutes }} 分{% endif %}</td>
-                <td>{{ station.station_train_code }}</td>
+                <td>{% if loop.first %}始发站{% elif loop.last %}终点站{% else %}{{ station.stop_minutes }} 分{% endif %}</td>
+                <td>{{ station.train_number }}</td>
               </tr>
               {% endfor -%}
             </tbody>
           </table>
         </div>
       </div>
     </div>
@@ -591,8 +581,8 @@
     doneDivElem.id = 'done';
     document.body.appendChild(doneDivElem);
   }
 
   main();
 </script>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
-{{ " / ".join(info.station_train_codes) }}
-{{ info.summary.from_station }}
+{{ summary.train_number }}
+{{ summary.begin_station_name }}
 始
-{{ info.stations[0].start_time }}
-{% set total_time = info.total_time -%} {%- if info.arrive_next_day -%}
-历时 {{ total_time[0] }} 时 {{ total_time[1] }} 分
-{%- else -%}
-{{ info.date_summary }}
-历时 {{ total_time[0] }} 时 {{ total_time[1] }} 分
-{%- endif %}
-{{ info.summary.to_station }}
-{{ info.stations[-1].arrive_time }}
+{{ summary.departure_time }}
+历时 {{ summary.pass_time }}
+{{ summary.end_station_name }}
+{{ summary.arrival_time }}
 终
-担当路局：{{ info.maintancer }}
-{%- if info.emu_no -%}
-车组号：{{ info.emu_no }}
+担当路局：{{ detail.company_name }}
+{%- if sn -%}
+车组号：{{ sn }}
+{%- else -%}
+列车型号：{{ detail.routing.train_model }}
 {%- endif %}
 经停站
- ?停?靠?站                  ?开?点                            ?到?点                             ?停?留                   ?车?次
-                      {%- if                        {%- if                         {% if loop.first
- {                    station.start_time.startswith station.arrive_time.startswith %}始发站{% elif         {
- {                    ("-") %}{                     ("-") %}{{ station.start_time  loop.last %}终点站{%    {
- station.station_name { station.arrive_time }} {%-  }} {%- else %}{                else %}{             station.station_train_code
- }}                   else %}{{ station.start_time  { station.arrive_time }}{%     {                    }}
-                      }}{% endif -%}                endif -%}                      station.stay_minutes
-                                                                                   }} 分{% endif %}
+ ?停?靠?站                  ?开?点                     ?到?点                     ?停?留                   ?车?次
+                                                                    {% if loop.first
+ {                    {% if loop.first %}-{% {% if loop.last %}-{%  %}始发站{% elif         {
+ {                    else %}{               else %}{               loop.last %}终点站{%    {
+ station.station_name {                      {                      else %}{             station.train_number
+ }}                   station.arrival_time}} station.departure_time {                    }}
+                      {% endif %}            }}{% endif %}          station.stop_minutes
+                                                                    }} 分{% endif %}
```

### Comparing `nonebot_plugin_cnrail-0.2.0/pyproject.toml` & `nonebot_plugin_cnrail-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
     { name = "XieXiLin", email = "support@xiexilin.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "httpx>=0.24",
-    "nonebot-plugin-alconna>=0.40.0rc1",
+    "nonebot-plugin-alconna>=0.40.1",
     "nonebot-plugin-htmlrender>=0.2.2",
     "jinja2>=3.1.2",
     "pytz>=2023.3.post1",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail"
```

### Comparing `nonebot_plugin_cnrail-0.2.0/PKG-INFO` & `nonebot_plugin_cnrail-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cnrail
-Version: 0.2.0
+Version: 0.2.1
 Summary: NoneBot2 plugin for query the train time table
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Author-Email: student_2333 <lgc2333@126.com>, XieXiLin <support@xiexilin.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: httpx>=0.24
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1
+Requires-Dist: nonebot-plugin-alconna>=0.40.1
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: pytz>=2023.3.post1
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
@@ -117,15 +117,17 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-暂无
+|         配置项         | 必填 |              默认值               |              说明              |
+| :--------------------: | :--: | :-------------------------------: | :----------------------------: |
+| `CNRAIL_ACG_IMAGE_URL` |  否  | `https://www.loliapi.com/acg/pe/` | 用于指令返回图片背景的图片 URL |
 
 ## 🎉 使用
 
 使用指令 `train -h` 查看帮助
 
 ### 效果图
 
@@ -158,14 +160,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.1
+
+- 适配 [MoeFactory API](https://train.moefactory.com)
+- 新增配置项 `CNRAIL_ACG_IMAGE_URL`
+
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 样式微调
 
 ### 0.1.7
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.1 Summary:
 NoneBot2 plugin for query the train time table Home-page: https://github.com/
 lgc-NB2Dev/nonebot-plugin-cnrail Author-Email: student_2333
 126.com>, XieXiLin
 xiexilin.com> License: MIT Project-URL: Homepage, https://github.com/lgc-
 NB2Dev/nonebot-plugin-cnrail Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: httpx>=0.24 Requires-Dist: nonebot-plugin-
-alconna>=0.40.0rc1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2 Requires-
-Dist: jinja2>=3.1.2 Requires-Dist: pytz>=2023.3.post1 Description-Content-Type:
-text/markdown
+alconna>=0.40.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2 Requires-Dist:
+jinja2>=3.1.2 Requires-Dist: pytz>=2023.3.post1 Description-Content-Type: text/
+markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # NoneBot-Plugin-CNRail _â¨ 12306 åè½¦æ¶å»è¡¨æ¥è¯¢æä»¶ â¨_[python]
                             _[_p_d_m_-_m_a_n_a_g_e_d_]_[_w_a_k_a_t_i_m_e_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
@@ -19,28 +19,32 @@
 ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-cnrail ``` pdm ```bash pdm add nonebot-
 plugin-cnrail ``` poetry ```bash poetry add nonebot-plugin-cnrail ``` conda
 ```bash conda install nonebot-plugin-cnrail ``` æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® ææ  ## ð ä½¿ç¨
-ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾](https://
-raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ## ð
-èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+"nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
+| è¯´æ | | :--------------------: | :--: | :-------------------------------:
+| :----------------------------: | | `CNRAIL_ACG_IMAGE_URL` | å¦ | `https://
+www.loliapi.com/acg/pe/` | ç¨äºæä»¤è¿åå¾çèæ¯çå¾ç URL | ##
+ð ä½¿ç¨ ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ##
+ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
 robot/qunshare?robot_uin=3889001607) & [Train-QQbot æä»¶](https://github.com/
 staytomorrow/FindTrain) çµææ¥æº ### [12306](https://www.12306.cn)
 æ°æ®æ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ ·å¼å¾®è° ### 0.1.7 -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.1 - éé [MoeFactory API]
+(https://train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ###
+0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
 æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
 ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
 h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
 fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
 ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
 Create this project
```


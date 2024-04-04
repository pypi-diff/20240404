# Comparing `tmp/segmentheepy_prak-1.0.0-py3-none-any.whl.zip` & `tmp/segmentheepy_prak-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10224 bytes, number of entries: 9
+Zip file size: 10589 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-31 09:33 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    23078 b- defN 24-Mar-18 12:22 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx    25467 b- defN 24-Apr-04 11:00 segmenthee/cart_api.py
 -rw-rw-r--  2.0 unx      766 b- defN 24-Mar-06 13:24 segmenthee/config.py
 -rw-rw-r--  2.0 unx     1979 b- defN 24-Mar-14 12:51 segmenthee/parser_api.py
 -rw-rw-r--  2.0 unx     9777 b- defN 24-Mar-18 11:06 segmenthee/shop.py
--rw-rw-r--  2.0 unx      258 b- defN 24-Mar-19 07:32 segmentheepy_prak-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-19 07:32 segmentheepy_prak-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 24-Mar-19 07:32 segmentheepy_prak-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      725 b- defN 24-Mar-19 07:32 segmentheepy_prak-1.0.0.dist-info/RECORD
-9 files, 36686 bytes uncompressed, 8970 bytes compressed:  75.5%
+-rw-rw-r--  2.0 unx      258 b- defN 24-Apr-04 11:49 segmentheepy_prak-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-04 11:49 segmentheepy_prak-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-04 11:49 segmentheepy_prak-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      725 b- defN 24-Apr-04 11:49 segmentheepy_prak-1.0.1.dist-info/RECORD
+9 files, 39075 bytes uncompressed, 9335 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_prak-1.0.0.dist-info/METADATA
+Filename: segmentheepy_prak-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_prak-1.0.0.dist-info/WHEEL
+Filename: segmentheepy_prak-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_prak-1.0.0.dist-info/top_level.txt
+Filename: segmentheepy_prak-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_prak-1.0.0.dist-info/RECORD
+Filename: segmentheepy_prak-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -26,14 +26,15 @@
 #collect name from classindex
 classnames = dict()
 
 params = {
     "clickrate": 0.75,
     "actionseparation": [0.5, 0.025],
     "actionaffinity": [0.5, 0.025],
+#    "categoryaffinity": [0.5, 0.025],
     "carttotaltrend": [0.5, 0.025],
     "cartcounttrend": [0.5, 0.025],
     "avgpricemanipulation": [0.5, 0.025],
     "lastpriceviewedtrend": [0.5, 0.025],
     "tabcounttrend": [0.5, 0.025],
     "redirectstrend": [0.5, 0.025],
     "tabtypetrend": [0.5, 0.025],
@@ -47,14 +48,15 @@
     global params
     for key in new_params:
         if key in params:
             params[key] = new_params[key]
     if verbose:
         print(params)
 
+# MAX_CATEGORY = 6
 tabtype_dict = {'New':0, 'Existing':1}
 navigation_dict = {'NAVIGATE':0,'FORWARD':1,'BACK':2,'RELOAD':3}
 origin_dict = {"facebook":0,"google":1,"shop":2}
 sort_dict = {'default': 0, 'price': 1, 'displayText': 2, 'popularityScore': 3}
 
 
 def get_navigation(navigation: str) -> int:
@@ -67,15 +69,15 @@
 
 def get_referrer(referrer: str) -> int:
     r = parser_api.parse_origin(referrer)
     return origin_dict.get(r, len(origin_dict))
 
 
 def get_sort(sort: str) -> int:
-    return sort_dict.get(parser_api.parse_sort(sort), len(sort_dict))
+    return sort_dict.get(parser_api.parse_sort(sort),len(sort_dict))
 
 
 def get_page(page: str) -> int:
     try:
         return int(page)
     except:
         return 0
@@ -97,14 +99,27 @@
 
 def get_cart_count(state: Dict[str, Any]) -> Union[Any, None]:
     return state.get('cartcount')
 
 
 # timeweights = json.load(open("vagyaim/timeweights.json"))
 
+# def LogCategory(retval,coeffs,category):
+#    if "categoryaffinity" not in retval:
+#        return None
+#    arr = retval["categoryaffinity"]
+#    categoryattfacts = coeffs["categoryaffinity"]
+#    for attix in range(len(categoryattfacts)):
+#        attfact = categoryattfacts[attix]
+#        for cat in range(MAX_CATEGORY):
+#            arr[attix][cat] *= attfact
+#    if category >= 0:
+#        for attix in range(len(categoryattfacts)):
+#            arr[attix][category] += 1 - categoryattfacts[attix]
+        
 def UpdateClickrates(retval,time,coeff,initialize=False):
     if "z_score" not in retval:
         return None
     if retval["clickrate_var"] > 0.0:
         retval["z_score"] = (time - retval["lastactioneventtime"] - retval["clickrate_avg"]) / (retval["clickrate_var"]**(1/2))
     if initialize:
         first_delta_time = retval["lastactioneventtime"] - retval["sessionstart"]
@@ -166,16 +181,16 @@
         return False
 
     def skip_update(self) -> bool:
         return False
 
     JSON_FIELDS: List[str] = [
         'time', 'delta_count', 'delta_total', 'event_label', 'referrer', 'tabcount', 'tabtype',
-        'navigation', 'redirects', 'title', 'utm_source', 'utm_medium', 'price', 'product_id',
-        'page', 'sort'
+        'navigation', 'redirects', 'title', 'utm_source', 'utm_medium', #'category_id', 
+        'price', 'product_id', 'page', 'sort'
     ]
 
     def to_dict(self, **kwargs) -> Dict[str, Any]:
         data = {key: value for (key, value) in vars(self).items() if key in SessionBodyEvent.JSON_FIELDS}
         data = {'constructor': self.__class__.__name__, **data, **kwargs}
         return data
 
@@ -302,24 +317,30 @@
 
 class MainPageBrowsingEvent(BrowsingEvent):
 
     cindex = nextclassindex()
     classnames[cindex] = "MainPageBrowsingEvent"
 
 class ProductPageBrowsingEvent(BrowsingEvent):
-    def __init__(self, time: int, price: int, referrer: int, tabcount: int, tabtype: int, navigation: int, redirects: int, title: str, utm_source: str, utm_medium: str, product_id: Any):
+    def __init__(self, time: int, # category_id: int, 
+                 price: int, referrer: int, tabcount: int, tabtype: int, navigation: int, redirects: int, 
+                 title: str, utm_source: str, utm_medium: str, product_id: Any):
         super().__init__(time,referrer,tabcount,tabtype,navigation,redirects,title,utm_source,utm_medium)
         self.product_id = product_id
+        # self.category_id = category_id
         self.price = price if price else 0
 
     cindex = nextclassindex()
     classnames[cindex] = "ProductPageBrowsingEvent"
 
     def Update(self,prevstate):
         retval = super().Update(prevstate)
+        # retval["lastcategory"] = self.category_id
+        # category = self.category_id
+        # LogCategory(retval,self.coeffs,category)
         retval["lastprice"] = self.price
         UpdateAttribute(retval, self.coeffs, "lastpriceviewedtrend", self.price)
         retval["producteverviewed"] = 1
         return retval
 
 
 class ProductPageScrollEvent(BrowsingEvent):
@@ -354,25 +375,52 @@
     
     def Update(self,prevstate):
         retval = super().Update(prevstate)
         UpdateAttribute(retval, self.coeffs, "sorttrend", self.sort)
         UpdateAttribute(retval, self.coeffs, "pagetrend", self.page)
         return retval
 
+# class CategoryPageBrowsingEvent(BrowsingEvent):
+#     def __init__(self, time: int, # category_id: int, 
+#                  referrer: int, tabcount: int, tabtype: int, navigation: int, redirects: int, title: str, 
+#                  utm_source: str, utm_medium: str, page: int, sort: int):
+#         super().__init__(time,referrer,tabcount,tabtype,navigation,redirects,title,utm_source,utm_medium)
+#         # self.category_id = category_id
+#         self.page = page
+#         self.sort = sort
+#
+#     cindex = nextclassindex()
+#     classnames[cindex] = "CategoryPageBrowsingEvent"
+#
+#     def Update(self,prevstate):
+#         retval = super().Update(prevstate)
+#         # retval["lastcategory"] = self.category_id
+#         # category = self.category_id
+#         # LogCategory(retval,self.coeffs,category)
+#         UpdateAttribute(retval, self.coeffs, "sorttrend", self.sort)
+#         UpdateAttribute(retval, self.coeffs, "pagetrend", self.page)
+#         return retval
+    
 class PredefinedFilterBrowsingEvent(BrowsingEvent):
-    def __init__(self, time: int, referrer: int, tabcount: int, tabtype: int, navigation: int, redirects: int, title: str, utm_source: str, utm_medium: str, page: int, sort: int):
+    def __init__(self, time: int, # category_id: int, 
+                 referrer: int, tabcount: int, tabtype: int, navigation: int, redirects: int, title: str, 
+                 utm_source: str, utm_medium: str, page: int, sort: int):
         super().__init__(time,referrer,tabcount,tabtype,navigation,redirects,title,utm_source,utm_medium)
+        # self.category_id = category_id
         self.page = page
         self.sort = sort
 
     cindex = nextclassindex()
     classnames[cindex] = "PredefinedFilterBrowsingEvent"
 
     def Update(self,prevstate):
         retval = super().Update(prevstate)
+        # retval["lastcategory"] = self.category_id
+        # category = self.category_id
+        # LogCategory(retval,self.coeffs,category)
         UpdateAttribute(retval, self.coeffs, "sorttrend", self.sort)
         UpdateAttribute(retval, self.coeffs, "pagetrend", self.page)
         return retval
     
 class InformationPageBrowsingEvent(BrowsingEvent):
 
     cindex = nextclassindex()
@@ -504,14 +552,16 @@
         "clickrate_squares": 0.0,
         "clickrate_var": 0.0,
         "z_score": 0.0,
         "sessionstatus": "Browsing",
         "clickrate": 0.0,
         "actionseparation": [0.0] * len(params["actionseparation"]),
         "actionaffinity": [[1/classcount] * classcount for _ in range(len(params["actionaffinity"]))],
+        # "lastcategory": None,
+        # "categoryaffinity": [[1/MAX_CATEGORY] * MAX_CATEGORY for _ in range(len(params["categoryaffinity"]))],
         "carttotal":0.0,
         "cartcount":0,
         "carttotaltrend": [0.0] * len(params["carttotaltrend"]),
         "cartcounttrend": [0.0] * len(params["cartcounttrend"]),
         "cartmodification": 0.0,
         "avgpricemanipulation": [0.0] * len(params["avgpricemanipulation"]),
         "couponstatus": 0,
@@ -548,14 +598,19 @@
         row["actionseparation_" + str(i)] = arr[i]
 
     arr = state["actionaffinity"]
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             row["actionaffinity_" + str(i) + "_" + classnames[j]] = arr[i][j]
 
+#    arr = state["categoryaffinity"]
+#    for i in range(len(arr)):
+#        for j in range(len(arr[0])):
+#            row["categoryaffinity_" + str(i) + "_" + str(j)] = arr[i][j]
+            
     arr = state["carttotaltrend"]
     for i in range(len(arr)):
         row["carttotaltrend_" + str(i)] = arr[i]
 
     arr = state["cartcounttrend"]
     for i in range(len(arr)):
         row["cartcounttrend_" + str(i)] = arr[i]
```

## Comparing `segmentheepy_prak-1.0.0.dist-info/RECORD` & `segmentheepy_prak-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 segmenthee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-segmenthee/cart_api.py,sha256=mEKAgRcK0UouwcrbC-dAuQ8q3jYVtjzPIrkWq7RZA7Q,23078
+segmenthee/cart_api.py,sha256=qM3_6LWZLaBhTX35_xibUdpFbljOfFZPLqhxblOIWwY,25467
 segmenthee/config.py,sha256=lXea6JINCK44eZP38JaQOlfgVerzFx0e9wDxObuw54c,766
 segmenthee/parser_api.py,sha256=tT6-_lOLLxIclnhXORg83LBP-hNJtlwsjZfivnn5jRk,1979
 segmenthee/shop.py,sha256=2dyYkOYmGvQsgHnUdcU97KngdjBhvWirPjWPwDlAKew,9777
-segmentheepy_prak-1.0.0.dist-info/METADATA,sha256=eepfMGfSgblxKzzfI6dafjZw091tZFFgI4vQkM0kIlk,258
-segmentheepy_prak-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-segmentheepy_prak-1.0.0.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
-segmentheepy_prak-1.0.0.dist-info/RECORD,,
+segmentheepy_prak-1.0.1.dist-info/METADATA,sha256=k_UfjnnOIBi1yqEx01LwFjIEPipGbNUrTbcLB4xWXBQ,258
+segmentheepy_prak-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+segmentheepy_prak-1.0.1.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
+segmentheepy_prak-1.0.1.dist-info/RECORD,,
```


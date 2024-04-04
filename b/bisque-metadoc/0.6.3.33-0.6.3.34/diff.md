# Comparing `tmp/bisque_metadoc-0.6.3.33-py3-none-any.whl.zip` & `tmp/bisque_metadoc-0.6.3.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11763 bytes, number of entries: 10
--rw-r--r--  2.0 unx      169 b- defN 24-Jan-06 00:51 bq/metadoc/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-Jan-06 00:51 bq/metadoc/etree.py
--rw-r--r--  2.0 unx    28237 b- defN 24-Jan-06 00:51 bq/metadoc/formats.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Jan-06 00:51 bq/metadoc/logging.py
--rw-r--r--  2.0 unx      418 b- defN 24-Jan-06 00:51 bq/metadoc/version.py
--rw-r--r--  2.0 unx     4486 b- defN 24-Jan-06 00:51 bq/metadoc/xmldict.py
--rw-r--r--  2.0 unx      764 b- defN 24-Jan-06 00:51 bisque_metadoc-0.6.3.33.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-06 00:51 bisque_metadoc-0.6.3.33.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-Jan-06 00:51 bisque_metadoc-0.6.3.33.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      802 b- defN 24-Jan-06 00:51 bisque_metadoc-0.6.3.33.dist-info/RECORD
-10 files, 38491 bytes uncompressed, 10395 bytes compressed:  73.0%
+Zip file size: 12279 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      169 b- defN 24-Apr-04 05:15 bq/metadoc/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-Apr-04 05:15 bq/metadoc/etree.py
+-rw-r--r--  2.0 unx    28221 b- defN 24-Apr-04 05:15 bq/metadoc/formats.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-04 05:15 bq/metadoc/logging.py
+-rw-r--r--  2.0 unx      418 b- defN 24-Apr-04 05:15 bq/metadoc/version.py
+-rw-r--r--  2.0 unx     6187 b- defN 24-Apr-04 05:15 bq/metadoc/xmldict.py
+-rw-r--r--  2.0 unx      764 b- defN 24-Apr-04 05:15 bisque_metadoc-0.6.3.34.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 05:15 bisque_metadoc-0.6.3.34.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 24-Apr-04 05:15 bisque_metadoc-0.6.3.34.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      802 b- defN 24-Apr-04 05:15 bisque_metadoc-0.6.3.34.dist-info/RECORD
+10 files, 40176 bytes uncompressed, 10911 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bq/metadoc/version.py
 Comment: 
 
 Filename: bq/metadoc/xmldict.py
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.33.dist-info/METADATA
+Filename: bisque_metadoc-0.6.3.34.dist-info/METADATA
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.33.dist-info/WHEEL
+Filename: bisque_metadoc-0.6.3.34.dist-info/WHEEL
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.33.dist-info/top_level.txt
+Filename: bisque_metadoc-0.6.3.34.dist-info/top_level.txt
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.33.dist-info/RECORD
+Filename: bisque_metadoc-0.6.3.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bq/metadoc/formats.py

```diff
@@ -17,14 +17,21 @@
     from collections import MutableMapping
 
 import re
 
 import simplejson as json
 from lxml import etree
 
+try:
+    _etree_string_result_types = (etree._ElementUnicodeResult, etree._ElementStringResult)
+except AttributeError:
+    # lxml versions >= 5.1.1 removed _ElementStringResult
+    _etree_string_result_types = (etree._ElementUnicodeResult,)
+
+
 from .xmldict import d2xml, xml2d
 
 log = logging.getLogger("bq.metadoc.formats")
 
 
 # set following to True to force Metadoc everywhere
 metadoc_everywhere = False
@@ -221,21 +228,19 @@
     pass
 
 
 def _clean_tree(elem, del_uri=True):
     res = copy.deepcopy(elem)
     _clean_tree_rec(res, del_uri=del_uri)
     return res
-    
+
 def _clean_tree_rec(elem, del_uri=True):
-    if "_id" in elem.attrib:
-        del elem.attrib["_id"]
+    elem.attrib.pop("_id", None)
     if del_uri is True:
-        if "uri" in elem.attrib:
-            del elem.attrib["uri"]
+        elem.attrib.pop("uri", None)
     for kid in elem:
         _clean_tree_rec(kid, del_uri=del_uri)
 
 
 def _tree_to_naturalxml(tree, keep_text=False):
     """WARNING: MODIFIES TREE IN PLACE!"""
     for node in tree.iter(tag=etree.Element):
@@ -498,17 +503,15 @@
     def convert(internal):
         if isinstance(internal, Metadoc):
             return internal
         if isinstance(internal, etree._Element):
             return Metadoc(et=internal)
         elif isinstance(internal, etree._ElementTree):
             return Metadoc(et=internal.getroot())
-        elif isinstance(
-            internal, (etree._ElementUnicodeResult, etree._ElementStringResult)
-        ):
+        elif isinstance(internal, _etree_string_result_types):
             return str(internal)
         elif isinstance(internal, list):
             return [Metadoc.convert(it) for it in internal]
         elif not internal:  # None, empty string ,or  empty list
             return None
         else:
             return (Metadoc.convert(it) for it in internal)
@@ -524,18 +527,18 @@
     def convert_to_etree(metadoc):
         return Metadoc.convert_back(metadoc)
 
     @staticmethod
     def from_tagxml(xmldoc: str) -> "Metadoc":
         """
         Create metadoc from "tag" XML string.
-        
+
         Args:
             xmldoc: "tag" XML string
-            
+
         Returns:
             created metadoc
         """
         try:
             xmldoc = _fromstring_fix_empty(xmldoc)
         except etree.ParseError as e:
             raise InvalidFormat(e)
@@ -544,31 +547,31 @@
     @staticmethod
     def from_tagxml_etree(xmldoc):
         return Metadoc(et=tagxml_to_internal(xmldoc))
 
     def to_tagxml(self) -> str:
         """
         Convert this metadoc to "tag" XML string.
-        
+
         Returns:
             "tag" XML string
         """
         return _tostring_fix_empty(self.to_tagxml_etree(), encoding="unicode")
 
     def to_tagxml_etree(self):
         return internal_to_tagxml(self.node)
 
     @staticmethod
     def from_naturalxml(xmldoc: str) -> "Metadoc":
         """
         Create metadoc from "natural" XML string.
-        
+
         Args:
             xmldoc: "natural" XML string
-            
+
         Returns:
             created metadoc
         """
         try:
             xmldoc = _fromstring_fix_empty(xmldoc)
         except etree.ParseError as e:
             raise InvalidFormat(e)
@@ -577,61 +580,61 @@
     @staticmethod
     def from_naturalxml_etree(xmldoc):
         return Metadoc(et=naturalxml_to_internal(xmldoc))
 
     def to_naturalxml(self) -> str:
         """
         Convert this metadoc to "natural" XML string.
-        
+
         Returns:
             "natural" XML string
         """
         return _tostring_fix_empty(self.to_naturalxml_etree(), encoding="unicode")
 
     def to_naturalxml_etree(self):
         return internal_to_naturalxml(self.node)
 
     @staticmethod
     def from_json(jsondoc) -> "Metadoc":
         """
         Create metadoc from JSON-like Python structure.
-        
+
         Args:
             jsondoc: JSON-like Python structure
-            
+
         Returns:
             created metadoc
         """
         return Metadoc(et=naturaljson_to_internal(jsondoc))
 
     def to_json(self) -> dict:
         """
         Convert this metadoc to JSON-like Python structure
-        
+
         Returns:
             JSON-like Python structure of dicts and lists
         """
         return internal_to_naturaljson(self.node)
 
     def as_xml(self) -> str:
         """
         Get tags in metadoc as "natural" XML string.
         This is NOT round-tripable through from_naturalxml!
-        
+
         Returns:
             "natural" XML string
         """
         res = internal_to_naturalxml(_clean_tree(self.node))
         return _tostring_fix_empty(res, encoding="unicode")
-    
+
     def as_dict(self) -> dict:
         """
         Get all tags in metadoc as a dictionary.
         This is NOT round-tripable through from_json!
-        
+
         Returns:
             dict
         """
         res = internal_to_naturaljson(_clean_tree(self.node))
         if len(res.keys()) == 1:
             res = res[list(res.keys())[0]]
         return res
@@ -783,15 +786,15 @@
 
     def _path_to_xpath(self, path):
         path = path.strip()
         if re.match(
             r"""^[\w"']""", path
         ):  # TODO: right now every tag has to start with '/' otherwise the regex below won't work
             path = "./" + path
-            
+
         # split into quoted and non-quoted parts
         QUOTED_STRING = re.compile("(\\\\?[\"']).*?\\1")  # a pattern to match strings between quotes
         result = []  # a store for the result pieces
         head = 0  # a search head reference
         for match in QUOTED_STRING.finditer(path):
             # process everything until the current quoted match and add it to the result
             unquoted_part = path[head:match.start()]
@@ -803,15 +806,15 @@
             result.append(self._path_to_xpath_single(unquoted_part))
             result.append(quoted_part)  # add the quoted match verbatim to the result
             head = match.end()  # move the search head to the end of the quoted match
         if head < len(path):  # if the search head is not at the end of the string
             # process the rest of the string and add it to the result
             result.append(self._path_to_xpath_single(path[head:]))
         return "".join(result)  # join back the result pieces and return them
-            
+
     def _path_to_xpath_single(self, path):
         res = ""
         path_pos = 0
         p = re.compile(
             r"""@[\w -]+|/[^"'/.*@[\]]+|/"[^"]+"|/'[^']+'"""
         )  # allow to escape tag names with " or '
         for m in p.finditer(path):
@@ -834,19 +837,19 @@
             path_pos = end
         res += path[path_pos:]
         return res
 
     def path_query(self, path: str) -> list["Metadoc"]:
         """
         Select nodes in this metadoc based on a path selector.
-        
+
         Args:
             path: path query (e.g., ``'//my tag/another tag with spaces[@attr = "...."]'``)
         """
-        
+
         # generic path query (Xpath/JSONpath compatible)
         # e.g.: '//my tag/another tag with spaces[@attr = "...."]'
         # becomes '//tag[@name="my tag"]/tag[@name="another tag with spaces"][@attr = "...."]' for Xpath
         # becomes '$..['my tag']['another tag with spaces'][?(@.attr = "....")]' for JSONpath
         xpath = self._path_to_xpath(path)
         log.debug(f"path_query {path} -> {xpath}")
         return Metadoc.convert(self.node.xpath(xpath))
```

## bq/metadoc/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.6.3.33'
-__version_tuple__ = version_tuple = (0, 6, 3, 33)
+__version__ = version = '0.6.3.34'
+__version_tuple__ = version_tuple = (0, 6, 3, 34)
```

## bq/metadoc/xmldict.py

```diff
@@ -1,25 +1,57 @@
 # Create python xml structures compatible with
 # http://search.cpan.org/~grantm/XML-Simple-2.18/lib/XML/Simple.pm
 
 from collections import OrderedDict
 from itertools import groupby
-
+from datetime import datetime
 from lxml import etree
 
 
+def asbool(obj):
+    if isinstance(obj, str):
+        obj = obj.strip().lower()
+        if obj in ["true", "yes", "on", "y", "t", "1"]:
+            return True
+        elif obj in ["false", "no", "off", "n", "f", "0"]:
+            return False
+        else:
+            raise ValueError("String is not true/false: %r" % obj)
+    return bool(obj)
+
+
 def xml2d(e, attribute_prefix=None, group_lists=False, keep_tags=False):
     """Convert an etree into a dict structure"""
 
     def _get_tag(el):
         if el.tag == "tag" and not keep_tags:
             return el.get("name", "tag")
         else:
             return el.tag
 
+    def _cast_str_to_native(val: str, d: dict) -> object:
+        attr_type = d.get(f"{attribute_prefix}type")
+        res = None
+        if attr_type == "number":
+            if "." in val:
+                res = float(val)
+            else:
+                res = int(val)
+        elif attr_type == "datetime":
+            res = datetime.strptime(val, "%Y-%m-%dT%H:%M:%S.%f%z")
+        elif attr_type == "boolean":
+            res = asbool(val)
+        elif attr_type == "string":
+            res = val
+        if res is not None:
+            del d[f"{attribute_prefix}type"]  # remove type attribute since we cast it
+            return res
+        else:
+            return val
+
     def _xml2d(e):
         # map attributes
         if attribute_prefix is not None:
             kids = {
                 f"{attribute_prefix}{k}": v
                 for k, v in e.attrib.items()
                 if e.tag != "tag" or k != "name" or keep_tags
@@ -33,14 +65,15 @@
         # map text
         if kids.get("%svalue" % attribute_prefix) is not None:
             node_val = kids["%svalue" % attribute_prefix]
             del kids["%svalue" % attribute_prefix]
         else:
             node_val = e.text
         if node_val is not None:
+            node_val = _cast_str_to_native(node_val, kids)   # use correct native type
             if len(e) == 0 and len(kids) == 0:
                 kids = node_val
                 return kids
             else:
                 kids["%svalue" % attribute_prefix] = node_val
         # map children
         for k, g in groupby(
@@ -56,22 +89,36 @@
 
 
 def d2xml(d: dict, attribute_prefix=None, keep_value_attr: bool = False):
     """convert dict to etree"""
     if not isinstance(d, dict):
         raise ValueError(f" Expected dict, got {type(d)}")
 
+    def _cast_native_to_str(val: object) -> (str, str):
+        if isinstance(val, bool):
+            return (str(val), "boolean")
+        elif isinstance(val, (int, float)):
+            return (str(val), "number")
+        elif isinstance(val, datetime):
+            if val.tzinfo is None or val.tzinfo.utcoffset(val) is None:
+                # no timezone => assume UTC
+                val = val.replace(tzinfo=timezone.utc)
+            return (val.strftime("%Y-%m-%dT%H:%M:%S.%f%z"), "datetime")
+        return (str(val), None)
+
     def _setval(node, val):
-        val = str(val)  # TODO: need to come up with better solution for numbers etc
+        val, type_attr = _cast_native_to_str(val)
         if (
             keep_value_attr or val.strip() != val
         ):  # keep vals with leading/trailing spaces in value attr for subsequent naturalxml_to_tree
             node.set("value", val)
         else:
             node.text = val
+        if type_attr:
+            node.set("type", type_attr)
 
     def _d2xml(d, p):
         for k, v in d.items():
             if isinstance(v, dict):
                 try:
                     node = etree.SubElement(p, k)
                 except ValueError:
```

## Comparing `bisque_metadoc-0.6.3.33.dist-info/METADATA` & `bisque_metadoc-0.6.3.34.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisque_metadoc
-Version: 0.6.3.33
+Version: 0.6.3.34
 Summary: Bisque Metadoc
 Author-email: ViQi Inc <info@viqi.org>
 Project-URL: homepage, https://gitlab.com/viqi/viqi-common/bisque_metadoc
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```


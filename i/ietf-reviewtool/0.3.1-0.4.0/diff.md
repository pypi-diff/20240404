# Comparing `tmp/ietf_reviewtool-0.3.1.tar.gz` & `tmp/ietf_reviewtool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietf_reviewtool-0.3.1.tar", max compression
+gzip compressed data, was "ietf_reviewtool-0.4.0.tar", max compression
```

## Comparing `ietf_reviewtool-0.3.1.tar` & `ietf_reviewtool-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    18092 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/LICENSE
--rw-r--r--   0        0        0     6700 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/README.md
--rw-r--r--   0        0        0      285 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/__init__.py
--rw-r--r--   0        0        0      146 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/__main__.py
--rw-r--r--   0        0        0     1183 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/agenda.py
--rw-r--r--   0        0        0    14217 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/boilerplate.py
--rw-r--r--   0        0        0     5144 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/doc.py
--rw-r--r--   0        0        0     4181 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/grammar.py
--rwxr-xr-x   0        0        0    30018 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/ietf_reviewtool.py
--rw-r--r--   0        0        0     2527 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/inclusive.py
--rw-r--r--   0        0        0     4829 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/metadata.py
--rw-r--r--   0        0        0    10926 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/references.py
--rw-r--r--   0        0        0    10872 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/review.py
--rw-r--r--   0        0        0        0 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/__init__.py
--rw-r--r--   0        0        0     2970 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/docposition.py
--rw-r--r--   0        0        0    11456 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/fetch.py
--rw-r--r--   0        0        0     2936 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/format.py
--rw-r--r--   0        0        0    10386 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/text.py
--rw-r--r--   0        0        0     2033 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/utils.py
--rw-r--r--   0        0        0     1376 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 ietf_reviewtool-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-04 14:25:57.261864 ietf_reviewtool-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6700 2024-04-04 14:25:57.261864 ietf_reviewtool-0.4.0/README.md
+-rw-r--r--   0        0        0      285 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/__main__.py
+-rw-r--r--   0        0        0     1183 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/agenda.py
+-rw-r--r--   0        0        0    14293 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/boilerplate.py
+-rw-r--r--   0        0        0     5478 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/doc.py
+-rw-r--r--   0        0        0     4313 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/grammar.py
+-rwxr-xr-x   0        0        0    30210 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/ietf_reviewtool.py
+-rw-r--r--   0        0        0     2527 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/inclusive.py
+-rw-r--r--   0        0        0     4829 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/metadata.py
+-rw-r--r--   0        0        0    10968 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/references.py
+-rw-r--r--   0        0        0    10872 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/review.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/docposition.py
+-rw-r--r--   0        0        0    11251 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/fetch.py
+-rw-r--r--   0        0        0     2936 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/format.py
+-rw-r--r--   0        0        0    11478 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/text.py
+-rw-r--r--   0        0        0     2319 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/utils.py
+-rw-r--r--   0        0        0     1400 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7794 1970-01-01 00:00:00.000000 ietf_reviewtool-0.4.0/PKG-INFO
```

### Comparing `ietf_reviewtool-0.3.1/LICENSE` & `ietf_reviewtool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/README.md` & `ietf_reviewtool-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/agenda.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/agenda.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/boilerplate.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/boilerplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,18 @@
 
     @param      doc     The document
     @param      review  The IETF Review document to add comments to
 
     @return     { description_of_the_return_value }
     """
     text = unfold(doc.orig)
-    if re.search(
-        r"""This\s+document\s+may\s+not\s+be\s+modified,?\s+and\s+derivative\s+
-            works\s+of\s+it\s+may\s+not\s+be\s+created""",
-        text,
-        re.VERBOSE,
-    ):
+    if re.search(TLP_6CI_PATTERN, text):
         msg = (
             "Document has an IETF Trust Provisions (TLP) Section 6.c(i) "
-            "Publication Limitation clause. This means it can in most cases"
+            "Publication Limitation clause. This means it can in most cases "
             "not be a WG document."
         )
         if doc.status.lower() == "standards track":
             msg += " And it cannot be published on the Standards Track."
         review.discuss("Boilerplate", msg)
 
     if re.search(r"Simplified\s+BSD\s+License", text, flags=re.IGNORECASE):
@@ -187,15 +182,15 @@
         sotm = re.sub(PRE_5378, r"", sotm)
         review.comment(
             "Boilerplate",
             'Document has a TLP Section 6.c.iii "pre-5378" boilerplate. '
             "Is this really needed?",
         )
 
-    if sotm:
+    if sotm and not re.match(TLP_6CI_PATTERN, sotm.strip()):
         review.nit(
             "Boilerplate",
             f'Found stray text in boilerplate: "{sotm.strip()}"',
         )
 
 
 # pattern matching RFC2119 keywords
@@ -243,14 +238,20 @@
 
 TLP_6A_PATTERN = re.compile(
     r"""\s*This\s+Internet-Draft\s+is\s+submitted\s+in\s+full\s+conformance\s+
         with\s+the\s+provisions\s+of\s+BCP\s*78\s+and\s+BCP\s*79\.\s+""",
     re.VERBOSE,
 )
 
+TLP_6CI_PATTERN = re.compile(
+    r"""This\s+document\s+may\s+not\s+be\s+modified,?\s+and\s+derivative\s+
+            works\s+of\s+it\s+may\s+not\s+be\s+created""",
+    re.VERBOSE,
+)
+
 ID_GUIDELINES_PATTERNS = [
     (
         True,
         re.compile(
             # this has an option for the pre-2010 text in it
             r"""Internet-Drafts\s+are\s+working\s+documents\s+of\s+the\s+
             Internet\s+Engineering\s+Task\s+Force\s+\(IETF\)
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/doc.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,23 @@
                 os.chdir(tmp)
                 orig_item = os.path.basename(item)
                 get_items([orig_item], log, datatracker)
                 self.orig = read(orig_item, log)
                 os.chdir(current_directory)
             self.current = read(item, log)
             if not self.orig:
-                log.error(
-                    "No original for %s, cannot review, only performing checks",
-                    item,
-                )
-                self.orig = self.current
+                # check if there is a ".orig" file to diff against
+                orig_item += ".orig"
+                self.orig = read(orig_item, log)
+                if not self.orig:
+                    log.error(
+                        "No original for %s, cannot review, only performing checks",
+                        item,
+                    )
+                    self.orig = self.current
 
         self.orig_lines = self.orig.splitlines(keepends=True)
         self.current_lines = self.current.splitlines(keepends=True)
 
         # difflib can't deal with single lines it seems
         if len(self.orig_lines) == 1:
             self.orig_lines.append("\n")
@@ -130,15 +134,18 @@
                     for match in re.finditer(
                         r"\b(draft-[-a-z\d_.]+|(?:RFC|rfc)\s*\d+)\b",
                         ref_text,
                         re.DOTALL,
                     ):
                         if match:
                             target = re.sub(r"\s+", "", match.group(0).lower())
+                            target = os.path.splitext(target)[0]
                             targets.add(target)
 
-                    if targets:
-                        self.references[part].append((ref, targets))
-                    else:
+                    if not targets:
                         urls = extract_urls(ref_text, log, True, True)
-                        self.references[part].append((ref, urls))
-        self.references["text"] = refs["text"]
+                        targets = set().union(*[urls[key] for key in urls])
+
+                    self.references[part].append((ref, targets))
+        self.references["text"] = set(
+            x.upper() if x.startswith("[rfc") else x for x in refs["text"]
+        )
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/grammar.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/grammar.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,49 +39,53 @@
         for i in lt.check(unfold("".join(text)))
         if i.ruleId
         not in [
             "ADVERTISEMENT_OF_FOR",
             "ALL_OF_THE",
             "ARROWS",
             "BOTH_AS_WELL_AS",
-            "COMMA_COMPOUND_SENTENCE_2",
             "COMMA_COMPOUND_SENTENCE",
+            "COMMA_COMPOUND_SENTENCE_2",
             "COMMA_PARENTHESIS_WHITESPACE",
             "COPYRIGHT",
             "CURRENCY",
             "DASH_RULE",
             "DATE_FUTURE_VERB_PAST",
             "DATE_NEW_YEAR",
+            "DIFFERENT_THAN",
             "DOUBLE_PUNCTUATION",
+            "EN_COMPOUNDS",
             "EN_QUOTES",
             "EN_UNPAIRED_BRACKETS",
             "ENGLISH_WORD_REPEAT_BEGINNING_RULE",
             "HYPOTHESIS_TYPOGRAPHY",
             "I_LOWERCASE",
             "IN_THE_INTERNET",
             "INCORRECT_POSSESSIVE_FORM_AFTER_A_NUMBER",
             "KEY_WORDS",
             "LARGE_NUMBER_OF",
             "MORFOLOGIK_RULE_EN_US",
             "MULTIPLICATION_SIGN",
             "NUMBERS_IN_WORDS",
             "OUTSIDE_OF",
             "PLUS_MINUS",
+            "POSSESSIVE_APOSTROPHE",
             "PUNCTUATION_PARAGRAPH_END",
             "R_SYMBOL",
             "RETURN_IN_THE",
             "SENTENCE_WHITESPACE",
             "SO_AS_TO",
             "SOME_OF_THE",
             "TRADEMARK",
             "UNIT_SPACE",
             "UNLIKELY_OPENING_PUNCTUATION",
             "UPPERCASE_SENTENCE_START",
             "WHETHER",
             "WHITESPACE_RULE",
+            "WITH_THE_EXCEPTION_OF",
             "WORD_CONTAINS_UNDERSCORE",
         ]
         and (not grammar_skip_rules or i.ruleId not in grammar_skip_rules.split(","))
     ]
     issues = [i for i in issues if not i.ruleId.startswith("EN_REPEATEDWORDS_")]
 
     doc_pos = DocPosition()
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/ietf_reviewtool.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/ietf_reviewtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,28 @@
     extract_ips,
     extract_urls,
     strip_pagination,
     unfold,
     undo_rfc8792,
     doc_parts,
 )
-from .util.utils import read, write
+from .util.utils import (
+    read,
+    write,
+    TEST_NET_1,
+    TEST_NET_2,
+    TEST_NET_3,
+    MCAST_TEST_NET,
+    TEST_NET_V6,
+)
 
 
 log = logging.getLogger(__name__)
 
 
-TEST_NET_1 = ipaddress.IPv4Network("192.0.2.0/24")
-TEST_NET_2 = ipaddress.IPv4Network("198.51.100.0/24")
-TEST_NET_3 = ipaddress.IPv4Network("203.0.113.0/24")
-MCAST_TEST_NET = ipaddress.IPv4Network("233.252.0.0/24")
-TEST_NET_V6 = ipaddress.IPv6Network("2001:db8::/32")
-
-
 class State:
     """
     This class describes the global state.
     """
 
     def __init__(self, datatracker=None, verbose=0, default=True, width=79):
         self.datatracker = datatracker
@@ -322,39 +323,43 @@
             log.debug("Review for %s was not completed", doc.name)
             continue
 
         if assignment["state"].endswith("withdrawn/"):
             log.debug("Review for %s was withdrawn", doc.name)
             continue
 
+        if not assignment["review"]:
+            log.warning("Could not fetch review for %s", doc.name)
+            continue
+
         art_review = fetch_dt(datatracker, assignment["review"], log)
 
         if not art_review:
             log.warning("Could not fetch review for %s", doc.name)
             continue
 
         group = fetch_dt(datatracker, art_review["group"], log)
 
         if not group:
             log.warning("Could not fetch ART for %s", doc.name)
             continue
 
-        if art_review["id"] in thanked:
+        if reviewer["id"] in thanked:
             log.warning(
                 "Already recorded %s for %s review", reviewer["name"], group["name"]
             )
             continue
 
         if group["acronym"].lower() == thank_art.lower():
             # remember we thanked for this
-            thanked.add(art_review["id"])
+            thanked.add(reviewer["id"])
 
             review.preface(
                 "",
-                f'Thanks to {reviewer["name_from_draft"] or reviewer["name"]} '
+                f'Thanks to {reviewer["name"] or reviewer["name_from_draft"]} '
                 + f'for the {group["name"]} review ({art_review["external_url"]}).',
             )
 
 
 def check_ips(doc: Doc, review: IetfReview, verbose: bool) -> None:
     """
     Check the IP addresses and blocks in the document.
@@ -601,15 +606,20 @@
     """
     snippets = re.finditer(r"^(\s*){\s*$", doc.orig, flags=re.MULTILINE)
     for snip in snippets:
         # parse JSON snippet until closing brace
         try:
             tokens = list(json5.tokenizer.tokenize(doc.orig[snip.start() :]))
         except json5.utils.JSON5DecodeError as err:
-            review.nit("JSON", str(err) + "\n", wrap=False)
+            msg = f"{str(err)}\n"
+            index_match = re.search(r"index (\d+)", msg)
+            if index_match:
+                index = int(index_match.groups()[0]) + 1
+                msg += f"```{doc.orig[snip.start() : snip.start() + index]}\n```\n"
+            review.nit("JSON", msg, wrap=False)
             return
         stack = []
         collected = []
         for token in tokens:
             collected.append(token.value)
             if token.type in ["WHITESPACE"]:
                 continue
@@ -628,16 +638,16 @@
         except json.decoder.JSONDecodeError as err:
             nit = ""
             quote = "> "
             if review.mkd:
                 nit += "```\n"
                 quote = ""
 
-            for i, line in enumerate(text.splitlines(keepends=True)):
-                nit += f"{quote}{line}"
+            for i, l in enumerate(text.splitlines(keepends=True)):
+                nit += f"{quote}{l}"
                 if i == err.lineno - 2:
                     nit += f"{quote}{' ' * (err.colno - 1)}^ {err.msg}\n"
 
             if review.mkd:
                 nit += "```\n"
 
             review.nit("JSON", nit, wrap=False)
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/inclusive.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/inclusive.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/metadata.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/metadata.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/references.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/references.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     quote = "`" if review.mkd else ""
 
     # check for duplicates
     for kind in ["normative", "informative"]:
         if not doc.references[kind]:
             continue
 
-        tags, tgts = zip(*doc.references[kind])
-        tgts = list(itertools.chain(*tgts))
+        tags = [x[0] for x in doc.references[kind]]
+        tgts = [next(iter(x[1])) if x[1] else None for x in doc.references[kind]]
         dupes = duplicates(tags)
         if dupes:
             review.nit(
                 "Duplicate references",
                 f"Duplicate {kind} references: "
                 f"{word_join(list(dupes), prefix=quote, suffix=quote)}.",
             )
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/review.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/review.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/util/docposition.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/util/docposition.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/util/fetch.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/util/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,21 +295,17 @@
                 datatracker,
                 f"doc/relateddocument/?relationship__slug={slug}&target__name={doc}",
                 log,
             )
             if not target:
                 log.warning("cannot find target for %s", doc)
                 continue
-            docalias = fetch_dt(datatracker, target[0]["target"], log)
-            if not docalias:
-                log.warning("cannot find docalias for %s", target[0]["target"])
-                continue
-            alias = fetch_dt(datatracker, docalias["document"], log)
+            alias = fetch_dt(datatracker, target[0]["target"], log)
             if not alias:
-                log.warning("cannot find doc for %s", docalias["document"])
+                log.warning("cannot find alias for %s", target[0]["target"])
                 continue
             items.append(f"{alias['name']}-{alias['rev']}.txt")
             do_strip = False
         # else:
         #     die(f"Unknown item type: {item}", log)
 
         if cache:
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/util/format.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/util/format.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/util/text.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/util/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 """ietf-reviewtool text module"""
 
+import ipaddress
 import logging
 import re
 import urllib.parse
 import os
 
 import textwrap
 import urlextract  # type: ignore
 
 from .docposition import SECTION_PATTERN
+from .utils import TEST_NET_1, TEST_NET_2, TEST_NET_3, MCAST_TEST_NET, TEST_NET_V6
 
-extractor = urlextract.URLExtract()
+extractor = urlextract.URLExtract(extract_localhost=False, limit=9999999)
 extractor.update_when_older(7)  # update TLDs when older than 7 days
+extractor.add_enclosure("<", ">")
+extractor.set_stop_chars_right(
+    extractor.get_stop_chars_right()
+    | {
+        '"',
+        "]",
+        ">",
+        ";",
+        # ",",
+        "'",
+        ")",
+    }
+)
 
 
 def normalize_ws(string: str) -> str:
     """
     Replace multiple white space characters by a single space.
 
     @param      string  The string to replace in
@@ -130,59 +145,71 @@
         if part not in urls:
             urls[part] = set()
 
         # find all URLs in part
         part_text = unfold(part_text)
         try:
             extracted_urls = extractor.find_urls(
-                text=part_text, with_schema_only=True, only_unique=True
+                text=part_text, with_schema_only=False, only_unique=True
             )
         except UnicodeDecodeError as err:
             log.warning("Could not extract URLs: %s", err)
             return {}
-
         for url in extracted_urls:
             url = url.rstrip(".\"]'>;,)")
+            # urllib doesn't seem to support schemes that don't end in //, work around:
+            fixed_url = re.sub(r"^(\w+:)([^/]{2}.*)", r"\1//\2", url, re.IGNORECASE)
             try:
-                urllib.parse.urlparse(url).netloc
+                netloc = urllib.parse.urlparse(fixed_url).netloc
+                if not netloc:
+                    netloc = url
             except ValueError as err:
                 log.warning("%s: %s", err, url)
                 continue
 
-            urls[part].add(url)
-
-        if not examples:
-            # remove example URLs
-            urls[part] = {
-                u
-                for u in urls[part]
-                if not re.search(
-                    r"example\.(com|net|org)|\.example",
-                    urllib.parse.urlparse(u).netloc
-                    if urllib.parse.urlparse(u).netloc
-                    else u,
+            if not examples:
+                # remove example URLs
+                if re.search(
+                    r"example\.(com|net|org)$|\.(test|example|invalid|localhost)$",
+                    netloc,
                     re.IGNORECASE,
-                )
-            }
+                ):
+                    continue
+
+                # remove URLs w/example IP addresses
+                try:
+                    addr = ipaddress.ip_address(netloc)
+                    if (
+                        isinstance(addr, ipaddress.IPv4Address)
+                        and (
+                            addr in TEST_NET_1
+                            or addr in TEST_NET_2
+                            or addr in TEST_NET_3
+                            or addr in MCAST_TEST_NET
+                        )
+                    ) or (
+                        isinstance(addr, ipaddress.IPv6Address) and addr in TEST_NET_V6
+                    ):
+                        continue
+                except ValueError:
+                    pass
 
-        if not common:
             # remove some common URLs
-            urls[part] = {
-                u
-                for u in urls[part]
-                if not re.search(
-                    r"""https?://
-                        datatracker\.ietf\.org/drafts/current/|
-                        trustee\.ietf\.org/license-info|
-                        (www\.)?rfc-editor\.org/info/rfc\d+|
-                        (www\.)?ietf\.org/archive/id/draft-""",
-                    u,
-                    flags=re.VERBOSE | re.IGNORECASE,
-                )
-            }
+            if not common and re.search(
+                r"""https?://
+                            datatracker\.ietf\.org/drafts/current/|
+                            trustee\.ietf\.org/license-info|
+                            (www\.)?rfc-editor\.org/(info|rfc)/rfc\d+|
+                            (www\.)?ietf\.org/archive/id/draft-""",
+                url,
+                flags=re.VERBOSE | re.IGNORECASE,
+            ):
+                continue
+
+            urls[part].add(url)
 
     return urls
 
 
 def strip_pagination(text: str) -> str:
     """
     Strip headers and footers, end-of-line whitespace and CR/LF, similar to the rfcstrip
```

### Comparing `ietf_reviewtool-0.3.1/ietf_reviewtool/util/utils.py` & `ietf_reviewtool-0.4.0/ietf_reviewtool/util/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """ietf-reviewtool utils module"""
 
 import datetime
+import ipaddress
 import logging
 import sys
 
 import charset_normalizer
 
+TEST_NET_1 = ipaddress.IPv4Network("192.0.2.0/24")
+TEST_NET_2 = ipaddress.IPv4Network("198.51.100.0/24")
+TEST_NET_3 = ipaddress.IPv4Network("203.0.113.0/24")
+MCAST_TEST_NET = ipaddress.IPv4Network("233.252.0.0/24")
+TEST_NET_V6 = ipaddress.IPv6Network("2001:db8::/32")
+
 
 def die(msg: str, log: logging.Logger, err: int = 1) -> None:
     """
     Print a message and exit with an error code.
 
     @param      msg   The message to print
     @param      log   The log
```

### Comparing `ietf_reviewtool-0.3.1/pyproject.toml` & `ietf_reviewtool-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ietf-reviewtool"
-version = "0.3.1"
+version = "0.4.0"
 description = "Review tool for IETF documents"
 authors = ["Lars Eggert <lars@eggert.org>"]
 readme = "README.md"
 homepage = "https://github.com/larseggert/ietf-reviewtool"
 repository = "https://github.com/larseggert/ietf-reviewtool"
 license = "GPL-2.0-only"
 
@@ -17,28 +17,30 @@
 PyYAML = ">=5.4.1"
 charset-normalizer = ">=2.0.6"
 urlextract = ">=1.5.0"
 num2words = ">=0.5.10"
 json-five = ">=0.8.0"
 urllib3 = ">=1.26.15"
 requests = ">=2.28.2"
+setuptools = "^69.0.2"
 
 [tool.poetry.dev-dependencies]
 mypy = ">=0.942"
 
 [tool.poetry.scripts]
 irt = "ietf_reviewtool.ietf_reviewtool:cli"
 ietf-reviewtool = "ietf_reviewtool.ietf_reviewtool:cli"
 
 [tool.poetry.group.types.dependencies]
 types-requests = "^2.31.0.0"
 types-appdirs = "^1.4.3.5"
 types-urllib3 = "^1.26.25.13"
 types-click = "^7.1.8"
 types-pyyaml = "^6.0.12.10"
+
 [tool.pylint.messages_control]
 # TODO: these are very high and should be gradually reduced during refactoring
 max-args = 15
 max-bool-expr = 10
 max-branches = 80
 max-locals = 50
 max-module-lines = 1500
```

### Comparing `ietf_reviewtool-0.3.1/PKG-INFO` & `ietf_reviewtool-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: ietf-reviewtool
-Version: 0.3.1
+Version: 0.4.0
 Summary: Review tool for IETF documents
 Home-page: https://github.com/larseggert/ietf-reviewtool
 License: GPL-2.0-only
 Author: Lars Eggert
 Author-email: lars@eggert.org
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: charset-normalizer (>=2.0.6)
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: json-five (>=0.8.0)
 Requires-Dist: language-tool-python (>=2.5.3)
 Requires-Dist: num2words (>=0.5.10)
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: requests-cache (>=1.0.0)
+Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Requires-Dist: urlextract (>=1.5.0)
 Requires-Dist: urllib3 (>=1.26.15)
 Project-URL: Repository, https://github.com/larseggert/ietf-reviewtool
 Description-Content-Type: text/markdown
 
 # ietf-reviewtool
```


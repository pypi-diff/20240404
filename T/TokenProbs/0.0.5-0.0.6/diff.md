# Comparing `tmp/TokenProbs-0.0.5.tar.gz` & `tmp/TokenProbs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokenProbs-0.0.5.tar", last modified: Tue Apr  2 20:13:01 2024, max compression
+gzip compressed data, was "TokenProbs-0.0.6.tar", last modified: Thu Apr  4 00:40:31 2024, max compression
```

## Comparing `TokenProbs-0.0.5.tar` & `TokenProbs-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 20:13:01.785016 TokenProbs-0.0.5/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.5/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-02 20:13:01.784603 TokenProbs-0.0.5/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.5/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-02 20:13:01.785081 TokenProbs-0.0.5/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-02 20:12:48.000000 TokenProbs-0.0.5/setup.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 20:13:01.781590 TokenProbs-0.0.5/src/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 20:13:01.782813 TokenProbs-0.0.5/src/TokenProbs/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-02 19:34:12.000000 TokenProbs-0.0.5/src/TokenProbs/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     8665 2024-04-02 20:08:38.000000 TokenProbs-0.0.5/src/TokenProbs/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 20:13:01.784158 TokenProbs-0.0.5/src/TokenProbs.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-02 20:13:01.783250 TokenProbs-0.0.5/src/TokenProbs.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-02 20:13:01.783524 TokenProbs-0.0.5/src/TokenProbs.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-02 20:13:01.783755 TokenProbs-0.0.5/src/TokenProbs.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-02 20:13:01.783982 TokenProbs-0.0.5/src/TokenProbs.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-02 20:13:01.784211 TokenProbs-0.0.5/src/TokenProbs.egg-info/top_level.txt
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.352748 TokenProbs-0.0.6/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.6/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:40:31.352156 TokenProbs-0.0.6/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.6/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-04 00:40:31.352810 TokenProbs-0.0.6/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-04 00:40:17.000000 TokenProbs-0.0.6/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.347717 TokenProbs-0.0.6/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.349579 TokenProbs-0.0.6/src/TokenProbs/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       73 2024-04-04 00:39:58.000000 TokenProbs-0.0.6/src/TokenProbs/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     8847 2024-04-02 22:14:09.000000 TokenProbs-0.0.6/src/TokenProbs/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.351701 TokenProbs-0.0.6/src/TokenProbs.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/top_level.txt
```

### Comparing `TokenProbs-0.0.5/PKG-INFO` & `TokenProbs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `TokenProbs-0.0.5/README.md` & `TokenProbs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TokenProbs-0.0.5/setup.py` & `TokenProbs-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities or other probability-based queries instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="TokenProbs",
     version=VERSION,
```

### Comparing `TokenProbs-0.0.5/src/TokenProbs/logit_extraction.py` & `TokenProbs-0.0.6/src/TokenProbs/logit_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,28 +134,29 @@
         if torch.cuda.is_available():
             device = 'cuda'
         else:
             device = 'cpu'
 
         preds = []
         self.model.eval()
-        for batch in tqdm(input_data):
-
-            output = self.model(
-                input_ids = batch['input_ids'].to(device),
-                attention_mask = batch['attention_mask'].to(device)
-            ).logits.detach().cpu()
-
-            # Extract predictions following end of prompt
-            generated = torch.vstack(
-                [output[i,batch['length'][i]-1,:] for i in range(len(batch['length']))]
-            )
-            preds.append(
-                softmax(generated[:,list(self.token_dict.values())],dim=-1).numpy()
-            )
+        with torch.no_grad():
+            for batch in tqdm(input_data):
+    
+                output = self.model(
+                    input_ids = batch['input_ids'].to(device),
+                    attention_mask = batch['attention_mask'].to(device)
+                ).logits.detach().cpu()
+    
+                # Extract predictions following end of prompt
+                generated = torch.vstack(
+                    [output[i,batch['length'][i]-1,:] for i in range(len(batch['length']))]
+                )
+                preds.append(
+                    softmax(generated[:,list(self.token_dict.values())],dim=-1).numpy()
+                )
 
         output_df = pd.DataFrame(np.vstack(preds),columns=list(self.token_dict.keys()))
 
         return output_df
 
     def text_generation(self,input_data,batch_size=1,max_new_tokens=100):
         if type(input_data) == list:
@@ -170,28 +171,29 @@
         if torch.cuda.is_available():
             device = 'cuda'
         else:
             device = 'cpu'
 
         preds = []
         self.model.eval()
-        for batch in tqdm(input_data):
-            output = self.model.generate(
-                input_ids = batch['input_ids'].to('cuda'),
-                attention_mask = batch['attention_mask'].to('cuda'),
-                max_new_tokens = max_new_tokens
-            )
-
-            preds.extend(
-                self.tokenizer.batch_decode(
-                    [output[i,batch['length'][i]:] for i in range(len(batch['length']))]
+        with torch.no_grad():
+            for batch in tqdm(input_data):
+                output = self.model.generate(
+                    input_ids = batch['input_ids'].to('cuda'),
+                    attention_mask = batch['attention_mask'].to('cuda'),
+                    max_new_tokens = max_new_tokens
+                )
+    
+                preds.extend(
+                    self.tokenizer.batch_decode(
+                        [output[i,batch['length'][i]:] for i in range(len(batch['length']))]
+                    )
                 )
-            )
 
-        preds = [i.replace('</s>','') for i in preds]
+        preds = [i.replace('</s>','').replace('<s>','') for i in preds]
         return preds
 
     def get_response_seq(self,response_seq):
         if type(response_seq) == list:
             return response_seq
         else:
             return self.tokenizer(response_seq)['input_ids'][1:]
```

### Comparing `TokenProbs-0.0.5/src/TokenProbs.egg-info/PKG-INFO` & `TokenProbs-0.0.6/src/TokenProbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


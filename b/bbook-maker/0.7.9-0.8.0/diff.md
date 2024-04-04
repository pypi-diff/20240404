# Comparing `tmp/bbook_maker-0.7.9.tar.gz` & `tmp/bbook_maker-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbook_maker-0.7.9.tar", last modified: Thu Feb 29 03:05:39 2024, max compression
+gzip compressed data, was "bbook_maker-0.8.0.tar", last modified: Thu Apr  4 13:03:26 2024, max compression
```

## Comparing `bbook_maker-0.7.9.tar` & `bbook_maker-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.369717 bbook_maker-0.7.9/
--rw-r--r--   0 hyi        (502) staff       (20)     1063 2023-03-30 08:35:07.000000 bbook_maker-0.7.9/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      825 2024-02-29 03:05:39.368777 bbook_maker-0.7.9/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)    12536 2024-02-29 03:05:11.000000 bbook_maker-0.7.9/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.367933 bbook_maker-0.7.9/bbook_maker.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      825 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1083 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       52 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      111 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       11 2024-02-29 03:05:39.000000 bbook_maker-0.7.9/bbook_maker.egg-info/top_level.txt
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.283011 bbook_maker-0.7.9/book_maker/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-30 08:35:07.000000 bbook_maker-0.7.9/book_maker/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       60 2023-03-30 08:35:07.000000 bbook_maker-0.7.9/book_maker/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)    14604 2024-01-30 13:58:42.000000 bbook_maker-0.7.9/book_maker/cli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.320272 bbook_maker-0.7.9/book_maker/loader/
--rw-r--r--   0 hyi        (502) staff       (20)      296 2023-12-26 08:27:25.000000 bbook_maker-0.7.9/book_maker/loader/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      491 2023-03-30 08:48:21.000000 bbook_maker-0.7.9/book_maker/loader/base_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)    20061 2024-01-27 14:28:19.000000 bbook_maker-0.7.9/book_maker/loader/epub_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3641 2024-02-29 03:05:11.000000 bbook_maker-0.7.9/book_maker/loader/helper.py
--rw-r--r--   0 hyi        (502) staff       (20)    10383 2024-01-27 14:28:19.000000 bbook_maker-0.7.9/book_maker/loader/srt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     4558 2023-07-30 13:14:07.000000 bbook_maker-0.7.9/book_maker/loader/txt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)    30290 2023-03-30 11:26:33.000000 bbook_maker-0.7.9/book_maker/obok.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.364167 bbook_maker-0.7.9/book_maker/translator/
--rw-r--r--   0 hyi        (502) staff       (20)      869 2024-02-29 03:05:11.000000 bbook_maker-0.7.9/book_maker/translator/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      391 2023-04-03 11:56:33.000000 bbook_maker-0.7.9/book_maker/translator/base_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2115 2023-05-28 12:22:19.000000 bbook_maker-0.7.9/book_maker/translator/caiyun_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)    10696 2024-01-30 14:00:34.000000 bbook_maker-0.7.9/book_maker/translator/chatgptapi_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1649 2023-05-21 11:18:16.000000 bbook_maker-0.7.9/book_maker/translator/claude_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)      846 2024-01-05 14:10:29.000000 bbook_maker-0.7.9/book_maker/translator/custom_api_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1525 2023-05-15 00:32:18.000000 bbook_maker-0.7.9/book_maker/translator/deepl_free_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2227 2024-01-31 02:15:04.000000 bbook_maker-0.7.9/book_maker/translator/deepl_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2810 2024-01-27 14:17:37.000000 bbook_maker-0.7.9/book_maker/translator/gemini_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1843 2023-05-24 01:29:57.000000 bbook_maker-0.7.9/book_maker/translator/google_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2472 2023-11-26 14:01:12.000000 bbook_maker-0.7.9/book_maker/translator/litellm_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2839 2024-02-29 03:05:11.000000 bbook_maker-0.7.9/book_maker/translator/tencent_transmart_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     4246 2023-03-30 08:35:07.000000 bbook_maker-0.7.9/book_maker/utils.py
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-02-29 03:05:39.369787 bbook_maker-0.7.9/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1000 2024-02-29 03:05:25.000000 bbook_maker-0.7.9/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-02-29 03:05:39.367143 bbook_maker-0.7.9/tests/
--rw-r--r--   0 hyi        (502) staff       (20)     9507 2023-08-23 02:01:55.000000 bbook_maker-0.7.9/tests/test_integration.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.480922 bbook_maker-0.8.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1063 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      825 2024-04-04 13:03:26.480493 bbook_maker-0.8.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)    13423 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.479889 bbook_maker-0.8.0/bbook_maker.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      825 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1083 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       52 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      111 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       11 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.454918 bbook_maker-0.8.0/book_maker/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       60 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    15333 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/cli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.463526 bbook_maker-0.8.0/book_maker/loader/
+-rw-r--r--   0 hyi        (502) staff       (20)      296 2023-12-26 08:27:25.000000 bbook_maker-0.8.0/book_maker/loader/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      491 2023-03-30 08:48:21.000000 bbook_maker-0.8.0/book_maker/loader/base_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)    20061 2024-01-27 14:28:19.000000 bbook_maker-0.8.0/book_maker/loader/epub_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3641 2024-02-29 03:05:11.000000 bbook_maker-0.8.0/book_maker/loader/helper.py
+-rw-r--r--   0 hyi        (502) staff       (20)    10383 2024-01-27 14:28:19.000000 bbook_maker-0.8.0/book_maker/loader/srt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4558 2023-07-30 13:14:07.000000 bbook_maker-0.8.0/book_maker/loader/txt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)    30290 2023-03-30 11:26:33.000000 bbook_maker-0.8.0/book_maker/obok.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.478262 bbook_maker-0.8.0/book_maker/translator/
+-rw-r--r--   0 hyi        (502) staff       (20)      895 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/translator/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      391 2023-04-03 11:56:33.000000 bbook_maker-0.8.0/book_maker/translator/base_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2115 2023-05-28 12:22:19.000000 bbook_maker-0.8.0/book_maker/translator/caiyun_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)    10874 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/translator/chatgptapi_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1649 2023-05-21 11:18:16.000000 bbook_maker-0.8.0/book_maker/translator/claude_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)      846 2024-01-05 14:10:29.000000 bbook_maker-0.8.0/book_maker/translator/custom_api_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1525 2023-05-15 00:32:18.000000 bbook_maker-0.8.0/book_maker/translator/deepl_free_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2227 2024-01-31 02:15:04.000000 bbook_maker-0.8.0/book_maker/translator/deepl_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2810 2024-01-27 14:17:37.000000 bbook_maker-0.8.0/book_maker/translator/gemini_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1843 2023-05-24 01:29:57.000000 bbook_maker-0.8.0/book_maker/translator/google_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2472 2023-11-26 14:01:12.000000 bbook_maker-0.8.0/book_maker/translator/litellm_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2839 2024-02-29 03:05:11.000000 bbook_maker-0.8.0/book_maker/translator/tencent_transmart_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4246 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-04 13:03:26.480992 bbook_maker-0.8.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1000 2024-04-04 13:03:18.000000 bbook_maker-0.8.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.478969 bbook_maker-0.8.0/tests/
+-rw-r--r--   0 hyi        (502) staff       (20)     9507 2023-08-23 02:01:55.000000 bbook_maker-0.8.0/tests/test_integration.py
```

### Comparing `bbook_maker-0.7.9/LICENSE` & `bbook_maker-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/PKG-INFO` & `bbook_maker-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbook_maker
-Version: 0.7.9
+Version: 0.8.0
 Summary: The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.
 Home-page: https://github.com/yihong0618/bilingual_book_maker
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbook_maker-0.7.9/README.md` & `bbook_maker-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 ## Use
 
 - `pip install -r requirements.txt` or `pip install -U bbook_maker`(you can use)
 - Use `--openai_key` option to specify OpenAI API key. If you have multiple keys, separate them by commas (xxx,xxx,xxx) to reduce errors caused by API call limits.
    Or, just set environment variable `BBM_OPENAI_API_KEY` instead.
 - A sample book, `test_books/animal_farm.epub`, is provided for testing purposes.
 - The default underlying model is [GPT-3.5-turbo](https://openai.com/blog/introducing-chatgpt-and-whisper-apis), which is used by ChatGPT currently. Use `--model gpt4` to change the underlying model to `GPT4`.
-   If using `GPT4`, you can add `--use_context` to add a context paragraph to each passage sent to the model for translation (see below)
-- support DeepL model [DeepL Translator](https://rapidapi.com/splintPRO/api/dpl-translator) need pay to get the token use `--model deepl --deepl_key ${deepl_key}`
+  - Important to note that `gpt-4` is significantly more expensive than `gpt-4-turbo`, but to avoid bumping into rate limits, we automatically balance queries across `gpt-4-1106-preview`, `gpt-4`, `gpt-4-32k`, `gpt-4-0613`,`gpt-4-32k-0613`.
+    - If you want to use a specific model alias with OpenAI (eg `gpt-4-1106-preview` or `gpt-3.5-turbo-0125`), you can use `--model openai --model_list gpt-4-1106-preview,gpt-3.5-turbo-0125`. `--model_list` takes a comma-separated list of model aliases.
+  - If using `GPT4`, you can add `--use_context` to add a context paragraph to each passage sent to the model for translation (see below).- support DeepL model [DeepL Translator](https://rapidapi.com/splintPRO/api/dpl-translator) need pay to get the token use `--model deepl --deepl_key ${deepl_key}`
 - support DeepL free model `--model deeplfree`
 - support Google [Gemini](https://makersuite.google.com/app/apikey) model `--model gemini --gemini_key ${gemini_key}`
 - Support [Claude](https://console.anthropic.com/docs) model, use `--model claude --claude_key ${claude_key}`
 - Support [Tencent TranSmart](https://transmart.qq.com) model (Free), use `--model tencentransmart`
 - Use `--test` option to preview the result if you haven't paid for the service. Note that there is a limit and it may take some time.
 - Set the target language like `--language "Simplified Chinese"`. Default target language is `"Simplified Chinese"`.
    Read available languages by helper message: `python make_book.py --help`
@@ -79,18 +80,23 @@
 
 # Set env OPENAI_API_KEY to ignore option --openai_key
 export OPENAI_API_KEY=${your_api_key}
 
 # Use the GPT-4 model with context to Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model gpt4 --use_context --language ja
 
+# Use a specific OpenAI model alias
+python3 make_book.py --book_name test_books/animal_farm.epub --model openai --model_list gpt-4-1106-preview --openai_key ${openai_key}
+
+# Use a specific list of OpenAI model aliases
+python3 make_book.py --book_name test_books/animal_farm.epub --model openai --model_list gpt-4-1106-preview,gpt-4-0125-preview,gpt-3.5-turbo-0125 --openai_key ${openai_key}
+
 # Use the DeepL model with Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model deepl --deepl_key ${deepl_key} --language ja
 
-
 # Use the Claude model with Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model claude --claude_key ${claude_key} --language ja
 
 # Use the CustomAPI model with Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model customapi --custom_api ${custom_api} --language ja
 
 # Translate contents in <div> and <p>
```

### Comparing `bbook_maker-0.7.9/bbook_maker.egg-info/PKG-INFO` & `bbook_maker-0.8.0/bbook_maker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbook_maker
-Version: 0.7.9
+Version: 0.8.0
 Summary: The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.
 Home-page: https://github.com/yihong0618/bilingual_book_maker
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbook_maker-0.7.9/bbook_maker.egg-info/SOURCES.txt` & `bbook_maker-0.8.0/bbook_maker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/cli.py` & `bbook_maker-0.8.0/book_maker/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -271,14 +271,20 @@
     )
     parser.add_argument(
         "--block_size",
         type=int,
         default=-1,
         help="merge multiple paragraphs into one block, may increase accuracy and speed up the process, but disturb the original format, must be used with `--single_translate`",
     )
+    parser.add_argument(
+        "--model_list",
+        type=str,
+        dest="model_list",
+        help="Rather than using our preset lists of models, specify exactly the models you want as a comma separated list `gpt-4-32k,gpt-3.5-turbo-0125` (Currently only supports: `openai`)",
+    )
 
     options = parser.parse_args()
 
     if not os.path.isfile(options.book_name):
         print(f"Error: {options.book_name} does not exist.")
         exit(1)
 
@@ -286,15 +292,15 @@
     if PROXY != "":
         os.environ["http_proxy"] = PROXY
         os.environ["https_proxy"] = PROXY
 
     translate_model = MODEL_DICT.get(options.model)
     assert translate_model is not None, "unsupported model"
     API_KEY = ""
-    if options.model in ["chatgptapi", "gpt4"]:
+    if options.model in ["openai", "chatgptapi", "gpt4"]:
         if OPENAI_API_KEY := (
             options.openai_key
             or env.get(
                 "OPENAI_API_KEY",
             )  # XXX: for backward compatibility, deprecate soon
             or env.get(
                 "BBM_OPENAI_API_KEY",
@@ -398,14 +404,22 @@
         assert options.model in [
             "chatgptapi",
             "gpt4",
         ], "only support chatgptapi for deployment_id"
         if not options.api_base:
             raise ValueError("`api_base` must be provided when using `deployment_id`")
         e.translate_model.set_deployment_id(options.deployment_id)
+    if options.model == "openai":
+        # Currently only supports `openai` when you also have --model_list set
+        if options.model_list:
+            e.translate_model.set_model_list(options.model_list.split(","))
+        else:
+            raise ValueError(
+                "When using `openai` model, you must also provide `--model_list`. For default model sets use `--model chatgptapi` or `--model gpt4`",
+            )
     # TODO refactor, quick fix for gpt4 model
     if options.model == "chatgptapi":
         e.translate_model.set_gpt35_models()
     if options.model == "gpt4":
         e.translate_model.set_gpt4_models()
     if options.block_size > 0:
         e.block_size = options.block_size
```

### Comparing `bbook_maker-0.7.9/book_maker/loader/epub_loader.py` & `bbook_maker-0.8.0/book_maker/loader/epub_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/loader/helper.py` & `bbook_maker-0.8.0/book_maker/loader/helper.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/loader/srt_loader.py` & `bbook_maker-0.8.0/book_maker/loader/srt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/loader/txt_loader.py` & `bbook_maker-0.8.0/book_maker/loader/txt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/obok.py` & `bbook_maker-0.8.0/book_maker/obok.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/__init__.py` & `bbook_maker-0.8.0/book_maker/translator/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from book_maker.translator.google_translator import Google
 from book_maker.translator.claude_translator import Claude
 from book_maker.translator.gemini_translator import Gemini
 from book_maker.translator.tencent_transmart_translator import TencentTranSmart
 from book_maker.translator.custom_api_translator import CustomAPI
 
 MODEL_DICT = {
+    "openai": ChatGPTAPI,
     "chatgptapi": ChatGPTAPI,
+    "gpt4": ChatGPTAPI,
     "google": Google,
     "caiyun": Caiyun,
     "deepl": DeepL,
     "deeplfree": DeepLFree,
-    "gpt4": ChatGPTAPI,
     "claude": Claude,
     "gemini": Gemini,
     "tencentransmart": TencentTranSmart,
     "customapi": CustomAPI,
     # add more here
 }
```

### Comparing `bbook_maker-0.7.9/book_maker/translator/caiyun_translator.py` & `bbook_maker-0.8.0/book_maker/translator/caiyun_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/chatgptapi_translator.py` & `bbook_maker-0.8.0/book_maker/translator/chatgptapi_translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -326,7 +326,12 @@
         else:
             my_model_list = [
                 i["id"] for i in self.openai_client.models.list().model_dump()["data"]
             ]
             model_list = list(set(my_model_list) & set(GPT4_MODEL_LIST))
             print(f"Using model list {model_list}")
             self.model_list = cycle(model_list)
+
+    def set_model_list(self, model_list):
+        model_list = list(set(model_list))
+        print(f"Using model list {model_list}")
+        self.model_list = cycle(model_list)
```

### Comparing `bbook_maker-0.7.9/book_maker/translator/claude_translator.py` & `bbook_maker-0.8.0/book_maker/translator/claude_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/custom_api_translator.py` & `bbook_maker-0.8.0/book_maker/translator/custom_api_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/deepl_free_translator.py` & `bbook_maker-0.8.0/book_maker/translator/deepl_free_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/deepl_translator.py` & `bbook_maker-0.8.0/book_maker/translator/deepl_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/gemini_translator.py` & `bbook_maker-0.8.0/book_maker/translator/gemini_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/google_translator.py` & `bbook_maker-0.8.0/book_maker/translator/google_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/litellm_translator.py` & `bbook_maker-0.8.0/book_maker/translator/litellm_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/translator/tencent_transmart_translator.py` & `bbook_maker-0.8.0/book_maker/translator/tencent_transmart_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/book_maker/utils.py` & `bbook_maker-0.8.0/book_maker/utils.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.7.9/setup.py` & `bbook_maker-0.8.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "backoff",
 ]
 
 
 setup(
     name="bbook_maker",
     description="The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.",
-    version="0.7.9",
+    version="0.8.0",
     license="MIT",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     packages=find_packages(),
     url="https://github.com/yihong0618/bilingual_book_maker",
     python_requires=">=3.8",
     install_requires=packages,
```

### Comparing `bbook_maker-0.7.9/tests/test_integration.py` & `bbook_maker-0.8.0/tests/test_integration.py`

 * *Files identical despite different names*


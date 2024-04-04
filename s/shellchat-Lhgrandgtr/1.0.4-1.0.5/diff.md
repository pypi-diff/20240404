# Comparing `tmp/shellchat_Lhgrandgtr-1.0.4.tar.gz` & `tmp/shellchat_Lhgrandgtr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellchat_Lhgrandgtr-1.0.4.tar", last modified: Thu Mar 21 09:03:25 2024, max compression
+gzip compressed data, was "shellchat_Lhgrandgtr-1.0.5.tar", last modified: Thu Apr  4 10:03:50 2024, max compression
```

## Comparing `shellchat_Lhgrandgtr-1.0.4.tar` & `shellchat_Lhgrandgtr-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-03-21 09:03:25.934728 shellchat_Lhgrandgtr-1.0.4/
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)      145 2024-03-21 09:03:25.934728 shellchat_Lhgrandgtr-1.0.4/PKG-INFO
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)       38 2024-03-21 09:03:25.934728 shellchat_Lhgrandgtr-1.0.4/setup.cfg
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)      353 2024-03-21 09:02:43.000000 shellchat_Lhgrandgtr-1.0.4/setup.py
-drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-03-21 09:03:25.930727 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr/
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)        0 2024-02-21 03:57:28.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr/__init__.py
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)     3632 2024-03-21 06:49:40.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr/main.py
-drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-03-21 09:03:25.934728 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)      145 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/PKG-INFO
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)      336 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/SOURCES.txt
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)        1 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/dependency_links.txt
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)       62 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/entry_points.txt
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)       35 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/requires.txt
--rw-r--r--   0 lahirud  (226828714) domain users (226800513)       21 2024-03-21 09:03:25.000000 shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr.egg-info/top_level.txt
+drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-04-04 10:03:50.489542 shellchat_Lhgrandgtr-1.0.5/
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)      145 2024-04-04 10:03:50.489542 shellchat_Lhgrandgtr-1.0.5/PKG-INFO
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)       38 2024-04-04 10:03:50.489542 shellchat_Lhgrandgtr-1.0.5/setup.cfg
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)      353 2024-04-04 10:03:10.000000 shellchat_Lhgrandgtr-1.0.5/setup.py
+drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-04-04 10:03:50.485542 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr/
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)        0 2024-02-21 03:57:28.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr/__init__.py
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)     4144 2024-04-04 09:55:22.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr/main.py
+drwxr-xr-x   0 lahirud  (226828714) domain users (226800513)        0 2024-04-04 10:03:50.489542 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)      145 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/PKG-INFO
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)      336 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/SOURCES.txt
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)        1 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/dependency_links.txt
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)       62 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/entry_points.txt
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)       35 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/requires.txt
+-rw-r--r--   0 lahirud  (226828714) domain users (226800513)       21 2024-04-04 10:03:50.000000 shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr.egg-info/top_level.txt
```

### Comparing `shellchat_Lhgrandgtr-1.0.4/shellchat_Lhgrandgtr/main.py` & `shellchat_Lhgrandgtr-1.0.5/shellchat_Lhgrandgtr/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
 from prompt_toolkit import prompt
 from prompt_toolkit.history import InMemoryHistory
 import requests
 import json
 import argparse
-from time import sleep
-from deprecated import deprecated
+
 
 style = Style.from_dict({
     "welcome": "bold underline",
     "question": "fg:#00FF00",
     "generated_text": "fg:#FF0000",
     "error": "fg:#FF0000",
     "prompt": "fg:#FFA500",
@@ -21,26 +20,31 @@
     payload = {
         "text": question
     }
 
     headers = {
         "Content-Type": "application/json"
     }
+    try:
+        response = requests.post(url, headers=headers, data=json.dumps(payload), stream=True)
 
-    response = requests.post(url, headers=headers, data=json.dumps(payload), stream=True)
-
-    if response.status_code == 200:
-        print_formatted_text(HTML("<ansired>B-chat:</ansired>"), style=style)
-        
-        # Print response character by character
-        for chunk in response.iter_content(chunk_size=1):
-            print_formatted_text(chunk.decode('utf-8'), end='', style=style)
-    else:
-        print_formatted_text(HTML("<ansired>Error:</ansired>"), HTML(f"<ansigreen>{response.text}</ansigreen>"), style=style)
-
+        if response.status_code == 200:
+            print_formatted_text(HTML("<ansired>B-chat:</ansired>"), style=style)
+          
+           
+            # Print response character by character
+            for chunk in response.iter_content(chunk_size=1):
+                print_formatted_text(chunk.decode(), end='', style=style)
+                
+            print()
+        else:
+            print_formatted_text(HTML("<ansired>Error:</ansired>"), HTML(f"<ansigreen>{response.text}</ansigreen>"), style=style)
+    except requests.exceptions.ConnectionError:
+        print_formatted_text(HTML("<ansired>Connection issue! Please try again.</ansired>"))
+        pass
 
     # # Execute the curl command to get the answer
     # process = subprocess.Popen(['curl', '-X', 'POST', 'http://10.101.15.172:8002/llm-process', '-H', 'Content-Type: application/json', '-d', f'{{"text": "{question}"}}', '--no-buffer'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     
     # # Initialize variables to track the first word arrival time and full response
     # first_word_received = False
     # first_word_time = None
@@ -78,29 +82,35 @@
 #             print_formatted_text(char, end='', style=style)
 #             sleep(0.05)
 #     else:
 #         print_formatted_text(HTML("<ansired>Error:</ansired>"), HTML(f"<ansigreen>{response.text}</ansigreen>"), style=style)
 
 
 def main():
-    print_formatted_text(HTML("<ansiblue>Welcome to Text Generation Interface!</ansiblue>"), style=style)
+    print_formatted_text(HTML("<ansibrightblue>Welcome to Text Generation Interface!</ansibrightblue>"), style=style)
     print_formatted_text(HTML("<ansiblue>Enter your question or type 'quit' to exit.</ansiblue>"), style=style)
 
     parser = argparse.ArgumentParser(description='Text Generation Interface')
-    parser.add_argument('--url', type=str, default='http://10.101.15.172:8002/llm-process',
-                        help='URL for text generation service')
+    parser.add_argument('--url', type=str,
+                        help='URL for text generation service', required=True)
 
     args = parser.parse_args()
+    
+    print_formatted_text(HTML(f"<ansicyan>Connected to {args.url}</ansicyan>"), style=style)
 
     history = InMemoryHistory()
 
     while True:
-        question = prompt("\nPrompt: ", style=style, history=history)
+        try:
+            question = prompt("\nPrompt: ", style=style, history=history)
 
-        if question.lower() == 'quit' or question.lower() == 'exit':
-            print("Goodbye!")
+            if question.lower() == 'quit' or question.lower() == 'exit':
+                print_formatted_text(HTML(f"<ansibrightgreen>Goodbye!</ansibrightgreen>"), style=style)
+                break
+
+            generate_text(question, args.url)
+        except KeyboardInterrupt:
+            print_formatted_text(HTML(f"<ansibrightgreen>Goodbye!</ansibrightgreen>"), style=style)
             break
 
-        generate_text(question, args.url)
-
 if __name__ == "__main__":
     main()
```


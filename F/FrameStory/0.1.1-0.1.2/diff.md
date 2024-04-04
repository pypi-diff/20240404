# Comparing `tmp/FrameStory-0.1.1.tar.gz` & `tmp/FrameStory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrameStory-0.1.1.tar", last modified: Thu Apr  4 14:40:43 2024, max compression
+gzip compressed data, was "FrameStory-0.1.2.tar", last modified: Thu Apr  4 14:52:32 2024, max compression
```

## Comparing `FrameStory-0.1.1.tar` & `FrameStory-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:40:43.651374 FrameStory-0.1.1/
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:40:43.650645 FrameStory-0.1.1/FrameStory.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3573 2024-04-04 14:40:43.000000 FrameStory-0.1.1/FrameStory.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      298 2024-04-04 14:40:43.000000 FrameStory-0.1.1/FrameStory.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-04 14:40:43.000000 FrameStory-0.1.1/FrameStory.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      104 2024-04-04 14:40:43.000000 FrameStory-0.1.1/FrameStory.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       18 2024-04-04 14:40:43.000000 FrameStory-0.1.1/FrameStory.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-04 13:56:00.000000 FrameStory-0.1.1/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3573 2024-04-04 14:40:43.651237 FrameStory-0.1.1/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2644 2024-04-04 14:36:29.000000 FrameStory-0.1.1/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:40:43.650871 FrameStory-0.1.1/frame_story/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 13:59:20.000000 FrameStory-0.1.1/frame_story/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3411 2024-04-04 14:31:09.000000 FrameStory-0.1.1/frame_story/video_describer.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-04 14:40:43.651431 FrameStory-0.1.1/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1278 2024-04-04 14:40:40.000000 FrameStory-0.1.1/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:40:43.651071 FrameStory-0.1.1/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 13:59:26.000000 FrameStory-0.1.1/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1805 2024-04-04 14:31:09.000000 FrameStory-0.1.1/tests/test_video_describer.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:32.812620 FrameStory-0.1.2/
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:32.811697 FrameStory-0.1.2/FrameStory.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3573 2024-04-04 14:52:32.000000 FrameStory-0.1.2/FrameStory.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      298 2024-04-04 14:52:32.000000 FrameStory-0.1.2/FrameStory.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-04 14:52:32.000000 FrameStory-0.1.2/FrameStory.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      104 2024-04-04 14:52:32.000000 FrameStory-0.1.2/FrameStory.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       18 2024-04-04 14:52:32.000000 FrameStory-0.1.2/FrameStory.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-04 13:56:00.000000 FrameStory-0.1.2/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3573 2024-04-04 14:52:32.812494 FrameStory-0.1.2/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2644 2024-04-04 14:36:29.000000 FrameStory-0.1.2/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:32.811923 FrameStory-0.1.2/frame_story/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 13:59:20.000000 FrameStory-0.1.2/frame_story/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3479 2024-04-04 14:50:50.000000 FrameStory-0.1.2/frame_story/video_describer.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-04 14:52:32.812662 FrameStory-0.1.2/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1278 2024-04-04 14:51:00.000000 FrameStory-0.1.2/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:32.812223 FrameStory-0.1.2/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 13:59:26.000000 FrameStory-0.1.2/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1805 2024-04-04 14:31:09.000000 FrameStory-0.1.2/tests/test_video_describer.py
```

### Comparing `FrameStory-0.1.1/FrameStory.egg-info/PKG-INFO` & `FrameStory-0.1.2/FrameStory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameStory
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for creating video descriptions by analyzing and extracting significant frames.
 Home-page: https://github.com/chigwell/FrameStory
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FrameStory-0.1.1/LICENSE` & `FrameStory-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FrameStory-0.1.1/PKG-INFO` & `FrameStory-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameStory
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for creating video descriptions by analyzing and extracting significant frames.
 Home-page: https://github.com/chigwell/FrameStory
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FrameStory-0.1.1/README.md` & `FrameStory-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FrameStory-0.1.1/frame_story/video_describer.py` & `FrameStory-0.1.2/frame_story/video_describer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from tqdm import tqdm
 
 
 IMAGE_CAPTIONING_MODEL = "Salesforce/blip-image-captioning-large"
 
 
 class VideoDescriber:
-    def __init__(self, model_name=IMAGE_CAPTIONING_MODEL, show_progress=True, max_tokens=100, temp_dir='tmp'):
+    def __init__(self, model_name=IMAGE_CAPTIONING_MODEL, show_progress=True, max_tokens=100, temp_dir='tmp', threshold=50000):
         self.processor = BlipProcessor.from_pretrained(model_name)
         self.model = BlipForConditionalGeneration.from_pretrained(model_name)
         self.show_progress = show_progress
         self.max_tokens = max_tokens
         self.temp_dir = temp_dir
+        self.threshold = threshold
 
     def download_video(self, video_url, save_path):
         video_content = requests.get(video_url).content
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         with open(save_path, 'wb') as video_file:
             video_file.write(video_content)
 
@@ -63,15 +64,15 @@
                     print({"start": time, "dur": duration, "desc": description})
         return descriptions
 
     def get_video_descriptions(self, video_path=None, video_url=None):
         if video_url:
             video_path = os.path.join(self.temp_dir, 'temp_video.mp4')
             self.download_video(video_url, video_path)
-        frames, times = self.extract_significant_frames(video_path)
+        frames, times = self.extract_significant_frames(video_path, self.threshold)
         descriptions = self.describe_frames(frames, times)
         return descriptions
 
 # Example usage
 # if __name__ == '__main__':
 #     video_url = 'https://cdn.vidwidget.ru/storage/videos/0d26ed03-2085-4977-92ce-930c5980173d.mp4'
 #     describer = VideoDescriber()
```

### Comparing `FrameStory-0.1.1/setup.py` & `FrameStory-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrameStory',
-    version='0.1.1',
+    version='0.1.2',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='A Python package for creating video descriptions by analyzing and extracting significant frames.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/FrameStory',
     packages=find_packages(),
```

### Comparing `FrameStory-0.1.1/tests/test_video_describer.py` & `FrameStory-0.1.2/tests/test_video_describer.py`

 * *Files identical despite different names*


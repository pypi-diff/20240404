# Comparing `tmp/python_course_by_ty-0.1.5.tar.gz` & `tmp/python_course_by_ty-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_course_by_ty-0.1.5.tar", last modified: Fri Mar  8 14:16:57 2024, max compression
+gzip compressed data, was "python_course_by_ty-0.1.6.tar", last modified: Thu Apr  4 21:37:02 2024, max compression
```

## Comparing `python_course_by_ty-0.1.5.tar` & `python_course_by_ty-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-03-08 14:16:57.493867 python_course_by_ty-0.1.5/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      590 2024-03-08 14:16:57.493591 python_course_by_ty-0.1.5/PKG-INFO
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-03-08 14:16:57.492349 python_course_by_ty-0.1.5/python_course_by_ty/
--rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.5/python_course_by_ty/__init__.py
--rw-r--r--   0 tygriffiths   (501) staff       (20)    87041 2024-03-08 14:15:48.000000 python_course_by_ty-0.1.5/python_course_by_ty/python_course.py
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-03-08 14:16:57.493274 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      590 2024-03-08 14:16:57.000000 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/PKG-INFO
--rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-03-08 14:16:57.000000 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/SOURCES.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-03-08 14:16:57.000000 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/dependency_links.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-03-08 14:16:57.000000 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/requires.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-03-08 14:16:57.000000 python_course_by_ty-0.1.5/python_course_by_ty.egg-info/top_level.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-03-08 14:16:57.493921 python_course_by_ty-0.1.5/setup.cfg
--rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-03-08 14:15:25.000000 python_course_by_ty-0.1.5/setup.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.823076 python_course_by_ty-0.1.6/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:37:02.822954 python_course_by_ty-0.1.6/PKG-INFO
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.821440 python_course_by_ty-0.1.6/python_course_by_ty/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.6/python_course_by_ty/__init__.py
+-rw-r--r--   0 tygriffiths   (501) staff       (20)    88802 2024-04-04 21:31:48.000000 python_course_by_ty-0.1.6/python_course_by_ty/python_course.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.822748 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/PKG-INFO
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/SOURCES.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/dependency_links.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/requires.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/top_level.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-04-04 21:37:02.823129 python_course_by_ty-0.1.6/setup.cfg
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-04-04 21:35:50.000000 python_course_by_ty-0.1.6/setup.py
```

### Comparing `python_course_by_ty-0.1.5/python_course_by_ty/python_course.py` & `python_course_by_ty-0.1.6/python_course_by_ty/python_course.py`

 * *Files 2% similar despite different names*

```diff
@@ -1044,19 +1044,19 @@
         content_score = content_scoring_test(content)
         genres = movie["genre"]
         try:
             imdb_rating = float(movie["imdb_rating"])
         except:
             imdb_rating = 0
         try:
-            rotten_rating = float(movie["ratings"][1]["value"][:-1])
+            rotten_rating = int(movie["ratings"][1]["value"][:-1])
         except:
             rotten_rating = 0
         try:
-            meta_rating = float(movie["ratings"][2]["value"][:-4])
+            meta_rating = int(movie["ratings"][2]["value"][:-4])
         except:
             meta_rating = 0
         movie_list = [
             m[0],
             m[1],
             content,
             genres,
@@ -1110,57 +1110,57 @@
     movie_list = movie_filter_test(movies)
     filtered_movies = filter_test(movie_list, content=content, genre=genre)
 
     if filtered_movies == answer:
         print("Angry Angels")
     else:
         print(
-            "Your function failed for the parameters 'movie_filter(movies, 'G', content_filter='Animation')'"
+            "Your function failed for the parameters 'movie_filter(all_movies, 'G', genre='Animation')'"
         )
 
 
 def test5_2(
     answer, movies, content=None, genre=None, imdb=None, rotten=None, meta=None
 ):
     movie_list = movie_filter_test(movies)
     filtered_movies = filter_test(movie_list, content=content, imdb=imdb)
 
     if filtered_movies == answer:
         print("Haunted Hot Dogs")
     else:
         print(
-            "Your function failed for the parameters 'movie_filter(movies, 'R', imdb_filter=8.0)'"
+            "Your function failed for the parameters 'movie_filter(all_movies, 'R', imdb=8.0)'"
         )
 
 
 def test5_3(
     answer, movies, content=None, genre=None, imdb=None, rotten=None, meta=None
 ):
     movie_list = movie_filter_test(movies)
     filtered_movies = filter_test(movie_list, content=content, rotten=rotten)
 
     if filtered_movies == answer:
         print("Goat Warriors")
     else:
         print(
-            "Your function failed for the parameters 'movie_filter(movies, 'PG', rotten_filter=60)'"
+            "Your function failed for the parameters 'movie_filter(all_movies, 'PG', rotten_filter=60)'"
         )
 
 
 def test5_4(
     answer, movies, content=None, genre=None, imdb=None, rotten=None, meta=None
 ):
     movie_list = movie_filter_test(movies)
     filtered_movies = filter_test(movie_list, content=content, meta=meta)
 
     if filtered_movies == answer:
         print("Fully Automatic PEZ Dispensers")
     else:
         print(
-            "Your function failed for the parameters 'movie_filter(movies, 'PG-13', meta_filter=75)'"
+            "Your function failed for the parameters 'movie_filter(all_movies, 'PG-13', meta_filter=75)'"
         )
 
 
 # Project 6 Problem 1
 def test6_1(answer):
     test = [
         (
@@ -1495,7 +1495,95 @@
     ]
     if answer == test:
         print("Vantablack")
     else:
         print(
             "Your query does not return the expected results. The top 10 expected films (not in order) are: The Godfather Part III, The Conversation, Network, Apocalypse Now, Star Wars: Episode IV - A New Hope, Sercipo, Dog Day Afternoon, Amadeus, Mr. Bean, The Simpsons"
         )
+
+
+# Project 9
+# Question 1
+def test9_1(answer):
+    if answer == "cool_stuff":
+        print("Taco Tornado")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 2
+def test9_2(answer):
+    if answer == "cool_stuff":
+        print("Enchilada Earthquake")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 3
+def test9_3(answer):
+    if answer == "1f50f920176fa81dab994f9023523100":
+        print("Hummus Hurricane")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 4
+def test9_4(answer):
+    if answer == "consoles_games":
+        print("Hamburger Hailstorm")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 5
+def test9_5(answer):
+    data = {
+        "month": [
+            "2017-01",
+            "2017-02",
+            "2017-03",
+            "2017-04",
+            "2017-05",
+            "2017-06",
+            "2017-07",
+            "2017-08",
+            "2017-09",
+            "2017-10",
+            "2017-11",
+            "2017-12",
+        ],
+        "avg_order": [
+            169.92,
+            161.36,
+            159.92,
+            170.99,
+            158.16,
+            154.14,
+            146.01,
+            156.35,
+            179.7,
+            168.13,
+            159.41,
+            150.89,
+        ],
+    }
+    df = pd.DataFrame(data)
+    if answer == df:
+        print("French Fries Flash Flood")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 6
+def test9_6(answer1, answer2):
+    if answer1 == 4.29 and answer2 == 2.35:
+        print("Avocado Avalanche")
+    else:
+        print("Your answer is incorrect.")
+
+
+# Question 7
+def test9_7(answer):
+    if answer == 0.51:
+        print("Lasagna Lighting Storm")
+    else:
+        print("Your answer is incorrect.")
```

### Comparing `python_course_by_ty-0.1.5/setup.py` & `python_course_by_ty-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python_course_by_ty",
-    version="0.1.5",
+    version="0.1.6",
     description="A package for testing student answers to project questions.",
     url="https://github.com/TyGriffiths/python_course_by_ty",
     author="Ty Griffiths",
     author_email="griffiths.ty@yahoo.com",
     license="GNU General Public License v3.0",
     packages=["python_course_by_ty"],
     install_requires=[
```


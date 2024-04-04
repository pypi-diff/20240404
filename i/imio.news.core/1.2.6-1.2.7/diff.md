# Comparing `tmp/imio.news.core-1.2.6.tar.gz` & `tmp/imio.news.core-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.news.core-1.2.6.tar", last modified: Fri Mar 29 10:50:51 2024, max compression
+gzip compressed data, was "imio.news.core-1.2.7.tar", last modified: Thu Apr  4 15:57:26 2024, max compression
```

## Comparing `imio.news.core-1.2.6.tar` & `imio.news.core-1.2.7.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3277 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      665 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6555 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2209 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.910371 imio.news.core-1.2.6/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7986 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       65 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-03-29 10:50:51.938371 imio.news.core-1.2.6/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2328 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.886371 imio.news.core-1.2.6/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.910371 imio.news.core-1.2.6/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.914371 imio.news.core-1.2.6/src/imio/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.918371 imio.news.core-1.2.6/src/imio/news/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      259 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.918371 imio.news.core-1.2.6/src/imio/news/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/browser/bring_news_into_news_folders/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3557 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      595 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      791 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      226 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1742 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/folder/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.922371 imio.news.core-1.2.6/src/imio/news/core/contents/newsfolder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsfolder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsfolder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsfolder/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.926371 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      690 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5073 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5608 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2415 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.894371 imio.news.core-1.2.6/src/imio/news/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.926371 imio.news.core-1.2.6/src/imio/news/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6592 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/faceted/config/news.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4126 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1543 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      199 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      347 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      762 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.894371 imio.news.core-1.2.6/src/imio/news/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.926371 imio.news.core-1.2.6/src/imio/news/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      167 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2007 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/repositorytool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      980 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.930371 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1613 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1372 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1432 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1554 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.930371 imio.news.core-1.2.6/src/imio/news/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      876 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.930371 imio.news.core-1.2.6/src/imio/news/core/serializer/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/serializer/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      175 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/serializer/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      579 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/serializer/newsitem.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      663 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6032 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1342 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1805 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.930371 imio.news.core-1.2.6/src/imio/news/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2801 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_bring_news_into_news_folders.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1598 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3380 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3550 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_indexer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2222 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8040 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9084 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_newsfolder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14046 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_newsitem.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      929 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1950 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3490 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5134 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4744 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.902371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1003_to_1004/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      282 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1007_to_1008/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.902371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      309 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1009_to_1010/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      218 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2185 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1660 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      519 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/viewlets/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.934371 imio.news.core-1.2.6/src/imio/news/core/viewlets/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      357 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/viewlets/news/button_to_bring_news.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1121 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/viewlets/news.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4363 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1003 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio/news/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-29 10:50:51.914371 imio.news.core-1.2.6/src/imio.news.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6555 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4992 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       15 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      278 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-03-29 10:50:51.000000 imio.news.core-1.2.6/src/imio.news.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3423 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      665 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6701 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2209 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7986 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       65 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/requirements.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2328 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      259 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3557 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      595 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      791 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      226 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/entity/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1742 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      690 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5073 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5483 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/serializer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5608 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2415 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/converters.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/faceted/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6592 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/faceted/config/news.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4126 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1543 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      199 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      347 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      762 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      167 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2007 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/contentrules.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/diff_tool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/repositorytool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      980 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1613 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1372 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1432 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1554 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      876 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/serializer/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      175 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      579 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/newsitem.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      663 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6032 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1342 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1805 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/resources/plone.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2801 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_bring_news_into_news_folders.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1598 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3380 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_entity.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3550 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_indexer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2222 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8040 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_multilingual.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9084 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_newsfolder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14046 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_newsitem.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      929 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1950 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3490 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5134 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4744 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      282 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      309 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1009_to_1010/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      218 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2185 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1660 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      519 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/viewlets/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      357 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/news/button_to_bring_news.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1121 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/news.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4363 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1003 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio.news.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6701 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4992 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       15 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      278 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/top_level.txt
```

### Comparing `imio.news.core-1.2.6/CHANGES.rst` & `imio.news.core-1.2.7/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.7 (2024-04-04)
+------------------
+
+- Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
+  [boulch]
+
+
 1.2.6 (2024-03-28)
 ------------------
 
 - MWEBPM-9 : Add container_uid as metadata_field to retrieve news folder id/title in news serializer and set it in our json dataset
   [boulch]
```

### Comparing `imio.news.core-1.2.6/DEVELOP.rst` & `imio.news.core-1.2.7/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/LICENSE.GPL` & `imio.news.core-1.2.7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/LICENSE.rst` & `imio.news.core-1.2.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/PKG-INFO` & `imio.news.core-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.6
+Version: 1.2.7
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
@@ -128,14 +128,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.7 (2024-04-04)
+------------------
+
+- Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
+  [boulch]
+
+
 1.2.6 (2024-03-28)
 ------------------
 
 - MWEBPM-9 : Add container_uid as metadata_field to retrieve news folder id/title in news serializer and set it in our json dataset
   [boulch]
```

### Comparing `imio.news.core-1.2.6/README.rst` & `imio.news.core-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/docs/conf.py` & `imio.news.core-1.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/setup.cfg` & `imio.news.core-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/setup.py` & `imio.news.core-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.news.core",
-    version="1.2.6",
+    version="1.2.7",
     description="Core product for iMio news website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.news.core-1.2.6/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py` & `imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/browser/configure.zcml` & `imio.news.core-1.2.7/src/imio/news/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/configure.zcml` & `imio.news.core-1.2.7/src/imio/news/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/entity/content.py` & `imio.news.core-1.2.7/src/imio/news/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/newsfolder/content.py` & `imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/configure.zcml` & `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/content.py` & `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/view.pt` & `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/view.pt`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/contents/newsitem/views.py` & `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/views.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/faceted/config/news.xml` & `imio.news.core-1.2.7/src/imio/news/core/faceted/config/news.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/indexers.py` & `imio.news.core-1.2.7/src/imio/news/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/indexers.zcml` & `imio.news.core-1.2.7/src/imio/news/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/permissions.zcml` & `imio.news.core-1.2.7/src/imio/news/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/catalog.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/contentrules.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/registry.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/rolemap.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.Entity.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.Folder.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml` & `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/profiles.zcml` & `imio.news.core-1.2.7/src/imio/news/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/serializer/newsitem.py` & `imio.news.core-1.2.7/src/imio/news/core/serializer/newsitem.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/setuphandlers.py` & `imio.news.core-1.2.7/src/imio/news/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/subscribers.py` & `imio.news.core-1.2.7/src/imio/news/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/subscribers.zcml` & `imio.news.core-1.2.7/src/imio/news/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/testing.py` & `imio.news.core-1.2.7/src/imio/news/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/resources/plone.png` & `imio.news.core-1.2.7/src/imio/news/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/robot/test_example.robot` & `imio.news.core-1.2.7/src/imio/news/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_bring_news_into_news_folders.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_bring_news_into_news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_cropping.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_entity.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_indexer.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_local_roles.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_multilingual.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_newsfolder.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_newsfolder.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_newsitem.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_newsitem.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_robot.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_setup.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_utils.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/tests/test_vocabularies.py` & `imio.news.core-1.2.7/src/imio/news/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/upgrades/configure.zcml` & `imio.news.core-1.2.7/src/imio/news/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml` & `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml` & `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml` & `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/upgrades/upgrades.py` & `imio.news.core-1.2.7/src/imio/news/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/utils.py` & `imio.news.core-1.2.7/src/imio/news/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/viewlets/configure.zcml` & `imio.news.core-1.2.7/src/imio/news/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/viewlets/news.py` & `imio.news.core-1.2.7/src/imio/news/core/viewlets/news.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/vocabularies.py` & `imio.news.core-1.2.7/src/imio/news/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio/news/core/vocabularies.zcml` & `imio.news.core-1.2.7/src/imio/news/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.6/src/imio.news.core.egg-info/PKG-INFO` & `imio.news.core-1.2.7/src/imio.news.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.6
+Version: 1.2.7
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
@@ -128,14 +128,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.7 (2024-04-04)
+------------------
+
+- Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
+  [boulch]
+
+
 1.2.6 (2024-03-28)
 ------------------
 
 - MWEBPM-9 : Add container_uid as metadata_field to retrieve news folder id/title in news serializer and set it in our json dataset
   [boulch]
```

### Comparing `imio.news.core-1.2.6/src/imio.news.core.egg-info/SOURCES.txt` & `imio.news.core-1.2.7/src/imio.news.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/powermanim-0.1.1.tar.gz` & `tmp/powermanim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powermanim-0.1.1.tar", last modified: Mon Mar 25 15:53:54 2024, max compression
+gzip compressed data, was "powermanim-0.1.2.tar", last modified: Wed Apr  3 22:28:46 2024, max compression
```

## Comparing `powermanim-0.1.1.tar` & `powermanim-0.1.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.881344 powermanim-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-25 15:51:12.000000 powermanim-0.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 15:51:12.000000 powermanim-0.1.1/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 15:51:12.000000 powermanim-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.865344 powermanim-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-25 15:51:12.000000 powermanim-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-25 15:51:12.000000 powermanim-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-25 15:51:12.000000 powermanim-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-25 15:51:12.000000 powermanim-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-25 15:51:12.000000 powermanim-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 15:53:54.881344 powermanim-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-25 15:51:12.000000 powermanim-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/data/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 15:51:12.000000 powermanim-0.1.1/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/.hugo_build.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/assets/media/
--rw-r--r--   0 runner    (1001) docker     (127)    39583 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/assets/media/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/assets/media/book.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/assets/media/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/assets/media/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/assets/media/icons/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/assets/scss/custom.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/config/_default/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/config/_default/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/config/_default/languages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/config/_default/menus.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/config/_default/params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/content/authors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/content/authors/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/authors/admin/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/content/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/content/docs/chapter1/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter1/_index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter1/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter1/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter1/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/content/docs/chapter2/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter2/_index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter2/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter2/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/docs/chapter2/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.873344 powermanim-0.1.1/docs/content/home/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/home/animations.md
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/home/features.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/content/home/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/go.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/layouts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/layouts/partials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/docs/layouts/partials/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/layouts/partials/views/masonry.html
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/netlify.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/docs/static/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/docs/static/uploads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-25 15:53:49.000000 powermanim-0.1.1/env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-25 15:51:12.000000 powermanim-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-25 15:53:54.881344 powermanim-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-25 15:51:12.000000 powermanim-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.869344 powermanim-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/components/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/directionalarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/groupactivable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/invariance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/components/numberslider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/layouts/arrangedbullets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/layouts/switchpalette.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2152 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/scripts/build_anims
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/showcase/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/showcase/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/directionalarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/groupactivable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/invariance.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/components/numberslider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim/showcase/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/layouts/arrangedbullets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/layouts/switchpalette.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/showcasescene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.881344 powermanim-0.1.1/src/powermanim/showcase/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/templates/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/showcase/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.881344 powermanim-0.1.1/src/powermanim/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/templates/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-25 15:51:12.000000 powermanim-0.1.1/src/powermanim/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.877344 powermanim-0.1.1/src/powermanim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:52:01.000000 powermanim-0.1.1/src/powermanim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-25 15:53:54.000000 powermanim-0.1.1/src/powermanim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.881344 powermanim-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:51:12.000000 powermanim-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:54.881344 powermanim-0.1.1/tests/showcase/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-25 15:51:12.000000 powermanim-0.1.1/tests/showcase/test_showcasing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.381869 powermanim-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 22:26:02.000000 powermanim-0.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 22:26:02.000000 powermanim-0.1.2/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 22:26:02.000000 powermanim-0.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-03 22:26:02.000000 powermanim-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-03 22:26:02.000000 powermanim-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 22:26:02.000000 powermanim-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-03 22:26:02.000000 powermanim-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 22:26:02.000000 powermanim-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 22:28:46.381869 powermanim-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-03 22:26:02.000000 powermanim-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 22:26:02.000000 powermanim-0.1.2/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/.hugo_build.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/assets/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    39583 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/assets/media/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/assets/media/book.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/assets/media/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/assets/media/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/assets/media/icons/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/assets/scss/custom.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/config/_default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/config/_default/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/config/_default/languages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/config/_default/menus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/config/_default/params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/content/authors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/content/authors/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/authors/admin/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/content/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/content/docs/chapter1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter1/_index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter1/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter1/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter1/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/content/docs/chapter2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter2/_index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter2/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter2/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/docs/chapter2/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/content/home/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/home/animations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/home/features.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/content/home/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/go.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/layouts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/layouts/partials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.373869 powermanim-0.1.2/docs/layouts/partials/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/layouts/partials/views/masonry.html
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/netlify.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/docs/static/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/docs/static/uploads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 22:28:43.000000 powermanim-0.1.2/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-03 22:26:02.000000 powermanim-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 22:28:46.381869 powermanim-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 22:26:02.000000 powermanim-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.369869 powermanim-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/directionalarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/groupactivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/invariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/components/numberslider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/layouts/arrangedbullets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/layouts/switchpalette.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2152 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/scripts/build_anims
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/showcase/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/showcase/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/directionalarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/groupactivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/invariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/components/numberslider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim/showcase/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/layouts/arrangedbullets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/layouts/switchpalette.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/showcasescene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.381869 powermanim-0.1.2/src/powermanim/showcase/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/templates/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/showcase/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.381869 powermanim-0.1.2/src/powermanim/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/templates/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-03 22:26:02.000000 powermanim-0.1.2/src/powermanim/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.377869 powermanim-0.1.2/src/powermanim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:26:52.000000 powermanim-0.1.2/src/powermanim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 22:28:46.000000 powermanim-0.1.2/src/powermanim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.381869 powermanim-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:26:02.000000 powermanim-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:28:46.381869 powermanim-0.1.2/tests/showcase/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 22:26:02.000000 powermanim-0.1.2/tests/showcase/test_showcasing.py
```

### Comparing `powermanim-0.1.1/.github/workflows/publish.yml` & `powermanim-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/.github/workflows/tests.yml` & `powermanim-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/.gitignore` & `powermanim-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/.pre-commit-config.yaml` & `powermanim-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/LICENSE` & `powermanim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/PKG-INFO` & `powermanim-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.1.1 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.1.2 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.1.1/README.md` & `powermanim-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/assets/media/banner.png` & `powermanim-0.1.2/docs/assets/media/banner.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/assets/media/book.svg` & `powermanim-0.1.2/docs/assets/media/book.svg`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/assets/media/icon.png` & `powermanim-0.1.2/docs/assets/media/icon.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/assets/scss/custom.scss` & `powermanim-0.1.2/docs/assets/scss/custom.scss`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/config/_default/config.yaml` & `powermanim-0.1.2/docs/config/_default/config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/config/_default/languages.yaml` & `powermanim-0.1.2/docs/config/_default/languages.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/config/_default/params.yaml` & `powermanim-0.1.2/docs/config/_default/params.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter1/_index.md` & `powermanim-0.1.2/docs/content/docs/chapter1/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter1/reading-list.md` & `powermanim-0.1.2/docs/content/docs/chapter1/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter1/syllabus.md` & `powermanim-0.1.2/docs/content/docs/chapter1/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter1/takeaways.md` & `powermanim-0.1.2/docs/content/docs/chapter1/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter2/_index.md` & `powermanim-0.1.2/docs/content/docs/chapter2/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter2/reading-list.md` & `powermanim-0.1.2/docs/content/docs/chapter2/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter2/syllabus.md` & `powermanim-0.1.2/docs/content/docs/chapter2/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/docs/chapter2/takeaways.md` & `powermanim-0.1.2/docs/content/docs/chapter2/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/content/home/animations.md` & `powermanim-0.1.2/docs/content/home/animations.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/docs/layouts/partials/views/masonry.html` & `powermanim-0.1.2/docs/layouts/partials/views/masonry.html`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/pyproject.toml` & `powermanim-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/setup.cfg` & `powermanim-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/__init__.py` & `powermanim-0.1.2/src/powermanim/__init__.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/chartbars.py` & `powermanim-0.1.2/src/powermanim/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/directionalarrow.py` & `powermanim-0.1.2/src/powermanim/components/directionalarrow.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/groupactivable.py` & `powermanim-0.1.2/src/powermanim/components/groupactivable.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/invariance.py` & `powermanim-0.1.2/src/powermanim/components/invariance.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/logo.py` & `powermanim-0.1.2/src/powermanim/components/logo.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/components/numberslider.py` & `powermanim-0.1.2/src/powermanim/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/layouts/switchpalette.py` & `powermanim-0.1.2/src/powermanim/layouts/switchpalette.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/scripts/build_anims` & `powermanim-0.1.2/src/powermanim/scripts/build_anims`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/__init__.py` & `powermanim-0.1.2/src/powermanim/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/components/chartbars.py` & `powermanim-0.1.2/src/powermanim/showcase/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/components/directionalarrow.py` & `powermanim-0.1.2/src/powermanim/showcase/components/directionalarrow.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/components/groupactivable.py` & `powermanim-0.1.2/src/powermanim/showcase/components/groupactivable.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/components/invariance.py` & `powermanim-0.1.2/src/powermanim/showcase/components/invariance.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/components/numberslider.py` & `powermanim-0.1.2/src/powermanim/showcase/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/layouts/arrangedbullets.py` & `powermanim-0.1.2/src/powermanim/showcase/layouts/arrangedbullets.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,16 +17,15 @@
             Bullet("First element", level=1, symbol="(1)"),
             Bullet("Second element", level=1, symbol="(2)"),
             Bullet("Third element", level=1, symbol="(3)"),
         ]
         g_rows = VGroup(*rows).set_opacity(0.25).scale(0.9)
         g_rows.target = ArrangedBullets(
             *g_rows.copy(),
-            line_spacing=MED_LARGE_BUFF * 1.25,
-            left_buff=MED_LARGE_BUFF * 3,
+            line_spacing_decay=0.65,
         ).set_opacity(1)
 
         self.play(
             MoveToTarget(g_rows),
             rate_func=there_and_back_with_pause,
             run_time=3,
         )
```

### Comparing `powermanim-0.1.1/src/powermanim/showcase/layouts/switchpalette.py` & `powermanim-0.1.2/src/powermanim/showcase/layouts/switchpalette.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/showcasescene.py` & `powermanim-0.1.2/src/powermanim/showcase/showcasescene.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/showcase/templates/bulletlist.py` & `powermanim-0.1.2/src/powermanim/showcase/templates/bulletlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             Bullet("Third element", level=1, symbol="(3)", group=4),
         ]
         VGroup(*rows).set_opacity(0.5).scale(0.8)
 
         bullets = BulletList(
             *rows,
             scale_active=1.2,
+            line_spacing_decay=0.65,
         )
         self.add(bullets)
 
         self.play(bullets.also_next())
         self.play(bullets.also_next())
         self.play(bullets.also_next())
         self.play(bullets.also_next())
```

### Comparing `powermanim-0.1.1/src/powermanim/showcase/templates/reference.py` & `powermanim-0.1.2/src/powermanim/showcase/templates/reference.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim/templates/bulletlist.py` & `powermanim-0.1.2/src/powermanim/templates/bulletlist.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 
 
 class BulletList(GroupActivable):
     def __init__(
         self,
         *rows: T.Union[MathBullet, Tex, Text],
         line_spacing: float = MED_LARGE_BUFF * 1.5,
+        line_spacing_decay: float = 1.0,  # TODO: in the next version, change default to 0.65
         indent_buff: float = MED_LARGE_BUFF * 1.5,
-        left_buff: float = MED_LARGE_BUFF * 2,
-        global_shift: float = 0.0,
         inactive_opacity: float = 0.5,
         active_opacity: float = 1.0,
-        scale_active: float = 1.0,
+        scale_active: float = 1.0,  # TODO: in the next version, change default to 1.2
         anim_lag_ratio: float = 0,
+        left_buff: float = MED_LARGE_BUFF * 2,
     ):
         """A class to represent an highlatable list of items.
 
         Args:
             rows: A list of items to be displayed.
             line_spacing: The spacing between the rows.
+            line_spacing_decay: The rate at which the spacing decays at each level
             indent_buff: The spacing between the bullet and the text.
-            left_buff: The spacing between the left edge of the rows and the left edge of the screen.
-            global_shift: The global_shift to apply to the rows.
             inactive_opacity: The opacity of the inactive items.
             active_opacity: The opacity of the active items.
             scale_active: The scale of the active items.
             anim_lag_ratio: The animation lag ratio.
+            left_buff: The buff from the left edge
         """
         self.arranged_list = ArrangedBullets(
             *rows,
             line_spacing=line_spacing,
+            line_spacing_decay=line_spacing_decay,
             indent_buff=indent_buff,
             left_buff=left_buff,
-            global_shift=global_shift,
         )
 
         super().__init__(
             *(
                 VAutoActivable(
                     x,
                     active_fill_opacity=active_opacity,
```

### Comparing `powermanim-0.1.1/src/powermanim/templates/sectiontitle.py` & `powermanim-0.1.2/src/powermanim/templates/sectiontitle.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.1.1/src/powermanim.egg-info/PKG-INFO` & `powermanim-0.1.2/src/powermanim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.1.1 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.1.2 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.1.1/src/powermanim.egg-info/SOURCES.txt` & `powermanim-0.1.2/src/powermanim.egg-info/SOURCES.txt`

 * *Files identical despite different names*


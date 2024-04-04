# Comparing `tmp/conan-2.2.1.tar.gz` & `tmp/conan-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.2.1.tar", last modified: Wed Mar 20 17:52:51 2024, max compression
+gzip compressed data, was "dist/conan-2.2.2.tar", last modified: Mon Mar 25 15:15:52 2024, max compression
```

## Comparing `conan-2.2.1.tar` & `conan-2.2.2.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.385523 conan-2.2.1/
--rw-r--r--   0 root         (0) root         (0)     1084 2024-03-20 17:52:44.000000 conan-2.2.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-20 17:52:44.000000 conan-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8618 2024-03-20 17:52:51.385523 conan-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6335 2024-03-20 17:52:44.000000 conan-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.347520 conan-2.2.1/conan/
--rw-r--r--   0 root         (0) root         (0)      165 2024-03-20 17:52:44.000000 conan-2.2.1/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.348521 conan-2.2.1/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2455 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)    12046 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     9460 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.350521 conan-2.2.1/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11757 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/command.py
--rw-r--r--   0 root         (0) root         (0)     9255 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     4793 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2714 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11805 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3961 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)    17548 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5465 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4808 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     7441 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)    13285 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     6670 2024-03-20 17:52:44.000000 conan-2.2.1/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.351521 conan-2.2.1/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7430 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    11875 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8279 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.354521 conan-2.2.1/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3994 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     7489 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     9158 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3252 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     3157 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5798 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)    21433 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4704 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)    13371 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     7511 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3244 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     6487 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     6871 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      653 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      490 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.354521 conan-2.2.1/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.354521 conan-2.2.1/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5535 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)    14752 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.355521 conan-2.2.1/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.355521 conan-2.2.1/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6412 2024-03-20 17:52:44.000000 conan-2.2.1/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2024-03-20 17:52:44.000000 conan-2.2.1/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.356521 conan-2.2.1/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.356521 conan-2.2.1/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19809 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/detect_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.358521 conan-2.2.1/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3810 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2916 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2041 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     4565 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     8212 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/local_recipes_index.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.358521 conan-2.2.1/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11189 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.359521 conan-2.2.1/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3949 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     9222 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/cache/home_paths.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/integrity_check.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/internal_tools.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-03-20 17:52:44.000000 conan-2.2.1/conan/internal/upload_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.359521 conan-2.2.1/conan/tools/
--rw-r--r--   0 root         (0) root         (0)      384 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.359521 conan-2.2.1/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.360521 conan-2.2.1/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11835 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16239 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.361522 conan-2.2.1/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11121 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    16208 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.361522 conan-2.2.1/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      217 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14472 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.361522 conan-2.2.1/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10886 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.362522 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3944 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14900 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    20156 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3656 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     4746 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    16611 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.363522 conan-2.2.1/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45120 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13892 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.363522 conan-2.2.1/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26546 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3601 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.364522 conan-2.2.1/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      535 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6925 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)    24002 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     4177 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     6540 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.365522 conan-2.2.1/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.366522 conan-2.2.1/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      320 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    14034 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3698 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)    27066 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/makedeps.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    19100 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.366522 conan-2.2.1/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3387 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    23416 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)     8113 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.367522 conan-2.2.1/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6498 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.367522 conan-2.2.1/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.367522 conan-2.2.1/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4702 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5093 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    23068 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.368522 conan-2.2.1/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19246 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2967 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4984 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    11139 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    15003 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.369522 conan-2.2.1/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.369522 conan-2.2.1/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9897 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.369522 conan-2.2.1/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12771 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.370522 conan-2.2.1/conan/tools/scons/
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/scons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/scons/sconsdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.370522 conan-2.2.1/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-03-20 17:52:44.000000 conan-2.2.1/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.348521 conan-2.2.1/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8618 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9622 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      469 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-20 17:52:51.000000 conan-2.2.1/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.371522 conan-2.2.1/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2024-03-20 17:52:44.000000 conan-2.2.1/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.373522 conan-2.2.1/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.373522 conan-2.2.1/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4924 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cache/editable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.373522 conan-2.2.1/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7808 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12332 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/cmd/uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.374523 conan-2.2.1/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conanfile/implementations.py
--rw-r--r--   0 root         (0) root         (0)     2138 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.375523 conan-2.2.1/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     7414 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7899 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     4582 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.375523 conan-2.2.1/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10333 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6706 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.375523 conan-2.2.1/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)    10315 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.377523 conan-2.2.1/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     4348 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    15453 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    23117 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    21937 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    21344 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     7221 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6480 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     5326 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21840 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    16978 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    14595 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.378523 conan-2.2.1/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5837 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6923 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     3945 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2488 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/remote_credentials.py
--rw-r--r--   0 root         (0) root         (0)     5424 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     9571 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    14934 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     9149 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/rest_client_local_recipe_index.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.378523 conan-2.2.1/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4205 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     4223 2024-03-20 17:52:44.000000 conan-2.2.1/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2024-03-20 17:52:44.000000 conan-2.2.1/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-03-20 17:52:44.000000 conan-2.2.1/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-03-20 17:52:44.000000 conan-2.2.1/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-03-20 17:52:44.000000 conan-2.2.1/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.381523 conan-2.2.1/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20506 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12679 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    32560 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     6168 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    13116 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    15205 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17829 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     7089 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     8089 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24648 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13805 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6184 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     8467 2024-03-20 17:52:44.000000 conan-2.2.1/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.381523 conan-2.2.1/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2151 2024-03-20 17:52:44.000000 conan-2.2.1/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      251 2024-03-20 17:52:44.000000 conan-2.2.1/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2024-03-20 17:52:44.000000 conan-2.2.1/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-20 17:52:44.000000 conan-2.2.1/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.381523 conan-2.2.1/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-03-20 17:52:44.000000 conan-2.2.1/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4474 2024-03-20 17:52:44.000000 conan-2.2.1/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.382523 conan-2.2.1/conans/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.383523 conan-2.2.1/conans/test/assets/
--rw-r--r--   0 root         (0) root         (0)      510 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1651 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/autotools.py
--rw-r--r--   0 root         (0) root         (0)     3753 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/cmake.py
--rw-r--r--   0 root         (0) root         (0)    17307 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/genconanfile.py
--rw-r--r--   0 root         (0) root         (0)     6352 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/pkg_cmake.py
--rw-r--r--   0 root         (0) root         (0)     6008 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/sources.py
--rw-r--r--   0 root         (0) root         (0)    11972 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/assets/visual_project_files.py
--rw-r--r--   0 root         (0) root         (0)    13204 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.384523 conan-2.2.1/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     2805 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/file_server.py
--rw-r--r--   0 root         (0) root         (0)     4155 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    37513 2024-03-20 17:52:44.000000 conan-2.2.1/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:52:51.385523 conan-2.2.1/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1396 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11974 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3729 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-03-20 17:52:44.000000 conan-2.2.1/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)       90 2024-03-20 17:52:44.000000 conan-2.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      101 2024-03-20 17:52:51.386523 conan-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5100 2024-03-20 17:52:44.000000 conan-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.571598 conan-2.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-03-25 15:15:44.000000 conan-2.2.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2024-03-25 15:15:44.000000 conan-2.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8618 2024-03-25 15:15:52.572598 conan-2.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6335 2024-03-25 15:15:44.000000 conan-2.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.534596 conan-2.2.2/conan/
+-rw-r--r--   0 root         (0) root         (0)      165 2024-03-25 15:15:44.000000 conan-2.2.2/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.535596 conan-2.2.2/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.537596 conan-2.2.2/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11757 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/command.py
+-rw-r--r--   0 root         (0) root         (0)     9255 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5465 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     7441 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    13285 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2024-03-25 15:15:44.000000 conan-2.2.2/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.538596 conan-2.2.2/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    11875 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.540596 conan-2.2.2/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5798 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)    21433 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)    13371 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     7511 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     6871 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      653 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.541596 conan-2.2.2/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.541596 conan-2.2.2/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)    14752 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.542596 conan-2.2.2/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.542596 conan-2.2.2/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2024-03-25 15:15:44.000000 conan-2.2.2/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-03-25 15:15:44.000000 conan-2.2.2/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.543596 conan-2.2.2/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.543596 conan-2.2.2/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19809 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/detect_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.545596 conan-2.2.2/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/local_recipes_index.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.545596 conan-2.2.2/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11189 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.546596 conan-2.2.2/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/cache/home_paths.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/internal_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-03-25 15:15:44.000000 conan-2.2.2/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.546596 conan-2.2.2/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.546596 conan-2.2.2/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.547597 conan-2.2.2/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11835 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.547597 conan-2.2.2/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    16208 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.548596 conan-2.2.2/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14472 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.548596 conan-2.2.2/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10886 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.549597 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14900 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    20156 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4746 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    16611 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.550597 conan-2.2.2/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45129 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13892 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.550597 conan-2.2.2/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26546 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.551597 conan-2.2.2/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    24002 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.551597 conan-2.2.2/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.552597 conan-2.2.2/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    14034 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)    27066 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/makedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.553597 conan-2.2.2/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    23416 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)     8113 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.553597 conan-2.2.2/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.553597 conan-2.2.2/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.554597 conan-2.2.2/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5093 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    23068 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.555597 conan-2.2.2/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19246 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    15003 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.555597 conan-2.2.2/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.556597 conan-2.2.2/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9897 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.556597 conan-2.2.2/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12771 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.556597 conan-2.2.2/conan/tools/scons/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/scons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/scons/sconsdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.556597 conan-2.2.2/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-03-25 15:15:44.000000 conan-2.2.2/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.534596 conan-2.2.2/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8618 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9622 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      469 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-03-25 15:15:52.000000 conan-2.2.2/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.557597 conan-2.2.2/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-03-25 15:15:44.000000 conan-2.2.2/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.559597 conan-2.2.2/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.559597 conan-2.2.2/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cache/editable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.560597 conan-2.2.2/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7808 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12332 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/cmd/uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.560597 conan-2.2.2/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)      638 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conanfile/implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.561597 conan-2.2.2/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     7414 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7899 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.561597 conan-2.2.2/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.562597 conan-2.2.2/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)    10315 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.563598 conan-2.2.2/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    15453 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    23117 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    21937 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    21344 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21840 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    17007 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14595 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.564598 conan-2.2.2/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6923 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/remote_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     5424 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     9571 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14934 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/rest_client_local_recipe_index.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.565598 conan-2.2.2/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2024-03-25 15:15:44.000000 conan-2.2.2/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2024-03-25 15:15:44.000000 conan-2.2.2/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-03-25 15:15:44.000000 conan-2.2.2/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-03-25 15:15:44.000000 conan-2.2.2/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-03-25 15:15:44.000000 conan-2.2.2/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.567598 conan-2.2.2/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20506 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12679 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    32560 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    13116 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    15205 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17829 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24648 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13805 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     8467 2024-03-25 15:15:44.000000 conan-2.2.2/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.567598 conan-2.2.2/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-03-25 15:15:44.000000 conan-2.2.2/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      251 2024-03-25 15:15:44.000000 conan-2.2.2/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2024-03-25 15:15:44.000000 conan-2.2.2/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-03-25 15:15:44.000000 conan-2.2.2/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.568598 conan-2.2.2/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-03-25 15:15:44.000000 conan-2.2.2/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-03-25 15:15:44.000000 conan-2.2.2/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.568598 conan-2.2.2/conans/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.569598 conan-2.2.2/conans/test/assets/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/cmake.py
+-rw-r--r--   0 root         (0) root         (0)    17307 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/genconanfile.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/pkg_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/sources.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/assets/visual_project_files.py
+-rw-r--r--   0 root         (0) root         (0)    13204 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.570598 conan-2.2.2/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/file_server.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    37513 2024-03-25 15:15:44.000000 conan-2.2.2/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:15:52.571598 conan-2.2.2/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-03-25 15:15:44.000000 conan-2.2.2/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)       90 2024-03-25 15:15:44.000000 conan-2.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      101 2024-03-25 15:15:52.572598 conan-2.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5100 2024-03-25 15:15:44.000000 conan-2.2.2/setup.py
```

### Comparing `conan-2.2.1/LICENSE.md` & `conan-2.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/PKG-INFO` & `conan-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.2.1
+Version: 2.2.2
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.2.1/README.md` & `conan-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/conan_api.py` & `conan-2.2.2/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/model.py` & `conan-2.2.2/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/output.py` & `conan-2.2.2/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/cache.py` & `conan-2.2.2/conan/api/subapi/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/command.py` & `conan-2.2.2/conan/api/subapi/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/config.py` & `conan-2.2.2/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/download.py` & `conan-2.2.2/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/export.py` & `conan-2.2.2/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/graph.py` & `conan-2.2.2/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/install.py` & `conan-2.2.2/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/list.py` & `conan-2.2.2/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/local.py` & `conan-2.2.2/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/lockfile.py` & `conan-2.2.2/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/new.py` & `conan-2.2.2/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/profiles.py` & `conan-2.2.2/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/remotes.py` & `conan-2.2.2/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/remove.py` & `conan-2.2.2/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/search.py` & `conan-2.2.2/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/api/subapi/upload.py` & `conan-2.2.2/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/args.py` & `conan-2.2.2/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/cli.py` & `conan-2.2.2/conan/cli/cli.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/command.py` & `conan-2.2.2/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/build.py` & `conan-2.2.2/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/cache.py` & `conan-2.2.2/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/config.py` & `conan-2.2.2/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/create.py` & `conan-2.2.2/conan/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/download.py` & `conan-2.2.2/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/editable.py` & `conan-2.2.2/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/export.py` & `conan-2.2.2/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/export_pkg.py` & `conan-2.2.2/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/graph.py` & `conan-2.2.2/conan/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/inspect.py` & `conan-2.2.2/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/install.py` & `conan-2.2.2/conan/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/list.py` & `conan-2.2.2/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/lock.py` & `conan-2.2.2/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/new.py` & `conan-2.2.2/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/profile.py` & `conan-2.2.2/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/remote.py` & `conan-2.2.2/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/remove.py` & `conan-2.2.2/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/search.py` & `conan-2.2.2/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/source.py` & `conan-2.2.2/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/test.py` & `conan-2.2.2/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/upload.py` & `conan-2.2.2/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/commands/version.py` & `conan-2.2.2/conan/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/graph/graph.py` & `conan-2.2.2/conan/cli/formatters/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.2.2/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.2.2/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/list/binary_html_table.py` & `conan-2.2.2/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/list/list.py` & `conan-2.2.2/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/formatters/list/search_table_html.py` & `conan-2.2.2/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/cli/printers/graph.py` & `conan-2.2.2/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/detect_api.py` & `conan-2.2.2/conan/internal/api/detect_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/autoools_exe.py` & `conan-2.2.2/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/autotools_lib.py` & `conan-2.2.2/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/basic.py` & `conan-2.2.2/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/bazel_exe.py` & `conan-2.2.2/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/bazel_lib.py` & `conan-2.2.2/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/cmake_exe.py` & `conan-2.2.2/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/cmake_lib.py` & `conan-2.2.2/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/local_recipes_index.py` & `conan-2.2.2/conan/internal/api/new/local_recipes_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/meson_exe.py` & `conan-2.2.2/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/meson_lib.py` & `conan-2.2.2/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/msbuild_exe.py` & `conan-2.2.2/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/api/new/msbuild_lib.py` & `conan-2.2.2/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/cache.py` & `conan-2.2.2/conan/internal/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/conan_reference_layout.py` & `conan-2.2.2/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/db/cache_database.py` & `conan-2.2.2/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/db/packages_table.py` & `conan-2.2.2/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/db/recipes_table.py` & `conan-2.2.2/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/db/table.py` & `conan-2.2.2/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/cache/home_paths.py` & `conan-2.2.2/conan/internal/cache/home_paths.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/conan_app.py` & `conan-2.2.2/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/deploy.py` & `conan-2.2.2/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/integrity_check.py` & `conan-2.2.2/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/internal_tools.py` & `conan-2.2.2/conan/internal/internal_tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/internal/upload_metadata.py` & `conan-2.2.2/conan/internal/upload_metadata.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/android/utils.py` & `conan-2.2.2/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/apple/__init__.py` & `conan-2.2.2/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/apple/apple.py` & `conan-2.2.2/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/apple/xcodebuild.py` & `conan-2.2.2/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/apple/xcodedeps.py` & `conan-2.2.2/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/apple/xcodetoolchain.py` & `conan-2.2.2/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/__init__.py` & `conan-2.2.2/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/cppstd.py` & `conan-2.2.2/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/cpu.py` & `conan-2.2.2/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/cross_building.py` & `conan-2.2.2/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/flags.py` & `conan-2.2.2/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/build/stdcpp_library.py` & `conan-2.2.2/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmake.py` & `conan-2.2.2/conan/tools/cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.2.2/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/layout.py` & `conan-2.2.2/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/presets.py` & `conan-2.2.2/conan/tools/cmake/presets.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/cmake/toolchain/blocks.py` & `conan-2.2.2/conan/tools/cmake/toolchain/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
         bin_dirs = ";".join(bin_dirs) if bin_dirs else None
         if bin_dirs:
             config_dict[build_type] = bin_dirs
 
         if not config_dict:
             return None
-        
+
         vs_debugger_path = ""
         for config, value in config_dict.items():
             vs_debugger_path += f"$<$<CONFIG:{config}>:{value}>"
         vs_debugger_path = f"PATH={vs_debugger_path};%PATH%"
         return {"vs_debugger_path": vs_debugger_path}
 
 
@@ -609,15 +609,17 @@
         string(APPEND CONAN_SHARED_LINKER_FLAGS{{suffix}} "{% for sharedlinkflag in sharedlinkflags %} {{ sharedlinkflag }}{% endfor %}")
         {% endif %}
         {% if exelinkflags %}
         string(APPEND CONAN_EXE_LINKER_FLAGS{{suffix}} "{% for exelinkflag in exelinkflags %} {{ exelinkflag }}{% endfor %}")
         {% endif %}
         {% if defines %}
         {% if config %}
-        add_compile_definitions($<$<CONFIG:{{config}}>:{% for define in defines %}" {{ define }}"{% endfor %}>)
+        {% for define in defines %}
+        add_compile_definitions($<$<CONFIG:{{config}}>:"{{ define }}">)
+        {% endfor %}
         {% else %}
         add_compile_definitions({% for define in defines %} "{{ define }}"{% endfor %})
         {% endif %}
         {% endif %}
         # Conan conf flags end
     """)
```

### Comparing `conan-2.2.1/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.2.2/conan/tools/cmake/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/env/environment.py` & `conan-2.2.2/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/env/virtualbuildenv.py` & `conan-2.2.2/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/env/virtualrunenv.py` & `conan-2.2.2/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/__init__.py` & `conan-2.2.2/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/conandata.py` & `conan-2.2.2/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/copy_pattern.py` & `conan-2.2.2/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/files.py` & `conan-2.2.2/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/packager.py` & `conan-2.2.2/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/patches.py` & `conan-2.2.2/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/files/symlinks/symlinks.py` & `conan-2.2.2/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/autotools.py` & `conan-2.2.2/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/autotoolsdeps.py` & `conan-2.2.2/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.2.2/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.2.2/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/gnudeps_flags.py` & `conan-2.2.2/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/makedeps.py` & `conan-2.2.2/conan/tools/gnu/makedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/pkgconfig.py` & `conan-2.2.2/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.2.2/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/google/bazel.py` & `conan-2.2.2/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/google/bazeldeps.py` & `conan-2.2.2/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/google/layout.py` & `conan-2.2.2/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/google/toolchain.py` & `conan-2.2.2/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/intel/intel_cc.py` & `conan-2.2.2/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/layout/__init__.py` & `conan-2.2.2/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/meson/helpers.py` & `conan-2.2.2/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/meson/meson.py` & `conan-2.2.2/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/meson/toolchain.py` & `conan-2.2.2/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/__init__.py` & `conan-2.2.2/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/layout.py` & `conan-2.2.2/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/msbuild.py` & `conan-2.2.2/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/msbuilddeps.py` & `conan-2.2.2/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/nmakedeps.py` & `conan-2.2.2/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.2.2/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/subsystems.py` & `conan-2.2.2/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/toolchain.py` & `conan-2.2.2/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/microsoft/visual.py` & `conan-2.2.2/conan/tools/microsoft/visual.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/premake/premake.py` & `conan-2.2.2/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/premake/premakedeps.py` & `conan-2.2.2/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/qbs/qbs.py` & `conan-2.2.2/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/qbs/qbsprofile.py` & `conan-2.2.2/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/scm/git.py` & `conan-2.2.2/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/scons/sconsdeps.py` & `conan-2.2.2/conan/tools/scons/sconsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan/tools/system/package_manager.py` & `conan-2.2.2/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conan.egg-info/PKG-INFO` & `conan-2.2.2/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.2.1
+Version: 2.2.2
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.2.1/conan.egg-info/SOURCES.txt` & `conan-2.2.2/conan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/cache/cache.py` & `conan-2.2.2/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/cache/editable.py` & `conan-2.2.2/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/cmd/export.py` & `conan-2.2.2/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/cmd/uploader.py` & `conan-2.2.2/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conanfile/build.py` & `conan-2.2.2/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conanfile/configure.py` & `conan-2.2.2/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conanfile/implementations.py` & `conan-2.2.2/conans/client/conanfile/implementations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conanfile/package.py` & `conan-2.2.2/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conf/__init__.py` & `conan-2.2.2/conans/client/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conf/config_installer.py` & `conan-2.2.2/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conf/detect.py` & `conan-2.2.2/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conf/detect_vs.py` & `conan-2.2.2/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/conf/required_version.py` & `conan-2.2.2/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/downloaders/caching_file_downloader.py` & `conan-2.2.2/conans/client/downloaders/caching_file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/downloaders/download_cache.py` & `conan-2.2.2/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/downloaders/file_downloader.py` & `conan-2.2.2/conans/client/downloaders/file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/generators/__init__.py` & `conan-2.2.2/conans/client/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/build_mode.py` & `conan-2.2.2/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/compatibility.py` & `conan-2.2.2/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/compute_pid.py` & `conan-2.2.2/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/graph.py` & `conan-2.2.2/conans/client/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/graph_binaries.py` & `conan-2.2.2/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/graph_builder.py` & `conan-2.2.2/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/graph_error.py` & `conan-2.2.2/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/install_graph.py` & `conan-2.2.2/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/profile_node_definer.py` & `conan-2.2.2/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/provides.py` & `conan-2.2.2/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/proxy.py` & `conan-2.2.2/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/python_requires.py` & `conan-2.2.2/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/graph/range_resolver.py` & `conan-2.2.2/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/hook_manager.py` & `conan-2.2.2/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/installer.py` & `conan-2.2.2/conans/client/installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/loader.py` & `conan-2.2.2/conans/client/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,16 @@
     """ From a given path, obtain the in memory python import module
     """
 
     if not os.path.exists(conan_file_path):
         raise NotFoundException("%s not found!" % conan_file_path)
 
     def new_print(*args, **kwargs):  # Make sure that all user python files print() goes to stderr
-        print(*args, **kwargs, file=sys.stderr)
+        kwargs.setdefault("file", sys.stderr)
+        print(*args, **kwargs)
 
     module_id = str(uuid.uuid1())
     current_dir = os.path.dirname(conan_file_path)
     sys.path.insert(0, current_dir)
     try:
         old_modules = list(sys.modules.keys())
         with chdir(current_dir):
```

### Comparing `conan-2.2.1/conans/client/loader_txt.py` & `conan-2.2.2/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/migrations.py` & `conan-2.2.2/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/pkg_sign.py` & `conan-2.2.2/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/profile_loader.py` & `conan-2.2.2/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/remote_manager.py` & `conan-2.2.2/conans/client/remote_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/__init__.py` & `conan-2.2.2/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/auth_manager.py` & `conan-2.2.2/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/client_routes.py` & `conan-2.2.2/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/conan_requester.py` & `conan-2.2.2/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/file_uploader.py` & `conan-2.2.2/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/remote_credentials.py` & `conan-2.2.2/conans/client/rest/remote_credentials.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/rest_client.py` & `conan-2.2.2/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/rest_client_common.py` & `conan-2.2.2/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest/rest_client_v2.py` & `conan-2.2.2/conans/client/rest/rest_client_v2.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/rest_client_local_recipe_index.py` & `conan-2.2.2/conans/client/rest_client_local_recipe_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/source.py` & `conan-2.2.2/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/store/localdb.py` & `conan-2.2.2/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/subsystems.py` & `conan-2.2.2/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/client/userio.py` & `conan-2.2.2/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/conan_server.py` & `conan-2.2.2/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/errors.py` & `conan-2.2.2/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/migrations.py` & `conan-2.2.2/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/build_info.py` & `conan-2.2.2/conans/model/build_info.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/conan_file.py` & `conan-2.2.2/conans/model/conan_file.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/conanfile_interface.py` & `conan-2.2.2/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/conf.py` & `conan-2.2.2/conans/model/conf.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/dependencies.py` & `conan-2.2.2/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/graph_lock.py` & `conan-2.2.2/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/info.py` & `conan-2.2.2/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/layout.py` & `conan-2.2.2/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/manifest.py` & `conan-2.2.2/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/options.py` & `conan-2.2.2/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/package_ref.py` & `conan-2.2.2/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/pkg_type.py` & `conan-2.2.2/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/profile.py` & `conan-2.2.2/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/recipe_ref.py` & `conan-2.2.2/conans/model/recipe_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/requires.py` & `conan-2.2.2/conans/model/requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/rest_routes.py` & `conan-2.2.2/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/settings.py` & `conan-2.2.2/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/version.py` & `conan-2.2.2/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/model/version_range.py` & `conan-2.2.2/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/paths/__init__.py` & `conan-2.2.2/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/search/query_parse.py` & `conan-2.2.2/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/search/search.py` & `conan-2.2.2/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/autotools.py` & `conan-2.2.2/conans/test/assets/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/cmake.py` & `conan-2.2.2/conans/test/assets/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/genconanfile.py` & `conan-2.2.2/conans/test/assets/genconanfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/pkg_cmake.py` & `conan-2.2.2/conans/test/assets/pkg_cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/sources.py` & `conan-2.2.2/conans/test/assets/sources.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/assets/visual_project_files.py` & `conan-2.2.2/conans/test/assets/visual_project_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/conftest.py` & `conan-2.2.2/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/artifactory.py` & `conan-2.2.2/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/file_server.py` & `conan-2.2.2/conans/test/utils/file_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/mocks.py` & `conan-2.2.2/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/profiles.py` & `conan-2.2.2/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/scm.py` & `conan-2.2.2/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/server_launcher.py` & `conan-2.2.2/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/test_files.py` & `conan-2.2.2/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/test/utils/tools.py` & `conan-2.2.2/conans/test/utils/tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/config_parser.py` & `conan-2.2.2/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/dates.py` & `conan-2.2.2/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/encrypt.py` & `conan-2.2.2/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/env.py` & `conan-2.2.2/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/files.py` & `conan-2.2.2/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/locks.py` & `conan-2.2.2/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/runners.py` & `conan-2.2.2/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/sha.py` & `conan-2.2.2/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/conans/util/windows.py` & `conan-2.2.2/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.1/setup.py` & `conan-2.2.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/gvsbuild-2024.3.1.tar.gz` & `tmp/gvsbuild-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvsbuild-2024.3.1.tar", max compression
+gzip compressed data, was "gvsbuild-2024.4.0.tar", max compression
```

## Comparing `gvsbuild-2024.3.1.tar` & `gvsbuild-2024.4.0.tar`

### file list

```diff
@@ -1,929 +1,932 @@
--rw-r--r--   0        0        0     2185 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/AUTHORS.md
--rw-r--r--   0        0        0    18433 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/COPYING
--rw-r--r--   0        0        0       37 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/__init__.py
--rw-r--r--   0        0        0    16410 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/build.py
--rw-r--r--   0        0        0     7322 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/deps.py
--rw-r--r--   0        0        0     2121 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/groups.py
--rw-r--r--   0        0        0      244 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/info.py
--rw-r--r--   0        0        0     5581 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/gvsbuild/list.py
--rw-r--r--   0        0        0     1977 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/main.py
--rw-r--r--   0        0        0     2609 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/outdated.py
--rw-r--r--   0        0        0      862 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/adwaita-icon-theme/001-fix-relative-cursor-path.patch
--rw-r--r--   0        0        0      634 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
--rw-r--r--   0        0        0      213 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/check_utils.c
--rw-r--r--   0        0        0      537 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/check_utils.h
--rw-r--r--   0        0        0    18437 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/COPYING
--rw-r--r--   0        0        0     9831 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/meson.build
--rw-r--r--   0        0        0      175 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_atk.c
--rw-r--r--   0        0        0      167 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_cairo.c
--rw-r--r--   0        0        0      224 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_freetype2.c
--rw-r--r--   0        0        0      205 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
--rw-r--r--   0        0        0      170 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_glib.c
--rw-r--r--   0        0        0      183 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_jasper.c
--rw-r--r--   0        0        0      204 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_json_glib.c
--rw-r--r--   0        0        0      201 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libarchive.c
--rw-r--r--   0        0        0      191 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libcurl.c
--rw-r--r--   0        0        0      125 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libffi.c
--rw-r--r--   0        0        0      193 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
--rw-r--r--   0        0        0      194 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libjpeg.c
--rw-r--r--   0        0        0      188 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libpng.c
--rw-r--r--   0        0        0      187 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libtiff-4.c
--rw-r--r--   0        0        0      179 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libxml2.c
--rw-r--r--   0        0        0      187 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_libyuv.c
--rw-r--r--   0        0        0      173 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_pango.c
--rw-r--r--   0        0        0      180 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_wing.c
--rw-r--r--   0        0        0      127 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/check-libs/test_zlib.c
--rw-r--r--   0        0        0     9047 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
--rw-r--r--   0        0        0    29220 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
--rw-r--r--   0        0        0    50071 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19138 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4749 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt
--rw-r--r--   0        0        0     8818 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0    13484 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
--rw-r--r--   0        0        0     5987 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
--rw-r--r--   0        0        0      464 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
--rw-r--r--   0        0        0     9685 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
--rw-r--r--   0        0        0     8719 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9047 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-03-28 22:44:15.409143 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27777 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
--rw-r--r--   0        0        0    50071 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19138 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4749 2024-03-28 22:44:15.393521 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt
--rw-r--r--   0        0        0     8818 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8719 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9126 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9180 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9636 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9164 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9112 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
--rw-r--r--   0        0        0    10744 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27909 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
--rw-r--r--   0        0        0    50150 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19138 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4749 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     8897 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8798 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8976 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8901 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8807 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8817 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8794 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8801 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8888 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
--rw-r--r--   0        0        0      316 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
--rw-r--r--   0        0        0      339 2024-03-28 22:44:15.411228 gvsbuild-2024.3.1/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
--rw-r--r--   0        0        0     3533 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
--rw-r--r--   0        0        0    48250 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19171 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4783 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt
--rw-r--r--   0        0        0    13862 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
--rw-r--r--   0        0        0    48250 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19171 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4783 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt
--rw-r--r--   0        0        0    13862 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
--rw-r--r--   0        0        0    10284 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8997 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9318 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
--rw-r--r--   0        0        0    14369 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12930 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16426 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
--rw-r--r--   0        0        0    12161 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
--rw-r--r--   0        0        0    48329 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19171 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4783 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt
--rw-r--r--   0        0        0    13941 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0   244356 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glcorearb.h
--rw-r--r--   0        0        0   810011 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glext.h
--rw-r--r--   0        0        0    48113 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glxext.h
--rw-r--r--   0        0        0    44095 2024-03-28 22:44:15.426903 gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/wglext.h
--rw-r--r--   0        0        0     1121 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
--rw-r--r--   0        0        0     1060 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
--rw-r--r--   0        0        0      740 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
--rw-r--r--   0        0        0     1135 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
--rw-r--r--   0        0        0     1045 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/include/md5global.h
--rw-r--r--   0        0        0      312 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
--rw-r--r--   0        0        0      418 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/enchant/src/config.h
--rw-r--r--   0        0        0      660 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/enchant/src/libenchant.rc
--rw-r--r--   0        0        0    17426 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/enchant/src/makefile.mak
--rw-r--r--   0        0        0      754 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
--rw-r--r--   0        0        0     2152 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/ffmpeg/build/build.sh
--rw-r--r--   0        0        0      787 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
--rw-r--r--   0        0        0     3296 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch
--rw-r--r--   0        0        0    33686 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/gettext-tools-c99.patch
--rw-r--r--   0        0        0      367 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
--rw-r--r--   0        0        0     9543 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/libtextstyle-c99.patch
--rw-r--r--   0        0        0     3065 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     7623 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33617 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0     2128 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43681 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27515 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4377 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32044 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
--rw-r--r--   0        0        0    37498 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
--rw-r--r--   0        0        0     4322 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63279 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63715 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
--rw-r--r--   0        0        0    44998 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0     3250 2024-03-28 22:44:15.442527 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    35655 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
--rw-r--r--   0        0        0    81450 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    62421 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38906 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    20126 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
--rw-r--r--   0        0        0    19299 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
--rw-r--r--   0        0        0     3088 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
--rw-r--r--   0        0        0     2708 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
--rw-r--r--   0        0        0     7648 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
--rw-r--r--   0        0        0     3065 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     2093 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
--rw-r--r--   0        0        0    22716 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
--rw-r--r--   0        0        0    30933 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
--rw-r--r--   0        0        0     7623 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33701 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0    25904 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
--rw-r--r--   0        0        0     2128 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43508 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27538 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4658 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4377 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32067 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
--rw-r--r--   0        0        0     1209 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
--rw-r--r--   0        0        0    23409 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
--rw-r--r--   0        0        0    37554 2024-03-28 22:44:15.458155 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
--rw-r--r--   0        0        0    61302 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
--rw-r--r--   0        0        0     4298 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63335 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63743 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
--rw-r--r--   0        0        0    24900 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
--rw-r--r--   0        0        0    32949 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
--rw-r--r--   0        0        0    44998 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0    29890 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
--rw-r--r--   0        0        0     3250 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    24835 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
--rw-r--r--   0        0        0    35681 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
--rw-r--r--   0        0        0     7748 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
--rw-r--r--   0        0        0    42529 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
--rw-r--r--   0        0        0     4287 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
--rw-r--r--   0        0        0     1625 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
--rw-r--r--   0        0        0    81730 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    24592 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
--rw-r--r--   0        0        0    62584 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38904 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    27214 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
--rw-r--r--   0        0        0     1287 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
--rw-r--r--   0        0        0    91289 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
--rw-r--r--   0        0        0     4873 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
--rw-r--r--   0        0        0    23344 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
--rw-r--r--   0        0        0    46391 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
--rw-r--r--   0        0        0     1629 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
--rw-r--r--   0        0        0     3065 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
--rw-r--r--   0        0        0     7648 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
--rw-r--r--   0        0        0    33726 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
--rw-r--r--   0        0        0    17539 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
--rw-r--r--   0        0        0    26333 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
--rw-r--r--   0        0        0    43508 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
--rw-r--r--   0        0        0     4402 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
--rw-r--r--   0        0        0    32092 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
--rw-r--r--   0        0        0    37579 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
--rw-r--r--   0        0        0     4333 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
--rw-r--r--   0        0        0    63360 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
--rw-r--r--   0        0        0    63768 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
--rw-r--r--   0        0        0    45023 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
--rw-r--r--   0        0        0     3275 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
--rw-r--r--   0        0        0    13023 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
--rw-r--r--   0        0        0    35677 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
--rw-r--r--   0        0        0     7748 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
--rw-r--r--   0        0        0    42529 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
--rw-r--r--   0        0        0     4287 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
--rw-r--r--   0        0        0    81764 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
--rw-r--r--   0        0        0    24256 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
--rw-r--r--   0        0        0     2201 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
--rw-r--r--   0        0        0     2239 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
--rw-r--r--   0        0        0    62609 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
--rw-r--r--   0        0        0    38929 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
--rw-r--r--   0        0        0    27563 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
--rw-r--r--   0        0        0     4432 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
--rw-r--r--   0        0        0    23446 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
--rw-r--r--   0        0        0     3065 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
--rw-r--r--   0        0        0     7643 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
--rw-r--r--   0        0        0    33637 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
--rw-r--r--   0        0        0     4938 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
--rw-r--r--   0        0        0     5545 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
--rw-r--r--   0        0        0     9729 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
--rw-r--r--   0        0        0     2028 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
--rw-r--r--   0        0        0     2257 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
--rw-r--r--   0        0        0    10124 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
--rw-r--r--   0        0        0     6212 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
--rw-r--r--   0        0        0    16052 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
--rw-r--r--   0        0        0     2765 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
--rw-r--r--   0        0        0     6279 2024-03-28 22:44:15.473778 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
--rw-r--r--   0        0        0    43677 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
--rw-r--r--   0        0        0     4658 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4396 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
--rw-r--r--   0        0        0    37518 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
--rw-r--r--   0        0        0     4873 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
--rw-r--r--   0        0        0     4326 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
--rw-r--r--   0        0        0    23157 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
--rw-r--r--   0        0        0    63299 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
--rw-r--r--   0        0        0    63735 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
--rw-r--r--   0        0        0    46251 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
--rw-r--r--   0        0        0    45018 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
--rw-r--r--   0        0        0    29922 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
--rw-r--r--   0        0        0     3272 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
--rw-r--r--   0        0        0     1649 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
--rw-r--r--   0        0        0     4432 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
--rw-r--r--   0        0        0    35661 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
--rw-r--r--   0        0        0    81477 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
--rw-r--r--   0        0        0    62439 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
--rw-r--r--   0        0        0    54409 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75068 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97908 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-03-28 22:44:15.489402 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75124 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75149 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54408 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75065 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97907 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75121 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75146 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54410 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97906 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    21997 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49879 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54407 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74958 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97900 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75014 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75039 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-03-28 22:44:15.505027 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54406 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97945 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    22956 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
--rw-r--r--   0        0        0     6490 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/config-msvc.mak
--rw-r--r--   0        0        0    16869 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
--rwxr-xr-x   0        0        0      846 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/create-lists.bat
--rw-r--r--   0        0        0     5708 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
--rw-r--r--   0        0        0      772 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak
--rw-r--r--   0        0        0     4576 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
--rw-r--r--   0        0        0     8982 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
--rw-r--r--   0        0        0     2466 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libgettextlib.def
--rw-r--r--   0        0        0     2852 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def
--rw-r--r--   0        0        0     3788 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
--rw-r--r--   0        0        0     2635 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libtextstyle.def
--rw-r--r--   0        0        0     1051 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/Makefile.vc
--rw-r--r--   0        0        0     1582 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
--rw-r--r--   0        0        0      823 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib/002-python-312-distutils-to-packaging.patch
--rw-r--r--   0        0        0       30 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
--rw-r--r--   0        0        0       27 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
--rw-r--r--   0        0        0     1123 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
--rw-r--r--   0        0        0      394 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/glib-py-wrapper/meson.build
--rw-r--r--   0        0        0      611 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch
--rw-r--r--   0        0        0     1468 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
--rw-r--r--   0        0        0      759 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
--rw-r--r--   0        0        0     2083 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
--rw-r--r--   0        0        0     1668 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch
--rw-r--r--   0        0        0     1958 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
--rw-r--r--   0        0        0     1186 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
--rw-r--r--   0        0        0     1920 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
--rw-r--r--   0        0        0     1956 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
--rw-r--r--   0        0        0     2185 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
--rw-r--r--   0        0        0     2185 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
--rw-r--r--   0        0        0    10679 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
--rw-r--r--   0        0        0     1080 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
--rw-r--r--   0        0        0    11397 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
--rw-r--r--   0        0        0     3760 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
--rw-r--r--   0        0        0    13364 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
--rw-r--r--   0        0        0     4222 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
--rw-r--r--   0        0        0     6519 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
--rw-r--r--   0        0        0     3640 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
--rw-r--r--   0        0        0    12279 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
--rw-r--r--   0        0        0     4640 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
--rw-r--r--   0        0        0     1962 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
--rw-r--r--   0        0        0    23804 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
--rw-r--r--   0        0        0     7938 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
--rw-r--r--   0        0        0     9247 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
--rw-r--r--   0        0        0      706 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
--rw-r--r--   0        0        0     2185 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
--rw-r--r--   0        0        0    26897 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
--rw-r--r--   0        0        0    26470 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
--rw-r--r--   0        0        0     9451 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
--rw-r--r--   0        0        0     1756 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
--rw-r--r--   0        0        0     3586 2024-03-28 22:44:15.520656 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
--rw-r--r--   0        0        0      803 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-accel.patch
--rw-r--r--   0        0        0      599 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-bgimg.patch
--rw-r--r--   0        0        0      682 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch
--rw-r--r--   0        0        0     2154 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
--rw-r--r--   0        0        0     1104 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk2/mod.md
--rw-r--r--   0        0        0     6104 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
--rw-r--r--   0        0        0    11322 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
--rw-r--r--   0        0        0     1630 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
--rw-r--r--   0        0        0      102 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/hello-world/hello-world.c
--rw-r--r--   0        0        0       66 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/hello-world/meson.build
--rw-r--r--   0        0        0      359 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/icu/pc-files/icu-uc.pc
--rw-r--r--   0        0        0      360 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
--rw-r--r--   0        0        0    28020 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
--rw-r--r--   0        0        0      652 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libcroco/mod.md
--rw-r--r--   0        0        0     3749 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
--rw-r--r--   0        0        0     4827 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/fficonfig.h.meson
--rw-r--r--   0        0        0      475 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/include/meson.build
--rw-r--r--   0        0        0      248 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
--rw-r--r--   0        0        0    13940 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/meson.build
--rw-r--r--   0        0        0     1154 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/meson_options.txt
--rw-r--r--   0        0        0     3334 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libffi/src/meson.build
--rw-r--r--   0        0        0      936 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
--rw-r--r--   0        0        0     1243 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
--rw-r--r--   0        0        0     9777 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
--rw-r--r--   0        0        0       44 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libpng/mod.md
--rw-r--r--   0        0        0      318 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libpng/pc-files/libpng.pc
--rw-r--r--   0        0        0      318 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libpng/pc-files/libpng16.pc
--rw-r--r--   0        0        0     2998 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
--rw-r--r--   0        0        0     2998 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
--rw-r--r--   0        0        0     9178 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
--rw-r--r--   0        0        0      937 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
--rw-r--r--   0        0        0     4286 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
--rw-r--r--   0        0        0      572 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    17549 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     3085 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     2998 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
--rw-r--r--   0        0        0     8574 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
--rw-r--r--   0        0        0     1026 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
--rw-r--r--   0        0        0      931 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
--rw-r--r--   0        0        0     2133 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
--rw-r--r--   0        0        0     6578 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
--rw-r--r--   0        0        0     2326 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
--rw-r--r--   0        0        0     8979 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
--rw-r--r--   0        0        0      925 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
--rw-r--r--   0        0        0    14576 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
--rw-r--r--   0        0        0     3427 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
--rw-r--r--   0        0        0      866 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
--rw-r--r--   0        0        0     5490 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/config.h
--rw-r--r--   0        0        0     8059 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj
--rw-r--r--   0        0        0      834 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
--rw-r--r--   0        0        0     3769 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/property.props
--rw-r--r--   0        0        0    40095 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/config.h
--rw-r--r--   0        0        0     8059 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj
--rw-r--r--   0        0        0      834 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
--rw-r--r--   0        0        0     3767 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/property.props
--rw-r--r--   0        0        0    40095 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/config.h
--rw-r--r--   0        0        0     8138 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj
--rw-r--r--   0        0        0      834 2024-03-28 22:44:15.536276 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
--rw-r--r--   0        0        0     3899 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/property.props
--rw-r--r--   0        0        0    40174 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     1079 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libssh/mod.md
--rw-r--r--   0        0        0      809 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
--rw-r--r--   0        0        0     2586 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
--rw-r--r--   0        0        0     1251 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
--rw-r--r--   0        0        0     1025 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libxml2/include/libxml/meson.build
--rw-r--r--   0        0        0     1089 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libxml2/LICENSE.build
--rw-r--r--   0        0        0     7284 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libxml2/meson.build
--rw-r--r--   0        0        0      323 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
--rw-r--r--   0        0        0      943 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libyuv/001-win-build.patch
--rw-r--r--   0        0        0      392 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/libyuv/pc-files/libyuv.pc
--rw-r--r--   0        0        0      352 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/luajit/pc-files/luajit.pc
--rw-r--r--   0        0        0      971 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/luajit/set-paths.patch
--rw-r--r--   0        0        0      319 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/pc-files/liblz4.pc
--rw-r--r--   0        0        0     8964 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
--rw-r--r--   0        0        0     8964 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
--rw-r--r--   0        0        0     8966 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9317 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9317 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10138 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9145 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9206 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9309 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
--rw-r--r--   0        0        0     8964 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
--rw-r--r--   0        0        0     9976 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
--rw-r--r--   0        0        0       93 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/mod.md
--rw-r--r--   0        0        0      733 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
--rw-r--r--   0        0        0     2184 2024-03-28 22:44:15.551902 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch
--rw-r--r--   0        0        0  1290625 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/certdata.txt
--rw-r--r--   0        0        0    19616 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
--rw-r--r--   0        0        0      412 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/mod.md
--rw-r--r--   0        0        0      275 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
--rw-r--r--   0        0        0      285 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/pc-files/libssl.pc
--rw-r--r--   0        0        0      236 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/pc-files/openssl.pc
--rw-r--r--   0        0        0      383 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/opus/pc-files/opus.pc
--rw-r--r--   0        0        0     1369 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pango/001-fix-double-free-crash.patch
--rw-r--r--   0        0        0     1089 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pcre2/LICENSE.build
--rw-r--r--   0        0        0     7523 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pcre2/meson.build
--rw-r--r--   0        0        0      473 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pcre2/meson_options.txt
--rw-r--r--   0        0        0     1241 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
--rw-r--r--   0        0        0     1036 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
--rw-r--r--   0        0        0     2647 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
--rw-r--r--   0        0        0      319 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
--rw-r--r--   0        0        0     1912 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
--rw-r--r--   0        0        0      633 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/stack.props
--rw-r--r--   0        0        0     1565 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/win-iconv/COPYING
--rw-r--r--   0        0        0       92 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/win-iconv/mod.md
--rw-r--r--   0        0        0      671 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/x264/build/build.sh
--rw-r--r--   0        0        0     1385 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
--rw-r--r--   0        0        0      343 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/patches/zlib/pc-files/zlib.pc
--rw-r--r--   0        0        0     4302 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/__init__.py
--rw-r--r--   0        0        0     2101 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/adwaita_icon_theme.py
--rw-r--r--   0        0        0     1808 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/atk.py
--rw-r--r--   0        0        0     1774 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/boringssl.py
--rw-r--r--   0        0        0     1563 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/cairo.py
--rw-r--r--   0        0        0     1509 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/cairomm.py
--rw-r--r--   0        0        0     1912 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/check_libs.py
--rw-r--r--   0        0        0     1620 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/clutter.py
--rw-r--r--   0        0        0     1758 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/cogl.py
--rw-r--r--   0        0        0     2872 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/cyrus_sasl.py
--rw-r--r--   0        0        0     2844 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/dev_shell.py
--rw-r--r--   0        0        0     1648 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/emeus.py
--rw-r--r--   0        0        0     2807 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/enchant.py
--rw-r--r--   0        0        0     1572 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/expat.py
--rw-r--r--   0        0        0     3388 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/ffmpeg.py
--rw-r--r--   0        0        0     1582 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/fontconfig.py
--rw-r--r--   0        0        0     1725 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/freerdp.py
--rw-r--r--   0        0        0     1638 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/freetype.py
--rw-r--r--   0        0        0     2093 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/fribidi.py
--rw-r--r--   0        0        0     2204 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gdk_pixbuf.py
--rw-r--r--   0        0        0     4032 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gettext.py
--rw-r--r--   0        0        0     3402 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/glib.py
--rw-r--r--   0        0        0     1704 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/glibmm.py
--rw-r--r--   0        0        0     2638 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gobject_introspection.py
--rw-r--r--   0        0        0     1312 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gperf.py
--rw-r--r--   0        0        0     1752 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/graphene.py
--rw-r--r--   0        0        0     1813 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gsettings_desktop_schemas.py
--rw-r--r--   0        0        0     8797 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gstreamer.py
--rw-r--r--   0        0        0     5803 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gtk.py
--rw-r--r--   0        0        0     1806 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gtkmm.py
--rw-r--r--   0        0        0     2743 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/gtksourceview.py
--rw-r--r--   0        0        0     1672 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/harfbuzz.py
--rw-r--r--   0        0        0     1184 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/hello_world.py
--rw-r--r--   0        0        0     1382 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/hicolor_icon_theme.py
--rw-r--r--   0        0        0     2276 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/icu.py
--rw-r--r--   0        0        0     1832 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/json_glib.py
--rw-r--r--   0        0        0     1392 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/jsonc.py
--rw-r--r--   0        0        0     1624 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/leveldb.py
--rw-r--r--   0        0        0     1417 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/lgi.py
--rw-r--r--   0        0        0     2063 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libadwaita.py
--rw-r--r--   0        0        0     2075 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libarchive.py
--rw-r--r--   0        0        0     1781 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libcbor.py
--rw-r--r--   0        0        0     1496 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libcroco.py
--rw-r--r--   0        0        0     1903 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libcurl.py
--rw-r--r--   0        0        0     1447 2024-03-28 22:44:15.567527 gvsbuild-2024.3.1/gvsbuild/projects/libepoxy.py
--rw-r--r--   0        0        0     1341 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libffi.py
--rw-r--r--   0        0        0     2597 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libfido2.py
--rw-r--r--   0        0        0     1989 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libgxps.py
--rw-r--r--   0        0        0     1741 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libjpeg_turbo.py
--rw-r--r--   0        0        0     2331 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libmicrohttpd.py
--rw-r--r--   0        0        0     1704 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libpng.py
--rw-r--r--   0        0        0     1595 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libpsl.py
--rw-r--r--   0        0        0     2405 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/librsvg.py
--rw-r--r--   0        0        0     1737 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libsigcplusplus.py
--rw-r--r--   0        0        0     3368 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libsoup.py
--rw-r--r--   0        0        0     2181 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libssh.py
--rw-r--r--   0        0        0     1586 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libtiff.py
--rw-r--r--   0        0        0     1514 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libuv.py
--rw-r--r--   0        0        0     1511 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libvorbis.py
--rw-r--r--   0        0        0     3265 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libvpx.py
--rw-r--r--   0        0        0     1574 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libxml2.py
--rw-r--r--   0        0        0     1576 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libyuv.py
--rw-r--r--   0        0        0     1411 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/libzip.py
--rw-r--r--   0        0        0     1426 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/lmdb.py
--rw-r--r--   0        0        0     1761 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/luajit.py
--rw-r--r--   0        0        0     1778 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/lz4.py
--rw-r--r--   0        0        0     2279 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/mit_kerberos.py
--rw-r--r--   0        0        0     1587 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/nghttp2.py
--rw-r--r--   0        0        0     1477 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/ogg.py
--rw-r--r--   0        0        0     1521 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/openh264.py
--rw-r--r--   0        0        0     3381 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/openssl.py
--rw-r--r--   0        0        0     2056 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/opus.py
--rw-r--r--   0        0        0     1912 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pango.py
--rw-r--r--   0        0        0     1768 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pangomm.py
--rw-r--r--   0        0        0      712 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pcre2.py
--rw-r--r--   0        0        0     1672 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pixman.py
--rw-r--r--   0        0        0     1692 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pkgconf.py
--rw-r--r--   0        0        0     2711 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/protobuf.py
--rw-r--r--   0        0        0     2102 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pycairo.py
--rw-r--r--   0        0        0     2591 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/pygobject.py
--rw-r--r--   0        0        0     1618 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/sqlite.py
--rw-r--r--   0        0        0     1607 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/win_iconv.py
--rw-r--r--   0        0        0     1470 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/wing.py
--rw-r--r--   0        0        0     2341 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/x264.py
--rw-r--r--   0        0        0     2444 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/projects/zlib.py
--rw-r--r--   0        0        0     7545 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/tools.py
--rw-r--r--   0        0        0       30 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/__init__.py
--rw-r--r--   0        0        0     8512 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/base_builders.py
--rw-r--r--   0        0        0    15193 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/base_expanders.py
--rw-r--r--   0        0        0     1339 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/base_group.py
--rw-r--r--   0        0        0    20353 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/base_project.py
--rw-r--r--   0        0        0     2749 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/base_tool.py
--rw-r--r--   0        0        0    38283 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/builder.py
--rw-r--r--   0        0        0     9899 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/simple_ui.py
--rw-r--r--   0        0        0     3846 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/gvsbuild/utils/utils.py
--rw-r--r--   0        0        0     1653 2024-03-28 22:44:15.583154 gvsbuild-2024.3.1/pyproject.toml
--rw-r--r--   0        0        0    12300 2024-03-28 22:44:15.377891 gvsbuild-2024.3.1/README.md
--rw-r--r--   0        0        0    13026 1970-01-01 00:00:00.000000 gvsbuild-2024.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/AUTHORS.md
+-rw-r--r--   0        0        0    18433 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/COPYING
+-rw-r--r--   0        0        0       37 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/__init__.py
+-rw-r--r--   0        0        0    16410 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/build.py
+-rw-r--r--   0        0        0     7322 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/deps.py
+-rw-r--r--   0        0        0     2121 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/groups.py
+-rw-r--r--   0        0        0      244 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/info.py
+-rw-r--r--   0        0        0     5581 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/list.py
+-rw-r--r--   0        0        0     1977 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/main.py
+-rw-r--r--   0        0        0     2609 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/outdated.py
+-rw-r--r--   0        0        0      634 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
+-rw-r--r--   0        0        0      213 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.c
+-rw-r--r--   0        0        0      537 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.h
+-rw-r--r--   0        0        0    18437 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/COPYING
+-rw-r--r--   0        0        0     9831 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/meson.build
+-rw-r--r--   0        0        0      175 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_atk.c
+-rw-r--r--   0        0        0      167 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_cairo.c
+-rw-r--r--   0        0        0      224 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_freetype2.c
+-rw-r--r--   0        0        0      205 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
+-rw-r--r--   0        0        0      170 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_glib.c
+-rw-r--r--   0        0        0      183 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_jasper.c
+-rw-r--r--   0        0        0      204 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_json_glib.c
+-rw-r--r--   0        0        0      201 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libarchive.c
+-rw-r--r--   0        0        0      191 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libcurl.c
+-rw-r--r--   0        0        0      125 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libffi.c
+-rw-r--r--   0        0        0      193 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
+-rw-r--r--   0        0        0      194 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libjpeg.c
+-rw-r--r--   0        0        0      188 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libpng.c
+-rw-r--r--   0        0        0      187 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libtiff-4.c
+-rw-r--r--   0        0        0      179 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libxml2.c
+-rw-r--r--   0        0        0      187 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_libyuv.c
+-rw-r--r--   0        0        0      173 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_pango.c
+-rw-r--r--   0        0        0      180 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_wing.c
+-rw-r--r--   0        0        0      127 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/check-libs/test_zlib.c
+-rw-r--r--   0        0        0     9047 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    29220 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0    13484 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
+-rw-r--r--   0        0        0     5987 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
+-rw-r--r--   0        0        0      464 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0     9685 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
+-rw-r--r--   0        0        0     8719 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9047 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27777 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.247884 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8719 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-04-04 01:48:14.263509 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9126 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9180 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9636 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9164 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9112 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
+-rw-r--r--   0        0        0    10744 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27909 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
+-rw-r--r--   0        0        0    50150 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8798 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8976 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8901 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8807 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8817 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8794 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8801 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8888 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
+-rw-r--r--   0        0        0      316 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
+-rw-r--r--   0        0        0      339 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
+-rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0    13862 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0    13862 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
+-rw-r--r--   0        0        0    10284 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8997 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9318 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
+-rw-r--r--   0        0        0    14369 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12930 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16426 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
+-rw-r--r--   0        0        0    12161 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
+-rw-r--r--   0        0        0    48329 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-04-04 01:48:14.310382 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0    13941 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0   244356 2024-04-04 01:48:14.279142 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glcorearb.h
+-rw-r--r--   0        0        0   810011 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glext.h
+-rw-r--r--   0        0        0    48113 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glxext.h
+-rw-r--r--   0        0        0    44095 2024-04-04 01:48:14.294760 gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/wglext.h
+-rw-r--r--   0        0        0     1121 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
+-rw-r--r--   0        0        0     1060 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
+-rw-r--r--   0        0        0      740 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
+-rw-r--r--   0        0        0     1135 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
+-rw-r--r--   0        0        0     1045 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/include/md5global.h
+-rw-r--r--   0        0        0      312 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
+-rw-r--r--   0        0        0      418 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/config.h
+-rw-r--r--   0        0        0      660 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/libenchant.rc
+-rw-r--r--   0        0        0    17426 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/makefile.mak
+-rw-r--r--   0        0        0      754 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
+-rw-r--r--   0        0        0     2152 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/ffmpeg/build/build.sh
+-rw-r--r--   0        0        0      787 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
+-rw-r--r--   0        0        0     3296 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch
+-rw-r--r--   0        0        0    33686 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-c99.patch
+-rw-r--r--   0        0        0      367 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
+-rw-r--r--   0        0        0     9543 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/libtextstyle-c99.patch
+-rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     7623 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33617 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0     2128 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43681 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27515 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4377 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32044 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
+-rw-r--r--   0        0        0    37498 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
+-rw-r--r--   0        0        0     4322 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63279 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63715 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
+-rw-r--r--   0        0        0    44998 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0     3250 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    35655 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
+-rw-r--r--   0        0        0    81450 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    62421 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38906 2024-04-04 01:48:14.311414 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    20126 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
+-rw-r--r--   0        0        0    19299 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
+-rw-r--r--   0        0        0     3088 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
+-rw-r--r--   0        0        0     2708 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
+-rw-r--r--   0        0        0     7648 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
+-rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     2093 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
+-rw-r--r--   0        0        0    22716 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
+-rw-r--r--   0        0        0    30933 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
+-rw-r--r--   0        0        0     7623 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33701 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0    25904 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
+-rw-r--r--   0        0        0     2128 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43508 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27538 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4658 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4377 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32067 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
+-rw-r--r--   0        0        0     1209 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
+-rw-r--r--   0        0        0    23409 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
+-rw-r--r--   0        0        0    37554 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
+-rw-r--r--   0        0        0    61302 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
+-rw-r--r--   0        0        0     4298 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63335 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63743 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
+-rw-r--r--   0        0        0    24900 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
+-rw-r--r--   0        0        0    32949 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
+-rw-r--r--   0        0        0    44998 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0    29890 2024-04-04 01:48:14.327090 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
+-rw-r--r--   0        0        0     3250 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    24835 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
+-rw-r--r--   0        0        0    35681 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
+-rw-r--r--   0        0        0     7748 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
+-rw-r--r--   0        0        0     4287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
+-rw-r--r--   0        0        0     1625 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
+-rw-r--r--   0        0        0    81730 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    24592 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
+-rw-r--r--   0        0        0    62584 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38904 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    27214 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
+-rw-r--r--   0        0        0     1287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
+-rw-r--r--   0        0        0    91289 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
+-rw-r--r--   0        0        0     4873 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
+-rw-r--r--   0        0        0    23344 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
+-rw-r--r--   0        0        0    46391 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
+-rw-r--r--   0        0        0     1629 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
+-rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
+-rw-r--r--   0        0        0     7648 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
+-rw-r--r--   0        0        0    33726 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
+-rw-r--r--   0        0        0    17539 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
+-rw-r--r--   0        0        0    26333 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
+-rw-r--r--   0        0        0    43508 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
+-rw-r--r--   0        0        0     4402 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
+-rw-r--r--   0        0        0    32092 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
+-rw-r--r--   0        0        0    37579 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
+-rw-r--r--   0        0        0     4333 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
+-rw-r--r--   0        0        0    63360 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
+-rw-r--r--   0        0        0    63768 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
+-rw-r--r--   0        0        0    45023 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
+-rw-r--r--   0        0        0     3275 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
+-rw-r--r--   0        0        0    13023 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
+-rw-r--r--   0        0        0    35677 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
+-rw-r--r--   0        0        0     7748 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
+-rw-r--r--   0        0        0     4287 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
+-rw-r--r--   0        0        0    81764 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
+-rw-r--r--   0        0        0    62609 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
+-rw-r--r--   0        0        0    38929 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
+-rw-r--r--   0        0        0    27563 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
+-rw-r--r--   0        0        0     4432 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    23446 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
+-rw-r--r--   0        0        0     3065 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
+-rw-r--r--   0        0        0     7643 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
+-rw-r--r--   0        0        0    33637 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
+-rw-r--r--   0        0        0     4938 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
+-rw-r--r--   0        0        0     5545 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
+-rw-r--r--   0        0        0     9729 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
+-rw-r--r--   0        0        0     2028 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
+-rw-r--r--   0        0        0     2257 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
+-rw-r--r--   0        0        0    10124 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
+-rw-r--r--   0        0        0     6212 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
+-rw-r--r--   0        0        0    16052 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
+-rw-r--r--   0        0        0     2765 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
+-rw-r--r--   0        0        0     6279 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
+-rw-r--r--   0        0        0    43677 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
+-rw-r--r--   0        0        0     4658 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-04-04 01:48:14.342715 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4396 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
+-rw-r--r--   0        0        0    37518 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
+-rw-r--r--   0        0        0     4873 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
+-rw-r--r--   0        0        0     4326 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
+-rw-r--r--   0        0        0    23157 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
+-rw-r--r--   0        0        0    63299 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
+-rw-r--r--   0        0        0    63735 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
+-rw-r--r--   0        0        0    46251 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
+-rw-r--r--   0        0        0    45018 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
+-rw-r--r--   0        0        0    29922 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
+-rw-r--r--   0        0        0     3272 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
+-rw-r--r--   0        0        0     1649 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
+-rw-r--r--   0        0        0     4432 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    35661 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
+-rw-r--r--   0        0        0    81477 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
+-rw-r--r--   0        0        0    62439 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
+-rw-r--r--   0        0        0    54409 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75068 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97908 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75124 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.358338 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75149 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54408 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75065 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97907 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75121 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75146 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54410 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97906 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    21997 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49879 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54407 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74958 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97900 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75014 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75039 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.374043 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54406 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97945 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    22956 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
+-rw-r--r--   0        0        0     6490 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/config-msvc.mak
+-rw-r--r--   0        0        0    16869 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
+-rwxr-xr-x   0        0        0      846 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists.bat
+-rw-r--r--   0        0        0     5708 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
+-rw-r--r--   0        0        0      772 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak
+-rw-r--r--   0        0        0     4576 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
+-rw-r--r--   0        0        0     8982 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
+-rw-r--r--   0        0        0     2466 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextlib.def
+-rw-r--r--   0        0        0     2852 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def
+-rw-r--r--   0        0        0     3788 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
+-rw-r--r--   0        0        0     2635 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle.def
+-rw-r--r--   0        0        0     1051 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/Makefile.vc
+-rw-r--r--   0        0        0     1582 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0     1582 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0       30 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
+-rw-r--r--   0        0        0       27 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
+-rw-r--r--   0        0        0     1123 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
+-rw-r--r--   0        0        0      394 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/meson.build
+-rw-r--r--   0        0        0      611 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch
+-rw-r--r--   0        0        0     1468 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
+-rw-r--r--   0        0        0      759 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
+-rw-r--r--   0        0        0     2083 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
+-rw-r--r--   0        0        0     1668 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch
+-rw-r--r--   0        0        0     1958 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
+-rw-r--r--   0        0        0     1186 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
+-rw-r--r--   0        0        0     1920 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
+-rw-r--r--   0        0        0     1956 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
+-rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
+-rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
+-rw-r--r--   0        0        0    10679 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
+-rw-r--r--   0        0        0     1080 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
+-rw-r--r--   0        0        0    11397 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
+-rw-r--r--   0        0        0     3760 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
+-rw-r--r--   0        0        0    13364 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
+-rw-r--r--   0        0        0     4222 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
+-rw-r--r--   0        0        0     6519 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
+-rw-r--r--   0        0        0     3640 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
+-rw-r--r--   0        0        0    12279 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
+-rw-r--r--   0        0        0     4640 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
+-rw-r--r--   0        0        0     1962 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
+-rw-r--r--   0        0        0    23804 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
+-rw-r--r--   0        0        0     7938 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
+-rw-r--r--   0        0        0     9247 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
+-rw-r--r--   0        0        0      706 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
+-rw-r--r--   0        0        0     2185 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
+-rw-r--r--   0        0        0    26897 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
+-rw-r--r--   0        0        0    26470 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
+-rw-r--r--   0        0        0     9451 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
+-rw-r--r--   0        0        0     1756 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
+-rw-r--r--   0        0        0     3586 2024-04-04 01:48:14.389600 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0      803 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-accel.patch
+-rw-r--r--   0        0        0      599 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-bgimg.patch
+-rw-r--r--   0        0        0      682 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch
+-rw-r--r--   0        0        0     2154 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
+-rw-r--r--   0        0        0     1104 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk2/mod.md
+-rw-r--r--   0        0        0     6104 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
+-rw-r--r--   0        0        0    11322 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
+-rw-r--r--   0        0        0     1630 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
+-rw-r--r--   0        0        0     1261 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtk4/001-fix-pangoft2-file-not-found.patch
+-rw-r--r--   0        0        0     1088 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch
+-rw-r--r--   0        0        0      102 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/hello-world/hello-world.c
+-rw-r--r--   0        0        0       66 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/hello-world/meson.build
+-rw-r--r--   0        0        0      359 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/icu/pc-files/icu-uc.pc
+-rw-r--r--   0        0        0      360 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
+-rw-r--r--   0        0        0    39523 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
+-rw-r--r--   0        0        0      652 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/mod.md
+-rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
+-rw-r--r--   0        0        0     4827 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/fficonfig.h.meson
+-rw-r--r--   0        0        0      475 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/include/meson.build
+-rw-r--r--   0        0        0      248 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
+-rw-r--r--   0        0        0    13940 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson.build
+-rw-r--r--   0        0        0     1154 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson_options.txt
+-rw-r--r--   0        0        0     3334 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libffi/src/meson.build
+-rw-r--r--   0        0        0      936 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
+-rw-r--r--   0        0        0     1243 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
+-rw-r--r--   0        0        0     9777 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
+-rw-r--r--   0        0        0       44 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/mod.md
+-rw-r--r--   0        0        0      318 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/pc-files/libpng.pc
+-rw-r--r--   0        0        0      318 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libpng/pc-files/libpng16.pc
+-rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
+-rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
+-rw-r--r--   0        0        0     9178 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
+-rw-r--r--   0        0        0      937 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
+-rw-r--r--   0        0        0     4286 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
+-rw-r--r--   0        0        0      572 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    17549 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     3085 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     2998 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
+-rw-r--r--   0        0        0     8574 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
+-rw-r--r--   0        0        0     1026 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
+-rw-r--r--   0        0        0      931 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
+-rw-r--r--   0        0        0     2133 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
+-rw-r--r--   0        0        0     6578 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
+-rw-r--r--   0        0        0     2326 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
+-rw-r--r--   0        0        0     8979 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
+-rw-r--r--   0        0        0      925 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
+-rw-r--r--   0        0        0    14576 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
+-rw-r--r--   0        0        0     3427 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
+-rw-r--r--   0        0        0      866 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
+-rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/config.h
+-rw-r--r--   0        0        0     8059 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
+-rw-r--r--   0        0        0     3769 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/property.props
+-rw-r--r--   0        0        0    40095 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/config.h
+-rw-r--r--   0        0        0     8059 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
+-rw-r--r--   0        0        0     3767 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/property.props
+-rw-r--r--   0        0        0    40095 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.405218 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/config.h
+-rw-r--r--   0        0        0     8138 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
+-rw-r--r--   0        0        0     3899 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/property.props
+-rw-r--r--   0        0        0    40174 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     1079 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libssh/mod.md
+-rw-r--r--   0        0        0      809 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
+-rw-r--r--   0        0        0     2586 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
+-rw-r--r--   0        0        0     1251 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
+-rw-r--r--   0        0        0     1025 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/include/libxml/meson.build
+-rw-r--r--   0        0        0     1089 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/LICENSE.build
+-rw-r--r--   0        0        0     7284 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/meson.build
+-rw-r--r--   0        0        0      323 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
+-rw-r--r--   0        0        0      943 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libyuv/001-win-build.patch
+-rw-r--r--   0        0        0      392 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/libyuv/pc-files/libyuv.pc
+-rw-r--r--   0        0        0      352 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/luajit/pc-files/luajit.pc
+-rw-r--r--   0        0        0      971 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/luajit/set-paths.patch
+-rw-r--r--   0        0        0      319 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/pc-files/liblz4.pc
+-rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
+-rw-r--r--   0        0        0     8966 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9317 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9317 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10138 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9145 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9206 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9309 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
+-rw-r--r--   0        0        0     9976 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
+-rw-r--r--   0        0        0       93 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/mod.md
+-rw-r--r--   0        0        0      733 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
+-rw-r--r--   0        0        0     2184 2024-04-04 01:48:14.420840 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch
+-rw-r--r--   0        0        0  1290625 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/certdata.txt
+-rw-r--r--   0        0        0    19616 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
+-rw-r--r--   0        0        0      412 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mod.md
+-rw-r--r--   0        0        0      275 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
+-rw-r--r--   0        0        0      285 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/libssl.pc
+-rw-r--r--   0        0        0      236 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/pc-files/openssl.pc
+-rw-r--r--   0        0        0      383 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/opus/pc-files/opus.pc
+-rw-r--r--   0        0        0    11464 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch
+-rw-r--r--   0        0        0     1027 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch
+-rw-r--r--   0        0        0     1089 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/LICENSE.build
+-rw-r--r--   0        0        0     7523 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson.build
+-rw-r--r--   0        0        0      473 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson_options.txt
+-rw-r--r--   0        0        0     1241 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
+-rw-r--r--   0        0        0     1036 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
+-rw-r--r--   0        0        0     2647 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
+-rw-r--r--   0        0        0      319 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
+-rw-r--r--   0        0        0     1912 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
+-rw-r--r--   0        0        0      633 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/stack.props
+-rw-r--r--   0        0        0     1565 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/COPYING
+-rw-r--r--   0        0        0       92 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/mod.md
+-rw-r--r--   0        0        0      671 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/x264/build/build.sh
+-rw-r--r--   0        0        0     1385 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
+-rw-r--r--   0        0        0      343 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/patches/zlib/pc-files/zlib.pc
+-rw-r--r--   0        0        0     4259 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/__init__.py
+-rw-r--r--   0        0        0     2040 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/adwaita_icon_theme.py
+-rw-r--r--   0        0        0     1808 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/atk.py
+-rw-r--r--   0        0        0     1774 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/boringssl.py
+-rw-r--r--   0        0        0     1598 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cairo.py
+-rw-r--r--   0        0        0     1509 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cairomm.py
+-rw-r--r--   0        0        0     1912 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/check_libs.py
+-rw-r--r--   0        0        0     1620 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/clutter.py
+-rw-r--r--   0        0        0     1758 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cogl.py
+-rw-r--r--   0        0        0     2872 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/cyrus_sasl.py
+-rw-r--r--   0        0        0     2844 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/dev_shell.py
+-rw-r--r--   0        0        0     1648 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/emeus.py
+-rw-r--r--   0        0        0     2807 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/enchant.py
+-rw-r--r--   0        0        0     1572 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/expat.py
+-rw-r--r--   0        0        0     3388 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/ffmpeg.py
+-rw-r--r--   0        0        0     1725 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/freerdp.py
+-rw-r--r--   0        0        0     1638 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/freetype.py
+-rw-r--r--   0        0        0     2093 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/fribidi.py
+-rw-r--r--   0        0        0     2204 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gdk_pixbuf.py
+-rw-r--r--   0        0        0     4032 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gettext.py
+-rw-r--r--   0        0        0     4682 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/glib.py
+-rw-r--r--   0        0        0     1704 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/glibmm.py
+-rw-r--r--   0        0        0     2684 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gobject_introspection.py
+-rw-r--r--   0        0        0     1312 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gperf.py
+-rw-r--r--   0        0        0     1752 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/graphene.py
+-rw-r--r--   0        0        0     1813 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gsettings_desktop_schemas.py
+-rw-r--r--   0        0        0     8797 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gstreamer.py
+-rw-r--r--   0        0        0     5945 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtk.py
+-rw-r--r--   0        0        0     1806 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtkmm.py
+-rw-r--r--   0        0        0     2846 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/gtksourceview.py
+-rw-r--r--   0        0        0     1672 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/harfbuzz.py
+-rw-r--r--   0        0        0     1184 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/hello_world.py
+-rw-r--r--   0        0        0     1382 2024-04-04 01:48:14.436468 gvsbuild-2024.4.0/gvsbuild/projects/hicolor_icon_theme.py
+-rw-r--r--   0        0        0     2276 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/icu.py
+-rw-r--r--   0        0        0     1832 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/json_glib.py
+-rw-r--r--   0        0        0     1392 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/jsonc.py
+-rw-r--r--   0        0        0     1624 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/leveldb.py
+-rw-r--r--   0        0        0     1417 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lgi.py
+-rw-r--r--   0        0        0     2063 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libadwaita.py
+-rw-r--r--   0        0        0     2075 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libarchive.py
+-rw-r--r--   0        0        0     1781 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcbor.py
+-rw-r--r--   0        0        0     1496 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcroco.py
+-rw-r--r--   0        0        0     1903 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libcurl.py
+-rw-r--r--   0        0        0     1447 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libepoxy.py
+-rw-r--r--   0        0        0     1341 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libffi.py
+-rw-r--r--   0        0        0     2597 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libfido2.py
+-rw-r--r--   0        0        0     1989 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libgxps.py
+-rw-r--r--   0        0        0     1741 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libjpeg_turbo.py
+-rw-r--r--   0        0        0     2331 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libmicrohttpd.py
+-rw-r--r--   0        0        0     1704 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libpng.py
+-rw-r--r--   0        0        0     1595 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libpsl.py
+-rw-r--r--   0        0        0     2405 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/librsvg.py
+-rw-r--r--   0        0        0     1737 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libsigcplusplus.py
+-rw-r--r--   0        0        0     3368 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libsoup.py
+-rw-r--r--   0        0        0     2181 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libssh.py
+-rw-r--r--   0        0        0     1586 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libtiff.py
+-rw-r--r--   0        0        0     1514 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libuv.py
+-rw-r--r--   0        0        0     1511 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libvorbis.py
+-rw-r--r--   0        0        0     3265 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libvpx.py
+-rw-r--r--   0        0        0     1574 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libxml2.py
+-rw-r--r--   0        0        0     1576 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libyuv.py
+-rw-r--r--   0        0        0     1411 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/libzip.py
+-rw-r--r--   0        0        0     1426 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lmdb.py
+-rw-r--r--   0        0        0     1761 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/luajit.py
+-rw-r--r--   0        0        0     1778 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/lz4.py
+-rw-r--r--   0        0        0     2279 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/mit_kerberos.py
+-rw-r--r--   0        0        0     1587 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/nghttp2.py
+-rw-r--r--   0        0        0     1477 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/ogg.py
+-rw-r--r--   0        0        0     1521 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/openh264.py
+-rw-r--r--   0        0        0     3381 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/openssl.py
+-rw-r--r--   0        0        0     2056 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/opus.py
+-rw-r--r--   0        0        0     2046 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pango.py
+-rw-r--r--   0        0        0     1768 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pangomm.py
+-rw-r--r--   0        0        0      712 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pcre2.py
+-rw-r--r--   0        0        0     1672 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pixman.py
+-rw-r--r--   0        0        0     1692 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pkgconf.py
+-rw-r--r--   0        0        0     2711 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/protobuf.py
+-rw-r--r--   0        0        0     2102 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pycairo.py
+-rw-r--r--   0        0        0     2591 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/pygobject.py
+-rw-r--r--   0        0        0     1618 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/sqlite.py
+-rw-r--r--   0        0        0     1607 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/win_iconv.py
+-rw-r--r--   0        0        0     1470 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/wing.py
+-rw-r--r--   0        0        0     2341 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/x264.py
+-rw-r--r--   0        0        0     2444 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/projects/zlib.py
+-rw-r--r--   0        0        0     7545 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/tools.py
+-rw-r--r--   0        0        0       30 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/__init__.py
+-rw-r--r--   0        0        0     8512 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_builders.py
+-rw-r--r--   0        0        0    15193 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_expanders.py
+-rw-r--r--   0        0        0     1339 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_group.py
+-rw-r--r--   0        0        0    20353 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_project.py
+-rw-r--r--   0        0        0     2749 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/base_tool.py
+-rw-r--r--   0        0        0    38283 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/builder.py
+-rw-r--r--   0        0        0     9899 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/simple_ui.py
+-rw-r--r--   0        0        0     3899 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/gvsbuild/utils/utils.py
+-rw-r--r--   0        0        0     1653 2024-04-04 01:48:14.452089 gvsbuild-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12300 2024-04-04 01:48:14.232260 gvsbuild-2024.4.0/README.md
+-rw-r--r--   0        0        0    13026 1970-01-01 00:00:00.000000 gvsbuild-2024.4.0/PKG-INFO
```

### Comparing `gvsbuild-2024.3.1/AUTHORS.md` & `gvsbuild-2024.4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/COPYING` & `gvsbuild-2024.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/build.py` & `gvsbuild-2024.4.0/gvsbuild/build.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/deps.py` & `gvsbuild-2024.4.0/gvsbuild/deps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/groups.py` & `gvsbuild-2024.4.0/gvsbuild/groups.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/list.py` & `gvsbuild-2024.4.0/gvsbuild/list.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/main.py` & `gvsbuild-2024.4.0/gvsbuild/main.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/outdated.py` & `gvsbuild-2024.4.0/gvsbuild/outdated.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/check-libs/check_utils.h` & `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/check_utils.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/check-libs/COPYING` & `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/check-libs/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/check-libs/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glcorearb.h` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glcorearb.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glext.h` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/glxext.h` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/glxext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cogl/GL/wglext.h` & `gvsbuild-2024.4.0/gvsbuild/patches/cogl/GL/wglext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/cyrus-sasl/include/md5global.h` & `gvsbuild-2024.4.0/gvsbuild/patches/cyrus-sasl/include/md5global.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/enchant/src/libenchant.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/libenchant.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/enchant/src/makefile.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/enchant/src/makefile.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/ffmpeg/build/build.sh` & `gvsbuild-2024.4.0/gvsbuild/patches/ffmpeg/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/gettext-tools-c99.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/gettext-tools-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/libtextstyle-c99.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/libtextstyle-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/config-msvc.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/config-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/create-lists.bat` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/create-lists.bat`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libgettextlib.def` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextlib.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/libtextstyle.def` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/libtextstyle.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gettext/nmake/Makefile.vc` & `gvsbuild-2024.4.0/gvsbuild/patches/gettext/nmake/Makefile.vc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c` & `gvsbuild-2024.4.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-accel.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-accel.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-bgimg.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-bgimg.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk2/mod.md` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk2/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 Subject: [PATCH] Remove appstream dependency
+
 ---
-Index: subprojects/appstream.wrap
-===================================================================
-diff --git a/subprojects/appstream.wrap b/subprojects/appstream.wrap
-deleted file mode 100644
---- a/subprojects/appstream.wrap	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ /dev/null	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-@@ -1,5 +0,0 @@
--[wrap-git]
--directory = appstream
--url = https://github.com/ximion/appstream.git
--revision = main
--depth = 1
-Index: tests/org.gnome.Adwaita1.Test.metainfo.xml
-===================================================================
-diff --git a/tests/org.gnome.Adwaita1.Test.metainfo.xml b/tests/org.gnome.Adwaita1.Test.metainfo.xml
-deleted file mode 100644
---- a/tests/org.gnome.Adwaita1.Test.metainfo.xml	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ /dev/null	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-@@ -1,29 +0,0 @@
--<?xml version="1.0" encoding="UTF-8"?>
--<component type="desktop-application">
--  <id>org.gnome.Adwaita1.Test</id>
--  <metadata_license>CC0-1.0</metadata_license>
--  <project_license>LGPL-2.1-or-later</project_license>
--  <launchable type="desktop-id">org.gnome.Adwaita1.Test.desktop</launchable>
--  <developer_name>The GNOME Project</developer_name>
--
--  <name>Adwaita Test</name>
--
--  <releases>
--    <release version="1.0">
--      <description>
--        <p>Testing Build</p>
--      </description>
--    </release>
--    <release version="0.1">
--      <description>
--        <p>Testing Build Older</p>
--      </description>
--    </release>
--  </releases>
--
--  <project_group>GNOME</project_group>
+ demo/adwaita-demo.c                        |  28 ++-
+ demo/adwaita-demo.gresources.xml           |   1 -
+ demo/data/meson.build                      |  19 --
+ demo/meson.build                           |   3 -
+ src/adw-about-dialog.c                     | 219 -----------------
+ src/adw-about-dialog.h                     |   7 -
+ src/adw-about-window.c                     | 259 ++-------------------
+ src/adw-about-window.h                     |  13 +-
+ src/meson.build                            |   8 -
+ subprojects/appstream.wrap                 |   5 -
+ tests/meson.build                          |  16 +-
+ tests/org.gnome.Adwaita1.Test.metainfo.xml |  29 ---
+ tests/test-about-dialog.c                  |  49 ----
+ tests/test-about-window.c                  |  49 ----
+ tests/tests.gresources.xml                 |   6 -
+ 15 files changed, 39 insertions(+), 672 deletions(-)
+ delete mode 100644 subprojects/appstream.wrap
+ delete mode 100644 tests/org.gnome.Adwaita1.Test.metainfo.xml
+ delete mode 100644 tests/tests.gresources.xml
+
+diff --git a/demo/adwaita-demo.c b/demo/adwaita-demo.c
+index f2d25f6e..a023275d 100644
+--- a/demo/adwaita-demo.c
++++ b/demo/adwaita-demo.c
+@@ -1,5 +1,3 @@
+-#include "config.h"
 -
--  <url type="homepage">https://gitlab.gnome.org/GNOME/libadwaita</url>
--  <url type="bugtracker">https://gitlab.gnome.org/GNOME/libadwaita/issues</url>
--  <url type="help">http://www.gnome.org/friends/</url>
--</component>
-Index: tests/tests.gresources.xml
-===================================================================
-diff --git a/tests/tests.gresources.xml b/tests/tests.gresources.xml
-deleted file mode 100644
---- a/tests/tests.gresources.xml	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ /dev/null	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-@@ -1,6 +0,0 @@
--<?xml version="1.0" encoding="UTF-8"?>
--<gresources>
--  <gresource prefix="/org/gnome/Adwaita1/Test">
--    <file compressed="true">org.gnome.Adwaita1.Test.metainfo.xml</file>
--  </gresource>
--</gresources>
-Index: demo/data/meson.build
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
+ #include <glib/gi18n.h>
+ #include <gtk/gtk.h>
+ #include <adwaita.h>
+@@ -57,15 +55,23 @@ show_about (GSimpleAction *action,
+ 
+   debug_info = adw_demo_generate_debug_info ();
+ 
+-  about = adw_about_dialog_new_from_appdata ("/org/gnome/Adwaita1/Demo/org.gnome.Adwaita1.Demo.metainfo.xml", NULL);
+-  adw_about_dialog_set_version (ADW_ABOUT_DIALOG (about), ADW_VERSION_S);
+-  adw_about_dialog_set_debug_info (ADW_ABOUT_DIALOG (about), debug_info);
+-  adw_about_dialog_set_debug_info_filename (ADW_ABOUT_DIALOG (about), "adwaita-1-demo-debug-info.txt");
+-  adw_about_dialog_set_copyright (ADW_ABOUT_DIALOG (about), "© 2017–2022 Purism SPC");
+-  adw_about_dialog_set_developers (ADW_ABOUT_DIALOG (about), developers);
+-  adw_about_dialog_set_designers (ADW_ABOUT_DIALOG (about), designers);
+-  adw_about_dialog_set_artists (ADW_ABOUT_DIALOG (about), designers);
+-  adw_about_dialog_set_translator_credits (ADW_ABOUT_DIALOG (about), _("translator-credits"));
++  about =
++    g_object_new (ADW_TYPE_ABOUT_DIALOG,
++                  "application-icon", "org.gnome.Adwaita1.Demo",
++                  "application-name", _("Adwaita Demo"),
++                  "developer-name", _("The GNOME Project"),
++                  "version", ADW_VERSION_S,
++                  "website", "https://gitlab.gnome.org/GNOME/libadwaita",
++                  "issue-url", "https://gitlab.gnome.org/GNOME/libadwaita/-/issues/new",
++                  "debug-info", debug_info,
++                  "debug-info-filename", "adwaita-1-demo-debug-info.txt",
++                  "copyright", "© 2017–2022 Purism SPC",
++                  "license-type", GTK_LICENSE_LGPL_2_1,
++                  "developers", developers,
++                  "designers", designers,
++                  "artists", designers,
++                  "translator-credits", _("translator-credits"),
++                  NULL);
+ 
+   adw_about_dialog_add_link (ADW_ABOUT_DIALOG (about),
+                              _("_Documentation"),
+diff --git a/demo/adwaita-demo.gresources.xml b/demo/adwaita-demo.gresources.xml
+index 86e6b067..acea0eb3 100644
+--- a/demo/adwaita-demo.gresources.xml
++++ b/demo/adwaita-demo.gresources.xml
+@@ -3,7 +3,6 @@
+   <gresource prefix="/org/gnome/Adwaita1/Demo">
+     <file preprocess="xml-stripblanks" alias="icons/scalable/apps/org.gnome.Adwaita1.Demo.svg">data/org.gnome.Adwaita1.Demo.svg</file>
+     <file preprocess="xml-stripblanks" alias="icons/symbolic/apps/org.gnome.Adwaita1.Demo-symbolic.svg">data/org.gnome.Adwaita1.Demo-symbolic.svg</file>
+-    <file preprocess="xml-stripblanks" alias="org.gnome.Adwaita1.Demo.metainfo.xml">data/org.gnome.Adwaita1.Demo.metainfo.xml</file>
+     <file preprocess="xml-stripblanks">icons/scalable/actions/avatar-delete-symbolic.svg</file>
+     <file preprocess="xml-stripblanks">icons/scalable/actions/avatar-save-symbolic.svg</file>
+     <file preprocess="xml-stripblanks">icons/scalable/actions/clock-alarm-symbolic.svg</file>
 diff --git a/demo/data/meson.build b/demo/data/meson.build
---- a/demo/data/meson.build	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/demo/data/meson.build	(date 1702739024177)
-@@ -40,25 +40,6 @@
+index 5d176351..12928ac2 100644
+--- a/demo/data/meson.build
++++ b/demo/data/meson.build
+@@ -34,25 +34,6 @@ appdata_config = configuration_data()
  appdata_config.set('BUILD_VERSION', meson.project_version())
  appdata_config.set('BUILD_DATE', today)
  
 -appstream_file = i18n.merge_file(
 -  input: configure_file(
 -    input: 'org.gnome.Adwaita1.Demo.metainfo.xml.in.in',
 -    output: 'org.gnome.Adwaita1.Demo.metainfo.xml.in',
@@ -91,31 +102,312 @@
 -    args: ['validate', '--no-net', '--explain', appstream_file]
 -  )
 -endif
 -
  install_data(
    'org.gnome.Adwaita1.Demo.svg',
    install_dir: datadir / 'icons' / 'hicolor' / 'scalable' / 'apps'
-Index: src/adw-about-window.c
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
+diff --git a/demo/meson.build b/demo/meson.build
+index ca04e31f..d01e1651 100644
+--- a/demo/meson.build
++++ b/demo/meson.build
+@@ -3,7 +3,6 @@ if get_option('examples')
+ subdir('data')
+ 
+ demo_config_data = configuration_data()
+-demo_config_data.set_quoted('ADW_METAINFO', appstream_file.full_path())
+ demo_config_data.set_quoted('ADW_DEMO_VCS_TAG', '@VCS_TAG@')
+ 
+ demo_config_h = vcs_tag(
+@@ -19,8 +18,6 @@ adwaita_demo_resources = gnome.compile_resources(
+    'adwaita-demo.gresources.xml',
+ 
+    c_name: 'adw',
+-   dependencies: appstream_file,
+-   source_dir: meson.current_build_dir(),
+ )
+ 
+ adwaita_demo_sources = [
+diff --git a/src/adw-about-dialog.c b/src/adw-about-dialog.c
+index 1bed7bed..73af0179 100644
+--- a/src/adw-about-dialog.c
++++ b/src/adw-about-dialog.c
+@@ -7,7 +7,6 @@
+ 
+ #include "config.h"
+ #include <glib/gi18n-lib.h>
+-#include <appstream.h>
+ 
+ #include "adw-about-dialog.h"
+ 
+@@ -411,13 +410,6 @@ legal_showing_cb (AdwAboutDialog *self)
+   self->legal_showing_idle_id = 0;
+ }
+ 
+-static gboolean
+-get_release_for_version (AsRelease  *rel,
+-                         const char *version)
+-{
+-  return !g_strcmp0 (as_release_get_version (rel), version);
+-}
+-
+ static void
+ update_credits_legal_group (AdwAboutDialog *self)
+ {
+@@ -1953,179 +1945,6 @@ adw_about_dialog_new (void)
+   return g_object_new (ADW_TYPE_ABOUT_DIALOG, NULL);
+ }
+ 
+-/**
+- * adw_about_dialog_new_from_appdata:
+- * @resource_path: The resource to use
+- * @release_notes_version: (nullable): The version to retrieve release notes for
+- *
+- * Creates a new `AdwAboutDialog` using AppStream metadata.
+- *
+- * This automatically sets the following properties with the following AppStream
+- * values:
+- *
+- * * [property@AboutDialog:application-icon] is set from the `<id>`
+- * * [property@AboutDialog:application-name] is set from the `<name>`
+- * * [property@AboutDialog:developer-name] is set from the `<developer_name>`
+- * * [property@AboutDialog:version] is set from the version of the latest release
+- * * [property@AboutDialog:website] is set from the `<url type="homepage">`
+- * * [property@AboutDialog:support-url] is set from the `<url type="help">`
+- * * [property@AboutDialog:issue-url] is set from the `<url type="bugtracker">`
+- * * [property@AboutDialog:license-type] is set from the `<project_license>`
+- *   If the license type retrieved from AppStream is not listed in
+- *   [enum@Gtk.License], it will be set to `GTK_LICENCE_CUSTOM`.
+- *
+- * If @release_notes_version is not `NULL`,
+- * [property@AboutDialog:release-notes-version] is set to match it, while
+- * [property@AboutDialog:release-notes] is set from the AppStream release
+- * description for that version.
+- *
+- * Returns: the newly created `AdwAboutDialog`
+- *
+- * Since: 1.5
+- */
+-AdwDialog *
+-adw_about_dialog_new_from_appdata (const char *resource_path,
+-                                   const char *release_notes_version)
+-{
+-  AdwAboutDialog *self;
+-  GFile *appdata_file;
+-  char *appdata_uri;
+-  AsMetadata *metadata;
+-  GPtrArray *releases;
+-  AsComponent *component;
+-  char *application_id;
+-  const char *name, *developer_name, *project_license;
+-  const char *issue_url, *support_url, *website_url;
+-  GError *error = NULL;
+-
+-  g_return_val_if_fail (resource_path, NULL);
+-
+-  appdata_uri = g_strconcat ("resource://", resource_path, NULL);
+-  appdata_file = g_file_new_for_uri (appdata_uri);
+-
+-  self = ADW_ABOUT_DIALOG (adw_about_dialog_new ());
+-  metadata = as_metadata_new ();
+-
+-  if (!as_metadata_parse_file (metadata, appdata_file, AS_FORMAT_KIND_UNKNOWN, &error)) {
+-    g_error ("Could not parse metadata file: %s", error->message);
+-    g_clear_error (&error);
+-  }
+-
+-  component = as_metadata_get_component (metadata);
+-
+-  if (component == NULL)
+-    g_error ("Could not find valid AppStream metadata");
+-
+-  application_id = g_strdup (as_component_get_id (component));
+-
+-  if (g_str_has_suffix (application_id, ".desktop")) {
+-    AsLaunchable *launchable;
+-    char *appid_desktop;
+-    GPtrArray *entries = NULL;
+-
+-    launchable = as_component_get_launchable (component,
+-                                              AS_LAUNCHABLE_KIND_DESKTOP_ID);
+-
+-    if (launchable)
+-      entries = as_launchable_get_entries (launchable);
+-
+-    appid_desktop = g_strconcat (application_id, ".desktop", NULL);
+-
+-    if (!entries || !g_ptr_array_find_with_equal_func (entries, appid_desktop,
+-                                                       g_str_equal, NULL))
+-      application_id[strlen(application_id) - 8] = '\0';
+-
+-    g_free (appid_desktop);
+-  }
+-
+-#if AS_CHECK_VERSION (1, 0, 0)
+-  releases = as_release_list_get_entries (as_component_get_releases_plain (component));
+-#else
+-  releases = as_component_get_releases (component);
+-#endif
+-
+-  if (release_notes_version) {
+-    guint release_index = 0;
+-
+-    if (g_ptr_array_find_with_equal_func (releases, release_notes_version,
+-                                         (GEqualFunc) get_release_for_version,
+-                                         &release_index)) {
+-      AsRelease *notes_release;
+-      const char *release_notes, *version;
+-
+-      notes_release = g_ptr_array_index (releases, release_index);
+-
+-      release_notes = as_release_get_description (notes_release);
+-      version = as_release_get_version (notes_release);
+-
+-      if (release_notes && version) {
+-        adw_about_dialog_set_release_notes (self, release_notes);
+-        adw_about_dialog_set_release_notes_version (self, version);
+-      }
+-    } else {
+-      g_critical ("No valid release found for version %s", release_notes_version);
+-    }
+-  }
+-
+-  if (releases->len > 0) {
+-    AsRelease *latest_release = g_ptr_array_index (releases, 0);
+-    const char *version = as_release_get_version (latest_release);
+-
+-    if (version)
+-      adw_about_dialog_set_version (self, version);
+-  }
+-
+-  name = as_component_get_name (component);
+-  project_license = as_component_get_project_license (component);
+-  issue_url = as_component_get_url (component, AS_URL_KIND_BUGTRACKER);
+-  support_url = as_component_get_url (component, AS_URL_KIND_HELP);
+-  website_url = as_component_get_url (component, AS_URL_KIND_HOMEPAGE);
+-
+-#if AS_CHECK_VERSION (0, 16, 4)
+-  developer_name = as_developer_get_name (as_component_get_developer (component));
+-#else
+-  developer_name = as_component_get_developer_name (component);
+-#endif
+-
+-  adw_about_dialog_set_application_icon (self, application_id);
+-
+-  if (name)
+-    adw_about_dialog_set_application_name (self, name);
+-
+-  if (developer_name)
+-    adw_about_dialog_set_developer_name (self, developer_name);
+-
+-  if (project_license) {
+-    int i;
+-
+-    for (i = 0; i < G_N_ELEMENTS (gtk_license_info); i++) {
+-      if (g_strcmp0 (gtk_license_info[i].spdx_id, project_license) == 0) {
+-        adw_about_dialog_set_license_type (self, (GtkLicense) i);
+-        break;
+-      }
+-    }
+-
+-    if (adw_about_dialog_get_license_type (self) == GTK_LICENSE_UNKNOWN)
+-      adw_about_dialog_set_license_type (self, GTK_LICENSE_CUSTOM);
+-  }
+-
+-  if (issue_url)
+-    adw_about_dialog_set_issue_url (self, issue_url);
+-
+-  if (support_url)
+-    adw_about_dialog_set_support_url (self, support_url);
+-
+-  if (website_url)
+-    adw_about_dialog_set_website (self, website_url);
+-
+-  g_object_unref (appdata_file);
+-  g_object_unref (metadata);
+-  g_free (application_id);
+-  g_free (appdata_uri);
+-
+-  return ADW_DIALOG (self);
+-}
+-
+ /**
+  * adw_about_dialog_get_application_icon: (attributes org.gtk.Method.get_property=application-icon)
+  * @self: an about dialog
+@@ -3422,41 +3241,3 @@ adw_show_about_dialog (GtkWidget  *parent,
+ 
+   adw_dialog_present (dialog, parent);
+ }
+-
+-/**
+- * adw_show_about_dialog_from_appdata: (skip)
+- * @parent: the parent widget
+- * @resource_path: The resource to use
+- * @release_notes_version: (nullable): The version to retrieve release notes for
+- * @first_property_name: the name of the first property
+- * @...: value of first property, followed by more pairs of property name and
+- *   value, `NULL`-terminated
+- *
+- * A convenience function for showing an application’s about dialog from
+- * AppStream metadata.
+- *
+- * See [ctor@AboutDialog.new_from_appdata] for details.
+- *
+- * Since: 1.5
+- */
+-void
+-adw_show_about_dialog_from_appdata (GtkWidget  *parent,
+-                                    const char *resource_path,
+-                                    const char *release_notes_version,
+-                                    const char *first_property_name,
+-                                    ...)
+-{
+-  AdwDialog *dialog;
+-  va_list var_args;
+-
+-  g_return_if_fail (GTK_IS_WIDGET (parent));
+-
+-  dialog = adw_about_dialog_new_from_appdata (resource_path,
+-                                              release_notes_version);
+-
+-  va_start (var_args, first_property_name);
+-  g_object_set_valist (G_OBJECT (dialog), first_property_name, var_args);
+-  va_end (var_args);
+-
+-  adw_dialog_present (dialog, parent);
+-}
+diff --git a/src/adw-about-dialog.h b/src/adw-about-dialog.h
+index b41bf11e..2f1d05d0 100644
+--- a/src/adw-about-dialog.h
++++ b/src/adw-about-dialog.h
+@@ -178,11 +178,4 @@ void adw_show_about_dialog (GtkWidget  *parent,
+                             const char *first_property_name,
+                             ...) G_GNUC_NULL_TERMINATED;
+ 
+-ADW_AVAILABLE_IN_1_5
+-void adw_show_about_dialog_from_appdata (GtkWidget  *parent,
+-                                         const char *resource_path,
+-                                         const char *release_notes_version,
+-                                         const char *first_property_name,
+-                                         ...) G_GNUC_NULL_TERMINATED;
+-
+ G_END_DECLS
 diff --git a/src/adw-about-window.c b/src/adw-about-window.c
---- a/src/adw-about-window.c	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/src/adw-about-window.c	(date 1702824178498)
+index 6a816177..9c37faf0 100644
+--- a/src/adw-about-window.c
++++ b/src/adw-about-window.c
 @@ -6,7 +6,6 @@
  
  #include "config.h"
  #include <glib/gi18n-lib.h>
 -#include <appstream.h>
  
  #include "adw-about-window.h"
  
-@@ -194,31 +193,30 @@
+@@ -194,32 +193,31 @@
  typedef struct {
    const char *name;
    const char *url;
 -  const char *spdx_id;
  } LicenseInfo;
  
  /* Copied from GTK 4 for consistency with GtkAboutDialog. */
@@ -135,15 +427,16 @@
 -  { N_("GNU General Public License, version 3 only"), "https://www.gnu.org/licenses/gpl-3.0.html", "GPL-3.0" },
 -  { N_("GNU Lesser General Public License, version 2.1 only"), "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html", "LGPL-2.1-only" },
 -  { N_("GNU Lesser General Public License, version 3 only"), "https://www.gnu.org/licenses/lgpl-3.0.html", "LGPL-3.0-only" },
 -  { N_("GNU Affero General Public License, version 3 or later"), "https://www.gnu.org/licenses/agpl-3.0.html", "AGPL-3.0-or-later" },
 -  { N_("GNU Affero General Public License, version 3 only"), "https://www.gnu.org/licenses/agpl-3.0.html", "AGPL-3.0-only" },
 -  { N_("BSD 3-Clause License"), "https://opensource.org/licenses/BSD-3-Clause", "BSD-3-Clause" },
 -  { N_("Apache License, Version 2.0"), "https://opensource.org/licenses/Apache-2.0", "Apache-2.0" },
--  { N_("Mozilla Public License 2.0"), "https://opensource.org/licenses/MPL-2.0", "MPL-2.0" }
+-  { N_("Mozilla Public License 2.0"), "https://opensource.org/licenses/MPL-2.0", "MPL-2.0" },
+-  { N_("BSD Zero-Clause License"), "https://opensource.org/license/0bsd", "0BSD" }
 +  { NULL, NULL },
 +  { NULL, NULL },
 +  { N_("GNU General Public License, version 2 or later"), "https://www.gnu.org/licenses/old-licenses/gpl-2.0.html" },
 +  { N_("GNU General Public License, version 3 or later"), "https://www.gnu.org/licenses/gpl-3.0.html" },
 +  { N_("GNU Lesser General Public License, version 2.1 or later"), "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html" },
 +  { N_("GNU Lesser General Public License, version 3 or later"), "https://www.gnu.org/licenses/lgpl-3.0.html" },
 +  { N_("BSD 2-Clause License"), "https://opensource.org/licenses/bsd-license.php" },
@@ -153,33 +446,34 @@
 +  { N_("GNU General Public License, version 3 only"), "https://www.gnu.org/licenses/gpl-3.0.html" },
 +  { N_("GNU Lesser General Public License, version 2.1 only"), "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html" },
 +  { N_("GNU Lesser General Public License, version 3 only"), "https://www.gnu.org/licenses/lgpl-3.0.html" },
 +  { N_("GNU Affero General Public License, version 3 or later"), "https://www.gnu.org/licenses/agpl-3.0.html" },
 +  { N_("GNU Affero General Public License, version 3 only"), "https://www.gnu.org/licenses/agpl-3.0.html" },
 +  { N_("BSD 3-Clause License"), "https://opensource.org/licenses/BSD-3-Clause" },
 +  { N_("Apache License, Version 2.0"), "https://opensource.org/licenses/Apache-2.0" },
-+  { N_("Mozilla Public License 2.0"), "https://opensource.org/licenses/MPL-2.0" }
++  { N_("Mozilla Public License 2.0"), "https://opensource.org/licenses/MPL-2.0" },
++  { N_("BSD Zero-Clause License"), "https://opensource.org/license/0bsd" }
  };
  /* Copied from GTK 4 for consistency with GtkAboutDialog. */
  /* Keep this static assertion updated with the last element of the enumeration,
-@@ -388,13 +386,6 @@
-   return GDK_EVENT_STOP;
+@@ -409,13 +407,6 @@ legal_showing_cb (AdwAboutWindow *self)
+     g_idle_add_once ((GSourceOnceFunc) legal_showing_idle_cb, self);
  }
  
 -static gboolean
 -get_release_for_version (AsRelease  *rel,
 -                         const char *version)
 -{
 -  return !g_strcmp0 (as_release_get_version (rel), version);
 -}
 -
  static void
  update_credits_legal_group (AdwAboutWindow *self)
  {
-@@ -1919,179 +1910,6 @@
+@@ -1952,179 +1943,6 @@ adw_about_window_new (void)
    return g_object_new (ADW_TYPE_ABOUT_WINDOW, NULL);
  }
  
 -/**
 - * adw_about_window_new_from_appdata:
 - * @resource_path: The resource to use
 - * @release_notes_version: (nullable): The version to retrieve release notes for
@@ -303,15 +597,15 @@
 -
 -  name = as_component_get_name (component);
 -  project_license = as_component_get_project_license (component);
 -  issue_url = as_component_get_url (component, AS_URL_KIND_BUGTRACKER);
 -  support_url = as_component_get_url (component, AS_URL_KIND_HELP);
 -  website_url = as_component_get_url (component, AS_URL_KIND_HOMEPAGE);
 -
--#if AS_CHECK_VERSION (1, 0, 0)
+-#if AS_CHECK_VERSION (0, 16, 4)
 -  developer_name = as_developer_get_name (as_component_get_developer (component));
 -#else
 -  developer_name = as_component_get_developer_name (component);
 -#endif
 -
 -  adw_about_window_set_application_icon (self, application_id);
 -
@@ -351,21 +645,21 @@
 -
 -  return GTK_WIDGET (self);
 -}
 -
  /**
   * adw_about_window_get_application_icon: (attributes org.gtk.Method.get_property=application-icon)
   * @self: an about window
-@@ -3389,42 +3207,3 @@
+@@ -3422,42 +3240,3 @@ adw_show_about_window (GtkWindow  *parent,
  
    gtk_window_present (GTK_WINDOW (window));
  }
 -
 -/**
-- * adw_show_about_window_from_appdata:
+- * adw_show_about_window_from_appdata: (skip)
 - * @parent: (nullable): the parent top-level window
 - * @resource_path: The resource to use
 - * @release_notes_version: (nullable): The version to retrieve release notes for
 - * @first_property_name: the name of the first property
 - * @...: value of first property, followed by more pairs of property name and
 - *   value, `NULL`-terminated
 - *
@@ -394,22 +688,231 @@
 -  va_end (var_args);
 -
 -  if (parent)
 -    gtk_window_set_transient_for (GTK_WINDOW (window), parent);
 -
 -  gtk_window_present (GTK_WINDOW (window));
 -}
-Index: tests/test-about-window.c
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
+diff --git a/src/adw-about-window.h b/src/adw-about-window.h
+index 79be5009..e6a041d4 100644
+--- a/src/adw-about-window.h
++++ b/src/adw-about-window.h
+@@ -25,10 +25,6 @@ G_DECLARE_FINAL_TYPE (AdwAboutWindow, adw_about_window, ADW, ABOUT_WINDOW, AdwWi
+ ADW_AVAILABLE_IN_1_2
+ GtkWidget *adw_about_window_new (void) G_GNUC_WARN_UNUSED_RESULT;
+ 
+-ADW_AVAILABLE_IN_1_4
+-GtkWidget *adw_about_window_new_from_appdata (const char *resource_path,
+-                                              const char *release_notes_version) G_GNUC_WARN_UNUSED_RESULT;
+-
+ ADW_AVAILABLE_IN_1_2
+ const char *adw_about_window_get_application_name (AdwAboutWindow *self);
+ ADW_AVAILABLE_IN_1_2
+@@ -174,13 +170,6 @@ void adw_about_window_add_legal_section (AdwAboutWindow *self,
+ ADW_AVAILABLE_IN_1_2
+ void adw_show_about_window (GtkWindow  *parent,
+                             const char *first_property_name,
+-                            ...) G_GNUC_NULL_TERMINATED;
+-
+-ADW_AVAILABLE_IN_1_4
+-void adw_show_about_window_from_appdata (GtkWindow  *parent,
+-                                         const char *resource_path,
+-                                         const char *release_notes_version,
+-                                         const char *first_property_name,
+-                                         ...) G_GNUC_NULL_TERMINATED;
++                            ...);
+ 
+ G_END_DECLS
+diff --git a/src/meson.build b/src/meson.build
+index aa71da24..5d7db8c4 100644
+--- a/src/meson.build
++++ b/src/meson.build
+@@ -283,20 +283,12 @@ gtk_min_version = '>= 4.13.4'
+ 
+ gio_dep = dependency('gio-2.0', version: glib_min_version)
+ gtk_dep = dependency('gtk4', version: gtk_min_version)
+-appstream_dep = dependency('appstream',
+-  fallback : ['appstream', 'appstream_dep'],
+-  default_options : [
+-    'systemd=false', 'apidocs=false', 'install-docs=false',
+-    'stemming=false', 'svg-support=false', 'gir=false',
+-  ],
+-)
+ 
+ libadwaita_deps = [
+   dependency('glib-2.0', version: glib_min_version),
+   dependency('fribidi'),
+   gio_dep,
+   gtk_dep,
+-  appstream_dep,
+   cc.find_library('m', required: false),
+ ]
+ 
+diff --git a/subprojects/appstream.wrap b/subprojects/appstream.wrap
+deleted file mode 100644
+index 4262a04b..00000000
+--- a/subprojects/appstream.wrap
++++ /dev/null
+@@ -1,5 +0,0 @@
+-[wrap-git]
+-directory = appstream
+-url = https://github.com/ximion/appstream.git
+-revision = main
+-depth = 1
+diff --git a/tests/meson.build b/tests/meson.build
+index a5312488..64bc27d0 100644
+--- a/tests/meson.build
++++ b/tests/meson.build
+@@ -2,13 +2,6 @@ if get_option('tests')
+ 
+ subdir('manual')
+ 
+-test_resources = gnome.compile_resources(
+-   'adwaita-test-resources',
+-   'tests.gresources.xml',
+-
+-   c_name: 'test',
+-)
+-
+ test_env = [
+   'G_TEST_SRCDIR=@0@'.format(meson.current_source_dir()),
+   'G_TEST_BUILDDIR=@0@'.format(meson.current_build_dir()),
+@@ -21,6 +14,7 @@ test_env = [
+ 
+ test_cflags = [
+   '-DADW_LOG_DOMAIN="Adwaita"',
++  '-DTEST_DATA_DIR="@0@/data"'.format(meson.current_source_dir()),
+ ]
+ 
+ test_link_args = []
+@@ -87,13 +81,7 @@ test_names = [
+ ]
+ 
+ foreach test_name : test_names
+-  test_sources = [
+-    test_name + '.c',
+-    test_resources,
+-    libadwaita_generated_headers
+-  ]
+-
+-  t = executable(test_name, test_sources,
++  t = executable(test_name, [test_name + '.c'] + libadwaita_generated_headers,
+                        c_args: test_cflags,
+                     link_args: test_link_args,
+                  dependencies: libadwaita_deps + [libadwaita_dep],
+diff --git a/tests/org.gnome.Adwaita1.Test.metainfo.xml b/tests/org.gnome.Adwaita1.Test.metainfo.xml
+deleted file mode 100644
+index 8b4af591..00000000
+--- a/tests/org.gnome.Adwaita1.Test.metainfo.xml
++++ /dev/null
+@@ -1,29 +0,0 @@
+-<?xml version="1.0" encoding="UTF-8"?>
+-<component type="desktop-application">
+-  <id>org.gnome.Adwaita1.Test</id>
+-  <metadata_license>CC0-1.0</metadata_license>
+-  <project_license>LGPL-2.1-or-later</project_license>
+-  <launchable type="desktop-id">org.gnome.Adwaita1.Test.desktop</launchable>
+-  <developer_name>The GNOME Project</developer_name>
+-
+-  <name>Adwaita Test</name>
+-
+-  <releases>
+-    <release version="1.0">
+-      <description>
+-        <p>Testing Build</p>
+-      </description>
+-    </release>
+-    <release version="0.1">
+-      <description>
+-        <p>Testing Build Older</p>
+-      </description>
+-    </release>
+-  </releases>
+-
+-  <project_group>GNOME</project_group>
+-
+-  <url type="homepage">https://gitlab.gnome.org/GNOME/libadwaita</url>
+-  <url type="bugtracker">https://gitlab.gnome.org/GNOME/libadwaita/issues</url>
+-  <url type="help">http://www.gnome.org/friends/</url>
+-</component>
+diff --git a/tests/test-about-dialog.c b/tests/test-about-dialog.c
+index 6c63aebf..f4577110 100644
+--- a/tests/test-about-dialog.c
++++ b/tests/test-about-dialog.c
+@@ -9,49 +9,6 @@
+ 
+ #include <adwaita.h>
+ 
+-#include "adwaita-test-resources.h"
+-
+-static void
+-test_adw_about_dialog_from_appdata (void)
+-{
+-  AdwAboutDialog *dialog = g_object_ref_sink (ADW_ABOUT_DIALOG (adw_about_dialog_new_from_appdata ("/org/gnome/Adwaita1/Test/org.gnome.Adwaita1.Test.metainfo.xml", "1.0")));
+-
+-  g_assert_nonnull (dialog);
+-
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes (dialog), ==, "<p>Testing Build</p>\n");
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes_version (dialog), ==, "1.0");
+-  g_assert_cmpstr (adw_about_dialog_get_version (dialog), ==, "1.0");
+-  g_assert_cmpstr (adw_about_dialog_get_application_icon (dialog), ==, "org.gnome.Adwaita1.Test");
+-  g_assert_cmpstr (adw_about_dialog_get_application_name (dialog), ==, "Adwaita Test");
+-  g_assert_cmpstr (adw_about_dialog_get_developer_name (dialog), ==, "The GNOME Project");
+-  g_assert_cmpstr (adw_about_dialog_get_issue_url (dialog), ==, "https://gitlab.gnome.org/GNOME/libadwaita/issues");
+-  g_assert_cmpstr (adw_about_dialog_get_support_url (dialog), ==, "http://www.gnome.org/friends/");
+-  g_assert_cmpstr (adw_about_dialog_get_website (dialog), ==, "https://gitlab.gnome.org/GNOME/libadwaita");
+-  g_assert_cmpuint (adw_about_dialog_get_license_type (dialog), ==, GTK_LICENSE_LGPL_2_1);
+-
+-  g_assert_finalize_object (dialog);
+-
+-  dialog = g_object_ref_sink (ADW_ABOUT_DIALOG (adw_about_dialog_new_from_appdata ("/org/gnome/Adwaita1/Test/org.gnome.Adwaita1.Test.metainfo.xml", "0.1")));
+-
+-  g_assert_nonnull (dialog);
+-
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes (dialog), ==, "<p>Testing Build Older</p>\n");
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes_version (dialog), ==, "0.1");
+-  g_assert_cmpstr (adw_about_dialog_get_version (dialog), ==, "1.0");
+-
+-  g_assert_finalize_object (dialog);
+-
+-  dialog = g_object_ref_sink (ADW_ABOUT_DIALOG (adw_about_dialog_new_from_appdata ("/org/gnome/Adwaita1/Test/org.gnome.Adwaita1.Test.metainfo.xml", NULL)));
+-
+-  g_assert_nonnull (dialog);
+-
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes (dialog), ==, "");
+-  g_assert_cmpstr (adw_about_dialog_get_release_notes_version (dialog), ==, "");
+-  g_assert_cmpstr (adw_about_dialog_get_version (dialog), ==, "1.0");
+-
+-  g_assert_finalize_object (dialog);
+-}
+-
+ static void
+ test_adw_about_dialog_create (void)
+ {
+@@ -144,16 +101,10 @@ int
+ main (int   argc,
+       char *argv[])
+ {
+-  GResource *test_resources;
+-
+   gtk_test_init (&argc, &argv, NULL);
+   adw_init ();
+ 
+-  test_resources = test_get_resource ();
+-  g_resources_register (test_resources);
+-
+   g_test_add_func ("/Adwaita/AboutDialog/create", test_adw_about_dialog_create);
+-  g_test_add_func ("/Adwaita/AboutDialog/from_appdata", test_adw_about_dialog_from_appdata);
+ 
+   return g_test_run ();
+ }
 diff --git a/tests/test-about-window.c b/tests/test-about-window.c
---- a/tests/test-about-window.c	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/tests/test-about-window.c	(date 1702739024467)
+index 1deda1ee..667a4443 100644
+--- a/tests/test-about-window.c
++++ b/tests/test-about-window.c
 @@ -8,49 +8,6 @@
  
  #include <adwaita.h>
  
 -#include "adwaita-test-resources.h"
 -
 -static void
@@ -452,15 +955,15 @@
 -
 -  g_assert_finalize_object (window);
 -}
 -
  static void
  test_adw_about_window_create (void)
  {
-@@ -143,16 +100,10 @@
+@@ -143,16 +100,10 @@ int
  main (int   argc,
        char *argv[])
  {
 -  GResource *test_resources;
 -
    gtk_test_init (&argc, &argv, NULL);
    adw_init ();
@@ -469,203 +972,22 @@
 -  g_resources_register (test_resources);
 -
    g_test_add_func ("/Adwaita/AboutWindow/create", test_adw_about_window_create);
 -  g_test_add_func ("/Adwaita/AboutWindow/from_appdata", test_adw_about_window_from_appdata);
  
    return g_test_run ();
  }
-Index: tests/meson.build
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/tests/meson.build b/tests/meson.build
---- a/tests/meson.build	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/tests/meson.build	(date 1702739024414)
-@@ -2,13 +2,6 @@
- 
- subdir('manual')
- 
--test_resources = gnome.compile_resources(
--   'adwaita-test-resources',
--   'tests.gresources.xml',
--
--   c_name: 'test',
--)
--
- test_env = [
-   'G_TEST_SRCDIR=@0@'.format(meson.current_source_dir()),
-   'G_TEST_BUILDDIR=@0@'.format(meson.current_build_dir()),
-@@ -21,6 +14,7 @@
- 
- test_cflags = [
-   '-DADW_LOG_DOMAIN="Adwaita"',
-+  '-DTEST_DATA_DIR="@0@/data"'.format(meson.current_source_dir()),
- ]
- 
- test_link_args = []
-@@ -83,13 +77,7 @@
- ]
- 
- foreach test_name : test_names
--  test_sources = [
--    test_name + '.c',
--    test_resources,
--    libadwaita_generated_headers
--  ]
--
--  t = executable(test_name, test_sources,
-+  t = executable(test_name, [test_name + '.c'] + libadwaita_generated_headers,
-                        c_args: test_cflags,
-                     link_args: test_link_args,
-                  dependencies: libadwaita_deps + [libadwaita_dep],
-Index: src/adw-about-window.h
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/src/adw-about-window.h b/src/adw-about-window.h
---- a/src/adw-about-window.h	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/src/adw-about-window.h	(date 1702739024348)
-@@ -25,10 +25,6 @@
- ADW_AVAILABLE_IN_1_2
- GtkWidget *adw_about_window_new (void) G_GNUC_WARN_UNUSED_RESULT;
- 
--ADW_AVAILABLE_IN_1_4
--GtkWidget *adw_about_window_new_from_appdata (const char *resource_path,
--                                              const char *release_notes_version) G_GNUC_WARN_UNUSED_RESULT;
--
- ADW_AVAILABLE_IN_1_2
- const char *adw_about_window_get_application_name (AdwAboutWindow *self);
- ADW_AVAILABLE_IN_1_2
-@@ -175,12 +171,5 @@
- void adw_show_about_window (GtkWindow  *parent,
-                             const char *first_property_name,
-                             ...);
--
--ADW_AVAILABLE_IN_1_4
--void adw_show_about_window_from_appdata (GtkWindow  *parent,
--                                         const char *resource_path,
--                                         const char *release_notes_version,
--                                         const char *first_property_name,
--                                         ...);
- 
- G_END_DECLS
-Index: demo/adwaita-demo.c
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/demo/adwaita-demo.c b/demo/adwaita-demo.c
---- a/demo/adwaita-demo.c	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/demo/adwaita-demo.c	(date 1702739024201)
-@@ -1,5 +1,3 @@
--#include "config.h"
--
- #include <glib/gi18n.h>
- #include <gtk/gtk.h>
- #include <adwaita.h>
-@@ -58,16 +56,24 @@
- 
-   debug_info = adw_demo_generate_debug_info ();
- 
--  about = adw_about_window_new_from_appdata ("/org/gnome/Adwaita1/Demo/org.gnome.Adwaita1.Demo.metainfo.xml", NULL);
--  gtk_window_set_transient_for (GTK_WINDOW (about), window);
--  adw_about_window_set_version (ADW_ABOUT_WINDOW (about), ADW_VERSION_S);
--  adw_about_window_set_debug_info (ADW_ABOUT_WINDOW (about), debug_info);
--  adw_about_window_set_debug_info_filename (ADW_ABOUT_WINDOW (about), "adwaita-1-demo-debug-info.txt");
--  adw_about_window_set_copyright (ADW_ABOUT_WINDOW (about), "© 2017–2022 Purism SPC");
--  adw_about_window_set_developers (ADW_ABOUT_WINDOW (about), developers);
--  adw_about_window_set_designers (ADW_ABOUT_WINDOW (about), designers);
--  adw_about_window_set_artists (ADW_ABOUT_WINDOW (about), designers);
--  adw_about_window_set_translator_credits (ADW_ABOUT_WINDOW (about), _("translator-credits"));
-+  about =
-+    g_object_new (ADW_TYPE_ABOUT_WINDOW,
-+                  "transient-for", window,
-+                  "application-icon", "org.gnome.Adwaita1.Demo",
-+                  "application-name", _("Adwaita Demo"),
-+                  "developer-name", _("The GNOME Project"),
-+                  "version", ADW_VERSION_S,
-+                  "website", "https://gitlab.gnome.org/GNOME/libadwaita",
-+                  "issue-url", "https://gitlab.gnome.org/GNOME/libadwaita/-/issues/new",
-+                  "debug-info", debug_info,
-+                  "debug-info-filename", "adwaita-1-demo-debug-info.txt",
-+                  "copyright", "© 2017–2022 Purism SPC",
-+                  "license-type", GTK_LICENSE_LGPL_2_1,
-+                  "developers", developers,
-+                  "designers", designers,
-+                  "artists", designers,
-+                  "translator-credits", _("translator-credits"),
-+                  NULL);
- 
-   adw_about_window_add_link (ADW_ABOUT_WINDOW (about),
-                              _("_Documentation"),
-Index: src/meson.build
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/src/meson.build b/src/meson.build
---- a/src/meson.build	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/src/meson.build	(date 1702739038248)
-@@ -271,20 +271,12 @@
- 
- gio_dep = dependency('gio-2.0', version: glib_min_version)
- gtk_dep = dependency('gtk4', version: gtk_min_version)
--appstream_dep = dependency('appstream',
--  fallback : ['appstream', 'appstream_dep'],
--  default_options : [
--    'systemd=false', 'apidocs=false', 'install-docs=false',
--    'stemming=false', 'svg-support=false', 'gir=false',
--  ],
--)
- 
- libadwaita_deps = [
-   dependency('glib-2.0', version: glib_min_version),
-   dependency('fribidi'),
-   gio_dep,
-   gtk_dep,
--  appstream_dep,
-   cc.find_library('m', required: false),
- ]
- 
-Index: demo/meson.build
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/demo/meson.build b/demo/meson.build
---- a/demo/meson.build	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/demo/meson.build	(date 1702739024229)
-@@ -3,7 +3,6 @@
- subdir('data')
- 
- demo_config_data = configuration_data()
--demo_config_data.set_quoted('ADW_METAINFO', appstream_file.full_path())
- demo_config_data.set_quoted('ADW_DEMO_VCS_TAG', '@VCS_TAG@')
- 
- demo_config_h = vcs_tag(
-@@ -19,8 +18,6 @@
-    'adwaita-demo.gresources.xml',
- 
-    c_name: 'adw',
--   dependencies: appstream_file,
--   source_dir: meson.current_build_dir(),
- )
- 
- adwaita_demo_sources = [
-Index: demo/adwaita-demo.gresources.xml
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/demo/adwaita-demo.gresources.xml b/demo/adwaita-demo.gresources.xml
---- a/demo/adwaita-demo.gresources.xml	(revision fd5892e94ddd9baf44dcfb2faaa97211a2532d6d)
-+++ b/demo/adwaita-demo.gresources.xml	(date 1702739024215)
-@@ -3,7 +3,6 @@
-   <gresource prefix="/org/gnome/Adwaita1/Demo">
-     <file preprocess="xml-stripblanks" alias="icons/scalable/apps/org.gnome.Adwaita1.Demo.svg">data/org.gnome.Adwaita1.Demo.svg</file>
-     <file preprocess="xml-stripblanks" alias="icons/symbolic/apps/org.gnome.Adwaita1.Demo-symbolic.svg">data/org.gnome.Adwaita1.Demo-symbolic.svg</file>
--    <file preprocess="xml-stripblanks" alias="org.gnome.Adwaita1.Demo.metainfo.xml">data/org.gnome.Adwaita1.Demo.metainfo.xml</file>
-     <file preprocess="xml-stripblanks">icons/scalable/actions/avatar-delete-symbolic.svg</file>
-     <file preprocess="xml-stripblanks">icons/scalable/actions/avatar-save-symbolic.svg</file>
-     <file preprocess="xml-stripblanks">icons/scalable/actions/clock-alarm-symbolic.svg</file>
+diff --git a/tests/tests.gresources.xml b/tests/tests.gresources.xml
+deleted file mode 100644
+index 23e90ea8..00000000
+--- a/tests/tests.gresources.xml
++++ /dev/null
+@@ -1,6 +0,0 @@
+-<?xml version="1.0" encoding="UTF-8"?>
+-<gresources>
+-  <gresource prefix="/org/gnome/Adwaita1/Test">
+-    <file compressed="true">org.gnome.Adwaita1.Test.metainfo.xml</file>
+-  </gresource>
+-</gresources>
+-- 
+2.44.0
+
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libcroco/mod.md` & `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libffi/fficonfig.h.meson` & `gvsbuild-2024.4.0/gvsbuild/patches/libffi/fficonfig.h.meson`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libffi/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libffi/meson_options.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/libffi/meson_options.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libffi/src/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/libffi/src/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/librsvg-legacy/vs2019-support.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/property.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/property.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/config.h` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/property.props` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libssh/mod.md` & `gvsbuild-2024.4.0/gvsbuild/patches/libssh/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libxml2/include/libxml/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/include/libxml/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libxml2/LICENSE.build` & `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libxml2/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/libxml2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/libyuv/001-win-build.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/libyuv/001-win-build.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/luajit/set-paths.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/luajit/set-paths.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln` & `gvsbuild-2024.4.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/certdata.txt` & `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/certdata.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl` & `gvsbuild-2024.4.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/pcre2/LICENSE.build` & `gvsbuild-2024.4.0/gvsbuild/patches/pcre2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/pcre2/meson.build` & `gvsbuild-2024.4.0/gvsbuild/patches/pcre2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/stack.props` & `gvsbuild-2024.4.0/gvsbuild/patches/stack.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/win-iconv/COPYING` & `gvsbuild-2024.4.0/gvsbuild/patches/win-iconv/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/x264/build/build.sh` & `gvsbuild-2024.4.0/gvsbuild/patches/x264/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch` & `gvsbuild-2024.4.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/__init__.py` & `gvsbuild-2024.4.0/gvsbuild/projects/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from gvsbuild.projects.cogl import Cogl
 from gvsbuild.projects.cyrus_sasl import CyrusSasl
 from gvsbuild.projects.dev_shell import DevShell
 from gvsbuild.projects.emeus import Emeus
 from gvsbuild.projects.enchant import Enchant
 from gvsbuild.projects.expat import Expat
 from gvsbuild.projects.ffmpeg import Ffmpeg, NvCodecHeaders
-from gvsbuild.projects.fontconfig import Fontconfig
 from gvsbuild.projects.freerdp import FreeRDP
 from gvsbuild.projects.freetype import Freetype
 from gvsbuild.projects.fribidi import Fribidi
 from gvsbuild.projects.gdk_pixbuf import GdkPixbuf
 from gvsbuild.projects.gettext import Gettext
-from gvsbuild.projects.glib import GLib, GLibNetworking, GLibPyWrapper
+from gvsbuild.projects.glib import GLib, GLibBase, GLibNetworking, GLibPyWrapper
 from gvsbuild.projects.glibmm import Glibmm
 from gvsbuild.projects.gobject_introspection import GObjectIntrospection
 from gvsbuild.projects.gperf import Gperf
 from gvsbuild.projects.graphene import Graphene
 from gvsbuild.projects.gsettings_desktop_schemas import GSettingsDesktopSchemas
 from gvsbuild.projects.gstreamer import (
     GstDevTools,
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/adwaita_icon_theme.py` & `gvsbuild-2024.4.0/gvsbuild/projects/adwaita_icon_theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,22 @@
 
 @project_add
 class AdwaitaIconTheme(Tarball, Meson):
     def __init__(self):
         Meson.__init__(
             self,
             "adwaita-icon-theme",
-            version="45.0",
+            version="46.0",
             repository="https://gitlab.gnome.org/GNOME/adwaita-icon-theme",
             archive_url="https://download.gnome.org/sources/adwaita-icon-theme/{major}/adwaita-icon-theme-{version}.tar.xz",
-            hash="2442bfb06f4e6cc95bf6e2682fdff98fa5eddc688751b9d6215c623cb4e42ff1",
+            hash="4bcb539bd75d64da385d6fa08cbaa9ddeaceb6ac8e82b85ba6c41117bf5ba64e",
             dependencies=[
                 "hicolor-icon-theme",
                 "librsvg",
             ],
-            patches=["001-fix-relative-cursor-path.patch"],
         )
 
     def build(self):
         Meson.build(self)
         # Work around for https://gitlab.gnome.org/GNOME/adwaita-icon-theme/-/issues/282
         self.builder.exec_msys(
             [
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/atk.py` & `gvsbuild-2024.4.0/gvsbuild/projects/atk.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/boringssl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/boringssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/cairo.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libffi.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,28 +11,24 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
-from gvsbuild.utils.base_project import project_add
+from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Cairo(Tarball, Meson):
+class Libffi(Tarball, Meson):
     def __init__(self):
-        Meson.__init__(
+        Project.__init__(
             self,
-            "cairo",
-            version="1.18.0",
-            lastversion_even=True,
-            archive_url="https://gitlab.freedesktop.org/cairo/cairo/-/archive/{version}/cairo-{version}.tar.gz",
-            hash="39a78afdc33a435c0f2ab53a5ec2a693c3c9b6d2ec9783ceecb2b94d54d942b0",
-            dependencies=["fontconfig", "freetype", "glib", "pixman", "libpng"],
-            patches=["0001-fix-alloca-unresolved.patch"],
+            "libffi",
+            version="3.4.6",
+            archive_url="https://github.com/libffi/libffi/releases/download/v{version}/libffi-{version}.tar.gz",
+            dependencies=["ninja", "meson"],
         )
-        self.add_param("-Dfreetype=enabled")
 
     def build(self):
-        Meson.build(self)
-        self.install(r".\COPYING share\doc\cairo")
+        Meson.build(self, meson_params="-Dtests=false")
+        self.install(r"LICENSE share\doc\libffi")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/cairomm.py` & `gvsbuild-2024.4.0/gvsbuild/projects/cairomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/check_libs.py` & `gvsbuild-2024.4.0/gvsbuild/projects/check_libs.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/clutter.py` & `gvsbuild-2024.4.0/gvsbuild/projects/clutter.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/cogl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/cogl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/cyrus_sasl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/cyrus_sasl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/dev_shell.py` & `gvsbuild-2024.4.0/gvsbuild/projects/dev_shell.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/emeus.py` & `gvsbuild-2024.4.0/gvsbuild/projects/emeus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/enchant.py` & `gvsbuild-2024.4.0/gvsbuild/projects/enchant.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/expat.py` & `gvsbuild-2024.4.0/gvsbuild/projects/expat.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/ffmpeg.py` & `gvsbuild-2024.4.0/gvsbuild/projects/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/fontconfig.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libadwaita.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,41 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Fontconfig(Tarball, Meson):
+class Libadwaita(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "fontconfig",
-            version="2.14.2",
+            "libadwaita",
+            repository="https://gitlab.gnome.org/GNOME/libadwaita",
+            version="1.5.0",
             lastversion_even=True,
-            repository="https://gitlab.freedesktop.org/fontconfig/fontconfig",
-            archive_url="https://www.freedesktop.org/software/fontconfig/release/fontconfig-{version}.tar.gz",
-            hash="3ba2dd92158718acec5caaf1a716043b5aa055c27b081d914af3ccb40dce8a55",
-            dependencies=["freetype", "gperf", "expat"],
+            archive_url="https://download.gnome.org/sources/libadwaita/{major}.{minor}/libadwaita-{version}.tar.xz",
+            hash="fd92287df9bb95c963654fb6e70d3e082e2bcb37b147e0e3c905567167993783",
+            dependencies=[
+                "ninja",
+                "meson",
+                "msys2",
+                "pkgconf",
+                "glib",
+                "gtk4",
+            ],
+            patches=[
+                "0001-remove-appstream-dependency.patch",
+            ],
         )
-        self.add_param("-Dtests=disabled")
+        gir = "disabled"
+        if self.opts.enable_gi:
+            self.add_dependency("gobject-introspection")
+            gir = "enabled"
 
-    def build(self):
+        self.add_param(f"-Dintrospection={gir}")
+        self.add_param("-Dgtk_doc=false")
+        self.add_param("-Dvapi=false")
+
+    def build(self, **kwargs):
         Meson.build(self)
-        self.install(r".\COPYING share\doc\fontconfig")
+        self.install(r".\COPYING share\doc\libadwaita")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/freerdp.py` & `gvsbuild-2024.4.0/gvsbuild/projects/freerdp.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/freetype.py` & `gvsbuild-2024.4.0/gvsbuild/projects/freetype.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/fribidi.py` & `gvsbuild-2024.4.0/gvsbuild/projects/fribidi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gdk_pixbuf.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gdk_pixbuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gettext.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gettext.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/glib.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gtksourceview.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,88 +10,62 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
-from gvsbuild.utils.base_expanders import NullExpander, Tarball
+from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class GLib(Tarball, Meson):
+class GtkSourceView4(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "glib",
-            version="2.78.4",
+            "gtksourceview4",
+            version="4.8.4",
+            lastversion_major=4,
             lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/glib",
-            archive_url="https://download.gnome.org/sources/glib/{major}.{minor}/glib-{version}.tar.xz",
-            hash="24b8e0672dca120cc32d394bccb85844e732e04fe75d18bb0573b2dbc7548f63",
-            dependencies=[
-                "ninja",
-                "meson",
-                "pkgconf",
-                "gettext",
-                "libffi",
-                "zlib",
-                "pcre2",
-            ],
-            patches=[
-                "001-glib-package-installation-directory.patch",
-                "002-python-312-distutils-to-packaging.patch",
-            ],
+            repository="https://gitlab.gnome.org/GNOME/gtksourceview",
+            archive_url="https://download.gnome.org/sources/gtksourceview/{major}.{minor}/gtksourceview-{version}.tar.xz",
+            hash="7ec9d18fb283d1f84a3a3eff3b7a72b09a10c9c006597b3fbabbb5958420a87d",
+            dependencies=["meson", "ninja", "gtk3", "pkgconf", "libxml2"],
         )
-        self.add_param("-Dman=false")
-        self.add_param("-Dtests=false")
-        self.add_param("-Dgtk_doc=false")
+        if Project.opts.enable_gi:
+            self.add_dependency("gobject-introspection")
+        else:
+            self.add_param("-Dgir=false")
+        self.add_param("-Dvapi=false")
 
     def build(self):
         Meson.build(self)
-        self.install(r".\LICENSES\* share\doc\glib")
+        self.install(r".\COPYING share\doc\gtksourceview4")
 
 
 @project_add
-class GLibNetworking(Tarball, Meson):
+class GtkSourceView5(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "glib-networking",
-            version="2.78.1",
+            "gtksourceview5",
+            version="5.12.0",
+            lastversion_major=5,
             lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/glib-networking",
-            archive_url="https://download.gnome.org/sources/glib-networking/{major}.{minor}/glib-networking-{version}.tar.xz",
-            hash="e48f2ddbb049832cbb09230529c5e45daca9f0df0eda325f832f7379859bf09f",
-            dependencies=[
-                "pkgconf",
-                "ninja",
-                "meson",
-                "glib",
-                "openssl",
-                "gsettings-desktop-schemas",
+            repository="https://gitlab.gnome.org/GNOME/gtksourceview",
+            archive_url="https://download.gnome.org/sources/gtksourceview/{major}.{minor}/gtksourceview-{version}.tar.xz",
+            hash="daf32ff5d3150d6385917d3503a85b9e047ba158b2b03079314c9c00813fa01f",
+            dependencies=["meson", "ninja", "gtk4", "pkgconf", "libxml2"],
+            patches=[
+                "001-fix-fontconfig-availability-check.patch",
             ],
         )
-
-    def build(self):
-        Meson.build(
-            self, meson_params="-Dgnutls=disabled -Dopenssl=enabled -Dlibproxy=disabled"
-        )
-        self.install(r".\COPYING share\doc\glib-networking")
-        self.install(r".\LICENSE_EXCEPTION share\doc\glib-networking")
-
-
-@project_add
-class GLibPyWrapper(NullExpander, Meson):
-    def __init__(self):
-        Project.__init__(
-            self,
-            "glib-py-wrapper",
-            dependencies=["glib"],
-            version="0.1.0",
-            internal=True,
-            repository="https://gitlab.gnome.org/GNOME/glib-py-wrapper",
-        )
+        if Project.opts.enable_gi:
+            self.add_dependency("gobject-introspection")
+        else:
+            self.add_param("-Dintrospection=disabled")
+        self.add_param("-Dvapi=false")
 
     def build(self):
         Meson.build(self)
+        self.install(r".\COPYING share\doc\gtksourceview5")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/glibmm.py` & `gvsbuild-2024.4.0/gvsbuild/projects/glibmm.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 @project_add
 class Glibmm(Tarball, Meson):
     def __init__(self):
         Meson.__init__(
             self,
             "glibmm",
             prj_dir="glibmm",
-            version="2.78.1",
+            version="2.80.0",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/glibmm",
             archive_url="https://download.gnome.org/sources/glibmm/{major}.{minor}/glibmm-{version}.tar.xz",
-            hash="f473f2975d26c3409e112ed11ed36406fb3843fa975df575c22d4cb843085f61",
+            hash="539b0a29e15a96676c4f0594541250566c5ca44da5d4d87a3732fa2d07909e4a",
             dependencies=[
                 "meson",
                 "ninja",
                 "libsigc++",
             ],
         )
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gobject_introspection.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gobject_introspection.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,28 +24,30 @@
 
 @project_add
 class GObjectIntrospection(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gobject-introspection",
-            version="1.78.1",
+            version="1.80.1",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gobject-introspection",
             archive_url="https://download.gnome.org/sources/gobject-introspection/{major}.{minor}/gobject-introspection-{version}.tar.xz",
-            hash="bd7babd99af7258e76819e45ba4a6bc399608fe762d83fde3cac033c50841bb4",
+            hash="a1df7c424e15bda1ab639c00e9051b9adf5cea1a9e512f8a603b53cd199bc6d8",
             dependencies=[
                 "ninja",
                 "meson",
                 "msys2",
                 "pkgconf",
-                "glib",
+                "glib-base",
+            ],
+            patches=[
+                # https://gitlab.gnome.org/GNOME/gobject-introspection/-/issues/427
+                "001-incorrect-giscanner-path.patch",
             ],
-            # https://gitlab.gnome.org/GNOME/gobject-introspection/-/issues/427
-            patches=["incorrect-giscanner-path.patch"],
         )
 
     def build(self):
         # For finding gobject-introspection.pc
         self.builder.mod_env("PKG_CONFIG_PATH", ".")
         # For finding & using girepository.lib/.dll
         self.builder.mod_env("LIB", r".\girepository")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gperf.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gperf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/graphene.py` & `gvsbuild-2024.4.0/gvsbuild/projects/graphene.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gsettings_desktop_schemas.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gsettings_desktop_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 @project_add
 class GSettingsDesktopSchemas(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gsettings-desktop-schemas",
-            version="45.0",
+            version="46.0",
             repository="https://gitlab.gnome.org/GNOME/gsettings-desktop-schemas",
             archive_url="https://download.gnome.org/sources/gsettings-desktop-schemas/{major}/gsettings-desktop-schemas-{version}.tar.xz",
-            hash="365c8d04daf79b38c8b3dc9626349a024f9e4befdd31fede74b42f7a9fbe0ae2",
+            hash="493a46a1161b6388d57aa72f632a79ce96c42d5ffbd1d0b00f496ec5876f8575",
             dependencies=["meson", "ninja", "pkgconf", "glib"],
         )
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "true"
         else:
             enable_gi = "false"
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gstreamer.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gstreamer.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gtk.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gtk.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,40 +118,44 @@
 @project_add
 class Gtk4(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gtk4",
             prj_dir="gtk4",
-            version="4.12.5",
+            version="4.14.1",
             lastversion_major=4,
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gtk",
             archive_url="https://download.gnome.org/sources/gtk/{major}.{minor}/gtk-{version}.tar.xz",
-            hash="28b356d590ee68ef626e2ef9820b2dd21441484a9a042a5a3f0c40e9dfc4f4f8",
+            hash="fcefb3f132f8cc4711a9efa5b353c9ae9bb5eeff0246fa74dbc2f2f839b9e308",
             dependencies=[
                 "gdk-pixbuf",
                 "pango",
                 "libepoxy",
                 "graphene",
                 "cairo",
                 "harfbuzz",
                 "glib",
                 "fribidi",
             ],
+            patches=[
+                "001-fix-pangoft2-file-not-found.patch",
+            ],
         )
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
             enable_gi = "disabled"
 
         self.add_param(f"-Dintrospection={enable_gi}")
         self.add_param("-Dbuild-tests=false")
         self.add_param("-Dbuild-demos=false")
         self.add_param("-Dbuild-examples=false")
         self.add_param("-Dmedia-gstreamer=disabled")
+        self.add_param("-Dvulkan=disabled")
 
     def build(self):
         Meson.build(self)
 
         self.install(r".\COPYING share\doc\gtk4")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gtkmm.py` & `gvsbuild-2024.4.0/gvsbuild/projects/gtkmm.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 @project_add
 class Gtkmm(Tarball, Meson):
     def __init__(self):
         Meson.__init__(
             self,
             "gtkmm",
             prj_dir="gtkmm",
-            version="4.12.0",
+            version="4.14.0",
             lastversion_major=4,
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gtkmm",
             archive_url="https://download.gnome.org/sources/gtkmm/{major}.{minor}/gtkmm-{version}.tar.xz",
-            hash="fbc3e7618123345c0148ef71abb6548d421f52bb224fbda34875b677dc032c92",
+            hash="9350a0444b744ca3dc69586ebd1b6707520922b6d9f4f232103ce603a271ecda",
             dependencies=[
                 "gdk-pixbuf",
                 "pangomm",
                 "glibmm",
                 "libepoxy",
                 "cairomm",
                 "gtk4",
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/gtksourceview.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libvpx.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,60 +9,73 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import Meson
+import os
+
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
+from gvsbuild.utils.utils import convert_to_msys
 
 
 @project_add
-class GtkSourceView4(Tarball, Meson):
+class Libvpx(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
-            "gtksourceview4",
-            version="4.8.4",
-            lastversion_major=4,
-            lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/gtksourceview",
-            archive_url="https://download.gnome.org/sources/gtksourceview/{major}.{minor}/gtksourceview-{version}.tar.xz",
-            hash="7ec9d18fb283d1f84a3a3eff3b7a72b09a10c9c006597b3fbabbb5958420a87d",
-            dependencies=["meson", "ninja", "gtk3", "pkgconf", "libxml2"],
+            "libvpx",
+            version="1.14.0",
+            archive_url="https://github.com/webmproject/libvpx/archive/v{version}.tar.gz",
+            archive_filename="libvpx-v{version}.tar.gz",
+            hash="5f21d2db27071c8a46f1725928a10227ae45c5cd1cad3727e4aafbe476e321fa",
+            dependencies=["nasm", "msys2", "libyuv", "perl"],
+            patches=[
+                "0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch",
+                "0001-Always-generate-pc-file.patch",
+            ],
         )
-        if Project.opts.enable_gi:
-            self.add_dependency("gobject-introspection")
-        else:
-            self.add_param("-Dgir=false")
-        self.add_param("-Dvapi=false")
 
     def build(self):
-        Meson.build(self)
-        self.install(r".\COPYING share\doc\gtksourceview4")
+        configure_options = (
+            "--enable-pic --as=nasm --disable-unit-tests --size-limit=16384x16384 "
+            "--enable-postproc --enable-multi-res-encoding --enable-temporal-denoising "
+            "--enable-vp9-temporal-denoising --enable-vp9-postproc --disable-tools "
+            "--disable-examples --disable-docs "
+        )
+        if self.builder.opts.configuration == "debug":
+            configure_options += "--enable-debug_libs"
 
+        target = "x86-win32-vs" if self.builder.x86 else "x86_64-win64-vs"
+        target += self.builder.opts.vs_ver
 
-@project_add
-class GtkSourceView5(Tarball, Meson):
-    def __init__(self):
-        Project.__init__(
-            self,
-            "gtksourceview5",
-            version="5.10.0",
-            lastversion_major=5,
-            lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/gtksourceview",
-            archive_url="https://download.gnome.org/sources/gtksourceview/{major}.{minor}/gtksourceview-{version}.tar.xz",
-            hash="b38a3010c34f59e13b05175e9d20ca02a3110443fec2b1e5747413801bc9c23f",
-            dependencies=["meson", "ninja", "gtk4", "pkgconf", "libxml2"],
+        msys_path = Project.get_tool_path("msys2")
+
+        self.exec_vs(
+            r"%s\bash ./configure --target=%s --prefix=%s %s"
+            % (
+                msys_path,
+                target,
+                convert_to_msys(self.builder.gtk_dir),
+                configure_options,
+            ),
+            add_path=msys_path,
         )
-        if Project.opts.enable_gi:
-            self.add_dependency("gobject-introspection")
-        else:
-            self.add_param("-Dintrospection=disabled")
-        self.add_param("-Dvapi=false")
+        self.exec_vs(r"make", add_path=msys_path)
+        self.exec_vs(r"make install", add_path=msys_path)
 
-    def build(self):
-        Meson.build(self)
-        self.install(r".\COPYING share\doc\gtksourceview5")
+        self.install(r".\LICENSE share\doc\libvpx")
+
+    def post_install(self):
+        # LibVPX generates a static library named 'vpxmd.lib' or 'vpxmdd.lib'
+        # in an unusual directory which is not the same as expected by the vpx.pc file
+        if self.builder.opts.configuration == "debug":
+            lib_name = "vpxmdd.lib"
+        else:
+            lib_name = "vpxmd.lib"
+        lib_path = f"Win32/{lib_name}" if self.builder.x86 else f"x64/{lib_name}"
+        self.builder.exec_msys(
+            ["mv", lib_path, "./vpx.lib"],
+            working_dir=os.path.join(self.builder.gtk_dir, "lib"),
+        )
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/harfbuzz.py` & `gvsbuild-2024.4.0/gvsbuild/projects/harfbuzz.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 @project_add
 class Harfbuzz(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "harfbuzz",
-            version="8.3.1",
+            version="8.4.0",
             archive_url="https://github.com/harfbuzz/harfbuzz/releases/download/{version}/harfbuzz-{version}.tar.xz",
-            hash="f73e1eacd7e2ffae687bc3f056bb0c705b7a05aee86337686e09da8fc1c2030c",
+            hash="af4ea73e25ab748c8c063b78c2f88e48833db9b2ac369e29bd115702e789755e",
             dependencies=["meson", "cmake", "freetype", "cairo", "pkgconf", "glib"],
         )
 
         if Project.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             self.add_param("-Dintrospection=enabled")
         else:
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/hello_world.py` & `gvsbuild-2024.4.0/gvsbuild/projects/hello_world.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/hicolor_icon_theme.py` & `gvsbuild-2024.4.0/gvsbuild/projects/hicolor_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/icu.py` & `gvsbuild-2024.4.0/gvsbuild/projects/icu.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/json_glib.py` & `gvsbuild-2024.4.0/gvsbuild/projects/json_glib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/jsonc.py` & `gvsbuild-2024.4.0/gvsbuild/projects/jsonc.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/leveldb.py` & `gvsbuild-2024.4.0/gvsbuild/projects/leveldb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/lgi.py` & `gvsbuild-2024.4.0/gvsbuild/projects/lgi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libadwaita.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libgxps.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libadwaita(Tarball, Meson):
+class Libgxps(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libadwaita",
-            repository="https://gitlab.gnome.org/GNOME/libadwaita",
-            version="1.4.4",
-            lastversion_even=True,
-            archive_url="https://download.gnome.org/sources/libadwaita/{major}.{minor}/libadwaita-{version}.tar.xz",
-            hash="f802b7d8d5ae33be4650ef571a580f144a806202a26f527dacd57d1560938828",
+            "libgxps",
+            version="0.3.2",
+            archive_url="https://download.gnome.org/sources/libgxps/{major}.{minor}/libgxps-{version}.tar.xz",
+            hash="6d27867256a35ccf9b69253eb2a88a32baca3b97d5f4ef7f82e3667fa435251c",
             dependencies=[
-                "ninja",
                 "meson",
-                "msys2",
+                "ninja",
                 "pkgconf",
                 "glib",
-                "gtk4",
-            ],
-            patches=[
-                "0001-remove-appstream-dependency.patch",
+                "libarchive",
+                "cairo",
+                "libpng",
+                "libjpeg-turbo",
+                "libtiff-4",
             ],
         )
-        gir = "disabled"
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
-            gir = "enabled"
+            disable_gi = "false"
+        else:
+            disable_gi = "true"
 
-        self.add_param(f"-Dintrospection={gir}")
-        self.add_param("-Dgtk_doc=false")
-        self.add_param("-Dvapi=false")
+        self.add_param(f"-Ddisable-introspection={disable_gi}")
+        self.add_param("-Dwith-liblcms2=false")
+        self.add_param("-Denable-test=false")
 
-    def build(self, **kwargs):
+    def build(self):
         Meson.build(self)
-        self.install(r".\COPYING share\doc\libadwaita")
+
+        self.install(r".\COPYING share\doc\libgxps")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libarchive.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libarchive.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libcbor.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libcbor.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libcroco.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libcroco.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libcurl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libcurl.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
 @project_add
 class Libcurl(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
             "libcurl",
-            version="8.6.0",
+            version="8.7.1",
             repository="https://github.com/curl/curl",
             archive_url="https://github.com/curl/curl/releases/download/curl-{major}_{minor}_{micro}/curl-{version}.tar.xz",
-            hash="3ccd55d91af9516539df80625f818c734dc6f2ecf9bada33c76765e99121db15",
+            hash="6fea2aac6a4610fbd0400afb0bcddbe7258a64c63f1f68e5855ebc0c659710cd",
             dependencies=[
                 "perl",
                 "cmake",
                 "ninja",
             ],
         )
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libepoxy.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libepoxy.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libffi.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libpsl.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,30 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libffi(Tarball, Meson):
+class Libpsl(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libffi",
-            version="3.4.6",
-            archive_url="https://github.com/libffi/libffi/releases/download/v{version}/libffi-{version}.tar.gz",
-            dependencies=["ninja", "meson"],
+            "libpsl",
+            version="0.21.5",
+            archive_url="https://github.com/rockdaboot/libpsl/releases/download/{version}/libpsl-{version}.tar.gz",
+            hash="1dcc9ceae8b128f3c0b3f654decd0e1e891afc6ff81098f227ef260449dae208",
+            dependencies=[
+                "meson",
+                "ninja",
+                "pkgconf",
+                "icu",
+            ],
         )
 
+        self.add_param("-Druntime=libicu")
+        self.add_param("-Dbuiltin=true")
+
     def build(self):
-        Meson.build(self, meson_params="-Dtests=false")
-        self.install(r"LICENSE share\doc\libffi")
+        Meson.build(self)
+
+        self.install(r".\LICENSE share\doc\libpsl")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libfido2.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libfido2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libgxps.py` & `gvsbuild-2024.4.0/gvsbuild/projects/wing.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,41 +15,22 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libgxps(Tarball, Meson):
+class Wing(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libgxps",
-            version="0.3.2",
-            archive_url="https://download.gnome.org/sources/libgxps/{major}.{minor}/libgxps-{version}.tar.xz",
-            hash="6d27867256a35ccf9b69253eb2a88a32baca3b97d5f4ef7f82e3667fa435251c",
-            dependencies=[
-                "meson",
-                "ninja",
-                "pkgconf",
-                "glib",
-                "libarchive",
-                "cairo",
-                "libpng",
-                "libjpeg-turbo",
-                "libtiff-4",
-            ],
+            "wing",
+            version="0.3.18",
+            repository="https://gitlab.gnome.org/GNOME/wing",
+            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
+            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
+            dependencies=["ninja", "meson", "pkgconf", "glib"],
         )
-        if self.opts.enable_gi:
-            self.add_dependency("gobject-introspection")
-            disable_gi = "false"
-        else:
-            disable_gi = "true"
-
-        self.add_param(f"-Ddisable-introspection={disable_gi}")
-        self.add_param("-Dwith-liblcms2=false")
-        self.add_param("-Denable-test=false")
 
     def build(self):
         Meson.build(self)
-
-        self.install(r".\COPYING share\doc\libgxps")
+        self.install(r".\COPYING share\doc\wing")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libjpeg_turbo.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libjpeg_turbo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libmicrohttpd.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libmicrohttpd.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libpng.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libpng.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libpsl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/openh264.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,30 +15,26 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libpsl(Tarball, Meson):
+class OpenH264(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libpsl",
-            version="0.21.5",
-            archive_url="https://github.com/rockdaboot/libpsl/releases/download/{version}/libpsl-{version}.tar.gz",
-            hash="1dcc9ceae8b128f3c0b3f654decd0e1e891afc6ff81098f227ef260449dae208",
+            "openh264",
+            version="2.4.1",
+            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
+            archive_filename="openh264-{version}.tar.gz",
+            hash="8ffbe944e74043d0d3fb53d4a2a14c94de71f58dbea6a06d0dc92369542958ea",
             dependencies=[
-                "meson",
                 "ninja",
-                "pkgconf",
-                "icu",
+                "meson",
+                "nasm",
             ],
         )
 
-        self.add_param("-Druntime=libicu")
-        self.add_param("-Dbuiltin=true")
-
     def build(self):
         Meson.build(self)
-
-        self.install(r".\LICENSE share\doc\libpsl")
+        self.install(r"LICENSE share\doc\openh264")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/librsvg.py` & `gvsbuild-2024.4.0/gvsbuild/projects/librsvg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libsigcplusplus.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libsigcplusplus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libsoup.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libsoup.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libssh.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libssh.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libtiff.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libtiff.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libuv.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libvorbis.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libvorbis.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libvpx.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pygobject.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,74 +8,53 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
+import sys
+from pathlib import Path
 
-import os
-
+from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
-from gvsbuild.utils.utils import convert_to_msys
 
 
 @project_add
-class Libvpx(Tarball, Project):
+class PyGObject(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libvpx",
-            version="1.14.0",
-            archive_url="https://github.com/webmproject/libvpx/archive/v{version}.tar.gz",
-            archive_filename="libvpx-v{version}.tar.gz",
-            hash="5f21d2db27071c8a46f1725928a10227ae45c5cd1cad3727e4aafbe476e321fa",
-            dependencies=["nasm", "msys2", "libyuv", "perl"],
+            "pygobject",
+            version="3.48.1",
+            lastversion_even=True,
+            repository="https://gitlab.gnome.org/GNOME/pygobject",
+            archive_url="https://download.gnome.org/sources/pygobject/{major}.{minor}/pygobject-{version}.tar.xz",
+            hash="3a0a2c0c0f25931b5840649c54834b9e58a63148d37fa9f6308887b7027e15c2",
+            dependencies=["pycairo", "gobject-introspection", "libffi"],
             patches=[
-                "0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch",
-                "0001-Always-generate-pc-file.patch",
+                "001-pygobject-py38-load-dll.patch",
             ],
         )
 
     def build(self):
-        configure_options = (
-            "--enable-pic --as=nasm --disable-unit-tests --size-limit=16384x16384 "
-            "--enable-postproc --enable-multi-res-encoding --enable-temporal-denoising "
-            "--enable-vp9-temporal-denoising --enable-vp9-postproc --disable-tools "
-            "--disable-examples --disable-docs "
-        )
-        if self.builder.opts.configuration == "debug":
-            configure_options += "--enable-debug_libs"
-
-        target = "x86-win32-vs" if self.builder.x86 else "x86_64-win64-vs"
-        target += self.builder.opts.vs_ver
-
-        msys_path = Project.get_tool_path("msys2")
-
-        self.exec_vs(
-            r"%s\bash ./configure --target=%s --prefix=%s %s"
-            % (
-                msys_path,
-                target,
-                convert_to_msys(self.builder.gtk_dir),
-                configure_options,
-            ),
-            add_path=msys_path,
-        )
-        self.exec_vs(r"make", add_path=msys_path)
-        self.exec_vs(r"make install", add_path=msys_path)
-
-        self.install(r".\LICENSE share\doc\libvpx")
-
-    def post_install(self):
-        # LibVPX generates a static library named 'vpxmd.lib' or 'vpxmdd.lib'
-        # in an unusual directory which is not the same as expected by the vpx.pc file
-        if self.builder.opts.configuration == "debug":
-            lib_name = "vpxmdd.lib"
-        else:
-            lib_name = "vpxmd.lib"
-        lib_path = f"Win32/{lib_name}" if self.builder.x86 else f"x64/{lib_name}"
-        self.builder.exec_msys(
-            ["mv", lib_path, "./vpx.lib"],
-            working_dir=os.path.join(self.builder.gtk_dir, "lib"),
-        )
+        py_dir = Path(sys.executable).parent
+        Meson.build(self, meson_params=f'-Dpython="{py_dir}\\python.exe"')
+        gtk_dir = self.builder.gtk_dir
+        add_inc = [
+            str(Path(gtk_dir) / "include" / "cairo"),
+            str(Path(gtk_dir) / "include" / "gobject-introspection-1.0"),
+            str(Path(gtk_dir) / "include" / "glib-2.0"),
+            str(Path(gtk_dir) / "lib" / "glib-2.0" / "include"),
+        ]
+        self.builder.mod_env("INCLUDE", ";".join(add_inc))
+        if self.builder.opts.py_wheel:
+            self.exec_vs(r"%(python_dir)s\python.exe -m build --wheel")
+            dist_dir = Path(self.build_dir) / "dist"
+            for path in dist_dir.rglob("*.whl"):
+                self.exec_vs(
+                    r"%(python_dir)s\python.exe -m pip install --force-reinstall "
+                    + str(path)
+                )
+                self.install_dir("dist", "python")
+        self.install(r".\COPYING share\doc\pygobject")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libxml2.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libxml2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libyuv.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libyuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/libzip.py` & `gvsbuild-2024.4.0/gvsbuild/projects/libzip.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/lmdb.py` & `gvsbuild-2024.4.0/gvsbuild/projects/lmdb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/luajit.py` & `gvsbuild-2024.4.0/gvsbuild/projects/luajit.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/lz4.py` & `gvsbuild-2024.4.0/gvsbuild/projects/lz4.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/mit_kerberos.py` & `gvsbuild-2024.4.0/gvsbuild/projects/mit_kerberos.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/nghttp2.py` & `gvsbuild-2024.4.0/gvsbuild/projects/nghttp2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/ogg.py` & `gvsbuild-2024.4.0/gvsbuild/projects/ogg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/openh264.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pixman.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class OpenH264(Tarball, Meson):
+class Pixman(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "openh264",
-            version="2.4.1",
-            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
-            archive_filename="openh264-{version}.tar.gz",
-            hash="8ffbe944e74043d0d3fb53d4a2a14c94de71f58dbea6a06d0dc92369542958ea",
-            dependencies=[
-                "ninja",
-                "meson",
-                "nasm",
-            ],
+            "pixman",
+            repository="https://gitlab.freedesktop.org/pixman/pixman",
+            version="0.42.2",
+            lastversion_even=True,
+            archive_url="http://cairographics.org/releases/pixman-{version}.tar.gz",
+            hash="ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e",
+            dependencies=["ninja", "meson"],
         )
 
     def build(self):
-        Meson.build(self)
-        self.install(r"LICENSE share\doc\openh264")
+        enable_mmx = "disabled" if self.builder.x64 else "enabled"
+        Meson.build(
+            self,
+            meson_params=f"-Dsse2=enabled -Dssse3=enabled -Dmmx={enable_mmx} -Dtests=disabled",
+        )
+
+        self.install(r".\COPYING share\doc\pixman")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/openssl.py` & `gvsbuild-2024.4.0/gvsbuild/projects/openssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/opus.py` & `gvsbuild-2024.4.0/gvsbuild/projects/opus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pango.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pango.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,36 @@
 
 @project_add
 class Pango(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "pango",
-            version="1.52.1",
+            version="1.52.2",
             repository="https://gitlab.gnome.org/GNOME/pango",
             archive_url="https://download.gnome.org/sources/pango/{major}.{minor}/pango-{version}.tar.xz",
-            hash="58728a0a2d86f60761208df9493033d18ecb2497abac80ee1a274ad0c6e55f0f",
+            hash="d0076afe01082814b853deec99f9349ece5f2ce83908b8e58ff736b41f78a96b",
             dependencies=[
                 "ninja",
                 "meson",
+                "freetype",
                 "cairo",
                 "harfbuzz",
                 "fribidi",
             ],
             patches=[
-                "001-fix-double-free-crash.patch",
+                "002-fix-wrong-usage-gweakref.patch",
+                "003-remove-extra-hb-face-font.patch",
             ],
         )
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
             enable_gi = "disabled"
 
         self.add_param(f"-Dintrospection={enable_gi}")
+        self.add_param("-Dfreetype=enabled")
 
     def build(self):
         Meson.build(self)
         self.install(r"COPYING share\doc\pango")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pangomm.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pangomm.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 @project_add
 class Pangomm(Tarball, Meson):
     def __init__(self):
         Meson.__init__(
             self,
             "pangomm",
             prj_dir="pangomm",
-            version="2.50.2",
+            version="2.52.0",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/pangomm",
             archive_url="https://download.gnome.org/sources/pangomm/{major}.{minor}/pangomm-{version}.tar.xz",
-            hash="1bc5ab4ea3280442580d68318226dab36ceedfc3288f9d83711cf7cfab50a9fb",
+            hash="34a134126a6484ff12f774358c36ecc44d0e9df094e1b83796d9774bb7d24947",
             dependencies=[
                 "meson",
                 "ninja",
                 "libsigc++",
                 "cairomm",
                 "pango",
                 "glibmm",
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pcre2.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pcre2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pixman.py` & `gvsbuild-2024.4.0/gvsbuild/projects/cairo.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,32 +11,29 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
-from gvsbuild.utils.base_project import Project, project_add
+from gvsbuild.utils.base_project import project_add
 
 
 @project_add
-class Pixman(Tarball, Meson):
+class Cairo(Tarball, Meson):
     def __init__(self):
-        Project.__init__(
+        Meson.__init__(
             self,
-            "pixman",
-            repository="https://gitlab.freedesktop.org/pixman/pixman",
-            version="0.42.2",
+            "cairo",
+            version="1.18.0",
             lastversion_even=True,
-            archive_url="http://cairographics.org/releases/pixman-{version}.tar.gz",
-            hash="ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e",
-            dependencies=["ninja", "meson"],
+            archive_url="https://gitlab.freedesktop.org/cairo/cairo/-/archive/{version}/cairo-{version}.tar.gz",
+            hash="39a78afdc33a435c0f2ab53a5ec2a693c3c9b6d2ec9783ceecb2b94d54d942b0",
+            dependencies=["freetype", "glib", "pixman", "libpng"],
+            patches=["0001-fix-alloca-unresolved.patch"],
         )
+        self.add_param("-Dfreetype=enabled")
+        self.add_param("-Dfontconfig=disabled")
 
     def build(self):
-        enable_mmx = "disabled" if self.builder.x64 else "enabled"
-        Meson.build(
-            self,
-            meson_params=f"-Dsse2=enabled -Dssse3=enabled -Dmmx={enable_mmx} -Dtests=disabled",
-        )
-
-        self.install(r".\COPYING share\doc\pixman")
+        Meson.build(self)
+        self.install(r".\COPYING share\doc\cairo")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pkgconf.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pkgconf.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 @project_add
 class PkgConf(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "pkgconf",
             prj_dir="pkgconf",
-            version="2.1.1",
+            version="2.2.0",
             archive_url="https://distfiles.ariadne.space/pkgconf/pkgconf-{version}.tar.gz",
-            hash="1a00b7fa08c7b506a24c40f7cc8d9e0e59be748d731af8f7aa0b4d722bd8ccbe",
+            hash="28f8dfc279a10ef66148befa3f6eb266e5f3570316600208ed50e9781c7269d8",
             dependencies=["ninja", "meson"],
             patches=["0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch"],
         )
         self.add_param("-Dtests=disabled")
 
     def build(self):
         Meson.build(self)
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/protobuf.py` & `gvsbuild-2024.4.0/gvsbuild/projects/protobuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pycairo.py` & `gvsbuild-2024.4.0/gvsbuild/projects/pycairo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/pygobject.py` & `gvsbuild-2024.4.0/gvsbuild/projects/x264.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,53 +8,58 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
-import sys
-from pathlib import Path
 
-from gvsbuild.utils.base_builders import Meson
-from gvsbuild.utils.base_expanders import Tarball
+import os
+
+from gvsbuild.utils.base_expanders import GitRepo
 from gvsbuild.utils.base_project import Project, project_add
+from gvsbuild.utils.utils import convert_to_msys
 
 
 @project_add
-class PyGObject(Tarball, Meson):
+class X264(GitRepo, Project):
     def __init__(self):
         Project.__init__(
             self,
-            "pygobject",
-            version="3.48.0",
-            lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/pygobject",
-            archive_url="https://download.gnome.org/sources/pygobject/{major}.{minor}/pygobject-{version}.tar.xz",
-            hash="e6aa8dd78284905ad8cad0f7be8cd59e6ab453b7b48803d0d70ecb8db5faea76",
-            dependencies=["pycairo", "gobject-introspection", "libffi"],
+            "x264",
+            repo_url="http://git.videolan.org/git/x264.git",
+            fetch_submodules=False,
+            dependencies=["nasm", "msys2"],
+            tag="31e19f92f00c7003fa115047ce50978bc98c3a0d",
             patches=[
-                "001-pygobject-py38-load-dll.patch",
+                "x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch",
             ],
         )
 
     def build(self):
-        py_dir = Path(sys.executable).parent
-        Meson.build(self, meson_params=f'-Dpython="{py_dir}\\python.exe"')
-        gtk_dir = self.builder.gtk_dir
-        add_inc = [
-            str(Path(gtk_dir) / "include" / "cairo"),
-            str(Path(gtk_dir) / "include" / "gobject-introspection-1.0"),
-            str(Path(gtk_dir) / "include" / "glib-2.0"),
-            str(Path(gtk_dir) / "lib" / "glib-2.0" / "include"),
-        ]
-        self.builder.mod_env("INCLUDE", ";".join(add_inc))
-        if self.builder.opts.py_wheel:
-            self.exec_vs(r"%(python_dir)s\python.exe -m build --wheel")
-            dist_dir = Path(self.build_dir) / "dist"
-            for path in dist_dir.rglob("*.whl"):
-                self.exec_vs(
-                    r"%(python_dir)s\python.exe -m pip install --force-reinstall "
-                    + str(path)
-                )
-                self.install_dir("dist", "python")
-        self.install(r".\COPYING share\doc\pygobject")
+        configuration = (
+            "debug-optimized"
+            if self.opts.release_configuration_is_actually_debug_optimized
+            else self.opts.configuration
+        )
+        msys_path = Project.get_tool_path("msys2")
+        self.exec_vs(
+            r"%s\bash build\build.sh %s %s"
+            % (
+                msys_path,
+                convert_to_msys(self.builder.gtk_dir),
+                configuration,
+            ),
+            add_path=msys_path,
+        )
+
+        # use the path expected when building with a dependent project
+        self.builder.exec_msys(
+            ["mv", "libx264.dll.lib", "libx264.lib"],
+            working_dir=os.path.join(self.builder.gtk_dir, "lib"),
+        )
+
+        if configuration in ["debug-optimized", "debug"]:
+            self.install(r".\libx264-164.pdb bin")
+            self.install(r".\x264.pdb bin")
+
+        self.install(r".\COPYING share\doc\x264")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/sqlite.py` & `gvsbuild-2024.4.0/gvsbuild/projects/sqlite.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/win_iconv.py` & `gvsbuild-2024.4.0/gvsbuild/projects/win_iconv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/projects/wing.py` & `gvsbuild-2024.4.0/gvsbuild/projects/zlib.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,29 +8,53 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
+#
+#  This program is free software; you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation; either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Wing(Tarball, Meson):
+class Zlib(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
-            "wing",
-            version="0.3.18",
-            repository="https://gitlab.gnome.org/GNOME/wing",
-            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
-            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
-            dependencies=["ninja", "meson", "pkgconf", "glib"],
+            "zlib",
+            version="1.3.1",
+            archive_url="https://github.com/madler/zlib/releases/download/v{version}/zlib-{version}.tar.xz",
+            hash="38ef96b8dfe510d42707d9c781877914792541133e1870841463bfa73f883e32",
+            patches=[],
         )
 
     def build(self):
-        Meson.build(self)
-        self.install(r".\COPYING share\doc\wing")
+        options = ""
+        if self.builder.opts.configuration == "debug":
+            options = 'CFLAGS="-nologo -MDd -W3 -Od -Zi -Fd\\"zlib\\""'
+
+        self.exec_vs(
+            r"nmake /nologo /f win32\Makefile.msc STATICLIB=zlib-static.lib IMPLIB=zlib1.lib "
+            + options
+        )
+
+        self.install(r".\zlib.h .\zconf.h include")
+        self.install(r".\zlib1.dll .\zlib1.pdb bin")
+        self.install(r".\zlib1.lib lib")
+
+        self.install_pc_files()
+        self.install(r".\README share\doc\zlib")
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/tools.py` & `gvsbuild-2024.4.0/gvsbuild/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @tool_add
 class ToolCargo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "cargo",
-            version="1.77.0",
+            version="1.77.1",
             repository="rust-lang/rust",
             archive_url="https://win.rustup.rs/x86_64",
             archive_filename="rustup-init.exe",
             exe_name="cargo.exe",
         )
 
     def load_defaults(self):
```

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/base_builders.py` & `gvsbuild-2024.4.0/gvsbuild/utils/base_builders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/base_expanders.py` & `gvsbuild-2024.4.0/gvsbuild/utils/base_expanders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/base_group.py` & `gvsbuild-2024.4.0/gvsbuild/utils/base_group.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/base_project.py` & `gvsbuild-2024.4.0/gvsbuild/utils/base_project.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/base_tool.py` & `gvsbuild-2024.4.0/gvsbuild/utils/base_tool.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/builder.py` & `gvsbuild-2024.4.0/gvsbuild/utils/builder.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/simple_ui.py` & `gvsbuild-2024.4.0/gvsbuild/utils/simple_ui.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/gvsbuild/utils/utils.py` & `gvsbuild-2024.4.0/gvsbuild/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         func(path)
         log.debug(f"rmtree:read-only file/path ({path})")
     else:
         raise
 
 
 def rmtree_full(dest_dir, retry=False):
+    if not os.path.isdir(dest_dir):
+        return
     if retry:
         for delay in [0.1, 0.2, 0.4, 0.8]:
             try:
                 shutil.rmtree(dest_dir, onerror=_rmtree_error_handler)
                 break
             except OSError:
                 # wait a little, don't ask me why ;(
```

### Comparing `gvsbuild-2024.3.1/pyproject.toml` & `gvsbuild-2024.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "gvsbuild"
-version = "2024.3.1"
+version = "2024.4.0"
 description = "GTK stack for Windows"
 authors = ["Ignacio Casal Quinteiro <qignacio@amazon.com>", "Dan Yeaw <dan@yeaw.me>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Build Tools",
     "Environment :: X11 Applications :: GTK",
     "Operating System :: Microsoft :: Windows",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-build = ">=0.9,<1.2"
+build = ">=0.9,<1.3"
 lastversion = { version = ">=2.4.2,<4.0.0", optional = true }
 packaging = { version = ">=21.3,<25.0", optional = true }
-typer = {extras = ["all"], version = ">=0.6.1,<0.11.0"}
+typer = {extras = ["all"], version = ">=0.6.1,<0.13.0"}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.1"
 pytest = ">=7.1.3,<9.0.0"
 tox = "^4.1.2"
 
 [tool.poetry.extras]
```

### Comparing `gvsbuild-2024.3.1/README.md` & `gvsbuild-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.3.1/PKG-INFO` & `gvsbuild-2024.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvsbuild
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: GTK stack for Windows
 License: GPL-2.0-only
 Author: Ignacio Casal Quinteiro
 Author-email: qignacio@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: outdated
-Requires-Dist: build (>=0.9,<1.2)
+Requires-Dist: build (>=0.9,<1.3)
 Requires-Dist: lastversion (>=2.4.2,<4.0.0) ; extra == "outdated"
 Requires-Dist: packaging (>=21.3,<25.0) ; extra == "outdated"
-Requires-Dist: typer[all] (>=0.6.1,<0.11.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 # gvsbuild
 
 ![CI](https://github.com/wingtk/gvsbuild/actions/workflows/ci.yml/badge.svg)
 
 This python script helps you build a full [GTK](https://www.gtk.org/) library
```


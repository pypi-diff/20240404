# Comparing `tmp/lightning-pose-1.2.2.tar.gz` & `tmp/lightning-pose-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-pose-1.2.2.tar", last modified: Mon Apr  1 21:48:35 2024, max compression
+gzip compressed data, was "lightning-pose-1.2.3.tar", last modified: Thu Apr  4 18:45:04 2024, max compression
```

## Comparing `lightning-pose-1.2.2.tar` & `lightning-pose-1.2.3.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.945308 lightning-pose-1.2.2/
--rw-r--r--   0 mattw     (1000) mattw     (1000)      751 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/Dockerfile.cuda11
--rw-r--r--   0 mattw     (1000) mattw     (1000)      564 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/Dockerfile.cuda12
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1069 2021-10-12 16:17:39.000000 lightning-pose-1.2.2/LICENSE
--rw-r--r--   0 mattw     (1000) mattw     (1000)      389 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/MANIFEST.in
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     2711 2024-04-01 21:48:35.945308 lightning-pose-1.2.2/PKG-INFO
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     2293 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/README.md
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.905307 lightning-pose-1.2.2/data/
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.909308 lightning-pose-1.2.2/data/mirror-mouse-example/
--rw-r--r--   0 mattw     (1000) mattw     (1000)    23291 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/CollectedData.csv
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.925308 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58061 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img00.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58061 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img01.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58823 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img02.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61321 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img03.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60514 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img04.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58845 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img05.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59644 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img06.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59770 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img07.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62981 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img08.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59896 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img09.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60176 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img10.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59447 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img11.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59594 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img12.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56872 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img13.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60321 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img14.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56750 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img15.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58859 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img16.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59711 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img17.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58963 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img18.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62030 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img19.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57946 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img20.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58369 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img21.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57289 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img22.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58406 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img23.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61508 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img24.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    55197 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img25.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61129 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img26.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59406 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img27.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58022 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img28.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60939 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img29.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59418 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img30.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57690 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img31.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61011 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img32.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61344 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img33.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59423 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img34.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58590 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img35.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58634 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img36.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59459 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img37.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60221 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img38.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59427 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img39.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59695 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img40.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59000 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img41.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56997 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img42.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56691 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img43.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56210 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img44.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58659 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img45.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58772 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img46.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57162 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img47.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58633 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img48.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59179 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img49.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58090 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img50.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59679 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img51.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60383 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img52.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58368 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img53.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56150 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img54.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58609 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img55.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57972 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img56.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56140 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img57.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58368 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img58.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59631 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img59.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57544 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img60.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56942 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img61.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58647 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img62.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58314 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img63.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59191 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img64.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58908 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img65.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57875 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img66.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59113 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img67.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61882 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img68.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58659 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img69.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58569 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img70.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58122 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img71.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57775 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img72.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57577 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img73.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60838 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img74.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59679 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img75.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59493 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img76.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60714 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img77.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57643 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img78.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59165 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img79.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58122 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img80.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58643 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img81.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57999 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img82.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62707 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img83.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    63460 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img84.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57620 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img85.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57186 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img86.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59946 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img87.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61352 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img88.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60565 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img89.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img90.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img91.png
--rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img92.png
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.925308 lightning-pose-1.2.2/data/mirror-mouse-example/videos/
--rw-r--r--   0 mattw     (1000) mattw     (1000)  1724850 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/data/mirror-mouse-example/videos/test_vid.mp4
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.925308 lightning-pose-1.2.2/docs/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6250 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/docs/README.md
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1298 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/docs/roadmap.md
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.925308 lightning-pose-1.2.2/lightning_pose/
--rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2022-02-01 19:50:48.000000 lightning-pose-1.2.2/lightning_pose/__init__.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/apps/
--rw-r--r--   0 mattw     (1000) mattw     (1000)    10743 2024-03-26 14:09:27.000000 lightning-pose-1.2.2/lightning_pose/apps/labeled_frame_diagnostics.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)     8707 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/lightning_pose/apps/plots.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)     8197 2024-03-26 14:09:27.000000 lightning-pose-1.2.2/lightning_pose/apps/utils.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)     7796 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/lightning_pose/apps/video_diagnostics.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1603 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/callbacks.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/data/
--rw-r--r--   0 mattw     (1000) mattw     (1000)      194 2023-03-06 14:42:52.000000 lightning-pose-1.2.2/lightning_pose/data/__init__.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     3937 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/data/augmentations.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    15050 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/data/dali.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     9305 2024-03-28 21:36:39.000000 lightning-pose-1.2.2/lightning_pose/data/datamodules.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    14144 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/data/datasets.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    20100 2024-03-28 17:59:46.000000 lightning-pose-1.2.2/lightning_pose/data/utils.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/losses/
--rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2022-02-01 19:50:48.000000 lightning-pose-1.2.2/lightning_pose/losses/__init__.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     2755 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/losses/factory.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1436 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/losses/helpers.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    29899 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/losses/losses.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6413 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/metrics.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/models/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)      626 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/__init__.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/models/backbones/
--rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/lightning_pose/models/backbones/__init__.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6253 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/backbones/torchvision.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4615 2024-03-29 17:58:38.000000 lightning-pose-1.2.2/lightning_pose/models/backbones/vit_img_encoder.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     3235 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/backbones/vits.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    17706 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/base.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    17062 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/heatmap_tracker.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    19105 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/heatmap_tracker_mhcrnn.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     8290 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/models/regression_tracker.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.929308 lightning-pose-1.2.2/lightning_pose/utils/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)      719 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/utils/__init__.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    11001 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/utils/fiftyone.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     7705 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/utils/io.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    15483 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/utils/pca.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    31356 2024-04-01 20:58:09.000000 lightning-pose-1.2.2/lightning_pose/utils/predictions.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    24957 2024-03-28 17:59:50.000000 lightning-pose-1.2.2/lightning_pose/utils/scripts.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1580 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/lightning_pose/utils/tests.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.925308 lightning-pose-1.2.2/lightning_pose.egg-info/
--rw-r--r--   0 mattw     (1000) mattw     (1000)     2711 2024-04-01 21:48:35.000000 lightning-pose-1.2.2/lightning_pose.egg-info/PKG-INFO
--rw-r--r--   0 mattw     (1000) mattw     (1000)     7027 2024-04-01 21:48:35.000000 lightning-pose-1.2.2/lightning_pose.egg-info/SOURCES.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)        1 2024-04-01 21:48:35.000000 lightning-pose-1.2.2/lightning_pose.egg-info/dependency_links.txt
--rw-r--r--   0 mattw     (1000) mattw     (1000)      368 2024-04-01 21:48:35.000000 lightning-pose-1.2.2/lightning_pose.egg-info/requires.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)       15 2024-04-01 21:48:35.000000 lightning-pose-1.2.2/lightning_pose.egg-info/top_level.txt
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/scripts/
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/scripts/configs/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6643 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_crim13.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6758 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_default.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6034 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_ibl-paw.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6060 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_ibl-pupil.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     8235 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_mirror-fish.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     8211 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_mirror-mouse-example.yaml
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     7381 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/configs/config_mirror-mouse.yaml
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/scripts/converters/
--rw-r--r--   0 mattw     (1000) mattw     (1000)     3265 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/scripts/converters/dlc2lp.py
--rwxrwxr-x   0 mattw     (1000) mattw     (1000)     1193 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/create_fiftyone_dataset.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)  8476261 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/litpose_training_demo.ipynb
--rwxrwxr-x   0 mattw     (1000) mattw     (1000)     6399 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/scripts/predict_new_vids.py
--rwxrwxr-x   0 mattw     (1000) mattw     (1000)     9218 2024-03-28 21:36:39.000000 lightning-pose-1.2.2/scripts/train_hydra.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)      230 2024-04-01 21:48:35.945308 lightning-pose-1.2.2/setup.cfg
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     3137 2024-04-01 21:48:29.000000 lightning-pose-1.2.2/setup.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/tests/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     8929 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/conftest.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/tests/data/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     3627 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/data/test_augmentations.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4088 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/data/test_dali.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     6855 2024-03-28 17:59:55.000000 lightning-pose-1.2.2/tests/data/test_datamodules.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     2262 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/data/test_datasets.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)    16658 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/tests/data/test_utils.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.941307 lightning-pose-1.2.2/tests/losses/
--rw-r--r--   0 mattw     (1000) mattw     (1000)      941 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/tests/losses/test_helpers.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)    18235 2023-08-09 16:18:22.000000 lightning-pose-1.2.2/tests/losses/test_losses.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.945308 lightning-pose-1.2.2/tests/models/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     7882 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/models/test_base.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1184 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/models/test_heatmap_tracker.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     2060 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/models/test_heatmap_tracker_mhcrnn.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1204 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/models/test_regression_tracker.py
--rw-r--r--   0 mattw     (1000) mattw     (1000)     3988 2024-03-26 14:09:27.000000 lightning-pose-1.2.2/tests/test_metrics.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-01 21:48:35.945308 lightning-pose-1.2.2/tests/utils/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     1279 2024-03-29 17:58:38.000000 lightning-pose-1.2.2/tests/utils/test_fiftyone.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     7898 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/utils/test_pca.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4776 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/utils/test_predictions.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4970 2024-03-28 15:28:56.000000 lightning-pose-1.2.2/tests/utils/test_scripts.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.981349 lightning-pose-1.2.3/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      751 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/Dockerfile.cuda11
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      564 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/Dockerfile.cuda12
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1069 2021-10-12 16:17:39.000000 lightning-pose-1.2.3/LICENSE
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      389 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/MANIFEST.in
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2711 2024-04-04 18:45:04.981349 lightning-pose-1.2.3/PKG-INFO
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2293 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/README.md
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.941349 lightning-pose-1.2.3/data/
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.945349 lightning-pose-1.2.3/data/mirror-mouse-example/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)    23291 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/CollectedData.csv
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58061 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img00.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58061 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img01.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58823 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img02.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61321 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img03.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60514 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img04.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58845 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img05.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59644 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img06.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59770 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img07.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62981 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img08.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59896 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img09.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60176 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img10.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59447 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img11.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59594 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img12.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56872 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img13.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60321 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img14.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56750 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img15.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58859 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img16.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59711 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img17.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58963 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img18.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62030 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img19.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57946 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img20.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58369 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img21.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57289 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img22.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58406 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img23.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61508 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img24.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    55197 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img25.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61129 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img26.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59406 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img27.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58022 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img28.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60939 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img29.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59418 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img30.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57690 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img31.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61011 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img32.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61344 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img33.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59423 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img34.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58590 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img35.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58634 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img36.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59459 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img37.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60221 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img38.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59427 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img39.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59695 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img40.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59000 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img41.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56997 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img42.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56691 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img43.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56210 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img44.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58659 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img45.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58772 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img46.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57162 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img47.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58633 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img48.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59179 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img49.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58090 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img50.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59679 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img51.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60383 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img52.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58368 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img53.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56150 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img54.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58609 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img55.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57972 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img56.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56140 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img57.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58368 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img58.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59631 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img59.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57544 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img60.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    56942 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img61.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58647 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img62.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58314 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img63.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59191 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img64.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58908 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img65.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57875 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img66.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59113 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img67.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61882 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img68.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58659 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img69.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58569 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img70.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58122 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img71.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57775 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img72.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57577 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img73.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60838 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img74.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59679 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img75.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59493 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img76.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60714 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img77.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57643 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img78.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59165 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img79.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58122 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img80.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    58643 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img81.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57999 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img82.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    62707 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img83.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    63460 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img84.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57620 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img85.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    57186 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img86.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    59946 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img87.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    61352 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img88.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60565 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img89.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img90.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img91.png
+-rwxr-xr-x   0 mattw     (1000) mattw     (1000)    60453 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img92.png
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/data/mirror-mouse-example/videos/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)  1724850 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/data/mirror-mouse-example/videos/test_vid.mp4
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/docs/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6250 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/docs/README.md
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1298 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/docs/roadmap.md
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/lightning_pose/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2022-02-01 19:50:48.000000 lightning-pose-1.2.3/lightning_pose/__init__.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/lightning_pose/apps/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)    10743 2024-03-26 14:09:27.000000 lightning-pose-1.2.3/lightning_pose/apps/labeled_frame_diagnostics.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     8707 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/lightning_pose/apps/plots.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     8197 2024-03-26 14:09:27.000000 lightning-pose-1.2.3/lightning_pose/apps/utils.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     7796 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/lightning_pose/apps/video_diagnostics.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1603 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/callbacks.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.965349 lightning-pose-1.2.3/lightning_pose/data/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      194 2023-03-06 14:42:52.000000 lightning-pose-1.2.3/lightning_pose/data/__init__.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     3937 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/data/augmentations.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    15050 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/data/dali.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     9305 2024-03-28 21:36:39.000000 lightning-pose-1.2.3/lightning_pose/data/datamodules.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    14144 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/data/datasets.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    20100 2024-03-28 17:59:46.000000 lightning-pose-1.2.3/lightning_pose/data/utils.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.965349 lightning-pose-1.2.3/lightning_pose/losses/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2022-02-01 19:50:48.000000 lightning-pose-1.2.3/lightning_pose/losses/__init__.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2755 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/losses/factory.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1436 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/losses/helpers.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    29899 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/losses/losses.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6413 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/metrics.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.965349 lightning-pose-1.2.3/lightning_pose/models/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)      626 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/__init__.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.965349 lightning-pose-1.2.3/lightning_pose/models/backbones/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)        0 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/lightning_pose/models/backbones/__init__.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6253 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/backbones/torchvision.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4615 2024-03-29 17:58:38.000000 lightning-pose-1.2.3/lightning_pose/models/backbones/vit_img_encoder.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     3235 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/backbones/vits.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    17706 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/base.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    17062 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/heatmap_tracker.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    19105 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/heatmap_tracker_mhcrnn.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     8290 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/models/regression_tracker.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.965349 lightning-pose-1.2.3/lightning_pose/utils/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)      719 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/utils/__init__.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    11001 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/utils/fiftyone.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     7705 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/utils/io.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    15483 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/utils/pca.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    31356 2024-04-01 20:58:09.000000 lightning-pose-1.2.3/lightning_pose/utils/predictions.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    24957 2024-03-28 17:59:50.000000 lightning-pose-1.2.3/lightning_pose/utils/scripts.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1580 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/lightning_pose/utils/tests.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.961349 lightning-pose-1.2.3/lightning_pose.egg-info/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     2711 2024-04-04 18:45:04.000000 lightning-pose-1.2.3/lightning_pose.egg-info/PKG-INFO
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     7027 2024-04-04 18:45:04.000000 lightning-pose-1.2.3/lightning_pose.egg-info/SOURCES.txt
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)        1 2024-04-04 18:45:04.000000 lightning-pose-1.2.3/lightning_pose.egg-info/dependency_links.txt
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      382 2024-04-04 18:45:04.000000 lightning-pose-1.2.3/lightning_pose.egg-info/requires.txt
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)       36 2024-04-04 18:45:04.000000 lightning-pose-1.2.3/lightning_pose.egg-info/top_level.txt
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/scripts/
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/scripts/configs/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6643 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_crim13.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6758 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_default.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6034 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_ibl-paw.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6060 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_ibl-pupil.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     8235 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_mirror-fish.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     8211 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_mirror-mouse-example.yaml
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     7381 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/configs/config_mirror-mouse.yaml
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/scripts/converters/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     3265 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/scripts/converters/dlc2lp.py
+-rwxrwxr-x   0 mattw     (1000) mattw     (1000)     1193 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/create_fiftyone_dataset.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)  8476261 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/litpose_training_demo.ipynb
+-rwxrwxr-x   0 mattw     (1000) mattw     (1000)     6399 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/scripts/predict_new_vids.py
+-rwxrwxr-x   0 mattw     (1000) mattw     (1000)     9218 2024-03-28 21:36:39.000000 lightning-pose-1.2.3/scripts/train_hydra.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      230 2024-04-04 18:45:04.981349 lightning-pose-1.2.3/setup.cfg
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     3089 2024-04-04 18:44:54.000000 lightning-pose-1.2.3/setup.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/tests/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     8929 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/conftest.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/tests/data/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     3627 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/data/test_augmentations.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4088 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/data/test_dali.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     6855 2024-03-28 17:59:55.000000 lightning-pose-1.2.3/tests/data/test_datamodules.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2262 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/data/test_datasets.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)    16658 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/tests/data/test_utils.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.977349 lightning-pose-1.2.3/tests/losses/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      941 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/tests/losses/test_helpers.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)    18235 2023-08-09 16:18:22.000000 lightning-pose-1.2.3/tests/losses/test_losses.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.981349 lightning-pose-1.2.3/tests/models/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     7882 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/models/test_base.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1184 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/models/test_heatmap_tracker.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2060 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/models/test_heatmap_tracker_mhcrnn.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1204 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/models/test_regression_tracker.py
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     3988 2024-03-26 14:09:27.000000 lightning-pose-1.2.3/tests/test_metrics.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-04 18:45:04.981349 lightning-pose-1.2.3/tests/utils/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1279 2024-03-29 17:58:38.000000 lightning-pose-1.2.3/tests/utils/test_fiftyone.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     7898 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/utils/test_pca.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4776 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/utils/test_predictions.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4970 2024-03-28 15:28:56.000000 lightning-pose-1.2.3/tests/utils/test_scripts.py
```

### Comparing `lightning-pose-1.2.2/Dockerfile.cuda11` & `lightning-pose-1.2.3/Dockerfile.cuda11`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/Dockerfile.cuda12` & `lightning-pose-1.2.3/Dockerfile.cuda12`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/LICENSE` & `lightning-pose-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/PKG-INFO` & `lightning-pose-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-pose
-Version: 1.2.2
+Version: 1.2.3
 Summary: Semi-supervised pose estimation using pytorch lightning
 Home-page: https://github.com/danbider/lightning-pose
 Author: Dan Biderman and Matt Whiteway
 Author-email: danbider@gmail.com
 Keywords: machine learning,deep learning,computer_vision
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `lightning-pose-1.2.2/README.md` & `lightning-pose-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/CollectedData.csv` & `lightning-pose-1.2.3/data/mirror-mouse-example/CollectedData.csv`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img00.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img00.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img01.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img01.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img02.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img02.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img03.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img03.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img04.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img04.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img05.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img05.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img06.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img06.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img07.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img07.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img08.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img08.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img09.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img09.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img10.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img10.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img11.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img11.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img12.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img12.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img13.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img13.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img14.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img14.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img15.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img15.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img16.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img16.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img17.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img17.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img18.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img18.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img19.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img19.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img20.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img20.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img21.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img21.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img22.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img22.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img23.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img23.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img24.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img24.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img25.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img25.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img26.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img26.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img27.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img27.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img28.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img28.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img29.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img29.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img30.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img30.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img31.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img31.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img32.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img32.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img33.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img33.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img34.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img34.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img35.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img35.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img36.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img36.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img37.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img37.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img38.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img38.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img39.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img39.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img40.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img40.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img41.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img41.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img42.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img42.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img43.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img43.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img44.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img44.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img45.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img45.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img46.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img46.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img47.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img47.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img48.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img48.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img49.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img49.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img50.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img50.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img51.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img51.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img52.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img52.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img53.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img53.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img54.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img54.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img55.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img55.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img56.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img56.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img57.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img57.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img58.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img58.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img59.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img59.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img60.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img60.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img61.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img61.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img62.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img62.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img63.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img63.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img64.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img64.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img65.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img65.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img66.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img66.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img67.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img67.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img68.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img68.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img69.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img69.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img70.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img70.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img71.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img71.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img72.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img72.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img73.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img73.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img74.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img74.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img75.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img75.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img76.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img76.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img77.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img77.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img78.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img78.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img79.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img79.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img80.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img80.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img81.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img81.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img82.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img82.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img83.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img83.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img84.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img84.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img85.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img85.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img86.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img86.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img87.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img87.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img88.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img88.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img89.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img89.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img90.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img90.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img91.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img91.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/labeled-data/img92.png` & `lightning-pose-1.2.3/data/mirror-mouse-example/labeled-data/img92.png`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/data/mirror-mouse-example/videos/test_vid.mp4` & `lightning-pose-1.2.3/data/mirror-mouse-example/videos/test_vid.mp4`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/docs/README.md` & `lightning-pose-1.2.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/docs/roadmap.md` & `lightning-pose-1.2.3/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/apps/labeled_frame_diagnostics.py` & `lightning-pose-1.2.3/lightning_pose/apps/labeled_frame_diagnostics.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/apps/plots.py` & `lightning-pose-1.2.3/lightning_pose/apps/plots.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/apps/utils.py` & `lightning-pose-1.2.3/lightning_pose/apps/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/apps/video_diagnostics.py` & `lightning-pose-1.2.3/lightning_pose/apps/video_diagnostics.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/callbacks.py` & `lightning-pose-1.2.3/lightning_pose/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/data/augmentations.py` & `lightning-pose-1.2.3/lightning_pose/data/augmentations.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/data/dali.py` & `lightning-pose-1.2.3/lightning_pose/data/dali.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/data/datamodules.py` & `lightning-pose-1.2.3/lightning_pose/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/data/datasets.py` & `lightning-pose-1.2.3/lightning_pose/data/datasets.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/data/utils.py` & `lightning-pose-1.2.3/lightning_pose/data/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/losses/factory.py` & `lightning-pose-1.2.3/lightning_pose/losses/factory.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/losses/helpers.py` & `lightning-pose-1.2.3/lightning_pose/losses/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/losses/losses.py` & `lightning-pose-1.2.3/lightning_pose/losses/losses.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/metrics.py` & `lightning-pose-1.2.3/lightning_pose/metrics.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/__init__.py` & `lightning-pose-1.2.3/lightning_pose/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/backbones/torchvision.py` & `lightning-pose-1.2.3/lightning_pose/models/backbones/torchvision.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/backbones/vit_img_encoder.py` & `lightning-pose-1.2.3/lightning_pose/models/backbones/vit_img_encoder.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/backbones/vits.py` & `lightning-pose-1.2.3/lightning_pose/models/backbones/vits.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/base.py` & `lightning-pose-1.2.3/lightning_pose/models/base.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/heatmap_tracker.py` & `lightning-pose-1.2.3/lightning_pose/models/heatmap_tracker.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/heatmap_tracker_mhcrnn.py` & `lightning-pose-1.2.3/lightning_pose/models/heatmap_tracker_mhcrnn.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/models/regression_tracker.py` & `lightning-pose-1.2.3/lightning_pose/models/regression_tracker.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/__init__.py` & `lightning-pose-1.2.3/lightning_pose/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/fiftyone.py` & `lightning-pose-1.2.3/lightning_pose/utils/fiftyone.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/io.py` & `lightning-pose-1.2.3/lightning_pose/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/pca.py` & `lightning-pose-1.2.3/lightning_pose/utils/pca.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/predictions.py` & `lightning-pose-1.2.3/lightning_pose/utils/predictions.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/scripts.py` & `lightning-pose-1.2.3/lightning_pose/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose/utils/tests.py` & `lightning-pose-1.2.3/lightning_pose/utils/tests.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/lightning_pose.egg-info/PKG-INFO` & `lightning-pose-1.2.3/lightning_pose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-pose
-Version: 1.2.2
+Version: 1.2.3
 Summary: Semi-supervised pose estimation using pytorch lightning
 Home-page: https://github.com/danbider/lightning-pose
 Author: Dan Biderman and Matt Whiteway
 Author-email: danbider@gmail.com
 Keywords: machine learning,deep learning,computer_vision
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `lightning-pose-1.2.2/lightning_pose.egg-info/SOURCES.txt` & `lightning-pose-1.2.3/lightning_pose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_crim13.yaml` & `lightning-pose-1.2.3/scripts/configs/config_crim13.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_default.yaml` & `lightning-pose-1.2.3/scripts/configs/config_default.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_ibl-paw.yaml` & `lightning-pose-1.2.3/scripts/configs/config_ibl-paw.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_ibl-pupil.yaml` & `lightning-pose-1.2.3/scripts/configs/config_ibl-pupil.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_mirror-fish.yaml` & `lightning-pose-1.2.3/scripts/configs/config_mirror-fish.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_mirror-mouse-example.yaml` & `lightning-pose-1.2.3/scripts/configs/config_mirror-mouse-example.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/configs/config_mirror-mouse.yaml` & `lightning-pose-1.2.3/scripts/configs/config_mirror-mouse.yaml`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/converters/dlc2lp.py` & `lightning-pose-1.2.3/scripts/converters/dlc2lp.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/create_fiftyone_dataset.py` & `lightning-pose-1.2.3/scripts/create_fiftyone_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/litpose_training_demo.ipynb` & `lightning-pose-1.2.3/scripts/litpose_training_demo.ipynb`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/predict_new_vids.py` & `lightning-pose-1.2.3/scripts/predict_new_vids.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/scripts/train_hydra.py` & `lightning-pose-1.2.3/scripts/train_hydra.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/setup.py` & `lightning-pose-1.2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import re
 import os
 import subprocess
 
 from setuptools import find_packages, setup
 
-VERSION = "1.2.2"
+VERSION = "1.2.3"
 
 # add the README.md file to the long_description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def get_cuda_version():
@@ -80,37 +80,33 @@
         "flake8",
         "isort",
         "Sphinx",
         "sphinx_rtd_theme",
         "sphinx-rtd-dark-mode",
         "sphinx-automodapi",
         "sphinx-copybutton",
+        "sphinx-design",
     },
     "extra_models": {
         "lightning-bolts",  # resnet-50 trained on imagenet using simclr
     },
 }
 
-# collect all data and script files
-data_files = []
-for root, dirs, files in os.walk("data"):
-    data_files.extend([os.path.join(root, f) for f in files])
-for root, dirs, files in os.walk("scripts"):
-    data_files.extend([os.path.join(root, f) for f in files])
-
-
 setup(
     name="lightning-pose",
-    packages=find_packages(exclude=("data", "docs", "scripts", "tests")),
+    packages=find_packages() + ["mirror_mouse_example"],  # include data for wheel packaging
     version=VERSION,
     description="Semi-supervised pose estimation using pytorch lightning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dan Biderman and Matt Whiteway",
     install_requires=install_requires,
     extras_require=extras_require,
     author_email="danbider@gmail.com",
     url="https://github.com/danbider/lightning-pose",
     keywords=["machine learning", "deep learning", "computer_vision"],
-    package_data={"lightning_pose": data_files},
-    include_package_data=True,
+    package_dir={
+        "lightning_pose": "lightning_pose",
+        "mirror_mouse_example": "data/mirror-mouse-example",  # remap 'data/mirror-mouse-example'
+    },
+    include_package_data=True,  # required to get the non-.py data files in the wheel
 )
```

### Comparing `lightning-pose-1.2.2/tests/conftest.py` & `lightning-pose-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/data/test_augmentations.py` & `lightning-pose-1.2.3/tests/data/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/data/test_dali.py` & `lightning-pose-1.2.3/tests/data/test_dali.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/data/test_datamodules.py` & `lightning-pose-1.2.3/tests/data/test_datamodules.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/data/test_datasets.py` & `lightning-pose-1.2.3/tests/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/data/test_utils.py` & `lightning-pose-1.2.3/tests/data/test_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/losses/test_helpers.py` & `lightning-pose-1.2.3/tests/losses/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/losses/test_losses.py` & `lightning-pose-1.2.3/tests/losses/test_losses.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/models/test_base.py` & `lightning-pose-1.2.3/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/models/test_heatmap_tracker.py` & `lightning-pose-1.2.3/tests/models/test_heatmap_tracker.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/models/test_heatmap_tracker_mhcrnn.py` & `lightning-pose-1.2.3/tests/models/test_heatmap_tracker_mhcrnn.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/models/test_regression_tracker.py` & `lightning-pose-1.2.3/tests/models/test_regression_tracker.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/test_metrics.py` & `lightning-pose-1.2.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/utils/test_fiftyone.py` & `lightning-pose-1.2.3/tests/utils/test_fiftyone.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/utils/test_pca.py` & `lightning-pose-1.2.3/tests/utils/test_pca.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/utils/test_predictions.py` & `lightning-pose-1.2.3/tests/utils/test_predictions.py`

 * *Files identical despite different names*

### Comparing `lightning-pose-1.2.2/tests/utils/test_scripts.py` & `lightning-pose-1.2.3/tests/utils/test_scripts.py`

 * *Files identical despite different names*


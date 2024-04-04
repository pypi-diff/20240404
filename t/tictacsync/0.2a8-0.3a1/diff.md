# Comparing `tmp/tictacsync-0.2a8.tar.gz` & `tmp/tictacsync-0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacsync-0.2a8.tar", last modified: Tue Mar 26 23:05:48 2024, max compression
+gzip compressed data, was "tictacsync-0.3a1.tar", last modified: Thu Apr  4 15:36:35 2024, max compression
```

## Comparing `tictacsync-0.2a8.tar` & `tictacsync-0.3a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-03-26 23:05:48.645741 tictacsync-0.2a8/
--rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.2a8/LICENSE
--rw-r--r--   0 lutzray    (501) staff       (20)     5040 2024-03-26 23:05:48.645243 tictacsync-0.2a8/PKG-INFO
--rw-rw-r--   0 lutzray    (501) staff       (20)     4187 2024-03-26 02:38:52.000000 tictacsync-0.2a8/README.md
--rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-03-26 23:05:48.645928 tictacsync-0.2a8/setup.cfg
--rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-03-26 22:47:52.000000 tictacsync-0.2a8/setup.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-03-26 23:05:48.638082 tictacsync-0.2a8/tictacsync/
--rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.2a8/tictacsync/__init__.py
--rw-r--r--   0 lutzray    (501) staff       (20)    27416 2024-03-26 22:47:26.000000 tictacsync-0.2a8/tictacsync/device_scanner.py
--rw-r--r--   0 lutzray    (501) staff       (20)    11329 2024-03-26 22:36:52.000000 tictacsync-0.2a8/tictacsync/entry.py
--rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.2a8/tictacsync/multi2polywav.py
--rw-r--r--   0 lutzray    (501) staff       (20)     4867 2024-03-16 14:09:41.000000 tictacsync-0.2a8/tictacsync/remergemix.py
--rw-r--r--   0 lutzray    (501) staff       (20)    40207 2024-03-26 22:26:55.000000 tictacsync-0.2a8/tictacsync/timeline.py
--rw-r--r--   0 lutzray    (501) staff       (20)    76505 2024-03-25 19:54:11.000000 tictacsync-0.2a8/tictacsync/yaltc.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-03-26 23:05:48.644410 tictacsync-0.2a8/tictacsync.egg-info/
--rw-r--r--   0 lutzray    (501) staff       (20)     5040 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/PKG-INFO
--rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/SOURCES.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/dependency_links.txt
--rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/entry_points.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.2a8/tictacsync.egg-info/not-zip-safe
--rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/requires.txt
--rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-03-26 23:05:48.000000 tictacsync-0.2a8/tictacsync.egg-info/top_level.txt
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.126706 tictacsync-0.3a1/
+-rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a1/LICENSE
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 15:36:35.126213 tictacsync-0.3a1/PKG-INFO
+-rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a1/README.md
+-rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-04 15:36:35.126843 tictacsync-0.3a1/setup.cfg
+-rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-04 15:36:22.000000 tictacsync-0.3a1/setup.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.121611 tictacsync-0.3a1/tictacsync/
+-rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a1/tictacsync/__init__.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    27558 2024-04-02 15:17:03.000000 tictacsync-0.3a1/tictacsync/device_scanner.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    11391 2024-04-04 14:48:23.000000 tictacsync-0.3a1/tictacsync/entry.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a1/tictacsync/multi2polywav.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a1/tictacsync/remergemix.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    45946 2024-04-04 14:45:33.000000 tictacsync-0.3a1/tictacsync/timeline.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a1/tictacsync/yaltc.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.125494 tictacsync-0.3a1/tictacsync.egg-info/
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/PKG-INFO
+-rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/entry_points.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a1/tictacsync.egg-info/not-zip-safe
+-rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/requires.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/top_level.txt
```

### Comparing `tictacsync-0.2a8/LICENSE` & `tictacsync-0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tictacsync-0.2a8/PKG-INFO` & `tictacsync-0.3a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.2a8
+Version: 0.3a1
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -79,15 +79,15 @@
 
 To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
-    > tictacsync -p tictacsync/tests/dailies/loose/MVI_0024.MP4
+    > tictacsync -p dailies/loose/MVI_0024.MP4
 
 Typical first plot produced :
 
 ![word](https://mamot.fr/system/media_attachments/files/110/279/794/002/305/269/original/0198908c6eb5c592.png)
 
 Typical second plot produced (note the 34 [FSK](https://en.wikipedia.org/wiki/Frequency-shift_keying) encoded bits `0010111101001111100110000110010000`):
 ![slicing](https://mamot.fr/system/media_attachments/files/110/279/794/021/372/766/original/6ec62bb417115f52.png)
```

### Comparing `tictacsync-0.2a8/README.md` & `tictacsync-0.3a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
-    > tictacsync -p tictacsync/tests/dailies/loose/MVI_0024.MP4
+    > tictacsync -p dailies/loose/MVI_0024.MP4
 
 Typical first plot produced :
 
 ![word](https://mamot.fr/system/media_attachments/files/110/279/794/002/305/269/original/0198908c6eb5c592.png)
 
 Typical second plot produced (note the 34 [FSK](https://en.wikipedia.org/wiki/Frequency-shift_keying) encoded bits `0010111101001111100110000110010000`):
 ![slicing](https://mamot.fr/system/media_attachments/files/110/279/794/021/372/766/original/6ec62bb417115f52.png)
```

### Comparing `tictacsync-0.2a8/setup.py` & `tictacsync-0.3a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     entry_points = {
         "console_scripts": [
         'tictacsync = tictacsync.entry:main',
         'remergemix = tictacsync.remergemix:main',
         'multi2polywav = tictacsync.multi2polywav:main',
         ]
         },
-    version = '0.2a8',
+    version = '0.3a1',
     description = "command for syncing audio video recordings",
     long_description_content_type='text/markdown',
     long_description = long_descr,
     include_package_data=True,
     zip_safe=False,
     author = "Raymond Lutz",
     author_email = "lutzrayblog@mac.com",
```

### Comparing `tictacsync-0.2a8/tictacsync/device_scanner.py` & `tictacsync-0.3a1/tictacsync/device_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,36 +54,14 @@
 
 def print_grby(grby):
     for key, keylist in grby:
         print('\ngrouped by %s:'%key)
         for e in keylist:
             print(' ', e)
 
-def media_at_path(p):
-        # return Media object for mediafile using ffprobe
-        dev_UID, dt = get_device_ffprobe_UID(p)
-        if dt == 'CAM':
-            streams = ffmpeg.probe(p)['streams']
-            audio_streams = [
-                stream 
-                for stream
-                in streams
-                if stream['codec_type']=='audio'
-                ]
-            if len(audio_streams) > 1:
-                raise Exception('ffprobe gave multiple audio streams?')
-            audio_str = audio_streams[0]
-            n = audio_str['channels']
-            # pprint(ffmpeg.probe(p))
-        else:
-            n = sox.file_info.channels(_pathname(p)) # eg 2
-        logger.debug('for file %s dev_UID established %s'%(p.name, dev_UID))
-        return Media(p,
-            Device(UID=dev_UID, folder=p.parent, name=None, dev_type=dt,
-                    n_chan=n, tracks=None))
 
 @dataclass
 class Tracks:
     # track numbers start at 1 for first track (as needed by sox)
     ttc: int # track number of TicTacCode signal
     unused: list # of unused tracks
     stereomics: list # of stereo mics track tuples (Lchan#, Rchan#)
@@ -107,16 +85,41 @@
 
 @dataclass
 class Media:
     """A custom data type that represents data for a media file.
     """
     path: Path
     device: Device
-
-
+def media_at_path(input_structure, p):
+    # return Media object for mediafile using ffprobe
+    dev_UID, dt = get_device_ffprobe_UID(p)
+    dev_name = None 
+    if input_structure == 'folder_is_device':
+        dev_name = p.parent.name
+        if dev_UID is None:
+            dev_UID = hash(dev_name)
+    if dt == 'CAM':
+        streams = ffmpeg.probe(p)['streams']
+        audio_streams = [
+            stream 
+            for stream
+            in streams
+            if stream['codec_type']=='audio'
+            ]
+        if len(audio_streams) > 1:
+            raise Exception('ffprobe gave multiple audio streams?')
+        audio_str = audio_streams[0]
+        n = audio_str['channels']
+        # pprint(ffmpeg.probe(p))
+    else:
+        n = sox.file_info.channels(_pathname(p)) # eg 2
+    logger.debug('for file %s dev_UID established %s'%(p.name, dev_UID))
+    return Media(p,
+        Device(UID=dev_UID, folder=p.parent, name=dev_name, dev_type=dt,
+                n_chan=n, tracks=None))
 
 def get_device_ffprobe_UID(file):
     """
     Tries to find an unique hash integer identifying the device that produced
     the file based on the string inside ffprobe metadata  without any
     reference to date nor length nor time. Find out with ffprobe the type
     of device: CAM or REC for videocamera or audio recorder.
@@ -246,15 +249,15 @@
         paths = [
             p
             for p in files
             if p.suffix[1:] in av_file_extensions
             and 'SyncedMedia' not in p.parts
         ]
         for p in paths:
-            new_media = media_at_path(p) # dev UID set here
+            new_media = media_at_path(self.input_structure, p) # dev UID set here
             self.found_media_files.append(new_media)
         # files from devices without UID or name
         def _same(l):
             return all(e == l[0] for e in l)
         def _try_name(medias):
             # return common first strings in filename
             names = [m.path.name for m in medias]
@@ -285,15 +288,15 @@
             print('UID: [gold1]%s[/gold1]'%start_string)
             for m in no_device_UID_media:
                 m.device = one_device
             logger.debug('new device added %s'%self.found_media_files)
         logger.debug('Scanner.found_media_files = %s'%self.found_media_files)
         if self.input_structure == 'folder_is_device':
             self._check_folders_have_same_device()
-            self._use_folder_as_device_name()
+            # self._use_folder_as_device_name()
             devices = set([m.device for m in self.found_media_files])
             audio_devices = [d for d in devices if d.dev_type == 'REC']
             for recorder in audio_devices:
                 recorder.tracks = self._get_tracks_from_file(recorder)
         no_name_devices = [m.device for m in self.found_media_files
             if not m.device.name]
         # if no_name_devices:
@@ -349,24 +352,24 @@
                 raise Exception
             else:
                 return tracks
         else:
             logger.debug('no tracks.txt file found')
             return None
 
-    def _use_folder_as_device_name(self):
-        """
-        For each media in self.found_media_files replace existing Device.name by
-        folder name.
-
-        Returns nothing
-        """
-        for m in self.found_media_files:
-            m.device.name = m.path.parent.name
-        logger.debug(self.found_media_files)
+    # def _use_folder_as_device_name(self):
+    #     """
+    #     For each media in self.found_media_files replace existing Device.name by
+    #     folder name.
+
+    #     Returns nothing
+    #     """
+    #     for m in self.found_media_files:
+    #         m.device.name = m.path.parent.name
+    #     logger.debug(self.found_media_files)
 
     def _check_folders_have_same_device(self):
         """
         Since input_structure == 'folder_is_device,
         checks for files in self.found_media_files for structure as following.
 
         Warns user and quit program for:
```

### Comparing `tictacsync-0.2a8/tictacsync/entry.py` & `tictacsync-0.3a1/tictacsync/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             rec_with_yaltc.append(r)
     for r in rec_with_yaltc:
         times.append(r.get_start_time())
     return recordings, rec_with_yaltc, times
 
 def process_single(file, args):
     # argument is a single file
-    m = device_scanner.media_at_path(Path(file))
+    m = device_scanner.media_at_path(None, Path(file))
     a_rec = yaltc.Recording(m)
     time = a_rec.get_start_time(plots=args.plotting)
     if time != None:
         frac_time = int(time.microsecond / 1e2)
         d = '%s.%s'%(time.strftime("%Y-%m-%d %H:%M:%S"),frac_time)
         if args.terse:
             print('%s UTC:%s pulse: %i in chan %i'%(file, d, a_rec.sync_position,
@@ -122,17 +122,18 @@
                     help='terse output')
     args = parser.parse_args()
     if args.verbose_output:
         logger.add(sys.stderr, level="DEBUG")
     # logger.add(sys.stdout, filter="__main__")
     # logger.add(sys.stdout, filter="device_scanner")
     # logger.add(sys.stdout, filter="yaltc") _extract_sound_to_merge
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "media_at_path")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "scan_media_and_build_devices_UID")
     # logger.add(sys.stdout, filter=lambda r: r["function"] == "build_audio_and_write_video")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_audio_devices")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_mix")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix")
     top_dir = args.directory[0]
     if os.path.isfile(top_dir):
         file = top_dir
         process_single(file, args)
     if not os.path.isdir(top_dir):
         print('%s is not a directory or doesnt exist.'%top_dir)
         sys.exit(1)
```

### Comparing `tictacsync-0.2a8/tictacsync/multi2polywav.py` & `tictacsync-0.3a1/tictacsync/multi2polywav.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.2a8/tictacsync/remergemix.py` & `tictacsync-0.3a1/tictacsync/remergemix.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import sox, tempfile, os, ffmpeg
 from rich import print
 import shutil
 
 
 logger.remove()
-OUT_DIR = 'SyncedMedia'
+# OUT_DIR = 'SyncedMedia'
 
 def _pathname(tempfile_or_path) -> str:
     if isinstance(tempfile_or_path, str):
         return tempfile_or_path
     if isinstance(tempfile_or_path, Path):
         return str(tempfile_or_path)
     if isinstance(tempfile_or_path, tempfile._TemporaryFileWrapper):
@@ -125,15 +125,15 @@
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
                 "directory",
                 type=str,
                 nargs='+',
-                help="path of media directory containing SyncedMedia/",
+                help="path of media directory containing Synced videos and their ISOs",
                 default='.'
                 )
     args = parser.parse_args()
     # logger.info('arguments: %s'%args)
     logger.debug('args %s'%args)
     synciso(args.directory)
         # for e in keylist:
```

### Comparing `tictacsync-0.2a8/tictacsync/timeline.py` & `tictacsync-0.3a1/tictacsync/timeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import sox
 from pathlib import Path
 from rich import print
 from itertools import groupby
 # import opentimelineio as otio
 from datetime import timedelta
 import pprint, shutil, os
+from subprocess import Popen, PIPE
 
 from inspect import currentframe, getframeinfo
 try:
     from . import yaltc
 except:
     import yaltc
 
 CLUSTER_GAP = 0.5 # secs between multicam clusters
 DEL_TEMP = False
+DB_OSX_NORM = -6 #dB
 OUT_DIR_DEFAULT = 'SyncedMedia'
 
 # utility for accessing pathnames
 def _pathname(tempfile_or_path) -> str:
     if isinstance(tempfile_or_path, str):
         return tempfile_or_path
     if isinstance(tempfile_or_path, yaltc.Recording):
@@ -56,14 +58,59 @@
     mix_dict = {1:[channel]}
     logger.debug('sox args %s %s %s'%(source, dest, mix_dict))    
     sox_transform.remix(mix_dict)
     logger.debug('sox transform %s'%str(sox_transform))
     status = sox_transform.build(str(source), str(dest))
     logger.debug('sox status %s'%status)
 
+def _sox_keep(audio_file, kept_channels) -> tempfile.NamedTemporaryFile:
+    """
+    Returns a NamedTemporaryFile containing the selected kept_channels
+
+    Building dict according to pysox.remix format.
+    https://pysox.readthedocs.io/en/latest/api.html#sox.transform.Transformer.remix
+    eg: 4 channels with TicTacCode_channel at #2 
+    returns {1: [1], 2: [3], 3: [4]}
+    ie the number of channels drops by one and chan 2 is missing
+    excluded_channels is a list of Zero Based indexing chan numbers
+
+    """
+    audio_file = _pathname(audio_file)
+    nchan = sox.file_info.channels(audio_file)
+    logger.debug('in file of %i chan, have to keep %s'%
+        (nchan, kept_channels))
+    all_channels = range(1, nchan + 1) # from 1 to nchan included
+    # list of list for pysox API
+    # eg [[1], [3], [4]]
+    kept_channels = [[n] for n in kept_channels]
+    sox_remix_dict = dict(zip(all_channels, kept_channels))
+    # {1: [1], 2: [3], 3: [4]} -> from 4 to 3 chan and chan 2 is dropped
+    output_fh = tempfile.NamedTemporaryFile(suffix='.wav', delete=DEL_TEMP)
+    out_file = _pathname(output_fh)
+    logger.debug('sox in and out files: %s %s'%(audio_file, out_file))
+    # sox_transform.set_output_format(channels=1)
+    sox_transform = sox.Transformer()
+    sox_transform.remix(sox_remix_dict)
+    logger.debug('sox remix transform: %s'%sox_transform)
+    logger.debug('sox remix dict: %s'%sox_remix_dict)
+    status = sox_transform.build(audio_file, out_file, return_output=True )
+    logger.debug('sox.build exit code %s'%str(status))
+    p = Popen('ffprobe %s -hide_banner'%audio_file,
+        shell=True, stdout=PIPE, stderr=PIPE)
+    stdout, stderr = p.communicate()
+    logger.debug('remixed input_file ffprobe:\n%s'%(stdout +
+        stderr).decode('utf-8'))
+    p = Popen('ffprobe %s -hide_banner'%out_file,
+        shell=True, stdout=PIPE, stderr=PIPE)
+    stdout, stderr = p.communicate()
+    logger.debug('remixed out_file ffprobe:\n%s'%(stdout +
+        stderr).decode('utf-8'))
+    return output_fh
+
+
 def _split_channels(multi_chan_audio:Path) -> list:
     nchan = sox.file_info.channels(_pathname(multi_chan_audio))
     source = _pathname(multi_chan_audio)
     paths = []
     for i in range(nchan):
         out_fh = tempfile.NamedTemporaryFile(suffix='.wav',
                 delete=DEL_TEMP)
@@ -74,19 +121,18 @@
         status = sox_transform.build(source, dest)
         logger.debug('source %s dest %s'%(source, dest))
         logger.debug('sox status %s'%status)
         paths.append(out_fh)
     logger.debug('paths %s'%paths)
     return paths
 
-
 def _sox_combine(paths) -> Path:
     """
-    Combines files referred by the list of Path into a new temporary files
-    passed on return each files are stacked in a different channel, so 
+    Combines (stacks) files referred by the list of Path into a new temporary
+    files passed on return each files are stacked in a different channel, so
     len(paths) == n_channels
     """
     if len(paths) == 1: # one device only, nothing to stack
         logger.debug('one device only, nothing to stack')
         return paths[0]
     out_file_handle = tempfile.NamedTemporaryFile(suffix='.wav',
         delete=DEL_TEMP)
@@ -113,33 +159,46 @@
         (merged_duration, nchan))
     return out_file_handle
 
 def _sox_mix(paths:list) -> tempfile.NamedTemporaryFile:
     """
     mix files referred by the list of Path into a new temporary files passed on return
     """
+    def _sox_norm(tempf):
+        normed_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
+                        delete=DEL_TEMP)
+        tfm = sox.Transformer()
+        tfm.norm(DB_OSX_NORM)
+        status = tfm.build(_pathname(tempf),_pathname(normed_tempfile))
+        logger.debug('sox.build status for norm(): %s'%status)
+        if status != True:
+            print('Error, sox did not normalize file in _sox_mix()')
+            sys.exit(1)
+        return normed_tempfile
+    paths = [_sox_norm(p) for p in paths]
     cbn = sox.Combiner()
     N = len(paths)
     if N == 1: # nothing to mix
+        logger.debug('one file: nothing to mix')
         return paths[0]
     cbn.set_input_format(file_type=['wav']*N)
     filenames = [_pathname(p) for p in paths]
-    logger.debug('files to mix %s'%filenames)
+    logger.debug('%i files to mix %s'%(N, filenames))
     mixed_tempf = tempfile.NamedTemporaryFile(suffix='.wav',delete=DEL_TEMP)
     status = cbn.build(filenames,
                 _pathname(mixed_tempf),
                 combine_type='mix',
                 input_volumes=[1/N]*N)
     logger.debug('sox.build status for mix: %s'%status)
     if status != True:
         print('Error, sox did not mix files in _sox_mix()')
         sys.exit(1)
     normed_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',delete=DEL_TEMP)
     tfm = sox.Transformer()
-    tfm.norm(-6)
+    tfm.norm(DB_OSX_NORM)
     status = tfm.build(_pathname(mixed_tempf),_pathname(normed_tempfile))
     logger.debug('sox.build status for norm(): %s'%status)
     if status != True:
         print('Error, sox did not normalize file in _sox_mix()')
         sys.exit(1)
     return normed_tempfile
 
@@ -212,16 +271,19 @@
         """
         Returns audio recordings that overlap self.ref_recording.
         Simply keys of self.edited_audio dict
         """
         return list(self.edited_audio.keys())
 
     def _get_audio_devices(self):
-        # ex {'RCR_A', 'RCR_B', 'RCR_C'} if multisound
-        return set([r.device for r in self.get_matched_audio_recs()])
+        devices = set([r.device for r in self.get_matched_audio_recs()])
+        logger.debug('get_matched_audio_recs: %s'%
+            pprint.pformat(self.get_matched_audio_recs()))
+        logger.debug('devices %s'%devices)
+        return devices
 
     def _get_all_recordings_for(self, device):
         # return recordings for a particular device, sorted by time
         recs = [a for a in self.get_matched_audio_recs() if a.device == device]
         recs.sort(key=lambda r: r.start_time)
         return recs
 
@@ -429,28 +491,22 @@
         out_file = _pathname(output_fh)
         logger.debug('sox in and out files: %s %s'%(input_file, out_file))
         status = sox_transform.build(input_file, out_file, return_output=True )
         logger.debug('sox.build exit code %s'%str(status))
         # audio_rec.edited_version = output_fh
         self.edited_audio[audio_rec] = output_fh
 
-
     def _write_ISOs(self, edited_audio_all_devices):
         """
         Writes isolated audio files that were synced to synced_clip_file,
         each track will have its dedicated monofile, named sequentially or with
         the name find in TRACKSFN if any, see Scanner._get_tracks_from_file()
 
-        synced_clip_file:
-            video to which audio has been merged
-        device:
-            instance of device_scanner.Device
-        dev_joined_audio:
-            NamedTemporaryFile for the joined synced (multi channel) audio for
-            a specific device
+        edited_audio_all_devices:
+            a list of (name, mono_tempfile)
 
         Returns nothing, output is written to filesystem as below.
         ISOs subfolders structure when user invokes the --isos flag:
 
         SyncedMedia/ (or output_dir)
 
                 leftCAM/
@@ -504,39 +560,75 @@
         ISOdir = synced_clip_dir/(video_stem_WO_suffix + '.ISO')
         os.makedirs(ISOdir, exist_ok=True)
         logger.debug('edited_audio_all_devices %s'%edited_audio_all_devices)
         logger.debug('ISOdir %s'%ISOdir)
         # ISO_multi_chan = ISOdir / 'ISO_multi_chan.wav'
         # logger.debug('temp file: %s'%(ISO_multi_chan))
         # logger.debug('will split audio to %s'%(ISOdir))
-        for name, audio_tempfile in edited_audio_all_devices:
+        for name, mono_tmpfl in edited_audio_all_devices:
              # pad(start_duration: float = 0.0, end_duration: float = 0.0)[source]
             destination = ISOdir/('%s.wav'%name)
-            audio_tempfile_trimpad = _fit_length(audio_tempfile)
-            shutil.copy(_pathname(audio_tempfile_trimpad), destination)
+            mono_tmpfl_trimpad = _fit_length(mono_tmpfl)
+            shutil.copy(_pathname(mono_tmpfl_trimpad), destination)
             logger.debug('destination:%s'%destination)
         # # mixNnormed = _sox_mix(tempfiles)
         # # print('516', _pathname(mixNnormed))
         # os.remove(ISO_multi_chan)
 
+    def _get_mix(self, device, multichan_tmpfl) -> tempfile.NamedTemporaryFile:
+        """        
+        If device has an associated Tracks description that declares a (mono or
+        stereo) mix track, returns a tmpfl containing the corresponding
+        tracks. If not, mix all the tracks with sox.
+
+        """
+        if device.tracks != None:
+            mix_tracks = device.tracks.mix
+            if len(mix_tracks) > 0:
+                logger.debug('%s has mix %s'%(device.name, mix_tracks))
+                logger.debug('device %s'%device)
+                if 'ttc' in device.tracks.rawtrx:
+                    sox_TTC_chan = device.tracks.rawtrx.index('ttc')
+                elif 'tc' in device.tracks.rawtrx:
+                    sox_TTC_chan = device.tracks.rawtrx.index('tc')
+                else:
+                    print('Error: no tc or ttc tag in track.txt')
+                    sys.exit(1)
+                sox_TTC_chan += 1 # sox NZBIDX
+                logger.debug('TTC chan %i'%sox_TTC_chan)
+                # redo indexing since tracks.txt numbers refere to complete
+                # files and here audio file had TTC and muted channels
+                # removed.
+                shift = 0
+                if mix_tracks[0] > sox_TTC_chan:
+                    shift += 1
+                for unused_tr in device.tracks.unused:
+                    if mix_tracks[0] > unused_tr:
+                        shift += 1
+                mix_tracks = [t-shift for t in mix_tracks]
+                logger.debug('new mix_tracks: %s'%mix_tracks)
+                return _sox_keep(multichan_tmpfl, mix_tracks)
+            else: # no tracks declaration, mix programmatically
+                return _sox_mix(_split_channels(multichan_tmpfl))
+
     def build_audio_and_write_video(self, top_dir, output_dir,
                                     write_multicam_structure,
                                     asked_ISOs):
         """
         top_dir: Path, directory where media were looked for
 
         output_dir: str for optional folder specified as CLI argument, if
         value is None, fall back to OUT_DIR_DEFAULT
 
         write_multicam_structure: True if needs to write multicam folders
 
         asked_ISOs: bool flag specified as CLI argument
 
         For each audio devices found overlapping self.ref_recording: pad, trim
-        or stretch audio files calling _get_concatenated_audiofile_for(), and
+        or stretch audio files by calling _get_concatenated_audiofile_for(), and
         put them in merged_audio_files_by_device. More than one audio recorder
         can be used for a shot: that's why merged_audio_files_by_device is a
         list
 
         Returns nothing
 
         Sets AudioStitcherVideoMerger.final_synced_file on completion
@@ -556,80 +648,104 @@
             synced_clip_dir = synced_clip_dir/device_name # = synced_clip_dir/ZOOM
         self.synced_clip_dir = synced_clip_dir
         os.makedirs(synced_clip_dir, exist_ok=True)
         logger.debug('synced_clip_dir is: %s'%synced_clip_dir)
         synced_clip_file = synced_clip_dir/\
             Path(self.ref_recording.new_rec_name).name
         logger.debug('editing files for %s'%synced_clip_file)
+        self.ref_recording.final_synced_file = synced_clip_file # relative
         # collecting edited audio by device, in (Device, tempfile) pairs:
         merged_audio_files_by_device = [
                             (d, self._get_concatenated_audiofile_for(d)) 
                             for d in self._get_audio_devices()]
         if len(merged_audio_files_by_device) == 0:
             # no audio file overlaps for this clip
             return
-        # split audio channels in mono wav tempfiles:    
-        edited_audio_all_devices = []
-        for device, multi_chan_audio in merged_audio_files_by_device:
-            mono_files = _split_channels(multi_chan_audio)
-            logger.debug('%i mono files for %s'%(len(mono_files), device.name))
-            dev_audio_tuples = [(device, idx, m) for idx, m
-                                            in enumerate(mono_files)]
-            edited_audio_all_devices += dev_audio_tuples
+        if len(merged_audio_files_by_device) == 1:
+            # only one audio recorder was used, pick singleton in list
+            dev, concatenate_audio_file = merged_audio_files_by_device[0]
+            logger.debug('one audio device only: %s'%dev)
+            # check if this sole recorder is stereo
+            if dev.n_chan == 2:
+                # stereo minus TTC chan = mono, check consistency:
+                nchan_sox = sox.file_info.channels(
+                    _pathname(concatenate_audio_file))
+                logger.debug('nchan_sox: %i mono?'%nchan_sox)
+                if not nchan_sox == 1:
+                    raise Exception('Error in channel processing')
+                # all OK, merge and return
+                logger.debug('simply mono to merge')
+                self.ref_recording.synced_audio = concatenate_audio_file
+                self._merge_audio_and_video()
+                return
+        # if still here, either multitracks and/or multi recorders so check if a
+        # mix has been done on location and identified as is in atracks.txt
+        # file. Split audio channels in mono wav tempfiles at the same time
+        #
         multiple_recorders = len(merged_audio_files_by_device) > 1
         logger.debug('multiple_recorder: %s'%multiple_recorders)
-        # replace device, idx pair with track name (+ device name if many)
-        def _trnm(dev, idx): # used in the list comprehension just below
-            if dev.tracks == None:
-                tag = 'chan%s'%str(idx+1).zfill(2)
-            else:
-                audio_tags = [tag for tag in dev.tracks.rawtrx
-                    if tag not in ['ttc','0','tc']]
-                tag = audio_tags[idx]
-            if multiple_recorders:
-                tag += '_' + dev.name
-            return tag
-        edited_audio_all_devices = [(_trnm(dev, idx), audio_tempfile)
-                    for dev, idx, audio_tempfile in edited_audio_all_devices]
-        logger.debug('edited_audio_all_devices %s'%edited_audio_all_devices)
-        video_path = self.ref_recording.AVpath
-        # stacked audio contains all audio recorders if many
-        mixed_audio = _sox_combine([audio for _, audio
-                in merged_audio_files_by_device]) # all devices
-        logger.debug('will merge with %s'%(_pathname(mixed_audio)))
-        self.ref_recording.synced_audio = mixed_audio
-        nchan = sox.file_info.channels(_pathname(mixed_audio))
-        logger.debug('mixed_audio n chan: %i'%nchan)
-        self.ref_recording.final_synced_file = synced_clip_file # relative
+        # dev_mixes_mix contains all audio recorders if many
+        mixes = [self._get_mix(device, multi_chan_audio)
+                for device, multi_chan_audio
+                in merged_audio_files_by_device]
+        logger.debug('thera are %i dev mixes'%len(mixes))
+        dev_mixes_mix = _sox_mix(mixes)
+        # dev_mixes_mix = _sox_combine([audio for _, audio
+        #         in merged_audio_files_by_device]) # all devices
+        logger.debug('will merge with %s'%(_pathname(dev_mixes_mix)))
+        self.ref_recording.synced_audio = dev_mixes_mix
+        logger.debug('dev_mixes_mix n chan: %i'%
+            sox.file_info.channels(_pathname(dev_mixes_mix)))
         self._merge_audio_and_video()
+        # devices_and_monofiles is list of (device, [monofiles])
+        # [(dev1, multichan1), (dev2, multichan2)] in
+        # merged_audio_files_by_device -> 
+        # [(dev1, [mono1_ch1, mono1_ch2]), (dev2, [mono2_ch1, mono2_ch2)]] in 
+        # devices_and_monofiles:
         if asked_ISOs:
-            self._write_ISOs(edited_audio_all_devices)
+            devices_and_monofiles = [(device, _split_channels(multi_chan_audio))
+                    for device, multi_chan_audio
+                    in merged_audio_files_by_device]
+            logger.debug('devices_and_monofiles: %s'%
+                pprint.pformat(devices_and_monofiles))
+            def _trnm(dev, idx): # used in the list comprehension just below
+                # generates track name for later if asked_ISOs
+                # idx is from 0 to nchan-1 for this device
+                if dev.tracks == None:
+                    tag = 'chan%s'%str(idx+1).zfill(2)
+                else:
+                    audio_tags = [tag for tag in dev.tracks.rawtrx
+                        if tag not in ['ttc','0','tc']]
+                    tag = audio_tags[idx]
+                if multiple_recorders:
+                    tag += '_' + dev.name
+                return tag
+            # replace device, idx pair with track name (+ device name if many)
+            # loop over devices than loop over tracks
+            names_audio_tempfiles = []
+            for dev, mono_tmpfiles_list in devices_and_monofiles:
+                for idx, monotf in enumerate(mono_tmpfiles_list):
+                    names_audio_tempfiles.append((_trnm(dev, idx), monotf))
+            logger.debug('names_audio_tempfiles %s'%names_audio_tempfiles)
+            self._write_ISOs(names_audio_tempfiles)
         logger.debug('merged_audio_files_by_device %s'%
             merged_audio_files_by_device)
-        for idx, pair in enumerate(merged_audio_files_by_device): # This loop for logging purpose only.
+        # This loop below for logging purpose only:
+        for idx, pair in enumerate(merged_audio_files_by_device):
             # dev_joined_audio is mono, stereo or even polywav from multitrack 
             # recorders. For one video there could be more than one dev_joined_audio
             # if multiple audio recorders where used during the take.
             # this loop is for one device at the time.
             device, dev_joined_audio = pair
             logger.debug('idx: % i device.folder: %s'%(idx, device.folder))
             nchan = sox.file_info.channels(_pathname(dev_joined_audio))
             logger.debug('dev_joined_audio: %s nchan:%i'%
                 (_pathname(dev_joined_audio), nchan))
             logger.debug('duration %f s'%
                 sox.file_info.duration(_pathname(dev_joined_audio)))
-        # generates ISOs too
-        # if asked_ISOs:
-        #     print('Writing ISO files for:')
-        #     for idx, pair in enumerate(merged_audio_files_by_device):
-        #         device, dev_joined_audio = pair
-        #         logger.debug('device %i, dev_joined_audio %s %s'%
-        #             (idx, device, _pathname(dev_joined_audio)))
-        #         self._write_ISOs_for(synced_clip_file,
-        #             device, dev_joined_audio)
 
     def _keep_VIDEO_only(self, video_path):
         # return file handle to a temp video file formed from the video_path
         # stripped of its sound
         in1 = ffmpeg.input(_pathname(video_path))
         video_extension = video_path.suffix
         silenced_opts = ["-loglevel", "quiet", "-nostats", "-hide_banner"]
@@ -638,20 +754,23 @@
         out1 = in1.output(file_handle.name, map='0:v', vcodec='copy')
         ffmpeg.run([out1.global_args(*silenced_opts)], overwrite_output=True)
         return file_handle
         # os.path.split audio channels if more than one
 
     def _merge_audio_and_video(self):
         """      
-        Calls ffmpeg to join audio and video.
+        Calls ffmpeg to join video in self.ref_recording.AVpath to
+        audio in self.ref_recording.synced_audio
 
         On entry, ref_recording.final_synced_file is a Path to an non existing
         file (contrarily to ref_recording.synced_audio).
-        On exit, ref_recording.final_synced_file points to the final synced
-        video file. Returns nothing.
+        On exit, self.ref_recording.final_synced_file points to the final synced
+        video file.
+
+        Returns nothing.
         """
         synced_clip_file = self.ref_recording.final_synced_file
         video_path = self.ref_recording.AVpath
         timecode = self.ref_recording.get_timecode()
         # self.ref_recording.synced_audio = audio_path
         audio_path = self.ref_recording.synced_audio
         vid_only_handle = self._keep_VIDEO_only(video_path)
@@ -695,15 +814,14 @@
                 video_path,
                 synced_clip_file
                 ))
             print(e)
             print(e.stderr.decode('UTF-8'))
             sys.exit(1)
 
-
 class Matcher:
     """
     Matcher looks for any video in self.recordings and for each one finds out
     all audio recordings (again in self.recordings) that time overlap
     (or against any designated 'main sound', see below). It then spawns
     AudioStitcherVideoMerger objects that do the actual file manipulations. Each video
     (and main sound) will have its AudioStitcherVideoMerger instance.
```

### Comparing `tictacsync-0.2a8/tictacsync/yaltc.py` & `tictacsync-0.3a1/tictacsync/yaltc.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,19 +787,20 @@
         return '1' if freq > mid_FSK else '0'
 
     def _get_int_from_binary_str(self, string_of_01s):
         return int(''.join(reversed(string_of_01s)),2)
         # LSB is leftmost in TicTacCode
 
     def _demod_values_are_OK(self, values_dict):
+        # TODO: use _get_timedate_from_dict rather (catching any ValueError)
         ranges = {
             'seconds': range(60),
             'minutes': range(60),
             'hours': range(24),
-            'day': range(1,32),
+            'day': range(1,32), # 32 ?
             'month': range(1,13),
             }
         for key in ranges:
             val = values_dict[key]
             ok =  val in ranges[key]
             logger.debug(
                 'checking range for %s: %i, Ok? %s'%(key, val, ok))
@@ -1249,22 +1250,26 @@
         self._read_sound_find_TicTacCode(there, SOUND_EXTRACT_LENGTH)
         if self.TicTacCode_channel is None:
             return None
         else:
             return self.decoder.get_time_in_sound_extract(plots)
 
     def _get_timedate_from_dict(self, time_dict):
-        python_datetime = datetime(
-            time_dict['year offset'] + YEAR_ZERO,
-            time_dict['month'],
-            time_dict['day'],
-            time_dict['hours'],
-            time_dict['minutes'],
-            time_dict['seconds'],
-            tzinfo=timezone.utc)
+        try:
+            python_datetime = datetime(
+                time_dict['year offset'] + YEAR_ZERO,
+                time_dict['month'],
+                time_dict['day'],
+                time_dict['hours'],
+                time_dict['minutes'],
+                time_dict['seconds'],
+                tzinfo=timezone.utc)
+        except ValueError as e:
+            print('Error converting date in _get_timedate_from_dict',e)
+            sys.exit(1)
         python_datetime += timedelta(seconds=1) # PPS precedes NMEA sequ
         return python_datetime
 
     def _two_times_are_coherent(self, t1, t2):
         """
         For error checking. This verifies if two sync pulse apart
         are correctly space with sample interval deduced from
@@ -1284,14 +1289,15 @@
         -------
         TYPE
             DESCRIPTION.
 
         """
         if t1 == None or t2 == None:
             return False
+        logger.debug('t1 : %s t2: %s'%(t1, t2))
         datetime_1 = self._get_timedate_from_dict(t1)
         datetime_2 = self._get_timedate_from_dict(t2)
         # if datetime_2 < datetime_1:
         #     return False
         sample_position_1 = t1['pulse at']
         sample_position_2 = t2['pulse at']
         samplerate = self.get_samplerate()
```

### Comparing `tictacsync-0.2a8/tictacsync.egg-info/PKG-INFO` & `tictacsync-0.3a1/tictacsync.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.2a8
+Version: 0.3a1
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -79,15 +79,15 @@
 
 To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
-    > tictacsync -p tictacsync/tests/dailies/loose/MVI_0024.MP4
+    > tictacsync -p dailies/loose/MVI_0024.MP4
 
 Typical first plot produced :
 
 ![word](https://mamot.fr/system/media_attachments/files/110/279/794/002/305/269/original/0198908c6eb5c592.png)
 
 Typical second plot produced (note the 34 [FSK](https://en.wikipedia.org/wiki/Frequency-shift_keying) encoded bits `0010111101001111100110000110010000`):
 ![slicing](https://mamot.fr/system/media_attachments/files/110/279/794/021/372/766/original/6ec62bb417115f52.png)
```


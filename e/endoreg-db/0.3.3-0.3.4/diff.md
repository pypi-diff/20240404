# Comparing `tmp/endoreg_db-0.3.3.tar.gz` & `tmp/endoreg_db-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endoreg_db-0.3.3.tar", max compression
+gzip compressed data, was "endoreg_db-0.3.4.tar", max compression
```

## Comparing `endoreg_db-0.3.3.tar` & `endoreg_db-0.3.4.tar`

### file list

```diff
@@ -1,180 +1,185 @@
--rw-r--r--   0        0        0    35149 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/LICENSE
--rw-r--r--   0        0        0       98 2024-03-05 12:16:35.964436 endoreg_db-0.3.3/README.md
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/__init__.py
--rw-r--r--   0        0        0       63 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/admin.py
--rw-r--r--   0        0        0      151 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/apps.py
--rw-r--r--   0        0        0      634 2024-03-24 14:31:29.686076 endoreg_db-0.3.3/endoreg_db/data/__init__.py
--rw-r--r--   0        0        0       86 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/active_model/data.yaml
--rw-r--r--   0        0        0     1067 2024-03-25 19:33:13.541166 endoreg_db-0.3.3/endoreg_db/data/center/data.yaml
--rw-r--r--   0        0        0      242 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/endoscope_type/data.yaml
--rw-r--r--   0        0        0     1044 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/endoscopy_processor/data.yaml
--rw-r--r--   0        0        0      330 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/examination/examinations/data.yaml
--rw-r--r--   0        0        0     1010 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/examination/time/data.yaml
--rw-r--r--   0        0        0      156 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/examination/time-type/data.yaml
--rw-r--r--   0        0        0      115 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/examination/type/data.yaml
--rw-r--r--   0        0        0      765 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/information_source/data.yaml
--rw-r--r--   0        0        0     1274 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/label/label/data.yaml
--rw-r--r--   0        0        0      339 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/label/label-set/data.yaml
--rw-r--r--   0        0        0      136 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/label/label-type/data.yaml
--rw-r--r--   0        0        0      149 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/model_type/data.yaml
--rw-r--r--   0        0        0      990 2024-03-24 20:28:31.556984 endoreg_db-0.3.3/endoreg_db/data/pdf_type/data.yaml
--rw-r--r--   0        0        0     2151 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/profession/data.yaml
--rw-r--r--   0        0        0      742 2024-03-24 18:40:23.800274 endoreg_db-0.3.3/endoreg_db/data/report_reader_flag/ukw-examination-generic.yaml
--rw-r--r--   0        0        0      493 2024-03-24 20:35:11.372513 endoreg_db-0.3.3/endoreg_db/data/report_reader_flag/ukw-histology-generic.yaml
--rw-r--r--   0        0        0      393 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/unit/data.yaml
--rw-r--r--   0        0        0      633 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/unit/length.yaml
--rw-r--r--   0        0        0      510 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/unit/volume.yaml
--rw-r--r--   0        0        0      622 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/data/unit/weight.yaml
--rw-r--r--   0        0        0       60 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/forms/__init__.py
--rw-r--r--   0        0        0      259 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/forms/settings/__init__.py
--rw-r--r--   0        0        0      116 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/forms/unit.py
--rw-r--r--   0        0        0     1379 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/_load_model_template.py
--rw-r--r--   0        0        0      974 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/delete_all.py
--rw-r--r--   0        0        0      639 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/delete_legacy_images.py
--rw-r--r--   0        0        0      574 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/delete_legacy_videos.py
--rw-r--r--   0        0        0      600 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/extract_legacy_video_frames.py
--rw-r--r--   0        0        0     1153 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/fetch_legacy_image_dataset.py
--rw-r--r--   0        0        0      947 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/fix_auth_permission.py
--rw-r--r--   0        0        0     3558 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/import_legacy_images.py
--rw-r--r--   0        0        0     2732 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/import_legacy_videos.py
--rw-r--r--   0        0        0     1337 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_active_model_data.py
--rw-r--r--   0        0        0     1329 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_ai_model_data.py
--rw-r--r--   0        0        0     3146 2024-03-24 16:07:49.128590 endoreg_db-0.3.3/endoreg_db/management/commands/load_base_db_data.py
--rw-r--r--   0        0        0     1339 2024-03-24 12:14:13.590876 endoreg_db-0.3.3/endoreg_db/management/commands/load_center_data.py
--rw-r--r--   0        0        0     1345 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_endoscope_type_data.py
--rw-r--r--   0        0        0     1365 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_endoscopy_processor_data.py
--rw-r--r--   0        0        0     2748 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_examination_data.py
--rw-r--r--   0        0        0     1347 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_information_source.py
--rw-r--r--   0        0        0     2217 2024-03-23 14:28:47.448620 endoreg_db-0.3.3/endoreg_db/management/commands/load_label_data.py
--rw-r--r--   0        0        0     1650 2024-03-24 15:32:13.299576 endoreg_db-0.3.3/endoreg_db/management/commands/load_pdf_type_data.py
--rw-r--r--   0        0        0     1321 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_profession_data.py
--rw-r--r--   0        0        0     1371 2024-03-24 14:30:40.985221 endoreg_db-0.3.3/endoreg_db/management/commands/load_report_reader_flag.py
--rw-r--r--   0        0        0     1319 2024-03-23 14:29:56.620369 endoreg_db-0.3.3/endoreg_db/management/commands/load_unit_data.py
--rw-r--r--   0        0        0     1031 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/load_user_groups.py
--rw-r--r--   0        0        0     2544 2024-03-05 11:49:34.872831 endoreg_db-0.3.3/endoreg_db/management/commands/register_ai_model.py
--rw-r--r--   0        0        0      386 2024-03-25 19:50:16.845508 endoreg_db-0.3.3/endoreg_db/management/commands/reset_celery_schedule.py
--rw-r--r--   0        0        0    33643 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/migrations/0001_initial.py
--rw-r--r--   0        0        0      935 2024-03-09 17:44:39.541452 endoreg_db-0.3.3/endoreg_db/migrations/0002_rawvideofile.py
--rw-r--r--   0        0        0      399 2024-03-09 20:44:34.505650 endoreg_db-0.3.3/endoreg_db/migrations/0003_rawvideofile_frames_required.py
--rw-r--r--   0        0        0      385 2024-03-10 12:08:15.004742 endoreg_db-0.3.3/endoreg_db/migrations/0004_rename_hash_rawvideofile_video_hash.py
--rw-r--r--   0        0        0     2658 2024-03-10 13:07:59.897688 endoreg_db-0.3.3/endoreg_db/migrations/0005_ffmpegmeta_remove_videoimportmeta_center_and_more.py
--rw-r--r--   0        0        0      809 2024-03-10 14:46:50.507015 endoreg_db-0.3.3/endoreg_db/migrations/0006_rawvideofile_center_alter_videometa_processor.py
--rw-r--r--   0        0        0      547 2024-03-10 15:05:02.392393 endoreg_db-0.3.3/endoreg_db/migrations/0007_rawvideofile_processor.py
--rw-r--r--   0        0        0      401 2024-03-10 15:45:49.956177 endoreg_db-0.3.3/endoreg_db/migrations/0008_rename_frames_required_rawvideofile_state_frames_required.py
--rw-r--r--   0        0        0     1334 2024-03-10 17:44:23.831611 endoreg_db-0.3.3/endoreg_db/migrations/0009_sensitivemeta_rawvideofile_sensitive_meta.py
--rw-r--r--   0        0        0      420 2024-03-10 17:50:57.746912 endoreg_db-0.3.3/endoreg_db/migrations/0010_rename_endoscope_serial_number_sensitivemeta_endoscope_sn.py
--rw-r--r--   0        0        0      460 2024-03-10 18:01:39.416125 endoreg_db-0.3.3/endoreg_db/migrations/0011_rawvideofile_state_sensitive_data_retrieved.py
--rw-r--r--   0        0        0     3769 2024-03-18 23:01:41.512429 endoreg_db-0.3.3/endoreg_db/migrations/0012_rawvideofile_prediction_dir_and_more.py
--rw-r--r--   0        0        0     1502 2024-03-23 15:39:16.694456 endoreg_db-0.3.3/endoreg_db/migrations/0013_rawpdffile.py
--rw-r--r--   0        0        0     1475 2024-03-23 16:45:34.578580 endoreg_db-0.3.3/endoreg_db/migrations/0014_pdftype_alter_rawpdffile_file_pdfmeta.py
--rw-r--r--   0        0        0      974 2024-03-24 09:20:42.333125 endoreg_db-0.3.3/endoreg_db/migrations/0015_rename_report_processed_rawpdffile_state_report_processed_and_more.py
--rw-r--r--   0        0        0      468 2024-03-24 10:09:24.645449 endoreg_db-0.3.3/endoreg_db/migrations/0016_rawpdffile_state_report_processing_required.py
--rw-r--r--   0        0        0     1255 2024-03-24 12:26:25.243723 endoreg_db-0.3.3/endoreg_db/migrations/0017_firstname_lastname_center_first_names_and_more.py
--rw-r--r--   0        0        0     2203 2024-03-24 14:13:22.132799 endoreg_db-0.3.3/endoreg_db/migrations/0018_reportreaderflag_reportreaderconfig.py
--rw-r--r--   0        0        0     1717 2024-03-24 14:57:24.930323 endoreg_db-0.3.3/endoreg_db/migrations/0019_pdftype_cut_off_above_lines_and_more.py
--rw-r--r--   0        0        0      412 2024-03-24 15:32:57.416398 endoreg_db-0.3.3/endoreg_db/migrations/0020_rename_endoscopy_info_line_pdftype_endoscope_info_line.py
--rw-r--r--   0        0        0      606 2024-03-24 19:02:47.832213 endoreg_db-0.3.3/endoreg_db/migrations/0021_alter_pdftype_endoscope_info_line.py
--rw-r--r--   0        0        0      574 2024-03-24 20:27:01.226316 endoreg_db-0.3.3/endoreg_db/migrations/0022_alter_pdftype_endoscope_info_line.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/migrations/__init__.py
--rw-r--r--   0        0        0     1045 2024-03-24 14:02:44.388925 endoreg_db-0.3.3/endoreg_db/models/__init__.py
--rw-r--r--   0        0        0      106 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/ai_model/__init__.py
--rw-r--r--   0        0        0      343 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/ai_model/active_model.py
--rw-r--r--   0        0        0      869 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/ai_model/model_meta.py
--rw-r--r--   0        0        0      638 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/ai_model/model_type.py
--rw-r--r--   0        0        0      270 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/ai_model/utils.py
--rw-r--r--   0        0        0      191 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/annotation/__init__.py
--rw-r--r--   0        0        0     3292 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/annotation/binary_classification_annotation_task.py
--rw-r--r--   0        0        0     1387 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/annotation/image_classification.py
--rw-r--r--   0        0        0      728 2024-03-24 13:01:29.514902 endoreg_db-0.3.3/endoreg_db/models/center.py
--rw-r--r--   0        0        0      252 2024-03-23 16:44:38.190609 endoreg_db-0.3.3/endoreg_db/models/data_file/__init__.py
--rw-r--r--   0        0        0       84 2024-03-09 17:43:37.053449 endoreg_db-0.3.3/endoreg_db/models/data_file/base_classes/__init__.py
--rw-r--r--   0        0        0     2214 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/data_file/base_classes/abstract_frame.py
--rw-r--r--   0        0        0     7406 2024-03-09 18:19:16.722853 endoreg_db-0.3.3/endoreg_db/models/data_file/base_classes/abstract_video.py
--rw-r--r--   0        0        0     1935 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/data_file/frame.py
--rw-r--r--   0        0        0     1168 2024-03-23 14:38:12.578379 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/__init__.py
--rw-r--r--   0        0        0      932 2024-03-25 19:43:24.078750 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/__init__.py
--rw-r--r--   0        0        0      716 2024-03-25 19:43:33.328547 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/pdf.py
--rw-r--r--   0        0        0     8530 2024-03-25 22:28:28.226750 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/video.py
--rw-r--r--   0        0        0     6509 2024-03-24 20:22:59.012208 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/raw_pdf.py
--rw-r--r--   0        0        0    12444 2024-03-23 16:02:01.976407 endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/raw_video.py
--rw-r--r--   0        0        0      144 2024-03-24 09:09:09.600289 endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/__init__.py
--rw-r--r--   0        0        0     2183 2024-03-24 20:32:45.325050 endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/pdf_meta.py
--rw-r--r--   0        0        0     1312 2024-03-24 09:46:50.786427 endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/sensitive_meta.py
--rw-r--r--   0        0        0     5354 2024-03-23 16:42:51.743617 endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/video_meta.py
--rw-r--r--   0        0        0     3564 2024-03-23 14:32:25.908942 endoreg_db-0.3.3/endoreg_db/models/data_file/report_file.py
--rw-r--r--   0        0        0       98 2024-03-10 13:07:44.587752 endoreg_db-0.3.3/endoreg_db/models/data_file/video/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-10 13:04:54.677453 endoreg_db-0.3.3/endoreg_db/models/data_file/video/import_meta.py
--rw-r--r--   0        0        0      673 2024-03-10 13:07:49.472732 endoreg_db-0.3.3/endoreg_db/models/data_file/video/video.py
--rw-r--r--   0        0        0     4652 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/data_file/video_segment.py
--rw-r--r--   0        0        0      183 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/examination/__init__.py
--rw-r--r--   0        0        0      834 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/examination/examination.py
--rw-r--r--   0        0        0      902 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/examination/examination_time.py
--rw-r--r--   0        0        0      767 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/examination/examination_time_type.py
--rw-r--r--   0        0        0      546 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/examination/examination_type.py
--rw-r--r--   0        0        0       99 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/hardware/__init__.py
--rw-r--r--   0        0        0     1200 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/hardware/endoscope.py
--rw-r--r--   0        0        0     5114 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/hardware/endoscopy_processor.py
--rw-r--r--   0        0        0      696 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/information_source.py
--rw-r--r--   0        0        0       45 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/label/__init__.py
--rw-r--r--   0        0        0     2156 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/label/label.py
--rw-r--r--   0        0        0      115 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/legacy_data/__init__.py
--rw-r--r--   0        0        0     1622 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/legacy_data/image.py
--rw-r--r--   0        0        0     1674 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/patient_examination/__init__.py
--rw-r--r--   0        0        0     1766 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/permissions/__init__.py
--rw-r--r--   0        0        0      250 2024-03-24 12:13:55.398954 endoreg_db-0.3.3/endoreg_db/models/persons/__init__.py
--rw-r--r--   0        0        0       92 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/examiner/__init__.py
--rw-r--r--   0        0        0      422 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/examiner/examiner.py
--rw-r--r--   0        0        0       72 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/examiner/examiner_type.py
--rw-r--r--   0        0        0      456 2024-03-24 11:48:51.872780 endoreg_db-0.3.3/endoreg_db/models/persons/first_name.py
--rw-r--r--   0        0        0      501 2024-03-24 11:48:10.741946 endoreg_db-0.3.3/endoreg_db/models/persons/last_name.py
--rw-r--r--   0        0        0     2396 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/patient.py
--rw-r--r--   0        0        0     1096 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/person.py
--rw-r--r--   0        0        0      969 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/persons/portal_user_information.py
--rw-r--r--   0        0        0      145 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/prediction/__init__.py
--rw-r--r--   0        0        0     1619 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/prediction/image_classification.py
--rw-r--r--   0        0        0     9492 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/prediction/video_prediction_meta.py
--rw-r--r--   0        0        0      101 2024-03-24 14:02:11.662855 endoreg_db-0.3.3/endoreg_db/models/report_reader/__init__.py
--rw-r--r--   0        0        0     2353 2024-03-24 14:13:15.086810 endoreg_db-0.3.3/endoreg_db/models/report_reader/report_reader_config.py
--rw-r--r--   0        0        0      536 2024-03-24 13:38:25.338358 endoreg_db-0.3.3/endoreg_db/models/report_reader/report_reader_flag.py
--rw-r--r--   0        0        0      774 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models/unit.py
--rw-r--r--   0        0        0       57 2024-03-05 11:49:34.873831 endoreg_db-0.3.3/endoreg_db/models.py
--rw-r--r--   0        0        0       83 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/__init__.py
--rw-r--r--   0        0        0       95 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/annotations/__init__.py
--rw-r--r--   0        0        0     6442 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/annotations/legacy.py
--rw-r--r--   0        0        0      147 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/annotation.py
--rw-r--r--   0        0        0     1155 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/center.py
--rw-r--r--   0        0        0      371 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/model.py
--rw-r--r--   0        0        0      358 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/patient.py
--rw-r--r--   0        0        0      728 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/patient_examination.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/prediction.py
--rw-r--r--   0        0        0      976 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/report_file.py
--rw-r--r--   0        0        0      887 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/video.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/video_import_meta.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/get/video_prediction_meta.py
--rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/queries/sanity/__init_.py
--rw-r--r--   0        0        0      235 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/__init__.py
--rw-r--r--   0        0        0      579 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/ai_model.py
--rw-r--r--   0        0        0      707 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/annotation.py
--rw-r--r--   0        0        0      207 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/center.py
--rw-r--r--   0        0        0      876 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/examination.py
--rw-r--r--   0        0        0      337 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/frame.py
--rw-r--r--   0        0        0      534 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/hardware.py
--rw-r--r--   0        0        0      490 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/label.py
--rw-r--r--   0        0        0      209 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/patient.py
--rw-r--r--   0        0        0      462 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/prediction.py
--rw-r--r--   0        0        0      208 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/report_file.py
--rw-r--r--   0        0        0      831 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/serializers/video.py
--rw-r--r--   0        0        0       60 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/tests.py
--rw-r--r--   0        0        0       49 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/utils/__init__.py
--rw-r--r--   0        0        0     1143 2024-03-10 16:59:25.021336 endoreg_db-0.3.3/endoreg_db/utils/cropping.py
--rw-r--r--   0        0        0     9129 2024-03-24 16:06:21.606922 endoreg_db-0.3.3/endoreg_db/utils/dataloader.py
--rw-r--r--   0        0        0      884 2024-03-10 19:11:38.341876 endoreg_db-0.3.3/endoreg_db/utils/file_operations.py
--rw-r--r--   0        0        0     1069 2024-03-23 14:06:20.493397 endoreg_db-0.3.3/endoreg_db/utils/hashs.py
--rw-r--r--   0        0        0     7633 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/utils/legacy_ocr.py
--rw-r--r--   0        0        0     7322 2024-03-10 17:31:08.360057 endoreg_db-0.3.3/endoreg_db/utils/ocr.py
--rw-r--r--   0        0        0       53 2024-03-05 17:01:14.457967 endoreg_db-0.3.3/endoreg_db/utils/uuid.py
--rw-r--r--   0        0        0     2613 2024-03-10 15:08:21.659998 endoreg_db-0.3.3/endoreg_db/utils/video_metadata.py
--rw-r--r--   0        0        0       63 2024-03-05 11:49:34.874831 endoreg_db-0.3.3/endoreg_db/views.py
--rw-r--r--   0        0        0      560 2024-03-25 22:51:15.833958 endoreg_db-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 endoreg_db-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/LICENSE
+-rw-r--r--   0        0        0       98 2024-03-05 12:16:35.964436 endoreg_db-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/__init__.py
+-rw-r--r--   0        0        0       63 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/admin.py
+-rw-r--r--   0        0        0      151 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/apps.py
+-rw-r--r--   0        0        0      634 2024-03-24 14:31:29.686076 endoreg_db-0.3.4/endoreg_db/data/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/active_model/data.yaml
+-rw-r--r--   0        0        0     1067 2024-03-25 19:33:13.541166 endoreg_db-0.3.4/endoreg_db/data/center/data.yaml
+-rw-r--r--   0        0        0      242 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/endoscope_type/data.yaml
+-rw-r--r--   0        0        0     1044 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/endoscopy_processor/data.yaml
+-rw-r--r--   0        0        0      330 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/examination/examinations/data.yaml
+-rw-r--r--   0        0        0     1010 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/examination/time/data.yaml
+-rw-r--r--   0        0        0      156 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/examination/time-type/data.yaml
+-rw-r--r--   0        0        0      115 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/examination/type/data.yaml
+-rw-r--r--   0        0        0      765 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/information_source/data.yaml
+-rw-r--r--   0        0        0     1274 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/label/label/data.yaml
+-rw-r--r--   0        0        0      339 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/label/label-set/data.yaml
+-rw-r--r--   0        0        0      136 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/label/label-type/data.yaml
+-rw-r--r--   0        0        0      149 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/model_type/data.yaml
+-rw-r--r--   0        0        0      990 2024-03-24 20:28:31.556984 endoreg_db-0.3.4/endoreg_db/data/pdf_type/data.yaml
+-rw-r--r--   0        0        0     2151 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/profession/data.yaml
+-rw-r--r--   0        0        0      742 2024-03-24 18:40:23.800274 endoreg_db-0.3.4/endoreg_db/data/report_reader_flag/ukw-examination-generic.yaml
+-rw-r--r--   0        0        0      493 2024-03-24 20:35:11.372513 endoreg_db-0.3.4/endoreg_db/data/report_reader_flag/ukw-histology-generic.yaml
+-rw-r--r--   0        0        0      393 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/unit/data.yaml
+-rw-r--r--   0        0        0      633 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/unit/length.yaml
+-rw-r--r--   0        0        0      510 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/unit/volume.yaml
+-rw-r--r--   0        0        0      622 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/data/unit/weight.yaml
+-rw-r--r--   0        0        0       90 2024-04-02 15:55:04.110678 endoreg_db-0.3.4/endoreg_db/forms/__init__.py
+-rw-r--r--   0        0        0       75 2024-04-02 15:58:51.586485 endoreg_db-0.3.4/endoreg_db/forms/questionnaires/__init__.py
+-rw-r--r--   0        0        0      890 2024-04-02 16:09:37.476360 endoreg_db-0.3.4/endoreg_db/forms/questionnaires/tto_questionnaire.py
+-rw-r--r--   0        0        0      259 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/forms/settings/__init__.py
+-rw-r--r--   0        0        0      116 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/forms/unit.py
+-rw-r--r--   0        0        0     1379 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/_load_model_template.py
+-rw-r--r--   0        0        0      974 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/delete_all.py
+-rw-r--r--   0        0        0      639 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/delete_legacy_images.py
+-rw-r--r--   0        0        0      574 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/delete_legacy_videos.py
+-rw-r--r--   0        0        0      600 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/extract_legacy_video_frames.py
+-rw-r--r--   0        0        0     1153 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/fetch_legacy_image_dataset.py
+-rw-r--r--   0        0        0      947 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/fix_auth_permission.py
+-rw-r--r--   0        0        0     3558 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/import_legacy_images.py
+-rw-r--r--   0        0        0     2732 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/import_legacy_videos.py
+-rw-r--r--   0        0        0     1337 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_active_model_data.py
+-rw-r--r--   0        0        0     1329 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_ai_model_data.py
+-rw-r--r--   0        0        0     3146 2024-03-24 16:07:49.128590 endoreg_db-0.3.4/endoreg_db/management/commands/load_base_db_data.py
+-rw-r--r--   0        0        0     1339 2024-03-24 12:14:13.590876 endoreg_db-0.3.4/endoreg_db/management/commands/load_center_data.py
+-rw-r--r--   0        0        0     1345 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_endoscope_type_data.py
+-rw-r--r--   0        0        0     1365 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_endoscopy_processor_data.py
+-rw-r--r--   0        0        0     2748 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_examination_data.py
+-rw-r--r--   0        0        0     1347 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_information_source.py
+-rw-r--r--   0        0        0     2217 2024-03-23 14:28:47.448620 endoreg_db-0.3.4/endoreg_db/management/commands/load_label_data.py
+-rw-r--r--   0        0        0     1650 2024-03-24 15:32:13.299576 endoreg_db-0.3.4/endoreg_db/management/commands/load_pdf_type_data.py
+-rw-r--r--   0        0        0     1321 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_profession_data.py
+-rw-r--r--   0        0        0     1371 2024-03-24 14:30:40.985221 endoreg_db-0.3.4/endoreg_db/management/commands/load_report_reader_flag.py
+-rw-r--r--   0        0        0     1319 2024-03-23 14:29:56.620369 endoreg_db-0.3.4/endoreg_db/management/commands/load_unit_data.py
+-rw-r--r--   0        0        0     1031 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/load_user_groups.py
+-rw-r--r--   0        0        0     2544 2024-03-05 11:49:34.872831 endoreg_db-0.3.4/endoreg_db/management/commands/register_ai_model.py
+-rw-r--r--   0        0        0      386 2024-03-25 19:50:16.845508 endoreg_db-0.3.4/endoreg_db/management/commands/reset_celery_schedule.py
+-rw-r--r--   0        0        0    33643 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/migrations/0001_initial.py
+-rw-r--r--   0        0        0      935 2024-03-09 17:44:39.541452 endoreg_db-0.3.4/endoreg_db/migrations/0002_rawvideofile.py
+-rw-r--r--   0        0        0      399 2024-03-09 20:44:34.505650 endoreg_db-0.3.4/endoreg_db/migrations/0003_rawvideofile_frames_required.py
+-rw-r--r--   0        0        0      385 2024-03-10 12:08:15.004742 endoreg_db-0.3.4/endoreg_db/migrations/0004_rename_hash_rawvideofile_video_hash.py
+-rw-r--r--   0        0        0     2658 2024-03-10 13:07:59.897688 endoreg_db-0.3.4/endoreg_db/migrations/0005_ffmpegmeta_remove_videoimportmeta_center_and_more.py
+-rw-r--r--   0        0        0      809 2024-03-10 14:46:50.507015 endoreg_db-0.3.4/endoreg_db/migrations/0006_rawvideofile_center_alter_videometa_processor.py
+-rw-r--r--   0        0        0      547 2024-03-10 15:05:02.392393 endoreg_db-0.3.4/endoreg_db/migrations/0007_rawvideofile_processor.py
+-rw-r--r--   0        0        0      401 2024-03-10 15:45:49.956177 endoreg_db-0.3.4/endoreg_db/migrations/0008_rename_frames_required_rawvideofile_state_frames_required.py
+-rw-r--r--   0        0        0     1334 2024-03-10 17:44:23.831611 endoreg_db-0.3.4/endoreg_db/migrations/0009_sensitivemeta_rawvideofile_sensitive_meta.py
+-rw-r--r--   0        0        0      420 2024-03-10 17:50:57.746912 endoreg_db-0.3.4/endoreg_db/migrations/0010_rename_endoscope_serial_number_sensitivemeta_endoscope_sn.py
+-rw-r--r--   0        0        0      460 2024-03-10 18:01:39.416125 endoreg_db-0.3.4/endoreg_db/migrations/0011_rawvideofile_state_sensitive_data_retrieved.py
+-rw-r--r--   0        0        0     3769 2024-03-18 23:01:41.512429 endoreg_db-0.3.4/endoreg_db/migrations/0012_rawvideofile_prediction_dir_and_more.py
+-rw-r--r--   0        0        0     1502 2024-03-23 15:39:16.694456 endoreg_db-0.3.4/endoreg_db/migrations/0013_rawpdffile.py
+-rw-r--r--   0        0        0     1475 2024-03-23 16:45:34.578580 endoreg_db-0.3.4/endoreg_db/migrations/0014_pdftype_alter_rawpdffile_file_pdfmeta.py
+-rw-r--r--   0        0        0      974 2024-03-24 09:20:42.333125 endoreg_db-0.3.4/endoreg_db/migrations/0015_rename_report_processed_rawpdffile_state_report_processed_and_more.py
+-rw-r--r--   0        0        0      468 2024-03-24 10:09:24.645449 endoreg_db-0.3.4/endoreg_db/migrations/0016_rawpdffile_state_report_processing_required.py
+-rw-r--r--   0        0        0     1255 2024-03-24 12:26:25.243723 endoreg_db-0.3.4/endoreg_db/migrations/0017_firstname_lastname_center_first_names_and_more.py
+-rw-r--r--   0        0        0     2203 2024-03-24 14:13:22.132799 endoreg_db-0.3.4/endoreg_db/migrations/0018_reportreaderflag_reportreaderconfig.py
+-rw-r--r--   0        0        0     1717 2024-03-24 14:57:24.930323 endoreg_db-0.3.4/endoreg_db/migrations/0019_pdftype_cut_off_above_lines_and_more.py
+-rw-r--r--   0        0        0      412 2024-03-24 15:32:57.416398 endoreg_db-0.3.4/endoreg_db/migrations/0020_rename_endoscopy_info_line_pdftype_endoscope_info_line.py
+-rw-r--r--   0        0        0      606 2024-03-24 19:02:47.832213 endoreg_db-0.3.4/endoreg_db/migrations/0021_alter_pdftype_endoscope_info_line.py
+-rw-r--r--   0        0        0      574 2024-03-24 20:27:01.226316 endoreg_db-0.3.4/endoreg_db/migrations/0022_alter_pdftype_endoscope_info_line.py
+-rw-r--r--   0        0        0     5828 2024-04-02 16:03:51.134458 endoreg_db-0.3.4/endoreg_db/migrations/0023_ttoquestionnaire_alter_pdftype_endoscope_info_line.py
+-rw-r--r--   0        0        0      812 2024-04-02 16:36:05.647357 endoreg_db-0.3.4/endoreg_db/migrations/0024_remove_ttoquestionnaire_infections_and_more.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/migrations/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-02 16:02:00.683976 endoreg_db-0.3.4/endoreg_db/models/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/ai_model/__init__.py
+-rw-r--r--   0        0        0      343 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/ai_model/active_model.py
+-rw-r--r--   0        0        0      869 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/ai_model/model_meta.py
+-rw-r--r--   0        0        0      638 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/ai_model/model_type.py
+-rw-r--r--   0        0        0      270 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/ai_model/utils.py
+-rw-r--r--   0        0        0      191 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/annotation/__init__.py
+-rw-r--r--   0        0        0     3292 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/annotation/binary_classification_annotation_task.py
+-rw-r--r--   0        0        0     1387 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/annotation/image_classification.py
+-rw-r--r--   0        0        0      728 2024-03-24 13:01:29.514902 endoreg_db-0.3.4/endoreg_db/models/center.py
+-rw-r--r--   0        0        0      252 2024-03-23 16:44:38.190609 endoreg_db-0.3.4/endoreg_db/models/data_file/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-09 17:43:37.053449 endoreg_db-0.3.4/endoreg_db/models/data_file/base_classes/__init__.py
+-rw-r--r--   0        0        0     2214 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/data_file/base_classes/abstract_frame.py
+-rw-r--r--   0        0        0     7406 2024-03-09 18:19:16.722853 endoreg_db-0.3.4/endoreg_db/models/data_file/base_classes/abstract_video.py
+-rw-r--r--   0        0        0     1935 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/data_file/frame.py
+-rw-r--r--   0        0        0     1168 2024-03-23 14:38:12.578379 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/__init__.py
+-rw-r--r--   0        0        0      932 2024-03-25 19:43:24.078750 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/__init__.py
+-rw-r--r--   0        0        0      716 2024-03-25 19:43:33.328547 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/pdf.py
+-rw-r--r--   0        0        0     8530 2024-03-25 22:28:28.226750 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/video.py
+-rw-r--r--   0        0        0     6509 2024-03-24 20:22:59.012208 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/raw_pdf.py
+-rw-r--r--   0        0        0    12444 2024-03-23 16:02:01.976407 endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/raw_video.py
+-rw-r--r--   0        0        0      144 2024-03-24 09:09:09.600289 endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/__init__.py
+-rw-r--r--   0        0        0     2183 2024-03-24 20:32:45.325050 endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/pdf_meta.py
+-rw-r--r--   0        0        0     1312 2024-03-24 09:46:50.786427 endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/sensitive_meta.py
+-rw-r--r--   0        0        0     5354 2024-03-23 16:42:51.743617 endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/video_meta.py
+-rw-r--r--   0        0        0     3564 2024-03-23 14:32:25.908942 endoreg_db-0.3.4/endoreg_db/models/data_file/report_file.py
+-rw-r--r--   0        0        0       98 2024-03-10 13:07:44.587752 endoreg_db-0.3.4/endoreg_db/models/data_file/video/__init__.py
+-rw-r--r--   0        0        0     1311 2024-03-10 13:04:54.677453 endoreg_db-0.3.4/endoreg_db/models/data_file/video/import_meta.py
+-rw-r--r--   0        0        0      673 2024-03-10 13:07:49.472732 endoreg_db-0.3.4/endoreg_db/models/data_file/video/video.py
+-rw-r--r--   0        0        0     4652 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/data_file/video_segment.py
+-rw-r--r--   0        0        0      183 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/examination/__init__.py
+-rw-r--r--   0        0        0      834 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/examination/examination.py
+-rw-r--r--   0        0        0      902 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/examination/examination_time.py
+-rw-r--r--   0        0        0      767 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/examination/examination_time_type.py
+-rw-r--r--   0        0        0      546 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/examination/examination_type.py
+-rw-r--r--   0        0        0       99 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/hardware/__init__.py
+-rw-r--r--   0        0        0     1200 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/hardware/endoscope.py
+-rw-r--r--   0        0        0     5114 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/hardware/endoscopy_processor.py
+-rw-r--r--   0        0        0      696 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/information_source.py
+-rw-r--r--   0        0        0       45 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/label/__init__.py
+-rw-r--r--   0        0        0     2156 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/label/label.py
+-rw-r--r--   0        0        0      115 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/legacy_data/__init__.py
+-rw-r--r--   0        0        0     1622 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/legacy_data/image.py
+-rw-r--r--   0        0        0     1674 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/patient_examination/__init__.py
+-rw-r--r--   0        0        0     1766 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/permissions/__init__.py
+-rw-r--r--   0        0        0      250 2024-03-24 12:13:55.398954 endoreg_db-0.3.4/endoreg_db/models/persons/__init__.py
+-rw-r--r--   0        0        0       92 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/examiner/__init__.py
+-rw-r--r--   0        0        0      422 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/examiner/examiner.py
+-rw-r--r--   0        0        0       72 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/examiner/examiner_type.py
+-rw-r--r--   0        0        0      456 2024-03-24 11:48:51.872780 endoreg_db-0.3.4/endoreg_db/models/persons/first_name.py
+-rw-r--r--   0        0        0      501 2024-03-24 11:48:10.741946 endoreg_db-0.3.4/endoreg_db/models/persons/last_name.py
+-rw-r--r--   0        0        0     2396 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/patient.py
+-rw-r--r--   0        0        0     1096 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/person.py
+-rw-r--r--   0        0        0      969 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/persons/portal_user_information.py
+-rw-r--r--   0        0        0      145 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/prediction/__init__.py
+-rw-r--r--   0        0        0     1619 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/prediction/image_classification.py
+-rw-r--r--   0        0        0     9492 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/prediction/video_prediction_meta.py
+-rw-r--r--   0        0        0     6029 2024-04-02 16:31:37.241753 endoreg_db-0.3.4/endoreg_db/models/questionnaires/__init__.py
+-rw-r--r--   0        0        0      101 2024-03-24 14:02:11.662855 endoreg_db-0.3.4/endoreg_db/models/report_reader/__init__.py
+-rw-r--r--   0        0        0     2353 2024-03-24 14:13:15.086810 endoreg_db-0.3.4/endoreg_db/models/report_reader/report_reader_config.py
+-rw-r--r--   0        0        0      536 2024-03-24 13:38:25.338358 endoreg_db-0.3.4/endoreg_db/models/report_reader/report_reader_flag.py
+-rw-r--r--   0        0        0      774 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models/unit.py
+-rw-r--r--   0        0        0       57 2024-03-05 11:49:34.873831 endoreg_db-0.3.4/endoreg_db/models.py
+-rw-r--r--   0        0        0       83 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/__init__.py
+-rw-r--r--   0        0        0       95 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/annotations/__init__.py
+-rw-r--r--   0        0        0     6442 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/annotations/legacy.py
+-rw-r--r--   0        0        0      147 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/annotation.py
+-rw-r--r--   0        0        0     1155 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/center.py
+-rw-r--r--   0        0        0      371 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/model.py
+-rw-r--r--   0        0        0      358 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/patient.py
+-rw-r--r--   0        0        0      728 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/patient_examination.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/prediction.py
+-rw-r--r--   0        0        0      976 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/report_file.py
+-rw-r--r--   0        0        0      887 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/video.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/video_import_meta.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/get/video_prediction_meta.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/queries/sanity/__init_.py
+-rw-r--r--   0        0        0      235 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/ai_model.py
+-rw-r--r--   0        0        0      707 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/annotation.py
+-rw-r--r--   0        0        0      207 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/center.py
+-rw-r--r--   0        0        0      876 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/examination.py
+-rw-r--r--   0        0        0      337 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/frame.py
+-rw-r--r--   0        0        0      534 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/hardware.py
+-rw-r--r--   0        0        0      490 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/label.py
+-rw-r--r--   0        0        0      209 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/patient.py
+-rw-r--r--   0        0        0      462 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/prediction.py
+-rw-r--r--   0        0        0      208 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/report_file.py
+-rw-r--r--   0        0        0      831 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/serializers/video.py
+-rw-r--r--   0        0        0       60 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/tests.py
+-rw-r--r--   0        0        0       49 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/utils/__init__.py
+-rw-r--r--   0        0        0     1143 2024-03-10 16:59:25.021336 endoreg_db-0.3.4/endoreg_db/utils/cropping.py
+-rw-r--r--   0        0        0     9129 2024-03-24 16:06:21.606922 endoreg_db-0.3.4/endoreg_db/utils/dataloader.py
+-rw-r--r--   0        0        0      884 2024-03-10 19:11:38.341876 endoreg_db-0.3.4/endoreg_db/utils/file_operations.py
+-rw-r--r--   0        0        0     1069 2024-03-23 14:06:20.493397 endoreg_db-0.3.4/endoreg_db/utils/hashs.py
+-rw-r--r--   0        0        0     7633 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/utils/legacy_ocr.py
+-rw-r--r--   0        0        0     7322 2024-03-10 17:31:08.360057 endoreg_db-0.3.4/endoreg_db/utils/ocr.py
+-rw-r--r--   0        0        0       53 2024-03-05 17:01:14.457967 endoreg_db-0.3.4/endoreg_db/utils/uuid.py
+-rw-r--r--   0        0        0     2613 2024-03-10 15:08:21.659998 endoreg_db-0.3.4/endoreg_db/utils/video_metadata.py
+-rw-r--r--   0        0        0       63 2024-03-05 11:49:34.874831 endoreg_db-0.3.4/endoreg_db/views.py
+-rw-r--r--   0        0        0      560 2024-04-04 09:23:11.444230 endoreg_db-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 endoreg_db-0.3.4/PKG-INFO
```

### Comparing `endoreg_db-0.3.3/LICENSE` & `endoreg_db-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/__init__.py` & `endoreg_db-0.3.4/endoreg_db/data/__init__.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/center/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/center/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/endoscopy_processor/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/endoscopy_processor/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/examination/time/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/examination/time/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/information_source/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/information_source/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/label/label/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/label/label/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/pdf_type/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/pdf_type/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/profession/data.yaml` & `endoreg_db-0.3.4/endoreg_db/data/profession/data.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/report_reader_flag/ukw-examination-generic.yaml` & `endoreg_db-0.3.4/endoreg_db/data/report_reader_flag/ukw-examination-generic.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/unit/length.yaml` & `endoreg_db-0.3.4/endoreg_db/data/unit/length.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/data/unit/weight.yaml` & `endoreg_db-0.3.4/endoreg_db/data/unit/weight.yaml`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/_load_model_template.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/_load_model_template.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/delete_all.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/delete_all.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/delete_legacy_images.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/delete_legacy_images.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/delete_legacy_videos.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/delete_legacy_videos.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/extract_legacy_video_frames.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/extract_legacy_video_frames.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/fetch_legacy_image_dataset.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/fetch_legacy_image_dataset.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/fix_auth_permission.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/fix_auth_permission.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/import_legacy_images.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/import_legacy_images.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/import_legacy_videos.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/import_legacy_videos.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_active_model_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_active_model_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_ai_model_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_ai_model_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_base_db_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_base_db_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_center_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_center_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_endoscope_type_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_endoscope_type_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_endoscopy_processor_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_endoscopy_processor_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_examination_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_examination_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_information_source.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_information_source.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_label_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_label_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_pdf_type_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_pdf_type_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_profession_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_profession_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_report_reader_flag.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_report_reader_flag.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_unit_data.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_unit_data.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/load_user_groups.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/load_user_groups.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/management/commands/register_ai_model.py` & `endoreg_db-0.3.4/endoreg_db/management/commands/register_ai_model.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0001_initial.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0002_rawvideofile.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0002_rawvideofile.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0005_ffmpegmeta_remove_videoimportmeta_center_and_more.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0005_ffmpegmeta_remove_videoimportmeta_center_and_more.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0006_rawvideofile_center_alter_videometa_processor.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0006_rawvideofile_center_alter_videometa_processor.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0007_rawvideofile_processor.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0007_rawvideofile_processor.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0009_sensitivemeta_rawvideofile_sensitive_meta.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0009_sensitivemeta_rawvideofile_sensitive_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0012_rawvideofile_prediction_dir_and_more.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0012_rawvideofile_prediction_dir_and_more.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0013_rawpdffile.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0013_rawpdffile.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0014_pdftype_alter_rawpdffile_file_pdfmeta.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0014_pdftype_alter_rawpdffile_file_pdfmeta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0015_rename_report_processed_rawpdffile_state_report_processed_and_more.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0015_rename_report_processed_rawpdffile_state_report_processed_and_more.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0017_firstname_lastname_center_first_names_and_more.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0017_firstname_lastname_center_first_names_and_more.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0018_reportreaderflag_reportreaderconfig.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0018_reportreaderflag_reportreaderconfig.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0019_pdftype_cut_off_above_lines_and_more.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0019_pdftype_cut_off_above_lines_and_more.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0021_alter_pdftype_endoscope_info_line.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0021_alter_pdftype_endoscope_info_line.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/migrations/0022_alter_pdftype_endoscope_info_line.py` & `endoreg_db-0.3.4/endoreg_db/migrations/0022_alter_pdftype_endoscope_info_line.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/__init__.py` & `endoreg_db-0.3.4/endoreg_db/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,7 +49,9 @@
 )
 
 from .hardware import (
     EndoscopyProcessor,
     Endoscope,
     EndoscopeType,
 )
+
+from .questionnaires import TtoQuestionnaire
```

### Comparing `endoreg_db-0.3.3/endoreg_db/models/ai_model/model_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/ai_model/model_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/ai_model/model_type.py` & `endoreg_db-0.3.4/endoreg_db/models/ai_model/model_type.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/annotation/binary_classification_annotation_task.py` & `endoreg_db-0.3.4/endoreg_db/models/annotation/binary_classification_annotation_task.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/annotation/image_classification.py` & `endoreg_db-0.3.4/endoreg_db/models/annotation/image_classification.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/center.py` & `endoreg_db-0.3.4/endoreg_db/models/center.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/base_classes/abstract_frame.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/base_classes/abstract_frame.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/base_classes/abstract_video.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/base_classes/abstract_video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/frame.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/frame.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/__init__.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/__init__.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/pdf.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/pdf.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/processing_functions/video.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/processing_functions/video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/raw_pdf.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/raw_pdf.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/import_classes/raw_video.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/import_classes/raw_video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/pdf_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/pdf_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/sensitive_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/sensitive_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/metadata/video_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/metadata/video_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/report_file.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/report_file.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/video/import_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/video/import_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/video/video.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/video/video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/data_file/video_segment.py` & `endoreg_db-0.3.4/endoreg_db/models/data_file/video_segment.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/examination/examination.py` & `endoreg_db-0.3.4/endoreg_db/models/examination/examination.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/examination/examination_time.py` & `endoreg_db-0.3.4/endoreg_db/models/examination/examination_time.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/examination/examination_time_type.py` & `endoreg_db-0.3.4/endoreg_db/models/examination/examination_time_type.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/examination/examination_type.py` & `endoreg_db-0.3.4/endoreg_db/models/examination/examination_type.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/hardware/endoscope.py` & `endoreg_db-0.3.4/endoreg_db/models/hardware/endoscope.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/hardware/endoscopy_processor.py` & `endoreg_db-0.3.4/endoreg_db/models/hardware/endoscopy_processor.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/information_source.py` & `endoreg_db-0.3.4/endoreg_db/models/information_source.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/label/label.py` & `endoreg_db-0.3.4/endoreg_db/models/label/label.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/legacy_data/image.py` & `endoreg_db-0.3.4/endoreg_db/models/legacy_data/image.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/patient_examination/__init__.py` & `endoreg_db-0.3.4/endoreg_db/models/patient_examination/__init__.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/permissions/__init__.py` & `endoreg_db-0.3.4/endoreg_db/models/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/persons/patient.py` & `endoreg_db-0.3.4/endoreg_db/models/persons/patient.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/persons/person.py` & `endoreg_db-0.3.4/endoreg_db/models/persons/person.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/persons/portal_user_information.py` & `endoreg_db-0.3.4/endoreg_db/models/persons/portal_user_information.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/prediction/image_classification.py` & `endoreg_db-0.3.4/endoreg_db/models/prediction/image_classification.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/prediction/video_prediction_meta.py` & `endoreg_db-0.3.4/endoreg_db/models/prediction/video_prediction_meta.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/report_reader/report_reader_config.py` & `endoreg_db-0.3.4/endoreg_db/models/report_reader/report_reader_config.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/report_reader/report_reader_flag.py` & `endoreg_db-0.3.4/endoreg_db/models/report_reader/report_reader_flag.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/models/unit.py` & `endoreg_db-0.3.4/endoreg_db/models/unit.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/queries/annotations/legacy.py` & `endoreg_db-0.3.4/endoreg_db/queries/annotations/legacy.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/queries/get/center.py` & `endoreg_db-0.3.4/endoreg_db/queries/get/center.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/queries/get/patient_examination.py` & `endoreg_db-0.3.4/endoreg_db/queries/get/patient_examination.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/queries/get/report_file.py` & `endoreg_db-0.3.4/endoreg_db/queries/get/report_file.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/queries/get/video.py` & `endoreg_db-0.3.4/endoreg_db/queries/get/video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/serializers/ai_model.py` & `endoreg_db-0.3.4/endoreg_db/serializers/ai_model.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/serializers/annotation.py` & `endoreg_db-0.3.4/endoreg_db/serializers/annotation.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/serializers/examination.py` & `endoreg_db-0.3.4/endoreg_db/serializers/examination.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/serializers/hardware.py` & `endoreg_db-0.3.4/endoreg_db/serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/serializers/video.py` & `endoreg_db-0.3.4/endoreg_db/serializers/video.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/cropping.py` & `endoreg_db-0.3.4/endoreg_db/utils/cropping.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/dataloader.py` & `endoreg_db-0.3.4/endoreg_db/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/file_operations.py` & `endoreg_db-0.3.4/endoreg_db/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/hashs.py` & `endoreg_db-0.3.4/endoreg_db/utils/hashs.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/legacy_ocr.py` & `endoreg_db-0.3.4/endoreg_db/utils/legacy_ocr.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/ocr.py` & `endoreg_db-0.3.4/endoreg_db/utils/ocr.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/endoreg_db/utils/video_metadata.py` & `endoreg_db-0.3.4/endoreg_db/utils/video_metadata.py`

 * *Files identical despite different names*

### Comparing `endoreg_db-0.3.3/pyproject.toml` & `endoreg_db-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "endoreg-db"
-version = "0.3.3"
+version = "0.3.4"
 description = "EndoReg Db Django App"
 authors = ["Thomas J. Lux"]
 license = "GNU3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `endoreg_db-0.3.3/PKG-INFO` & `endoreg_db-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endoreg-db
-Version: 0.3.3
+Version: 0.3.4
 Summary: EndoReg Db Django App
 License: GNU3
 Author: Thomas J. Lux
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


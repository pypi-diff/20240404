# Comparing `tmp/cumulus_library_covid-0.2.2.tar.gz` & `tmp/cumulus_library_covid-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_covid-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_covid-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_covid-0.2.2.tar` & `cumulus_library_covid-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1048 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/__init__.py
--rw-r--r--   0        0        0        0 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/__init__.py
--rw-r--r--   0        0        0     3782 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/counts.py
--rw-r--r--   0        0        0    10373 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/counts.sql
--rw-r--r--   0        0        0     2678 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_age_general.sql
--rw-r--r--   0        0        0      600 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
--rw-r--r--   0        0        0      192 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
--rw-r--r--   0        0        0     4154 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
--rw-r--r--   0        0        0     1586 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_ed_note.sql
--rw-r--r--   0        0        0     8576 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr.sql
--rw-r--r--   0        0        0     1522 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
--rw-r--r--   0        0        0     2022 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
--rw-r--r--   0        0        0     2747 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
--rw-r--r--   0        0        0      732 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_study_period.sql
--rw-r--r--   0        0        0      731 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_symptom.py
--rw-r--r--   0        0        0    16063 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_symptom.sql
--rw-r--r--   0        0        0     1209 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/manifest.toml
--rw-r--r--   0        0        0      841 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_dx.sql
--rw-r--r--   0        0        0     1583 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_pcr.sql
--rw-r--r--   0        0        0     1479 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
--rw-r--r--   0        0        0     1070 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_study_period.sql
--rw-r--r--   0        0        0     2289 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_symptom.sql
--rw-r--r--   0        0        0     2522 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/typesystem.py
--rw-r--r--   0        0        0     1905 2023-10-23 16:10:00.857675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
--rw-r--r--   0        0        0     5415 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
--rw-r--r--   0        0        0     3376 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
--rw-r--r--   0        0        0     4037 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
--rw-r--r--   0        0        0     4602 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
--rw-r--r--   0        0        0     3369 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
--rw-r--r--   0        0        0     8196 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
--rw-r--r--   0        0        0       78 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/version.sql
--rw-r--r--   0        0        0      970 2023-10-23 16:10:00.861675 cumulus_library_covid-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 cumulus_library_covid-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1336 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/__init__.py
+-rw-r--r--   0        0        0     3796 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/counts.py
+-rw-r--r--   0        0        0    30420 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/counts.sql
+-rw-r--r--   0        0        0     2678 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_age_general.sql
+-rw-r--r--   0        0        0      600 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
+-rw-r--r--   0        0        0      192 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
+-rw-r--r--   0        0        0     4154 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
+-rw-r--r--   0        0        0     1590 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_ed_note.sql
+-rw-r--r--   0        0        0     8576 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr.sql
+-rw-r--r--   0        0        0     1522 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
+-rw-r--r--   0        0        0     2022 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
+-rw-r--r--   0        0        0     2747 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
+-rw-r--r--   0        0        0      736 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_study_period.sql
+-rw-r--r--   0        0        0      732 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_symptom.py
+-rw-r--r--   0        0        0    16067 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_symptom.sql
+-rw-r--r--   0        0        0     1209 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/manifest.toml
+-rw-r--r--   0        0        0      853 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_dx.sql
+-rw-r--r--   0        0        0     1659 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_pcr.sql
+-rw-r--r--   0        0        0     1483 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
+-rw-r--r--   0        0        0     1184 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_study_period.sql
+-rw-r--r--   0        0        0     2255 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_symptom.sql
+-rw-r--r--   0        0        0     2523 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/typesystem.py
+-rw-r--r--   0        0        0     1905 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
+-rw-r--r--   0        0        0     5415 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
+-rw-r--r--   0        0        0     3376 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
+-rw-r--r--   0        0        0     4037 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
+-rw-r--r--   0        0        0     4602 2024-04-04 13:29:42.655185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
+-rw-r--r--   0        0        0     3369 2024-04-04 13:29:42.659185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
+-rw-r--r--   0        0        0     8196 2024-04-04 13:29:42.659185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
+-rw-r--r--   0        0        0       78 2024-04-04 13:29:42.659185 cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/version.sql
+-rw-r--r--   0        0        0      981 2024-04-04 13:29:42.659185 cumulus_library_covid-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 cumulus_library_covid-1.0.0/PKG-INFO
```

### Comparing `cumulus_library_covid-0.2.2/README.md` & `cumulus_library_covid-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 This will add a `covid_symptoms` study target to `cumulus-library`.
 
 ## Publications
 
 The following publications leveraged this module:
 
+__Moving Biosurveillance Beyond Coded Data: AI for Symptom Detection from Physician Notes__
+Andrew McMurry, Amy R Zipursky, Alon Geva, Karen L Olson, James Jones, Vlad Ignatov, Timothy Miller, Kenneth D Mandl
+medRxiv 2023.09.24.23295960; doi: https://doi.org/10.1101/2023.09.24.23295960
+
 __A computable phenotype for patients with SARS-CoV2 testing that occurred outside the hospital__
 Lijing Wang, Amy Zipursky, Alon Geva, Andrew J. McMurry, Kenneth D. Mandl, Timothy A. Miller
 JAMIA Open, 2023;, ooad047,doi: https://doi.org/10.1093/jamiaopen/ooad047 
 
 __The SMART Text2FHIR Pipeline__
 Timothy A. Miller, Andrew J. McMurry, James Jones, Daniel Gottlieb, Kenneth D. Mandl
 medRxiv 2023.03.21.23287499; doi: https://doi.org/10.1101/2023.03.21.23287499 (Preprint)
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/counts.py` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from cumulus_library.schema.counts import CountsBuilder
+from cumulus_library.statistics.counts import CountsBuilder
 
 
 class CovidCountsBuilder(CountsBuilder):
     display_text = "Creating covid counts..."
 
     def count_dx(self, duration="week"):
         """
@@ -94,15 +94,15 @@
             "gender",
             "race_display",
             "enc_class_display",
             "ed_note",
         ]
         return self.count_encounter(view_name, from_table, cols)
 
-    def prepare_queries(self, cursor=None, schema=None):
+    def prepare_queries(self, cursor=None, schema=None, **kwargs):
         self.queries = [
             self.count_dx("month"),
             self.count_dx("week"),
             self.count_pcr("month"),
             self.count_pcr("week"),
             self.count_study_period("month"),
             self.count_study_period("week"),
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_age_general.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_age_general.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_age_pediatric.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_age_pediatric.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_dx_snomed.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_dx_snomed.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_ed_note.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_ed_note.sql`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
             'NOTE:3710480',
             'ED Consultation',
             'http://loinc.org',
             '51846-4',
             'Emergency department Consult note'
         )
     )
-    AS t (from_system, from_code, from_display, system, code, display); --noqa: AL05
+        AS t (from_system, from_code, from_display, system, code, display); --noqa: AL05
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_custom.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_custom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_negative.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_negative.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_pcr_positive.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_pcr_positive.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_study_period.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_study_period.sql`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     t.variant_end
 FROM (
     VALUES
     ('before-delta', date('2020-03-01'), date('2021-06-20')),
     ('delta', date('2021-06-21'), date('2021-12-19')),
     ('omicron', date('2021-12-20'), date('2022-06-01'))
 )
-AS t (variant_era, variant_start, variant_end);
+    AS t (variant_era, variant_start, variant_end);
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_symptom.py` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_symptom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ util for sql view creation"""
+
 import ctakesclient
 
 
 def main():
     """convenice script for writing define sql views"""
     symptoms_list = ctakesclient.filesystem.covid_symptoms()
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/define_symptom.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/define_symptom.sql`

 * *Files 0% similar despite different names*

```diff
@@ -524,8 +524,8 @@
     ),
     ('C0242429', 'T184', '162397003', 'SNOMEDCT_US', 'Throat soreness', 'Sore throat'),
     ('C0242429', 'T184', '162397003', 'SNOMEDCT_US', 'Throat soreness', 'Sore throat'),
     ('C0242429', 'T184', '162397003', 'SNOMEDCT_US', 'Pharyngitis', 'Sore throat'),
     ('C0242429', 'T184', '162397003', 'SNOMEDCT_US', 'dynophagia', 'Sore throat'),
     ('C0242429', 'T184', 'R07.0', 'ICD10CM', 'R07.0', 'Sore throat')
 )
-AS t (cui, tui, code, code_system, text, pref);
+    AS t (cui, tui, code, code_system, text, pref);
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/manifest.toml` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_dx.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_dx.sql`

 * *Files 13% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 )
 
 SELECT DISTINCT
     c.subject_ref,
     c.encounter_ref,
     s.status,
     c.code AS cond_code, -- noqa: LT01,RF02
-    c.recorded_week AS cond_week,
-    c.recorded_month AS cond_month,
-    c.recorded_year AS cond_year,
+    c.recordeddate_week AS cond_week,
+    c.recordeddate_month AS cond_month,
+    c.recordeddate_year AS cond_year,
     s.enc_class_display,
     s.age_at_visit,
     s.ed_note,
     s.variant_era
 FROM core__condition AS c,
     covid_symptom__study_period AS s,
     define_dx
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_pcr.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_pcr.sql`

 * *Files 27% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         from_code AS code,
         display
     FROM covid_symptom__define_pcr_custom
 )
 
 SELECT DISTINCT
     obs_interpret.display AS covid_pcr_result_display,
-    o.lab_code AS covid_pcr_code,
-    o.lab_date AS covid_pcr_date,
-    o.lab_week AS covid_pcr_week,
-    o.lab_month AS covid_pcr_month,
+    o.observation_code AS covid_pcr_code,
+    o.effectivedatetime_day AS covid_pcr_date,
+    o.effectivedatetime_week AS covid_pcr_week,
+    o.effectivedatetime_month AS covid_pcr_month,
     s.status,
     s.variant_era,
     s.author_date,
     s.author_week,
     s.author_month,
     s.ed_note,
     s.start_date,
@@ -47,13 +47,13 @@
     covid_symptom__define_period AS p,
     covid_symptom__study_period AS s,
     covid_symptom__define_pcr AS pcr,
     obs_interpret
 WHERE
     (s.encounter_ref = o.encounter_ref)
     AND (s.variant_era = p.variant_era)
-    AND (o.lab_week BETWEEN p.variant_start AND p.variant_end)
-    AND (o.lab_code.code = pcr.code)
-    AND (o.lab_result.code = obs_interpret.code);
+    AND (o.effectivedatetime_week BETWEEN p.variant_start AND p.variant_end)
+    AND (o.observation_code = pcr.code)
+    AND (o.valuecodeableconcept_code = obs_interpret.code);
 
 -- TODO Cerner specific handling of lab RESULT
 -- https://github.com/smart-on-fhir/cumulus-library-covid/issues/13
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         p.variant_era,
         p.enc_class_display,
         p.subject_ref,
         p.encounter_ref,
         COALESCE(pcr.covid_pcr_result_display, 'None') AS covid_pcr_result,
         COALESCE(dx.cond_code, 'None') AS covid_icd10,
         (dx.cond_code IS NOT NULL OR pcr.covid_pcr_result_display = 'POSITIVE')
-        AS covid_dx,
+            AS covid_dx,
         COALESCE(cn.symptom_display, 'None') AS covid_symptom,
         COALESCE(icd10.icd10_display, 'None') AS symptom_icd10_display
     FROM study_period AS p
     LEFT JOIN covid_symptom__dx AS dx ON p.encounter_ref = dx.encounter_ref
     LEFT JOIN covid_symptom__pcr AS pcr ON p.encounter_ref = pcr.encounter_ref
     LEFT JOIN covid_symptom__symptom_ctakes_negation AS cn
         ON p.encounter_ref = cn.encounter_ref
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_study_period.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_study_period.sql`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 CREATE TABLE covid_symptom__study_period AS
 SELECT DISTINCT
     v.variant_era,
-    s.start_date,
-    s.start_week,
-    s.start_month,
-    s.end_date,
+    s.period_start_day AS start_date,
+    s.period_start_week AS start_week,
+    s.period_start_month AS start_month,
+    s.period_end_day AS end_date,
     s.age_at_visit,
-    s.author_date,
+    s.author_day AS author_date,
     s.author_week,
     s.author_month,
     s.author_year,
     s.gender,
     s.race_display,
     s.subject_ref,
     s.encounter_ref,
-    s.doc_ref,
+    s.documentreference_ref,
     s.diff_enc_note_days,
     s.enc_class_code,
     s.enc_class_display,
     s.doc_type_code,
     s.doc_type_display,
     s.ed_note, -- TODO https://github.com/smart-on-fhir/cumulus-library-covid/issues/10
     a.age_group,
     s.status
 FROM core__study_period AS s,
     covid_symptom__define_period AS v,
     covid_symptom__define_age AS a
 WHERE
     s.age_at_visit = a.age
     AND s.gender IN ('female', 'male')
-    AND s.author_date BETWEEN v.variant_start AND v.variant_end
-    AND s.start_date BETWEEN v.variant_start AND v.variant_end
+    AND s.author_day BETWEEN v.variant_start AND v.variant_end
+    AND s.period_start_day BETWEEN v.variant_start AND v.variant_end
     AND s.diff_enc_note_days BETWEEN -30 AND 30;
 
 CREATE TABLE covid_symptom__meta_date AS
 SELECT
     min(start_date) AS min_date,
     max(end_date) AS max_date
 FROM covid_symptom__study_period;
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/table_symptom.sql` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/table_symptom.sql`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 SELECT DISTINCT
     s.variant_era,
     s.subject_ref,
     s.encounter_ref,
     m.docref_id,
     def.pref AS symptom_display,
-    s.start_date AS start_date,
-    s.end_date AS end_date,
+    s.start_date,
+    s.end_date,
     s.author_week,
     s.author_month,
     s.age_group,
     s.gender,
     s.race_display,
     s.enc_class_display,
     s.ed_note,
@@ -69,16 +69,15 @@
         encounter_ref,
         start_date,
         author_week,
         author_month,
         age_group,
         gender,
         race_display,
-        enc_class_display
-        AS ed_note
+        enc_class_display AS ed_note
     FROM covid_symptom__study_period
 ),
 
 icd10_list AS (
     SELECT DISTINCT
         code AS icd10_code,
         CONCAT('ICD10:', pref) AS icd10_display
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/typesystem.py` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/typesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Utility classes for verifying/generating covid sql definitions"""
+
 from cumulus_library.schema.columns import Coding, Vocab
 from cumulus_library.library.schema.typesystem import Period
 from cumulus_library.library.schema.valueset import (
     ValueSet,
     ObservationInterpretationDetection,
 )
```

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json` & `cumulus_library_covid-1.0.0/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.2.2/pyproject.toml` & `cumulus_library_covid-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "cumulus-library-covid"
 requires-python = ">= 3.9"
-version = "0.2.2"
+version = "1.0.0"
 dependencies = [
-    "cumulus-library >= 1.4.0",
-    "sqlfluff == 2.0.2"
+    "cumulus-library >= 2.0, <3",
+    "sqlfluff >= 3"
 ]
 description = "SQL generation for cumulus covid symptom analysis"
 readme = "README.md"
 license = { text="Apache License 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -24,13 +24,13 @@
 
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project.optional-dependencies]
 dev = [
-    "black",
+    "black >= 24.3, <25",
     "pylint",    
 ]
 
 [tool.flit.sdist]
 include = ["covid_symptom/"]
```

### Comparing `cumulus_library_covid-0.2.2/PKG-INFO` & `cumulus_library_covid-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cumulus-library-covid
-Version: 0.2.2
+Version: 1.0.0
 Summary: SQL generation for cumulus covid symptom analysis
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cumulus-library >= 1.4.0
-Requires-Dist: sqlfluff == 2.0.2
-Requires-Dist: black ; extra == "dev"
+Requires-Dist: cumulus-library >= 2.0, <3
+Requires-Dist: sqlfluff >= 3
+Requires-Dist: black >= 24.3, <25 ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library-covid
 Provides-Extra: dev
 
 # Cumulus Library - Covid
@@ -30,14 +30,18 @@
 
 This will add a `covid_symptoms` study target to `cumulus-library`.
 
 ## Publications
 
 The following publications leveraged this module:
 
+__Moving Biosurveillance Beyond Coded Data: AI for Symptom Detection from Physician Notes__
+Andrew McMurry, Amy R Zipursky, Alon Geva, Karen L Olson, James Jones, Vlad Ignatov, Timothy Miller, Kenneth D Mandl
+medRxiv 2023.09.24.23295960; doi: https://doi.org/10.1101/2023.09.24.23295960
+
 __A computable phenotype for patients with SARS-CoV2 testing that occurred outside the hospital__
 Lijing Wang, Amy Zipursky, Alon Geva, Andrew J. McMurry, Kenneth D. Mandl, Timothy A. Miller
 JAMIA Open, 2023;, ooad047,doi: https://doi.org/10.1093/jamiaopen/ooad047 
 
 __The SMART Text2FHIR Pipeline__
 Timothy A. Miller, Andrew J. McMurry, James Jones, Daniel Gottlieb, Kenneth D. Mandl
 medRxiv 2023.03.21.23287499; doi: https://doi.org/10.1101/2023.03.21.23287499 (Preprint)
```


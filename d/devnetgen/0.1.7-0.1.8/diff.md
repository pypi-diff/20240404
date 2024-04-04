# Comparing `tmp/devnetgen-0.1.7.tar.gz` & `tmp/devnetgen-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devnetgen-0.1.7.tar", max compression
+gzip compressed data, was "devnetgen-0.1.8.tar", max compression
```

## Comparing `devnetgen-0.1.7.tar` & `devnetgen-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2946 2024-03-19 04:06:15.336189 devnetgen-0.1.7/README.md
--rw-r--r--   0        0        0     3078 2024-02-28 08:18:22.032103 devnetgen-0.1.7/devnetgen/.gitignore
--rw-r--r--   0        0        0        0 2024-02-27 11:20:06.339953 devnetgen-0.1.7/devnetgen/__init__.py
--rw-r--r--   0        0        0      208 2024-03-06 08:19:46.002243 devnetgen-0.1.7/devnetgen/config.py
--rw-r--r--   0        0        0    23205 2024-03-06 11:34:01.273157 devnetgen-0.1.7/devnetgen/entities.py
--rw-r--r--   0        0        0    14917 2024-03-06 12:00:29.677437 devnetgen-0.1.7/devnetgen/executors.py
--rw-r--r--   0        0        0      859 2024-03-19 04:02:30.323027 devnetgen-0.1.7/devnetgen/main.py
--rw-r--r--   0        0        0     1901 2024-02-26 09:24:38.375535 devnetgen-0.1.7/devnetgen/pluralize.py
--rw-r--r--   0        0        0     4139 2024-02-29 12:13:35.573413 devnetgen-0.1.7/devnetgen/templates/Controller.cs.j2
--rw-r--r--   0        0        0     1330 2024-03-19 03:56:21.921218 devnetgen-0.1.7/devnetgen/templates/CreateCommand.cs.j2
--rw-r--r--   0        0        0     1472 2024-02-27 10:06:38.150527 devnetgen-0.1.7/devnetgen/templates/DeleteCommand.cs.j2
--rw-r--r--   0        0        0     1273 2024-03-06 10:34:04.383376 devnetgen-0.1.7/devnetgen/templates/DtoTemplate.cs.j2
--rw-r--r--   0        0        0     1327 2024-02-27 10:07:34.796089 devnetgen-0.1.7/devnetgen/templates/GetEntitiesQuery.cs.j2
--rw-r--r--   0        0        0     2429 2024-03-19 04:01:13.062636 devnetgen-0.1.7/devnetgen/templates/GetEntityGridQuery.cs.j2
--rw-r--r--   0        0        0     1602 2024-02-27 10:07:34.792090 devnetgen-0.1.7/devnetgen/templates/GetEntityQuery.cs.j2
--rw-r--r--   0        0        0     3942 2024-02-29 12:10:21.779577 devnetgen-0.1.7/devnetgen/templates/LegacyController.cs.j2
--rw-r--r--   0        0        0     1603 2024-02-27 10:06:38.158527 devnetgen-0.1.7/devnetgen/templates/UpdateCommand.cs.j2
--rw-r--r--   0        0        0     1521 2024-02-27 07:07:11.050803 devnetgen-0.1.7/devnetgen/templates/Validator.cs.j2
--rw-r--r--   0        0        0     1223 2024-03-06 10:37:24.065096 devnetgen-0.1.7/devnetgen/templates/VmTemplate.cs.j2
--rw-r--r--   0        0        0      414 2024-03-19 04:03:35.811362 devnetgen-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 devnetgen-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-03-19 04:06:15.336189 devnetgen-0.1.8/README.md
+-rw-r--r--   0        0        0     3078 2024-02-28 08:18:22.032103 devnetgen-0.1.8/devnetgen/.gitignore
+-rw-r--r--   0        0        0        0 2024-02-27 11:20:06.339953 devnetgen-0.1.8/devnetgen/__init__.py
+-rw-r--r--   0        0        0      208 2024-03-06 08:19:46.002243 devnetgen-0.1.8/devnetgen/config.py
+-rw-r--r--   0        0        0    23282 2024-04-04 08:32:12.537803 devnetgen-0.1.8/devnetgen/entities.py
+-rw-r--r--   0        0        0    14917 2024-03-06 12:00:29.677437 devnetgen-0.1.8/devnetgen/executors.py
+-rw-r--r--   0        0        0      866 2024-04-04 08:33:42.082484 devnetgen-0.1.8/devnetgen/main.py
+-rw-r--r--   0        0        0     1901 2024-02-26 09:24:38.375535 devnetgen-0.1.8/devnetgen/pluralize.py
+-rw-r--r--   0        0        0     4139 2024-02-29 12:13:35.573413 devnetgen-0.1.8/devnetgen/templates/Controller.cs.j2
+-rw-r--r--   0        0        0     1349 2024-04-04 08:36:30.171768 devnetgen-0.1.8/devnetgen/templates/CreateCommand.cs.j2
+-rw-r--r--   0        0        0     1472 2024-02-27 10:06:38.150527 devnetgen-0.1.8/devnetgen/templates/DeleteCommand.cs.j2
+-rw-r--r--   0        0        0     1273 2024-03-06 10:34:04.383376 devnetgen-0.1.8/devnetgen/templates/DtoTemplate.cs.j2
+-rw-r--r--   0        0        0     1327 2024-02-27 10:07:34.796089 devnetgen-0.1.8/devnetgen/templates/GetEntitiesQuery.cs.j2
+-rw-r--r--   0        0        0     2429 2024-03-19 04:01:13.062636 devnetgen-0.1.8/devnetgen/templates/GetEntityGridQuery.cs.j2
+-rw-r--r--   0        0        0     1602 2024-02-27 10:07:34.792090 devnetgen-0.1.8/devnetgen/templates/GetEntityQuery.cs.j2
+-rw-r--r--   0        0        0     3942 2024-02-29 12:10:21.779577 devnetgen-0.1.8/devnetgen/templates/LegacyController.cs.j2
+-rw-r--r--   0        0        0     1603 2024-02-27 10:06:38.158527 devnetgen-0.1.8/devnetgen/templates/UpdateCommand.cs.j2
+-rw-r--r--   0        0        0     1521 2024-02-27 07:07:11.050803 devnetgen-0.1.8/devnetgen/templates/Validator.cs.j2
+-rw-r--r--   0        0        0     1223 2024-03-06 10:37:24.065096 devnetgen-0.1.8/devnetgen/templates/VmTemplate.cs.j2
+-rw-r--r--   0        0        0      414 2024-04-04 08:37:37.648285 devnetgen-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 devnetgen-0.1.8/PKG-INFO
```

### Comparing `devnetgen-0.1.7/README.md` & `devnetgen-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/.gitignore` & `devnetgen-0.1.8/devnetgen/.gitignore`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/entities.py` & `devnetgen-0.1.8/devnetgen/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,17 +377,17 @@
             namespace_obj = self._get_namespace_obj(prev_part)
             self.upper_namespaces.add(namespace_obj)
 
     def _get_class_summary(self):
         """
         Извлечь summary сущности
         """
-        regex = r"/// <summary>\s*/// ((?:.|\n)*?)\s*/// </summary>\s*public class"
+        regex = r"/// <summary>\s*/// (?P<summary>(?:.|\n)*?)\s*/// </summary>\s*(?P<tags>(?:///.+>\s*)+)?(?P<attributes>(?:\[.+]\s*)+)?\s*public class"
         if match := re.search(regex, self.file_text, re.MULTILINE):
-            self.class_summary = match.group(1)
+            self.class_summary = match.group('summary')
 
     def _extract_properties(self, filter_properties: bool = False):
         """
         Извлечь свойства сущности и относящуюся к ним информацию
         """
         class_body_lines = self._get_body_lines()
         class_body_text = ''.join(class_body_lines)
```

### Comparing `devnetgen-0.1.7/devnetgen/executors.py` & `devnetgen-0.1.8/devnetgen/executors.py`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/main.py` & `devnetgen-0.1.8/devnetgen/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,9 +22,9 @@
         entity.add_class_summary()
     else:
         entity = Entity(path)
         executor = SummariesExecutor(entity)
         executor.add_summaries()
 
 
-#if __name__ == "__main__":
-    #add_summaries('/home/alex/Documents/RiderProjects/SystemsRegistryCore/Domain/Entities/InformationSystems/DatasetHystory.cs')
+if __name__ == "__main__":
+    create_crud('/home/alex/Documents/RiderProjects/migrationcompatriots/MigrationCompatriots/Domain/Entities/References/Nationality.cs')
```

### Comparing `devnetgen-0.1.7/devnetgen/pluralize.py` & `devnetgen-0.1.8/devnetgen/pluralize.py`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/Controller.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/Controller.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/CreateCommand.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/CreateCommand.cs.j2`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         _mapper = mapper;
     }
 
     public async {{ return_value }}<long> Handle({{ command_name }} request, CancellationToken cancellationToken)
     {
         var entity = _mapper.Map<{{ file.class_name }}>(request.Dto);
 
-        await _context.{{ file.pluralized_class_name }}.AddAsync(entity);
+        await _context.{{ file.pluralized_class_name }}.AddAsync(entity, cancellationToken);
         await _context.SaveChangesAsync(cancellationToken);
 
         return entity.Id;
     }
 }
```

### Comparing `devnetgen-0.1.7/devnetgen/templates/DeleteCommand.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/DeleteCommand.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/DtoTemplate.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/DtoTemplate.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/GetEntitiesQuery.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/GetEntitiesQuery.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/GetEntityGridQuery.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/GetEntityGridQuery.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/GetEntityQuery.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/GetEntityQuery.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/LegacyController.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/LegacyController.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/UpdateCommand.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/UpdateCommand.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/Validator.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/Validator.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/devnetgen/templates/VmTemplate.cs.j2` & `devnetgen-0.1.8/devnetgen/templates/VmTemplate.cs.j2`

 * *Files identical despite different names*

### Comparing `devnetgen-0.1.7/PKG-INFO` & `devnetgen-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devnetgen
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Александр Окунев
 Author-email: a.okunev@mininform74.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


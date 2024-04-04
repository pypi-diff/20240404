# Comparing `tmp/django_sync_env-0.2.8.tar.gz` & `tmp/django_sync_env-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.2.8.tar", max compression
+gzip compressed data, was "django_sync_env-0.2.9.tar", max compression
```

## Comparing `django_sync_env-0.2.8.tar` & `django_sync_env-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2086 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/README.md
--rw-r--r--   0        0        0      497 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      303 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      194 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     3988 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5237 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7307 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8095 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     2414 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2333 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6561 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5480 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1634 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9332 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14531 2024-01-11 02:19:38.261572 django_sync_env-0.2.8/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_sync_env-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.2.9/README.md
+-rw-r--r--   0        0        0      497 2024-02-07 21:28:28.094401 django_sync_env-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-02-07 21:28:28.095420 django_sync_env-0.2.9/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.2.9/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-02-07 19:58:44.767684 django_sync_env-0.2.9/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.2.9/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.2.9/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.2.9/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.2.9/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.2.9/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.2.9/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     3988 2024-02-07 19:58:44.769120 django_sync_env-0.2.9/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.2.9/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.2.9/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.2.9/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.2.9/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5237 2024-02-07 19:58:44.770356 django_sync_env-0.2.9/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     2467 2024-02-07 21:28:28.097749 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.2.9/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.2.9/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.2.9/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.2.9/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14531 2024-02-07 19:58:44.773054 django_sync_env-0.2.9/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_sync_env-0.2.9/PKG-INFO
```

### Comparing `django_sync_env-0.2.8/README.md` & `django_sync_env-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/checks.py` & `django_sync_env-0.2.9/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/db/base.py` & `django_sync_env-0.2.9/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.2.9/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/db/mysql.py` & `django_sync_env-0.2.9/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.2.9/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.2.9/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,37 +42,39 @@
         self.compress = True  # enforce compression
         self.exclude_tables = None  # not in use yet
         # self.exclude_tables = options.get("exclude_tables")  # wip for later release
 
         database_keys = settings.DATABASES
         storage_config = utils.get_storage_config(settings.ENVIRONMENT, settings.SYNC_ENV_ENVIRONMENTS)
         storage = get_storage(settings.ENVIRONMENT, storage_config)
+        if storage:
+            for database_key in database_keys:
+                self.connector = get_connector(database_key)
+                if self.connector and self.exclude_tables:
+                    self.connector.exclude.extend(
+                        list(self.exclude_tables.replace(" ", "").split(","))
+                    )
+                database = self.connector.settings
 
-        for database_key in database_keys:
-            self.connector = get_connector(database_key)
-            if self.connector and self.exclude_tables:
-                self.connector.exclude.extend(
-                    list(self.exclude_tables.replace(" ", "").split(","))
-                )
-            database = self.connector.settings
+                try:
+                    self._save_new_backup(database, storage)
+                except StorageError as err:
+                    if self.notifications.enabled:
+                        rich_text_blocks, text = self._format_slack_failure_notification(database)
+                        self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
+                    raise CommandError(err) from err
 
-            try:
-                self._save_new_backup(database, storage)
-            except StorageError as err:
+                if not self.quiet:
+                    self.logger.info(f"Successfully backed up database: {database['NAME']}!", )
                 if self.notifications.enabled:
-                    rich_text_blocks, text = self._format_slack_failure_notification(database)
+                    # database backup was successful
+                    rich_text_blocks, text = self._format_slack_success_notification(database)
                     self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
-                raise CommandError(err) from err
-
-            if not self.quiet:
-                self.logger.info(f"Successfully backed up database: {database['NAME']}!", )
-            if self.notifications.enabled:
-                # database backup was successful
-                rich_text_blocks, text = self._format_slack_success_notification(database)
-                self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
+        else:
+            self.logger.error(f'Unable to connect to storage for environment: {settings.ENVIRONMENT}, check config')
 
     def _save_new_backup(self, database, storage):
         """
         Save a new backup file.
         """
         if not self.quiet:
             self.logger.info("Backing Up Database: %s", database["NAME"])
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,25 @@
         self.path = options.get("output_path")
 
         try:
             media_storage = get_storage_class()()
             environment = settings.ENVIRONMENT
             storage_config = utils.get_storage_config(environment, settings.SYNC_ENV_ENVIRONMENTS)
             storage = get_storage(environment, storage_config)
-            self.backup_mediafiles(media_storage, storage)
-            if self.notifications.enabled:
-                rich_text_blocks, text = self._format_slack_success_notification()
-                self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
 
-            if options.get("clean"):
-                self._cleanup_old_backups(environment=environment)
+            if storage:
+                self.backup_mediafiles(media_storage, storage)
+                if self.notifications.enabled:
+                    rich_text_blocks, text = self._format_slack_success_notification()
+                    self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
+
+                if options.get("clean"):
+                    self._cleanup_old_backups(environment=environment)
+            else:
+                self.logger.error(f'Unable to connect to storage for environment: {environment}, check config')
 
         except StorageError as err:
             if self.notifications.enabled:
                 rich_text_blocks, text = self._format_slack_failure_notification()
                 self.notifications.send_slack_message(blocks=rich_text_blocks, text=text)
             raise CommandError(err) from err
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         self.quiet = options.get("quiet")
         self.logger.info("Connecting to configured storage endpoints to get a list of database backups")
         files_attr = []
 
         for env, config in settings.SYNC_ENV_ENVIRONMENTS.items():
             options.update({"content_type": "db"})
             storage = get_storage(env, config)
+            if not storage:
+                continue
             files_attr += self.get_backups_attrs(storage, options, env)
             # Sort the list of file dictionaries using the custom_sort function
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
             title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
                                         content_type="Content Type")
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         self.quiet = options.get("quiet")
         self.logger.info("Connecting to configured storage endpoints to get a list of media backups")
 
         files_attr = []
         for env, config in settings.SYNC_ENV_ENVIRONMENTS.items():
             options.update({"content_type": "media"})
             storage = get_storage(env, config)
+            if not storage:
+                continue
             files_attr += self.get_backups_attrs(storage, options, env)
             # Sort the list of dictionaries using the custom_sort function
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
             title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
                                         content_type="Content Type")
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,18 @@
             if not self.environment:
                 self.logger.error("An environment and database must be specified")
                 exit(1)
 
             environment = self.environment
             storage_config = utils.get_storage_config(environment, sync_env_settings.SYNC_ENV_ENVIRONMENTS)
             storage = get_storage(environment, storage_config)
-
-            self._restore_backup(storage, self.input_database_name, environment)
+            if storage:
+                self._restore_backup(storage, self.input_database_name, environment)
+            else:
+                self.logger.error(f'Unable to connect to storage for environment: {environment}, check config')
 
         except StorageError as err:
             raise CommandError(err) from err
 
     def _get_database(self, database_name: str):
         """Get the database to restore."""
         if not database_name:
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
         self.servername = options.get("servername")
         self.uncompress = options.get("uncompress")
         self.filename = options.get("input_filename")
         self.path = options.get("input_path")
         self.replace = options.get("replace")
         self.passphrase = options.get("passphrase")
         self.interactive = options.get("interactive")
-
-        # self.storage = get_storage()
         self.media_storage = get_storage_class()()
         self.noinput = options.get("noinput")
 
         options['content_type'] = 'media'
 
         if self.noinput:
             self._restore_interactive_backup(options)
@@ -81,15 +79,15 @@
                 return
             self.media_storage.delete(name)
             self.logger.info(f"{name} - deleted")
         self.media_storage.save(name, media_file)
         self.logger.info(f"{name} - uploaded")
 
     def _restore_interactive_backup(self, options):
-        self.logger.info("Please select a database to restore")
+        self.logger.info("Please select media to restore")
         environment_choices = sync_env_settings.SYNC_ENV_ENVIRONMENTS.keys()
 
         environments = [
             inquirer.List(
                 "environment",
                 message="Select a environment to restore from",
                 choices=environment_choices,
@@ -101,14 +99,17 @@
         if not selected_environment:
             self.logger.error("No environment selected, exiting")
             return
 
         environment = selected_environment.get('environment')
         storage_config = utils.get_storage_config(environment, sync_env_settings.SYNC_ENV_ENVIRONMENTS)
         storage = get_storage(environment, storage_config)
+        if not storage:
+            self.logger.error(f'Unable to connect to storage for environment: {environment}, check config')
+            return
 
         media_backups = self.get_backups_attrs(storage, options, environment)
         date_format = "%x %X"  # aka "%m/%d/%y %H:%M:%S"
         media_backups = sorted(
             media_backups,
             key=lambda x: datetime.datetime.strptime(x['datetime'], date_format),
             reverse=True
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/notifications.py` & `django_sync_env-0.2.9/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/settings.py` & `django_sync_env-0.2.9/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/storage.py` & `django_sync_env-0.2.9/src/django_sync_env/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "You must specify an options dictionary to configure storage see sync readme", storage_config
         )
 
     enabled = storage_config.get('enabled', None)
 
     if not enabled:
         logger.error(f"{environment} it is missing configuration or is disabled")
-        exit(1)
+        return
 
     # Get store options
     storage_obj = Storage(storage_config['storage_class'], **storage_config['options'])
     return storage_obj
 
 
 class StorageError(Exception):
```

### Comparing `django_sync_env-0.2.8/src/django_sync_env/tasks.py` & `django_sync_env-0.2.9/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/src/django_sync_env/utils.py` & `django_sync_env-0.2.9/src/django_sync_env/utils.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.8/PKG-INFO` & `django_sync_env-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.2.8
+Version: 0.2.9
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


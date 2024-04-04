# Comparing `tmp/ynab_api_import-0.6.1.tar.gz` & `tmp/ynab_api_import-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_api_import-0.6.1.tar", max compression
+gzip compressed data, was "ynab_api_import-1.0.0.tar", max compression
```

## Comparing `ynab_api_import-0.6.1.tar` & `ynab_api_import-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2024-03-24 06:21:59.149195 ynab_api_import-0.6.1/LICENSE
--rw-r--r--   0        0        0     5658 2024-03-24 06:21:59.149195 ynab_api_import-0.6.1/README.md
--rw-r--r--   0        0        0      832 2024-03-24 06:22:15.025176 ynab_api_import-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/__init__.py
--rw-r--r--   0        0        0     1465 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/accountfetcher.py
--rw-r--r--   0        0        0      340 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/memocleaner.py
--rw-r--r--   0        0        0      757 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/models/config.py
--rw-r--r--   0        0        0      223 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/models/exceptions.py
--rw-r--r--   0        0        0     1466 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/models/transaction.py
--rw-r--r--   0        0        0     2820 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/requisitionhandler.py
--rw-r--r--   0        0        0      904 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/transactionfetcher.py
--rw-r--r--   0        0        0     3495 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/ynabapiimport.py
--rw-r--r--   0        0        0      801 2024-03-24 06:21:59.153195 ynab_api_import-0.6.1/ynabapiimport/ynabclient.py
--rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 ynab_api_import-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6098 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/README.md
+-rw-r--r--   0        0        0      832 2024-04-04 16:33:53.200009 ynab_api_import-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/__init__.py
+-rw-r--r--   0        0        0     1465 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/accountfetcher.py
+-rw-r--r--   0        0        0      340 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/memocleaner.py
+-rw-r--r--   0        0        0      757 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/config.py
+-rw-r--r--   0        0        0      223 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/exceptions.py
+-rw-r--r--   0        0        0     1466 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/transaction.py
+-rw-r--r--   0        0        0     2913 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/requisitionhandler.py
+-rw-r--r--   0        0        0      904 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/transactionfetcher.py
+-rw-r--r--   0        0        0     3548 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/ynabapiimport.py
+-rw-r--r--   0        0        0      801 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/ynabclient.py
+-rw-r--r--   0        0        0     6907 1970-01-01 00:00:00.000000 ynab_api_import-1.0.0/PKG-INFO
```

### Comparing `ynab_api_import-0.6.1/LICENSE` & `ynab_api_import-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/README.md` & `ynab_api_import-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 transaction history provided by the bank. Find and save the institution_id of your bank.
 ```py
 [{'name': '<name>', 'institution_id': '<institution_id>', 'max_history_days': 'ddd'}]
 ```
 
 ### 3. Create Auth Link and authenticate with your bank
 Provide the institution_id. You get back a link which you need to copy to your browser and go through authentication 
-flow with your bank
+flow with your bank. By default, the authorization will allow you to fetch 90 days of your transaction history. You can 
+set the option `use_max_historical_days` to `True` in order to fetch longer transaction history. This is known to cause 
+issues sometimes, so in case you get an 500 error from the Gocardless API try an authorization with default 90 days.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>')
 ```
 
 ### 4. Run import with your reference and YNAB identifiers
 Optionally you can provide a `startdate` argument in form of a `datetime.date` object to only import transactions 
 from a specific date onwards. Equally optionally you can provide a `memo_regex` argument in from of a regex string 
@@ -91,31 +93,32 @@
                                 secret_key='<secret_key>',
                                 reference='<reference>',
                                 token='<ynab_token>',
                                 budget_id='<budget_id>',
                                 account_id='<account_id>')
 ```
 ### Delete current bank authorization
-By default you can create only one bank authorization per reference. If you need to replace the authorization under your 
-current reference you can explicitly do that by calling the following function.
+By default you can create only one bank authorization per reference. If you need to replace the authorization under 
+your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
+link.
 ```py
-ynab_api_import.delete_currrent_auth()
+ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
 ### Show Logs
 The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs 
 import the logging module and set it to the level `INFO`. You can also access the logger for advanced configuration 
 via the `logger` attribute of your `YnabApiImport`instance.
 ```py
 import logging
 
 logging.basicConfig(level='INFO')
 ```
 ### Testing your `memo_regex`
 You can test your `memo_regex` with a call to `test_memo_regex()`. The function will fetch transactions from your 
-bank account, apply the regex and output the old and new memo strings in a dict for inspection
+bank account, apply the regex and output the old and new memo strings in a dictionary for inspection.
 ```py
 ynab_api_import.test_memo_regex(memo_regex=r'<memo_regex')
 ```
 returns a list of `dict` with following content
 ```
 [{original_memo: cleaned_memo}]
 ```
```

### Comparing `ynab_api_import-0.6.1/pyproject.toml` & `ynab_api_import-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-api-import"
-version = "0.6.1"
+version = "1.0.0"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to import bank transactions via API into You Need A Budget (YNAB)"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabapiimport'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_api_import-0.6.1/ynabapiimport/accountfetcher.py` & `ynab_api_import-1.0.0/ynabapiimport/accountfetcher.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/ynabapiimport/models/config.py` & `ynab_api_import-1.0.0/ynabapiimport/models/config.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/ynabapiimport/models/transaction.py` & `ynab_api_import-1.0.0/ynabapiimport/models/transaction.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/ynabapiimport/requisitionhandler.py` & `ynab_api_import-1.0.0/ynabapiimport/requisitionhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,26 @@
 			except StopIteration:
 				try:
 					r = next(r for r in reqs if r['status'] == 'EX')
 					raise NoRequisitionError("Requisition expired")
 				except StopIteration:
 					raise NoRequisitionError(f"Requisition not valid. Current status: {[r['status'] for r in reqs]}'")
 
-	def create_requisition_auth_link(self, institution_id: str) -> str:
+	def create_requisition_auth_link(self, institution_id: str, use_max_historical_days: bool) -> str:
 		req_list = self._client.requisition.get_requisitions()['results']
 
 		self.delete_inactive_requisitions(req_list=req_list)
 		self.reference_is_unique(req_list=req_list)
 		self.reference_is_valid()
 
 		# get max days for institution
-		institution_dict = self._client.institution.get_institution_by_id(institution_id)
-		transaction_total_days = institution_dict['transaction_total_days']
+		transaction_total_days = 90
+		if use_max_historical_days:
+			institution_dict = self._client.institution.get_institution_by_id(institution_id)
+			transaction_total_days = institution_dict['transaction_total_days']
 
 		init_session = self._client.initialize_session(institution_id=institution_id,
 													   redirect_uri='http://localhost:',
 													   reference_id=f"{self._reference}::{uuid4()}",
 													   max_historical_days=transaction_total_days)
 		return init_session.link
```

### Comparing `ynab_api_import-0.6.1/ynabapiimport/transactionfetcher.py` & `ynab_api_import-1.0.0/ynabapiimport/transactionfetcher.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/ynabapiimport/ynabapiimport.py` & `ynab_api_import-1.0.0/ynabapiimport/ynabapiimport.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 			mc = MemoCleaner(memo_regex=memo_regex)
 			transactions = [mc.clean(t) for t in transactions]
 
 		i = self._ynab_client.insert(transactions)
 		self.logger.info(f"inserted {i} transactions for {self._reference}")
 		return i
 
-	def create_auth_link(self, institution_id: str) -> str:
+	def create_auth_link(self, institution_id: str, use_max_historical_days: bool = False,
+						 delete_current_auth: bool = False) -> str:
 		rh = RequisitionHandler(client=self._gocardless_client, reference=self._reference)
-		auth_link = rh.create_requisition_auth_link(institution_id=institution_id)
+		if delete_current_auth:
+			rh.delete_current_requisition()
+			self.logger.info(f'deleted auth for reference {self._reference}')
+		auth_link = rh.create_requisition_auth_link(institution_id=institution_id,
+													use_max_historical_days=use_max_historical_days)
 		self.logger.info(f'created auth link for {institution_id} under reference {self._reference}')
 		return auth_link
 
-	def delete_current_auth(self):
-		rh = RequisitionHandler(client=self._gocardless_client, reference=self._reference)
-		rh.delete_current_requisition()
-		self.logger.info(f'deleted auth for reference {self._reference}')
-
 	def fetch_institutions(self, countrycode: str) -> List[dict]:
 		rh = RequisitionHandler(client=self._gocardless_client, reference=self._reference)
 		institutions = rh.get_institutions(countrycode=countrycode)
 		self.logger.info(f'fetched list with {len(institutions)} institutions for countrycode {countrycode}')
 		return institutions
 
 	def test_memo_regex(self, memo_regex: str) -> List[dict]:
```

### Comparing `ynab_api_import-0.6.1/ynabapiimport/ynabclient.py` & `ynab_api_import-1.0.0/ynabapiimport/ynabclient.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-0.6.1/PKG-INFO` & `ynab_api_import-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-api-import
-Version: 0.6.1
+Version: 1.0.0
 Summary: Library to import bank transactions via API into You Need A Budget (YNAB)
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -84,15 +84,17 @@
 transaction history provided by the bank. Find and save the institution_id of your bank.
 ```py
 [{'name': '<name>', 'institution_id': '<institution_id>', 'max_history_days': 'ddd'}]
 ```
 
 ### 3. Create Auth Link and authenticate with your bank
 Provide the institution_id. You get back a link which you need to copy to your browser and go through authentication 
-flow with your bank
+flow with your bank. By default, the authorization will allow you to fetch 90 days of your transaction history. You can 
+set the option `use_max_historical_days` to `True` in order to fetch longer transaction history. This is known to cause 
+issues sometimes, so in case you get an 500 error from the Gocardless API try an authorization with default 90 days.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>')
 ```
 
 ### 4. Run import with your reference and YNAB identifiers
 Optionally you can provide a `startdate` argument in form of a `datetime.date` object to only import transactions 
 from a specific date onwards. Equally optionally you can provide a `memo_regex` argument in from of a regex string 
@@ -113,31 +115,32 @@
                                 secret_key='<secret_key>',
                                 reference='<reference>',
                                 token='<ynab_token>',
                                 budget_id='<budget_id>',
                                 account_id='<account_id>')
 ```
 ### Delete current bank authorization
-By default you can create only one bank authorization per reference. If you need to replace the authorization under your 
-current reference you can explicitly do that by calling the following function.
+By default you can create only one bank authorization per reference. If you need to replace the authorization under 
+your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
+link.
 ```py
-ynab_api_import.delete_currrent_auth()
+ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
 ### Show Logs
 The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs 
 import the logging module and set it to the level `INFO`. You can also access the logger for advanced configuration 
 via the `logger` attribute of your `YnabApiImport`instance.
 ```py
 import logging
 
 logging.basicConfig(level='INFO')
 ```
 ### Testing your `memo_regex`
 You can test your `memo_regex` with a call to `test_memo_regex()`. The function will fetch transactions from your 
-bank account, apply the regex and output the old and new memo strings in a dict for inspection
+bank account, apply the regex and output the old and new memo strings in a dictionary for inspection.
 ```py
 ynab_api_import.test_memo_regex(memo_regex=r'<memo_regex')
 ```
 returns a list of `dict` with following content
 ```
 [{original_memo: cleaned_memo}]
 ```
```


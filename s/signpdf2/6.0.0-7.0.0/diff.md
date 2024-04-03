# Comparing `tmp/signpdf2-6.0.0.tar.gz` & `tmp/signpdf2-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signpdf2-6.0.0.tar", last modified: Thu Sep  9 06:14:39 2021, max compression
+gzip compressed data, was "signpdf2-7.0.0.tar", last modified: Wed Apr  3 23:17:29 2024, max compression
```

## Comparing `signpdf2-6.0.0.tar` & `signpdf2-7.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2021-09-09 06:14:39.940171 signpdf2-6.0.0/
--rw-r--r--   0 aseem     (1000) aseem     (1000)     1081 2021-09-07 03:24:36.000000 signpdf2-6.0.0/LICENSE
--rw-rw-r--   0 aseem     (1000) aseem     (1000)     2791 2021-09-09 06:14:39.940171 signpdf2-6.0.0/PKG-INFO
--rw-r--r--   0 aseem     (1000) aseem     (1000)     1863 2021-09-08 04:40:43.000000 signpdf2-6.0.0/README.md
--rw-rw-r--   0 aseem     (1000) aseem     (1000)       38 2021-09-09 06:14:39.940171 signpdf2-6.0.0/setup.cfg
--rw-r--r--   0 aseem     (1000) aseem     (1000)      868 2021-09-09 06:14:39.000000 signpdf2-6.0.0/setup.py
-drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2021-09-09 06:14:39.940171 signpdf2-6.0.0/signpdf2/
--rw-rw-r--   0 aseem     (1000) aseem     (1000)        7 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2/__init__.py
--rw-r--r--   0 aseem     (1000) aseem     (1000)      320 2021-09-07 03:24:36.000000 signpdf2-6.0.0/signpdf2/create_tmp_file.py
--rw-r--r--   0 aseem     (1000) aseem     (1000)      666 2021-09-07 03:24:36.000000 signpdf2-6.0.0/signpdf2/example.py
--rw-r--r--   0 aseem     (1000) aseem     (1000)     1398 2021-09-09 06:13:44.000000 signpdf2-6.0.0/signpdf2/file_utilities.py
--rw-r--r--   0 aseem     (1000) aseem     (1000)      763 2021-09-07 03:24:36.000000 signpdf2-6.0.0/signpdf2/pdf_utilites.py
--rw-r--r--   0 aseem     (1000) aseem     (1000)     4391 2021-09-09 06:04:55.000000 signpdf2-6.0.0/signpdf2/sign_pdf.py
-drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2021-09-09 06:14:39.940171 signpdf2-6.0.0/signpdf2.egg-info/
--rw-rw-r--   0 aseem     (1000) aseem     (1000)     2791 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2.egg-info/PKG-INFO
--rw-rw-r--   0 aseem     (1000) aseem     (1000)      336 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2.egg-info/SOURCES.txt
--rw-rw-r--   0 aseem     (1000) aseem     (1000)        1 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2.egg-info/dependency_links.txt
--rw-rw-r--   0 aseem     (1000) aseem     (1000)       34 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2.egg-info/requires.txt
--rw-rw-r--   0 aseem     (1000) aseem     (1000)        9 2021-09-09 06:14:39.000000 signpdf2-6.0.0/signpdf2.egg-info/top_level.txt
+drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2024-04-03 23:17:29.140431 signpdf2-7.0.0/
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     1081 2021-09-07 03:24:36.000000 signpdf2-7.0.0/LICENSE
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     4009 2024-04-03 23:17:29.140431 signpdf2-7.0.0/PKG-INFO
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     3457 2024-04-03 23:08:53.000000 signpdf2-7.0.0/README.md
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)       38 2024-04-03 23:17:29.140431 signpdf2-7.0.0/setup.cfg
+-rw-r--r--   0 aseem     (1000) aseem     (1000)      874 2024-04-03 23:00:20.000000 signpdf2-7.0.0/setup.py
+drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2024-04-03 23:17:29.140431 signpdf2-7.0.0/signpdf2/
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)        7 2021-09-09 06:14:39.000000 signpdf2-7.0.0/signpdf2/__init__.py
+-rw-r--r--   0 aseem     (1000) aseem     (1000)      320 2021-09-07 03:24:36.000000 signpdf2-7.0.0/signpdf2/create_tmp_file.py
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     2040 2024-04-03 23:00:56.000000 signpdf2-7.0.0/signpdf2/example.py
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     1436 2024-04-03 19:31:02.000000 signpdf2-7.0.0/signpdf2/file_utilities.py
+-rw-r--r--   0 aseem     (1000) aseem     (1000)      801 2024-04-03 19:30:31.000000 signpdf2-7.0.0/signpdf2/pdf_utilites.py
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     5402 2024-04-03 23:07:34.000000 signpdf2-7.0.0/signpdf2/sign_pdf.py
+drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2024-04-03 23:17:29.140431 signpdf2-7.0.0/signpdf2.egg-info/
+-rw-r--r--   0 aseem     (1000) aseem     (1000)     4009 2024-04-03 23:17:29.000000 signpdf2-7.0.0/signpdf2.egg-info/PKG-INFO
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)      359 2024-04-03 23:17:29.000000 signpdf2-7.0.0/signpdf2.egg-info/SOURCES.txt
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)        1 2024-04-03 23:17:29.000000 signpdf2-7.0.0/signpdf2.egg-info/dependency_links.txt
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)       38 2024-04-03 23:17:29.000000 signpdf2-7.0.0/signpdf2.egg-info/requires.txt
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)        9 2024-04-03 23:17:29.000000 signpdf2-7.0.0/signpdf2.egg-info/top_level.txt
+drwxrwxr-x   0 aseem     (1000) aseem     (1000)        0 2024-04-03 23:17:29.140431 signpdf2-7.0.0/tests/
+-rw-rw-r--   0 aseem     (1000) aseem     (1000)     1095 2024-04-03 19:31:42.000000 signpdf2-7.0.0/tests/test_sign_pdf.py
```

### Comparing `signpdf2-6.0.0/LICENSE` & `signpdf2-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signpdf2-6.0.0/setup.py` & `signpdf2-7.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="signpdf2",
-    version="6.0.0",
-    description="Read the latest Real Python tutorials",
+    version="7.0.0",
+    description="Sign PDFs using a signature image",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/aseem-hegshetye/signpdf",
     author="Aseem Hegshetye",
     author_email="aseem.hegshetye@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     packages=["signpdf2"],
     include_package_data=True,
-    install_requires=["PyPDF2", "requests", "urllib3", "reportlab"],
+    install_requires=["pypdf", "requests", "urllib3", "reportlab", "pytz"],
 
 )
```

### Comparing `signpdf2-6.0.0/signpdf2/file_utilities.py` & `signpdf2-7.0.0/signpdf2/file_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
             response = requests.get(url)
             file.write(response.content)
 
         return temp_file
 
 
 class WritePdfToDisk:
+    def __init__(self):
+        pass
+
     def write_pdf_to_disk(self, pdf_writer, pdf_name):
         """
         :param pdf_writer: PdfFileWriter object
         :param pdf_name: pdf file name along with entire path
         :return: write pdf to pdf_name
         """
         with open(pdf_name, 'wb') as file:
```

### Comparing `signpdf2-6.0.0/signpdf2/pdf_utilites.py` & `signpdf2-7.0.0/signpdf2/pdf_utilites.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from pdfminer.pdfdocument import PDFDocument
 from pdfminer.pdfinterp import resolve1
 from pdfminer.pdfparser import PDFParser
 
 
 class PdfUtilities:
 
+    def __init__(self):
+        pass
+
     def get_total_number_of_pages(self, pdf_file_name):
         with open(pdf_file_name, 'rb') as file:
             parser = PDFParser(file)
             document = PDFDocument(parser)
             total_pages = resolve1(document.catalog['Pages'])['Count']
 
         return total_pages
```

### Comparing `signpdf2-6.0.0/signpdf2/sign_pdf.py` & `signpdf2-7.0.0/signpdf2/sign_pdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,135 @@
 import datetime
 
-import PyPDF2
+import pypdf
+import pytz
 from reportlab.pdfgen import canvas
 
 from signpdf2.create_tmp_file import CreateTmpFileMixin
 
 
 class SignPdf(CreateTmpFileMixin):
     """
     Sign a pdf with signature image at desired location.
+    A signature image is placed(overlayed) at desired location on a pdf page.
     we use units instead of pixel. Units are pdf-standard units (1/72 inch)
     """
 
-    def __init__(self, sign_w: int, sign_h: int,
-                 page_num: int, offset_x: int, offset_y: int,
-                 pdf_file: str, signature_file: str):
+    def __init__(
+            self,
+            sign_w: int,
+            sign_h: int,
+            page_num: int,
+            offset_x: int,
+            offset_y: int,
+            pdf_file: str,
+            signature_file: str,
+            signature_expand: bool = False,
+            signature_over: bool = True,
+            sign_timestamp: bool = True,
+            timezone: str = 'UTC'
+    ):
         """
         :param sign_w: signature width in units
         :param sign_h: signature height in units
         :param pdf_file:  name and path of pdf file on local system
         :param signature_file: name and path of signature image file
         :param page_num: page number of pdf to sign. Index starts at 0
         :param offset_x: offset units horizontally from left
         :param offset_y: offset units vertically from bottom
+        :param signature_expand: Original page dimension is expanded to
+            accomodate signature if signature dimensions are more than original
+        :param signature_over: Signature is over or under the original pdf
+        :param sign_timestamp: Bool. If true, then add current timestamp below
+            signature
         """
         self.sign_w = sign_w
         self.sign_h = sign_h
         self.page_num = page_num
         self.offset_x = offset_x
         self.offset_y = offset_y
         self.pdf_file = pdf_file
         self.signature_file = signature_file
+        self.signature_expand = signature_expand
+        self.signature_over = signature_over
+        self.sign_timestamp = sign_timestamp
+        self.timezone = timezone
 
-    def sign_pdf(self, sign_date: bool = True):
+    def sign_pdf(self):
         """
         Draw signature on a temporary empty single page pdf.
         Then merge this page with original pdf page. If signature is needed
         on 2nd page, then merge this temp signed page on page2.
 
-        :param sign_date: Bool. If true, then add current timestamp below
+        :param sign_timestamp: Bool. If true, then add current timestamp below
             signature
         :return: PdfFileWriter object with signed pdf
         """
-        writer = PyPDF2.PdfFileWriter()
-        pdf_reader = self.get_pdf_file_reader()
+        writer = pypdf.PdfWriter()
+        pdf_reader = pypdf.PdfReader(self.pdf_file)
 
-        for i in range(0, pdf_reader.getNumPages()):
-            orignal_pdf_page = pdf_reader.getPage(i)
+        for i in range(0, len(pdf_reader.pages)):
+            orignal_pdf_page = pdf_reader.pages[i]
 
             if i == self.page_num:
                 temp_signature_pdf = self.create_tmp_file()
 
                 self.draw_signature_on_pdf(
                     temp_signature_pdf,
-                    page_size=orignal_pdf_page.cropBox,
-                    sign_date=sign_date
+                    page_size=orignal_pdf_page.cropbox,
+                    sign_date=self.sign_timestamp
                 )
 
                 # Merge signed temp PDF in to original page
                 signed_pdf_reader = self.get_pdf_file_reader(temp_signature_pdf)
-                signed_page = signed_pdf_reader.getPage(0)
+                signed_page = signed_pdf_reader.pages[0]
                 orignal_pdf_page = self.merge_two_pdf_pages(orignal_pdf_page,
                                                             signed_page)
 
-            writer.addPage(orignal_pdf_page)
+            writer.add_page(orignal_pdf_page)  # addPage
 
         return writer
 
     def get_pdf_file_reader(self, file: str = None):
         """
         :param file: pdf file name with path
         :return: file reader object , keeping file open in read mode. if we
         close the file, then that pdf_reader is of no use
         """
         if file is None:
             file = self.pdf_file
 
-        pdf_file = open(file, 'rb')
-        return PyPDF2.PdfFileReader(pdf_file)
+        return pypdf.PdfReader(file)
 
     def merge_two_pdf_pages(
             self,
-            page1: PyPDF2.pdf.PageObject,
-            page2: PyPDF2.pdf.PageObject
-    ) -> PyPDF2.pdf.PageObject:
+            page1: pypdf.PageObject,
+            page2: pypdf.PageObject
+    ) -> pypdf.PageObject:  # PyPDF2.pdf.PageObject:
         """
         Merge page2 in page1
-        :param page1: pdf page - PyPDF2.pdf.PageObject
+        :param page1: pdf page
         :param page2: pdf page
         :return: page1 after page2 is merged in it
         """
-        page2.mediaBox = page1.mediaBox
-        page1.mergePage(page2)
+        page2.mediabox = page1.mediabox
+        page1.merge_page(
+            page2,
+            over=self.signature_over,
+            expand=self.signature_expand
+        )
         return page1
 
     def get_current_timestamp_str(self):
-        return datetime.datetime.now().strftime(
-            "%m-%d-%Y - %H:%M"
+        """
+        :return: current timestamp in string format and timezone
+        """
+        timezone = pytz.timezone(self.timezone)
+        return datetime.datetime.now(timezone).strftime(
+            "%m-%d-%Y - %I:%M %p - %Z"
         )
 
     def draw_signature_on_pdf(
             self,
             pdf_file_name,
             page_size,
             sign_date
```


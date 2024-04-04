# Comparing `tmp/ocx-3.0.0rc5.tar.gz` & `tmp/ocx-3.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocx-3.0.0rc5.tar", max compression
+gzip compressed data, was "ocx-3.0.0rc6.tar", max compression
```

## Comparing `ocx-3.0.0rc5.tar` & `ocx-3.0.0rc6.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     2305 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/DATABINDING.md
--rw-r--r--   0        0        0    11359 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/LICENSE
--rw-r--r--   0        0        0   252470 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/ocx/OCX_Schema.xsd
--rw-r--r--   0        0        0       25 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/ocx/__init__.py
--rw-r--r--   0        0        0    10427 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/ocx/ocx_286/__init__.py
--rw-r--r--   0        0        0   347292 2024-03-22 12:29:32.751647 ocx-3.0.0rc5/ocx/ocx_286/ocx_286.py
--rw-r--r--   0        0        0    10426 2024-03-22 12:29:32.755647 ocx-3.0.0rc5/ocx/ocx_286_fix/__init__.py
--rw-r--r--   0        0        0   370511 2024-03-22 12:29:32.755647 ocx-3.0.0rc5/ocx/ocx_286_fix/ocx_286_fix.py
--rw-r--r--   0        0        0    10269 2024-03-22 12:29:32.755647 ocx-3.0.0rc5/ocx/ocx_300b0/__init__.py
--rw-r--r--   0        0        0   359814 2024-03-22 12:29:32.755647 ocx-3.0.0rc5/ocx/ocx_300b0/ocx_300b0.py
--rw-r--r--   0        0        0    10269 2024-03-22 12:29:32.755647 ocx-3.0.0rc5/ocx/ocx_300b3/__init__.py
--rw-r--r--   0        0        0   360029 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b3/ocx_300b3.py
--rw-r--r--   0        0        0    10269 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b4/__init__.py
--rw-r--r--   0        0        0   360028 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b4/ocx_300b4.py
--rw-r--r--   0        0        0    10269 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b5/__init__.py
--rw-r--r--   0        0        0   359068 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b5/ocx_300b5.py
--rw-r--r--   0        0        0    10017 2024-03-22 12:29:32.759647 ocx-3.0.0rc5/ocx/ocx_300b6/__init__.py
--rw-r--r--   0        0        0   368690 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300b6/ocx_300b6.py
--rw-r--r--   0        0        0    10200 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300b7/__init__.py
--rw-r--r--   0        0        0   364833 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300b7/ocx_300b7.py
--rw-r--r--   0        0        0    10278 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300rc1/__init__.py
--rw-r--r--   0        0        0   359787 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300rc1/ocx_300rc1.py
--rw-r--r--   0        0        0    10297 2024-03-22 12:29:32.763647 ocx-3.0.0rc5/ocx/ocx_300rc2/__init__.py
--rw-r--r--   0        0        0   359310 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc2/ocx_300rc2.py
--rw-r--r--   0        0        0    10315 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc3/__init__.py
--rw-r--r--   0        0        0   360787 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc3/ocx_300rc3.py
--rw-r--r--   0        0        0    10315 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc4/__init__.py
--rw-r--r--   0        0        0   360787 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc4/ocx_300rc4.py
--rw-r--r--   0        0        0    10219 2024-03-22 12:29:32.767647 ocx-3.0.0rc5/ocx/ocx_300rc5/__init__.py
--rw-r--r--   0        0        0   362169 2024-03-22 12:29:32.771647 ocx-3.0.0rc5/ocx/ocx_300rc5/ocx_300rc5.py
--rw-r--r--   0        0        0     2438 2024-03-22 12:29:32.771647 ocx-3.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 ocx-3.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     2305 2024-04-04 12:30:50.924782 ocx-3.0.0rc6/DATABINDING.md
+-rw-r--r--   0        0        0    11359 2024-04-04 12:30:50.924782 ocx-3.0.0rc6/LICENSE
+-rw-r--r--   0        0        0   253964 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/OCX_Schema.xsd
+-rw-r--r--   0        0        0       25 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/__init__.py
+-rw-r--r--   0        0        0    10427 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/ocx_286/__init__.py
+-rw-r--r--   0        0        0   347292 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/ocx_286/ocx_286.py
+-rw-r--r--   0        0        0    10426 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/ocx_286_fix/__init__.py
+-rw-r--r--   0        0        0   370511 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/ocx_286_fix/ocx_286_fix.py
+-rw-r--r--   0        0        0    10269 2024-04-04 12:30:50.928783 ocx-3.0.0rc6/ocx/ocx_300b0/__init__.py
+-rw-r--r--   0        0        0   359814 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b0/ocx_300b0.py
+-rw-r--r--   0        0        0    10269 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b3/__init__.py
+-rw-r--r--   0        0        0   360029 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b3/ocx_300b3.py
+-rw-r--r--   0        0        0    10269 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b4/__init__.py
+-rw-r--r--   0        0        0   360028 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b4/ocx_300b4.py
+-rw-r--r--   0        0        0    10269 2024-04-04 12:30:50.932783 ocx-3.0.0rc6/ocx/ocx_300b5/__init__.py
+-rw-r--r--   0        0        0   359068 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300b5/ocx_300b5.py
+-rw-r--r--   0        0        0    10017 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300b6/__init__.py
+-rw-r--r--   0        0        0   368690 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300b6/ocx_300b6.py
+-rw-r--r--   0        0        0    10200 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300b7/__init__.py
+-rw-r--r--   0        0        0   364833 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300b7/ocx_300b7.py
+-rw-r--r--   0        0        0    10278 2024-04-04 12:30:50.936782 ocx-3.0.0rc6/ocx/ocx_300rc1/__init__.py
+-rw-r--r--   0        0        0   359787 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc1/ocx_300rc1.py
+-rw-r--r--   0        0        0    10297 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc2/__init__.py
+-rw-r--r--   0        0        0   359310 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc2/ocx_300rc2.py
+-rw-r--r--   0        0        0    10315 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc3/__init__.py
+-rw-r--r--   0        0        0   360787 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc3/ocx_300rc3.py
+-rw-r--r--   0        0        0    10315 2024-04-04 12:30:50.940782 ocx-3.0.0rc6/ocx/ocx_300rc4/__init__.py
+-rw-r--r--   0        0        0   360787 2024-04-04 12:30:50.944782 ocx-3.0.0rc6/ocx/ocx_300rc4/ocx_300rc4.py
+-rw-r--r--   0        0        0    10219 2024-04-04 12:30:50.944782 ocx-3.0.0rc6/ocx/ocx_300rc5/__init__.py
+-rw-r--r--   0        0        0   362169 2024-04-04 12:30:50.944782 ocx-3.0.0rc6/ocx/ocx_300rc5/ocx_300rc5.py
+-rw-r--r--   0        0        0    10219 2024-04-04 12:30:50.944782 ocx-3.0.0rc6/ocx/ocx_300rc6/__init__.py
+-rw-r--r--   0        0        0   364284 2024-04-04 12:30:50.944782 ocx-3.0.0rc6/ocx/ocx_300rc6/ocx_300rc6.py
+-rw-r--r--   0        0        0     2438 2024-04-04 12:30:50.948782 ocx-3.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 ocx-3.0.0rc6/PKG-INFO
```

### Comparing `ocx-3.0.0rc5/DATABINDING.md` & `ocx-3.0.0rc6/DATABINDING.md`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/LICENSE` & `ocx-3.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/OCX_Schema.xsd` & `ocx-3.0.0rc6/ocx/OCX_Schema.xsd`

 * *Files 0% similar despite different names*

#### Comparing `ocx-3.0.0rc5/ocx/OCX_Schema.xsd` & `ocx-3.0.0rc6/ocx/OCX_Schema.xsd`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- edited with XMLSpy v2024 (x64) (http://www.altova.com) by Astrup, Ole Christian (DNV AS) -->
 <!-- Copyright 2024 Open Class 3D Exchange (OCX) Consortium (https://3docx.org)			Licensed under the Apache License, Version 2.0 (the "License"); 			You may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0			Unless required by applicable law or agreed to in writing, the 3Docx standard and software distributed under the License is distributed on an 			"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either expressed or implied.			The OCX Consortium is not liable to any use whatsoever of the distributed standard or software based on the standard.			See the License for the specific language governing permissions and limitations under the License.  -->
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:vc="http://www.w3.org/2007/XMLSchema-versioning" xmlns:ocx="https://3docx.org/fileadmin//ocx_schema//V300rc5//OCX_Schema.xsd" xmlns:unitsml="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" targetNamespace="https://3docx.org/fileadmin//ocx_schema//V300rc5//OCX_Schema.xsd" elementFormDefault="qualified" attributeFormDefault="unqualified" vc:minVersion="1.0">
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:vc="http://www.w3.org/2007/XMLSchema-versioning" xmlns:ocx="https://3docx.org/fileadmin//ocx_schema//V300rc6//OCX_Schema.xsd" xmlns:unitsml="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" targetNamespace="https://3docx.org/fileadmin//ocx_schema//V300rc6//OCX_Schema.xsd" elementFormDefault="qualified" attributeFormDefault="unqualified" vc:minVersion="1.0">
   <!-- Import the NIST unitsML lite schema -->
   <xs:import namespace="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" schemaLocation="https://3docx.org/fileadmin/ocx_schema/unitsml/unitsmlSchema_lite-0.9.18.xsd"/>
   <xs:annotation>
     <xs:documentation>Copyright 2024 Open Class 3D Exchange (OCX) Consortium (https://3docx.org). Licensed under the Apache License, Version 2.0 (the &quot;License&quot;); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0. Unless required by applicable law or agreed to in writing, the 3Docx standard and software distributed under the License is distributed on an &quot;AS IS&quot; BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either expressed or implied.	The OCX Consortium is not liable to any use whatsoever of the distributed standard or software based on the standard. See the License for the specific language governing permissions and limitations under the License.</xs:documentation>
   </xs:annotation>
   <xs:element name="Header" type="ocx:Header_T">
     <xs:annotation>
@@ -66,15 +66,15 @@
   <xs:complexType name="DocumentBase_T" abstract="true">
     <xs:annotation>
       <xs:documentation>Type definition of the abstract base class for the XML document defined in this schema.</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element ref="ocx:Header"/>
     </xs:sequence>
-    <xs:attribute name="schemaVersion" type="xs:string" use="required" fixed="3.0.0rc5">
+    <xs:attribute name="schemaVersion" type="xs:string" use="required" fixed="3.0.0rc6">
       <xs:annotation>
         <xs:documentation>Current XML schema version (Format - x.y.z) x : Incremented for backward incompatible changes ( Ex - Adding a required attribute, etc.) y : Major backward compatible changes [ Ex - Adding a new node ,fixing major CRs,etc..] z : Minor backward compatible changes (Ex - adding an optional attribute, etc).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="language" type="xs:language" use="optional" default="en">
       <xs:annotation>
         <xs:documentation>Language used by the application.</xs:documentation>
@@ -865,25 +865,36 @@
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:complexType name="OccurrenceGroup_T">
     <xs:annotation>
       <xs:documentation>Type definition</xs:documentation>
     </xs:annotation>
-    <xs:complexContent>
-      <xs:extension base="ocx:DescriptionBase_T">
-        <xs:choice>
-          <xs:annotation>
-            <xs:documentation>Any numbers of Occurrence or OccurrenceGroup can be present. At least one instance must exist.</xs:documentation>
-          </xs:annotation>
-          <xs:element ref="ocx:Occurrence" maxOccurs="unbounded"/>
-          <xs:element ref="ocx:OccurrenceGroup" maxOccurs="unbounded"/>
-        </xs:choice>
-      </xs:extension>
-    </xs:complexContent>
+    <xs:choice>
+      <xs:annotation>
+        <xs:documentation>Any numbers of Occurrence or OccurrenceGroup can be present. At least one instance must exist.</xs:documentation>
+      </xs:annotation>
+      <xs:element ref="ocx:Occurrence" maxOccurs="unbounded"/>
+      <xs:element ref="ocx:OccurrenceGroup" maxOccurs="unbounded"/>
+    </xs:choice>
+    <xs:attribute name="id" type="xs:ID" use="required">
+      <xs:annotation>
+        <xs:documentation>An identifier for an element unique within the scope of the XML file. Each id must be unique within a document. The attribute uses the standard XML 1.0 ID type as defined in the XML Schema specification. This attribute is required in many OCX XML elements and an application should generate them automatically.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
+    <xs:attribute name="name" type="xs:string" use="required">
+      <xs:annotation>
+        <xs:documentation>The name of the node.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
+    <xs:attribute name="type">
+      <xs:annotation>
+        <xs:documentation>The occurrence group design/product view type</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
   </xs:complexType>
   <xs:element name="DesignView">
     <xs:annotation>
       <xs:documentation>A manifestation of some or all the components in the exporting application that contains configuration information for the parts it includes.</xs:documentation>
     </xs:annotation>
     <xs:complexType>
       <xs:complexContent>
@@ -926,14 +937,29 @@
     </xs:annotation>
     <xs:choice maxOccurs="unbounded">
       <xs:element ref="ocx:StructureRef" maxOccurs="unbounded"/>
       <xs:element ref="ocx:StiffenerRef" maxOccurs="unbounded"/>
       <xs:element ref="ocx:SeamRef" maxOccurs="unbounded"/>
       <xs:element ref="ocx:HoleRef" maxOccurs="unbounded"/>
     </xs:choice>
+    <xs:attribute name="id" type="xs:ID" use="required">
+      <xs:annotation>
+        <xs:documentation>An identifier for an element unique within the scope of the XML file. Each id must be unique within a document. The attribute uses the standard XML 1.0 ID type as defined in the XML Schema specification. This attribute is required in many OCX XML elements and an application should generate them automatically.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
+    <xs:attribute name="name" type="xs:string" use="required">
+      <xs:annotation>
+        <xs:documentation>The name of the node</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
+    <xs:attribute name="type">
+      <xs:annotation>
+        <xs:documentation>The design/product  view type</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
   </xs:complexType>
   <!-- ========================================================================================  -->
   <!-- OCX Process Layer -->
   <!-- ========================================================================================  -->
   <xs:element name="ProcessLayer" type="ocx:ProcessLayer_T" abstract="true">
     <xs:annotation>
       <xs:documentation>Abstract element which can hold any process related business information. (To be designed).</xs:documentation>
```

### Comparing `ocx-3.0.0rc5/ocx/ocx_286/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_286/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_286/ocx_286.py` & `ocx-3.0.0rc6/ocx/ocx_286/ocx_286.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_286_fix/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_286_fix/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_286_fix/ocx_286_fix.py` & `ocx-3.0.0rc6/ocx/ocx_286_fix/ocx_286_fix.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b0/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b0/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b0/ocx_300b0.py` & `ocx-3.0.0rc6/ocx/ocx_300b0/ocx_300b0.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b3/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b3/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b3/ocx_300b3.py` & `ocx-3.0.0rc6/ocx/ocx_300b3/ocx_300b3.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b4/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b4/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b4/ocx_300b4.py` & `ocx-3.0.0rc6/ocx/ocx_300b4/ocx_300b4.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b5/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b5/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b5/ocx_300b5.py` & `ocx-3.0.0rc6/ocx/ocx_300b5/ocx_300b5.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b6/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b6/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b6/ocx_300b6.py` & `ocx-3.0.0rc6/ocx/ocx_300b6/ocx_300b6.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b7/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300b7/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300b7/ocx_300b7.py` & `ocx-3.0.0rc6/ocx/ocx_300b7/ocx_300b7.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc1/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300rc1/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc1/ocx_300rc1.py` & `ocx-3.0.0rc6/ocx/ocx_300rc1/ocx_300rc1.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc2/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300rc2/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc2/ocx_300rc2.py` & `ocx-3.0.0rc6/ocx/ocx_300rc2/ocx_300rc2.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc3/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300rc3/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc3/ocx_300rc3.py` & `ocx-3.0.0rc6/ocx/ocx_300rc3/ocx_300rc3.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc4/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300rc4/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc4/ocx_300rc4.py` & `ocx-3.0.0rc6/ocx/ocx_300rc4/ocx_300rc4.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc5/__init__.py` & `ocx-3.0.0rc6/ocx/ocx_300rc5/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/ocx/ocx_300rc5/ocx_300rc5.py` & `ocx-3.0.0rc6/ocx/ocx_300rc5/ocx_300rc5.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc5/pyproject.toml` & `ocx-3.0.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "OCX"
-version = "3.0.0rc5"
+version = "3.0.0rc6"
 description = ""
 authors = ["ocastrup <ole.christain.astrup@dnv.com>"]
 readme = "DATABINDING.md"
 packages = [{include = "ocx"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,15 +23,15 @@
 ocx_databinding = "^2.6"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/OCXStandard/OCX_Schema"
 
 [tool.tbump.version]
-current = "3.0.0rc5"
+current = "3.0.0rc6"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `ocx-3.0.0rc5/PKG-INFO` & `ocx-3.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCX
-Version: 3.0.0rc5
+Version: 3.0.0rc6
 Summary: 
 Author: ocastrup
 Author-email: ole.christain.astrup@dnv.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


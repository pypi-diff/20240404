# Comparing `tmp/opus_protobuf-1.0.47.tar.gz` & `tmp/opus_protobuf-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opus_protobuf-1.0.47.tar", last modified: Wed Mar  6 02:50:25 2024, max compression
+gzip compressed data, was "opus_protobuf-1.0.54.tar", last modified: Tue Mar 19 05:30:45 2024, max compression
```

## Comparing `opus_protobuf-1.0.47.tar` & `opus_protobuf-1.0.54.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:50:25.013450 opus_protobuf-1.0.47/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-06 02:50:25.013450 opus_protobuf-1.0.47/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:50:25.013450 opus_protobuf-1.0.47/opus_protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/authentication_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24683 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/payment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/payment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/payment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/score_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/score_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/score_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/statistic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/statistic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    45525 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/statistic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-03-06 02:50:24.929451 opus_protobuf-1.0.47/opus_protobuf/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-06 02:50:24.941451 opus_protobuf-1.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:30:45.382083 opus_protobuf-1.0.54/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-19 05:30:45.382083 opus_protobuf-1.0.54/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:30:45.382083 opus_protobuf-1.0.54/opus_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/authentication_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26314 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/payment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/payment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/payment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/score_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/score_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/score_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/statistic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/statistic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47097 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/statistic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-03-19 05:30:45.306083 opus_protobuf-1.0.54/opus_protobuf/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-19 05:30:45.314083 opus_protobuf-1.0.54/setup.py
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/authentication_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/authentication_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from opus_protobuf import user_pb2 as opus__protobuf_dot_user__pb2
 from opus_protobuf import common_pb2 as opus__protobuf_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"opus_protobuf/authentication.proto\x12\x0e\x61uthentication\x1a\x1bgoogle/protobuf/empty.proto\x1a\x18opus_protobuf/user.proto\x1a\x1aopus_protobuf/common.proto\"/\n\x0cLoginRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\x8a\x01\n\rSignupRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x15\n\x08password\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x16\n\tlast_name\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x0c\n\x04type\x18\x05 \x01(\tB\x0b\n\t_passwordB\x0c\n\n_last_name\"\x1c\n\x0bJWTResponse\x12\r\n\x05token\x18\x01 \x01(\t\"2\n\x13SignupGoogleRequest\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"1\n\x12SignupAppleRequest\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x8d\x01\n\x1dTalentProfileCreateCsvRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08\x62irthday\x18\x02 \x01(\t\x12\x0e\n\x06tenant\x18\x03 \x03(\t\x12\x10\n\x08industry\x18\x04 \x01(\t\x12\x18\n\x10industry_segment\x18\x05 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x06 \x01(\t2\xcf\x07\n\x18\x41uthenticationController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12\x44\n\x05Login\x12\x1c.authentication.LoginRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12\x46\n\x06Signup\x12\x1d.authentication.SignupRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12\x33\n\x0bGetUserData\x12\x16.google.protobuf.Empty\x1a\n.user.User\"\x00\x12R\n\x0cSignupGoogle\x12#.authentication.SignupGoogleRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12P\n\x0bSignupApple\x12\".authentication.SignupAppleRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12<\n\x14UploadProfilePicture\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12?\n\x17UploadProfilePictureUrl\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12\x39\n\x11UploadTacticCover\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12\x38\n\x10UploadTacticIcon\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12<\n\x14UploadSubtacticCover\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12;\n\x13UploadSubtacticIcon\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12[\n\x16TalentProfileCreateCSV\x12-.authentication.TalentProfileCreateCsvRequest\x1a\x10.common.Document\"\x00\x12\x45\n\x0cRefreshToken\x12\x16.google.protobuf.Empty\x1a\x1b.authentication.JWTResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"opus_protobuf/authentication.proto\x12\x0e\x61uthentication\x1a\x1bgoogle/protobuf/empty.proto\x1a\x18opus_protobuf/user.proto\x1a\x1aopus_protobuf/common.proto\"/\n\x0cLoginRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\x8a\x01\n\rSignupRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x15\n\x08password\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x16\n\tlast_name\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x0c\n\x04type\x18\x05 \x01(\tB\x0b\n\t_passwordB\x0c\n\n_last_name\"\x1c\n\x0bJWTResponse\x12\r\n\x05token\x18\x01 \x01(\t\"2\n\x13SignupGoogleRequest\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"1\n\x12SignupAppleRequest\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xc1\x02\n\x1dTalentProfileCreateCsvRequest\x12\x12\n\x05\x65mail\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08\x62irthday\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x0e\n\x06tenant\x18\x03 \x03(\t\x12\x10\n\x08industry\x18\x04 \x03(\t\x12\x18\n\x10industry_segment\x18\x05 \x03(\t\x12\x14\n\x07\x63ountry\x18\x06 \x01(\tH\x02\x88\x01\x01\x12\x11\n\x04\x63ity\x18\x07 \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06gender\x18\x08 \x01(\tH\x04\x88\x01\x01\x12\x11\n\x04user\x18\t \x01(\tH\x05\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\n \x01(\tH\x06\x88\x01\x01\x42\x08\n\x06_emailB\x0b\n\t_birthdayB\n\n\x08_countryB\x07\n\x05_cityB\t\n\x07_genderB\x07\n\x05_userB\x0e\n\x0c_description2\x86\x08\n\x18\x41uthenticationController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12\x44\n\x05Login\x12\x1c.authentication.LoginRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12\x46\n\x06Signup\x12\x1d.authentication.SignupRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12\x33\n\x0bGetUserData\x12\x16.google.protobuf.Empty\x1a\n.user.User\"\x00\x12R\n\x0cSignupGoogle\x12#.authentication.SignupGoogleRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12P\n\x0bSignupApple\x12\".authentication.SignupAppleRequest\x1a\x1b.authentication.JWTResponse\"\x00\x12<\n\x14UploadProfilePicture\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12?\n\x17UploadProfilePictureUrl\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12\x35\n\ruploadPostUrl\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12\x39\n\x11UploadTacticCover\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12\x38\n\x10UploadTacticIcon\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12<\n\x14UploadSubtacticCover\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12;\n\x13UploadSubtacticIcon\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12[\n\x16TalentProfileCreateCSV\x12-.authentication.TalentProfileCreateCsvRequest\x1a\x10.common.Document\"\x00\x12\x45\n\x0cRefreshToken\x12\x16.google.protobuf.Empty\x1a\x1b.authentication.JWTResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'opus_protobuf.authentication_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_LOGINREQUEST']._serialized_start=137
@@ -31,11 +31,11 @@
   _globals['_JWTRESPONSE']._serialized_start=327
   _globals['_JWTRESPONSE']._serialized_end=355
   _globals['_SIGNUPGOOGLEREQUEST']._serialized_start=357
   _globals['_SIGNUPGOOGLEREQUEST']._serialized_end=407
   _globals['_SIGNUPAPPLEREQUEST']._serialized_start=409
   _globals['_SIGNUPAPPLEREQUEST']._serialized_end=458
   _globals['_TALENTPROFILECREATECSVREQUEST']._serialized_start=461
-  _globals['_TALENTPROFILECREATECSVREQUEST']._serialized_end=602
-  _globals['_AUTHENTICATIONCONTROLLER']._serialized_start=605
-  _globals['_AUTHENTICATIONCONTROLLER']._serialized_end=1580
+  _globals['_TALENTPROFILECREATECSVREQUEST']._serialized_end=782
+  _globals['_AUTHENTICATIONCONTROLLER']._serialized_start=785
+  _globals['_AUTHENTICATIONCONTROLLER']._serialized_end=1815
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/authentication_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/authentication_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -49,21 +49,29 @@
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     token: str
     type: str
     def __init__(self, token: _Optional[str] = ..., type: _Optional[str] = ...) -> None: ...
 
 class TalentProfileCreateCsvRequest(_message.Message):
-    __slots__ = ("email", "birthday", "tenant", "industry", "industry_segment", "country")
+    __slots__ = ("email", "birthday", "tenant", "industry", "industry_segment", "country", "city", "gender", "user", "description")
     EMAIL_FIELD_NUMBER: _ClassVar[int]
     BIRTHDAY_FIELD_NUMBER: _ClassVar[int]
     TENANT_FIELD_NUMBER: _ClassVar[int]
     INDUSTRY_FIELD_NUMBER: _ClassVar[int]
     INDUSTRY_SEGMENT_FIELD_NUMBER: _ClassVar[int]
     COUNTRY_FIELD_NUMBER: _ClassVar[int]
+    CITY_FIELD_NUMBER: _ClassVar[int]
+    GENDER_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     email: str
     birthday: str
     tenant: _containers.RepeatedScalarFieldContainer[str]
-    industry: str
-    industry_segment: str
+    industry: _containers.RepeatedScalarFieldContainer[str]
+    industry_segment: _containers.RepeatedScalarFieldContainer[str]
     country: str
-    def __init__(self, email: _Optional[str] = ..., birthday: _Optional[str] = ..., tenant: _Optional[_Iterable[str]] = ..., industry: _Optional[str] = ..., industry_segment: _Optional[str] = ..., country: _Optional[str] = ...) -> None: ...
+    city: str
+    gender: str
+    user: str
+    description: str
+    def __init__(self, email: _Optional[str] = ..., birthday: _Optional[str] = ..., tenant: _Optional[_Iterable[str]] = ..., industry: _Optional[_Iterable[str]] = ..., industry_segment: _Optional[_Iterable[str]] = ..., country: _Optional[str] = ..., city: _Optional[str] = ..., gender: _Optional[str] = ..., user: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/authentication_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/authentication_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,19 @@
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
         self.UploadProfilePictureUrl = channel.unary_unary(
                 '/authentication.AuthenticationController/UploadProfilePictureUrl',
                 request_serializer=opus__protobuf_dot_common__pb2.Document.SerializeToString,
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
+        self.uploadPostUrl = channel.unary_unary(
+                '/authentication.AuthenticationController/uploadPostUrl',
+                request_serializer=opus__protobuf_dot_common__pb2.Document.SerializeToString,
+                response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
+                )
         self.UploadTacticCover = channel.unary_unary(
                 '/authentication.AuthenticationController/UploadTacticCover',
                 request_serializer=opus__protobuf_dot_common__pb2.Document.SerializeToString,
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
         self.UploadTacticIcon = channel.unary_unary(
                 '/authentication.AuthenticationController/UploadTacticIcon',
@@ -136,14 +141,20 @@
 
     def UploadProfilePictureUrl(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def uploadPostUrl(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def UploadTacticCover(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UploadTacticIcon(self, request, context):
@@ -215,14 +226,19 @@
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
             'UploadProfilePictureUrl': grpc.unary_unary_rpc_method_handler(
                     servicer.UploadProfilePictureUrl,
                     request_deserializer=opus__protobuf_dot_common__pb2.Document.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
+            'uploadPostUrl': grpc.unary_unary_rpc_method_handler(
+                    servicer.uploadPostUrl,
+                    request_deserializer=opus__protobuf_dot_common__pb2.Document.FromString,
+                    response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
+            ),
             'UploadTacticCover': grpc.unary_unary_rpc_method_handler(
                     servicer.UploadTacticCover,
                     request_deserializer=opus__protobuf_dot_common__pb2.Document.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
             'UploadTacticIcon': grpc.unary_unary_rpc_method_handler(
                     servicer.UploadTacticIcon,
@@ -392,14 +408,31 @@
         return grpc.experimental.unary_unary(request, target, '/authentication.AuthenticationController/UploadProfilePictureUrl',
             opus__protobuf_dot_common__pb2.Document.SerializeToString,
             opus__protobuf_dot_common__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def uploadPostUrl(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/authentication.AuthenticationController/uploadPostUrl',
+            opus__protobuf_dot_common__pb2.Document.SerializeToString,
+            opus__protobuf_dot_common__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def UploadTacticCover(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/common_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/common_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/common_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/notification_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/notification_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from opus_protobuf import common_pb2 as opus__protobuf_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n opus_protobuf/notification.proto\x12\x0cnotification\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\":\n\x1eSendValidationCodeEmailRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"O\n\x1cSendTalentOpportunityRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06talent\x18\x02 \x01(\t\x12\x13\n\x0bopportunity\x18\x03 \x01(\t\"$\n\x14SendCsvReportRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"L\n!SendInquireByCulturalAlertRequest\x12\x0f\n\x07\x63ompany\x18\x01 \x01(\t\x12\x16\n\x0e\x63ultural_alert\x18\x02 \x01(\t\"\xab\x01\n\'SendOpportunityEmailNotificationRequest\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07subject\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x0e\n\x06\x65mails\x18\x03 \x03(\t\x12\x11\n\x04\x62ody\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x11\n\x04html\x18\x05 \x01(\tH\x03\x88\x01\x01\x42\x05\n\x03_idB\n\n\x08_subjectB\x07\n\x05_bodyB\x07\n\x05_html2\xe6\x04\n\x16NotificationController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12\x42\n\x17SendForgotPasswordEmail\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12[\n\x17SendValidationCodeEmail\x12,.notification.SendValidationCodeEmailRequest\x1a\x10.common.Response\"\x00\x12W\n\x15SendTalentOpportunity\x12*.notification.SendTalentOpportunityRequest\x1a\x10.common.Response\"\x00\x12G\n\rSendCsvReport\x12\".notification.SendCsvReportRequest\x1a\x10.common.Response\"\x00\x12\x61\n\x1aSendInquireByCulturalAlert\x12/.notification.SendInquireByCulturalAlertRequest\x1a\x10.common.Response\"\x00\x12m\n SendOpportunityEmailNotification\x12\x35.notification.SendOpportunityEmailNotificationRequest\x1a\x10.common.Response\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n opus_protobuf/notification.proto\x12\x0cnotification\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\":\n\x1eSendValidationCodeEmailRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"O\n\x1cSendTalentOpportunityRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06talent\x18\x02 \x01(\t\x12\x13\n\x0bopportunity\x18\x03 \x01(\t\"$\n\x14SendCsvReportRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"L\n!SendInquireByCulturalAlertRequest\x12\x0f\n\x07\x63ompany\x18\x01 \x01(\t\x12\x16\n\x0e\x63ultural_alert\x18\x02 \x01(\t\"\xab\x01\n\'SendOpportunityEmailNotificationRequest\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07subject\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x0e\n\x06\x65mails\x18\x03 \x03(\t\x12\x11\n\x04\x62ody\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x11\n\x04html\x18\x05 \x01(\tH\x03\x88\x01\x01\x42\x05\n\x03_idB\n\n\x08_subjectB\x07\n\x05_bodyB\x07\n\x05_html\"D\n\x1fSendCulturalAlertInquireRequest\x12\x13\n\x0bopportunity\x18\x01 \x01(\t\x12\x0c\n\x04user\x18\x02 \x01(\t2\xc5\x05\n\x16NotificationController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12\x42\n\x17SendForgotPasswordEmail\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12[\n\x17SendValidationCodeEmail\x12,.notification.SendValidationCodeEmailRequest\x1a\x10.common.Response\"\x00\x12W\n\x15SendTalentOpportunity\x12*.notification.SendTalentOpportunityRequest\x1a\x10.common.Response\"\x00\x12G\n\rSendCsvReport\x12\".notification.SendCsvReportRequest\x1a\x10.common.Response\"\x00\x12\x61\n\x1aSendInquireByCulturalAlert\x12/.notification.SendInquireByCulturalAlertRequest\x1a\x10.common.Response\"\x00\x12m\n SendOpportunityEmailNotification\x12\x35.notification.SendOpportunityEmailNotificationRequest\x1a\x10.common.Response\"\x00\x12]\n\x18SendCulturalAlertInquire\x12-.notification.SendCulturalAlertInquireRequest\x1a\x10.common.Response\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'opus_protobuf.notification_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_SENDVALIDATIONCODEEMAILREQUEST']._serialized_start=107
@@ -29,10 +29,12 @@
   _globals['_SENDTALENTOPPORTUNITYREQUEST']._serialized_end=246
   _globals['_SENDCSVREPORTREQUEST']._serialized_start=248
   _globals['_SENDCSVREPORTREQUEST']._serialized_end=284
   _globals['_SENDINQUIREBYCULTURALALERTREQUEST']._serialized_start=286
   _globals['_SENDINQUIREBYCULTURALALERTREQUEST']._serialized_end=362
   _globals['_SENDOPPORTUNITYEMAILNOTIFICATIONREQUEST']._serialized_start=365
   _globals['_SENDOPPORTUNITYEMAILNOTIFICATIONREQUEST']._serialized_end=536
-  _globals['_NOTIFICATIONCONTROLLER']._serialized_start=539
-  _globals['_NOTIFICATIONCONTROLLER']._serialized_end=1153
+  _globals['_SENDCULTURALALERTINQUIREREQUEST']._serialized_start=538
+  _globals['_SENDCULTURALALERTINQUIREREQUEST']._serialized_end=606
+  _globals['_NOTIFICATIONCONTROLLER']._serialized_start=609
+  _globals['_NOTIFICATIONCONTROLLER']._serialized_end=1318
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/notification_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/notification_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,7 +48,15 @@
     HTML_FIELD_NUMBER: _ClassVar[int]
     id: str
     subject: str
     emails: _containers.RepeatedScalarFieldContainer[str]
     body: str
     html: str
     def __init__(self, id: _Optional[str] = ..., subject: _Optional[str] = ..., emails: _Optional[_Iterable[str]] = ..., body: _Optional[str] = ..., html: _Optional[str] = ...) -> None: ...
+
+class SendCulturalAlertInquireRequest(_message.Message):
+    __slots__ = ("opportunity", "user")
+    OPPORTUNITY_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    opportunity: str
+    user: str
+    def __init__(self, opportunity: _Optional[str] = ..., user: _Optional[str] = ...) -> None: ...
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/notification_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/notification_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,19 @@
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
         self.SendOpportunityEmailNotification = channel.unary_unary(
                 '/notification.NotificationController/SendOpportunityEmailNotification',
                 request_serializer=opus__protobuf_dot_notification__pb2.SendOpportunityEmailNotificationRequest.SerializeToString,
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
+        self.SendCulturalAlertInquire = channel.unary_unary(
+                '/notification.NotificationController/SendCulturalAlertInquire',
+                request_serializer=opus__protobuf_dot_notification__pb2.SendCulturalAlertInquireRequest.SerializeToString,
+                response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
+                )
 
 
 class NotificationControllerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def HealthCheck(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -94,14 +99,20 @@
 
     def SendOpportunityEmailNotification(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SendCulturalAlertInquire(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_NotificationControllerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'HealthCheck': grpc.unary_unary_rpc_method_handler(
                     servicer.HealthCheck,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Health.SerializeToString,
@@ -132,14 +143,19 @@
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
             'SendOpportunityEmailNotification': grpc.unary_unary_rpc_method_handler(
                     servicer.SendOpportunityEmailNotification,
                     request_deserializer=opus__protobuf_dot_notification__pb2.SendOpportunityEmailNotificationRequest.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
+            'SendCulturalAlertInquire': grpc.unary_unary_rpc_method_handler(
+                    servicer.SendCulturalAlertInquire,
+                    request_deserializer=opus__protobuf_dot_notification__pb2.SendCulturalAlertInquireRequest.FromString,
+                    response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'notification.NotificationController', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -260,7 +276,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/notification.NotificationController/SendOpportunityEmailNotification',
             opus__protobuf_dot_notification__pb2.SendOpportunityEmailNotificationRequest.SerializeToString,
             opus__protobuf_dot_common__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SendCulturalAlertInquire(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/notification.NotificationController/SendCulturalAlertInquire',
+            opus__protobuf_dot_notification__pb2.SendCulturalAlertInquireRequest.SerializeToString,
+            opus__protobuf_dot_common__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/payment_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/payment_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/payment_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/payment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/score_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/score_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/score_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/score_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/statistic_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/statistic_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from opus_protobuf import common_pb2 as opus__protobuf_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dopus_protobuf/statistic.proto\x12\tstatistic\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\"e\n\x14UploadPictureRequest\x12\x13\n\x06userId\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x07picture\x18\x03 \x01(\x0b\x32\x10.common.DocumentB\t\n\x07_userId\"\x1b\n\x0b\x44\x61taRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"\x82\x01\n\x0f\x41\x63\x63\x65ssInstagram\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x02id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04user\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03url\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\tB\x05\n\x03_idB\x07\n\x05_userB\x06\n\x04_url\"_\n\x1bInstagramControllerResponse\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.statistic.InstagramApiResponse\x12\x11\n\thave_mean\x18\x02 \x01(\x08\"[\n\x14InstagramApiResponse\x12\r\n\x05value\x18\x01 \x01(\x05\x12\x10\n\x08metadata\x18\x02 \x01(\t\x12\x15\n\x08\x65nd_time\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_end_time\"b\n\x18GetInstagramLikesRequest\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1a.statistic.AccessInstagram\x12\x12\n\x05\x62roke\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_broke\"!\n\x11LinkTikTokRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xce\x01\n\x17LinkTensorSocialRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x0e\n\x06tenant\x18\x05 \x01(\t\x12\x10\n\x08industry\x18\x06 \x01(\t\x12\x18\n\x10industry_segment\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x10\n\x08\x62irthday\x18\t \x01(\t\x12\x0c\n\x04\x63ity\x18\n \x01(\t\"\x8c\x01\n\rTalentProfile\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x0e\n\x06tenant\x18\x03 \x01(\t\x12\x10\n\x08industry\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x18\n\x10industry_segment\x18\x06 \x01(\t\x12\x0e\n\x06gender\x18\x07 \x01(\t\"\xad\x01\n\x0bTalentMedia\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04user\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04link\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05order\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x1e\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x10.common.DocumentB\x07\n\x05_userB\x08\n\x06_titleB\x07\n\x05_linkB\x08\n\x06_order2\x9c\x10\n\x13StatisticController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12G\n\x10uploadSkuPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\x13UserConnectAyrshare\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12>\n\x10GetInstagramInfo\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12]\n\x15GetInstagramFollowers\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12[\n\x13GetInstagramFollows\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramAudienceGender\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramAudienceCity\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x63\n\x1bGetInstagramAudienceCountry\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12Y\n\x11GetInstagramReach\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramInteractions\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x11GetInstagramLikes\x12#.statistic.GetInstagramLikesRequest\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramEngagementRate\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x41\n\x13UpdateSocialNetwork\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12I\n\x17\x43reateAudienceInstagram\x12\x1a.statistic.AccessInstagram\x1a\x10.common.Response\"\x00\x12I\n\x12UploadBrandPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12M\n\x16UploadOpportunityImage\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12Q\n\x1aUploadOpportunityTreatment\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12L\n\x15UploadInterestPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\nLinkTikTok\x12\x1c.statistic.LinkTikTokRequest\x1a\x10.common.Response\"\x00\x12J\n\x10LinkTensorSocial\x12\".statistic.LinkTensorSocialRequest\x1a\x10.common.Response\"\x00\x12\x33\n\x0bReadCsvUser\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12M\n\x16UploadCoverListPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12?\n\x0fTalentUpdateOne\x12\x18.statistic.TalentProfile\x1a\x10.common.Response\"\x00\x12<\n\x0eResyncAllUsers\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x12?\n\x11UploadTalentMedia\x12\x16.statistic.TalentMedia\x1a\x10.common.Response\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dopus_protobuf/statistic.proto\x12\tstatistic\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\"e\n\x14UploadPictureRequest\x12\x13\n\x06userId\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x07picture\x18\x03 \x01(\x0b\x32\x10.common.DocumentB\t\n\x07_userId\"\x1b\n\x0b\x44\x61taRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"\x82\x01\n\x0f\x41\x63\x63\x65ssInstagram\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x02id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04user\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03url\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\tB\x05\n\x03_idB\x07\n\x05_userB\x06\n\x04_url\"_\n\x1bInstagramControllerResponse\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.statistic.InstagramApiResponse\x12\x11\n\thave_mean\x18\x02 \x01(\x08\"[\n\x14InstagramApiResponse\x12\r\n\x05value\x18\x01 \x01(\x05\x12\x10\n\x08metadata\x18\x02 \x01(\t\x12\x15\n\x08\x65nd_time\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_end_time\"b\n\x18GetInstagramLikesRequest\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1a.statistic.AccessInstagram\x12\x12\n\x05\x62roke\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_broke\"!\n\x11LinkTikTokRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xce\x01\n\x17LinkTensorSocialRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x0e\n\x06tenant\x18\x05 \x01(\t\x12\x10\n\x08industry\x18\x06 \x01(\t\x12\x18\n\x10industry_segment\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x10\n\x08\x62irthday\x18\t \x01(\t\x12\x0c\n\x04\x63ity\x18\n \x01(\t\"\x8c\x01\n\rTalentProfile\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x0e\n\x06tenant\x18\x03 \x01(\t\x12\x10\n\x08industry\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x18\n\x10industry_segment\x18\x06 \x01(\t\x12\x0e\n\x06gender\x18\x07 \x01(\t\"\xad\x01\n\x0bTalentMedia\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04user\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04link\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05order\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x1e\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x10.common.DocumentB\x07\n\x05_userB\x08\n\x06_titleB\x07\n\x05_linkB\x08\n\x06_order2\xd3\x10\n\x13StatisticController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12G\n\x10uploadSkuPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\x13UserConnectAyrshare\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12>\n\x10GetInstagramInfo\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12]\n\x15GetInstagramFollowers\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12[\n\x13GetInstagramFollows\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramAudienceGender\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramAudienceCity\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x63\n\x1bGetInstagramAudienceCountry\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12Y\n\x11GetInstagramReach\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramInteractions\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x11GetInstagramLikes\x12#.statistic.GetInstagramLikesRequest\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramEngagementRate\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x41\n\x13UpdateSocialNetwork\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12I\n\x17\x43reateAudienceInstagram\x12\x1a.statistic.AccessInstagram\x1a\x10.common.Response\"\x00\x12I\n\x12UploadBrandPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12M\n\x16UploadOpportunityImage\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12Q\n\x1aUploadOpportunityTreatment\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12L\n\x15UploadInterestPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\nLinkTikTok\x12\x1c.statistic.LinkTikTokRequest\x1a\x10.common.Response\"\x00\x12J\n\x10LinkTensorSocial\x12\".statistic.LinkTensorSocialRequest\x1a\x10.common.Response\"\x00\x12\x33\n\x0bReadCsvUser\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12M\n\x16UploadCoverListPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12?\n\x0fTalentUpdateOne\x12\x18.statistic.TalentProfile\x1a\x10.common.Response\"\x00\x12<\n\x0eResyncAllUsers\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x12?\n\x11UploadTalentMedia\x12\x16.statistic.TalentMedia\x1a\x10.common.Response\"\x00\x12\x35\n\x07\x41\x64\x64Post\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'opus_protobuf.statistic_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_UPLOADPICTUREREQUEST']._serialized_start=101
@@ -40,9 +40,9 @@
   _globals['_LINKTENSORSOCIALREQUEST']._serialized_start=692
   _globals['_LINKTENSORSOCIALREQUEST']._serialized_end=898
   _globals['_TALENTPROFILE']._serialized_start=901
   _globals['_TALENTPROFILE']._serialized_end=1041
   _globals['_TALENTMEDIA']._serialized_start=1044
   _globals['_TALENTMEDIA']._serialized_end=1217
   _globals['_STATISTICCONTROLLER']._serialized_start=1220
-  _globals['_STATISTICCONTROLLER']._serialized_end=3296
+  _globals['_STATISTICCONTROLLER']._serialized_end=3351
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/statistic_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/statistic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/statistic_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/statistic_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,19 @@
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
         self.UploadTalentMedia = channel.unary_unary(
                 '/statistic.StatisticController/UploadTalentMedia',
                 request_serializer=opus__protobuf_dot_statistic__pb2.TalentMedia.SerializeToString,
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
+        self.AddPost = channel.unary_unary(
+                '/statistic.StatisticController/AddPost',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
+                )
 
 
 class StatisticControllerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def HealthCheck(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -303,14 +308,20 @@
 
     def UploadTalentMedia(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def AddPost(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_StatisticControllerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'HealthCheck': grpc.unary_unary_rpc_method_handler(
                     servicer.HealthCheck,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Health.SerializeToString,
@@ -436,14 +447,19 @@
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
             'UploadTalentMedia': grpc.unary_unary_rpc_method_handler(
                     servicer.UploadTalentMedia,
                     request_deserializer=opus__protobuf_dot_statistic__pb2.TalentMedia.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
+            'AddPost': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddPost,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'statistic.StatisticController', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -887,7 +903,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/statistic.StatisticController/UploadTalentMedia',
             opus__protobuf_dot_statistic__pb2.TalentMedia.SerializeToString,
             opus__protobuf_dot_common__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def AddPost(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/statistic.StatisticController/AddPost',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            opus__protobuf_dot_common__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `opus_protobuf-1.0.47/opus_protobuf/user_pb2.py` & `opus_protobuf-1.0.54/opus_protobuf/user_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/user_pb2.pyi` & `opus_protobuf-1.0.54/opus_protobuf/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/opus_protobuf/user_pb2_grpc.py` & `opus_protobuf-1.0.54/opus_protobuf/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.47/setup.py` & `opus_protobuf-1.0.54/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'opus_protobuf',         # How you named your package folder (MyLib)
   packages = ['opus_protobuf'],   # Chose the same as "name"
-  version = '1.0.47',      # Start with a small number and increase it with every change you make
+  version = '1.0.54',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```


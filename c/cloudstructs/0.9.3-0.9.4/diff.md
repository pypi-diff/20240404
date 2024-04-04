# Comparing `tmp/cloudstructs-0.9.3.tar.gz` & `tmp/cloudstructs-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstructs-0.9.3.tar", last modified: Wed Apr  3 13:32:44 2024, max compression
+gzip compressed data, was "cloudstructs-0.9.4.tar", last modified: Thu Apr  4 14:19:38 2024, max compression
```

## Comparing `cloudstructs-0.9.3.tar` & `cloudstructs-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:32:44.184400 cloudstructs-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 13:32:44.184400 cloudstructs-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:32:44.184400 cloudstructs-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:32:44.180400 cloudstructs-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:32:44.180400 cloudstructs-0.9.3/src/cloudstructs/
--rw-r--r--   0 runner    (1001) docker     (127)   182936 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/src/cloudstructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:32:44.180400 cloudstructs-0.9.3/src/cloudstructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/src/cloudstructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3235602 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/src/cloudstructs/_jsii/cloudstructs@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:32:32.000000 cloudstructs-0.9.3/src/cloudstructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:32:44.180400 cloudstructs-0.9.3/src/cloudstructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 13:32:44.000000 cloudstructs-0.9.3/src/cloudstructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 13:32:44.000000 cloudstructs-0.9.3/src/cloudstructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:32:44.000000 cloudstructs-0.9.3/src/cloudstructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 13:32:44.000000 cloudstructs-0.9.3/src/cloudstructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 13:32:44.000000 cloudstructs-0.9.3/src/cloudstructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   184196 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3235913 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/_jsii/cloudstructs@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/top_level.txt
```

### Comparing `cloudstructs-0.9.3/LICENSE` & `cloudstructs-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.3/PKG-INFO` & `cloudstructs-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.3
+Version: 0.9.4
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudstructs-0.9.3/README.md` & `cloudstructs-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.3/setup.py` & `cloudstructs-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudstructs",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "High-level constructs for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/jogold/cloudstructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Jonathan Goldwasser<jonathan.goldwasser@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudstructs",
         "cloudstructs._jsii"
     ],
     "package_data": {
         "cloudstructs._jsii": [
-            "cloudstructs@0.9.3.jsii.tgz"
+            "cloudstructs@0.9.4.jsii.tgz"
         ],
         "cloudstructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudstructs-0.9.3/src/cloudstructs/__init__.py` & `cloudstructs-0.9.4/src/cloudstructs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3041,36 +3041,39 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         domain_name: builtins.str,
         hosted_zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
         backend_configuration: typing.Any = None,
+        cache_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy] = None,
         edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
         redirects: typing.Optional[typing.Sequence[builtins.str]] = None,
         response_headers_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ResponseHeadersPolicy] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param domain_name: The domain name for this static website.
         :param hosted_zone: The hosted zone where records should be added.
         :param backend_configuration: A backend configuration that will be saved as ``config.json`` in the S3 bucket of the static website. The frontend can query this config by doing ``fetch('/config.json')``.
+        :param cache_policy: Cache policy for the default behavior. Default: CachePolicy.CACHING_OPTIMIZED
         :param edge_lambdas: The Lambda@Edge functions to invoke before serving the contents. Default: - an origin request function that redirects all requests for a path to /index.html
         :param redirects: A list of domain names that should redirect to ``domainName``. Default: - the domain name of the hosted zone
         :param response_headers_policy: Response headers policy for the default behavior. Default: - a new policy is created with best practice security headers
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5c6cce44b6a8e2d4fefe372623c811f7e7e92ce467f8e830604203b6e57fafd1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StaticWebsiteProps(
             domain_name=domain_name,
             hosted_zone=hosted_zone,
             backend_configuration=backend_configuration,
+            cache_policy=cache_policy,
             edge_lambdas=edge_lambdas,
             redirects=redirects,
             response_headers_policy=response_headers_policy,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -3108,53 +3111,59 @@
 @jsii.data_type(
     jsii_type="cloudstructs.StaticWebsiteProps",
     jsii_struct_bases=[],
     name_mapping={
         "domain_name": "domainName",
         "hosted_zone": "hostedZone",
         "backend_configuration": "backendConfiguration",
+        "cache_policy": "cachePolicy",
         "edge_lambdas": "edgeLambdas",
         "redirects": "redirects",
         "response_headers_policy": "responseHeadersPolicy",
     },
 )
 class StaticWebsiteProps:
     def __init__(
         self,
         *,
         domain_name: builtins.str,
         hosted_zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
         backend_configuration: typing.Any = None,
+        cache_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy] = None,
         edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
         redirects: typing.Optional[typing.Sequence[builtins.str]] = None,
         response_headers_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ResponseHeadersPolicy] = None,
     ) -> None:
         '''Properties for a StaticWebsite.
 
         :param domain_name: The domain name for this static website.
         :param hosted_zone: The hosted zone where records should be added.
         :param backend_configuration: A backend configuration that will be saved as ``config.json`` in the S3 bucket of the static website. The frontend can query this config by doing ``fetch('/config.json')``.
+        :param cache_policy: Cache policy for the default behavior. Default: CachePolicy.CACHING_OPTIMIZED
         :param edge_lambdas: The Lambda@Edge functions to invoke before serving the contents. Default: - an origin request function that redirects all requests for a path to /index.html
         :param redirects: A list of domain names that should redirect to ``domainName``. Default: - the domain name of the hosted zone
         :param response_headers_policy: Response headers policy for the default behavior. Default: - a new policy is created with best practice security headers
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4daf76d01dee77dafb229e369b86df1b96ef0477a43bf4df595b7453b0e74392)
             check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
             check_type(argname="argument hosted_zone", value=hosted_zone, expected_type=type_hints["hosted_zone"])
             check_type(argname="argument backend_configuration", value=backend_configuration, expected_type=type_hints["backend_configuration"])
+            check_type(argname="argument cache_policy", value=cache_policy, expected_type=type_hints["cache_policy"])
             check_type(argname="argument edge_lambdas", value=edge_lambdas, expected_type=type_hints["edge_lambdas"])
             check_type(argname="argument redirects", value=redirects, expected_type=type_hints["redirects"])
             check_type(argname="argument response_headers_policy", value=response_headers_policy, expected_type=type_hints["response_headers_policy"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain_name": domain_name,
             "hosted_zone": hosted_zone,
         }
         if backend_configuration is not None:
             self._values["backend_configuration"] = backend_configuration
+        if cache_policy is not None:
+            self._values["cache_policy"] = cache_policy
         if edge_lambdas is not None:
             self._values["edge_lambdas"] = edge_lambdas
         if redirects is not None:
             self._values["redirects"] = redirects
         if response_headers_policy is not None:
             self._values["response_headers_policy"] = response_headers_policy
 
@@ -3187,14 +3196,25 @@
 
             { userPoolId: '1234', apiEndoint: 'https://www.my-api.com/api' }
         '''
         result = self._values.get("backend_configuration")
         return typing.cast(typing.Any, result)
 
     @builtins.property
+    def cache_policy(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy]:
+        '''Cache policy for the default behavior.
+
+        :default: CachePolicy.CACHING_OPTIMIZED
+        '''
+        result = self._values.get("cache_policy")
+        return typing.cast(typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy], result)
+
+    @builtins.property
     def edge_lambdas(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda]]:
         '''The Lambda@Edge functions to invoke before serving the contents.
 
         :default: - an origin request function that redirects all requests for a path to /index.html
         '''
@@ -4036,14 +4056,15 @@
 def _typecheckingstub__5c6cce44b6a8e2d4fefe372623c811f7e7e92ce467f8e830604203b6e57fafd1(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     domain_name: builtins.str,
     hosted_zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
     backend_configuration: typing.Any = None,
+    cache_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy] = None,
     edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
     redirects: typing.Optional[typing.Sequence[builtins.str]] = None,
     response_headers_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ResponseHeadersPolicy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -4054,14 +4075,15 @@
     pass
 
 def _typecheckingstub__4daf76d01dee77dafb229e369b86df1b96ef0477a43bf4df595b7453b0e74392(
     *,
     domain_name: builtins.str,
     hosted_zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
     backend_configuration: typing.Any = None,
+    cache_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ICachePolicy] = None,
     edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
     redirects: typing.Optional[typing.Sequence[builtins.str]] = None,
     response_headers_policy: typing.Optional[_aws_cdk_aws_cloudfront_ceddda9d.ResponseHeadersPolicy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cloudstructs-0.9.3/src/cloudstructs.egg-info/PKG-INFO` & `cloudstructs-0.9.4/src/cloudstructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.3
+Version: 0.9.4
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


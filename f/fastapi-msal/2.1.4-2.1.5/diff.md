# Comparing `tmp/fastapi_msal-2.1.4.tar.gz` & `tmp/fastapi_msal-2.1.5.tar.gz`

## Comparing `fastapi_msal-2.1.4.tar` & `fastapi_msal-2.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/_version.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/py.typed
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/clients/__init__.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/clients/async_conf_client.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/core/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/core/msal_client_config.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/core/session_manager.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/core/utils.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/auth_code.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/auth_token.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/base_auth_model.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/common.py
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/id_token_claims.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/local_account.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/models/user_info.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/security/__init__.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/security/msal_auth_code_handler.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/fastapi_msal/security/msal_scheme.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/LICENSE
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/README.md
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 fastapi_msal-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/_version.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/auth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/py.typed
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/clients/__init__.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/clients/async_conf_client.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/core/__init__.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/core/msal_client_config.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/core/session_manager.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/core/utils.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/auth_code.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/auth_token.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/base_auth_model.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/common.py
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/id_token_claims.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/local_account.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/models/user_info.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/security/__init__.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/security/msal_auth_code_handler.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/fastapi_msal/security/msal_scheme.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/LICENSE
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/README.md
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 fastapi_msal-2.1.5/PKG-INFO
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/auth.py` & `fastapi_msal-2.1.5/fastapi_msal/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,18 @@
         redirect_uri: OptStr = None,
         state: OptStr = None,
         client_id: OptStr = None,
     ) -> RedirectResponse:
         if client_id:
             print(client_id)
         if not redirect_uri:
-            redirect_uri = str(request.url_for("_get_token_route"))
+            if self.handler.client_config.redirect_uri:
+                redirect_uri = self.handler.client_config.redirect_uri
+            else:
+                redirect_uri = str(request.url_for("_get_token_route"))
         return await self.handler.authorize_redirect(request=request, redirec_uri=redirect_uri, state=state)
 
     async def _get_token_route(self, request: Request, code: str, state: OptStr) -> RedirectResponse:
         await self.handler.authorize_access_token(request=request, code=code, state=state)
         return RedirectResponse(url=f"{self.return_to_path}", headers=dict(request.headers.items()))
 
     async def _post_token_route(
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/clients/async_conf_client.py` & `fastapi_msal-2.1.5/fastapi_msal/clients/async_conf_client.py`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/fastapi_msal/core/msal_client_config.py` & `fastapi_msal-2.1.5/fastapi_msal/core/msal_client_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     # Set the following params if you wish to change the default MSAL Router endpoints
     path_prefix: str = ""
     login_path: str = "/_login_route"
     token_path: str = "/token"
     logout_path: str = "/_logout_route"
     show_in_docs: bool = False
 
+    # Optional uri for redirect (token path) in cases where the app is behind a reverse proxy (PR #35)
+    redirect_uri: OptStr = None
+
     # Optional Params for Logging and Telemetry with AAD
     app_name: OptStr = None
     app_version: OptStr = None
 
     @property
     def authority(self) -> str:
         if not self.policy:
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/core/session_manager.py` & `fastapi_msal-2.1.5/fastapi_msal/core/session_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/fastapi_msal/models/auth_token.py` & `fastapi_msal-2.1.5/fastapi_msal/models/auth_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/fastapi_msal/models/base_auth_model.py` & `fastapi_msal-2.1.5/fastapi_msal/models/base_auth_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import Optional, TypeVar
 
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 
 from fastapi_msal.core import OptStrsDict, SessionManager, StrsDict
 
 AuthModel = TypeVar("AuthModel", bound="BaseAuthModel")
 
 
 class BaseAuthModel(BaseModel):
     _recieved: OptStrsDict = PrivateAttr(None)
+    model_config = ConfigDict(extra="allow")
+    """
+    extra="allow"
+        for Pydantic to save additional fields that are not defined in the model.
+        Since the ID token can have additional fields defined in the app registration portal.
+        To access these fields (if any), use the `__pydantic_extra__` attribute of the object.
+        https://docs.pydantic.dev/latest/concepts/models/#extra-fields
+    """
 
     @classmethod
     def parse_obj_debug(cls: type[AuthModel], to_parse: StrsDict) -> AuthModel:
         debug_model: AuthModel = cls.model_validate(obj=to_parse)
         debug_model.__setattr__("_recieved", to_parse)
         return debug_model
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/models/id_token_claims.py` & `fastapi_msal-2.1.5/fastapi_msal/models/id_token_claims.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Union
 
 from msal.oauth2cli import oidc
 from pydantic import BaseModel, Field, PrivateAttr
 
 from fastapi_msal.core import MSALPolicies, OptStr, OptStrsDict
 
+from .base_auth_model import BaseAuthModel
 from .user_info import UserInfo
 
 
 class TokenStatus(Enum):
     """
     The validateion status of a token.
     https://openid.net/specs/openid-connect-core-1_0.html#IDTokenValidation
@@ -72,59 +73,66 @@
     uti: OptStr = None
     """
     Token identifier claim, equivalent to jti in the JWT specification. Unique,
      per-token identifier that is case-sensitive.
     """
 
 
-class IDTokenClaims(UserInfo, AADInternalClaims):
+class IDTokenClaims(UserInfo, AADInternalClaims, BaseAuthModel):
     """
     The ID token is a security token that contains claims about the authentication of an end-user by
       an authorization server, when using a client, and potentially other requested claims.
     The ID token is represented as a JSON Web Token (JWT).
     For more information: https://learn.microsoft.com/en-us/entra/identity-platform/id-token-claims-reference
     """
 
-    exp: Optional[float] = None
-    """
-    The expiration time claim is the time at which the token becomes invalid, represented in epoch time.
-    Your app should use this claim to verify the validity of the token lifetime.
-    """
-
-    not_before: Optional[float] = Field(time.time() - 1, alias="nbf")
-    """
-    This claim is the time at which the token becomes valid, represented in epoch time.
-    This is usually the same as the time the token was issued.
-    Your app should use this claim to verify the validity of the token lifetime.
-    """
-
-    ver: OptStr = None
+    audience: Union[OptStr, list[str]] = Field(None, alias="aud")
     """
-    Indicates the version of the token.
+    An audience claim identifies the intended recipient of the token.
+    For Azure AD B2C, the audience is your app's Application ID, as assigned to your app in the app registration portal.
+    Your app should validate this value and reject the token if it does not match.
     """
 
     issuer: OptStr = Field(None, alias="iss")
     """
     This claim identifies the fastpi_msal token service (STS) that constructs and returns the token.
     It also identifies the Azure AD directory in which the user was authenticated.
     Your app should validate the issuer claim to ensure that the token came from the v2.0 endpoint.
     It also should use the GUID portion of the claim to restrict the set of tenants that can sign in to the app.
     """
 
+    issue_time: Optional[float] = Field(None, alias="iat")
+    """
+    The time at which the token was issued, represented in epoch time.
+    """
+
     identity_provider: OptStr = Field(None, alias="idp")
     """
     Records the identity provider that authenticated the subject of the token.
     This value is identical to the value of the issuer claim unless the user account isn't in the same tenant-
      as the issuer - guests, for instance.
     If the claim isn't present, it means that the value of iss can be used instead.
     For personal accounts being used in an organizational context (for instance, a personal account invited to a tenant),
     the idp claim may be 'live.com' or an STS URI containing the Microsoft account tenant-
      9188040d-6c67-4c5b-b112-36a304b66dad.
     """
 
+    not_before: Optional[float] = Field(time.time() - 1, alias="nbf")
+    """
+    This claim is the time at which the token becomes valid, represented in epoch time.
+    This is usually the same as the time the token was issued.
+    Your app should use this claim to verify the validity of the token lifetime.
+    """
+
+    exp: Optional[float] = None
+    """
+    The expiration time claim is the time at which the token becomes invalid, represented in epoch time.
+    Your app should use this claim to verify the validity of the token lifetime.
+    """
+
     code_hash: OptStr = Field(None, alias="c_hash")
     """
     The code hash is included in ID tokens only when the ID token is issued with an OAuth 2.0 authorization code.
     It can be used to validate the authenticity of an authorization code. To understand how to do this validation,
     see the OpenID Connect specification: https://openid.net/specs/openid-connect-core-1_0.html#HybridIDToken
 
     This claim isn't returned on ID tokens from the /token endpoint.
@@ -137,14 +145,24 @@
     It can be used to validate the authenticity of an access token.
     To understand how to do this validation, see the OpenID Connect specification.
     https://openid.net/specs/openid-connect-core-1_0.html#HybridIDToken
 
     This claim isn't returned on ID tokens from the /token endpoint.
     """
 
+    nonce: OptStr = None
+    """
+    A nonce is a strategy used to mitigate token replay attacks.
+    Your app can specify a nonce in an authorization request by using the nonce query parameter.
+    The value you provide in the request will be emitted unmodified in the nonce claim of an ID token only.
+    This allows your app to verify the value against the value it specified on the request,
+    which associates the app's session with a given ID token.
+    Your app should perform this validation during the ID token validation process.
+    """
+
     subject: OptStr = Field(None, alias="sub")
     """
     This is the principal about which the token asserts information, such as the user of an app.
     This value is immutable and cannot be reassigned or reused.
     It can be used to perform authorization checks safely, such as when the token is used to access a resource.
     By default, the subject claim is populated with the object ID of the user in the directory.
     To learn more: https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-token-session-sso
@@ -154,49 +172,37 @@
     """
     Represents the tenant that the user is signing in to.
     For work and school accounts, the GUID is the immutable tenant ID of the organization that the user is signing in to.
     For sign-ins to the personal Microsoft account tenant (services like Xbox, Teams for Life, or Outlook),
      the value is 9188040d-6c67-4c5b-b112-36a304b66dad.
     """
 
-    audience: Union[OptStr, list[str]] = Field(None, alias="aud")
-    """
-    An audience claim identifies the intended recipient of the token.
-    For Azure AD B2C, the audience is your app's Application ID, as assigned to your app in the app registration portal.
-    Your app should validate this value and reject the token if it does not match.
-    """
-
-    nonce: OptStr = None
+    ver: OptStr = None
     """
-    A nonce is a strategy used to mitigate token replay attacks.
-    Your app can specify a nonce in an authorization request by using the nonce query parameter.
-    The value you provide in the request will be emitted unmodified in the nonce claim of an ID token only.
-    This allows your app to verify the value against the value it specified on the request,
-    which associates the app's session with a given ID token.
-    Your app should perform this validation during the ID token validation process.
+    Indicates the version of the token.
     """
 
-    issue_time: Optional[float] = Field(None, alias="iat")
-    """
-    The time at which the token was issued, represented in epoch time.
-    """
+    #### Review the below claims if still needed
 
     auth_time: Optional[float] = None
     """
     This claim is the time at which a user last entered credentials, represented in epoch time.
     """
 
     msal_policy: Optional[MSALPolicies] = Field(None, alias="tfp")
     """
     This is the name of the policy that was used to acquire the token.
     """
 
+    ### Private attributes
+
     _id_token: Optional[str] = PrivateAttr(None)
     """
     The raw id_token that was used to create this object - private attribute for internal use only
+    Will be set only via the `decode_id_token` method
     """
 
     @staticmethod
     def decode_id_token(id_token: str) -> Optional["IDTokenClaims"]:
         decoded: OptStrsDict = json.loads(oidc.decode_part(id_token.split(".")[1]))
         if decoded:
             token_claims = IDTokenClaims.model_validate(decoded)
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/models/user_info.py` & `fastapi_msal-2.1.5/fastapi_msal/models/user_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,52 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pydantic import BaseModel, Field
+from pydantic import Field
 
-from fastapi_msal.core import OptStr, OptStrList
+from fastapi_msal.core import OptStr, OptStrList, StrList
 
+from .base_auth_model import BaseAuthModel
 
-class UserInfo(BaseModel):
-    first_name: OptStr = Field(None, alias="given_name")
+
+class UserInfo(BaseAuthModel):
+    preferred_username: OptStr = None
     """
-    The user's given name (also known as first name).
+    The primary username that represents the user.
+    It could be an email address, phone number, or a generic username without a specified format.
+    Its value is mutable and might change over time.
+    Since it is mutable, this value must not be used to make authorization decisions.
+    It can be used for username hints, however, and in human-readable UI as a username.
+    The profile scope is required in order to receive this claim. Present only in v2.0 tokens.
     """
 
-    last_name: OptStr = Field(None, alias="family_name")
+    email: OptStr = None
     """
-    The user's surname (also known as last name).
+    Present by default for guest accounts that have an email address.
+    Your app can request the email claim for managed users (from the same tenant) using the email optional claim.
+    This value isn't guaranteed to be correct and is mutable over time.
+    Never use it for authorization or to save data for a user.
+    On the v2.0 endpoint, your app can also request the email OpenID Connect scope -
+    you don't need to request both the optional claim and the scope to get the claim.
     """
 
     display_name: OptStr = Field(None, alias="name")
     """
-    The user's full name in displayable form including all name parts, possibly including titles and suffixes.
+    The name claim provides a human-readable value that identifies the subject of the token.
+    The value isn't guaranteed to be unique, it can be changed, and should be used only for display purposes.
+    The profile scope is required to receive this claim.
+    """
+
+    first_name: OptStr = Field(None, alias="given_name")
+    """
+    The user's given name (also known as first name).
+    """
+
+    last_name: OptStr = Field(None, alias="family_name")
+    """
+    The user's surname (also known as last name).
     """
 
     city: OptStr = None
     """
     The user's city
     """
 
@@ -54,24 +78,14 @@
     It can be used to perform authorization checks safely and as a key in database tables.
     This ID uniquely identifies the user across applications -
     two different applications signing in the same user will receive the same value in the oid claim.
     This means that it can be used when making queries to Microsoft online services, such as the Microsoft Graph.
     The Microsoft Graph will return this ID as the id property for a given user account.
     """
 
-    preferred_username: OptStr = None
-    """
-    The primary username that represents the user.
-    It could be an email address, phone number, or a generic username without a specified format.
-    Its value is mutable and might change over time.
-    Since it is mutable, this value must not be used to make authorization decisions.
-    It can be used for username hints, however, and in human-readable UI as a username.
-    The profile scope is required in order to receive this claim. Present only in v2.0 tokens.
-    """
-
     unique_name: OptStr = None
     """
     Only present in v1.0 tokens. Provides a human readable value that identifies the subject of the token.
     This value isn't guaranteed to be unique within a tenant and should be used only for display purposes.
     """
 
     is_new_user: Optional[bool] = Field(None, alias="newUser")
@@ -89,7 +103,20 @@
     """
     If present, always true, denoting the user is in at least one group.
     Used in place of the groups claim for JWTs in implicit grant flows when the full groups claim extends-
      the URI fragment beyond the URL length limits (currently six or more groups).
     Indicates that the client should use the Microsoft Graph API to determine the user's groups
     (https://graph.microsoft.com/v1.0/users/{userID}/getMemberObjects).
     """
+
+    groups: Union[StrList, str, None] = None
+    """
+    Provides object IDs that represent the group memberships of the subject.
+    The groupMembershipClaims property of the application manifest configures the groups claim on a per-application basis.
+    A value of null excludes all groups, a value of SecurityGroup includes only Active Directory Security Groups,
+    and a value of All includes both Security Groups and Microsoft 365 Distribution Lists.
+
+    See the hasgroups claim for details on using the groups claim with the implicit grant. For other flows,
+    if the number of groups the user is in goes over 150 for SAML and 200 for JWT,
+    then Microsoft Entra ID adds an overage claim to the claim sources.
+    The claim sources point to the Microsoft Graph endpoint that contains the list of groups for the user.
+    """
```

### Comparing `fastapi_msal-2.1.4/fastapi_msal/security/msal_auth_code_handler.py` & `fastapi_msal-2.1.5/fastapi_msal/security/msal_auth_code_handler.py`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/fastapi_msal/security/msal_scheme.py` & `fastapi_msal-2.1.5/fastapi_msal/security/msal_scheme.py`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/.gitignore` & `fastapi_msal-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/LICENSE` & `fastapi_msal-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/README.md` & `fastapi_msal-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_msal-2.1.4/pyproject.toml` & `fastapi_msal-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,28 @@
 
 [tool.hatch.envs.default]
 path         = ".venv"
 dependencies = ["fastapi_msal[dev]"]
 
 [tool.hatch.envs.default.scripts]
 typing = "mypy --install-types --non-interactive {args:fastapi_msal}"
-style  = ["ruff {args:.}", "black --check --diff {args:.}"]
+style  = ["ruff check {args:.}", "black --check --diff {args:.}"]
 fmt    = ["black {args:.}", "ruff --fix {args:.}", "style"]
 test   = "pytest {args:tests}"
 all    = ["style", "typing"]
 
 [tool.black]
 line-length               = 122
 skip-string-normalization = true
 
 [tool.ruff]
 line-length = 122
+
+
+[tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
     "E",
@@ -118,22 +121,22 @@
 ]
 unfixable = [
     # Don't touch unused imports
     "F401",
 ]
 ignore-init-module-imports = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # avoid warnings related to __init__.py files imports
 "__init__.py" = ["PLC0414"]
 
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["fastapi_msal"]
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 
 follow_imports        = "silent"
 warn_redundant_casts  = true
```

### Comparing `fastapi_msal-2.1.4/PKG-INFO` & `fastapi_msal-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_msal
-Version: 2.1.4
+Version: 2.1.5
 Summary: FastAPI/MSAL - The MSAL (Microsoft Authentication Library) plugin for FastAPI!
 Project-URL: Homepage, https://github.com/dudil/fastapi_msal
 Project-URL: Documentation, https://github.com/dudil/fastapi_msal#readme
 Project-URL: Issues, https://github.com/dudil/fastapi_msal/issues
 Project-URL: Source, https://github.com/dudil/fastapi_msal
 Author-email: Dudi Levy <4785835+dudil@users.noreply.github.com>
 License-Expression: MIT
```


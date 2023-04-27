---
title: Using the API global authentication service
description: Contact Center has moved to a global authentication service. The authentication allows for a "clusterless" design pattern and future product expansion. You can utilize this service with backend REST application programming interface (API) server-to-server communication.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Using the API global authentication service
redirect_from:
    - https://support.ringcentral.com/article-v2/Using-the-API-global-authentication-service.html?brand=RingCentral&product=CC&language=en_US
---


### Using the API global authentication service

Contact Center has moved to a global authentication service. The authentication allows for a "clusterless" design pattern and future product expansion. You can utilize this service with backend REST application programming interface (API) server-to-server communication.
Using the service

**Register your application.**
Go to the Application Registration page on the developer portal. Note: If you plan on doing any browser development, you must include any API call origins you plan to use. Failure to do so will cause the browser to reject your API calls due to Cross-Origin Resource Sharing (CORS) policies.
When you register your application, you will receive a client_id and client_secret.

**Create a "Client Password"**
Using RFC 6749 Section 2.3.1 requirements, create a password with your client_id and client_secret.
Use the schema defined in RFC 2617 Section 2 to create a basic authentication string using the client_id as the user ID and client_secret as a password, separated by a colon, then base64 encoded (with padding).

**Example:**
client_id = "NICE"
client_secret = "CXone"
Formatted resulting string = "NICE:CXone"
Formatted and Base64 encoded string = "Zm9vOmJhcg=="
Use the /openid-configuration discovery service to get the token URL.
Make a GET API call to the /openid-configuration endpoint as described on the OpenId Discovery Documentation page.
Use the appropriate "issuer" you selected when registering your application.
The response will include a "token_endpoint" value to use as the URL in the next step to get a token.
You can find additional documentation about this discovery endpoint on the OpenId Connect Discovery Service page.
Make a token request to the endpoint gathered in the previous step.
Use your "Client Password" from the previous steps, along with your AccessKeyId and accessKeySecret, to make a token request (generated in the CXone interface on the Employees Page for Userhub and Users Page for Central).
You must set the Content-Type header to "application/x-www-form-urlencoded".
Client Password is used in the authorization header as a basic authentication.
Example: "Authorization: Basic Zm9vOmJhcg=="
AccessKeyId and accessKeySecret pass as an http body/payload using the "Password" grant type as described in RFC 6749 Section 4.3.2, with the username being the urlencoded accessKeyId and password being the urlencoded accessKeySecret.

**Example:**
accessKeyId = "qwer====" (Note: A real key will be around 50 alphanumeric characters with equal signs at the end)
accessKeySecret = "asdf====" (Note: A real key will be around 50 alphanumeric characters with equals signs at the end)
Formatting rules: "grant_type=password&username={urlencode(accessKeyId)}&password={urlencode(accessKeySecret)}"
Fully formatted example: payload: "grant_type=password&username=qwer%3D%3D%3D%3D&password=asdf%3D%3D%3D%3D"
The response to this request will include an "access_token" to use as a "bearer token" in an authorization header for all API requests.
Use the /cxone-configuration discovery service to get the API base URL.
Make a GET API call to the /cxone-configuration endpoint as described on the CXone Discovery Documentation page.
Use the appropriate "issuer" you selected when registering your application.
Your tenantId passes as a querystring parameter on the URL.
You can get the tenant ID by base64URL decoding the payload portion of your access token. The resulting JSON will contain a "tenantId" ( typically a UUID/GUID).
Linked base64URL decoder is a third-party service with no affiliation to NICE. You should never include the "signature" part of your token when using a third-party service since no signature invalidates a token.
If you want to build your code without giving your info to a third party, you can reverse engineer the sample code on this website and recreate it for your given environment.
You can also use an expired token on the third-party website jwt.io, and it will decode the token for you.
Note: Assure it’s an expired token, as you shouldn’t trust this service with an active access token.
Example url: https://cxone.niceincontact.com/.well-known/cxone-configuration?tenantId=11eb660f-4c6d-34a0-8733-0242ac110002
The response will include the appropriate "api_endpoint" for your business unit to use as the baseURL in all future API calls to the platform, aside from additional authorization calls.

**Example token requests/responses**
We used these example credentials for the requests/responses.
client_id: 067ed166-3fdc-4d83-xxxx
client_secret: GAB1777F2D82BBA6xxxx
accessKeyId: AJ26OWRCU6O6R4MS2KMDM5M7XN3X5YXD74Kxxxxxxxxxx====
accessKeySecret: C5U4J7ZJQAZQRS5N4JFIQLC155VD2SK6GKxxxxxxxxxx====
tenantId: 11e24-4c6d-34a0-8733-0242ac1xxxx
issuer: cxone.niceincontact.com
Using the query discovery service for a token endpoint

**Request**
GET /.well-known/openid-configuration HTTP/1.1        Host: cxone.niceincontact.com

**Response**
HTTP/1.1 200 OKContent-Type: application/json {    "issuer": "https://cxone.niceincontact.com"",    "authorization_endpoint": "https://cxone.niceincontact.com/auth/authorize"",    "token_endpoint": "https://cxone.niceincontact.com/auth/token"",    "userinfo_endpoint": "https://cxone.niceincontact.com/auth/userinfo"",    "jwks_uri": "https://cxone.niceincontact.com/auth/jwks"",    "token_endpoint_auth_methods_supported": [        "client_secret_basic",        "client_secret_post"    ],    "token_endpoint_auth_signing_alg_values_supported": [        "RS256"    ],    "end_session_endpoint": "https://cxone.niceincontact.com/auth/authorize/logout"",    "scopes_supported": [        "openid"    ],    "response_types_supported": [        "code"    ],    "subject_types_supported": [        "public"    ],    "id_token_signing_alg_values_supported": [        "RS256"    ],    "request_object_signing_alg_values_supported": [        "none"    ],    "display_values_supported": [        "page",        "popup"    ],    "claim_types_supported": [        "normal"    ],    "code_challenge_methods_supported": [        "S256"    ]}
Getting a token

**Request**
POST /auth/token HTTP/1.1Host: cxone.niceincontact.comContent-Type: application/x-www-form-urlencodedAuthorization: Basic MDY3ZWQxNjYtM2ZkYy00ZDgzLTgxMDMtZjMyMzVkMDA3OTYxOkZBQjFCQTlDQUM1MjQ3NzdGMkQ4MkJCQTZEMkNDgrant_type=password&username=AJ26OWRCU6OR4MS2KQMV4GSDLCMDM5M7XN3XYXD7KXDFIFT6FFXA%3D%3D%3D%3D&password=C5UJHWRFOPDPWV7ZJQAZQRS5NJFIQLC5VD2SK6GKD6PHKI7OC6ZQ%3D%3D%3D%3D

**Response**
HTTP/1.1 200 OKContent-Type: application/json{    "access_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJyb2xlIjp7ImxlZ2FjeUlkIjoiQWRtaW5pc3RyYXRvciIsImlkIjoiMTFlYjY2MGYtNGUzMC04ZjgwLWEyNTUtMDI0MmFjMTEwMDAyIiwib    GFzdFVwZGF0ZVRpbWUiOjE2MTQyMjU4NDUwMDAsInNlY29uZGFyeVJvbGVzIjpbeyJpZCI6IjExZWI2NjBmLTRlMzAtNDE2MS1hY2UxLTAyNDJhYzExMDAwMyIsImxhc3RVcGRhdGVUaW1lIjoxNjE0MjI1ODIwMDAw    fV19LCJzdWIiOiJ1c2VyOjExZWI2NjBmLTRmZGYtMDJkMC04ZjI4LTAyNDJhYzExMDAwMiIsImlzcyI6Imh0dHBzOi8vYXV0aC5kZXYubmljZS1pbmNvbnRhY3QuY29tIiwiZ2l2ZW5fbmFtZSI6ImZpcnN0IiwiYXV    kIjoiaW5Db250YWN0IEV2b2x2ZUBpbkNvbnRhY3QuY29tIiwiaWNCVUlkIjotNzIxNDg4NjYyLCJuYW1lIjoidXNlcjFAbmljZS5jb20iLCJ0ZW5hbnRJZCI6IjExZWI2NjBmLTRjNmQtMzRhMC04NzMzLTAyNDJhYz    ExMDAwMiIsImZhbWlseV9uYW1lIjoibGFzdCIsInRlbmFudCI6InBlcm1fdGVzdEdBMSIsImljQ2x1c3RlcklkIjoiRE8zMSIsImlhdCI6MTYyNjg3NDY4NiwiZXhwIjoxNjI2ODc4Mjg2fQ.lhMFTwAW1TSo0wxs8W    8LaIcIm3gJWEHUKSJ9eaY0zVAj8HOeAKQgewAba4tTncFlQr9nFn7nD3T0jxZQYkYTRXamHEqXViJOkSeMRrM96FZQ3gNkVjwYCLQs3kkvTlY4bkQh3OZl2FBwo8xii2e8TbeGOJG5LwJhbMrLY56g8",    "token_type": "Bearer",    "expires_in": 3600,    "refresh_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJpbkNvbnRhY3QgRXZvbHZlQGluQ29udGFjdC5jb20iLCJpc3MiOiJodHRwczovL2N4b25lLmRldi5uaWNlaW5jb250YWN0LmNv    bSIsImlkIjoiMTFlYjY2MGYtNGZkZi0wMmQwLThmMjgtMDI0MmFjMTEwMDAyIiwic2Vzc2lvbklkIjoiN2E2YmYzMTQtNGI4Ni00YjA1LTkwOTUtNjNmMzJkNWM0MDZmIiwiaWF0IjoxNjI2ODc0Njg2LCJleHAiOjE    2MjY4ODE4ODZ9.JANoH0SuWtQs0mKJjh8hpwPiH0qTLFwx9TaHnruxeI9pJm4iaTsNcWYix0fOls5Rc0boRtWYzhmJm6xfAoi15O1ioySEpsmYRhkKiVdBDeiR9rIrZHqJxRBaUaSVGosyVUnRvw7NWvEeq7eKt194B    NLZaewLPiC7uCwh4",    "id_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6ImRlZmF1bHQifQ.eyJzdWIiOiJ1c2VyOjExZWI2NjBmLTRmZGYtMDJkMC04ZjI4LTAyNDJhYzExMDAwMiIsImljRG9tYWluIjoiZGV2Lm5    pY2UtaW5jb250YWN0LmNvbSIsImlzcyI6Imh0dHBzOi8vY3hvbmUuZGV2Lm5pY2VpbmNvbnRhY3QuY29tIiwiZ2l2ZW5fbmFtZSI6ImZpcnN0IiwidXNlcklkIjoiMTFlYjY2MGYtNGZkZi0wMmQwLThmMjgtMDI0Mm    FjMTEwMDAyIiwiYXVkIjoiaW5Db250YWN0IEV2b2x2ZUBpbkNvbnRhY3QuY29tIiwiaWNCVUlkIjotNzIxNDg4NjYyLCJ0ZW5hbnRJZCI6IjExZWI2NjBmLTRjNmQtMzRhMC04NzMzLTAyNDJhYzExMDAwMiIsIm5hb    WUiOiJ1c2VyMUBuaWNlLmNvbSIsImZhbWlseV9uYW1lIjoibGFzdCIsInRlbmFudCI6InBlcm1fdGVzdEdBMSIsImljQ2x1c3RlcklkIjoiRE8zMSIsImlhdCI6MTYyNjg3NDY4NiwiZXhwIjoxNjI2ODc4Mjg2fQ.e    4jZoktlg3qbLezAAB9r7C4PhaLBTKWQkLprnEKbLk9FYfBU4bSoh22s94pcxnsHRiC55vpKXbj5hVh7iZUmHv4M2JXSpxwyJcTYQQVtxIiXpfjiAackLUfuEGzEkVTk0EJC4Q9VU3ivyetBeMpkNFh11MfiZfS1b8",    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token"
Using query discovery service for api_endpoint base URL

**Request**
GET /.well-known/cxone-configuration?tenantId=11eb660f-4c6d-34a0-8733-0242ac110002 HTTP/1.1     Host: cxone.niceincontact.com

**Response**
HTTP/1.1 200 OKContent-Type: application/json{    "private": false,    "area": "na1",    "cluster": "B32",    "domain": "niceincontact.com",    "acdDomain": "nice-incontact.com",    "uhDomain": "nice-incontact.com",    "ui_endpoint": "https://na1.nice-incontact.com"",    "auth_endpoint": "https://na1.nice-incontact.com"",    "api_endpoint": "https://api-na1.niceincontact.com"",    "tenantId": "11eb660f-4c6d-34a0-8733-0242ac110002"
Making an API request

**Request**
GET /inContactAPI/services/v25.0/server-time HTTP/1.1Host: api-na1.niceincontact.comAuthorization: bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJyb2xlIjp7ImxlZ2FjeUlkIjoiQWRtaW5pc3RyYXRvciIsImlkIjoiMTFlYjY2MGYtNGUzMC04ZjgwLWEyNTUtMDI0MmFjMTEwMDAyIiwibGFzdFVwZGF0ZVRpbWUiOjE2MTQyMjU4NDUwMDAsInNlY29uZGFyeVJvbGVzIjpbeyJpZCI6IjExZWI2NjBmLTRlMzAtNDE2MS1hY2UxLTAyNDJhYzExMDAwMyIsImxhc3RVcGRhdGVUaW1lIjoxNjE0MjI1ODIwMDAwfV19 LCJzdWIiOiJ1c2VyOjExZWI2NjBmLTRmZGYtMDJkMC04ZjI4LTAyNDJhYzExMDAwMiIsImlzcyI6Imh0dHBzOi8vYXV0aC5kZXYubmljZS1pbmNvbnRhY3QuY29tIiwiZ2l2ZW5fbmFtZSI6ImZpcnN0IiwiYXVkIjoiaW5 Db250YWN0IEV2b2x2ZUBpbkNvbnRhY3QuY29tIiwiaWNCVUlkIjotNzIxNDg4NjYyLCJuYW1lIjoidXNlcjFAbmljZS5jb20iLCJ0ZW5hbnRJZCI6IjExZWI2NjBmLTRjNmQtMzRhMC04NzMzLTAyNDJhYzExMDAwMiIsImZhbWlseV9uYW1lIjoibGFzdCIsInRlbmFudCI6InBlcm1fdGVzdEdBMSIsImljQ2x1c3RlcklkIjoiRE8zMSIsImlhdCI6MTYyNjg3NDY4NiwiZXhwIjoxNjI2ODc4Mjg2fQ.lhMFTwAW1TSo0wxs8W8 - LaIcIm3gJWEHU    KSJ9eaY0zVAj8HOeAKQgewAba4tTncF_lQr9nFn7nD3T0jxZQYkYTRXamHEqXViJOkSeMRrM96FZQ3gNkVjwYCLQs3kkvTlY4bkQh3OZl2FBwo8xii2e8TbeGOJG5LwJhbMrLY56g8 

**Response**
HTTP/1.1 200 SuccessContent-Type: application/json {    "ServerTime": "2021-07-21T13:38:15.3560573Z"}

# Authentication / Authorization

Patient Platorm API's all use OpenId Connect/OAuth 2.0 protocals for authentication and authorization

## Gaining Access

Some instructions on getting credentials

## Authentication

Authenticate using client_credentials against https://pp-sso-alpha.azurewebsites.net/.well-known/openid-configuration

## Authorization

Depending on which api you want to use depends on the scope required.

* Directory - ppd:read
* Query -  ppq:authenticated
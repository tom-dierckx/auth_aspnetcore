# Auth Toolbox

## 3.2.3
- added the current principal to the `IIPermissionApplicationNameProvider.ApplicationName(...)` method, so one can use the claims of the current user in the logic.

## 3.2.2
- Fixed the service registration which gave runtime exceptions due to previous change.

## 3.2.1
- Made it possible to override the default behaviour of retrieving the ApplicationName

## 3.2.0
- Update Digipolis.DataProtection.Postgres to 3.0.0 (.NET Standard 2.0 compatible)

## 3.1.0
- Support for OAuth jwt-up token (userid in X-Authenticated-UserId claim)

## 3.0.0
- Upgrade to ASP.NET Core 2.0

## 2.5.0
- Added header jwt token read with option JwtTokenSource in AuthService.

## 2.4.0
- Added option to disable token lifetimevalidation to enable easier testing.
- Added support for serviceaccount permissions

## 2.3.0

- AspNet CookieAuth authentication ticket lifetime configurable through options
- Add querystring to return url on redirect
- Token refresh when using jwt in session

## 2.2.1

- Clear the authentication cookie on redirect to login.

## 2.2.0

- Return http status codes instead of redirects when request is XMLHttpRequest or call to /api route with CookieAuth

## 2.1.0

- Added possibility to disable the jwt token cookie
- Added possibility to add the jwt token to the session state

## 2.0.0

- conversion to csproj en MSBuild.

## 1.1.2

- Audience validation on token refresh only when set in options and partial match

## 1.1.0

- Added shared data protection key storage for load ballanced setup

## 1.0.5

- Added PDP api key
- Removed caching of PDP response without permission

## 1.0.4

- Added possibility to disable jwt token signature verification for testing purposes

## 1.0.3

- Bugfix token validation on linux

## 1.0.2

- Bugfix client_redirect url buildup due to nginx changing host header

## 1.0.1

- Added development permissions feature

## 1.0.0

- Initial version

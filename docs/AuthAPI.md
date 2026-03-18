# \AuthAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthConfirmPasswordReset**](AuthAPI.md#AuthConfirmPasswordReset) | **Post** /api/auth/local/password-reset/confirm | Confirm password reset with OTP
[**AuthConvertAnonymous**](AuthAPI.md#AuthConvertAnonymous) | **Post** /api/auth/anonymous/convert | Convert anonymous account to full account
[**AuthCreateAnonymous**](AuthAPI.md#AuthCreateAnonymous) | **Post** /api/auth/anonymous | Create anonymous session
[**AuthGetOAuthProviders**](AuthAPI.md#AuthGetOAuthProviders) | **Get** /api/auth/oauth/providers/available | Get all available OAuth providers
[**AuthGetSession**](AuthAPI.md#AuthGetSession) | **Get** /api/auth/local/session | Get current session
[**AuthLogin**](AuthAPI.md#AuthLogin) | **Post** /api/auth/local/login | Login user
[**AuthLogout**](AuthAPI.md#AuthLogout) | **Post** /api/auth/local/logout | Logout user
[**AuthOauthCallback**](AuthAPI.md#AuthOauthCallback) | **Get** /api/auth/oauth/callback/{provider} | OAuth callback handler
[**AuthOauthInitiate**](AuthAPI.md#AuthOauthInitiate) | **Get** /api/auth/oauth/{provider}/{projectId} | Initiate OAuth authentication
[**AuthRefresh**](AuthAPI.md#AuthRefresh) | **Post** /api/auth/refresh | Refresh access token (org and project)
[**AuthRegister**](AuthAPI.md#AuthRegister) | **Post** /api/auth/local/register | Register new user
[**AuthRequestPasswordReset**](AuthAPI.md#AuthRequestPasswordReset) | **Post** /api/auth/local/password-reset | Request password reset (OTP)
[**AuthResetPassword**](AuthAPI.md#AuthResetPassword) | **Post** /api/auth/local/password-reset/{token} | Reset password with token (legacy)
[**AuthSendMagicLink**](AuthAPI.md#AuthSendMagicLink) | **Post** /api/auth/magic-link/send | Send magic link
[**AuthSendOtp**](AuthAPI.md#AuthSendOtp) | **Post** /api/auth/otp/send | Send OTP code
[**AuthVerifyMagicLink**](AuthAPI.md#AuthVerifyMagicLink) | **Post** /api/auth/magic-link/verify | Verify magic link
[**AuthVerifyOtp**](AuthAPI.md#AuthVerifyOtp) | **Post** /api/auth/otp/verify | Verify OTP code



## AuthConfirmPasswordReset

> MessageResponse AuthConfirmPasswordReset(ctx).AuthConfirmPasswordResetRequest(authConfirmPasswordResetRequest).Execute()

Confirm password reset with OTP



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authConfirmPasswordResetRequest := *openapiclient.NewAuthConfirmPasswordResetRequest("user@example.com", "685ad30be129932fbb7a1047", "123456", "NewSecurePass123!") // AuthConfirmPasswordResetRequest | Email, projectId, OTP code, and new password.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthConfirmPasswordReset(context.Background()).AuthConfirmPasswordResetRequest(authConfirmPasswordResetRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthConfirmPasswordReset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthConfirmPasswordReset`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthConfirmPasswordReset`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthConfirmPasswordResetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authConfirmPasswordResetRequest** | [**AuthConfirmPasswordResetRequest**](AuthConfirmPasswordResetRequest.md) | Email, projectId, OTP code, and new password. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthConvertAnonymous

> AuthConvertAnonymous200Response AuthConvertAnonymous(ctx).AuthConvertAnonymousRequest(authConvertAnonymousRequest).Execute()

Convert anonymous account to full account



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authConvertAnonymousRequest := *openapiclient.NewAuthConvertAnonymousRequest("user@example.com", "SecurePassword123!") // AuthConvertAnonymousRequest | Email, password, and optional firstName, lastName for the new full account.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthConvertAnonymous(context.Background()).AuthConvertAnonymousRequest(authConvertAnonymousRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthConvertAnonymous``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthConvertAnonymous`: AuthConvertAnonymous200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthConvertAnonymous`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthConvertAnonymousRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authConvertAnonymousRequest** | [**AuthConvertAnonymousRequest**](AuthConvertAnonymousRequest.md) | Email, password, and optional firstName, lastName for the new full account. | 

### Return type

[**AuthConvertAnonymous200Response**](AuthConvertAnonymous200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthCreateAnonymous

> AuthCreateAnonymous200Response AuthCreateAnonymous(ctx).AuthCreateAnonymousRequest(authCreateAnonymousRequest).Execute()

Create anonymous session



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authCreateAnonymousRequest := *openapiclient.NewAuthCreateAnonymousRequest() // AuthCreateAnonymousRequest | Optional projectId and deviceId for the anonymous session. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthCreateAnonymous(context.Background()).AuthCreateAnonymousRequest(authCreateAnonymousRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthCreateAnonymous``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthCreateAnonymous`: AuthCreateAnonymous200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthCreateAnonymous`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthCreateAnonymousRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authCreateAnonymousRequest** | [**AuthCreateAnonymousRequest**](AuthCreateAnonymousRequest.md) | Optional projectId and deviceId for the anonymous session. | 

### Return type

[**AuthCreateAnonymous200Response**](AuthCreateAnonymous200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthGetOAuthProviders

> AuthGetOAuthProviders200Response AuthGetOAuthProviders(ctx).Execute()

Get all available OAuth providers



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthGetOAuthProviders(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthGetOAuthProviders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthGetOAuthProviders`: AuthGetOAuthProviders200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthGetOAuthProviders`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAuthGetOAuthProvidersRequest struct via the builder pattern


### Return type

[**AuthGetOAuthProviders200Response**](AuthGetOAuthProviders200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthGetSession

> AuthGetSession200Response AuthGetSession(ctx).ProjectId(projectId).Execute()

Get current session



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	projectId := "projectId_example" // string | Project ID to get session for.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthGetSession(context.Background()).ProjectId(projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthGetSession``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthGetSession`: AuthGetSession200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthGetSession`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthGetSessionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **projectId** | **string** | Project ID to get session for. | 

### Return type

[**AuthGetSession200Response**](AuthGetSession200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthLogin

> AuthLogin200Response AuthLogin(ctx).AuthLoginRequest(authLoginRequest).Execute()

Login user



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authLoginRequest := *openapiclient.NewAuthLoginRequest("Email_example", "Password_example") // AuthLoginRequest | Login credentials (email, password) and project ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthLogin(context.Background()).AuthLoginRequest(authLoginRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthLogin``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthLogin`: AuthLogin200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthLogin`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthLoginRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authLoginRequest** | [**AuthLoginRequest**](AuthLoginRequest.md) | Login credentials (email, password) and project ID. | 

### Return type

[**AuthLogin200Response**](AuthLogin200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthLogout

> MessageResponse AuthLogout(ctx).Execute()

Logout user



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthLogout(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthLogout``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthLogout`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthLogout`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAuthLogoutRequest struct via the builder pattern


### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthOauthCallback

> AuthOauthCallback200Response AuthOauthCallback(ctx, provider).Execute()

OAuth callback handler



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	provider := "provider_example" // string | OAuth provider identifier (e.g. google, github).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthOauthCallback(context.Background(), provider).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthOauthCallback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthOauthCallback`: AuthOauthCallback200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthOauthCallback`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**provider** | **string** | OAuth provider identifier (e.g. google, github). | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthOauthCallbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AuthOauthCallback200Response**](AuthOauthCallback200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthOauthInitiate

> AuthOauthInitiate200Response AuthOauthInitiate(ctx, provider, projectId).RedirectUrl(redirectUrl).Execute()

Initiate OAuth authentication



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	provider := "google" // string | OAuth provider identifier (e.g. google, github).
	projectId := "685ad30be129932fbb7a1047" // string | Project ID for which OAuth is configured.
	redirectUrl := "https://client.app/auth/callback" // string | The URL to redirect to after authentication. Must be pre-registered in project settings. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthOauthInitiate(context.Background(), provider, projectId).RedirectUrl(redirectUrl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthOauthInitiate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthOauthInitiate`: AuthOauthInitiate200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthOauthInitiate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**provider** | **string** | OAuth provider identifier (e.g. google, github). | 
**projectId** | **string** | Project ID for which OAuth is configured. | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthOauthInitiateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **redirectUrl** | **string** | The URL to redirect to after authentication. Must be pre-registered in project settings. | 

### Return type

[**AuthOauthInitiate200Response**](AuthOauthInitiate200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthRefresh

> AuthRefresh200Response AuthRefresh(ctx).AuthRefreshRequest(authRefreshRequest).Execute()

Refresh access token (org and project)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authRefreshRequest := *openapiclient.NewAuthRefreshRequest("RefreshToken_example") // AuthRefreshRequest | JSON body containing the refresh token to exchange for a new access token and refresh token (token rotation).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthRefresh(context.Background()).AuthRefreshRequest(authRefreshRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthRefresh``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthRefresh`: AuthRefresh200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthRefresh`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthRefreshRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authRefreshRequest** | [**AuthRefreshRequest**](AuthRefreshRequest.md) | JSON body containing the refresh token to exchange for a new access token and refresh token (token rotation). | 

### Return type

[**AuthRefresh200Response**](AuthRefresh200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthRegister

> AuthRegister201Response AuthRegister(ctx).AuthRegisterRequest(authRegisterRequest).Execute()

Register new user



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authRegisterRequest := *openapiclient.NewAuthRegisterRequest("Email_example", "Password_example", "FirstName_example", "LastName_example", "ProjectId_example") // AuthRegisterRequest | Registration payload (email, password, firstName, lastName, projectId).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthRegister(context.Background()).AuthRegisterRequest(authRegisterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthRegister``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthRegister`: AuthRegister201Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthRegister`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthRegisterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authRegisterRequest** | [**AuthRegisterRequest**](AuthRegisterRequest.md) | Registration payload (email, password, firstName, lastName, projectId). | 

### Return type

[**AuthRegister201Response**](AuthRegister201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthRequestPasswordReset

> MessageResponse AuthRequestPasswordReset(ctx).AuthRequestPasswordResetRequest(authRequestPasswordResetRequest).Execute()

Request password reset (OTP)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authRequestPasswordResetRequest := *openapiclient.NewAuthRequestPasswordResetRequest("user@example.com") // AuthRequestPasswordResetRequest | Email and optional projectId for app OTP or org token link.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthRequestPasswordReset(context.Background()).AuthRequestPasswordResetRequest(authRequestPasswordResetRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthRequestPasswordReset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthRequestPasswordReset`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthRequestPasswordReset`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthRequestPasswordResetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authRequestPasswordResetRequest** | [**AuthRequestPasswordResetRequest**](AuthRequestPasswordResetRequest.md) | Email and optional projectId for app OTP or org token link. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthResetPassword

> MessageResponse AuthResetPassword(ctx, token).AuthResetPasswordRequest(authResetPasswordRequest).Execute()

Reset password with token (legacy)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	token := "token_example" // string | Password reset token from email link.
	authResetPasswordRequest := *openapiclient.NewAuthResetPasswordRequest("NewSecurePass123!") // AuthResetPasswordRequest | New password and optional projectId.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthResetPassword(context.Background(), token).AuthResetPasswordRequest(authResetPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthResetPassword``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthResetPassword`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthResetPassword`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Password reset token from email link. | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthResetPasswordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **authResetPasswordRequest** | [**AuthResetPasswordRequest**](AuthResetPasswordRequest.md) | New password and optional projectId. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthSendMagicLink

> MessageResponse AuthSendMagicLink(ctx).MagicLinkRequest(magicLinkRequest).Execute()

Send magic link



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	magicLinkRequest := *openapiclient.NewMagicLinkRequest("Email_example", "ProjectId_example") // MagicLinkRequest | Email, projectId, and optional redirect URL for the magic link.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthSendMagicLink(context.Background()).MagicLinkRequest(magicLinkRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthSendMagicLink``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthSendMagicLink`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthSendMagicLink`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthSendMagicLinkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **magicLinkRequest** | [**MagicLinkRequest**](MagicLinkRequest.md) | Email, projectId, and optional redirect URL for the magic link. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthSendOtp

> MessageResponse AuthSendOtp(ctx).OTPSendRequest(oTPSendRequest).Execute()

Send OTP code



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	oTPSendRequest := *openapiclient.NewOTPSendRequest("ProjectId_example", "Method_example") // OTPSendRequest | Project ID, delivery method (sms/email), and phone or email.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthSendOtp(context.Background()).OTPSendRequest(oTPSendRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthSendOtp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthSendOtp`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthSendOtp`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthSendOtpRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oTPSendRequest** | [**OTPSendRequest**](OTPSendRequest.md) | Project ID, delivery method (sms/email), and phone or email. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthVerifyMagicLink

> AuthResponse AuthVerifyMagicLink(ctx).AuthVerifyMagicLinkRequest(authVerifyMagicLinkRequest).Execute()

Verify magic link



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authVerifyMagicLinkRequest := *openapiclient.NewAuthVerifyMagicLinkRequest("eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InVzZXJAZXhhbXBsZS5jb20iLCJwcm9qZWN0SWQiOiI2ODVhZDMwYmUxMjk5MzJmYmI3YTEwNDciLCJpYXQiOjE3NTA3ODA4OTgsImV4cCI6MTc1MDc4NDQ5OH0.example") // AuthVerifyMagicLinkRequest | The token from the magic link URL.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthVerifyMagicLink(context.Background()).AuthVerifyMagicLinkRequest(authVerifyMagicLinkRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthVerifyMagicLink``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthVerifyMagicLink`: AuthResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthVerifyMagicLink`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthVerifyMagicLinkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authVerifyMagicLinkRequest** | [**AuthVerifyMagicLinkRequest**](AuthVerifyMagicLinkRequest.md) | The token from the magic link URL. | 

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthVerifyOtp

> AuthResponse AuthVerifyOtp(ctx).OTPVerifyRequest(oTPVerifyRequest).Execute()

Verify OTP code



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	oTPVerifyRequest := *openapiclient.NewOTPVerifyRequest("Otp_example", "ProjectId_example") // OTPVerifyRequest | Identifier (phone/email), OTP code, and project ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.AuthVerifyOtp(context.Background()).OTPVerifyRequest(oTPVerifyRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.AuthVerifyOtp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthVerifyOtp`: AuthResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.AuthVerifyOtp`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthVerifyOtpRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oTPVerifyRequest** | [**OTPVerifyRequest**](OTPVerifyRequest.md) | Identifier (phone/email), OTP code, and project ID. | 

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


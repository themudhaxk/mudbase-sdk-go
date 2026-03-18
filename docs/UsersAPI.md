# \UsersAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**UsersChangePassword**](UsersAPI.md#UsersChangePassword) | **Patch** /api/users/password | Change password
[**UsersDisable2fa**](UsersAPI.md#UsersDisable2fa) | **Post** /api/users/2fa/disable | Disable 2FA
[**UsersEraseData**](UsersAPI.md#UsersEraseData) | **Post** /api/users/me/erase | Delete user data (GDPR Article 17)
[**UsersExportData**](UsersAPI.md#UsersExportData) | **Get** /api/users/me/export | Export user data (GDPR Article 15)
[**UsersGet**](UsersAPI.md#UsersGet) | **Get** /api/users/me | Get current user profile
[**UsersLinkOAuthProvider**](UsersAPI.md#UsersLinkOAuthProvider) | **Get** /api/users/me/oauth-providers/link/{provider} | Link OAuth provider to account
[**UsersListOAuthProviders**](UsersAPI.md#UsersListOAuthProviders) | **Get** /api/users/me/oauth-providers | List linked OAuth providers
[**UsersResendVerification**](UsersAPI.md#UsersResendVerification) | **Post** /api/users/resend-verification | Resend verification email
[**UsersSetup2fa**](UsersAPI.md#UsersSetup2fa) | **Post** /api/users/2fa/setup | Initiate two-factor authentication setup (secret, QR code, backup codes)
[**UsersUnlinkOAuthProvider**](UsersAPI.md#UsersUnlinkOAuthProvider) | **Delete** /api/users/me/oauth-providers/{provider} | Unlink OAuth provider
[**UsersUpdate**](UsersAPI.md#UsersUpdate) | **Patch** /api/users/update | Update user profile
[**UsersVerify2fa**](UsersAPI.md#UsersVerify2fa) | **Post** /api/users/2fa/verify | Verify and enable 2FA
[**UsersVerifyEmail**](UsersAPI.md#UsersVerifyEmail) | **Post** /api/users/verify-email | Verify email address (organization and project)



## UsersChangePassword

> MessageResponse UsersChangePassword(ctx).ChangePasswordRequest(changePasswordRequest).Execute()

Change password



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
	changePasswordRequest := *openapiclient.NewChangePasswordRequest("CurrentPassword_example", "NewPassword_example") // ChangePasswordRequest | Current password and new password.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersChangePassword(context.Background()).ChangePasswordRequest(changePasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersChangePassword``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersChangePassword`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersChangePassword`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersChangePasswordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **changePasswordRequest** | [**ChangePasswordRequest**](ChangePasswordRequest.md) | Current password and new password. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersDisable2fa

> MessageResponse UsersDisable2fa(ctx).UsersDisable2faRequest(usersDisable2faRequest).Execute()

Disable 2FA



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
	usersDisable2faRequest := *openapiclient.NewUsersDisable2faRequest("SecurePass123!", "123456") // UsersDisable2faRequest | Current password and one-time code to confirm disable.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersDisable2fa(context.Background()).UsersDisable2faRequest(usersDisable2faRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersDisable2fa``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersDisable2fa`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersDisable2fa`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersDisable2faRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **usersDisable2faRequest** | [**UsersDisable2faRequest**](UsersDisable2faRequest.md) | Current password and one-time code to confirm disable. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersEraseData

> UsersEraseData200Response UsersEraseData(ctx).UsersEraseDataRequest(usersEraseDataRequest).Execute()

Delete user data (GDPR Article 17)



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
	usersEraseDataRequest := *openapiclient.NewUsersEraseDataRequest("DELETE_MY_ACCOUNT") // UsersEraseDataRequest | Confirmation string (DELETE_MY_ACCOUNT) and optional reason for erasure.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersEraseData(context.Background()).UsersEraseDataRequest(usersEraseDataRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersEraseData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersEraseData`: UsersEraseData200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersEraseData`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersEraseDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **usersEraseDataRequest** | [**UsersEraseDataRequest**](UsersEraseDataRequest.md) | Confirmation string (DELETE_MY_ACCOUNT) and optional reason for erasure. | 

### Return type

[**UsersEraseData200Response**](UsersEraseData200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersExportData

> UsersExportData200Response UsersExportData(ctx).Execute()

Export user data (GDPR Article 15)



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
	resp, r, err := apiClient.UsersAPI.UsersExportData(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersExportData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersExportData`: UsersExportData200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersExportData`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUsersExportDataRequest struct via the builder pattern


### Return type

[**UsersExportData200Response**](UsersExportData200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersGet

> UsersGet200Response UsersGet(ctx).Execute()

Get current user profile



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
	resp, r, err := apiClient.UsersAPI.UsersGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersGet`: UsersGet200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUsersGetRequest struct via the builder pattern


### Return type

[**UsersGet200Response**](UsersGet200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersLinkOAuthProvider

> UsersLinkOAuthProvider200Response UsersLinkOAuthProvider(ctx, provider).ProjectId(projectId).Execute()

Link OAuth provider to account



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
	provider := "google" // string | OAuth provider to link (e.g. google, github).
	projectId := "685ad30be129932fbb7a1047" // string | Project ID for the OAuth link context. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersLinkOAuthProvider(context.Background(), provider).ProjectId(projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersLinkOAuthProvider``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersLinkOAuthProvider`: UsersLinkOAuthProvider200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersLinkOAuthProvider`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**provider** | **string** | OAuth provider to link (e.g. google, github). | 

### Other Parameters

Other parameters are passed through a pointer to a apiUsersLinkOAuthProviderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **projectId** | **string** | Project ID for the OAuth link context. | 

### Return type

[**UsersLinkOAuthProvider200Response**](UsersLinkOAuthProvider200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersListOAuthProviders

> UsersListOAuthProviders200Response UsersListOAuthProviders(ctx).Execute()

List linked OAuth providers



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
	resp, r, err := apiClient.UsersAPI.UsersListOAuthProviders(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersListOAuthProviders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersListOAuthProviders`: UsersListOAuthProviders200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersListOAuthProviders`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUsersListOAuthProvidersRequest struct via the builder pattern


### Return type

[**UsersListOAuthProviders200Response**](UsersListOAuthProviders200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersResendVerification

> MessageResponse UsersResendVerification(ctx).Execute()

Resend verification email



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
	resp, r, err := apiClient.UsersAPI.UsersResendVerification(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersResendVerification``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersResendVerification`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersResendVerification`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUsersResendVerificationRequest struct via the builder pattern


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


## UsersSetup2fa

> TwoFASetupResponse UsersSetup2fa(ctx).Execute()

Initiate two-factor authentication setup (secret, QR code, backup codes)



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
	resp, r, err := apiClient.UsersAPI.UsersSetup2fa(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersSetup2fa``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersSetup2fa`: TwoFASetupResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersSetup2fa`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiUsersSetup2faRequest struct via the builder pattern


### Return type

[**TwoFASetupResponse**](TwoFASetupResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersUnlinkOAuthProvider

> UsersUnlinkOAuthProvider200Response UsersUnlinkOAuthProvider(ctx, provider).Execute()

Unlink OAuth provider



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
	provider := "github" // string | OAuth provider to unlink (e.g. google, github).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersUnlinkOAuthProvider(context.Background(), provider).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersUnlinkOAuthProvider``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersUnlinkOAuthProvider`: UsersUnlinkOAuthProvider200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersUnlinkOAuthProvider`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**provider** | **string** | OAuth provider to unlink (e.g. google, github). | 

### Other Parameters

Other parameters are passed through a pointer to a apiUsersUnlinkOAuthProviderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**UsersUnlinkOAuthProvider200Response**](UsersUnlinkOAuthProvider200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersUpdate

> UsersUpdate200Response UsersUpdate(ctx).UpdateUserRequest(updateUserRequest).Execute()

Update user profile



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
	updateUserRequest := *openapiclient.NewUpdateUserRequest() // UpdateUserRequest | Profile fields to update (firstName, lastName, avatar).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersUpdate(context.Background()).UpdateUserRequest(updateUserRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersUpdate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersUpdate`: UsersUpdate200Response
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersUpdate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersUpdateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateUserRequest** | [**UpdateUserRequest**](UpdateUserRequest.md) | Profile fields to update (firstName, lastName, avatar). | 

### Return type

[**UsersUpdate200Response**](UsersUpdate200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersVerify2fa

> MessageResponse UsersVerify2fa(ctx).UsersVerify2faRequest(usersVerify2faRequest).Execute()

Verify and enable 2FA



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
	usersVerify2faRequest := *openapiclient.NewUsersVerify2faRequest("123456") // UsersVerify2faRequest | One-time code from the authenticator app.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersVerify2fa(context.Background()).UsersVerify2faRequest(usersVerify2faRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersVerify2fa``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersVerify2fa`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersVerify2fa`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersVerify2faRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **usersVerify2faRequest** | [**UsersVerify2faRequest**](UsersVerify2faRequest.md) | One-time code from the authenticator app. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsersVerifyEmail

> MessageResponse UsersVerifyEmail(ctx).UsersVerifyEmailRequest(usersVerifyEmailRequest).Execute()

Verify email address (organization and project)



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
	usersVerifyEmailRequest := *openapiclient.NewUsersVerifyEmailRequest("Token_example") // UsersVerifyEmailRequest | Verification token from the email link; optional projectId for project context.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UsersVerifyEmail(context.Background()).UsersVerifyEmailRequest(usersVerifyEmailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UsersVerifyEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsersVerifyEmail`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UsersVerifyEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsersVerifyEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **usersVerifyEmailRequest** | [**UsersVerifyEmailRequest**](UsersVerifyEmailRequest.md) | Verification token from the email link; optional projectId for project context. | 

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


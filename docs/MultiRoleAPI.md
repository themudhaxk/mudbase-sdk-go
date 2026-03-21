# \MultiRoleAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthOauthSignupWithRole**](MultiRoleAPI.md#AuthOauthSignupWithRole) | **Get** /api/auth/oauth/signup/{role}/{provider}/{projectId} | OAuth signup with specific role
[**AuthRegisterWithRole**](MultiRoleAPI.md#AuthRegisterWithRole) | **Post** /api/auth/local/signup/{role} | Register user with specific role (Local Auth)



## AuthOauthSignupWithRole

> UsersLinkOAuthProvider200Response AuthOauthSignupWithRole(ctx, role, provider, projectId).RedirectUrl(redirectUrl).Execute()

OAuth signup with specific role



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
	role := "customer" // string | Path segment must match the role's `signupEndpoint` (default `customer`; use each role's configured endpoint).
	provider := "google" // string | OAuth provider (e.g. google, github).
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	redirectUrl := "https://client.app/auth/callback" // string | The URL to redirect to after authentication (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.AuthOauthSignupWithRole(context.Background(), role, provider, projectId).RedirectUrl(redirectUrl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.AuthOauthSignupWithRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthOauthSignupWithRole`: UsersLinkOAuthProvider200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.AuthOauthSignupWithRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**role** | **string** | Path segment must match the role&#39;s &#x60;signupEndpoint&#x60; (default &#x60;customer&#x60;; use each role&#39;s configured endpoint). | 
**provider** | **string** | OAuth provider (e.g. google, github). | 
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthOauthSignupWithRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **redirectUrl** | **string** | The URL to redirect to after authentication | 

### Return type

[**UsersLinkOAuthProvider200Response**](UsersLinkOAuthProvider200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AuthRegisterWithRole

> AuthRegisterWithRole(ctx, role).AuthRegisterWithRoleRequest(authRegisterWithRoleRequest).Execute()

Register user with specific role (Local Auth)



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
	role := "customer" // string | Must match the role's `signupEndpoint` (default `customer`; other values for roles you add).
	authRegisterWithRoleRequest := *openapiclient.NewAuthRegisterWithRoleRequest("Email_example", "Password_example", "FirstName_example", "LastName_example", "ProjectId_example") // AuthRegisterWithRoleRequest | Registration payload (email, password, firstName, lastName, projectId).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MultiRoleAPI.AuthRegisterWithRole(context.Background(), role).AuthRegisterWithRoleRequest(authRegisterWithRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.AuthRegisterWithRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**role** | **string** | Must match the role&#39;s &#x60;signupEndpoint&#x60; (default &#x60;customer&#x60;; other values for roles you add). | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthRegisterWithRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **authRegisterWithRoleRequest** | [**AuthRegisterWithRoleRequest**](AuthRegisterWithRoleRequest.md) | Registration payload (email, password, firstName, lastName, projectId). | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


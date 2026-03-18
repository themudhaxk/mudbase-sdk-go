# \MultiRoleAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthOauthSignupWithRole**](MultiRoleAPI.md#AuthOauthSignupWithRole) | **Get** /api/auth/oauth/signup/{role}/{provider}/{projectId} | OAuth signup with specific role
[**AuthRegisterWithRole**](MultiRoleAPI.md#AuthRegisterWithRole) | **Post** /api/auth/local/signup/{role} | Register user with specific role (Local Auth)
[**MultiRoleAddRole**](MultiRoleAPI.md#MultiRoleAddRole) | **Post** /api/projects/{projectId}/multi-role/roles | Add custom role
[**MultiRoleGetAvailableRoles**](MultiRoleAPI.md#MultiRoleGetAvailableRoles) | **Get** /api/projects/{projectId}/multi-role/roles/available | Get available roles for signup
[**MultiRoleGetConfig**](MultiRoleAPI.md#MultiRoleGetConfig) | **Get** /api/projects/{projectId}/multi-role | Get multi-role feature configuration
[**MultiRoleToggleRole**](MultiRoleAPI.md#MultiRoleToggleRole) | **Patch** /api/projects/{projectId}/multi-role/roles/{roleSlug}/toggle | Toggle role on/off
[**MultiRoleUpdateCollectionPermissions**](MultiRoleAPI.md#MultiRoleUpdateCollectionPermissions) | **Patch** /api/projects/{projectId}/multi-role/roles/{roleSlug}/collections/{collectionId}/permissions | Update collection permissions for a role
[**MultiRoleUpdateRole**](MultiRoleAPI.md#MultiRoleUpdateRole) | **Patch** /api/projects/{projectId}/multi-role/roles/{roleSlug} | Update role configuration
[**MultiRoleUpdateSettings**](MultiRoleAPI.md#MultiRoleUpdateSettings) | **Patch** /api/projects/{projectId}/multi-role/settings | Update multi-role feature settings



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
	role := "vendor" // string | Role slug for signup (e.g. customer, vendor, seller).
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
**role** | **string** | Role slug for signup (e.g. customer, vendor, seller). | 
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
	role := "customer" // string | Role slug for signup (e.g. customer, vendor).
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
**role** | **string** | Role slug for signup (e.g. customer, vendor). | 

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


## MultiRoleAddRole

> MultiRoleUpdateSettings200Response MultiRoleAddRole(ctx, projectId).MultiRoleAddRoleRequest(multiRoleAddRoleRequest).Execute()

Add custom role



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	multiRoleAddRoleRequest := *openapiclient.NewMultiRoleAddRoleRequest("rider", "Delivery Rider", "/api/auth/local/signup/rider") // MultiRoleAddRoleRequest | Custom role definition (slug, name, description, signupEndpoint, hierarchy, defaultPermissions).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleAddRole(context.Background(), projectId).MultiRoleAddRoleRequest(multiRoleAddRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleAddRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleAddRole`: MultiRoleUpdateSettings200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleAddRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleAddRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **multiRoleAddRoleRequest** | [**MultiRoleAddRoleRequest**](MultiRoleAddRoleRequest.md) | Custom role definition (slug, name, description, signupEndpoint, hierarchy, defaultPermissions). | 

### Return type

[**MultiRoleUpdateSettings200Response**](MultiRoleUpdateSettings200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleGetAvailableRoles

> MultiRoleGetAvailableRoles200Response MultiRoleGetAvailableRoles(ctx, projectId).Execute()

Get available roles for signup



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleGetAvailableRoles(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleGetAvailableRoles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleGetAvailableRoles`: MultiRoleGetAvailableRoles200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleGetAvailableRoles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleGetAvailableRolesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**MultiRoleGetAvailableRoles200Response**](MultiRoleGetAvailableRoles200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleGetConfig

> MultiRoleGetConfig200Response MultiRoleGetConfig(ctx, projectId).Execute()

Get multi-role feature configuration



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleGetConfig(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleGetConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleGetConfig`: MultiRoleGetConfig200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleGetConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleGetConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**MultiRoleGetConfig200Response**](MultiRoleGetConfig200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleToggleRole

> MultiRoleUpdateSettings200Response MultiRoleToggleRole(ctx, projectId, roleSlug).MultiRoleToggleRoleRequest(multiRoleToggleRoleRequest).Execute()

Toggle role on/off



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	roleSlug := "vendor" // string | Role slug to toggle (e.g. vendor, customer).
	multiRoleToggleRoleRequest := *openapiclient.NewMultiRoleToggleRoleRequest(true) // MultiRoleToggleRoleRequest | Whether the role is enabled (true) or disabled (false).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleToggleRole(context.Background(), projectId, roleSlug).MultiRoleToggleRoleRequest(multiRoleToggleRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleToggleRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleToggleRole`: MultiRoleUpdateSettings200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleToggleRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug to toggle (e.g. vendor, customer). | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleToggleRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **multiRoleToggleRoleRequest** | [**MultiRoleToggleRoleRequest**](MultiRoleToggleRoleRequest.md) | Whether the role is enabled (true) or disabled (false). | 

### Return type

[**MultiRoleUpdateSettings200Response**](MultiRoleUpdateSettings200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleUpdateCollectionPermissions

> MultiRoleUpdateSettings200Response MultiRoleUpdateCollectionPermissions(ctx, projectId, roleSlug, collectionId).MultiRoleUpdateCollectionPermissionsRequest(multiRoleUpdateCollectionPermissionsRequest).Execute()

Update collection permissions for a role



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	roleSlug := "vendor" // string | Role slug (e.g. vendor, customer).
	collectionId := "696ba6e4f4a9422ac4be4f74" // string | Collection ID to set permissions for.
	multiRoleUpdateCollectionPermissionsRequest := *openapiclient.NewMultiRoleUpdateCollectionPermissionsRequest() // MultiRoleUpdateCollectionPermissionsRequest | Allowed actions and optional conditions for the role on this collection.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleUpdateCollectionPermissions(context.Background(), projectId, roleSlug, collectionId).MultiRoleUpdateCollectionPermissionsRequest(multiRoleUpdateCollectionPermissionsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleUpdateCollectionPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleUpdateCollectionPermissions`: MultiRoleUpdateSettings200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleUpdateCollectionPermissions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug (e.g. vendor, customer). | 
**collectionId** | **string** | Collection ID to set permissions for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleUpdateCollectionPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **multiRoleUpdateCollectionPermissionsRequest** | [**MultiRoleUpdateCollectionPermissionsRequest**](MultiRoleUpdateCollectionPermissionsRequest.md) | Allowed actions and optional conditions for the role on this collection. | 

### Return type

[**MultiRoleUpdateSettings200Response**](MultiRoleUpdateSettings200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleUpdateRole

> MultiRoleUpdateSettings200Response MultiRoleUpdateRole(ctx, projectId, roleSlug).MultiRoleUpdateRoleRequest(multiRoleUpdateRoleRequest).Execute()

Update role configuration



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	roleSlug := "vendor" // string | Role slug to update (e.g. vendor, customer).
	multiRoleUpdateRoleRequest := *openapiclient.NewMultiRoleUpdateRoleRequest() // MultiRoleUpdateRoleRequest | Role fields to update (name, description, hierarchy, requiresApproval, requiresPayment, requiresKYC).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleUpdateRole(context.Background(), projectId, roleSlug).MultiRoleUpdateRoleRequest(multiRoleUpdateRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleUpdateRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleUpdateRole`: MultiRoleUpdateSettings200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleUpdateRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug to update (e.g. vendor, customer). | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleUpdateRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **multiRoleUpdateRoleRequest** | [**MultiRoleUpdateRoleRequest**](MultiRoleUpdateRoleRequest.md) | Role fields to update (name, description, hierarchy, requiresApproval, requiresPayment, requiresKYC). | 

### Return type

[**MultiRoleUpdateSettings200Response**](MultiRoleUpdateSettings200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleUpdateSettings

> MultiRoleUpdateSettings200Response MultiRoleUpdateSettings(ctx, projectId).MultiRoleUpdateSettingsRequest(multiRoleUpdateSettingsRequest).Execute()

Update multi-role feature settings



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID.
	multiRoleUpdateSettingsRequest := *openapiclient.NewMultiRoleUpdateSettingsRequest() // MultiRoleUpdateSettingsRequest | Multi-role settings (e.g. isEnabled, defaultRole, allowMultipleRoles, requireApproval).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleUpdateSettings(context.Background(), projectId).MultiRoleUpdateSettingsRequest(multiRoleUpdateSettingsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleUpdateSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleUpdateSettings`: MultiRoleUpdateSettings200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleUpdateSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleUpdateSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **multiRoleUpdateSettingsRequest** | [**MultiRoleUpdateSettingsRequest**](MultiRoleUpdateSettingsRequest.md) | Multi-role settings (e.g. isEnabled, defaultRole, allowMultipleRoles, requireApproval). | 

### Return type

[**MultiRoleUpdateSettings200Response**](MultiRoleUpdateSettings200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


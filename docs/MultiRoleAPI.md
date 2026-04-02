# \MultiRoleAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthOauthSignupWithRole**](MultiRoleAPI.md#AuthOauthSignupWithRole) | **Get** /api/auth/oauth/signup/{role}/{provider}/{projectId} | OAuth signup with specific role
[**AuthRegisterWithRole**](MultiRoleAPI.md#AuthRegisterWithRole) | **Post** /api/auth/local/signup/{role} | Register user with specific role (Local Auth)
[**MultiRoleAddRole**](MultiRoleAPI.md#MultiRoleAddRole) | **Post** /api/projects/{projectId}/multi-role/roles | Add custom role
[**MultiRoleApplyRoleFeaturePreset**](MultiRoleAPI.md#MultiRoleApplyRoleFeaturePreset) | **Post** /api/projects/{projectId}/multi-role/roles/{roleSlug}/apply-preset | Apply Admin / User / Viewer feature permission preset
[**MultiRoleGetAvailableRoles**](MultiRoleAPI.md#MultiRoleGetAvailableRoles) | **Get** /api/projects/{projectId}/multi-role/roles/available | Get available roles for signup
[**MultiRoleGetConfig**](MultiRoleAPI.md#MultiRoleGetConfig) | **Get** /api/projects/{projectId}/multi-role | Get multi-role feature configuration
[**MultiRoleGetPermissionsMatrix**](MultiRoleAPI.md#MultiRoleGetPermissionsMatrix) | **Get** /api/projects/{projectId}/permissions-matrix | Get permissions matrix (collections + featurePermissions)
[**MultiRoleSimulateAppPermissions**](MultiRoleAPI.md#MultiRoleSimulateAppPermissions) | **Post** /api/projects/{projectId}/multi-role/simulate-permissions | Simulate app-role feature permission for a path
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


## MultiRoleAddRole

> MultiRoleToggleRole200Response MultiRoleAddRole(ctx, projectId).MultiRoleAddRoleRequest(multiRoleAddRoleRequest).Execute()

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
	multiRoleAddRoleRequest := *openapiclient.NewMultiRoleAddRoleRequest("seller", "Seller", "seller") // MultiRoleAddRoleRequest | Custom role definition. Use `collectionPermissions` to apply CRUD per collection slug (e.g. users/products/orders). `defaultPermissions` is optional for global/base permissions.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleAddRole(context.Background(), projectId).MultiRoleAddRoleRequest(multiRoleAddRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleAddRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleAddRole`: MultiRoleToggleRole200Response
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

 **multiRoleAddRoleRequest** | [**MultiRoleAddRoleRequest**](MultiRoleAddRoleRequest.md) | Custom role definition. Use &#x60;collectionPermissions&#x60; to apply CRUD per collection slug (e.g. users/products/orders). &#x60;defaultPermissions&#x60; is optional for global/base permissions. | 

### Return type

[**MultiRoleToggleRole200Response**](MultiRoleToggleRole200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleApplyRoleFeaturePreset

> MultiRoleApplyRoleFeaturePreset(ctx, projectId, roleSlug).MultiRoleApplyRoleFeaturePresetRequest(multiRoleApplyRoleFeaturePresetRequest).Execute()

Apply Admin / User / Viewer feature permission preset



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
	projectId := "projectId_example" // string | Project ID.
	roleSlug := "roleSlug_example" // string | Role slug to apply the preset to (e.g. `customer`).
	multiRoleApplyRoleFeaturePresetRequest := *openapiclient.NewMultiRoleApplyRoleFeaturePresetRequest("Preset_example") // MultiRoleApplyRoleFeaturePresetRequest | JSON body with `preset` set to `admin`, `user`, or `viewer`.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MultiRoleAPI.MultiRoleApplyRoleFeaturePreset(context.Background(), projectId, roleSlug).MultiRoleApplyRoleFeaturePresetRequest(multiRoleApplyRoleFeaturePresetRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleApplyRoleFeaturePreset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug to apply the preset to (e.g. &#x60;customer&#x60;). | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleApplyRoleFeaturePresetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **multiRoleApplyRoleFeaturePresetRequest** | [**MultiRoleApplyRoleFeaturePresetRequest**](MultiRoleApplyRoleFeaturePresetRequest.md) | JSON body with &#x60;preset&#x60; set to &#x60;admin&#x60;, &#x60;user&#x60;, or &#x60;viewer&#x60;. | 

### Return type

 (empty response body)

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


## MultiRoleGetPermissionsMatrix

> MultiRoleGetPermissionsMatrix200Response MultiRoleGetPermissionsMatrix(ctx, projectId).Execute()

Get permissions matrix (collections + featurePermissions)



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID whose multi-role matrix is returned.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleGetPermissionsMatrix(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleGetPermissionsMatrix``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleGetPermissionsMatrix`: MultiRoleGetPermissionsMatrix200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleGetPermissionsMatrix`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID whose multi-role matrix is returned. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleGetPermissionsMatrixRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**MultiRoleGetPermissionsMatrix200Response**](MultiRoleGetPermissionsMatrix200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleSimulateAppPermissions

> map[string]interface{} MultiRoleSimulateAppPermissions(ctx, projectId).MultiRoleSimulateAppPermissionsRequest(multiRoleSimulateAppPermissionsRequest).Execute()

Simulate app-role feature permission for a path



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
	projectId := "projectId_example" // string | Project ID used to resolve role configuration.
	multiRoleSimulateAppPermissionsRequest := *openapiclient.NewMultiRoleSimulateAppPermissionsRequest("Role_example") // MultiRoleSimulateAppPermissionsRequest | Role slug plus either OpenAPI `operationId` or HTTP `method` and `pathname` to evaluate.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleSimulateAppPermissions(context.Background(), projectId).MultiRoleSimulateAppPermissionsRequest(multiRoleSimulateAppPermissionsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleSimulateAppPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleSimulateAppPermissions`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleSimulateAppPermissions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID used to resolve role configuration. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleSimulateAppPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **multiRoleSimulateAppPermissionsRequest** | [**MultiRoleSimulateAppPermissionsRequest**](MultiRoleSimulateAppPermissionsRequest.md) | Role slug plus either OpenAPI &#x60;operationId&#x60; or HTTP &#x60;method&#x60; and &#x60;pathname&#x60; to evaluate. | 

### Return type

**map[string]interface{}**

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleToggleRole

> MultiRoleToggleRole200Response MultiRoleToggleRole(ctx, projectId, roleSlug).MultiRoleToggleRoleRequest(multiRoleToggleRoleRequest).Execute()

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
	roleSlug := "customer" // string | Role slug to toggle (e.g. starter `customer` or a role you added).
	multiRoleToggleRoleRequest := *openapiclient.NewMultiRoleToggleRoleRequest(true) // MultiRoleToggleRoleRequest | Whether the role is enabled (true) or disabled (false).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleToggleRole(context.Background(), projectId, roleSlug).MultiRoleToggleRoleRequest(multiRoleToggleRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleToggleRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleToggleRole`: MultiRoleToggleRole200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleToggleRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug to toggle (e.g. starter &#x60;customer&#x60; or a role you added). | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleToggleRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **multiRoleToggleRoleRequest** | [**MultiRoleToggleRoleRequest**](MultiRoleToggleRoleRequest.md) | Whether the role is enabled (true) or disabled (false). | 

### Return type

[**MultiRoleToggleRole200Response**](MultiRoleToggleRole200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleUpdateCollectionPermissions

> MultiRoleToggleRole200Response MultiRoleUpdateCollectionPermissions(ctx, projectId, roleSlug, collectionId).MultiRoleUpdateCollectionPermissionsRequest(multiRoleUpdateCollectionPermissionsRequest).Execute()

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
	roleSlug := "customer" // string | Role slug (e.g. starter `customer` or a role you added).
	collectionId := "696ba6e4f4a9422ac4be4f74" // string | Collection ID to set permissions for.
	multiRoleUpdateCollectionPermissionsRequest := *openapiclient.NewMultiRoleUpdateCollectionPermissionsRequest() // MultiRoleUpdateCollectionPermissionsRequest | Allowed actions and optional conditions for the role on this collection.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleUpdateCollectionPermissions(context.Background(), projectId, roleSlug, collectionId).MultiRoleUpdateCollectionPermissionsRequest(multiRoleUpdateCollectionPermissionsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleUpdateCollectionPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleUpdateCollectionPermissions`: MultiRoleToggleRole200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleUpdateCollectionPermissions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug (e.g. starter &#x60;customer&#x60; or a role you added). | 
**collectionId** | **string** | Collection ID to set permissions for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleUpdateCollectionPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **multiRoleUpdateCollectionPermissionsRequest** | [**MultiRoleUpdateCollectionPermissionsRequest**](MultiRoleUpdateCollectionPermissionsRequest.md) | Allowed actions and optional conditions for the role on this collection. | 

### Return type

[**MultiRoleToggleRole200Response**](MultiRoleToggleRole200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MultiRoleUpdateRole

> MultiRoleToggleRole200Response MultiRoleUpdateRole(ctx, projectId, roleSlug).MultiRoleUpdateRoleRequest(multiRoleUpdateRoleRequest).Execute()

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
	roleSlug := "customer" // string | Role slug to update (e.g. starter `customer` or a role you added).
	multiRoleUpdateRoleRequest := *openapiclient.NewMultiRoleUpdateRoleRequest() // MultiRoleUpdateRoleRequest | Same fields as **Add custom role** — send only fields you want to change. `defaultPermissions` / `collectionPermissions` are normalized the same way as on create.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MultiRoleAPI.MultiRoleUpdateRole(context.Background(), projectId, roleSlug).MultiRoleUpdateRoleRequest(multiRoleUpdateRoleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MultiRoleAPI.MultiRoleUpdateRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MultiRoleUpdateRole`: MultiRoleToggleRole200Response
	fmt.Fprintf(os.Stdout, "Response from `MultiRoleAPI.MultiRoleUpdateRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**roleSlug** | **string** | Role slug to update (e.g. starter &#x60;customer&#x60; or a role you added). | 

### Other Parameters

Other parameters are passed through a pointer to a apiMultiRoleUpdateRoleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **multiRoleUpdateRoleRequest** | [**MultiRoleUpdateRoleRequest**](MultiRoleUpdateRoleRequest.md) | Same fields as **Add custom role** — send only fields you want to change. &#x60;defaultPermissions&#x60; / &#x60;collectionPermissions&#x60; are normalized the same way as on create. | 

### Return type

[**MultiRoleToggleRole200Response**](MultiRoleToggleRole200Response.md)

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
	multiRoleUpdateSettingsRequest := *openapiclient.NewMultiRoleUpdateSettingsRequest() // MultiRoleUpdateSettingsRequest | Feature flags only — not per-role approval. Use `settings.allowMultipleRoles`, `requireRoleSelection`, `autoAssignDefault`, `dataOwnerField`.

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

 **multiRoleUpdateSettingsRequest** | [**MultiRoleUpdateSettingsRequest**](MultiRoleUpdateSettingsRequest.md) | Feature flags only — not per-role approval. Use &#x60;settings.allowMultipleRoles&#x60;, &#x60;requireRoleSelection&#x60;, &#x60;autoAssignDefault&#x60;, &#x60;dataOwnerField&#x60;. | 

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


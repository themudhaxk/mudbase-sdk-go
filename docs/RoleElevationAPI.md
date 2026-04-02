# \RoleElevationAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RoleElevationGetStatus**](RoleElevationAPI.md#RoleElevationGetStatus) | **Get** /api/projects/{projectId}/role-elevation/status | Get role elevation status
[**RoleElevationRequest**](RoleElevationAPI.md#RoleElevationRequest) | **Post** /api/projects/{projectId}/role-elevation/request | Request role elevation
[**RoleElevationUploadDocuments**](RoleElevationAPI.md#RoleElevationUploadDocuments) | **Post** /api/projects/{projectId}/role-elevation/documents | Upload verification documents



## RoleElevationGetStatus

> RoleElevationGetStatus200Response RoleElevationGetStatus(ctx, projectId).RoleSlug(roleSlug).Execute()

Get role elevation status



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
	roleSlug := "roleSlug_example" // string | Optional filter by role slug. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoleElevationAPI.RoleElevationGetStatus(context.Background(), projectId).RoleSlug(roleSlug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoleElevationAPI.RoleElevationGetStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RoleElevationGetStatus`: RoleElevationGetStatus200Response
	fmt.Fprintf(os.Stdout, "Response from `RoleElevationAPI.RoleElevationGetStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRoleElevationGetStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **roleSlug** | **string** | Optional filter by role slug. | 

### Return type

[**RoleElevationGetStatus200Response**](RoleElevationGetStatus200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RoleElevationRequest

> RoleElevationRequest200Response RoleElevationRequest(ctx, projectId).RoleElevationRequestRequest(roleElevationRequestRequest).Execute()

Request role elevation



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
	roleElevationRequestRequest := *openapiclient.NewRoleElevationRequestRequest("seller") // RoleElevationRequestRequest | Role slug to request elevation to (e.g. a higher-privilege role you configured).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoleElevationAPI.RoleElevationRequest(context.Background(), projectId).RoleElevationRequestRequest(roleElevationRequestRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoleElevationAPI.RoleElevationRequest``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RoleElevationRequest`: RoleElevationRequest200Response
	fmt.Fprintf(os.Stdout, "Response from `RoleElevationAPI.RoleElevationRequest`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRoleElevationRequestRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **roleElevationRequestRequest** | [**RoleElevationRequestRequest**](RoleElevationRequestRequest.md) | Role slug to request elevation to (e.g. a higher-privilege role you configured). | 

### Return type

[**RoleElevationRequest200Response**](RoleElevationRequest200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RoleElevationUploadDocuments

> RoleElevationUploadDocuments(ctx, projectId).RoleElevationUploadDocumentsRequest(roleElevationUploadDocumentsRequest).Execute()

Upload verification documents



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
	roleElevationUploadDocumentsRequest := *openapiclient.NewRoleElevationUploadDocumentsRequest("RoleSlug_example", []openapiclient.RoleElevationUploadDocumentsRequestDocumentsInner{*openapiclient.NewRoleElevationUploadDocumentsRequestDocumentsInner()}) // RoleElevationUploadDocumentsRequest | Role slug and array of document objects (type, url).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RoleElevationAPI.RoleElevationUploadDocuments(context.Background(), projectId).RoleElevationUploadDocumentsRequest(roleElevationUploadDocumentsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoleElevationAPI.RoleElevationUploadDocuments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRoleElevationUploadDocumentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **roleElevationUploadDocumentsRequest** | [**RoleElevationUploadDocumentsRequest**](RoleElevationUploadDocumentsRequest.md) | Role slug and array of document objects (type, url). | 

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


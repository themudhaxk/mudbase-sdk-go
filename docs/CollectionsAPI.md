# \CollectionsAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CollectionsCreate**](CollectionsAPI.md#CollectionsCreate) | **Post** /api/schemas/projects/{projectId}/collections | Create new collection
[**CollectionsDelete**](CollectionsAPI.md#CollectionsDelete) | **Delete** /api/schemas/projects/{projectId}/collections/{collectionId} | Delete collection
[**CollectionsGet**](CollectionsAPI.md#CollectionsGet) | **Get** /api/schemas/projects/{projectId}/collections/{collectionId} | Get single collection
[**CollectionsList**](CollectionsAPI.md#CollectionsList) | **Get** /api/schemas/projects/{projectId}/collections | List collections in project
[**CollectionsUpdate**](CollectionsAPI.md#CollectionsUpdate) | **Patch** /api/schemas/projects/{projectId}/collections/{collectionId} | Update collection



## CollectionsCreate

> CollectionsCreate201Response CollectionsCreate(ctx, projectId).CreateCollectionRequest(createCollectionRequest).Execute()

Create new collection



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
	createCollectionRequest := *openapiclient.NewCreateCollectionRequest("Name_example", []openapiclient.Field{*openapiclient.NewField("Name_example", "Type_example")}) // CreateCollectionRequest | Collection name, optional slug, fields, permissions, and settings.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CollectionsAPI.CollectionsCreate(context.Background(), projectId).CreateCollectionRequest(createCollectionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CollectionsAPI.CollectionsCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CollectionsCreate`: CollectionsCreate201Response
	fmt.Fprintf(os.Stdout, "Response from `CollectionsAPI.CollectionsCreate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCollectionsCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createCollectionRequest** | [**CreateCollectionRequest**](CreateCollectionRequest.md) | Collection name, optional slug, fields, permissions, and settings. | 

### Return type

[**CollectionsCreate201Response**](CollectionsCreate201Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CollectionsDelete

> MessageResponse CollectionsDelete(ctx, projectId, collectionId).Execute()

Delete collection



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
	collectionId := "collectionId_example" // string | Collection ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CollectionsAPI.CollectionsDelete(context.Background(), projectId, collectionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CollectionsAPI.CollectionsDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CollectionsDelete`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `CollectionsAPI.CollectionsDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCollectionsDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



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


## CollectionsGet

> Collection CollectionsGet(ctx, projectId, collectionId).Execute()

Get single collection



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
	collectionId := "collectionId_example" // string | Collection ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CollectionsAPI.CollectionsGet(context.Background(), projectId, collectionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CollectionsAPI.CollectionsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CollectionsGet`: Collection
	fmt.Fprintf(os.Stdout, "Response from `CollectionsAPI.CollectionsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCollectionsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Collection**](Collection.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CollectionsList

> CollectionsList200Response CollectionsList(ctx, projectId).Execute()

List collections in project



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CollectionsAPI.CollectionsList(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CollectionsAPI.CollectionsList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CollectionsList`: CollectionsList200Response
	fmt.Fprintf(os.Stdout, "Response from `CollectionsAPI.CollectionsList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCollectionsListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CollectionsList200Response**](CollectionsList200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CollectionsUpdate

> CollectionsCreate201Response CollectionsUpdate(ctx, projectId, collectionId).UpdateCollectionRequest(updateCollectionRequest).Execute()

Update collection



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
	collectionId := "collectionId_example" // string | Collection ID.
	updateCollectionRequest := *openapiclient.NewUpdateCollectionRequest() // UpdateCollectionRequest | Fields to update (name, fields, permissions, settings).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CollectionsAPI.CollectionsUpdate(context.Background(), projectId, collectionId).UpdateCollectionRequest(updateCollectionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CollectionsAPI.CollectionsUpdate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CollectionsUpdate`: CollectionsCreate201Response
	fmt.Fprintf(os.Stdout, "Response from `CollectionsAPI.CollectionsUpdate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCollectionsUpdateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateCollectionRequest** | [**UpdateCollectionRequest**](UpdateCollectionRequest.md) | Fields to update (name, fields, permissions, settings). | 

### Return type

[**CollectionsCreate201Response**](CollectionsCreate201Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


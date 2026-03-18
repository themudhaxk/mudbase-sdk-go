# \DataAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DataCreate**](DataAPI.md#DataCreate) | **Post** /api/data/projects/{projectId}/collections/{collectionId}/data | Create data in collection
[**DataDelete**](DataAPI.md#DataDelete) | **Delete** /api/data/projects/{projectId}/collections/{collectionId}/data/{documentId} | Delete document
[**DataGet**](DataAPI.md#DataGet) | **Get** /api/data/projects/{projectId}/collections/{collectionId}/data/{documentId} | Get single document
[**DataList**](DataAPI.md#DataList) | **Get** /api/data/projects/{projectId}/collections/{collectionId}/data | List data in collection
[**DataUpdate**](DataAPI.md#DataUpdate) | **Patch** /api/data/projects/{projectId}/collections/{collectionId}/data/{documentId} | Update document



## DataCreate

> DataResponse DataCreate(ctx, projectId, collectionId).Body(body).Execute()

Create data in collection



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
	body := map[string]interface{}{ ... } // map[string]interface{} | Document fields matching the collection schema.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DataAPI.DataCreate(context.Background(), projectId, collectionId).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DataAPI.DataCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DataCreate`: DataResponse
	fmt.Fprintf(os.Stdout, "Response from `DataAPI.DataCreate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDataCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **map[string]interface{}** | Document fields matching the collection schema. | 

### Return type

[**DataResponse**](DataResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DataDelete

> MessageResponse DataDelete(ctx, projectId, collectionId, documentId).Execute()

Delete document



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
	documentId := "documentId_example" // string | Document ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DataAPI.DataDelete(context.Background(), projectId, collectionId, documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DataAPI.DataDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DataDelete`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `DataAPI.DataDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 
**documentId** | **string** | Document ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDataDeleteRequest struct via the builder pattern


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


## DataGet

> DataResponse DataGet(ctx, projectId, collectionId, documentId).Execute()

Get single document



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
	documentId := "documentId_example" // string | Document ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DataAPI.DataGet(context.Background(), projectId, collectionId, documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DataAPI.DataGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DataGet`: DataResponse
	fmt.Fprintf(os.Stdout, "Response from `DataAPI.DataGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 
**documentId** | **string** | Document ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDataGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**DataResponse**](DataResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DataList

> DataListResponse DataList(ctx, projectId, collectionId).Page(page).Limit(limit).Sort(sort).Filter(filter).Execute()

List data in collection



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
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Number of documents per page. (optional) (default to 20)
	sort := "sort_example" // string | Sort field and order (e.g. -createdAt, name). (optional) (default to "-createdAt")
	filter := "filter_example" // string | JSON string for filtering documents (e.g. {\"status\":\"active\"}). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DataAPI.DataList(context.Background(), projectId, collectionId).Page(page).Limit(limit).Sort(sort).Filter(filter).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DataAPI.DataList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DataList`: DataListResponse
	fmt.Fprintf(os.Stdout, "Response from `DataAPI.DataList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDataListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of documents per page. | [default to 20]
 **sort** | **string** | Sort field and order (e.g. -createdAt, name). | [default to &quot;-createdAt&quot;]
 **filter** | **string** | JSON string for filtering documents (e.g. {\&quot;status\&quot;:\&quot;active\&quot;}). | 

### Return type

[**DataListResponse**](DataListResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DataUpdate

> DataResponse DataUpdate(ctx, projectId, collectionId, documentId).Body(body).Execute()

Update document



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
	documentId := "documentId_example" // string | Document ID.
	body := map[string]interface{}{ ... } // map[string]interface{} | Partial document fields to update.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DataAPI.DataUpdate(context.Background(), projectId, collectionId, documentId).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DataAPI.DataUpdate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DataUpdate`: DataResponse
	fmt.Fprintf(os.Stdout, "Response from `DataAPI.DataUpdate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**collectionId** | **string** | Collection ID. | 
**documentId** | **string** | Document ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDataUpdateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | **map[string]interface{}** | Partial document fields to update. | 

### Return type

[**DataResponse**](DataResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


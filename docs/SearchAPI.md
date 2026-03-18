# \SearchAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SearchGetAnalytics**](SearchAPI.md#SearchGetAnalytics) | **Get** /api/search/projects/{projectId}/search/analytics | Get search analytics
[**SearchGetSuggestions**](SearchAPI.md#SearchGetSuggestions) | **Get** /api/search/projects/{projectId}/search/suggestions | Get search suggestions
[**SearchSearch**](SearchAPI.md#SearchSearch) | **Get** /api/search/projects/{projectId}/search | Full-text search



## SearchGetAnalytics

> SearchGetAnalytics200Response SearchGetAnalytics(ctx, projectId).Timeframe(timeframe).Execute()

Get search analytics



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID (MongoDB ObjectId) to get analytics for.
	timeframe := "timeframe_example" // string | Timeframe for analytics (1d, 7d, or 30d). (optional) (default to "7d")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.SearchGetAnalytics(context.Background(), projectId).Timeframe(timeframe).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.SearchGetAnalytics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchGetAnalytics`: SearchGetAnalytics200Response
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.SearchGetAnalytics`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to get analytics for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchGetAnalyticsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **timeframe** | **string** | Timeframe for analytics (1d, 7d, or 30d). | [default to &quot;7d&quot;]

### Return type

[**SearchGetAnalytics200Response**](SearchGetAnalytics200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchGetSuggestions

> SearchGetSuggestions200Response SearchGetSuggestions(ctx, projectId).Q(q).Limit(limit).Execute()

Get search suggestions



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID (MongoDB ObjectId) to get suggestions for.
	q := "q_example" // string | Partial search query (min 2 characters, max 50); suggestions are based on past queries and indexed content.
	limit := int32(56) // int32 | Maximum number of suggestions to return (1–20). (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.SearchGetSuggestions(context.Background(), projectId).Q(q).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.SearchGetSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchGetSuggestions`: SearchGetSuggestions200Response
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.SearchGetSuggestions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to get suggestions for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchGetSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **q** | **string** | Partial search query (min 2 characters, max 50); suggestions are based on past queries and indexed content. | 
 **limit** | **int32** | Maximum number of suggestions to return (1–20). | [default to 10]

### Return type

[**SearchGetSuggestions200Response**](SearchGetSuggestions200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchSearch

> SearchResponse SearchSearch(ctx, projectId).Q(q).Collections(collections).Fields(fields).Limit(limit).Page(page).Execute()

Full-text search



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) to search within.
	q := "q_example" // string | Full-text search query string.
	collections := "collections_example" // string | Comma-separated collection slugs or IDs to limit search scope. (optional)
	fields := "fields_example" // string | Comma-separated field names to search or return in highlights. (optional)
	limit := int32(56) // int32 | Maximum number of results to return per page. (optional) (default to 20)
	page := int32(56) // int32 | Page number for pagination (1-based). (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.SearchSearch(context.Background(), projectId).Q(q).Collections(collections).Fields(fields).Limit(limit).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.SearchSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchSearch`: SearchResponse
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.SearchSearch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to search within. | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **q** | **string** | Full-text search query string. | 
 **collections** | **string** | Comma-separated collection slugs or IDs to limit search scope. | 
 **fields** | **string** | Comma-separated field names to search or return in highlights. | 
 **limit** | **int32** | Maximum number of results to return per page. | [default to 20]
 **page** | **int32** | Page number for pagination (1-based). | [default to 1]

### Return type

[**SearchResponse**](SearchResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


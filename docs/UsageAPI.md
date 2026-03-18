# \UsageAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**UsageGetProject**](UsageAPI.md#UsageGetProject) | **Get** /api/usage/projects/{projectId} | Get project usage
[**UsageGetTrends**](UsageAPI.md#UsageGetTrends) | **Get** /api/usage/trends | Get usage trends



## UsageGetProject

> ProjectUsageStatsResponse UsageGetProject(ctx, projectId).Period(period).Execute()

Get project usage



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) to get usage for.
	period := "period_example" // string | Aggregation period for usage (day, week, or month). (optional) (default to "month")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsageAPI.UsageGetProject(context.Background(), projectId).Period(period).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsageAPI.UsageGetProject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsageGetProject`: ProjectUsageStatsResponse
	fmt.Fprintf(os.Stdout, "Response from `UsageAPI.UsageGetProject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to get usage for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUsageGetProjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **period** | **string** | Aggregation period for usage (day, week, or month). | [default to &quot;month&quot;]

### Return type

[**ProjectUsageStatsResponse**](ProjectUsageStatsResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UsageGetTrends

> UsageTrendsResponse UsageGetTrends(ctx).Days(days).Execute()

Get usage trends



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
	days := int32(56) // int32 | Number of days of trend data to return (default 30). (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsageAPI.UsageGetTrends(context.Background()).Days(days).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsageAPI.UsageGetTrends``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UsageGetTrends`: UsageTrendsResponse
	fmt.Fprintf(os.Stdout, "Response from `UsageAPI.UsageGetTrends`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUsageGetTrendsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **days** | **int32** | Number of days of trend data to return (default 30). | [default to 30]

### Return type

[**UsageTrendsResponse**](UsageTrendsResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


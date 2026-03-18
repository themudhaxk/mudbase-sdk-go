# \RealtimeAnalyticsAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RealtimeAnalyticsCheckUserPresence**](RealtimeAnalyticsAPI.md#RealtimeAnalyticsCheckUserPresence) | **Post** /api/realtime/projects/{projectId}/presence | Check presence status for users
[**RealtimeAnalyticsGetActiveUsers**](RealtimeAnalyticsAPI.md#RealtimeAnalyticsGetActiveUsers) | **Get** /api/realtime/projects/{projectId}/active-users | Get active users for a project
[**RealtimeAnalyticsGetEventThroughput**](RealtimeAnalyticsAPI.md#RealtimeAnalyticsGetEventThroughput) | **Get** /api/realtime/projects/{projectId}/throughput | Get event throughput metrics
[**RealtimeAnalyticsGetHistoricalAnalytics**](RealtimeAnalyticsAPI.md#RealtimeAnalyticsGetHistoricalAnalytics) | **Get** /api/realtime/projects/{projectId}/history | Get historical analytics
[**RealtimeAnalyticsGetProject**](RealtimeAnalyticsAPI.md#RealtimeAnalyticsGetProject) | **Get** /api/realtime/projects/{projectId}/analytics | Get project real-time analytics



## RealtimeAnalyticsCheckUserPresence

> RealtimeAnalyticsCheckUserPresence200Response RealtimeAnalyticsCheckUserPresence(ctx, projectId).RealtimeAnalyticsCheckUserPresenceRequest(realtimeAnalyticsCheckUserPresenceRequest).Execute()

Check presence status for users



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
	realtimeAnalyticsCheckUserPresenceRequest := *openapiclient.NewRealtimeAnalyticsCheckUserPresenceRequest([]string{"UserIds_example"}) // RealtimeAnalyticsCheckUserPresenceRequest | Array of user IDs to check presence for.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtimeAnalyticsAPI.RealtimeAnalyticsCheckUserPresence(context.Background(), projectId).RealtimeAnalyticsCheckUserPresenceRequest(realtimeAnalyticsCheckUserPresenceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAnalyticsAPI.RealtimeAnalyticsCheckUserPresence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtimeAnalyticsCheckUserPresence`: RealtimeAnalyticsCheckUserPresence200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAnalyticsAPI.RealtimeAnalyticsCheckUserPresence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtimeAnalyticsCheckUserPresenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **realtimeAnalyticsCheckUserPresenceRequest** | [**RealtimeAnalyticsCheckUserPresenceRequest**](RealtimeAnalyticsCheckUserPresenceRequest.md) | Array of user IDs to check presence for. | 

### Return type

[**RealtimeAnalyticsCheckUserPresence200Response**](RealtimeAnalyticsCheckUserPresence200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RealtimeAnalyticsGetActiveUsers

> RealtimeAnalyticsGetActiveUsers200Response RealtimeAnalyticsGetActiveUsers(ctx, projectId).Execute()

Get active users for a project



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
	resp, r, err := apiClient.RealtimeAnalyticsAPI.RealtimeAnalyticsGetActiveUsers(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAnalyticsAPI.RealtimeAnalyticsGetActiveUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtimeAnalyticsGetActiveUsers`: RealtimeAnalyticsGetActiveUsers200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAnalyticsAPI.RealtimeAnalyticsGetActiveUsers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtimeAnalyticsGetActiveUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RealtimeAnalyticsGetActiveUsers200Response**](RealtimeAnalyticsGetActiveUsers200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RealtimeAnalyticsGetEventThroughput

> RealtimeAnalyticsGetEventThroughput200Response RealtimeAnalyticsGetEventThroughput(ctx, projectId).Window(window).Execute()

Get event throughput metrics



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
	window := int32(56) // int32 | Time window in milliseconds (optional) (default to 60000)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtimeAnalyticsAPI.RealtimeAnalyticsGetEventThroughput(context.Background(), projectId).Window(window).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAnalyticsAPI.RealtimeAnalyticsGetEventThroughput``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtimeAnalyticsGetEventThroughput`: RealtimeAnalyticsGetEventThroughput200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAnalyticsAPI.RealtimeAnalyticsGetEventThroughput`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtimeAnalyticsGetEventThroughputRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **window** | **int32** | Time window in milliseconds | [default to 60000]

### Return type

[**RealtimeAnalyticsGetEventThroughput200Response**](RealtimeAnalyticsGetEventThroughput200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RealtimeAnalyticsGetHistoricalAnalytics

> RealtimeAnalyticsGetHistoricalAnalytics200Response RealtimeAnalyticsGetHistoricalAnalytics(ctx, projectId).Period(period).Execute()

Get historical analytics



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
	period := "period_example" // string | Time period for historical data (optional) (default to "hour")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtimeAnalyticsAPI.RealtimeAnalyticsGetHistoricalAnalytics(context.Background(), projectId).Period(period).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAnalyticsAPI.RealtimeAnalyticsGetHistoricalAnalytics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtimeAnalyticsGetHistoricalAnalytics`: RealtimeAnalyticsGetHistoricalAnalytics200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAnalyticsAPI.RealtimeAnalyticsGetHistoricalAnalytics`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtimeAnalyticsGetHistoricalAnalyticsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **period** | **string** | Time period for historical data | [default to &quot;hour&quot;]

### Return type

[**RealtimeAnalyticsGetHistoricalAnalytics200Response**](RealtimeAnalyticsGetHistoricalAnalytics200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RealtimeAnalyticsGetProject

> RealtimeAnalyticsGetProject200Response RealtimeAnalyticsGetProject(ctx, projectId).Execute()

Get project real-time analytics



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
	projectId := "685ad30be129932fbb7a1047" // string | Project ID (MongoDB ObjectId) to get real-time analytics for.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtimeAnalyticsAPI.RealtimeAnalyticsGetProject(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAnalyticsAPI.RealtimeAnalyticsGetProject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtimeAnalyticsGetProject`: RealtimeAnalyticsGetProject200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAnalyticsAPI.RealtimeAnalyticsGetProject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to get real-time analytics for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtimeAnalyticsGetProjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RealtimeAnalyticsGetProject200Response**](RealtimeAnalyticsGetProject200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


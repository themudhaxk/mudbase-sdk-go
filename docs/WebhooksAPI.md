# \WebhooksAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WebhooksGetStats**](WebhooksAPI.md#WebhooksGetStats) | **Get** /api/webhooks/stats | Get webhook statistics



## WebhooksGetStats

> WebhookStatsResponse WebhooksGetStats(ctx).ProjectId(projectId).Days(days).Execute()

Get webhook statistics



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
	projectId := "projectId_example" // string | Project ID to filter stats (optional). (optional)
	days := int32(56) // int32 | Number of days to include in the stats window. (optional) (default to 7)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.WebhooksGetStats(context.Background()).ProjectId(projectId).Days(days).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.WebhooksGetStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WebhooksGetStats`: WebhookStatsResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.WebhooksGetStats`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWebhooksGetStatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **projectId** | **string** | Project ID to filter stats (optional). | 
 **days** | **int32** | Number of days to include in the stats window. | [default to 7]

### Return type

[**WebhookStatsResponse**](WebhookStatsResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


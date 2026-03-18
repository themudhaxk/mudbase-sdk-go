# \IntegrationsAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**IntegrationsExecute**](IntegrationsAPI.md#IntegrationsExecute) | **Post** /api/integrations/projects/{projectId}/integrations/{integrationId}/execute | Execute integration
[**IntegrationsList**](IntegrationsAPI.md#IntegrationsList) | **Get** /api/integrations/projects/{projectId}/integrations | Get project integrations



## IntegrationsExecute

> WalletTestWebhook200Response IntegrationsExecute(ctx, projectId, integrationId).IntegrationsExecuteRequest(integrationsExecuteRequest).Execute()

Execute integration



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
	integrationId := "integrationId_example" // string | Integration ID to execute.
	integrationsExecuteRequest := *openapiclient.NewIntegrationsExecuteRequest("Endpoint_example", "Method_example") // IntegrationsExecuteRequest | Endpoint path, HTTP method, optional params and body for the integration call.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.IntegrationsExecute(context.Background(), projectId, integrationId).IntegrationsExecuteRequest(integrationsExecuteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.IntegrationsExecute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IntegrationsExecute`: WalletTestWebhook200Response
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.IntegrationsExecute`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**integrationId** | **string** | Integration ID to execute. | 

### Other Parameters

Other parameters are passed through a pointer to a apiIntegrationsExecuteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **integrationsExecuteRequest** | [**IntegrationsExecuteRequest**](IntegrationsExecuteRequest.md) | Endpoint path, HTTP method, optional params and body for the integration call. | 

### Return type

[**WalletTestWebhook200Response**](WalletTestWebhook200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## IntegrationsList

> IntegrationsList200Response IntegrationsList(ctx, projectId).Execute()

Get project integrations



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
	resp, r, err := apiClient.IntegrationsAPI.IntegrationsList(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.IntegrationsList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IntegrationsList`: IntegrationsList200Response
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.IntegrationsList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiIntegrationsListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**IntegrationsList200Response**](IntegrationsList200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


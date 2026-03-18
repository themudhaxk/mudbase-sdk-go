# \FunctionsAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FunctionsActivate**](FunctionsAPI.md#FunctionsActivate) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/activate | Activate function
[**FunctionsCreate**](FunctionsAPI.md#FunctionsCreate) | **Post** /api/functions/projects/{projectId}/functions | Create function
[**FunctionsDeactivate**](FunctionsAPI.md#FunctionsDeactivate) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/deactivate | Deactivate function
[**FunctionsDelete**](FunctionsAPI.md#FunctionsDelete) | **Delete** /api/functions/projects/{projectId}/functions/{functionId} | Delete function
[**FunctionsExecute**](FunctionsAPI.md#FunctionsExecute) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/execute | Execute function
[**FunctionsGet**](FunctionsAPI.md#FunctionsGet) | **Get** /api/functions/projects/{projectId}/functions/{functionId} | Get function
[**FunctionsGetLogs**](FunctionsAPI.md#FunctionsGetLogs) | **Get** /api/functions/projects/{projectId}/functions/{functionId}/logs | Get function execution logs
[**FunctionsGetVersions**](FunctionsAPI.md#FunctionsGetVersions) | **Get** /api/functions/projects/{projectId}/functions/{functionId}/versions | Get function versions
[**FunctionsList**](FunctionsAPI.md#FunctionsList) | **Get** /api/functions/projects/{projectId}/functions | List functions
[**FunctionsRetry**](FunctionsAPI.md#FunctionsRetry) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/retry/{executionIndex} | Retry failed execution
[**FunctionsRollback**](FunctionsAPI.md#FunctionsRollback) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/rollback | Rollback to previous version
[**FunctionsSimulate**](FunctionsAPI.md#FunctionsSimulate) | **Post** /api/functions/projects/{projectId}/functions/{functionId}/simulate | Simulate trigger
[**FunctionsTriggerWebhook**](FunctionsAPI.md#FunctionsTriggerWebhook) | **Post** /api/functions/webhook/{projectId} | Trigger webhook functions
[**FunctionsUpdate**](FunctionsAPI.md#FunctionsUpdate) | **Put** /api/functions/projects/{projectId}/functions/{functionId} | Update function



## FunctionsActivate

> FunctionResponse FunctionsActivate(ctx, projectId, functionId).Execute()

Activate function



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to activate.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsActivate(context.Background(), projectId, functionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsActivate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsActivate`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsActivate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to activate. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsActivateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsCreate

> FunctionResponse FunctionsCreate(ctx, projectId).CreateFunctionRequest(createFunctionRequest).Execute()

Create function



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
	createFunctionRequest := *openapiclient.NewCreateFunctionRequest("Name_example", "Code_example", *openapiclient.NewFunctionTrigger("Type_example")) // CreateFunctionRequest | Function name, description, code, trigger config, and optional environment.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsCreate(context.Background(), projectId).CreateFunctionRequest(createFunctionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsCreate`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsCreate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createFunctionRequest** | [**CreateFunctionRequest**](CreateFunctionRequest.md) | Function name, description, code, trigger config, and optional environment. | 

### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsDeactivate

> FunctionResponse FunctionsDeactivate(ctx, projectId, functionId).Execute()

Deactivate function



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to deactivate.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsDeactivate(context.Background(), projectId, functionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsDeactivate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsDeactivate`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsDeactivate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to deactivate. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsDeactivateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsDelete

> FunctionsDelete200Response FunctionsDelete(ctx, projectId, functionId).Execute()

Delete function



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
	functionId := "functionId_example" // string | Function ID to delete.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsDelete(context.Background(), projectId, functionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsDelete`: FunctionsDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**functionId** | **string** | Function ID to delete. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionsDelete200Response**](FunctionsDelete200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsExecute

> FunctionExecutionResponse FunctionsExecute(ctx, projectId, functionId).FunctionsExecuteRequest(functionsExecuteRequest).Execute()

Execute function



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to execute.
	functionsExecuteRequest := *openapiclient.NewFunctionsExecuteRequest() // FunctionsExecuteRequest | Optional JSON payload merged with trigger context (e.g. document, file, webhook body). Omit for no custom input. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsExecute(context.Background(), projectId, functionId).FunctionsExecuteRequest(functionsExecuteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsExecute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsExecute`: FunctionExecutionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsExecute`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to execute. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsExecuteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionsExecuteRequest** | [**FunctionsExecuteRequest**](FunctionsExecuteRequest.md) | Optional JSON payload merged with trigger context (e.g. document, file, webhook body). Omit for no custom input. | 

### Return type

[**FunctionExecutionResponse**](FunctionExecutionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsGet

> FunctionResponse FunctionsGet(ctx, projectId, functionId).Execute()

Get function



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
	functionId := "functionId_example" // string | Function ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsGet(context.Background(), projectId, functionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsGet`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**functionId** | **string** | Function ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsGetLogs

> FunctionLogsResponse FunctionsGetLogs(ctx, projectId, functionId).Limit(limit).Offset(offset).Execute()

Get function execution logs



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to get logs for.
	limit := int32(56) // int32 | Maximum number of log entries to return. (optional) (default to 50)
	offset := int32(56) // int32 | Number of log entries to skip for pagination. (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsGetLogs(context.Background(), projectId, functionId).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsGetLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsGetLogs`: FunctionLogsResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsGetLogs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to get logs for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsGetLogsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** | Maximum number of log entries to return. | [default to 50]
 **offset** | **int32** | Number of log entries to skip for pagination. | [default to 0]

### Return type

[**FunctionLogsResponse**](FunctionLogsResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsGetVersions

> FunctionsGetVersions200Response FunctionsGetVersions(ctx, projectId, functionId).Execute()

Get function versions



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to list versions for.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsGetVersions(context.Background(), projectId, functionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsGetVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsGetVersions`: FunctionsGetVersions200Response
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsGetVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to list versions for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsGetVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionsGetVersions200Response**](FunctionsGetVersions200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsList

> FunctionListResponse FunctionsList(ctx, projectId).Page(page).Limit(limit).Search(search).TriggerType(triggerType).IsActive(isActive).Execute()

List functions



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
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Number of functions per page. (optional) (default to 20)
	search := "search_example" // string | Search by name or description (optional)
	triggerType := "triggerType_example" // string | Filter by trigger type (optional)
	isActive := true // bool | Filter by active status (true/false) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsList(context.Background(), projectId).Page(page).Limit(limit).Search(search).TriggerType(triggerType).IsActive(isActive).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsList`: FunctionListResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of functions per page. | [default to 20]
 **search** | **string** | Search by name or description | 
 **triggerType** | **string** | Filter by trigger type | 
 **isActive** | **bool** | Filter by active status (true/false) | 

### Return type

[**FunctionListResponse**](FunctionListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsRetry

> FunctionExecutionResponse FunctionsRetry(ctx, projectId, functionId, executionIndex).Execute()

Retry failed execution



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to retry execution for.
	executionIndex := int32(56) // int32 | 0-based index of the execution in logs

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsRetry(context.Background(), projectId, functionId, executionIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsRetry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsRetry`: FunctionExecutionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsRetry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to retry execution for. | 
**executionIndex** | **int32** | 0-based index of the execution in logs | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsRetryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**FunctionExecutionResponse**](FunctionExecutionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsRollback

> FunctionResponse FunctionsRollback(ctx, projectId, functionId).FunctionsRollbackRequest(functionsRollbackRequest).Execute()

Rollback to previous version



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to rollback.
	functionsRollbackRequest := *openapiclient.NewFunctionsRollbackRequest(int32(123)) // FunctionsRollbackRequest | Version number (integer) to rollback to; use GET .../versions to list available versions.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsRollback(context.Background(), projectId, functionId).FunctionsRollbackRequest(functionsRollbackRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsRollback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsRollback`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsRollback`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to rollback. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsRollbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionsRollbackRequest** | [**FunctionsRollbackRequest**](FunctionsRollbackRequest.md) | Version number (integer) to rollback to; use GET .../versions to list available versions. | 

### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsSimulate

> FunctionExecutionResponse FunctionsSimulate(ctx, projectId, functionId).FunctionsSimulateRequest(functionsSimulateRequest).Execute()

Simulate trigger



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) that owns the function.
	functionId := "functionId_example" // string | Function ID (MongoDB ObjectId) to simulate.
	functionsSimulateRequest := *openapiclient.NewFunctionsSimulateRequest() // FunctionsSimulateRequest | Simulated trigger (type, event) and eventContext (document, file, webhook, wallet, message, or cron). Merged into the function payload for testing. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsSimulate(context.Background(), projectId, functionId).FunctionsSimulateRequest(functionsSimulateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsSimulate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsSimulate`: FunctionExecutionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsSimulate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) that owns the function. | 
**functionId** | **string** | Function ID (MongoDB ObjectId) to simulate. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsSimulateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionsSimulateRequest** | [**FunctionsSimulateRequest**](FunctionsSimulateRequest.md) | Simulated trigger (type, event) and eventContext (document, file, webhook, wallet, message, or cron). Merged into the function payload for testing. | 

### Return type

[**FunctionExecutionResponse**](FunctionExecutionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsTriggerWebhook

> FunctionsTriggerWebhook200Response FunctionsTriggerWebhook(ctx, projectId).XWebhookSecret(xWebhookSecret).Body(body).Execute()

Trigger webhook functions



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
	xWebhookSecret := "xWebhookSecret_example" // string | Optional webhook secret for verification (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} | Payload sent to the triggered function(s). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsTriggerWebhook(context.Background(), projectId).XWebhookSecret(xWebhookSecret).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsTriggerWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsTriggerWebhook`: FunctionsTriggerWebhook200Response
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsTriggerWebhook`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsTriggerWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xWebhookSecret** | **string** | Optional webhook secret for verification | 
 **body** | **map[string]interface{}** | Payload sent to the triggered function(s). | 

### Return type

[**FunctionsTriggerWebhook200Response**](FunctionsTriggerWebhook200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/x-www-form-urlencoded, text/plain
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FunctionsUpdate

> FunctionResponse FunctionsUpdate(ctx, projectId, functionId).UpdateFunctionRequest(updateFunctionRequest).Execute()

Update function



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
	functionId := "functionId_example" // string | Function ID.
	updateFunctionRequest := *openapiclient.NewUpdateFunctionRequest() // UpdateFunctionRequest | Fields to update (name, description, code, trigger, environment, isActive, limits, retryPolicy). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionsAPI.FunctionsUpdate(context.Background(), projectId, functionId).UpdateFunctionRequest(updateFunctionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionsAPI.FunctionsUpdate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FunctionsUpdate`: FunctionResponse
	fmt.Fprintf(os.Stdout, "Response from `FunctionsAPI.FunctionsUpdate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**functionId** | **string** | Function ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFunctionsUpdateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateFunctionRequest** | [**UpdateFunctionRequest**](UpdateFunctionRequest.md) | Fields to update (name, description, code, trigger, environment, isActive, limits, retryPolicy). | 

### Return type

[**FunctionResponse**](FunctionResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


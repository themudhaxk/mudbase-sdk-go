# \MessagingAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetMessageHistory**](MessagingAPI.md#GetMessageHistory) | **Get** /api/messaging/projects/{projectId}/messaging/history | Get message history
[**GetMessageStats**](MessagingAPI.md#GetMessageStats) | **Get** /api/messaging/projects/{projectId}/messaging/stats | Get message statistics
[**GetProjectFcmConfig**](MessagingAPI.md#GetProjectFcmConfig) | **Get** /api/messaging/projects/{projectId}/messaging/push-config | Get bring-your-own push credentials status (masked)
[**GetProjectSmsByo**](MessagingAPI.md#GetProjectSmsByo) | **Get** /api/messaging/projects/{projectId}/messaging/sms-provider | Get BYO SMS provider configuration (masked)
[**GetProjectVapidPublicKey**](MessagingAPI.md#GetProjectVapidPublicKey) | **Get** /api/messaging/projects/{projectId}/messaging/web-push/public-key | Get the Web Push public key (public)
[**GetProjectWebPushConfig**](MessagingAPI.md#GetProjectWebPushConfig) | **Get** /api/messaging/projects/{projectId}/messaging/web-push-config | Get native Web Push (VAPID) configuration
[**ListDeviceTokens**](MessagingAPI.md#ListDeviceTokens) | **Get** /api/messaging/projects/{projectId}/messaging/devices | List registered device tokens
[**ListWebPushSubscriptions**](MessagingAPI.md#ListWebPushSubscriptions) | **Get** /api/messaging/projects/{projectId}/messaging/web-push/subscriptions | List registered Web Push subscriptions
[**PatchProjectFcmConfig**](MessagingAPI.md#PatchProjectFcmConfig) | **Patch** /api/messaging/projects/{projectId}/messaging/push-config | Set or clear your own push service account (optional)
[**PatchProjectSmsByo**](MessagingAPI.md#PatchProjectSmsByo) | **Patch** /api/messaging/projects/{projectId}/messaging/sms-provider | Update BYO SMS provider credentials
[**PatchProjectWebPushConfig**](MessagingAPI.md#PatchProjectWebPushConfig) | **Patch** /api/messaging/projects/{projectId}/messaging/web-push-config | Update native Web Push (VAPID) configuration
[**RegisterDeviceToken**](MessagingAPI.md#RegisterDeviceToken) | **Post** /api/messaging/projects/{projectId}/messaging/devices | Register a device push token
[**RegisterWebPushSubscription**](MessagingAPI.md#RegisterWebPushSubscription) | **Post** /api/messaging/projects/{projectId}/messaging/web-push/subscriptions | Register a browser Web Push subscription
[**RemoveWebPushSubscription**](MessagingAPI.md#RemoveWebPushSubscription) | **Delete** /api/messaging/projects/{projectId}/messaging/web-push/subscriptions | Unregister a Web Push subscription
[**SendEmail**](MessagingAPI.md#SendEmail) | **Post** /api/messaging/projects/{projectId}/messaging/email | Send email
[**SendPushNotification**](MessagingAPI.md#SendPushNotification) | **Post** /api/messaging/projects/{projectId}/messaging/push | Send push notification
[**SendSMS**](MessagingAPI.md#SendSMS) | **Post** /api/messaging/projects/{projectId}/messaging/sms | Send SMS
[**UnregisterDeviceToken**](MessagingAPI.md#UnregisterDeviceToken) | **Delete** /api/messaging/projects/{projectId}/messaging/devices | Unregister a device push token



## GetMessageHistory

> MessageHistoryResponse GetMessageHistory(ctx, projectId).Type_(type_).Page(page).Limit(limit).Status(status).Execute()

Get message history



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	type_ := "type__example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	limit := int32(56) // int32 |  (optional) (default to 20)
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetMessageHistory(context.Background(), projectId).Type_(type_).Page(page).Limit(limit).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetMessageHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMessageHistory`: MessageHistoryResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetMessageHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMessageHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **type_** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **limit** | **int32** |  | [default to 20]
 **status** | **string** |  | 

### Return type

[**MessageHistoryResponse**](MessageHistoryResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMessageStats

> MessageStatsResponse GetMessageStats(ctx, projectId).StartDate(startDate).EndDate(endDate).Execute()

Get message statistics



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	startDate := time.Now() // time.Time |  (optional)
	endDate := time.Now() // time.Time |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetMessageStats(context.Background(), projectId).StartDate(startDate).EndDate(endDate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetMessageStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMessageStats`: MessageStatsResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetMessageStats`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMessageStatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startDate** | **time.Time** |  | 
 **endDate** | **time.Time** |  | 

### Return type

[**MessageStatsResponse**](MessageStatsResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectFcmConfig

> GetProjectFcmConfig200Response GetProjectFcmConfig(ctx, projectId).Execute()

Get bring-your-own push credentials status (masked)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetProjectFcmConfig(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetProjectFcmConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectFcmConfig`: GetProjectFcmConfig200Response
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetProjectFcmConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectFcmConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**GetProjectFcmConfig200Response**](GetProjectFcmConfig200Response.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectSmsByo

> GetProjectSmsByo200Response GetProjectSmsByo(ctx, projectId).Execute()

Get BYO SMS provider configuration (masked)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetProjectSmsByo(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetProjectSmsByo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectSmsByo`: GetProjectSmsByo200Response
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetProjectSmsByo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectSmsByoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**GetProjectSmsByo200Response**](GetProjectSmsByo200Response.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectVapidPublicKey

> WebPushPublicKeyResponse GetProjectVapidPublicKey(ctx, projectId).Execute()

Get the Web Push public key (public)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetProjectVapidPublicKey(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetProjectVapidPublicKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectVapidPublicKey`: WebPushPublicKeyResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetProjectVapidPublicKey`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectVapidPublicKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebPushPublicKeyResponse**](WebPushPublicKeyResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectWebPushConfig

> WebPushConfigResponse GetProjectWebPushConfig(ctx, projectId).Execute()

Get native Web Push (VAPID) configuration



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.GetProjectWebPushConfig(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.GetProjectWebPushConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectWebPushConfig`: WebPushConfigResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.GetProjectWebPushConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectWebPushConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebPushConfigResponse**](WebPushConfigResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDeviceTokens

> DeviceListResponse ListDeviceTokens(ctx, projectId).Execute()

List registered device tokens



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.ListDeviceTokens(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.ListDeviceTokens``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDeviceTokens`: DeviceListResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.ListDeviceTokens`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDeviceTokensRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeviceListResponse**](DeviceListResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWebPushSubscriptions

> WebPushSubscriptionListResponse ListWebPushSubscriptions(ctx, projectId).Execute()

List registered Web Push subscriptions



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.ListWebPushSubscriptions(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.ListWebPushSubscriptions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWebPushSubscriptions`: WebPushSubscriptionListResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.ListWebPushSubscriptions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListWebPushSubscriptionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebPushSubscriptionListResponse**](WebPushSubscriptionListResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchProjectFcmConfig

> PatchProjectFcmConfig(ctx, projectId).PatchProjectFcmConfigRequest(patchProjectFcmConfigRequest).Execute()

Set or clear your own push service account (optional)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	patchProjectFcmConfigRequest := openapiclient.patchProjectFcmConfig_request{PatchProjectFcmConfigRequestOneOf: models.NewPatchProjectFcmConfigRequestOneOf(map[string]interface{}(123))} // PatchProjectFcmConfigRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MessagingAPI.PatchProjectFcmConfig(context.Background(), projectId).PatchProjectFcmConfigRequest(patchProjectFcmConfigRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.PatchProjectFcmConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchProjectFcmConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **patchProjectFcmConfigRequest** | [**PatchProjectFcmConfigRequest**](PatchProjectFcmConfigRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchProjectSmsByo

> GetProjectSmsByo200Response PatchProjectSmsByo(ctx, projectId).ProjectSmsByoPatchRequest(projectSmsByoPatchRequest).Execute()

Update BYO SMS provider credentials



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	projectSmsByoPatchRequest := *models.NewProjectSmsByoPatchRequest() // ProjectSmsByoPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.PatchProjectSmsByo(context.Background(), projectId).ProjectSmsByoPatchRequest(projectSmsByoPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.PatchProjectSmsByo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchProjectSmsByo`: GetProjectSmsByo200Response
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.PatchProjectSmsByo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchProjectSmsByoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **projectSmsByoPatchRequest** | [**ProjectSmsByoPatchRequest**](ProjectSmsByoPatchRequest.md) |  | 

### Return type

[**GetProjectSmsByo200Response**](GetProjectSmsByo200Response.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchProjectWebPushConfig

> WebPushConfigResponse PatchProjectWebPushConfig(ctx, projectId).WebPushConfigPatchRequest(webPushConfigPatchRequest).Execute()

Update native Web Push (VAPID) configuration



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	webPushConfigPatchRequest := *models.NewWebPushConfigPatchRequest() // WebPushConfigPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.PatchProjectWebPushConfig(context.Background(), projectId).WebPushConfigPatchRequest(webPushConfigPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.PatchProjectWebPushConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchProjectWebPushConfig`: WebPushConfigResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.PatchProjectWebPushConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchProjectWebPushConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **webPushConfigPatchRequest** | [**WebPushConfigPatchRequest**](WebPushConfigPatchRequest.md) |  | 

### Return type

[**WebPushConfigResponse**](WebPushConfigResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterDeviceToken

> DeviceRegisteredResponse RegisterDeviceToken(ctx, projectId).DeviceRegisterRequest(deviceRegisterRequest).Execute()

Register a device push token



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	deviceRegisterRequest := *models.NewDeviceRegisterRequest("Token_example") // DeviceRegisterRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.RegisterDeviceToken(context.Background(), projectId).DeviceRegisterRequest(deviceRegisterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.RegisterDeviceToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterDeviceToken`: DeviceRegisteredResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.RegisterDeviceToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegisterDeviceTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deviceRegisterRequest** | [**DeviceRegisterRequest**](DeviceRegisterRequest.md) |  | 

### Return type

[**DeviceRegisteredResponse**](DeviceRegisteredResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterWebPushSubscription

> WebPushSubscribeResponse RegisterWebPushSubscription(ctx, projectId).WebPushSubscribeRequest(webPushSubscribeRequest).Execute()

Register a browser Web Push subscription



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	webPushSubscribeRequest := *models.NewWebPushSubscribeRequest(*models.NewWebPushSubscription("Endpoint_example", *models.NewWebPushSubscriptionKeys("P256dh_example", "Auth_example"))) // WebPushSubscribeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.RegisterWebPushSubscription(context.Background(), projectId).WebPushSubscribeRequest(webPushSubscribeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.RegisterWebPushSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterWebPushSubscription`: WebPushSubscribeResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.RegisterWebPushSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegisterWebPushSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **webPushSubscribeRequest** | [**WebPushSubscribeRequest**](WebPushSubscribeRequest.md) |  | 

### Return type

[**WebPushSubscribeResponse**](WebPushSubscribeResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveWebPushSubscription

> WebPushUnsubscribeResponse RemoveWebPushSubscription(ctx, projectId).WebPushUnsubscribeRequest(webPushUnsubscribeRequest).Execute()

Unregister a Web Push subscription



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	webPushUnsubscribeRequest := *models.NewWebPushUnsubscribeRequest("Endpoint_example") // WebPushUnsubscribeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.RemoveWebPushSubscription(context.Background(), projectId).WebPushUnsubscribeRequest(webPushUnsubscribeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.RemoveWebPushSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveWebPushSubscription`: WebPushUnsubscribeResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.RemoveWebPushSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveWebPushSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **webPushUnsubscribeRequest** | [**WebPushUnsubscribeRequest**](WebPushUnsubscribeRequest.md) |  | 

### Return type

[**WebPushUnsubscribeResponse**](WebPushUnsubscribeResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendEmail

> MessageSentResponse SendEmail(ctx, projectId).EmailRequest(emailRequest).Execute()

Send email



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	emailRequest := *models.NewEmailRequest(openapiclient.EmailRequest_to{ArrayOfString: new([]string)}, "Subject_example") // EmailRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.SendEmail(context.Background(), projectId).EmailRequest(emailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.SendEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendEmail`: MessageSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.SendEmail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **emailRequest** | [**EmailRequest**](EmailRequest.md) |  | 

### Return type

[**MessageSentResponse**](MessageSentResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendPushNotification

> PushSentResponse SendPushNotification(ctx, projectId).PushNotificationRequest(pushNotificationRequest).Execute()

Send push notification



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	pushNotificationRequest := *models.NewPushNotificationRequest("Title_example", "Body_example") // PushNotificationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.SendPushNotification(context.Background(), projectId).PushNotificationRequest(pushNotificationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.SendPushNotification``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendPushNotification`: PushSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.SendPushNotification`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendPushNotificationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **pushNotificationRequest** | [**PushNotificationRequest**](PushNotificationRequest.md) |  | 

### Return type

[**PushSentResponse**](PushSentResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendSMS

> MessageSentResponse SendSMS(ctx, projectId).SMSRequest(sMSRequest).Execute()

Send SMS



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	sMSRequest := *models.NewSMSRequest("To_example", "Message_example") // SMSRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.SendSMS(context.Background(), projectId).SMSRequest(sMSRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.SendSMS``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendSMS`: MessageSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.SendSMS`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendSMSRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sMSRequest** | [**SMSRequest**](SMSRequest.md) |  | 

### Return type

[**MessageSentResponse**](MessageSentResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UnregisterDeviceToken

> DeviceUnregisteredResponse UnregisterDeviceToken(ctx, projectId).DeviceUnregisterRequest(deviceUnregisterRequest).Execute()

Unregister a device push token



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/themudhaxk/mudbase-sdk-go"
	models "github.com/themudhaxk/mudbase-sdk-go/models"
)

func main() {
	projectId := "projectId_example" // string | 
	deviceUnregisterRequest := *models.NewDeviceUnregisterRequest("Token_example") // DeviceUnregisterRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.UnregisterDeviceToken(context.Background(), projectId).DeviceUnregisterRequest(deviceUnregisterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.UnregisterDeviceToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UnregisterDeviceToken`: DeviceUnregisteredResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.UnregisterDeviceToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUnregisterDeviceTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deviceUnregisterRequest** | [**DeviceUnregisterRequest**](DeviceUnregisterRequest.md) |  | 

### Return type

[**DeviceUnregisteredResponse**](DeviceUnregisteredResponse.md)

### Authorization

[OrgBearerAuth](../README.md#OrgBearerAuth), [ApiKeyAuth](../README.md#ApiKeyAuth), [ProjectBearerAuth](../README.md#ProjectBearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


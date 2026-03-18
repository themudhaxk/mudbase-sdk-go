# \MessagingAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MessagingGetHistory**](MessagingAPI.md#MessagingGetHistory) | **Get** /api/messaging/projects/{projectId}/messaging/history | Get message history
[**MessagingGetStats**](MessagingAPI.md#MessagingGetStats) | **Get** /api/messaging/projects/{projectId}/messaging/stats | Get message statistics
[**MessagingSendEmail**](MessagingAPI.md#MessagingSendEmail) | **Post** /api/messaging/projects/{projectId}/messaging/email | Send transactional email
[**MessagingSendPush**](MessagingAPI.md#MessagingSendPush) | **Post** /api/messaging/projects/{projectId}/messaging/push | Send push notification
[**MessagingSendSms**](MessagingAPI.md#MessagingSendSms) | **Post** /api/messaging/projects/{projectId}/messaging/sms | Send SMS to one or more recipients (E.164 format)



## MessagingGetHistory

> MessageHistoryResponse MessagingGetHistory(ctx, projectId).Type_(type_).Page(page).Limit(limit).Status(status).Execute()

Get message history



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the messaging project.
	type_ := "type__example" // string | Filter by message type (push, email, or sms). (optional)
	page := int32(56) // int32 | Page number for pagination (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Maximum number of messages per page. (optional) (default to 20)
	status := "status_example" // string | Filter by delivery status. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.MessagingGetHistory(context.Background(), projectId).Type_(type_).Page(page).Limit(limit).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.MessagingGetHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MessagingGetHistory`: MessageHistoryResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.MessagingGetHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the messaging project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMessagingGetHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **type_** | **string** | Filter by message type (push, email, or sms). | 
 **page** | **int32** | Page number for pagination (1-based). | [default to 1]
 **limit** | **int32** | Maximum number of messages per page. | [default to 20]
 **status** | **string** | Filter by delivery status. | 

### Return type

[**MessageHistoryResponse**](MessageHistoryResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MessagingGetStats

> MessageStatsResponse MessagingGetStats(ctx, projectId).StartDate(startDate).EndDate(endDate).Execute()

Get message statistics



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the messaging project.
	startDate := time.Now() // time.Time | Start of the date range for statistics (ISO 8601). (optional)
	endDate := time.Now() // time.Time | End of the date range for statistics (ISO 8601). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.MessagingGetStats(context.Background(), projectId).StartDate(startDate).EndDate(endDate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.MessagingGetStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MessagingGetStats`: MessageStatsResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.MessagingGetStats`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the messaging project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMessagingGetStatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startDate** | **time.Time** | Start of the date range for statistics (ISO 8601). | 
 **endDate** | **time.Time** | End of the date range for statistics (ISO 8601). | 

### Return type

[**MessageStatsResponse**](MessageStatsResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MessagingSendEmail

> MessageSentResponse MessagingSendEmail(ctx, projectId).EmailRequest(emailRequest).Execute()

Send transactional email



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the messaging project.
	emailRequest := *openapiclient.NewEmailRequest(openapiclient.EmailRequest_to{ArrayOfString: new([]string)}, "Subject_example") // EmailRequest | Recipient(s), subject, HTML and/or plain text body; optional reply-to and attachments.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.MessagingSendEmail(context.Background(), projectId).EmailRequest(emailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.MessagingSendEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MessagingSendEmail`: MessageSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.MessagingSendEmail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the messaging project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMessagingSendEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **emailRequest** | [**EmailRequest**](EmailRequest.md) | Recipient(s), subject, HTML and/or plain text body; optional reply-to and attachments. | 

### Return type

[**MessageSentResponse**](MessageSentResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MessagingSendPush

> MessageSentResponse MessagingSendPush(ctx, projectId).PushNotificationRequest(pushNotificationRequest).Execute()

Send push notification



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the messaging project.
	pushNotificationRequest := *openapiclient.NewPushNotificationRequest([]string{"Tokens_example"}, "Title_example", "Body_example") // PushNotificationRequest | Device tokens, notification title/body, optional data payload and image URL.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.MessagingSendPush(context.Background(), projectId).PushNotificationRequest(pushNotificationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.MessagingSendPush``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MessagingSendPush`: MessageSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.MessagingSendPush`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the messaging project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMessagingSendPushRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **pushNotificationRequest** | [**PushNotificationRequest**](PushNotificationRequest.md) | Device tokens, notification title/body, optional data payload and image URL. | 

### Return type

[**MessageSentResponse**](MessageSentResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MessagingSendSms

> MessageSentResponse MessagingSendSms(ctx, projectId).SMSRequest(sMSRequest).Execute()

Send SMS to one or more recipients (E.164 format)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the messaging project.
	sMSRequest := *openapiclient.NewSMSRequest("To_example", "Message_example") // SMSRequest | Recipient phone number(s), message body, and optional sender ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessagingAPI.MessagingSendSms(context.Background(), projectId).SMSRequest(sMSRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessagingAPI.MessagingSendSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MessagingSendSms`: MessageSentResponse
	fmt.Fprintf(os.Stdout, "Response from `MessagingAPI.MessagingSendSms`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the messaging project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMessagingSendSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sMSRequest** | [**SMSRequest**](SMSRequest.md) | Recipient phone number(s), message body, and optional sender ID. | 

### Return type

[**MessageSentResponse**](MessageSentResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


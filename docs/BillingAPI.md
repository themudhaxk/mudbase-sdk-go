# \BillingAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BillingCheckFeatureAccess**](BillingAPI.md#BillingCheckFeatureAccess) | **Get** /api/billing/public/projects/{projectId}/feature-access | Check feature access (public)
[**BillingCheckSubscription**](BillingAPI.md#BillingCheckSubscription) | **Get** /api/billing/public/projects/{projectId}/subscription | Check subscription status (public)
[**BillingCreateCheckoutSession**](BillingAPI.md#BillingCreateCheckoutSession) | **Post** /api/billing/public/projects/{projectId}/checkout | Create checkout session (Flutterwave or crypto)
[**BillingGetCheckoutPayment**](BillingAPI.md#BillingGetCheckoutPayment) | **Get** /api/billing/public/projects/{projectId}/checkout/{paymentId} | Get checkout payment details
[**BillingGetPublicPlans**](BillingAPI.md#BillingGetPublicPlans) | **Get** /api/billing/public/projects/{projectId}/plans | Get public plans (no auth required)
[**BillingHandleCryptoWebhook**](BillingAPI.md#BillingHandleCryptoWebhook) | **Post** /api/billing/webhooks/crypto | Crypto payment processor webhook
[**BillingHandleFlutterwaveWebhook**](BillingAPI.md#BillingHandleFlutterwaveWebhook) | **Post** /api/billing/webhooks/flutterwave | Flutterwave webhook
[**BillingInitializePayment**](BillingAPI.md#BillingInitializePayment) | **Post** /api/projects/{projectId}/payment-processing/initialize-payment | Initialize fiat payment (app-scoped)
[**BillingRecordUsage**](BillingAPI.md#BillingRecordUsage) | **Post** /api/billing/public/projects/{projectId}/usage | Record usage (public)
[**BillingVerifyPayment**](BillingAPI.md#BillingVerifyPayment) | **Post** /api/billing/public/projects/{projectId}/verify-payment | Verify payment and create subscription



## BillingCheckFeatureAccess

> BillingCheckFeatureAccess200Response BillingCheckFeatureAccess(ctx, projectId).Email(email).Feature(feature).Execute()

Check feature access (public)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	email := "email_example" // string | Customer email
	feature := "feature_example" // string | Feature slug to check access for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingCheckFeatureAccess(context.Background(), projectId).Email(email).Feature(feature).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingCheckFeatureAccess``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingCheckFeatureAccess`: BillingCheckFeatureAccess200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingCheckFeatureAccess`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingCheckFeatureAccessRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **email** | **string** | Customer email | 
 **feature** | **string** | Feature slug to check access for | 

### Return type

[**BillingCheckFeatureAccess200Response**](BillingCheckFeatureAccess200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingCheckSubscription

> BillingCheckSubscription200Response BillingCheckSubscription(ctx, projectId).Email(email).Execute()

Check subscription status (public)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	email := "email_example" // string | Customer email to check subscription for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingCheckSubscription(context.Background(), projectId).Email(email).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingCheckSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingCheckSubscription`: BillingCheckSubscription200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingCheckSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingCheckSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **email** | **string** | Customer email to check subscription for | 

### Return type

[**BillingCheckSubscription200Response**](BillingCheckSubscription200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingCreateCheckoutSession

> BillingCreateCheckoutSession200Response BillingCreateCheckoutSession(ctx, projectId).BillingCreateCheckoutSessionRequest(billingCreateCheckoutSessionRequest).Execute()

Create checkout session (Flutterwave or crypto)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	billingCreateCheckoutSessionRequest := *openapiclient.NewBillingCreateCheckoutSessionRequest("PlanId_example", "BillingCycle_example", *openapiclient.NewBillingCreateCheckoutSessionRequestCustomerInfo("Email_example")) // BillingCreateCheckoutSessionRequest | Plan to subscribe to, billing cycle, customer email/name, and optional success/cancel redirect URLs.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingCreateCheckoutSession(context.Background(), projectId).BillingCreateCheckoutSessionRequest(billingCreateCheckoutSessionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingCreateCheckoutSession``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingCreateCheckoutSession`: BillingCreateCheckoutSession200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingCreateCheckoutSession`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingCreateCheckoutSessionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **billingCreateCheckoutSessionRequest** | [**BillingCreateCheckoutSessionRequest**](BillingCreateCheckoutSessionRequest.md) | Plan to subscribe to, billing cycle, customer email/name, and optional success/cancel redirect URLs. | 

### Return type

[**BillingCreateCheckoutSession200Response**](BillingCreateCheckoutSession200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingGetCheckoutPayment

> BillingGetCheckoutPayment200Response BillingGetCheckoutPayment(ctx, projectId, paymentId).Execute()

Get checkout payment details



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	paymentId := "paymentId_example" // string | Payment ID or reference from checkout session

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingGetCheckoutPayment(context.Background(), projectId, paymentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingGetCheckoutPayment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingGetCheckoutPayment`: BillingGetCheckoutPayment200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingGetCheckoutPayment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 
**paymentId** | **string** | Payment ID or reference from checkout session | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingGetCheckoutPaymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**BillingGetCheckoutPayment200Response**](BillingGetCheckoutPayment200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingGetPublicPlans

> BillingGetPublicPlans200Response BillingGetPublicPlans(ctx, projectId).Execute()

Get public plans (no auth required)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) to list plans for.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingGetPublicPlans(context.Background(), projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingGetPublicPlans``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingGetPublicPlans`: BillingGetPublicPlans200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingGetPublicPlans`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) to list plans for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingGetPublicPlansRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BillingGetPublicPlans200Response**](BillingGetPublicPlans200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingHandleCryptoWebhook

> BillingHandleCryptoWebhook200Response BillingHandleCryptoWebhook(ctx).BillingHandleCryptoWebhookRequest(billingHandleCryptoWebhookRequest).Execute()

Crypto payment processor webhook



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
	billingHandleCryptoWebhookRequest := *openapiclient.NewBillingHandleCryptoWebhookRequest("Event_example", *openapiclient.NewBillingHandleCryptoWebhookRequestData()) // BillingHandleCryptoWebhookRequest | Crypto payment webhook payload (event type and data with paymentId, reference, amount, currency, network, status, metadata).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingHandleCryptoWebhook(context.Background()).BillingHandleCryptoWebhookRequest(billingHandleCryptoWebhookRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingHandleCryptoWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingHandleCryptoWebhook`: BillingHandleCryptoWebhook200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingHandleCryptoWebhook`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBillingHandleCryptoWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **billingHandleCryptoWebhookRequest** | [**BillingHandleCryptoWebhookRequest**](BillingHandleCryptoWebhookRequest.md) | Crypto payment webhook payload (event type and data with paymentId, reference, amount, currency, network, status, metadata). | 

### Return type

[**BillingHandleCryptoWebhook200Response**](BillingHandleCryptoWebhook200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingHandleFlutterwaveWebhook

> BillingHandleCryptoWebhook200Response BillingHandleFlutterwaveWebhook(ctx).BillingHandleFlutterwaveWebhookRequest(billingHandleFlutterwaveWebhookRequest).Execute()

Flutterwave webhook



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
	billingHandleFlutterwaveWebhookRequest := *openapiclient.NewBillingHandleFlutterwaveWebhookRequest() // BillingHandleFlutterwaveWebhookRequest | Flutterwave webhook payload (event and data with id, tx_ref, amount, currency, status, customer, meta for subscription or payment-processing).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingHandleFlutterwaveWebhook(context.Background()).BillingHandleFlutterwaveWebhookRequest(billingHandleFlutterwaveWebhookRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingHandleFlutterwaveWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingHandleFlutterwaveWebhook`: BillingHandleCryptoWebhook200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingHandleFlutterwaveWebhook`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBillingHandleFlutterwaveWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **billingHandleFlutterwaveWebhookRequest** | [**BillingHandleFlutterwaveWebhookRequest**](BillingHandleFlutterwaveWebhookRequest.md) | Flutterwave webhook payload (event and data with id, tx_ref, amount, currency, status, customer, meta for subscription or payment-processing). | 

### Return type

[**BillingHandleCryptoWebhook200Response**](BillingHandleCryptoWebhook200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingInitializePayment

> BillingInitializePayment(ctx, projectId).BillingInitializePaymentRequest(billingInitializePaymentRequest).Execute()

Initialize fiat payment (app-scoped)



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
	projectId := "projectId_example" // string | Project ID for payment scope and tx_ref.
	billingInitializePaymentRequest := *openapiclient.NewBillingInitializePaymentRequest(float32(123), *openapiclient.NewBillingInitializePaymentRequestCustomer("Email_example")) // BillingInitializePaymentRequest | Payment amount, currency, customer (email, name), and optional metadata.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.BillingAPI.BillingInitializePayment(context.Background(), projectId).BillingInitializePaymentRequest(billingInitializePaymentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingInitializePayment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID for payment scope and tx_ref. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingInitializePaymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **billingInitializePaymentRequest** | [**BillingInitializePaymentRequest**](BillingInitializePaymentRequest.md) | Payment amount, currency, customer (email, name), and optional metadata. | 

### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingRecordUsage

> MessageResponse BillingRecordUsage(ctx, projectId).BillingRecordUsageRequest(billingRecordUsageRequest).Execute()

Record usage (public)



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	billingRecordUsageRequest := *openapiclient.NewBillingRecordUsageRequest("Email_example", "Metric_example", float32(123)) // BillingRecordUsageRequest | Customer email, metric name (e.g. api_calls, storage_mb), and quantity to record.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingRecordUsage(context.Background(), projectId).BillingRecordUsageRequest(billingRecordUsageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingRecordUsage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingRecordUsage`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingRecordUsage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingRecordUsageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **billingRecordUsageRequest** | [**BillingRecordUsageRequest**](BillingRecordUsageRequest.md) | Customer email, metric name (e.g. api_calls, storage_mb), and quantity to record. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BillingVerifyPayment

> BillingVerifyPayment200Response BillingVerifyPayment(ctx, projectId).Reference(reference).Execute()

Verify payment and create subscription



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
	projectId := "projectId_example" // string | Project ID (MongoDB ObjectId) for the billing project.
	reference := "reference_example" // string | Payment reference (e.g. mudbase_abc123 or pmt_abc123)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.BillingVerifyPayment(context.Background(), projectId).Reference(reference).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.BillingVerifyPayment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BillingVerifyPayment`: BillingVerifyPayment200Response
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.BillingVerifyPayment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID (MongoDB ObjectId) for the billing project. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBillingVerifyPaymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **reference** | **string** | Payment reference (e.g. mudbase_abc123 or pmt_abc123) | 

### Return type

[**BillingVerifyPayment200Response**](BillingVerifyPayment200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


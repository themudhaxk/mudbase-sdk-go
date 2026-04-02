# \WalletAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WalletBroadcastTransaction**](WalletAPI.md#WalletBroadcastTransaction) | **Post** /api/wallet/non-custodial/broadcast | Broadcast a client-signed transaction
[**WalletCreateWebhook**](WalletAPI.md#WalletCreateWebhook) | **Post** /api/wallet/non-custodial/webhooks | Create a wallet webhook
[**WalletDeleteAddress**](WalletAPI.md#WalletDeleteAddress) | **Delete** /api/wallet/non-custodial/addresses/{addressId} | Delete (soft-delete) a non-custodial address
[**WalletDeleteWebhook**](WalletAPI.md#WalletDeleteWebhook) | **Delete** /api/wallet/non-custodial/webhooks/{webhookId} | Delete a wallet webhook
[**WalletEstimateGas**](WalletAPI.md#WalletEstimateGas) | **Post** /api/wallet/non-custodial/estimate-gas | Estimate network fee from blockchain (all supported chains; not controlled by Mudbase)
[**WalletGetAddress**](WalletAPI.md#WalletGetAddress) | **Get** /api/wallet/non-custodial/addresses/{addressId} | Get non-custodial address by ID
[**WalletGetBalance**](WalletAPI.md#WalletGetBalance) | **Get** /api/wallet/non-custodial/addresses/{addressId}/balance | Get balance for a non-custodial address
[**WalletGetCancelParams**](WalletAPI.md#WalletGetCancelParams) | **Post** /api/wallet/non-custodial/cancel | Get replacement tx params for cancel (stuck EVM tx)
[**WalletGetSpeedUpParams**](WalletAPI.md#WalletGetSpeedUpParams) | **Post** /api/wallet/non-custodial/speed-up | Get replacement tx params for speed-up (stuck EVM tx)
[**WalletGetTransactionByHash**](WalletAPI.md#WalletGetTransactionByHash) | **Get** /api/wallet/non-custodial/transactions/{txHash} | Get transaction by hash
[**WalletGetTransactions**](WalletAPI.md#WalletGetTransactions) | **Get** /api/wallet/non-custodial/addresses/{addressId}/transactions | Get transaction history for a non-custodial address
[**WalletGetWebhookLogs**](WalletAPI.md#WalletGetWebhookLogs) | **Get** /api/wallet/non-custodial/webhooks/{webhookId}/logs | Get webhook delivery logs
[**WalletListAddresses**](WalletAPI.md#WalletListAddresses) | **Get** /api/wallet/non-custodial/addresses | List registered non-custodial addresses
[**WalletListWebhooks**](WalletAPI.md#WalletListWebhooks) | **Get** /api/wallet/non-custodial/webhooks | List wallet webhooks
[**WalletRegisterAddress**](WalletAPI.md#WalletRegisterAddress) | **Post** /api/wallet/non-custodial/register-address | Register a non-custodial wallet address
[**WalletTestWebhook**](WalletAPI.md#WalletTestWebhook) | **Post** /api/wallet/non-custodial/webhooks/test | Test a webhook delivery (sends a single test payload)
[**WalletUpdateWebhook**](WalletAPI.md#WalletUpdateWebhook) | **Put** /api/wallet/non-custodial/webhooks/{webhookId} | Update a wallet webhook



## WalletBroadcastTransaction

> WalletBroadcastTransaction200Response WalletBroadcastTransaction(ctx).WalletBroadcastTransactionRequest(walletBroadcastTransactionRequest).Execute()

Broadcast a client-signed transaction



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
	walletBroadcastTransactionRequest := *openapiclient.NewWalletBroadcastTransactionRequest("Chain_example", "0x02f8...", "0x742d35Cc6634C0532925a3b844Bc9e7595f0bEb") // WalletBroadcastTransactionRequest | Chain, signed transaction (hex), and fromAddress (must be registered).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletBroadcastTransaction(context.Background()).WalletBroadcastTransactionRequest(walletBroadcastTransactionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletBroadcastTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletBroadcastTransaction`: WalletBroadcastTransaction200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletBroadcastTransaction`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletBroadcastTransactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletBroadcastTransactionRequest** | [**WalletBroadcastTransactionRequest**](WalletBroadcastTransactionRequest.md) | Chain, signed transaction (hex), and fromAddress (must be registered). | 

### Return type

[**WalletBroadcastTransaction200Response**](WalletBroadcastTransaction200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletCreateWebhook

> WalletCreateWebhook201Response WalletCreateWebhook(ctx).WalletCreateWebhookRequest(walletCreateWebhookRequest).Execute()

Create a wallet webhook



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
	walletCreateWebhookRequest := *openapiclient.NewWalletCreateWebhookRequest("https://your-app.com/webhooks/wallet", []string{"Events_example"}) // WalletCreateWebhookRequest | Webhook URL, events array, optional secret and filters (addresses, chains, projectId).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletCreateWebhook(context.Background()).WalletCreateWebhookRequest(walletCreateWebhookRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletCreateWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletCreateWebhook`: WalletCreateWebhook201Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletCreateWebhook`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletCreateWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletCreateWebhookRequest** | [**WalletCreateWebhookRequest**](WalletCreateWebhookRequest.md) | Webhook URL, events array, optional secret and filters (addresses, chains, projectId). | 

### Return type

[**WalletCreateWebhook201Response**](WalletCreateWebhook201Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletDeleteAddress

> FunctionsDelete200Response WalletDeleteAddress(ctx, addressId).Execute()

Delete (soft-delete) a non-custodial address



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
	addressId := "addressId_example" // string | Registered address ID to delete.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletDeleteAddress(context.Background(), addressId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletDeleteAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletDeleteAddress`: FunctionsDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletDeleteAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**addressId** | **string** | Registered address ID to delete. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletDeleteAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**FunctionsDelete200Response**](FunctionsDelete200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletDeleteWebhook

> FunctionsDelete200Response WalletDeleteWebhook(ctx, webhookId).Execute()

Delete a wallet webhook



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
	webhookId := "webhookId_example" // string | Webhook ID (MongoDB ObjectId) to delete.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletDeleteWebhook(context.Background(), webhookId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletDeleteWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletDeleteWebhook`: FunctionsDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletDeleteWebhook`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**webhookId** | **string** | Webhook ID (MongoDB ObjectId) to delete. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletDeleteWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**FunctionsDelete200Response**](FunctionsDelete200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletEstimateGas

> WalletEstimateGas200Response WalletEstimateGas(ctx).WalletEstimateGasRequest(walletEstimateGasRequest).Execute()

Estimate network fee from blockchain (all supported chains; not controlled by Mudbase)



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
	walletEstimateGasRequest := *openapiclient.NewWalletEstimateGasRequest("Chain_example") // WalletEstimateGasRequest | Chain and optional transaction shape (required for EVM). Returns network fee from blockchain.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletEstimateGas(context.Background()).WalletEstimateGasRequest(walletEstimateGasRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletEstimateGas``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletEstimateGas`: WalletEstimateGas200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletEstimateGas`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletEstimateGasRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletEstimateGasRequest** | [**WalletEstimateGasRequest**](WalletEstimateGasRequest.md) | Chain and optional transaction shape (required for EVM). Returns network fee from blockchain. | 

### Return type

[**WalletEstimateGas200Response**](WalletEstimateGas200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetAddress

> NonCustodialAddressResponse WalletGetAddress(ctx, addressId).Execute()

Get non-custodial address by ID



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
	addressId := "addressId_example" // string | Registered address ID (MongoDB ObjectId).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetAddress(context.Background(), addressId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetAddress`: NonCustodialAddressResponse
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**addressId** | **string** | Registered address ID (MongoDB ObjectId). | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NonCustodialAddressResponse**](NonCustodialAddressResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetBalance

> WalletGetBalance200Response WalletGetBalance(ctx, addressId).Execute()

Get balance for a non-custodial address



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
	addressId := "addressId_example" // string | Registered address ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetBalance(context.Background(), addressId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetBalance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetBalance`: WalletGetBalance200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetBalance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**addressId** | **string** | Registered address ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetBalanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WalletGetBalance200Response**](WalletGetBalance200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetCancelParams

> WalletGetCancelParams200Response WalletGetCancelParams(ctx).WalletGetCancelParamsRequest(walletGetCancelParamsRequest).Execute()

Get replacement tx params for cancel (stuck EVM tx)



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
	walletGetCancelParamsRequest := *openapiclient.NewWalletGetCancelParamsRequest("Chain_example") // WalletGetCancelParamsRequest | Stuck transaction identifier (txId or txHash) and EVM chain for cancel.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetCancelParams(context.Background()).WalletGetCancelParamsRequest(walletGetCancelParamsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetCancelParams``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetCancelParams`: WalletGetCancelParams200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetCancelParams`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetCancelParamsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletGetCancelParamsRequest** | [**WalletGetCancelParamsRequest**](WalletGetCancelParamsRequest.md) | Stuck transaction identifier (txId or txHash) and EVM chain for cancel. | 

### Return type

[**WalletGetCancelParams200Response**](WalletGetCancelParams200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetSpeedUpParams

> WalletGetSpeedUpParams200Response WalletGetSpeedUpParams(ctx).WalletGetSpeedUpParamsRequest(walletGetSpeedUpParamsRequest).Execute()

Get replacement tx params for speed-up (stuck EVM tx)



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
	walletGetSpeedUpParamsRequest := *openapiclient.NewWalletGetSpeedUpParamsRequest("Chain_example") // WalletGetSpeedUpParamsRequest | Stuck transaction identifier (txId or txHash) and EVM chain.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetSpeedUpParams(context.Background()).WalletGetSpeedUpParamsRequest(walletGetSpeedUpParamsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetSpeedUpParams``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetSpeedUpParams`: WalletGetSpeedUpParams200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetSpeedUpParams`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetSpeedUpParamsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletGetSpeedUpParamsRequest** | [**WalletGetSpeedUpParamsRequest**](WalletGetSpeedUpParamsRequest.md) | Stuck transaction identifier (txId or txHash) and EVM chain. | 

### Return type

[**WalletGetSpeedUpParams200Response**](WalletGetSpeedUpParams200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetTransactionByHash

> WalletGetTransactionByHash200Response WalletGetTransactionByHash(ctx, txHash).Chain(chain).Execute()

Get transaction by hash



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
	txHash := "txHash_example" // string | Transaction hash (e.g. 0x... for EVM, or block explorer format for UTXO)
	chain := "chain_example" // string | Chain the transaction belongs to (required for lookup)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetTransactionByHash(context.Background(), txHash).Chain(chain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetTransactionByHash``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetTransactionByHash`: WalletGetTransactionByHash200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetTransactionByHash`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**txHash** | **string** | Transaction hash (e.g. 0x... for EVM, or block explorer format for UTXO) | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetTransactionByHashRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **chain** | **string** | Chain the transaction belongs to (required for lookup) | 

### Return type

[**WalletGetTransactionByHash200Response**](WalletGetTransactionByHash200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetTransactions

> WalletGetTransactions200Response WalletGetTransactions(ctx, addressId).Limit(limit).Page(page).Execute()

Get transaction history for a non-custodial address



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
	addressId := "addressId_example" // string | Registered address ID.
	limit := int32(56) // int32 | Number of transactions per page. (optional) (default to 50)
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetTransactions(context.Background(), addressId).Limit(limit).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetTransactions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetTransactions`: WalletGetTransactions200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetTransactions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**addressId** | **string** | Registered address ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetTransactionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | Number of transactions per page. | [default to 50]
 **page** | **int32** | Page number (1-based). | [default to 1]

### Return type

[**WalletGetTransactions200Response**](WalletGetTransactions200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletGetWebhookLogs

> WalletGetWebhookLogs200Response WalletGetWebhookLogs(ctx, webhookId).Limit(limit).Execute()

Get webhook delivery logs



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
	webhookId := "webhookId_example" // string | Webhook ID (MongoDB ObjectId) to get logs for.
	limit := int32(56) // int32 | Maximum number of log entries to return. (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletGetWebhookLogs(context.Background(), webhookId).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletGetWebhookLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletGetWebhookLogs`: WalletGetWebhookLogs200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletGetWebhookLogs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**webhookId** | **string** | Webhook ID (MongoDB ObjectId) to get logs for. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletGetWebhookLogsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | Maximum number of log entries to return. | [default to 50]

### Return type

[**WalletGetWebhookLogs200Response**](WalletGetWebhookLogs200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletListAddresses

> WalletListAddresses200Response WalletListAddresses(ctx).Chain(chain).ProjectId(projectId).Execute()

List registered non-custodial addresses



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
	chain := "chain_example" // string | Filter by chain (optional) (optional)
	projectId := "projectId_example" // string | Filter by project ID (optional). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletListAddresses(context.Background()).Chain(chain).ProjectId(projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletListAddresses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletListAddresses`: WalletListAddresses200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletListAddresses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletListAddressesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chain** | **string** | Filter by chain (optional) | 
 **projectId** | **string** | Filter by project ID (optional). | 

### Return type

[**WalletListAddresses200Response**](WalletListAddresses200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletListWebhooks

> WalletListWebhooks200Response WalletListWebhooks(ctx).ProjectId(projectId).Execute()

List wallet webhooks



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
	projectId := "projectId_example" // string | Filter by project ID (optional). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletListWebhooks(context.Background()).ProjectId(projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletListWebhooks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletListWebhooks`: WalletListWebhooks200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletListWebhooks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletListWebhooksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **projectId** | **string** | Filter by project ID (optional). | 

### Return type

[**WalletListWebhooks200Response**](WalletListWebhooks200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletRegisterAddress

> NonCustodialAddressResponse WalletRegisterAddress(ctx).WalletRegisterAddressRequest(walletRegisterAddressRequest).Execute()

Register a non-custodial wallet address



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
	walletRegisterAddressRequest := *openapiclient.NewWalletRegisterAddressRequest("0x742d35Cc6634C0532925a3b844Bc9e7595f0bEb", "Chain_example") // WalletRegisterAddressRequest | Public address, chain identifier, and optional derivation path and label. projectId scopes the registration to a project.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletRegisterAddress(context.Background()).WalletRegisterAddressRequest(walletRegisterAddressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletRegisterAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletRegisterAddress`: NonCustodialAddressResponse
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletRegisterAddress`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletRegisterAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletRegisterAddressRequest** | [**WalletRegisterAddressRequest**](WalletRegisterAddressRequest.md) | Public address, chain identifier, and optional derivation path and label. projectId scopes the registration to a project. | 

### Return type

[**NonCustodialAddressResponse**](NonCustodialAddressResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletTestWebhook

> MultiRoleGetPermissionsMatrix200Response WalletTestWebhook(ctx).WalletTestWebhookRequest(walletTestWebhookRequest).Execute()

Test a webhook delivery (sends a single test payload)



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
	walletTestWebhookRequest := *openapiclient.NewWalletTestWebhookRequest("Url_example") // WalletTestWebhookRequest | URL to send the test POST to; optional secret and projectId for scoping; optional event type to simulate.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletTestWebhook(context.Background()).WalletTestWebhookRequest(walletTestWebhookRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletTestWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletTestWebhook`: MultiRoleGetPermissionsMatrix200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletTestWebhook`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalletTestWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **walletTestWebhookRequest** | [**WalletTestWebhookRequest**](WalletTestWebhookRequest.md) | URL to send the test POST to; optional secret and projectId for scoping; optional event type to simulate. | 

### Return type

[**MultiRoleGetPermissionsMatrix200Response**](MultiRoleGetPermissionsMatrix200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WalletUpdateWebhook

> WalletUpdateWebhook200Response WalletUpdateWebhook(ctx, webhookId).WalletUpdateWebhookRequest(walletUpdateWebhookRequest).Execute()

Update a wallet webhook



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
	webhookId := "webhookId_example" // string | Webhook ID (MongoDB ObjectId) to update.
	walletUpdateWebhookRequest := *openapiclient.NewWalletUpdateWebhookRequest() // WalletUpdateWebhookRequest | Fields to update (url, events, secret, filters). Omitted fields are left unchanged.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalletAPI.WalletUpdateWebhook(context.Background(), webhookId).WalletUpdateWebhookRequest(walletUpdateWebhookRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalletAPI.WalletUpdateWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalletUpdateWebhook`: WalletUpdateWebhook200Response
	fmt.Fprintf(os.Stdout, "Response from `WalletAPI.WalletUpdateWebhook`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**webhookId** | **string** | Webhook ID (MongoDB ObjectId) to update. | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalletUpdateWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **walletUpdateWebhookRequest** | [**WalletUpdateWebhookRequest**](WalletUpdateWebhookRequest.md) | Fields to update (url, events, secret, filters). Omitted fields are left unchanged. | 

### Return type

[**WalletUpdateWebhook200Response**](WalletUpdateWebhook200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


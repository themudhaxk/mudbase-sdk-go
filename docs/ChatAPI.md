# \ChatAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChatAddParticipant**](ChatAPI.md#ChatAddParticipant) | **Post** /api/chat/projects/{projectId}/chats/{chatId}/participants | Add participant to chat
[**ChatAddReaction**](ChatAPI.md#ChatAddReaction) | **Post** /api/chat/projects/{projectId}/chats/{chatId}/messages/{messageId}/reactions | Add reaction to message
[**ChatCreate**](ChatAPI.md#ChatCreate) | **Post** /api/chat/projects/{projectId}/chats | Create new chat
[**ChatDeleteMessage**](ChatAPI.md#ChatDeleteMessage) | **Delete** /api/chat/projects/{projectId}/chats/{chatId}/messages/{messageId} | Delete message
[**ChatEditMessage**](ChatAPI.md#ChatEditMessage) | **Patch** /api/chat/projects/{projectId}/chats/{chatId}/messages/{messageId} | Edit message
[**ChatGet**](ChatAPI.md#ChatGet) | **Get** /api/chat/projects/{projectId}/chats/{chatId} | Get chat details
[**ChatGetChatE2eeParticipantKeys**](ChatAPI.md#ChatGetChatE2eeParticipantKeys) | **Get** /api/chat/projects/{projectId}/chats/{chatId}/e2ee/participant-keys | List participant E2EE public keys
[**ChatGetMessages**](ChatAPI.md#ChatGetMessages) | **Get** /api/chat/projects/{projectId}/chats/{chatId}/messages | Get chat messages
[**ChatList**](ChatAPI.md#ChatList) | **Get** /api/chat/projects/{projectId}/chats | Get user chats
[**ChatMarkAsRead**](ChatAPI.md#ChatMarkAsRead) | **Post** /api/chat/projects/{projectId}/chats/{chatId}/messages/read | Mark messages as read
[**ChatPutChatE2eeKey**](ChatAPI.md#ChatPutChatE2eeKey) | **Put** /api/chat/projects/{projectId}/me/chat-e2ee-key | Register chat E2EE identity public key
[**ChatRemoveParticipant**](ChatAPI.md#ChatRemoveParticipant) | **Delete** /api/chat/projects/{projectId}/chats/{chatId}/participants | Remove participant from chat
[**ChatRemoveReaction**](ChatAPI.md#ChatRemoveReaction) | **Delete** /api/chat/projects/{projectId}/chats/{chatId}/messages/{messageId}/reactions | Remove reaction from message
[**ChatSendMessage**](ChatAPI.md#ChatSendMessage) | **Post** /api/chat/projects/{projectId}/chats/{chatId}/messages | Send message



## ChatAddParticipant

> ChatAddParticipant200Response ChatAddParticipant(ctx, projectId, chatId).ChatAddParticipantRequest(chatAddParticipantRequest).Execute()

Add participant to chat



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
	chatId := "chatId_example" // string | Chat ID.
	chatAddParticipantRequest := *openapiclient.NewChatAddParticipantRequest("UserId_example") // ChatAddParticipantRequest | User ID to add and optional role (admin, member).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatAddParticipant(context.Background(), projectId, chatId).ChatAddParticipantRequest(chatAddParticipantRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatAddParticipant``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatAddParticipant`: ChatAddParticipant200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatAddParticipant`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatAddParticipantRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **chatAddParticipantRequest** | [**ChatAddParticipantRequest**](ChatAddParticipantRequest.md) | User ID to add and optional role (admin, member). | 

### Return type

[**ChatAddParticipant200Response**](ChatAddParticipant200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatAddReaction

> ChatAddReaction200Response ChatAddReaction(ctx, projectId, chatId, messageId).ChatAddReactionRequest(chatAddReactionRequest).Execute()

Add reaction to message



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
	chatId := "chatId_example" // string | Chat ID.
	messageId := "messageId_example" // string | Message ID.
	chatAddReactionRequest := *openapiclient.NewChatAddReactionRequest("Emoji_example") // ChatAddReactionRequest | Emoji reaction (e.g. 👍, ❤️).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatAddReaction(context.Background(), projectId, chatId, messageId).ChatAddReactionRequest(chatAddReactionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatAddReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatAddReaction`: ChatAddReaction200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatAddReaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 
**messageId** | **string** | Message ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatAddReactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **chatAddReactionRequest** | [**ChatAddReactionRequest**](ChatAddReactionRequest.md) | Emoji reaction (e.g. 👍, ❤️). | 

### Return type

[**ChatAddReaction200Response**](ChatAddReaction200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatCreate

> ChatCreate201Response ChatCreate(ctx, projectId).ChatCreateRequest(chatCreateRequest).Execute()

Create new chat



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
	chatCreateRequest := *openapiclient.NewChatCreateRequest("Name_example", "Type_example", []string{"Participants_example"}) // ChatCreateRequest | Chat name, type (direct/group/channel/broadcast), participants array, optional description and settings.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatCreate(context.Background(), projectId).ChatCreateRequest(chatCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatCreate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatCreate`: ChatCreate201Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatCreate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatCreateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **chatCreateRequest** | [**ChatCreateRequest**](ChatCreateRequest.md) | Chat name, type (direct/group/channel/broadcast), participants array, optional description and settings. | 

### Return type

[**ChatCreate201Response**](ChatCreate201Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatDeleteMessage

> MessageResponse ChatDeleteMessage(ctx, projectId, chatId, messageId).Execute()

Delete message



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
	chatId := "chatId_example" // string | Chat ID.
	messageId := "messageId_example" // string | Message ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatDeleteMessage(context.Background(), projectId, chatId, messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatDeleteMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatDeleteMessage`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatDeleteMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 
**messageId** | **string** | Message ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatDeleteMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatEditMessage

> ChatEditMessage200Response ChatEditMessage(ctx, projectId, chatId, messageId).ChatEditMessageRequest(chatEditMessageRequest).Execute()

Edit message



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
	chatId := "chatId_example" // string | Chat ID.
	messageId := "messageId_example" // string | Message ID.
	chatEditMessageRequest := *openapiclient.NewChatEditMessageRequest() // ChatEditMessageRequest | New plaintext content (non-E2EE messages) or new e2ee ciphertext (E2EE messages). One of content or e2ee.ciphertext is required.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatEditMessage(context.Background(), projectId, chatId, messageId).ChatEditMessageRequest(chatEditMessageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatEditMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatEditMessage`: ChatEditMessage200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatEditMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 
**messageId** | **string** | Message ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatEditMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **chatEditMessageRequest** | [**ChatEditMessageRequest**](ChatEditMessageRequest.md) | New plaintext content (non-E2EE messages) or new e2ee ciphertext (E2EE messages). One of content or e2ee.ciphertext is required. | 

### Return type

[**ChatEditMessage200Response**](ChatEditMessage200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatGet

> ChatGet200Response ChatGet(ctx, projectId, chatId).Execute()

Get chat details



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
	chatId := "chatId_example" // string | Chat ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatGet(context.Background(), projectId, chatId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatGet`: ChatGet200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ChatGet200Response**](ChatGet200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatGetChatE2eeParticipantKeys

> ChatGetChatE2eeParticipantKeys200Response ChatGetChatE2eeParticipantKeys(ctx, projectId, chatId).Execute()

List participant E2EE public keys



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
	chatId := "chatId_example" // string | Chat ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatGetChatE2eeParticipantKeys(context.Background(), projectId, chatId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatGetChatE2eeParticipantKeys``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatGetChatE2eeParticipantKeys`: ChatGetChatE2eeParticipantKeys200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatGetChatE2eeParticipantKeys`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatGetChatE2eeParticipantKeysRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ChatGetChatE2eeParticipantKeys200Response**](ChatGetChatE2eeParticipantKeys200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatGetMessages

> ChatGetMessages200Response ChatGetMessages(ctx, projectId, chatId).Page(page).Limit(limit).Before(before).After(after).Execute()

Get chat messages



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
	projectId := "projectId_example" // string | Project ID.
	chatId := "chatId_example" // string | Chat ID.
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Number of messages per page. (optional) (default to 50)
	before := time.Now() // time.Time | Return messages before this timestamp (cursor). (optional)
	after := time.Now() // time.Time | Return messages after this timestamp (cursor). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatGetMessages(context.Background(), projectId, chatId).Page(page).Limit(limit).Before(before).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatGetMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatGetMessages`: ChatGetMessages200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatGetMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatGetMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of messages per page. | [default to 50]
 **before** | **time.Time** | Return messages before this timestamp (cursor). | 
 **after** | **time.Time** | Return messages after this timestamp (cursor). | 

### Return type

[**ChatGetMessages200Response**](ChatGetMessages200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatList

> ChatList200Response ChatList(ctx, projectId).Page(page).Limit(limit).Execute()

Get user chats



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
	limit := int32(56) // int32 | Number of chats per page. (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatList(context.Background(), projectId).Page(page).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatList`: ChatList200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of chats per page. | [default to 20]

### Return type

[**ChatList200Response**](ChatList200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatMarkAsRead

> ChatMarkAsRead200Response ChatMarkAsRead(ctx, projectId, chatId).ChatMarkAsReadRequest(chatMarkAsReadRequest).Execute()

Mark messages as read



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
	chatId := "chatId_example" // string | Chat ID.
	chatMarkAsReadRequest := *openapiclient.NewChatMarkAsReadRequest([]string{"MessageIds_example"}) // ChatMarkAsReadRequest | Array of message IDs to mark as read.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatMarkAsRead(context.Background(), projectId, chatId).ChatMarkAsReadRequest(chatMarkAsReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatMarkAsRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatMarkAsRead`: ChatMarkAsRead200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatMarkAsRead`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatMarkAsReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **chatMarkAsReadRequest** | [**ChatMarkAsReadRequest**](ChatMarkAsReadRequest.md) | Array of message IDs to mark as read. | 

### Return type

[**ChatMarkAsRead200Response**](ChatMarkAsRead200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatPutChatE2eeKey

> ChatPutChatE2eeKey200Response ChatPutChatE2eeKey(ctx, projectId).ChatPutChatE2eeKeyRequest(chatPutChatE2eeKeyRequest).Execute()

Register chat E2EE identity public key



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
	chatPutChatE2eeKeyRequest := *openapiclient.NewChatPutChatE2eeKeyRequest("IdentityPublicKey_example") // ChatPutChatE2eeKeyRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatPutChatE2eeKey(context.Background(), projectId).ChatPutChatE2eeKeyRequest(chatPutChatE2eeKeyRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatPutChatE2eeKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatPutChatE2eeKey`: ChatPutChatE2eeKey200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatPutChatE2eeKey`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatPutChatE2eeKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **chatPutChatE2eeKeyRequest** | [**ChatPutChatE2eeKeyRequest**](ChatPutChatE2eeKeyRequest.md) |  | 

### Return type

[**ChatPutChatE2eeKey200Response**](ChatPutChatE2eeKey200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatRemoveParticipant

> MessageResponse ChatRemoveParticipant(ctx, projectId, chatId).ChatRemoveParticipantRequest(chatRemoveParticipantRequest).Execute()

Remove participant from chat



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
	chatId := "chatId_example" // string | Chat ID.
	chatRemoveParticipantRequest := *openapiclient.NewChatRemoveParticipantRequest("UserId_example") // ChatRemoveParticipantRequest | User ID of the participant to remove.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatRemoveParticipant(context.Background(), projectId, chatId).ChatRemoveParticipantRequest(chatRemoveParticipantRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatRemoveParticipant``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatRemoveParticipant`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatRemoveParticipant`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatRemoveParticipantRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **chatRemoveParticipantRequest** | [**ChatRemoveParticipantRequest**](ChatRemoveParticipantRequest.md) | User ID of the participant to remove. | 

### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatRemoveReaction

> ChatRemoveReaction200Response ChatRemoveReaction(ctx, projectId, chatId, messageId).ChatAddReactionRequest(chatAddReactionRequest).Execute()

Remove reaction from message



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
	chatId := "chatId_example" // string | Chat ID.
	messageId := "messageId_example" // string | Message ID.
	chatAddReactionRequest := *openapiclient.NewChatAddReactionRequest("Emoji_example") // ChatAddReactionRequest | Emoji to remove (must match the reaction added by the user).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatRemoveReaction(context.Background(), projectId, chatId, messageId).ChatAddReactionRequest(chatAddReactionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatRemoveReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatRemoveReaction`: ChatRemoveReaction200Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatRemoveReaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 
**messageId** | **string** | Message ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatRemoveReactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **chatAddReactionRequest** | [**ChatAddReactionRequest**](ChatAddReactionRequest.md) | Emoji to remove (must match the reaction added by the user). | 

### Return type

[**ChatRemoveReaction200Response**](ChatRemoveReaction200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ChatSendMessage

> ChatSendMessage201Response ChatSendMessage(ctx, projectId, chatId).ChatSendMessageRequest(chatSendMessageRequest).Execute()

Send message



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
	chatId := "chatId_example" // string | Chat ID.
	chatSendMessageRequest := *openapiclient.NewChatSendMessageRequest("Type_example") // ChatSendMessageRequest | Message type and content, or E2EE ciphertext for text messages. Plaintext requires content; E2EE requires type=text and e2ee.ciphertext (omit plaintext content).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatAPI.ChatSendMessage(context.Background(), projectId, chatId).ChatSendMessageRequest(chatSendMessageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatAPI.ChatSendMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatSendMessage`: ChatSendMessage201Response
	fmt.Fprintf(os.Stdout, "Response from `ChatAPI.ChatSendMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**chatId** | **string** | Chat ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiChatSendMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **chatSendMessageRequest** | [**ChatSendMessageRequest**](ChatSendMessageRequest.md) | Message type and content, or E2EE ciphertext for text messages. Plaintext requires content; E2EE requires type&#x3D;text and e2ee.ciphertext (omit plaintext content). | 

### Return type

[**ChatSendMessage201Response**](ChatSendMessage201Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


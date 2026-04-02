# ChatSendMessageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Content** | Pointer to **string** | Plaintext body; omit when sending e2ee (use e2ee.ciphertext for E2EE text). | [optional] 
**E2ee** | Pointer to [**ChatSendMessageRequestE2ee**](ChatSendMessageRequestE2ee.md) |  | [optional] 
**ReplyTo** | Pointer to **string** |  | [optional] 
**Mentions** | Pointer to **[]string** |  | [optional] 

## Methods

### NewChatSendMessageRequest

`func NewChatSendMessageRequest(type_ string, ) *ChatSendMessageRequest`

NewChatSendMessageRequest instantiates a new ChatSendMessageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatSendMessageRequestWithDefaults

`func NewChatSendMessageRequestWithDefaults() *ChatSendMessageRequest`

NewChatSendMessageRequestWithDefaults instantiates a new ChatSendMessageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ChatSendMessageRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ChatSendMessageRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ChatSendMessageRequest) SetType(v string)`

SetType sets Type field to given value.


### GetContent

`func (o *ChatSendMessageRequest) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *ChatSendMessageRequest) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *ChatSendMessageRequest) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *ChatSendMessageRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetE2ee

`func (o *ChatSendMessageRequest) GetE2ee() ChatSendMessageRequestE2ee`

GetE2ee returns the E2ee field if non-nil, zero value otherwise.

### GetE2eeOk

`func (o *ChatSendMessageRequest) GetE2eeOk() (*ChatSendMessageRequestE2ee, bool)`

GetE2eeOk returns a tuple with the E2ee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetE2ee

`func (o *ChatSendMessageRequest) SetE2ee(v ChatSendMessageRequestE2ee)`

SetE2ee sets E2ee field to given value.

### HasE2ee

`func (o *ChatSendMessageRequest) HasE2ee() bool`

HasE2ee returns a boolean if a field has been set.

### GetReplyTo

`func (o *ChatSendMessageRequest) GetReplyTo() string`

GetReplyTo returns the ReplyTo field if non-nil, zero value otherwise.

### GetReplyToOk

`func (o *ChatSendMessageRequest) GetReplyToOk() (*string, bool)`

GetReplyToOk returns a tuple with the ReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplyTo

`func (o *ChatSendMessageRequest) SetReplyTo(v string)`

SetReplyTo sets ReplyTo field to given value.

### HasReplyTo

`func (o *ChatSendMessageRequest) HasReplyTo() bool`

HasReplyTo returns a boolean if a field has been set.

### GetMentions

`func (o *ChatSendMessageRequest) GetMentions() []string`

GetMentions returns the Mentions field if non-nil, zero value otherwise.

### GetMentionsOk

`func (o *ChatSendMessageRequest) GetMentionsOk() (*[]string, bool)`

GetMentionsOk returns a tuple with the Mentions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMentions

`func (o *ChatSendMessageRequest) SetMentions(v []string)`

SetMentions sets Mentions field to given value.

### HasMentions

`func (o *ChatSendMessageRequest) HasMentions() bool`

HasMentions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



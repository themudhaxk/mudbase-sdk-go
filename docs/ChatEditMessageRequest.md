# ChatEditMessageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Content** | Pointer to **string** | New plaintext (non-E2EE messages only). | [optional] 
**E2ee** | Pointer to [**ChatEditMessageRequestE2ee**](ChatEditMessageRequestE2ee.md) |  | [optional] 

## Methods

### NewChatEditMessageRequest

`func NewChatEditMessageRequest() *ChatEditMessageRequest`

NewChatEditMessageRequest instantiates a new ChatEditMessageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatEditMessageRequestWithDefaults

`func NewChatEditMessageRequestWithDefaults() *ChatEditMessageRequest`

NewChatEditMessageRequestWithDefaults instantiates a new ChatEditMessageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetContent

`func (o *ChatEditMessageRequest) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *ChatEditMessageRequest) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *ChatEditMessageRequest) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *ChatEditMessageRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetE2ee

`func (o *ChatEditMessageRequest) GetE2ee() ChatEditMessageRequestE2ee`

GetE2ee returns the E2ee field if non-nil, zero value otherwise.

### GetE2eeOk

`func (o *ChatEditMessageRequest) GetE2eeOk() (*ChatEditMessageRequestE2ee, bool)`

GetE2eeOk returns a tuple with the E2ee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetE2ee

`func (o *ChatEditMessageRequest) SetE2ee(v ChatEditMessageRequestE2ee)`

SetE2ee sets E2ee field to given value.

### HasE2ee

`func (o *ChatEditMessageRequest) HasE2ee() bool`

HasE2ee returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



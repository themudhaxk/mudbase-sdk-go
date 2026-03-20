# ChatGetMessages200ResponseDataMessagesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Content** | Pointer to **string** |  | [optional] 
**Sender** | Pointer to [**ChatGetMessages200ResponseDataMessagesInnerSender**](ChatGetMessages200ResponseDataMessagesInnerSender.md) |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewChatGetMessages200ResponseDataMessagesInner

`func NewChatGetMessages200ResponseDataMessagesInner() *ChatGetMessages200ResponseDataMessagesInner`

NewChatGetMessages200ResponseDataMessagesInner instantiates a new ChatGetMessages200ResponseDataMessagesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatGetMessages200ResponseDataMessagesInnerWithDefaults

`func NewChatGetMessages200ResponseDataMessagesInnerWithDefaults() *ChatGetMessages200ResponseDataMessagesInner`

NewChatGetMessages200ResponseDataMessagesInnerWithDefaults instantiates a new ChatGetMessages200ResponseDataMessagesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ChatGetMessages200ResponseDataMessagesInner) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ChatGetMessages200ResponseDataMessagesInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetContent

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *ChatGetMessages200ResponseDataMessagesInner) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *ChatGetMessages200ResponseDataMessagesInner) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetSender

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetSender() ChatGetMessages200ResponseDataMessagesInnerSender`

GetSender returns the Sender field if non-nil, zero value otherwise.

### GetSenderOk

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetSenderOk() (*ChatGetMessages200ResponseDataMessagesInnerSender, bool)`

GetSenderOk returns a tuple with the Sender field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSender

`func (o *ChatGetMessages200ResponseDataMessagesInner) SetSender(v ChatGetMessages200ResponseDataMessagesInnerSender)`

SetSender sets Sender field to given value.

### HasSender

`func (o *ChatGetMessages200ResponseDataMessagesInner) HasSender() bool`

HasSender returns a boolean if a field has been set.

### GetCreatedAt

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ChatGetMessages200ResponseDataMessagesInner) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ChatGetMessages200ResponseDataMessagesInner) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ChatGetMessages200ResponseDataMessagesInner) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



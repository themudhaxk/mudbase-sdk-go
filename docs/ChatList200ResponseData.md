# ChatList200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Chats** | Pointer to [**[]ChatList200ResponseDataChatsInner**](ChatList200ResponseDataChatsInner.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewChatList200ResponseData

`func NewChatList200ResponseData() *ChatList200ResponseData`

NewChatList200ResponseData instantiates a new ChatList200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatList200ResponseDataWithDefaults

`func NewChatList200ResponseDataWithDefaults() *ChatList200ResponseData`

NewChatList200ResponseDataWithDefaults instantiates a new ChatList200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChats

`func (o *ChatList200ResponseData) GetChats() []ChatList200ResponseDataChatsInner`

GetChats returns the Chats field if non-nil, zero value otherwise.

### GetChatsOk

`func (o *ChatList200ResponseData) GetChatsOk() (*[]ChatList200ResponseDataChatsInner, bool)`

GetChatsOk returns a tuple with the Chats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChats

`func (o *ChatList200ResponseData) SetChats(v []ChatList200ResponseDataChatsInner)`

SetChats sets Chats field to given value.

### HasChats

`func (o *ChatList200ResponseData) HasChats() bool`

HasChats returns a boolean if a field has been set.

### GetTotal

`func (o *ChatList200ResponseData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ChatList200ResponseData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ChatList200ResponseData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ChatList200ResponseData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ChatGetMessages200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Messages** | Pointer to [**[]ChatGetMessages200ResponseDataMessagesInner**](ChatGetMessages200ResponseDataMessagesInner.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewChatGetMessages200ResponseData

`func NewChatGetMessages200ResponseData() *ChatGetMessages200ResponseData`

NewChatGetMessages200ResponseData instantiates a new ChatGetMessages200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatGetMessages200ResponseDataWithDefaults

`func NewChatGetMessages200ResponseDataWithDefaults() *ChatGetMessages200ResponseData`

NewChatGetMessages200ResponseDataWithDefaults instantiates a new ChatGetMessages200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessages

`func (o *ChatGetMessages200ResponseData) GetMessages() []ChatGetMessages200ResponseDataMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *ChatGetMessages200ResponseData) GetMessagesOk() (*[]ChatGetMessages200ResponseDataMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *ChatGetMessages200ResponseData) SetMessages(v []ChatGetMessages200ResponseDataMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *ChatGetMessages200ResponseData) HasMessages() bool`

HasMessages returns a boolean if a field has been set.

### GetTotal

`func (o *ChatGetMessages200ResponseData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ChatGetMessages200ResponseData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ChatGetMessages200ResponseData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ChatGetMessages200ResponseData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



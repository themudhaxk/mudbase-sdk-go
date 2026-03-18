# ChatSendMessage201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**ChatSendMessage201ResponseData**](ChatSendMessage201ResponseData.md) |  | [optional] 

## Methods

### NewChatSendMessage201Response

`func NewChatSendMessage201Response() *ChatSendMessage201Response`

NewChatSendMessage201Response instantiates a new ChatSendMessage201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatSendMessage201ResponseWithDefaults

`func NewChatSendMessage201ResponseWithDefaults() *ChatSendMessage201Response`

NewChatSendMessage201ResponseWithDefaults instantiates a new ChatSendMessage201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *ChatSendMessage201Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *ChatSendMessage201Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *ChatSendMessage201Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *ChatSendMessage201Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *ChatSendMessage201Response) GetData() ChatSendMessage201ResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ChatSendMessage201Response) GetDataOk() (*ChatSendMessage201ResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ChatSendMessage201Response) SetData(v ChatSendMessage201ResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *ChatSendMessage201Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



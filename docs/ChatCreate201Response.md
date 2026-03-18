# ChatCreate201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**ChatCreate201ResponseData**](ChatCreate201ResponseData.md) |  | [optional] 

## Methods

### NewChatCreate201Response

`func NewChatCreate201Response() *ChatCreate201Response`

NewChatCreate201Response instantiates a new ChatCreate201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatCreate201ResponseWithDefaults

`func NewChatCreate201ResponseWithDefaults() *ChatCreate201Response`

NewChatCreate201ResponseWithDefaults instantiates a new ChatCreate201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *ChatCreate201Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *ChatCreate201Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *ChatCreate201Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *ChatCreate201Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *ChatCreate201Response) GetData() ChatCreate201ResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ChatCreate201Response) GetDataOk() (*ChatCreate201ResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ChatCreate201Response) SetData(v ChatCreate201ResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *ChatCreate201Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



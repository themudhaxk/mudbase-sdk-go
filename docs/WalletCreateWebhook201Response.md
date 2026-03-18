# WalletCreateWebhook201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Data** | Pointer to [**WalletWebhook**](WalletWebhook.md) |  | [optional] 

## Methods

### NewWalletCreateWebhook201Response

`func NewWalletCreateWebhook201Response() *WalletCreateWebhook201Response`

NewWalletCreateWebhook201Response instantiates a new WalletCreateWebhook201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletCreateWebhook201ResponseWithDefaults

`func NewWalletCreateWebhook201ResponseWithDefaults() *WalletCreateWebhook201Response`

NewWalletCreateWebhook201ResponseWithDefaults instantiates a new WalletCreateWebhook201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WalletCreateWebhook201Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WalletCreateWebhook201Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WalletCreateWebhook201Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WalletCreateWebhook201Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetMessage

`func (o *WalletCreateWebhook201Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WalletCreateWebhook201Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WalletCreateWebhook201Response) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *WalletCreateWebhook201Response) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetData

`func (o *WalletCreateWebhook201Response) GetData() WalletWebhook`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletCreateWebhook201Response) GetDataOk() (*WalletWebhook, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletCreateWebhook201Response) SetData(v WalletWebhook)`

SetData sets Data field to given value.

### HasData

`func (o *WalletCreateWebhook201Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



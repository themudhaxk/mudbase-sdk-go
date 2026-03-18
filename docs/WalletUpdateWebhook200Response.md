# WalletUpdateWebhook200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WalletWebhook**](WalletWebhook.md) |  | [optional] 

## Methods

### NewWalletUpdateWebhook200Response

`func NewWalletUpdateWebhook200Response() *WalletUpdateWebhook200Response`

NewWalletUpdateWebhook200Response instantiates a new WalletUpdateWebhook200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletUpdateWebhook200ResponseWithDefaults

`func NewWalletUpdateWebhook200ResponseWithDefaults() *WalletUpdateWebhook200Response`

NewWalletUpdateWebhook200ResponseWithDefaults instantiates a new WalletUpdateWebhook200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WalletUpdateWebhook200Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WalletUpdateWebhook200Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WalletUpdateWebhook200Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WalletUpdateWebhook200Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WalletUpdateWebhook200Response) GetData() WalletWebhook`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletUpdateWebhook200Response) GetDataOk() (*WalletWebhook, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletUpdateWebhook200Response) SetData(v WalletWebhook)`

SetData sets Data field to given value.

### HasData

`func (o *WalletUpdateWebhook200Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



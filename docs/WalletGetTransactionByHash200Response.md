# WalletGetTransactionByHash200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WalletTransaction**](WalletTransaction.md) |  | [optional] 

## Methods

### NewWalletGetTransactionByHash200Response

`func NewWalletGetTransactionByHash200Response() *WalletGetTransactionByHash200Response`

NewWalletGetTransactionByHash200Response instantiates a new WalletGetTransactionByHash200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletGetTransactionByHash200ResponseWithDefaults

`func NewWalletGetTransactionByHash200ResponseWithDefaults() *WalletGetTransactionByHash200Response`

NewWalletGetTransactionByHash200ResponseWithDefaults instantiates a new WalletGetTransactionByHash200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WalletGetTransactionByHash200Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WalletGetTransactionByHash200Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WalletGetTransactionByHash200Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WalletGetTransactionByHash200Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WalletGetTransactionByHash200Response) GetData() WalletTransaction`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletGetTransactionByHash200Response) GetDataOk() (*WalletTransaction, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletGetTransactionByHash200Response) SetData(v WalletTransaction)`

SetData sets Data field to given value.

### HasData

`func (o *WalletGetTransactionByHash200Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



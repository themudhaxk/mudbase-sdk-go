# WalletGetSpeedUpParamsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TxId** | Pointer to **string** | WalletTransaction _id (MongoDB ObjectId) | [optional] 
**TxHash** | Pointer to **string** | mainTxHash or txHash of the stuck transaction | [optional] 
**Chain** | **string** | EVM chain (speed-up is EVM only) | 

## Methods

### NewWalletGetSpeedUpParamsRequest

`func NewWalletGetSpeedUpParamsRequest(chain string, ) *WalletGetSpeedUpParamsRequest`

NewWalletGetSpeedUpParamsRequest instantiates a new WalletGetSpeedUpParamsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletGetSpeedUpParamsRequestWithDefaults

`func NewWalletGetSpeedUpParamsRequestWithDefaults() *WalletGetSpeedUpParamsRequest`

NewWalletGetSpeedUpParamsRequestWithDefaults instantiates a new WalletGetSpeedUpParamsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTxId

`func (o *WalletGetSpeedUpParamsRequest) GetTxId() string`

GetTxId returns the TxId field if non-nil, zero value otherwise.

### GetTxIdOk

`func (o *WalletGetSpeedUpParamsRequest) GetTxIdOk() (*string, bool)`

GetTxIdOk returns a tuple with the TxId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxId

`func (o *WalletGetSpeedUpParamsRequest) SetTxId(v string)`

SetTxId sets TxId field to given value.

### HasTxId

`func (o *WalletGetSpeedUpParamsRequest) HasTxId() bool`

HasTxId returns a boolean if a field has been set.

### GetTxHash

`func (o *WalletGetSpeedUpParamsRequest) GetTxHash() string`

GetTxHash returns the TxHash field if non-nil, zero value otherwise.

### GetTxHashOk

`func (o *WalletGetSpeedUpParamsRequest) GetTxHashOk() (*string, bool)`

GetTxHashOk returns a tuple with the TxHash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxHash

`func (o *WalletGetSpeedUpParamsRequest) SetTxHash(v string)`

SetTxHash sets TxHash field to given value.

### HasTxHash

`func (o *WalletGetSpeedUpParamsRequest) HasTxHash() bool`

HasTxHash returns a boolean if a field has been set.

### GetChain

`func (o *WalletGetSpeedUpParamsRequest) GetChain() string`

GetChain returns the Chain field if non-nil, zero value otherwise.

### GetChainOk

`func (o *WalletGetSpeedUpParamsRequest) GetChainOk() (*string, bool)`

GetChainOk returns a tuple with the Chain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChain

`func (o *WalletGetSpeedUpParamsRequest) SetChain(v string)`

SetChain sets Chain field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



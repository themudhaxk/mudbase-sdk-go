# WalletGetCancelParamsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TxId** | Pointer to **string** | WalletTransaction _id | [optional] 
**TxHash** | Pointer to **string** | mainTxHash or txHash of the stuck transaction | [optional] 
**Chain** | **string** |  | 

## Methods

### NewWalletGetCancelParamsRequest

`func NewWalletGetCancelParamsRequest(chain string, ) *WalletGetCancelParamsRequest`

NewWalletGetCancelParamsRequest instantiates a new WalletGetCancelParamsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletGetCancelParamsRequestWithDefaults

`func NewWalletGetCancelParamsRequestWithDefaults() *WalletGetCancelParamsRequest`

NewWalletGetCancelParamsRequestWithDefaults instantiates a new WalletGetCancelParamsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTxId

`func (o *WalletGetCancelParamsRequest) GetTxId() string`

GetTxId returns the TxId field if non-nil, zero value otherwise.

### GetTxIdOk

`func (o *WalletGetCancelParamsRequest) GetTxIdOk() (*string, bool)`

GetTxIdOk returns a tuple with the TxId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxId

`func (o *WalletGetCancelParamsRequest) SetTxId(v string)`

SetTxId sets TxId field to given value.

### HasTxId

`func (o *WalletGetCancelParamsRequest) HasTxId() bool`

HasTxId returns a boolean if a field has been set.

### GetTxHash

`func (o *WalletGetCancelParamsRequest) GetTxHash() string`

GetTxHash returns the TxHash field if non-nil, zero value otherwise.

### GetTxHashOk

`func (o *WalletGetCancelParamsRequest) GetTxHashOk() (*string, bool)`

GetTxHashOk returns a tuple with the TxHash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxHash

`func (o *WalletGetCancelParamsRequest) SetTxHash(v string)`

SetTxHash sets TxHash field to given value.

### HasTxHash

`func (o *WalletGetCancelParamsRequest) HasTxHash() bool`

HasTxHash returns a boolean if a field has been set.

### GetChain

`func (o *WalletGetCancelParamsRequest) GetChain() string`

GetChain returns the Chain field if non-nil, zero value otherwise.

### GetChainOk

`func (o *WalletGetCancelParamsRequest) GetChainOk() (*string, bool)`

GetChainOk returns a tuple with the Chain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChain

`func (o *WalletGetCancelParamsRequest) SetChain(v string)`

SetChain sets Chain field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



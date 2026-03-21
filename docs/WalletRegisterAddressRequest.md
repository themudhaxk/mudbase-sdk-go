# WalletRegisterAddressRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Address** | **string** | Public wallet address | 
**Chain** | **string** | Blockchain network (EVM, UTXO, or chain-specific). Use bsc or binance for BNB Smart Chain; avalanche for Avalanche C-Chain. | 
**DerivationPath** | Pointer to **string** | HD wallet derivation path (metadata only) | [optional] 
**Label** | Pointer to **string** | Optional label for the address | [optional] 
**ProjectId** | Pointer to **string** | Optional project ID | [optional] 

## Methods

### NewWalletRegisterAddressRequest

`func NewWalletRegisterAddressRequest(address string, chain string, ) *WalletRegisterAddressRequest`

NewWalletRegisterAddressRequest instantiates a new WalletRegisterAddressRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletRegisterAddressRequestWithDefaults

`func NewWalletRegisterAddressRequestWithDefaults() *WalletRegisterAddressRequest`

NewWalletRegisterAddressRequestWithDefaults instantiates a new WalletRegisterAddressRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddress

`func (o *WalletRegisterAddressRequest) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *WalletRegisterAddressRequest) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *WalletRegisterAddressRequest) SetAddress(v string)`

SetAddress sets Address field to given value.


### GetChain

`func (o *WalletRegisterAddressRequest) GetChain() string`

GetChain returns the Chain field if non-nil, zero value otherwise.

### GetChainOk

`func (o *WalletRegisterAddressRequest) GetChainOk() (*string, bool)`

GetChainOk returns a tuple with the Chain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChain

`func (o *WalletRegisterAddressRequest) SetChain(v string)`

SetChain sets Chain field to given value.


### GetDerivationPath

`func (o *WalletRegisterAddressRequest) GetDerivationPath() string`

GetDerivationPath returns the DerivationPath field if non-nil, zero value otherwise.

### GetDerivationPathOk

`func (o *WalletRegisterAddressRequest) GetDerivationPathOk() (*string, bool)`

GetDerivationPathOk returns a tuple with the DerivationPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDerivationPath

`func (o *WalletRegisterAddressRequest) SetDerivationPath(v string)`

SetDerivationPath sets DerivationPath field to given value.

### HasDerivationPath

`func (o *WalletRegisterAddressRequest) HasDerivationPath() bool`

HasDerivationPath returns a boolean if a field has been set.

### GetLabel

`func (o *WalletRegisterAddressRequest) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *WalletRegisterAddressRequest) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *WalletRegisterAddressRequest) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *WalletRegisterAddressRequest) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetProjectId

`func (o *WalletRegisterAddressRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *WalletRegisterAddressRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *WalletRegisterAddressRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *WalletRegisterAddressRequest) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



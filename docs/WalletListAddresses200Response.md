# WalletListAddresses200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**[]NonCustodialAddress**](NonCustodialAddress.md) |  | [optional] 
**Count** | Pointer to **int32** |  | [optional] 

## Methods

### NewWalletListAddresses200Response

`func NewWalletListAddresses200Response() *WalletListAddresses200Response`

NewWalletListAddresses200Response instantiates a new WalletListAddresses200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletListAddresses200ResponseWithDefaults

`func NewWalletListAddresses200ResponseWithDefaults() *WalletListAddresses200Response`

NewWalletListAddresses200ResponseWithDefaults instantiates a new WalletListAddresses200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WalletListAddresses200Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WalletListAddresses200Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WalletListAddresses200Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WalletListAddresses200Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WalletListAddresses200Response) GetData() []NonCustodialAddress`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletListAddresses200Response) GetDataOk() (*[]NonCustodialAddress, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletListAddresses200Response) SetData(v []NonCustodialAddress)`

SetData sets Data field to given value.

### HasData

`func (o *WalletListAddresses200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetCount

`func (o *WalletListAddresses200Response) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *WalletListAddresses200Response) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *WalletListAddresses200Response) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *WalletListAddresses200Response) HasCount() bool`

HasCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



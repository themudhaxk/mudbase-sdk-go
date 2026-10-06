# InitializePayment200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Link** | Pointer to **string** |  | [optional] 
**TxRef** | Pointer to **string** |  | [optional] 
**ProviderRef** | Pointer to **string** |  | [optional] 
**Amount** | Pointer to **float32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**OrgReceives** | Pointer to **float32** | What the org nets after the single all-in Mudbase fee. | [optional] 
**Fee** | Pointer to **float32** | The single all-in Mudbase fee, in the same currency as amount. | [optional] 
**FeeRate** | Pointer to **float32** | The effective fee rate applied (fee / amount). | [optional] 

## Methods

### NewInitializePayment200ResponseData

`func NewInitializePayment200ResponseData() *InitializePayment200ResponseData`

NewInitializePayment200ResponseData instantiates a new InitializePayment200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInitializePayment200ResponseDataWithDefaults

`func NewInitializePayment200ResponseDataWithDefaults() *InitializePayment200ResponseData`

NewInitializePayment200ResponseDataWithDefaults instantiates a new InitializePayment200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLink

`func (o *InitializePayment200ResponseData) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *InitializePayment200ResponseData) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *InitializePayment200ResponseData) SetLink(v string)`

SetLink sets Link field to given value.

### HasLink

`func (o *InitializePayment200ResponseData) HasLink() bool`

HasLink returns a boolean if a field has been set.

### GetTxRef

`func (o *InitializePayment200ResponseData) GetTxRef() string`

GetTxRef returns the TxRef field if non-nil, zero value otherwise.

### GetTxRefOk

`func (o *InitializePayment200ResponseData) GetTxRefOk() (*string, bool)`

GetTxRefOk returns a tuple with the TxRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxRef

`func (o *InitializePayment200ResponseData) SetTxRef(v string)`

SetTxRef sets TxRef field to given value.

### HasTxRef

`func (o *InitializePayment200ResponseData) HasTxRef() bool`

HasTxRef returns a boolean if a field has been set.

### GetProviderRef

`func (o *InitializePayment200ResponseData) GetProviderRef() string`

GetProviderRef returns the ProviderRef field if non-nil, zero value otherwise.

### GetProviderRefOk

`func (o *InitializePayment200ResponseData) GetProviderRefOk() (*string, bool)`

GetProviderRefOk returns a tuple with the ProviderRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviderRef

`func (o *InitializePayment200ResponseData) SetProviderRef(v string)`

SetProviderRef sets ProviderRef field to given value.

### HasProviderRef

`func (o *InitializePayment200ResponseData) HasProviderRef() bool`

HasProviderRef returns a boolean if a field has been set.

### GetAmount

`func (o *InitializePayment200ResponseData) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *InitializePayment200ResponseData) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *InitializePayment200ResponseData) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *InitializePayment200ResponseData) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *InitializePayment200ResponseData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *InitializePayment200ResponseData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *InitializePayment200ResponseData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *InitializePayment200ResponseData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetOrgReceives

`func (o *InitializePayment200ResponseData) GetOrgReceives() float32`

GetOrgReceives returns the OrgReceives field if non-nil, zero value otherwise.

### GetOrgReceivesOk

`func (o *InitializePayment200ResponseData) GetOrgReceivesOk() (*float32, bool)`

GetOrgReceivesOk returns a tuple with the OrgReceives field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrgReceives

`func (o *InitializePayment200ResponseData) SetOrgReceives(v float32)`

SetOrgReceives sets OrgReceives field to given value.

### HasOrgReceives

`func (o *InitializePayment200ResponseData) HasOrgReceives() bool`

HasOrgReceives returns a boolean if a field has been set.

### GetFee

`func (o *InitializePayment200ResponseData) GetFee() float32`

GetFee returns the Fee field if non-nil, zero value otherwise.

### GetFeeOk

`func (o *InitializePayment200ResponseData) GetFeeOk() (*float32, bool)`

GetFeeOk returns a tuple with the Fee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFee

`func (o *InitializePayment200ResponseData) SetFee(v float32)`

SetFee sets Fee field to given value.

### HasFee

`func (o *InitializePayment200ResponseData) HasFee() bool`

HasFee returns a boolean if a field has been set.

### GetFeeRate

`func (o *InitializePayment200ResponseData) GetFeeRate() float32`

GetFeeRate returns the FeeRate field if non-nil, zero value otherwise.

### GetFeeRateOk

`func (o *InitializePayment200ResponseData) GetFeeRateOk() (*float32, bool)`

GetFeeRateOk returns a tuple with the FeeRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeeRate

`func (o *InitializePayment200ResponseData) SetFeeRate(v float32)`

SetFeeRate sets FeeRate field to given value.

### HasFeeRate

`func (o *InitializePayment200ResponseData) HasFeeRate() bool`

HasFeeRate returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# GetFeeBreakdown200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amount** | Pointer to **float32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**OrgReceives** | Pointer to **float32** |  | [optional] 
**Fee** | Pointer to **float32** | The single all-in Mudbase fee. | [optional] 
**FeeRate** | Pointer to **float32** | The effective fee rate applied (fee / amount). | [optional] 

## Methods

### NewGetFeeBreakdown200ResponseData

`func NewGetFeeBreakdown200ResponseData() *GetFeeBreakdown200ResponseData`

NewGetFeeBreakdown200ResponseData instantiates a new GetFeeBreakdown200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetFeeBreakdown200ResponseDataWithDefaults

`func NewGetFeeBreakdown200ResponseDataWithDefaults() *GetFeeBreakdown200ResponseData`

NewGetFeeBreakdown200ResponseDataWithDefaults instantiates a new GetFeeBreakdown200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmount

`func (o *GetFeeBreakdown200ResponseData) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *GetFeeBreakdown200ResponseData) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *GetFeeBreakdown200ResponseData) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *GetFeeBreakdown200ResponseData) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *GetFeeBreakdown200ResponseData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *GetFeeBreakdown200ResponseData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *GetFeeBreakdown200ResponseData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *GetFeeBreakdown200ResponseData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetOrgReceives

`func (o *GetFeeBreakdown200ResponseData) GetOrgReceives() float32`

GetOrgReceives returns the OrgReceives field if non-nil, zero value otherwise.

### GetOrgReceivesOk

`func (o *GetFeeBreakdown200ResponseData) GetOrgReceivesOk() (*float32, bool)`

GetOrgReceivesOk returns a tuple with the OrgReceives field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrgReceives

`func (o *GetFeeBreakdown200ResponseData) SetOrgReceives(v float32)`

SetOrgReceives sets OrgReceives field to given value.

### HasOrgReceives

`func (o *GetFeeBreakdown200ResponseData) HasOrgReceives() bool`

HasOrgReceives returns a boolean if a field has been set.

### GetFee

`func (o *GetFeeBreakdown200ResponseData) GetFee() float32`

GetFee returns the Fee field if non-nil, zero value otherwise.

### GetFeeOk

`func (o *GetFeeBreakdown200ResponseData) GetFeeOk() (*float32, bool)`

GetFeeOk returns a tuple with the Fee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFee

`func (o *GetFeeBreakdown200ResponseData) SetFee(v float32)`

SetFee sets Fee field to given value.

### HasFee

`func (o *GetFeeBreakdown200ResponseData) HasFee() bool`

HasFee returns a boolean if a field has been set.

### GetFeeRate

`func (o *GetFeeBreakdown200ResponseData) GetFeeRate() float32`

GetFeeRate returns the FeeRate field if non-nil, zero value otherwise.

### GetFeeRateOk

`func (o *GetFeeBreakdown200ResponseData) GetFeeRateOk() (*float32, bool)`

GetFeeRateOk returns a tuple with the FeeRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeeRate

`func (o *GetFeeBreakdown200ResponseData) SetFeeRate(v float32)`

SetFeeRate sets FeeRate field to given value.

### HasFeeRate

`func (o *GetFeeBreakdown200ResponseData) HasFeeRate() bool`

HasFeeRate returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



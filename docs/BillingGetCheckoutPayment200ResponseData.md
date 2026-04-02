# BillingGetCheckoutPayment200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PaymentId** | Pointer to **string** |  | [optional] 
**PaymentAddress** | Pointer to **NullableString** |  | [optional] 
**Network** | Pointer to **NullableString** |  | [optional] 
**Asset** | Pointer to **NullableString** |  | [optional] 
**Amount** | Pointer to **float32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**TotalDue** | Pointer to **NullableString** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewBillingGetCheckoutPayment200ResponseData

`func NewBillingGetCheckoutPayment200ResponseData() *BillingGetCheckoutPayment200ResponseData`

NewBillingGetCheckoutPayment200ResponseData instantiates a new BillingGetCheckoutPayment200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingGetCheckoutPayment200ResponseDataWithDefaults

`func NewBillingGetCheckoutPayment200ResponseDataWithDefaults() *BillingGetCheckoutPayment200ResponseData`

NewBillingGetCheckoutPayment200ResponseDataWithDefaults instantiates a new BillingGetCheckoutPayment200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaymentId

`func (o *BillingGetCheckoutPayment200ResponseData) GetPaymentId() string`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetPaymentIdOk() (*string, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *BillingGetCheckoutPayment200ResponseData) SetPaymentId(v string)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *BillingGetCheckoutPayment200ResponseData) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetPaymentAddress

`func (o *BillingGetCheckoutPayment200ResponseData) GetPaymentAddress() string`

GetPaymentAddress returns the PaymentAddress field if non-nil, zero value otherwise.

### GetPaymentAddressOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetPaymentAddressOk() (*string, bool)`

GetPaymentAddressOk returns a tuple with the PaymentAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAddress

`func (o *BillingGetCheckoutPayment200ResponseData) SetPaymentAddress(v string)`

SetPaymentAddress sets PaymentAddress field to given value.

### HasPaymentAddress

`func (o *BillingGetCheckoutPayment200ResponseData) HasPaymentAddress() bool`

HasPaymentAddress returns a boolean if a field has been set.

### SetPaymentAddressNil

`func (o *BillingGetCheckoutPayment200ResponseData) SetPaymentAddressNil(b bool)`

 SetPaymentAddressNil sets the value for PaymentAddress to be an explicit nil

### UnsetPaymentAddress
`func (o *BillingGetCheckoutPayment200ResponseData) UnsetPaymentAddress()`

UnsetPaymentAddress ensures that no value is present for PaymentAddress, not even an explicit nil
### GetNetwork

`func (o *BillingGetCheckoutPayment200ResponseData) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *BillingGetCheckoutPayment200ResponseData) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *BillingGetCheckoutPayment200ResponseData) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### SetNetworkNil

`func (o *BillingGetCheckoutPayment200ResponseData) SetNetworkNil(b bool)`

 SetNetworkNil sets the value for Network to be an explicit nil

### UnsetNetwork
`func (o *BillingGetCheckoutPayment200ResponseData) UnsetNetwork()`

UnsetNetwork ensures that no value is present for Network, not even an explicit nil
### GetAsset

`func (o *BillingGetCheckoutPayment200ResponseData) GetAsset() string`

GetAsset returns the Asset field if non-nil, zero value otherwise.

### GetAssetOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetAssetOk() (*string, bool)`

GetAssetOk returns a tuple with the Asset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsset

`func (o *BillingGetCheckoutPayment200ResponseData) SetAsset(v string)`

SetAsset sets Asset field to given value.

### HasAsset

`func (o *BillingGetCheckoutPayment200ResponseData) HasAsset() bool`

HasAsset returns a boolean if a field has been set.

### SetAssetNil

`func (o *BillingGetCheckoutPayment200ResponseData) SetAssetNil(b bool)`

 SetAssetNil sets the value for Asset to be an explicit nil

### UnsetAsset
`func (o *BillingGetCheckoutPayment200ResponseData) UnsetAsset()`

UnsetAsset ensures that no value is present for Asset, not even an explicit nil
### GetAmount

`func (o *BillingGetCheckoutPayment200ResponseData) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *BillingGetCheckoutPayment200ResponseData) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *BillingGetCheckoutPayment200ResponseData) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *BillingGetCheckoutPayment200ResponseData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *BillingGetCheckoutPayment200ResponseData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *BillingGetCheckoutPayment200ResponseData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetTotalDue

`func (o *BillingGetCheckoutPayment200ResponseData) GetTotalDue() string`

GetTotalDue returns the TotalDue field if non-nil, zero value otherwise.

### GetTotalDueOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetTotalDueOk() (*string, bool)`

GetTotalDueOk returns a tuple with the TotalDue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalDue

`func (o *BillingGetCheckoutPayment200ResponseData) SetTotalDue(v string)`

SetTotalDue sets TotalDue field to given value.

### HasTotalDue

`func (o *BillingGetCheckoutPayment200ResponseData) HasTotalDue() bool`

HasTotalDue returns a boolean if a field has been set.

### SetTotalDueNil

`func (o *BillingGetCheckoutPayment200ResponseData) SetTotalDueNil(b bool)`

 SetTotalDueNil sets the value for TotalDue to be an explicit nil

### UnsetTotalDue
`func (o *BillingGetCheckoutPayment200ResponseData) UnsetTotalDue()`

UnsetTotalDue ensures that no value is present for TotalDue, not even an explicit nil
### GetStatus

`func (o *BillingGetCheckoutPayment200ResponseData) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BillingGetCheckoutPayment200ResponseData) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *BillingGetCheckoutPayment200ResponseData) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetExpiresAt

`func (o *BillingGetCheckoutPayment200ResponseData) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *BillingGetCheckoutPayment200ResponseData) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *BillingGetCheckoutPayment200ResponseData) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *BillingGetCheckoutPayment200ResponseData) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *BillingGetCheckoutPayment200ResponseData) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *BillingGetCheckoutPayment200ResponseData) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



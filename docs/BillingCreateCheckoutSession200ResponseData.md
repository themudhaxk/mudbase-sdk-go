# BillingCreateCheckoutSession200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CheckoutUrl** | Pointer to **string** | Checkout/page URL (crypto) or null when Flutterwave | [optional] 
**AuthorizationUrl** | Pointer to **string** | Flutterwave redirect URL (when Flutterwave is used) | [optional] 
**AccessCode** | Pointer to **string** | Flutterwave access code | [optional] 
**Reference** | Pointer to **string** | Payment reference (e.g. mudbase_xxx or pmt_xxx) | [optional] 
**PaymentId** | Pointer to **string** | Payment intent ID (crypto) | [optional] 
**PaymentOptions** | Pointer to [**[]BillingCreateCheckoutSession200ResponseDataPaymentOptionsInner**](BillingCreateCheckoutSession200ResponseDataPaymentOptionsInner.md) | Multi-chain payment options (crypto) | [optional] 
**PaymentAddress** | Pointer to **string** |  | [optional] 
**Network** | Pointer to **string** |  | [optional] 
**Asset** | Pointer to **string** |  | [optional] 
**Amount** | Pointer to **float32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 

## Methods

### NewBillingCreateCheckoutSession200ResponseData

`func NewBillingCreateCheckoutSession200ResponseData() *BillingCreateCheckoutSession200ResponseData`

NewBillingCreateCheckoutSession200ResponseData instantiates a new BillingCreateCheckoutSession200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingCreateCheckoutSession200ResponseDataWithDefaults

`func NewBillingCreateCheckoutSession200ResponseDataWithDefaults() *BillingCreateCheckoutSession200ResponseData`

NewBillingCreateCheckoutSession200ResponseDataWithDefaults instantiates a new BillingCreateCheckoutSession200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCheckoutUrl

`func (o *BillingCreateCheckoutSession200ResponseData) GetCheckoutUrl() string`

GetCheckoutUrl returns the CheckoutUrl field if non-nil, zero value otherwise.

### GetCheckoutUrlOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetCheckoutUrlOk() (*string, bool)`

GetCheckoutUrlOk returns a tuple with the CheckoutUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCheckoutUrl

`func (o *BillingCreateCheckoutSession200ResponseData) SetCheckoutUrl(v string)`

SetCheckoutUrl sets CheckoutUrl field to given value.

### HasCheckoutUrl

`func (o *BillingCreateCheckoutSession200ResponseData) HasCheckoutUrl() bool`

HasCheckoutUrl returns a boolean if a field has been set.

### GetAuthorizationUrl

`func (o *BillingCreateCheckoutSession200ResponseData) GetAuthorizationUrl() string`

GetAuthorizationUrl returns the AuthorizationUrl field if non-nil, zero value otherwise.

### GetAuthorizationUrlOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetAuthorizationUrlOk() (*string, bool)`

GetAuthorizationUrlOk returns a tuple with the AuthorizationUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorizationUrl

`func (o *BillingCreateCheckoutSession200ResponseData) SetAuthorizationUrl(v string)`

SetAuthorizationUrl sets AuthorizationUrl field to given value.

### HasAuthorizationUrl

`func (o *BillingCreateCheckoutSession200ResponseData) HasAuthorizationUrl() bool`

HasAuthorizationUrl returns a boolean if a field has been set.

### GetAccessCode

`func (o *BillingCreateCheckoutSession200ResponseData) GetAccessCode() string`

GetAccessCode returns the AccessCode field if non-nil, zero value otherwise.

### GetAccessCodeOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetAccessCodeOk() (*string, bool)`

GetAccessCodeOk returns a tuple with the AccessCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessCode

`func (o *BillingCreateCheckoutSession200ResponseData) SetAccessCode(v string)`

SetAccessCode sets AccessCode field to given value.

### HasAccessCode

`func (o *BillingCreateCheckoutSession200ResponseData) HasAccessCode() bool`

HasAccessCode returns a boolean if a field has been set.

### GetReference

`func (o *BillingCreateCheckoutSession200ResponseData) GetReference() string`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetReferenceOk() (*string, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *BillingCreateCheckoutSession200ResponseData) SetReference(v string)`

SetReference sets Reference field to given value.

### HasReference

`func (o *BillingCreateCheckoutSession200ResponseData) HasReference() bool`

HasReference returns a boolean if a field has been set.

### GetPaymentId

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentId() string`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentIdOk() (*string, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *BillingCreateCheckoutSession200ResponseData) SetPaymentId(v string)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *BillingCreateCheckoutSession200ResponseData) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetPaymentOptions

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentOptions() []BillingCreateCheckoutSession200ResponseDataPaymentOptionsInner`

GetPaymentOptions returns the PaymentOptions field if non-nil, zero value otherwise.

### GetPaymentOptionsOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentOptionsOk() (*[]BillingCreateCheckoutSession200ResponseDataPaymentOptionsInner, bool)`

GetPaymentOptionsOk returns a tuple with the PaymentOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentOptions

`func (o *BillingCreateCheckoutSession200ResponseData) SetPaymentOptions(v []BillingCreateCheckoutSession200ResponseDataPaymentOptionsInner)`

SetPaymentOptions sets PaymentOptions field to given value.

### HasPaymentOptions

`func (o *BillingCreateCheckoutSession200ResponseData) HasPaymentOptions() bool`

HasPaymentOptions returns a boolean if a field has been set.

### GetPaymentAddress

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentAddress() string`

GetPaymentAddress returns the PaymentAddress field if non-nil, zero value otherwise.

### GetPaymentAddressOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetPaymentAddressOk() (*string, bool)`

GetPaymentAddressOk returns a tuple with the PaymentAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAddress

`func (o *BillingCreateCheckoutSession200ResponseData) SetPaymentAddress(v string)`

SetPaymentAddress sets PaymentAddress field to given value.

### HasPaymentAddress

`func (o *BillingCreateCheckoutSession200ResponseData) HasPaymentAddress() bool`

HasPaymentAddress returns a boolean if a field has been set.

### GetNetwork

`func (o *BillingCreateCheckoutSession200ResponseData) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *BillingCreateCheckoutSession200ResponseData) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *BillingCreateCheckoutSession200ResponseData) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetAsset

`func (o *BillingCreateCheckoutSession200ResponseData) GetAsset() string`

GetAsset returns the Asset field if non-nil, zero value otherwise.

### GetAssetOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetAssetOk() (*string, bool)`

GetAssetOk returns a tuple with the Asset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsset

`func (o *BillingCreateCheckoutSession200ResponseData) SetAsset(v string)`

SetAsset sets Asset field to given value.

### HasAsset

`func (o *BillingCreateCheckoutSession200ResponseData) HasAsset() bool`

HasAsset returns a boolean if a field has been set.

### GetAmount

`func (o *BillingCreateCheckoutSession200ResponseData) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *BillingCreateCheckoutSession200ResponseData) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *BillingCreateCheckoutSession200ResponseData) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *BillingCreateCheckoutSession200ResponseData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *BillingCreateCheckoutSession200ResponseData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *BillingCreateCheckoutSession200ResponseData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *BillingCreateCheckoutSession200ResponseData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



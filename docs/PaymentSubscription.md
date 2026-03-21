# PaymentSubscription

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Merchant** | Pointer to **string** | Merchant ID | [optional] 
**Project** | Pointer to **string** | Project ID | [optional] 
**Amount** | Pointer to **float32** | Subscription amount | [optional] 
**Interval** | Pointer to **string** |  | [optional] 
**Network** | Pointer to **string** |  | [optional] 
**Token** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**NextPaymentAt** | Pointer to **time.Time** | Next payment due date | [optional] 
**GracePeriodDays** | Pointer to **int32** | Grace period in days | [optional] [default to 3]
**EarlyPaymentAllowed** | Pointer to **bool** |  | [optional] [default to true]
**LatePaymentAllowed** | Pointer to **bool** |  | [optional] [default to true]
**ProrationEnabled** | Pointer to **bool** |  | [optional] [default to false]
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewPaymentSubscription

`func NewPaymentSubscription() *PaymentSubscription`

NewPaymentSubscription instantiates a new PaymentSubscription object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentSubscriptionWithDefaults

`func NewPaymentSubscriptionWithDefaults() *PaymentSubscription`

NewPaymentSubscriptionWithDefaults instantiates a new PaymentSubscription object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PaymentSubscription) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PaymentSubscription) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PaymentSubscription) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *PaymentSubscription) HasId() bool`

HasId returns a boolean if a field has been set.

### GetMerchant

`func (o *PaymentSubscription) GetMerchant() string`

GetMerchant returns the Merchant field if non-nil, zero value otherwise.

### GetMerchantOk

`func (o *PaymentSubscription) GetMerchantOk() (*string, bool)`

GetMerchantOk returns a tuple with the Merchant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMerchant

`func (o *PaymentSubscription) SetMerchant(v string)`

SetMerchant sets Merchant field to given value.

### HasMerchant

`func (o *PaymentSubscription) HasMerchant() bool`

HasMerchant returns a boolean if a field has been set.

### GetProject

`func (o *PaymentSubscription) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *PaymentSubscription) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *PaymentSubscription) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *PaymentSubscription) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetAmount

`func (o *PaymentSubscription) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentSubscription) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentSubscription) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *PaymentSubscription) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetInterval

`func (o *PaymentSubscription) GetInterval() string`

GetInterval returns the Interval field if non-nil, zero value otherwise.

### GetIntervalOk

`func (o *PaymentSubscription) GetIntervalOk() (*string, bool)`

GetIntervalOk returns a tuple with the Interval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterval

`func (o *PaymentSubscription) SetInterval(v string)`

SetInterval sets Interval field to given value.

### HasInterval

`func (o *PaymentSubscription) HasInterval() bool`

HasInterval returns a boolean if a field has been set.

### GetNetwork

`func (o *PaymentSubscription) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *PaymentSubscription) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *PaymentSubscription) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *PaymentSubscription) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetToken

`func (o *PaymentSubscription) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *PaymentSubscription) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *PaymentSubscription) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *PaymentSubscription) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetStatus

`func (o *PaymentSubscription) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PaymentSubscription) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PaymentSubscription) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PaymentSubscription) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetNextPaymentAt

`func (o *PaymentSubscription) GetNextPaymentAt() time.Time`

GetNextPaymentAt returns the NextPaymentAt field if non-nil, zero value otherwise.

### GetNextPaymentAtOk

`func (o *PaymentSubscription) GetNextPaymentAtOk() (*time.Time, bool)`

GetNextPaymentAtOk returns a tuple with the NextPaymentAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPaymentAt

`func (o *PaymentSubscription) SetNextPaymentAt(v time.Time)`

SetNextPaymentAt sets NextPaymentAt field to given value.

### HasNextPaymentAt

`func (o *PaymentSubscription) HasNextPaymentAt() bool`

HasNextPaymentAt returns a boolean if a field has been set.

### GetGracePeriodDays

`func (o *PaymentSubscription) GetGracePeriodDays() int32`

GetGracePeriodDays returns the GracePeriodDays field if non-nil, zero value otherwise.

### GetGracePeriodDaysOk

`func (o *PaymentSubscription) GetGracePeriodDaysOk() (*int32, bool)`

GetGracePeriodDaysOk returns a tuple with the GracePeriodDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGracePeriodDays

`func (o *PaymentSubscription) SetGracePeriodDays(v int32)`

SetGracePeriodDays sets GracePeriodDays field to given value.

### HasGracePeriodDays

`func (o *PaymentSubscription) HasGracePeriodDays() bool`

HasGracePeriodDays returns a boolean if a field has been set.

### GetEarlyPaymentAllowed

`func (o *PaymentSubscription) GetEarlyPaymentAllowed() bool`

GetEarlyPaymentAllowed returns the EarlyPaymentAllowed field if non-nil, zero value otherwise.

### GetEarlyPaymentAllowedOk

`func (o *PaymentSubscription) GetEarlyPaymentAllowedOk() (*bool, bool)`

GetEarlyPaymentAllowedOk returns a tuple with the EarlyPaymentAllowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEarlyPaymentAllowed

`func (o *PaymentSubscription) SetEarlyPaymentAllowed(v bool)`

SetEarlyPaymentAllowed sets EarlyPaymentAllowed field to given value.

### HasEarlyPaymentAllowed

`func (o *PaymentSubscription) HasEarlyPaymentAllowed() bool`

HasEarlyPaymentAllowed returns a boolean if a field has been set.

### GetLatePaymentAllowed

`func (o *PaymentSubscription) GetLatePaymentAllowed() bool`

GetLatePaymentAllowed returns the LatePaymentAllowed field if non-nil, zero value otherwise.

### GetLatePaymentAllowedOk

`func (o *PaymentSubscription) GetLatePaymentAllowedOk() (*bool, bool)`

GetLatePaymentAllowedOk returns a tuple with the LatePaymentAllowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatePaymentAllowed

`func (o *PaymentSubscription) SetLatePaymentAllowed(v bool)`

SetLatePaymentAllowed sets LatePaymentAllowed field to given value.

### HasLatePaymentAllowed

`func (o *PaymentSubscription) HasLatePaymentAllowed() bool`

HasLatePaymentAllowed returns a boolean if a field has been set.

### GetProrationEnabled

`func (o *PaymentSubscription) GetProrationEnabled() bool`

GetProrationEnabled returns the ProrationEnabled field if non-nil, zero value otherwise.

### GetProrationEnabledOk

`func (o *PaymentSubscription) GetProrationEnabledOk() (*bool, bool)`

GetProrationEnabledOk returns a tuple with the ProrationEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProrationEnabled

`func (o *PaymentSubscription) SetProrationEnabled(v bool)`

SetProrationEnabled sets ProrationEnabled field to given value.

### HasProrationEnabled

`func (o *PaymentSubscription) HasProrationEnabled() bool`

HasProrationEnabled returns a boolean if a field has been set.

### GetCreatedAt

`func (o *PaymentSubscription) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PaymentSubscription) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PaymentSubscription) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *PaymentSubscription) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *PaymentSubscription) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *PaymentSubscription) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *PaymentSubscription) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *PaymentSubscription) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



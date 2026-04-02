# BillingHandleFlutterwaveWebhookRequestData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **float32** |  | [optional] 
**TxRef** | Pointer to **string** |  | [optional] 
**FlwRef** | Pointer to **string** |  | [optional] 
**Amount** | Pointer to **float32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**Customer** | Pointer to [**BillingHandleFlutterwaveWebhookRequestDataCustomer**](BillingHandleFlutterwaveWebhookRequestDataCustomer.md) |  | [optional] 
**Meta** | Pointer to **map[string]interface{}** | orgId, projectId, planId, billingCycle; or isPaymentProcessing true for fiat payment-processing | [optional] 

## Methods

### NewBillingHandleFlutterwaveWebhookRequestData

`func NewBillingHandleFlutterwaveWebhookRequestData() *BillingHandleFlutterwaveWebhookRequestData`

NewBillingHandleFlutterwaveWebhookRequestData instantiates a new BillingHandleFlutterwaveWebhookRequestData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingHandleFlutterwaveWebhookRequestDataWithDefaults

`func NewBillingHandleFlutterwaveWebhookRequestDataWithDefaults() *BillingHandleFlutterwaveWebhookRequestData`

NewBillingHandleFlutterwaveWebhookRequestDataWithDefaults instantiates a new BillingHandleFlutterwaveWebhookRequestData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetId() float32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetIdOk() (*float32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetId(v float32)`

SetId sets Id field to given value.

### HasId

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTxRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetTxRef() string`

GetTxRef returns the TxRef field if non-nil, zero value otherwise.

### GetTxRefOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetTxRefOk() (*string, bool)`

GetTxRefOk returns a tuple with the TxRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetTxRef(v string)`

SetTxRef sets TxRef field to given value.

### HasTxRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasTxRef() bool`

HasTxRef returns a boolean if a field has been set.

### GetFlwRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetFlwRef() string`

GetFlwRef returns the FlwRef field if non-nil, zero value otherwise.

### GetFlwRefOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetFlwRefOk() (*string, bool)`

GetFlwRefOk returns a tuple with the FlwRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFlwRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetFlwRef(v string)`

SetFlwRef sets FlwRef field to given value.

### HasFlwRef

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasFlwRef() bool`

HasFlwRef returns a boolean if a field has been set.

### GetAmount

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetStatus

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetCustomer

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetCustomer() BillingHandleFlutterwaveWebhookRequestDataCustomer`

GetCustomer returns the Customer field if non-nil, zero value otherwise.

### GetCustomerOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetCustomerOk() (*BillingHandleFlutterwaveWebhookRequestDataCustomer, bool)`

GetCustomerOk returns a tuple with the Customer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomer

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetCustomer(v BillingHandleFlutterwaveWebhookRequestDataCustomer)`

SetCustomer sets Customer field to given value.

### HasCustomer

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasCustomer() bool`

HasCustomer returns a boolean if a field has been set.

### GetMeta

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetMeta() map[string]interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *BillingHandleFlutterwaveWebhookRequestData) GetMetaOk() (*map[string]interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *BillingHandleFlutterwaveWebhookRequestData) SetMeta(v map[string]interface{})`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *BillingHandleFlutterwaveWebhookRequestData) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



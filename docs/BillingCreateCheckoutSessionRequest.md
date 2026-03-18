# BillingCreateCheckoutSessionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PlanId** | **string** | Plan ID to subscribe to | 
**BillingCycle** | **string** | Billing interval | 
**CustomerInfo** | [**BillingCreateCheckoutSessionRequestCustomerInfo**](BillingCreateCheckoutSessionRequestCustomerInfo.md) |  | 
**SuccessUrl** | Pointer to **string** | Redirect URL after successful payment | [optional] 
**CancelUrl** | Pointer to **string** | Redirect URL if user cancels | [optional] 

## Methods

### NewBillingCreateCheckoutSessionRequest

`func NewBillingCreateCheckoutSessionRequest(planId string, billingCycle string, customerInfo BillingCreateCheckoutSessionRequestCustomerInfo, ) *BillingCreateCheckoutSessionRequest`

NewBillingCreateCheckoutSessionRequest instantiates a new BillingCreateCheckoutSessionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingCreateCheckoutSessionRequestWithDefaults

`func NewBillingCreateCheckoutSessionRequestWithDefaults() *BillingCreateCheckoutSessionRequest`

NewBillingCreateCheckoutSessionRequestWithDefaults instantiates a new BillingCreateCheckoutSessionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPlanId

`func (o *BillingCreateCheckoutSessionRequest) GetPlanId() string`

GetPlanId returns the PlanId field if non-nil, zero value otherwise.

### GetPlanIdOk

`func (o *BillingCreateCheckoutSessionRequest) GetPlanIdOk() (*string, bool)`

GetPlanIdOk returns a tuple with the PlanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanId

`func (o *BillingCreateCheckoutSessionRequest) SetPlanId(v string)`

SetPlanId sets PlanId field to given value.


### GetBillingCycle

`func (o *BillingCreateCheckoutSessionRequest) GetBillingCycle() string`

GetBillingCycle returns the BillingCycle field if non-nil, zero value otherwise.

### GetBillingCycleOk

`func (o *BillingCreateCheckoutSessionRequest) GetBillingCycleOk() (*string, bool)`

GetBillingCycleOk returns a tuple with the BillingCycle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBillingCycle

`func (o *BillingCreateCheckoutSessionRequest) SetBillingCycle(v string)`

SetBillingCycle sets BillingCycle field to given value.


### GetCustomerInfo

`func (o *BillingCreateCheckoutSessionRequest) GetCustomerInfo() BillingCreateCheckoutSessionRequestCustomerInfo`

GetCustomerInfo returns the CustomerInfo field if non-nil, zero value otherwise.

### GetCustomerInfoOk

`func (o *BillingCreateCheckoutSessionRequest) GetCustomerInfoOk() (*BillingCreateCheckoutSessionRequestCustomerInfo, bool)`

GetCustomerInfoOk returns a tuple with the CustomerInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerInfo

`func (o *BillingCreateCheckoutSessionRequest) SetCustomerInfo(v BillingCreateCheckoutSessionRequestCustomerInfo)`

SetCustomerInfo sets CustomerInfo field to given value.


### GetSuccessUrl

`func (o *BillingCreateCheckoutSessionRequest) GetSuccessUrl() string`

GetSuccessUrl returns the SuccessUrl field if non-nil, zero value otherwise.

### GetSuccessUrlOk

`func (o *BillingCreateCheckoutSessionRequest) GetSuccessUrlOk() (*string, bool)`

GetSuccessUrlOk returns a tuple with the SuccessUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccessUrl

`func (o *BillingCreateCheckoutSessionRequest) SetSuccessUrl(v string)`

SetSuccessUrl sets SuccessUrl field to given value.

### HasSuccessUrl

`func (o *BillingCreateCheckoutSessionRequest) HasSuccessUrl() bool`

HasSuccessUrl returns a boolean if a field has been set.

### GetCancelUrl

`func (o *BillingCreateCheckoutSessionRequest) GetCancelUrl() string`

GetCancelUrl returns the CancelUrl field if non-nil, zero value otherwise.

### GetCancelUrlOk

`func (o *BillingCreateCheckoutSessionRequest) GetCancelUrlOk() (*string, bool)`

GetCancelUrlOk returns a tuple with the CancelUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelUrl

`func (o *BillingCreateCheckoutSessionRequest) SetCancelUrl(v string)`

SetCancelUrl sets CancelUrl field to given value.

### HasCancelUrl

`func (o *BillingCreateCheckoutSessionRequest) HasCancelUrl() bool`

HasCancelUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



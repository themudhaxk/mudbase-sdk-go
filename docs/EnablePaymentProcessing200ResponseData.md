# EnablePaymentProcessing200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Onboarded** | Pointer to **bool** |  | [optional] 
**AlreadyEnabled** | Pointer to **bool** |  | [optional] 
**ApprovalStatus** | Pointer to **string** | pending_review, approved, or rejected. Payments only start succeeding once this is approved, poll GET /payment-processing/status to track it. | [optional] 

## Methods

### NewEnablePaymentProcessing200ResponseData

`func NewEnablePaymentProcessing200ResponseData() *EnablePaymentProcessing200ResponseData`

NewEnablePaymentProcessing200ResponseData instantiates a new EnablePaymentProcessing200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnablePaymentProcessing200ResponseDataWithDefaults

`func NewEnablePaymentProcessing200ResponseDataWithDefaults() *EnablePaymentProcessing200ResponseData`

NewEnablePaymentProcessing200ResponseDataWithDefaults instantiates a new EnablePaymentProcessing200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOnboarded

`func (o *EnablePaymentProcessing200ResponseData) GetOnboarded() bool`

GetOnboarded returns the Onboarded field if non-nil, zero value otherwise.

### GetOnboardedOk

`func (o *EnablePaymentProcessing200ResponseData) GetOnboardedOk() (*bool, bool)`

GetOnboardedOk returns a tuple with the Onboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnboarded

`func (o *EnablePaymentProcessing200ResponseData) SetOnboarded(v bool)`

SetOnboarded sets Onboarded field to given value.

### HasOnboarded

`func (o *EnablePaymentProcessing200ResponseData) HasOnboarded() bool`

HasOnboarded returns a boolean if a field has been set.

### GetAlreadyEnabled

`func (o *EnablePaymentProcessing200ResponseData) GetAlreadyEnabled() bool`

GetAlreadyEnabled returns the AlreadyEnabled field if non-nil, zero value otherwise.

### GetAlreadyEnabledOk

`func (o *EnablePaymentProcessing200ResponseData) GetAlreadyEnabledOk() (*bool, bool)`

GetAlreadyEnabledOk returns a tuple with the AlreadyEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlreadyEnabled

`func (o *EnablePaymentProcessing200ResponseData) SetAlreadyEnabled(v bool)`

SetAlreadyEnabled sets AlreadyEnabled field to given value.

### HasAlreadyEnabled

`func (o *EnablePaymentProcessing200ResponseData) HasAlreadyEnabled() bool`

HasAlreadyEnabled returns a boolean if a field has been set.

### GetApprovalStatus

`func (o *EnablePaymentProcessing200ResponseData) GetApprovalStatus() string`

GetApprovalStatus returns the ApprovalStatus field if non-nil, zero value otherwise.

### GetApprovalStatusOk

`func (o *EnablePaymentProcessing200ResponseData) GetApprovalStatusOk() (*string, bool)`

GetApprovalStatusOk returns a tuple with the ApprovalStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApprovalStatus

`func (o *EnablePaymentProcessing200ResponseData) SetApprovalStatus(v string)`

SetApprovalStatus sets ApprovalStatus field to given value.

### HasApprovalStatus

`func (o *EnablePaymentProcessing200ResponseData) HasApprovalStatus() bool`

HasApprovalStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# GetPaymentProcessingStatus200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Onboarded** | Pointer to **bool** |  | [optional] 
**Enabled** | Pointer to **bool** | Whether payment collection is actually toggled on (implies approved). | [optional] 
**ApprovalStatus** | Pointer to **string** | not_submitted, pending_review, approved, or rejected. | [optional] 
**Status** | Pointer to **string** | Derived overall status for the console to render: not_onboarded, pending_review, rejected, disabled, or active. | [optional] 
**RejectionReason** | Pointer to **NullableString** |  | [optional] 
**Stablecoin** | Pointer to [**GetPaymentProcessingStatus200ResponseDataStablecoin**](GetPaymentProcessingStatus200ResponseDataStablecoin.md) |  | [optional] 

## Methods

### NewGetPaymentProcessingStatus200ResponseData

`func NewGetPaymentProcessingStatus200ResponseData() *GetPaymentProcessingStatus200ResponseData`

NewGetPaymentProcessingStatus200ResponseData instantiates a new GetPaymentProcessingStatus200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetPaymentProcessingStatus200ResponseDataWithDefaults

`func NewGetPaymentProcessingStatus200ResponseDataWithDefaults() *GetPaymentProcessingStatus200ResponseData`

NewGetPaymentProcessingStatus200ResponseDataWithDefaults instantiates a new GetPaymentProcessingStatus200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOnboarded

`func (o *GetPaymentProcessingStatus200ResponseData) GetOnboarded() bool`

GetOnboarded returns the Onboarded field if non-nil, zero value otherwise.

### GetOnboardedOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetOnboardedOk() (*bool, bool)`

GetOnboardedOk returns a tuple with the Onboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnboarded

`func (o *GetPaymentProcessingStatus200ResponseData) SetOnboarded(v bool)`

SetOnboarded sets Onboarded field to given value.

### HasOnboarded

`func (o *GetPaymentProcessingStatus200ResponseData) HasOnboarded() bool`

HasOnboarded returns a boolean if a field has been set.

### GetEnabled

`func (o *GetPaymentProcessingStatus200ResponseData) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *GetPaymentProcessingStatus200ResponseData) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *GetPaymentProcessingStatus200ResponseData) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetApprovalStatus

`func (o *GetPaymentProcessingStatus200ResponseData) GetApprovalStatus() string`

GetApprovalStatus returns the ApprovalStatus field if non-nil, zero value otherwise.

### GetApprovalStatusOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetApprovalStatusOk() (*string, bool)`

GetApprovalStatusOk returns a tuple with the ApprovalStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApprovalStatus

`func (o *GetPaymentProcessingStatus200ResponseData) SetApprovalStatus(v string)`

SetApprovalStatus sets ApprovalStatus field to given value.

### HasApprovalStatus

`func (o *GetPaymentProcessingStatus200ResponseData) HasApprovalStatus() bool`

HasApprovalStatus returns a boolean if a field has been set.

### GetStatus

`func (o *GetPaymentProcessingStatus200ResponseData) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *GetPaymentProcessingStatus200ResponseData) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *GetPaymentProcessingStatus200ResponseData) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetRejectionReason

`func (o *GetPaymentProcessingStatus200ResponseData) GetRejectionReason() string`

GetRejectionReason returns the RejectionReason field if non-nil, zero value otherwise.

### GetRejectionReasonOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetRejectionReasonOk() (*string, bool)`

GetRejectionReasonOk returns a tuple with the RejectionReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRejectionReason

`func (o *GetPaymentProcessingStatus200ResponseData) SetRejectionReason(v string)`

SetRejectionReason sets RejectionReason field to given value.

### HasRejectionReason

`func (o *GetPaymentProcessingStatus200ResponseData) HasRejectionReason() bool`

HasRejectionReason returns a boolean if a field has been set.

### SetRejectionReasonNil

`func (o *GetPaymentProcessingStatus200ResponseData) SetRejectionReasonNil(b bool)`

 SetRejectionReasonNil sets the value for RejectionReason to be an explicit nil

### UnsetRejectionReason
`func (o *GetPaymentProcessingStatus200ResponseData) UnsetRejectionReason()`

UnsetRejectionReason ensures that no value is present for RejectionReason, not even an explicit nil
### GetStablecoin

`func (o *GetPaymentProcessingStatus200ResponseData) GetStablecoin() GetPaymentProcessingStatus200ResponseDataStablecoin`

GetStablecoin returns the Stablecoin field if non-nil, zero value otherwise.

### GetStablecoinOk

`func (o *GetPaymentProcessingStatus200ResponseData) GetStablecoinOk() (*GetPaymentProcessingStatus200ResponseDataStablecoin, bool)`

GetStablecoinOk returns a tuple with the Stablecoin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStablecoin

`func (o *GetPaymentProcessingStatus200ResponseData) SetStablecoin(v GetPaymentProcessingStatus200ResponseDataStablecoin)`

SetStablecoin sets Stablecoin field to given value.

### HasStablecoin

`func (o *GetPaymentProcessingStatus200ResponseData) HasStablecoin() bool`

HasStablecoin returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



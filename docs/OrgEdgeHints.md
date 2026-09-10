# OrgEdgeHints

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SaasIntegrationEnabled** | Pointer to **bool** |  | [optional] 
**Skipped** | Pointer to **bool** |  | [optional] 
**Reason** | Pointer to **NullableString** |  | [optional] 
**CustomHostnameId** | Pointer to **NullableString** |  | [optional] 
**HostnameStatus** | Pointer to **NullableString** |  | [optional] 
**SslStatus** | Pointer to **NullableString** |  | [optional] 
**OwnershipVerification** | Pointer to [**NullableOrgEdgeHintsOwnershipVerification**](OrgEdgeHintsOwnershipVerification.md) |  | [optional] 
**SslValidationRecords** | Pointer to [**[]OrgSslValidationRecord**](OrgSslValidationRecord.md) |  | [optional] 
**LastError** | Pointer to **NullableString** |  | [optional] 
**Instructions** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewOrgEdgeHints

`func NewOrgEdgeHints() *OrgEdgeHints`

NewOrgEdgeHints instantiates a new OrgEdgeHints object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrgEdgeHintsWithDefaults

`func NewOrgEdgeHintsWithDefaults() *OrgEdgeHints`

NewOrgEdgeHintsWithDefaults instantiates a new OrgEdgeHints object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSaasIntegrationEnabled

`func (o *OrgEdgeHints) GetSaasIntegrationEnabled() bool`

GetSaasIntegrationEnabled returns the SaasIntegrationEnabled field if non-nil, zero value otherwise.

### GetSaasIntegrationEnabledOk

`func (o *OrgEdgeHints) GetSaasIntegrationEnabledOk() (*bool, bool)`

GetSaasIntegrationEnabledOk returns a tuple with the SaasIntegrationEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaasIntegrationEnabled

`func (o *OrgEdgeHints) SetSaasIntegrationEnabled(v bool)`

SetSaasIntegrationEnabled sets SaasIntegrationEnabled field to given value.

### HasSaasIntegrationEnabled

`func (o *OrgEdgeHints) HasSaasIntegrationEnabled() bool`

HasSaasIntegrationEnabled returns a boolean if a field has been set.

### GetSkipped

`func (o *OrgEdgeHints) GetSkipped() bool`

GetSkipped returns the Skipped field if non-nil, zero value otherwise.

### GetSkippedOk

`func (o *OrgEdgeHints) GetSkippedOk() (*bool, bool)`

GetSkippedOk returns a tuple with the Skipped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkipped

`func (o *OrgEdgeHints) SetSkipped(v bool)`

SetSkipped sets Skipped field to given value.

### HasSkipped

`func (o *OrgEdgeHints) HasSkipped() bool`

HasSkipped returns a boolean if a field has been set.

### GetReason

`func (o *OrgEdgeHints) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *OrgEdgeHints) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *OrgEdgeHints) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *OrgEdgeHints) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *OrgEdgeHints) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *OrgEdgeHints) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetCustomHostnameId

`func (o *OrgEdgeHints) GetCustomHostnameId() string`

GetCustomHostnameId returns the CustomHostnameId field if non-nil, zero value otherwise.

### GetCustomHostnameIdOk

`func (o *OrgEdgeHints) GetCustomHostnameIdOk() (*string, bool)`

GetCustomHostnameIdOk returns a tuple with the CustomHostnameId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomHostnameId

`func (o *OrgEdgeHints) SetCustomHostnameId(v string)`

SetCustomHostnameId sets CustomHostnameId field to given value.

### HasCustomHostnameId

`func (o *OrgEdgeHints) HasCustomHostnameId() bool`

HasCustomHostnameId returns a boolean if a field has been set.

### SetCustomHostnameIdNil

`func (o *OrgEdgeHints) SetCustomHostnameIdNil(b bool)`

 SetCustomHostnameIdNil sets the value for CustomHostnameId to be an explicit nil

### UnsetCustomHostnameId
`func (o *OrgEdgeHints) UnsetCustomHostnameId()`

UnsetCustomHostnameId ensures that no value is present for CustomHostnameId, not even an explicit nil
### GetHostnameStatus

`func (o *OrgEdgeHints) GetHostnameStatus() string`

GetHostnameStatus returns the HostnameStatus field if non-nil, zero value otherwise.

### GetHostnameStatusOk

`func (o *OrgEdgeHints) GetHostnameStatusOk() (*string, bool)`

GetHostnameStatusOk returns a tuple with the HostnameStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostnameStatus

`func (o *OrgEdgeHints) SetHostnameStatus(v string)`

SetHostnameStatus sets HostnameStatus field to given value.

### HasHostnameStatus

`func (o *OrgEdgeHints) HasHostnameStatus() bool`

HasHostnameStatus returns a boolean if a field has been set.

### SetHostnameStatusNil

`func (o *OrgEdgeHints) SetHostnameStatusNil(b bool)`

 SetHostnameStatusNil sets the value for HostnameStatus to be an explicit nil

### UnsetHostnameStatus
`func (o *OrgEdgeHints) UnsetHostnameStatus()`

UnsetHostnameStatus ensures that no value is present for HostnameStatus, not even an explicit nil
### GetSslStatus

`func (o *OrgEdgeHints) GetSslStatus() string`

GetSslStatus returns the SslStatus field if non-nil, zero value otherwise.

### GetSslStatusOk

`func (o *OrgEdgeHints) GetSslStatusOk() (*string, bool)`

GetSslStatusOk returns a tuple with the SslStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSslStatus

`func (o *OrgEdgeHints) SetSslStatus(v string)`

SetSslStatus sets SslStatus field to given value.

### HasSslStatus

`func (o *OrgEdgeHints) HasSslStatus() bool`

HasSslStatus returns a boolean if a field has been set.

### SetSslStatusNil

`func (o *OrgEdgeHints) SetSslStatusNil(b bool)`

 SetSslStatusNil sets the value for SslStatus to be an explicit nil

### UnsetSslStatus
`func (o *OrgEdgeHints) UnsetSslStatus()`

UnsetSslStatus ensures that no value is present for SslStatus, not even an explicit nil
### GetOwnershipVerification

`func (o *OrgEdgeHints) GetOwnershipVerification() OrgEdgeHintsOwnershipVerification`

GetOwnershipVerification returns the OwnershipVerification field if non-nil, zero value otherwise.

### GetOwnershipVerificationOk

`func (o *OrgEdgeHints) GetOwnershipVerificationOk() (*OrgEdgeHintsOwnershipVerification, bool)`

GetOwnershipVerificationOk returns a tuple with the OwnershipVerification field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnershipVerification

`func (o *OrgEdgeHints) SetOwnershipVerification(v OrgEdgeHintsOwnershipVerification)`

SetOwnershipVerification sets OwnershipVerification field to given value.

### HasOwnershipVerification

`func (o *OrgEdgeHints) HasOwnershipVerification() bool`

HasOwnershipVerification returns a boolean if a field has been set.

### SetOwnershipVerificationNil

`func (o *OrgEdgeHints) SetOwnershipVerificationNil(b bool)`

 SetOwnershipVerificationNil sets the value for OwnershipVerification to be an explicit nil

### UnsetOwnershipVerification
`func (o *OrgEdgeHints) UnsetOwnershipVerification()`

UnsetOwnershipVerification ensures that no value is present for OwnershipVerification, not even an explicit nil
### GetSslValidationRecords

`func (o *OrgEdgeHints) GetSslValidationRecords() []OrgSslValidationRecord`

GetSslValidationRecords returns the SslValidationRecords field if non-nil, zero value otherwise.

### GetSslValidationRecordsOk

`func (o *OrgEdgeHints) GetSslValidationRecordsOk() (*[]OrgSslValidationRecord, bool)`

GetSslValidationRecordsOk returns a tuple with the SslValidationRecords field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSslValidationRecords

`func (o *OrgEdgeHints) SetSslValidationRecords(v []OrgSslValidationRecord)`

SetSslValidationRecords sets SslValidationRecords field to given value.

### HasSslValidationRecords

`func (o *OrgEdgeHints) HasSslValidationRecords() bool`

HasSslValidationRecords returns a boolean if a field has been set.

### GetLastError

`func (o *OrgEdgeHints) GetLastError() string`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *OrgEdgeHints) GetLastErrorOk() (*string, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *OrgEdgeHints) SetLastError(v string)`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *OrgEdgeHints) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *OrgEdgeHints) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *OrgEdgeHints) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetInstructions

`func (o *OrgEdgeHints) GetInstructions() string`

GetInstructions returns the Instructions field if non-nil, zero value otherwise.

### GetInstructionsOk

`func (o *OrgEdgeHints) GetInstructionsOk() (*string, bool)`

GetInstructionsOk returns a tuple with the Instructions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstructions

`func (o *OrgEdgeHints) SetInstructions(v string)`

SetInstructions sets Instructions field to given value.

### HasInstructions

`func (o *OrgEdgeHints) HasInstructions() bool`

HasInstructions returns a boolean if a field has been set.

### SetInstructionsNil

`func (o *OrgEdgeHints) SetInstructionsNil(b bool)`

 SetInstructionsNil sets the value for Instructions to be an explicit nil

### UnsetInstructions
`func (o *OrgEdgeHints) UnsetInstructions()`

UnsetInstructions ensures that no value is present for Instructions, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



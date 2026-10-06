# OrgSslValidationRecord

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TxtName** | Pointer to **NullableString** |  | [optional] 
**TxtValue** | Pointer to **NullableString** |  | [optional] 
**HttpUrl** | Pointer to **NullableString** |  | [optional] 
**HttpBody** | Pointer to **NullableString** |  | [optional] 
**Cname** | Pointer to **NullableString** |  | [optional] 
**CnameTarget** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewOrgSslValidationRecord

`func NewOrgSslValidationRecord() *OrgSslValidationRecord`

NewOrgSslValidationRecord instantiates a new OrgSslValidationRecord object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrgSslValidationRecordWithDefaults

`func NewOrgSslValidationRecordWithDefaults() *OrgSslValidationRecord`

NewOrgSslValidationRecordWithDefaults instantiates a new OrgSslValidationRecord object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTxtName

`func (o *OrgSslValidationRecord) GetTxtName() string`

GetTxtName returns the TxtName field if non-nil, zero value otherwise.

### GetTxtNameOk

`func (o *OrgSslValidationRecord) GetTxtNameOk() (*string, bool)`

GetTxtNameOk returns a tuple with the TxtName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxtName

`func (o *OrgSslValidationRecord) SetTxtName(v string)`

SetTxtName sets TxtName field to given value.

### HasTxtName

`func (o *OrgSslValidationRecord) HasTxtName() bool`

HasTxtName returns a boolean if a field has been set.

### SetTxtNameNil

`func (o *OrgSslValidationRecord) SetTxtNameNil(b bool)`

 SetTxtNameNil sets the value for TxtName to be an explicit nil

### UnsetTxtName
`func (o *OrgSslValidationRecord) UnsetTxtName()`

UnsetTxtName ensures that no value is present for TxtName, not even an explicit nil
### GetTxtValue

`func (o *OrgSslValidationRecord) GetTxtValue() string`

GetTxtValue returns the TxtValue field if non-nil, zero value otherwise.

### GetTxtValueOk

`func (o *OrgSslValidationRecord) GetTxtValueOk() (*string, bool)`

GetTxtValueOk returns a tuple with the TxtValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxtValue

`func (o *OrgSslValidationRecord) SetTxtValue(v string)`

SetTxtValue sets TxtValue field to given value.

### HasTxtValue

`func (o *OrgSslValidationRecord) HasTxtValue() bool`

HasTxtValue returns a boolean if a field has been set.

### SetTxtValueNil

`func (o *OrgSslValidationRecord) SetTxtValueNil(b bool)`

 SetTxtValueNil sets the value for TxtValue to be an explicit nil

### UnsetTxtValue
`func (o *OrgSslValidationRecord) UnsetTxtValue()`

UnsetTxtValue ensures that no value is present for TxtValue, not even an explicit nil
### GetHttpUrl

`func (o *OrgSslValidationRecord) GetHttpUrl() string`

GetHttpUrl returns the HttpUrl field if non-nil, zero value otherwise.

### GetHttpUrlOk

`func (o *OrgSslValidationRecord) GetHttpUrlOk() (*string, bool)`

GetHttpUrlOk returns a tuple with the HttpUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpUrl

`func (o *OrgSslValidationRecord) SetHttpUrl(v string)`

SetHttpUrl sets HttpUrl field to given value.

### HasHttpUrl

`func (o *OrgSslValidationRecord) HasHttpUrl() bool`

HasHttpUrl returns a boolean if a field has been set.

### SetHttpUrlNil

`func (o *OrgSslValidationRecord) SetHttpUrlNil(b bool)`

 SetHttpUrlNil sets the value for HttpUrl to be an explicit nil

### UnsetHttpUrl
`func (o *OrgSslValidationRecord) UnsetHttpUrl()`

UnsetHttpUrl ensures that no value is present for HttpUrl, not even an explicit nil
### GetHttpBody

`func (o *OrgSslValidationRecord) GetHttpBody() string`

GetHttpBody returns the HttpBody field if non-nil, zero value otherwise.

### GetHttpBodyOk

`func (o *OrgSslValidationRecord) GetHttpBodyOk() (*string, bool)`

GetHttpBodyOk returns a tuple with the HttpBody field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpBody

`func (o *OrgSslValidationRecord) SetHttpBody(v string)`

SetHttpBody sets HttpBody field to given value.

### HasHttpBody

`func (o *OrgSslValidationRecord) HasHttpBody() bool`

HasHttpBody returns a boolean if a field has been set.

### SetHttpBodyNil

`func (o *OrgSslValidationRecord) SetHttpBodyNil(b bool)`

 SetHttpBodyNil sets the value for HttpBody to be an explicit nil

### UnsetHttpBody
`func (o *OrgSslValidationRecord) UnsetHttpBody()`

UnsetHttpBody ensures that no value is present for HttpBody, not even an explicit nil
### GetCname

`func (o *OrgSslValidationRecord) GetCname() string`

GetCname returns the Cname field if non-nil, zero value otherwise.

### GetCnameOk

`func (o *OrgSslValidationRecord) GetCnameOk() (*string, bool)`

GetCnameOk returns a tuple with the Cname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCname

`func (o *OrgSslValidationRecord) SetCname(v string)`

SetCname sets Cname field to given value.

### HasCname

`func (o *OrgSslValidationRecord) HasCname() bool`

HasCname returns a boolean if a field has been set.

### SetCnameNil

`func (o *OrgSslValidationRecord) SetCnameNil(b bool)`

 SetCnameNil sets the value for Cname to be an explicit nil

### UnsetCname
`func (o *OrgSslValidationRecord) UnsetCname()`

UnsetCname ensures that no value is present for Cname, not even an explicit nil
### GetCnameTarget

`func (o *OrgSslValidationRecord) GetCnameTarget() string`

GetCnameTarget returns the CnameTarget field if non-nil, zero value otherwise.

### GetCnameTargetOk

`func (o *OrgSslValidationRecord) GetCnameTargetOk() (*string, bool)`

GetCnameTargetOk returns a tuple with the CnameTarget field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCnameTarget

`func (o *OrgSslValidationRecord) SetCnameTarget(v string)`

SetCnameTarget sets CnameTarget field to given value.

### HasCnameTarget

`func (o *OrgSslValidationRecord) HasCnameTarget() bool`

HasCnameTarget returns a boolean if a field has been set.

### SetCnameTargetNil

`func (o *OrgSslValidationRecord) SetCnameTargetNil(b bool)`

 SetCnameTargetNil sets the value for CnameTarget to be an explicit nil

### UnsetCnameTarget
`func (o *OrgSslValidationRecord) UnsetCnameTarget()`

UnsetCnameTarget ensures that no value is present for CnameTarget, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



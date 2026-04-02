# MultiRoleUpdateSettingsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsEnabled** | Pointer to **bool** |  | [optional] 
**DefaultRole** | Pointer to **string** |  | [optional] 
**Settings** | Pointer to [**MultiRoleUpdateSettingsRequestSettings**](MultiRoleUpdateSettingsRequestSettings.md) |  | [optional] 

## Methods

### NewMultiRoleUpdateSettingsRequest

`func NewMultiRoleUpdateSettingsRequest() *MultiRoleUpdateSettingsRequest`

NewMultiRoleUpdateSettingsRequest instantiates a new MultiRoleUpdateSettingsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleUpdateSettingsRequestWithDefaults

`func NewMultiRoleUpdateSettingsRequestWithDefaults() *MultiRoleUpdateSettingsRequest`

NewMultiRoleUpdateSettingsRequestWithDefaults instantiates a new MultiRoleUpdateSettingsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIsEnabled

`func (o *MultiRoleUpdateSettingsRequest) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *MultiRoleUpdateSettingsRequest) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *MultiRoleUpdateSettingsRequest) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.

### HasIsEnabled

`func (o *MultiRoleUpdateSettingsRequest) HasIsEnabled() bool`

HasIsEnabled returns a boolean if a field has been set.

### GetDefaultRole

`func (o *MultiRoleUpdateSettingsRequest) GetDefaultRole() string`

GetDefaultRole returns the DefaultRole field if non-nil, zero value otherwise.

### GetDefaultRoleOk

`func (o *MultiRoleUpdateSettingsRequest) GetDefaultRoleOk() (*string, bool)`

GetDefaultRoleOk returns a tuple with the DefaultRole field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultRole

`func (o *MultiRoleUpdateSettingsRequest) SetDefaultRole(v string)`

SetDefaultRole sets DefaultRole field to given value.

### HasDefaultRole

`func (o *MultiRoleUpdateSettingsRequest) HasDefaultRole() bool`

HasDefaultRole returns a boolean if a field has been set.

### GetSettings

`func (o *MultiRoleUpdateSettingsRequest) GetSettings() MultiRoleUpdateSettingsRequestSettings`

GetSettings returns the Settings field if non-nil, zero value otherwise.

### GetSettingsOk

`func (o *MultiRoleUpdateSettingsRequest) GetSettingsOk() (*MultiRoleUpdateSettingsRequestSettings, bool)`

GetSettingsOk returns a tuple with the Settings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettings

`func (o *MultiRoleUpdateSettingsRequest) SetSettings(v MultiRoleUpdateSettingsRequestSettings)`

SetSettings sets Settings field to given value.

### HasSettings

`func (o *MultiRoleUpdateSettingsRequest) HasSettings() bool`

HasSettings returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



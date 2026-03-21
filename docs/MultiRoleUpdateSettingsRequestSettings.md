# MultiRoleUpdateSettingsRequestSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AllowMultipleRoles** | Pointer to **bool** | Whether an end user may hold multiple app roles. | [optional] 
**RequireRoleSelection** | Pointer to **bool** | If true, signup must pick a role; if false and &#x60;autoAssignDefault&#x60; is true, &#x60;defaultRole&#x60; is used when omitted. | [optional] 
**AutoAssignDefault** | Pointer to **bool** | When true, assigns &#x60;defaultRole&#x60; when the client does not specify a role at signup. | [optional] 

## Methods

### NewMultiRoleUpdateSettingsRequestSettings

`func NewMultiRoleUpdateSettingsRequestSettings() *MultiRoleUpdateSettingsRequestSettings`

NewMultiRoleUpdateSettingsRequestSettings instantiates a new MultiRoleUpdateSettingsRequestSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleUpdateSettingsRequestSettingsWithDefaults

`func NewMultiRoleUpdateSettingsRequestSettingsWithDefaults() *MultiRoleUpdateSettingsRequestSettings`

NewMultiRoleUpdateSettingsRequestSettingsWithDefaults instantiates a new MultiRoleUpdateSettingsRequestSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllowMultipleRoles

`func (o *MultiRoleUpdateSettingsRequestSettings) GetAllowMultipleRoles() bool`

GetAllowMultipleRoles returns the AllowMultipleRoles field if non-nil, zero value otherwise.

### GetAllowMultipleRolesOk

`func (o *MultiRoleUpdateSettingsRequestSettings) GetAllowMultipleRolesOk() (*bool, bool)`

GetAllowMultipleRolesOk returns a tuple with the AllowMultipleRoles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowMultipleRoles

`func (o *MultiRoleUpdateSettingsRequestSettings) SetAllowMultipleRoles(v bool)`

SetAllowMultipleRoles sets AllowMultipleRoles field to given value.

### HasAllowMultipleRoles

`func (o *MultiRoleUpdateSettingsRequestSettings) HasAllowMultipleRoles() bool`

HasAllowMultipleRoles returns a boolean if a field has been set.

### GetRequireRoleSelection

`func (o *MultiRoleUpdateSettingsRequestSettings) GetRequireRoleSelection() bool`

GetRequireRoleSelection returns the RequireRoleSelection field if non-nil, zero value otherwise.

### GetRequireRoleSelectionOk

`func (o *MultiRoleUpdateSettingsRequestSettings) GetRequireRoleSelectionOk() (*bool, bool)`

GetRequireRoleSelectionOk returns a tuple with the RequireRoleSelection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequireRoleSelection

`func (o *MultiRoleUpdateSettingsRequestSettings) SetRequireRoleSelection(v bool)`

SetRequireRoleSelection sets RequireRoleSelection field to given value.

### HasRequireRoleSelection

`func (o *MultiRoleUpdateSettingsRequestSettings) HasRequireRoleSelection() bool`

HasRequireRoleSelection returns a boolean if a field has been set.

### GetAutoAssignDefault

`func (o *MultiRoleUpdateSettingsRequestSettings) GetAutoAssignDefault() bool`

GetAutoAssignDefault returns the AutoAssignDefault field if non-nil, zero value otherwise.

### GetAutoAssignDefaultOk

`func (o *MultiRoleUpdateSettingsRequestSettings) GetAutoAssignDefaultOk() (*bool, bool)`

GetAutoAssignDefaultOk returns a tuple with the AutoAssignDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoAssignDefault

`func (o *MultiRoleUpdateSettingsRequestSettings) SetAutoAssignDefault(v bool)`

SetAutoAssignDefault sets AutoAssignDefault field to given value.

### HasAutoAssignDefault

`func (o *MultiRoleUpdateSettingsRequestSettings) HasAutoAssignDefault() bool`

HasAutoAssignDefault returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



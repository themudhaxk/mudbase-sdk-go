# MultiRoleUpdateCollectionPermissionsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Actions** | Pointer to **[]string** |  | [optional] 
**Conditions** | Pointer to **map[string]interface{}** |  | [optional] 
**DataScope** | Pointer to **string** | &#x60;all&#x60; &#x3D; no automatic row-owner filter. &#x60;own&#x60; &#x3D; only documents where the owner field (default &#x60;createdBy&#x60;) matches the authenticated app user. | [optional] 
**OwnerField** | Pointer to **string** | Optional per-assignment override for the document field used when &#x60;dataScope&#x60; is &#x60;own&#x60; (project default is &#x60;settings.dataOwnerField&#x60;, usually &#x60;createdBy&#x60;). | [optional] 

## Methods

### NewMultiRoleUpdateCollectionPermissionsRequest

`func NewMultiRoleUpdateCollectionPermissionsRequest() *MultiRoleUpdateCollectionPermissionsRequest`

NewMultiRoleUpdateCollectionPermissionsRequest instantiates a new MultiRoleUpdateCollectionPermissionsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleUpdateCollectionPermissionsRequestWithDefaults

`func NewMultiRoleUpdateCollectionPermissionsRequestWithDefaults() *MultiRoleUpdateCollectionPermissionsRequest`

NewMultiRoleUpdateCollectionPermissionsRequestWithDefaults instantiates a new MultiRoleUpdateCollectionPermissionsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetActions() []string`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetActionsOk() (*[]string, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) SetActions(v []string)`

SetActions sets Actions field to given value.

### HasActions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) HasActions() bool`

HasActions returns a boolean if a field has been set.

### GetConditions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetConditions() map[string]interface{}`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetConditionsOk() (*map[string]interface{}, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) SetConditions(v map[string]interface{})`

SetConditions sets Conditions field to given value.

### HasConditions

`func (o *MultiRoleUpdateCollectionPermissionsRequest) HasConditions() bool`

HasConditions returns a boolean if a field has been set.

### GetDataScope

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetDataScope() string`

GetDataScope returns the DataScope field if non-nil, zero value otherwise.

### GetDataScopeOk

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetDataScopeOk() (*string, bool)`

GetDataScopeOk returns a tuple with the DataScope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataScope

`func (o *MultiRoleUpdateCollectionPermissionsRequest) SetDataScope(v string)`

SetDataScope sets DataScope field to given value.

### HasDataScope

`func (o *MultiRoleUpdateCollectionPermissionsRequest) HasDataScope() bool`

HasDataScope returns a boolean if a field has been set.

### GetOwnerField

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetOwnerField() string`

GetOwnerField returns the OwnerField field if non-nil, zero value otherwise.

### GetOwnerFieldOk

`func (o *MultiRoleUpdateCollectionPermissionsRequest) GetOwnerFieldOk() (*string, bool)`

GetOwnerFieldOk returns a tuple with the OwnerField field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerField

`func (o *MultiRoleUpdateCollectionPermissionsRequest) SetOwnerField(v string)`

SetOwnerField sets OwnerField field to given value.

### HasOwnerField

`func (o *MultiRoleUpdateCollectionPermissionsRequest) HasOwnerField() bool`

HasOwnerField returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



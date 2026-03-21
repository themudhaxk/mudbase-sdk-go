# MultiRoleAddRoleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Slug** | **string** |  | 
**Name** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**SignupEndpoint** | **string** |  | 
**DefaultPermissions** | Pointer to [**[]MultiRoleAddRoleRequestDefaultPermissionsInner**](MultiRoleAddRoleRequestDefaultPermissionsInner.md) | Optional global/base permissions. For collection-level CRUD use &#x60;collectionPermissions&#x60;. | [optional] 
**CollectionPermissions** | Pointer to [**map[string]MultiRoleUpdateRoleRequestCollectionPermissionsValue**](MultiRoleUpdateRoleRequestCollectionPermissionsValue.md) | Per-collection CRUD map. Keys are collection slugs; values are action arrays or objects with &#x60;actions&#x60; + optional &#x60;conditions&#x60;. | [optional] 

## Methods

### NewMultiRoleAddRoleRequest

`func NewMultiRoleAddRoleRequest(slug string, name string, signupEndpoint string, ) *MultiRoleAddRoleRequest`

NewMultiRoleAddRoleRequest instantiates a new MultiRoleAddRoleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleAddRoleRequestWithDefaults

`func NewMultiRoleAddRoleRequestWithDefaults() *MultiRoleAddRoleRequest`

NewMultiRoleAddRoleRequestWithDefaults instantiates a new MultiRoleAddRoleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSlug

`func (o *MultiRoleAddRoleRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *MultiRoleAddRoleRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *MultiRoleAddRoleRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *MultiRoleAddRoleRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *MultiRoleAddRoleRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *MultiRoleAddRoleRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *MultiRoleAddRoleRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *MultiRoleAddRoleRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *MultiRoleAddRoleRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *MultiRoleAddRoleRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetSignupEndpoint

`func (o *MultiRoleAddRoleRequest) GetSignupEndpoint() string`

GetSignupEndpoint returns the SignupEndpoint field if non-nil, zero value otherwise.

### GetSignupEndpointOk

`func (o *MultiRoleAddRoleRequest) GetSignupEndpointOk() (*string, bool)`

GetSignupEndpointOk returns a tuple with the SignupEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignupEndpoint

`func (o *MultiRoleAddRoleRequest) SetSignupEndpoint(v string)`

SetSignupEndpoint sets SignupEndpoint field to given value.


### GetDefaultPermissions

`func (o *MultiRoleAddRoleRequest) GetDefaultPermissions() []MultiRoleAddRoleRequestDefaultPermissionsInner`

GetDefaultPermissions returns the DefaultPermissions field if non-nil, zero value otherwise.

### GetDefaultPermissionsOk

`func (o *MultiRoleAddRoleRequest) GetDefaultPermissionsOk() (*[]MultiRoleAddRoleRequestDefaultPermissionsInner, bool)`

GetDefaultPermissionsOk returns a tuple with the DefaultPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultPermissions

`func (o *MultiRoleAddRoleRequest) SetDefaultPermissions(v []MultiRoleAddRoleRequestDefaultPermissionsInner)`

SetDefaultPermissions sets DefaultPermissions field to given value.

### HasDefaultPermissions

`func (o *MultiRoleAddRoleRequest) HasDefaultPermissions() bool`

HasDefaultPermissions returns a boolean if a field has been set.

### GetCollectionPermissions

`func (o *MultiRoleAddRoleRequest) GetCollectionPermissions() map[string]MultiRoleUpdateRoleRequestCollectionPermissionsValue`

GetCollectionPermissions returns the CollectionPermissions field if non-nil, zero value otherwise.

### GetCollectionPermissionsOk

`func (o *MultiRoleAddRoleRequest) GetCollectionPermissionsOk() (*map[string]MultiRoleUpdateRoleRequestCollectionPermissionsValue, bool)`

GetCollectionPermissionsOk returns a tuple with the CollectionPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCollectionPermissions

`func (o *MultiRoleAddRoleRequest) SetCollectionPermissions(v map[string]MultiRoleUpdateRoleRequestCollectionPermissionsValue)`

SetCollectionPermissions sets CollectionPermissions field to given value.

### HasCollectionPermissions

`func (o *MultiRoleAddRoleRequest) HasCollectionPermissions() bool`

HasCollectionPermissions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



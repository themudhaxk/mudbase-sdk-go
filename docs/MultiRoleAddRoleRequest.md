# MultiRoleAddRoleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Slug** | **string** |  | 
**Name** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**SignupEndpoint** | **string** |  | 
**RequiresApproval** | Pointer to **bool** |  | [optional] 
**RequiresPayment** | Pointer to **bool** |  | [optional] 
**RequiresKYC** | Pointer to **bool** |  | [optional] 
**DefaultPermissions** | Pointer to [**[]MultiRoleAddRoleRequestDefaultPermissionsInner**](MultiRoleAddRoleRequestDefaultPermissionsInner.md) | Optional global/base permissions. For collection-level CRUD use &#x60;collectionPermissions&#x60;. | [optional] 
**CollectionPermissions** | Pointer to [**map[string]AppRoleCollectionPermissionValue**](AppRoleCollectionPermissionValue.md) | Per-collection CRUD map. Keys are collection slugs; values are action arrays or objects with &#x60;actions&#x60; + optional &#x60;conditions&#x60;. | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**FeaturePermissions** | Pointer to **map[string]map[string]bool** | Per-role feature toggles for app JWTs: &#x60;{ [resource]: { [action]: boolean } }&#x60;. Use resource and action names that match the public API contract (see multi-role guide and simulate-permissions). **Messaging** accepts legacy keys (&#x60;email&#x60;, &#x60;sms&#x60;, &#x60;push&#x60;, …) and newer names (&#x60;send_email&#x60;, &#x60;send_sms&#x60;, …) as synonyms. Common resources: &#x60;messaging&#x60;, &#x60;integration&#x60;, &#x60;functions&#x60;, &#x60;data&#x60;, &#x60;search&#x60;, &#x60;usage&#x60;, &#x60;storage&#x60;, &#x60;chat&#x60;, &#x60;realtime&#x60;, &#x60;roleElevation&#x60;, &#x60;webhooks&#x60;.  | [optional] 

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


### GetRequiresApproval

`func (o *MultiRoleAddRoleRequest) GetRequiresApproval() bool`

GetRequiresApproval returns the RequiresApproval field if non-nil, zero value otherwise.

### GetRequiresApprovalOk

`func (o *MultiRoleAddRoleRequest) GetRequiresApprovalOk() (*bool, bool)`

GetRequiresApprovalOk returns a tuple with the RequiresApproval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresApproval

`func (o *MultiRoleAddRoleRequest) SetRequiresApproval(v bool)`

SetRequiresApproval sets RequiresApproval field to given value.

### HasRequiresApproval

`func (o *MultiRoleAddRoleRequest) HasRequiresApproval() bool`

HasRequiresApproval returns a boolean if a field has been set.

### GetRequiresPayment

`func (o *MultiRoleAddRoleRequest) GetRequiresPayment() bool`

GetRequiresPayment returns the RequiresPayment field if non-nil, zero value otherwise.

### GetRequiresPaymentOk

`func (o *MultiRoleAddRoleRequest) GetRequiresPaymentOk() (*bool, bool)`

GetRequiresPaymentOk returns a tuple with the RequiresPayment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresPayment

`func (o *MultiRoleAddRoleRequest) SetRequiresPayment(v bool)`

SetRequiresPayment sets RequiresPayment field to given value.

### HasRequiresPayment

`func (o *MultiRoleAddRoleRequest) HasRequiresPayment() bool`

HasRequiresPayment returns a boolean if a field has been set.

### GetRequiresKYC

`func (o *MultiRoleAddRoleRequest) GetRequiresKYC() bool`

GetRequiresKYC returns the RequiresKYC field if non-nil, zero value otherwise.

### GetRequiresKYCOk

`func (o *MultiRoleAddRoleRequest) GetRequiresKYCOk() (*bool, bool)`

GetRequiresKYCOk returns a tuple with the RequiresKYC field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresKYC

`func (o *MultiRoleAddRoleRequest) SetRequiresKYC(v bool)`

SetRequiresKYC sets RequiresKYC field to given value.

### HasRequiresKYC

`func (o *MultiRoleAddRoleRequest) HasRequiresKYC() bool`

HasRequiresKYC returns a boolean if a field has been set.

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

`func (o *MultiRoleAddRoleRequest) GetCollectionPermissions() map[string]AppRoleCollectionPermissionValue`

GetCollectionPermissions returns the CollectionPermissions field if non-nil, zero value otherwise.

### GetCollectionPermissionsOk

`func (o *MultiRoleAddRoleRequest) GetCollectionPermissionsOk() (*map[string]AppRoleCollectionPermissionValue, bool)`

GetCollectionPermissionsOk returns a tuple with the CollectionPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCollectionPermissions

`func (o *MultiRoleAddRoleRequest) SetCollectionPermissions(v map[string]AppRoleCollectionPermissionValue)`

SetCollectionPermissions sets CollectionPermissions field to given value.

### HasCollectionPermissions

`func (o *MultiRoleAddRoleRequest) HasCollectionPermissions() bool`

HasCollectionPermissions returns a boolean if a field has been set.

### GetMetadata

`func (o *MultiRoleAddRoleRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *MultiRoleAddRoleRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *MultiRoleAddRoleRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *MultiRoleAddRoleRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetFeaturePermissions

`func (o *MultiRoleAddRoleRequest) GetFeaturePermissions() map[string]map[string]bool`

GetFeaturePermissions returns the FeaturePermissions field if non-nil, zero value otherwise.

### GetFeaturePermissionsOk

`func (o *MultiRoleAddRoleRequest) GetFeaturePermissionsOk() (*map[string]map[string]bool, bool)`

GetFeaturePermissionsOk returns a tuple with the FeaturePermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeaturePermissions

`func (o *MultiRoleAddRoleRequest) SetFeaturePermissions(v map[string]map[string]bool)`

SetFeaturePermissions sets FeaturePermissions field to given value.

### HasFeaturePermissions

`func (o *MultiRoleAddRoleRequest) HasFeaturePermissions() bool`

HasFeaturePermissions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



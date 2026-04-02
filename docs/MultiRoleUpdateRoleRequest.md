# MultiRoleUpdateRoleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**SignupEndpoint** | Pointer to **string** |  | [optional] 
**RequiresApproval** | Pointer to **bool** |  | [optional] 
**RequiresPayment** | Pointer to **bool** |  | [optional] 
**RequiresKYC** | Pointer to **bool** |  | [optional] 
**DefaultPermissions** | Pointer to **[]map[string]interface{}** |  | [optional] 
**CollectionPermissions** | Pointer to [**map[string]AppRoleCollectionPermissionValue**](AppRoleCollectionPermissionValue.md) | Per-collection CRUD map (same as POST add role). | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**FeaturePermissions** | Pointer to **map[string]map[string]bool** | Per-role feature toggles for app JWTs: &#x60;{ [resource]: { [action]: boolean } }&#x60;. Use resource and action names that match the public API contract (see multi-role guide and simulate-permissions). **Messaging** accepts legacy keys (&#x60;email&#x60;, &#x60;sms&#x60;, &#x60;push&#x60;, …) and newer names (&#x60;send_email&#x60;, &#x60;send_sms&#x60;, …) as synonyms. Common resources: &#x60;messaging&#x60;, &#x60;integration&#x60;, &#x60;functions&#x60;, &#x60;data&#x60;, &#x60;search&#x60;, &#x60;usage&#x60;, &#x60;storage&#x60;, &#x60;chat&#x60;, &#x60;realtime&#x60;, &#x60;roleElevation&#x60;, &#x60;webhooks&#x60;.  | [optional] 

## Methods

### NewMultiRoleUpdateRoleRequest

`func NewMultiRoleUpdateRoleRequest() *MultiRoleUpdateRoleRequest`

NewMultiRoleUpdateRoleRequest instantiates a new MultiRoleUpdateRoleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleUpdateRoleRequestWithDefaults

`func NewMultiRoleUpdateRoleRequestWithDefaults() *MultiRoleUpdateRoleRequest`

NewMultiRoleUpdateRoleRequestWithDefaults instantiates a new MultiRoleUpdateRoleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *MultiRoleUpdateRoleRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *MultiRoleUpdateRoleRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *MultiRoleUpdateRoleRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *MultiRoleUpdateRoleRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *MultiRoleUpdateRoleRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *MultiRoleUpdateRoleRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *MultiRoleUpdateRoleRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *MultiRoleUpdateRoleRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetSignupEndpoint

`func (o *MultiRoleUpdateRoleRequest) GetSignupEndpoint() string`

GetSignupEndpoint returns the SignupEndpoint field if non-nil, zero value otherwise.

### GetSignupEndpointOk

`func (o *MultiRoleUpdateRoleRequest) GetSignupEndpointOk() (*string, bool)`

GetSignupEndpointOk returns a tuple with the SignupEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignupEndpoint

`func (o *MultiRoleUpdateRoleRequest) SetSignupEndpoint(v string)`

SetSignupEndpoint sets SignupEndpoint field to given value.

### HasSignupEndpoint

`func (o *MultiRoleUpdateRoleRequest) HasSignupEndpoint() bool`

HasSignupEndpoint returns a boolean if a field has been set.

### GetRequiresApproval

`func (o *MultiRoleUpdateRoleRequest) GetRequiresApproval() bool`

GetRequiresApproval returns the RequiresApproval field if non-nil, zero value otherwise.

### GetRequiresApprovalOk

`func (o *MultiRoleUpdateRoleRequest) GetRequiresApprovalOk() (*bool, bool)`

GetRequiresApprovalOk returns a tuple with the RequiresApproval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresApproval

`func (o *MultiRoleUpdateRoleRequest) SetRequiresApproval(v bool)`

SetRequiresApproval sets RequiresApproval field to given value.

### HasRequiresApproval

`func (o *MultiRoleUpdateRoleRequest) HasRequiresApproval() bool`

HasRequiresApproval returns a boolean if a field has been set.

### GetRequiresPayment

`func (o *MultiRoleUpdateRoleRequest) GetRequiresPayment() bool`

GetRequiresPayment returns the RequiresPayment field if non-nil, zero value otherwise.

### GetRequiresPaymentOk

`func (o *MultiRoleUpdateRoleRequest) GetRequiresPaymentOk() (*bool, bool)`

GetRequiresPaymentOk returns a tuple with the RequiresPayment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresPayment

`func (o *MultiRoleUpdateRoleRequest) SetRequiresPayment(v bool)`

SetRequiresPayment sets RequiresPayment field to given value.

### HasRequiresPayment

`func (o *MultiRoleUpdateRoleRequest) HasRequiresPayment() bool`

HasRequiresPayment returns a boolean if a field has been set.

### GetRequiresKYC

`func (o *MultiRoleUpdateRoleRequest) GetRequiresKYC() bool`

GetRequiresKYC returns the RequiresKYC field if non-nil, zero value otherwise.

### GetRequiresKYCOk

`func (o *MultiRoleUpdateRoleRequest) GetRequiresKYCOk() (*bool, bool)`

GetRequiresKYCOk returns a tuple with the RequiresKYC field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiresKYC

`func (o *MultiRoleUpdateRoleRequest) SetRequiresKYC(v bool)`

SetRequiresKYC sets RequiresKYC field to given value.

### HasRequiresKYC

`func (o *MultiRoleUpdateRoleRequest) HasRequiresKYC() bool`

HasRequiresKYC returns a boolean if a field has been set.

### GetDefaultPermissions

`func (o *MultiRoleUpdateRoleRequest) GetDefaultPermissions() []map[string]interface{}`

GetDefaultPermissions returns the DefaultPermissions field if non-nil, zero value otherwise.

### GetDefaultPermissionsOk

`func (o *MultiRoleUpdateRoleRequest) GetDefaultPermissionsOk() (*[]map[string]interface{}, bool)`

GetDefaultPermissionsOk returns a tuple with the DefaultPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultPermissions

`func (o *MultiRoleUpdateRoleRequest) SetDefaultPermissions(v []map[string]interface{})`

SetDefaultPermissions sets DefaultPermissions field to given value.

### HasDefaultPermissions

`func (o *MultiRoleUpdateRoleRequest) HasDefaultPermissions() bool`

HasDefaultPermissions returns a boolean if a field has been set.

### GetCollectionPermissions

`func (o *MultiRoleUpdateRoleRequest) GetCollectionPermissions() map[string]AppRoleCollectionPermissionValue`

GetCollectionPermissions returns the CollectionPermissions field if non-nil, zero value otherwise.

### GetCollectionPermissionsOk

`func (o *MultiRoleUpdateRoleRequest) GetCollectionPermissionsOk() (*map[string]AppRoleCollectionPermissionValue, bool)`

GetCollectionPermissionsOk returns a tuple with the CollectionPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCollectionPermissions

`func (o *MultiRoleUpdateRoleRequest) SetCollectionPermissions(v map[string]AppRoleCollectionPermissionValue)`

SetCollectionPermissions sets CollectionPermissions field to given value.

### HasCollectionPermissions

`func (o *MultiRoleUpdateRoleRequest) HasCollectionPermissions() bool`

HasCollectionPermissions returns a boolean if a field has been set.

### GetMetadata

`func (o *MultiRoleUpdateRoleRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *MultiRoleUpdateRoleRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *MultiRoleUpdateRoleRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *MultiRoleUpdateRoleRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetFeaturePermissions

`func (o *MultiRoleUpdateRoleRequest) GetFeaturePermissions() map[string]map[string]bool`

GetFeaturePermissions returns the FeaturePermissions field if non-nil, zero value otherwise.

### GetFeaturePermissionsOk

`func (o *MultiRoleUpdateRoleRequest) GetFeaturePermissionsOk() (*map[string]map[string]bool, bool)`

GetFeaturePermissionsOk returns a tuple with the FeaturePermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeaturePermissions

`func (o *MultiRoleUpdateRoleRequest) SetFeaturePermissions(v map[string]map[string]bool)`

SetFeaturePermissions sets FeaturePermissions field to given value.

### HasFeaturePermissions

`func (o *MultiRoleUpdateRoleRequest) HasFeaturePermissions() bool`

HasFeaturePermissions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MultiRoleSimulateAppPermissionsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Role** | **string** |  | 
**OperationId** | Pointer to **string** | OpenAPI operationId (e.g. sendEmail). Optional if method + pathname are sent. | [optional] 
**Method** | Pointer to **string** |  | [optional] 
**Pathname** | Pointer to **string** | Full API path, e.g. /api/messaging/projects/{projectId}/messaging/email | [optional] 
**Path** | Pointer to **string** | Alias for pathname | [optional] 

## Methods

### NewMultiRoleSimulateAppPermissionsRequest

`func NewMultiRoleSimulateAppPermissionsRequest(role string, ) *MultiRoleSimulateAppPermissionsRequest`

NewMultiRoleSimulateAppPermissionsRequest instantiates a new MultiRoleSimulateAppPermissionsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMultiRoleSimulateAppPermissionsRequestWithDefaults

`func NewMultiRoleSimulateAppPermissionsRequestWithDefaults() *MultiRoleSimulateAppPermissionsRequest`

NewMultiRoleSimulateAppPermissionsRequestWithDefaults instantiates a new MultiRoleSimulateAppPermissionsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRole

`func (o *MultiRoleSimulateAppPermissionsRequest) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *MultiRoleSimulateAppPermissionsRequest) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *MultiRoleSimulateAppPermissionsRequest) SetRole(v string)`

SetRole sets Role field to given value.


### GetOperationId

`func (o *MultiRoleSimulateAppPermissionsRequest) GetOperationId() string`

GetOperationId returns the OperationId field if non-nil, zero value otherwise.

### GetOperationIdOk

`func (o *MultiRoleSimulateAppPermissionsRequest) GetOperationIdOk() (*string, bool)`

GetOperationIdOk returns a tuple with the OperationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperationId

`func (o *MultiRoleSimulateAppPermissionsRequest) SetOperationId(v string)`

SetOperationId sets OperationId field to given value.

### HasOperationId

`func (o *MultiRoleSimulateAppPermissionsRequest) HasOperationId() bool`

HasOperationId returns a boolean if a field has been set.

### GetMethod

`func (o *MultiRoleSimulateAppPermissionsRequest) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *MultiRoleSimulateAppPermissionsRequest) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *MultiRoleSimulateAppPermissionsRequest) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *MultiRoleSimulateAppPermissionsRequest) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### GetPathname

`func (o *MultiRoleSimulateAppPermissionsRequest) GetPathname() string`

GetPathname returns the Pathname field if non-nil, zero value otherwise.

### GetPathnameOk

`func (o *MultiRoleSimulateAppPermissionsRequest) GetPathnameOk() (*string, bool)`

GetPathnameOk returns a tuple with the Pathname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPathname

`func (o *MultiRoleSimulateAppPermissionsRequest) SetPathname(v string)`

SetPathname sets Pathname field to given value.

### HasPathname

`func (o *MultiRoleSimulateAppPermissionsRequest) HasPathname() bool`

HasPathname returns a boolean if a field has been set.

### GetPath

`func (o *MultiRoleSimulateAppPermissionsRequest) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *MultiRoleSimulateAppPermissionsRequest) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *MultiRoleSimulateAppPermissionsRequest) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *MultiRoleSimulateAppPermissionsRequest) HasPath() bool`

HasPath returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



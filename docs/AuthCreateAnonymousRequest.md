# AuthCreateAnonymousRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProjectId** | Pointer to **string** | Project ID for the anonymous session | [optional] 
**DeviceId** | Pointer to **string** | Optional device identifier | [optional] 

## Methods

### NewAuthCreateAnonymousRequest

`func NewAuthCreateAnonymousRequest() *AuthCreateAnonymousRequest`

NewAuthCreateAnonymousRequest instantiates a new AuthCreateAnonymousRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthCreateAnonymousRequestWithDefaults

`func NewAuthCreateAnonymousRequestWithDefaults() *AuthCreateAnonymousRequest`

NewAuthCreateAnonymousRequestWithDefaults instantiates a new AuthCreateAnonymousRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProjectId

`func (o *AuthCreateAnonymousRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *AuthCreateAnonymousRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *AuthCreateAnonymousRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *AuthCreateAnonymousRequest) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.

### GetDeviceId

`func (o *AuthCreateAnonymousRequest) GetDeviceId() string`

GetDeviceId returns the DeviceId field if non-nil, zero value otherwise.

### GetDeviceIdOk

`func (o *AuthCreateAnonymousRequest) GetDeviceIdOk() (*string, bool)`

GetDeviceIdOk returns a tuple with the DeviceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceId

`func (o *AuthCreateAnonymousRequest) SetDeviceId(v string)`

SetDeviceId sets DeviceId field to given value.

### HasDeviceId

`func (o *AuthCreateAnonymousRequest) HasDeviceId() bool`

HasDeviceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# DeviceToken

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | Pointer to **string** |  | [optional] 
**Platform** | Pointer to **string** |  | [optional] 
**LastSeenAt** | Pointer to **time.Time** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewDeviceToken

`func NewDeviceToken() *DeviceToken`

NewDeviceToken instantiates a new DeviceToken object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceTokenWithDefaults

`func NewDeviceTokenWithDefaults() *DeviceToken`

NewDeviceTokenWithDefaults instantiates a new DeviceToken object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *DeviceToken) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *DeviceToken) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *DeviceToken) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *DeviceToken) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetPlatform

`func (o *DeviceToken) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *DeviceToken) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *DeviceToken) SetPlatform(v string)`

SetPlatform sets Platform field to given value.

### HasPlatform

`func (o *DeviceToken) HasPlatform() bool`

HasPlatform returns a boolean if a field has been set.

### GetLastSeenAt

`func (o *DeviceToken) GetLastSeenAt() time.Time`

GetLastSeenAt returns the LastSeenAt field if non-nil, zero value otherwise.

### GetLastSeenAtOk

`func (o *DeviceToken) GetLastSeenAtOk() (*time.Time, bool)`

GetLastSeenAtOk returns a tuple with the LastSeenAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenAt

`func (o *DeviceToken) SetLastSeenAt(v time.Time)`

SetLastSeenAt sets LastSeenAt field to given value.

### HasLastSeenAt

`func (o *DeviceToken) HasLastSeenAt() bool`

HasLastSeenAt returns a boolean if a field has been set.

### GetCreatedAt

`func (o *DeviceToken) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *DeviceToken) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *DeviceToken) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *DeviceToken) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



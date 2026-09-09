# DeviceRegisteredResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | Pointer to **string** |  | [optional] 
**Platform** | Pointer to **string** |  | [optional] 
**LastSeenAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewDeviceRegisteredResponseData

`func NewDeviceRegisteredResponseData() *DeviceRegisteredResponseData`

NewDeviceRegisteredResponseData instantiates a new DeviceRegisteredResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceRegisteredResponseDataWithDefaults

`func NewDeviceRegisteredResponseDataWithDefaults() *DeviceRegisteredResponseData`

NewDeviceRegisteredResponseDataWithDefaults instantiates a new DeviceRegisteredResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *DeviceRegisteredResponseData) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *DeviceRegisteredResponseData) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *DeviceRegisteredResponseData) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *DeviceRegisteredResponseData) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetPlatform

`func (o *DeviceRegisteredResponseData) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *DeviceRegisteredResponseData) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *DeviceRegisteredResponseData) SetPlatform(v string)`

SetPlatform sets Platform field to given value.

### HasPlatform

`func (o *DeviceRegisteredResponseData) HasPlatform() bool`

HasPlatform returns a boolean if a field has been set.

### GetLastSeenAt

`func (o *DeviceRegisteredResponseData) GetLastSeenAt() time.Time`

GetLastSeenAt returns the LastSeenAt field if non-nil, zero value otherwise.

### GetLastSeenAtOk

`func (o *DeviceRegisteredResponseData) GetLastSeenAtOk() (*time.Time, bool)`

GetLastSeenAtOk returns a tuple with the LastSeenAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenAt

`func (o *DeviceRegisteredResponseData) SetLastSeenAt(v time.Time)`

SetLastSeenAt sets LastSeenAt field to given value.

### HasLastSeenAt

`func (o *DeviceRegisteredResponseData) HasLastSeenAt() bool`

HasLastSeenAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



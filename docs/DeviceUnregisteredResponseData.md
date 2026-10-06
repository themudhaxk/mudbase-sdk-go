# DeviceUnregisteredResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Removed** | Pointer to **bool** | True if a matching token was removed; false if none was registered. | [optional] 

## Methods

### NewDeviceUnregisteredResponseData

`func NewDeviceUnregisteredResponseData() *DeviceUnregisteredResponseData`

NewDeviceUnregisteredResponseData instantiates a new DeviceUnregisteredResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceUnregisteredResponseDataWithDefaults

`func NewDeviceUnregisteredResponseDataWithDefaults() *DeviceUnregisteredResponseData`

NewDeviceUnregisteredResponseDataWithDefaults instantiates a new DeviceUnregisteredResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRemoved

`func (o *DeviceUnregisteredResponseData) GetRemoved() bool`

GetRemoved returns the Removed field if non-nil, zero value otherwise.

### GetRemovedOk

`func (o *DeviceUnregisteredResponseData) GetRemovedOk() (*bool, bool)`

GetRemovedOk returns a tuple with the Removed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoved

`func (o *DeviceUnregisteredResponseData) SetRemoved(v bool)`

SetRemoved sets Removed field to given value.

### HasRemoved

`func (o *DeviceUnregisteredResponseData) HasRemoved() bool`

HasRemoved returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



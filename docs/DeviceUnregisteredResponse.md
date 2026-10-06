# DeviceUnregisteredResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**DeviceUnregisteredResponseData**](DeviceUnregisteredResponseData.md) |  | [optional] 

## Methods

### NewDeviceUnregisteredResponse

`func NewDeviceUnregisteredResponse() *DeviceUnregisteredResponse`

NewDeviceUnregisteredResponse instantiates a new DeviceUnregisteredResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceUnregisteredResponseWithDefaults

`func NewDeviceUnregisteredResponseWithDefaults() *DeviceUnregisteredResponse`

NewDeviceUnregisteredResponseWithDefaults instantiates a new DeviceUnregisteredResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *DeviceUnregisteredResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *DeviceUnregisteredResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *DeviceUnregisteredResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *DeviceUnregisteredResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *DeviceUnregisteredResponse) GetData() DeviceUnregisteredResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DeviceUnregisteredResponse) GetDataOk() (*DeviceUnregisteredResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DeviceUnregisteredResponse) SetData(v DeviceUnregisteredResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *DeviceUnregisteredResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# DeviceRegisteredResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**DeviceRegisteredResponseData**](DeviceRegisteredResponseData.md) |  | [optional] 

## Methods

### NewDeviceRegisteredResponse

`func NewDeviceRegisteredResponse() *DeviceRegisteredResponse`

NewDeviceRegisteredResponse instantiates a new DeviceRegisteredResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceRegisteredResponseWithDefaults

`func NewDeviceRegisteredResponseWithDefaults() *DeviceRegisteredResponse`

NewDeviceRegisteredResponseWithDefaults instantiates a new DeviceRegisteredResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *DeviceRegisteredResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *DeviceRegisteredResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *DeviceRegisteredResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *DeviceRegisteredResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *DeviceRegisteredResponse) GetData() DeviceRegisteredResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DeviceRegisteredResponse) GetDataOk() (*DeviceRegisteredResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DeviceRegisteredResponse) SetData(v DeviceRegisteredResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *DeviceRegisteredResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



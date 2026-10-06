# DeviceListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**[]DeviceToken**](DeviceToken.md) |  | [optional] 

## Methods

### NewDeviceListResponse

`func NewDeviceListResponse() *DeviceListResponse`

NewDeviceListResponse instantiates a new DeviceListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceListResponseWithDefaults

`func NewDeviceListResponseWithDefaults() *DeviceListResponse`

NewDeviceListResponseWithDefaults instantiates a new DeviceListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *DeviceListResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *DeviceListResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *DeviceListResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *DeviceListResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *DeviceListResponse) GetData() []DeviceToken`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DeviceListResponse) GetDataOk() (*[]DeviceToken, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DeviceListResponse) SetData(v []DeviceToken)`

SetData sets Data field to given value.

### HasData

`func (o *DeviceListResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WebPushConfigResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WebPushConfigResponseData**](WebPushConfigResponseData.md) |  | [optional] 

## Methods

### NewWebPushConfigResponse

`func NewWebPushConfigResponse() *WebPushConfigResponse`

NewWebPushConfigResponse instantiates a new WebPushConfigResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushConfigResponseWithDefaults

`func NewWebPushConfigResponseWithDefaults() *WebPushConfigResponse`

NewWebPushConfigResponseWithDefaults instantiates a new WebPushConfigResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WebPushConfigResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WebPushConfigResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WebPushConfigResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WebPushConfigResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WebPushConfigResponse) GetData() WebPushConfigResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebPushConfigResponse) GetDataOk() (*WebPushConfigResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebPushConfigResponse) SetData(v WebPushConfigResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *WebPushConfigResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



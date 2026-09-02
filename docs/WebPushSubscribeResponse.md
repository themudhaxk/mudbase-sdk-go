# WebPushSubscribeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WebPushSubscribeResponseData**](WebPushSubscribeResponseData.md) |  | [optional] 

## Methods

### NewWebPushSubscribeResponse

`func NewWebPushSubscribeResponse() *WebPushSubscribeResponse`

NewWebPushSubscribeResponse instantiates a new WebPushSubscribeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushSubscribeResponseWithDefaults

`func NewWebPushSubscribeResponseWithDefaults() *WebPushSubscribeResponse`

NewWebPushSubscribeResponseWithDefaults instantiates a new WebPushSubscribeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WebPushSubscribeResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WebPushSubscribeResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WebPushSubscribeResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WebPushSubscribeResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WebPushSubscribeResponse) GetData() WebPushSubscribeResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebPushSubscribeResponse) GetDataOk() (*WebPushSubscribeResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebPushSubscribeResponse) SetData(v WebPushSubscribeResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *WebPushSubscribeResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



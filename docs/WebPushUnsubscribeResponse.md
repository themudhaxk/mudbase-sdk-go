# WebPushUnsubscribeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WebPushUnsubscribeResponseData**](WebPushUnsubscribeResponseData.md) |  | [optional] 

## Methods

### NewWebPushUnsubscribeResponse

`func NewWebPushUnsubscribeResponse() *WebPushUnsubscribeResponse`

NewWebPushUnsubscribeResponse instantiates a new WebPushUnsubscribeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushUnsubscribeResponseWithDefaults

`func NewWebPushUnsubscribeResponseWithDefaults() *WebPushUnsubscribeResponse`

NewWebPushUnsubscribeResponseWithDefaults instantiates a new WebPushUnsubscribeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WebPushUnsubscribeResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WebPushUnsubscribeResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WebPushUnsubscribeResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WebPushUnsubscribeResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WebPushUnsubscribeResponse) GetData() WebPushUnsubscribeResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebPushUnsubscribeResponse) GetDataOk() (*WebPushUnsubscribeResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebPushUnsubscribeResponse) SetData(v WebPushUnsubscribeResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *WebPushUnsubscribeResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



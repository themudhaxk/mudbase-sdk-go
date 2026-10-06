# WebPushPublicKeyResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to [**WebPushPublicKeyResponseData**](WebPushPublicKeyResponseData.md) |  | [optional] 

## Methods

### NewWebPushPublicKeyResponse

`func NewWebPushPublicKeyResponse() *WebPushPublicKeyResponse`

NewWebPushPublicKeyResponse instantiates a new WebPushPublicKeyResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushPublicKeyResponseWithDefaults

`func NewWebPushPublicKeyResponseWithDefaults() *WebPushPublicKeyResponse`

NewWebPushPublicKeyResponseWithDefaults instantiates a new WebPushPublicKeyResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *WebPushPublicKeyResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WebPushPublicKeyResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WebPushPublicKeyResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *WebPushPublicKeyResponse) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetData

`func (o *WebPushPublicKeyResponse) GetData() WebPushPublicKeyResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebPushPublicKeyResponse) GetDataOk() (*WebPushPublicKeyResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebPushPublicKeyResponse) SetData(v WebPushPublicKeyResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *WebPushPublicKeyResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



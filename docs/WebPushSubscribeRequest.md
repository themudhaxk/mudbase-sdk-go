# WebPushSubscribeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subscription** | [**WebPushSubscription**](WebPushSubscription.md) |  | 
**UserId** | Pointer to **string** | Optional end-user id to associate with this subscription, for targeted sends. | [optional] 
**DeviceId** | Pointer to **string** | Optional client-supplied device identifier. | [optional] 

## Methods

### NewWebPushSubscribeRequest

`func NewWebPushSubscribeRequest(subscription WebPushSubscription, ) *WebPushSubscribeRequest`

NewWebPushSubscribeRequest instantiates a new WebPushSubscribeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushSubscribeRequestWithDefaults

`func NewWebPushSubscribeRequestWithDefaults() *WebPushSubscribeRequest`

NewWebPushSubscribeRequestWithDefaults instantiates a new WebPushSubscribeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubscription

`func (o *WebPushSubscribeRequest) GetSubscription() WebPushSubscription`

GetSubscription returns the Subscription field if non-nil, zero value otherwise.

### GetSubscriptionOk

`func (o *WebPushSubscribeRequest) GetSubscriptionOk() (*WebPushSubscription, bool)`

GetSubscriptionOk returns a tuple with the Subscription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscription

`func (o *WebPushSubscribeRequest) SetSubscription(v WebPushSubscription)`

SetSubscription sets Subscription field to given value.


### GetUserId

`func (o *WebPushSubscribeRequest) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *WebPushSubscribeRequest) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *WebPushSubscribeRequest) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *WebPushSubscribeRequest) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetDeviceId

`func (o *WebPushSubscribeRequest) GetDeviceId() string`

GetDeviceId returns the DeviceId field if non-nil, zero value otherwise.

### GetDeviceIdOk

`func (o *WebPushSubscribeRequest) GetDeviceIdOk() (*string, bool)`

GetDeviceIdOk returns a tuple with the DeviceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceId

`func (o *WebPushSubscribeRequest) SetDeviceId(v string)`

SetDeviceId sets DeviceId field to given value.

### HasDeviceId

`func (o *WebPushSubscribeRequest) HasDeviceId() bool`

HasDeviceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



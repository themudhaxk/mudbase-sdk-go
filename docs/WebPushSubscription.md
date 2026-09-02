# WebPushSubscription

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Endpoint** | **string** | The push-service endpoint URL returned by &#x60;pushManager.subscribe()&#x60;. | 
**Keys** | [**WebPushSubscriptionKeys**](WebPushSubscriptionKeys.md) |  | 

## Methods

### NewWebPushSubscription

`func NewWebPushSubscription(endpoint string, keys WebPushSubscriptionKeys, ) *WebPushSubscription`

NewWebPushSubscription instantiates a new WebPushSubscription object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushSubscriptionWithDefaults

`func NewWebPushSubscriptionWithDefaults() *WebPushSubscription`

NewWebPushSubscriptionWithDefaults instantiates a new WebPushSubscription object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEndpoint

`func (o *WebPushSubscription) GetEndpoint() string`

GetEndpoint returns the Endpoint field if non-nil, zero value otherwise.

### GetEndpointOk

`func (o *WebPushSubscription) GetEndpointOk() (*string, bool)`

GetEndpointOk returns a tuple with the Endpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoint

`func (o *WebPushSubscription) SetEndpoint(v string)`

SetEndpoint sets Endpoint field to given value.


### GetKeys

`func (o *WebPushSubscription) GetKeys() WebPushSubscriptionKeys`

GetKeys returns the Keys field if non-nil, zero value otherwise.

### GetKeysOk

`func (o *WebPushSubscription) GetKeysOk() (*WebPushSubscriptionKeys, bool)`

GetKeysOk returns a tuple with the Keys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeys

`func (o *WebPushSubscription) SetKeys(v WebPushSubscriptionKeys)`

SetKeys sets Keys field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



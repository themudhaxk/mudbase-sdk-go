# WebPushSubscriptionKeys

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**P256dh** | **string** | The subscription&#39;s P-256 ECDH public key (base64url). | 
**Auth** | **string** | The subscription&#39;s auth secret (base64url). | 

## Methods

### NewWebPushSubscriptionKeys

`func NewWebPushSubscriptionKeys(p256dh string, auth string, ) *WebPushSubscriptionKeys`

NewWebPushSubscriptionKeys instantiates a new WebPushSubscriptionKeys object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushSubscriptionKeysWithDefaults

`func NewWebPushSubscriptionKeysWithDefaults() *WebPushSubscriptionKeys`

NewWebPushSubscriptionKeysWithDefaults instantiates a new WebPushSubscriptionKeys object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetP256dh

`func (o *WebPushSubscriptionKeys) GetP256dh() string`

GetP256dh returns the P256dh field if non-nil, zero value otherwise.

### GetP256dhOk

`func (o *WebPushSubscriptionKeys) GetP256dhOk() (*string, bool)`

GetP256dhOk returns a tuple with the P256dh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetP256dh

`func (o *WebPushSubscriptionKeys) SetP256dh(v string)`

SetP256dh sets P256dh field to given value.


### GetAuth

`func (o *WebPushSubscriptionKeys) GetAuth() string`

GetAuth returns the Auth field if non-nil, zero value otherwise.

### GetAuthOk

`func (o *WebPushSubscriptionKeys) GetAuthOk() (*string, bool)`

GetAuthOk returns a tuple with the Auth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuth

`func (o *WebPushSubscriptionKeys) SetAuth(v string)`

SetAuth sets Auth field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



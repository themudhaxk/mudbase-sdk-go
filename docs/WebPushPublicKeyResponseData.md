# WebPushPublicKeyResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**PublicKey** | Pointer to **NullableString** | The VAPID application-server public key, or null when native Web Push is not enabled.  | [optional] 

## Methods

### NewWebPushPublicKeyResponseData

`func NewWebPushPublicKeyResponseData() *WebPushPublicKeyResponseData`

NewWebPushPublicKeyResponseData instantiates a new WebPushPublicKeyResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushPublicKeyResponseDataWithDefaults

`func NewWebPushPublicKeyResponseDataWithDefaults() *WebPushPublicKeyResponseData`

NewWebPushPublicKeyResponseDataWithDefaults instantiates a new WebPushPublicKeyResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *WebPushPublicKeyResponseData) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *WebPushPublicKeyResponseData) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *WebPushPublicKeyResponseData) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *WebPushPublicKeyResponseData) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetPublicKey

`func (o *WebPushPublicKeyResponseData) GetPublicKey() string`

GetPublicKey returns the PublicKey field if non-nil, zero value otherwise.

### GetPublicKeyOk

`func (o *WebPushPublicKeyResponseData) GetPublicKeyOk() (*string, bool)`

GetPublicKeyOk returns a tuple with the PublicKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublicKey

`func (o *WebPushPublicKeyResponseData) SetPublicKey(v string)`

SetPublicKey sets PublicKey field to given value.

### HasPublicKey

`func (o *WebPushPublicKeyResponseData) HasPublicKey() bool`

HasPublicKey returns a boolean if a field has been set.

### SetPublicKeyNil

`func (o *WebPushPublicKeyResponseData) SetPublicKeyNil(b bool)`

 SetPublicKeyNil sets the value for PublicKey to be an explicit nil

### UnsetPublicKey
`func (o *WebPushPublicKeyResponseData) UnsetPublicKey()`

UnsetPublicKey ensures that no value is present for PublicKey, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



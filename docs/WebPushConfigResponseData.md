# WebPushConfigResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Whether native Web Push is enabled for this project. | [optional] 
**HasKeys** | Pointer to **bool** | Whether a VAPID keypair has been provisioned. | [optional] 
**PublicKey** | Pointer to **NullableString** | The VAPID application-server public key clients subscribe with. Null when native Web Push is not enabled.  | [optional] 
**VapidSubject** | Pointer to **NullableString** | RFC 8292 contact subject (a &#x60;mailto:&#x60; address or &#x60;https&#x60; URL). | [optional] 
**GeneratedAt** | Pointer to **NullableTime** | When the current VAPID keypair was generated. | [optional] 

## Methods

### NewWebPushConfigResponseData

`func NewWebPushConfigResponseData() *WebPushConfigResponseData`

NewWebPushConfigResponseData instantiates a new WebPushConfigResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushConfigResponseDataWithDefaults

`func NewWebPushConfigResponseDataWithDefaults() *WebPushConfigResponseData`

NewWebPushConfigResponseDataWithDefaults instantiates a new WebPushConfigResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *WebPushConfigResponseData) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *WebPushConfigResponseData) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *WebPushConfigResponseData) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *WebPushConfigResponseData) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetHasKeys

`func (o *WebPushConfigResponseData) GetHasKeys() bool`

GetHasKeys returns the HasKeys field if non-nil, zero value otherwise.

### GetHasKeysOk

`func (o *WebPushConfigResponseData) GetHasKeysOk() (*bool, bool)`

GetHasKeysOk returns a tuple with the HasKeys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasKeys

`func (o *WebPushConfigResponseData) SetHasKeys(v bool)`

SetHasKeys sets HasKeys field to given value.

### HasHasKeys

`func (o *WebPushConfigResponseData) HasHasKeys() bool`

HasHasKeys returns a boolean if a field has been set.

### GetPublicKey

`func (o *WebPushConfigResponseData) GetPublicKey() string`

GetPublicKey returns the PublicKey field if non-nil, zero value otherwise.

### GetPublicKeyOk

`func (o *WebPushConfigResponseData) GetPublicKeyOk() (*string, bool)`

GetPublicKeyOk returns a tuple with the PublicKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublicKey

`func (o *WebPushConfigResponseData) SetPublicKey(v string)`

SetPublicKey sets PublicKey field to given value.

### HasPublicKey

`func (o *WebPushConfigResponseData) HasPublicKey() bool`

HasPublicKey returns a boolean if a field has been set.

### SetPublicKeyNil

`func (o *WebPushConfigResponseData) SetPublicKeyNil(b bool)`

 SetPublicKeyNil sets the value for PublicKey to be an explicit nil

### UnsetPublicKey
`func (o *WebPushConfigResponseData) UnsetPublicKey()`

UnsetPublicKey ensures that no value is present for PublicKey, not even an explicit nil
### GetVapidSubject

`func (o *WebPushConfigResponseData) GetVapidSubject() string`

GetVapidSubject returns the VapidSubject field if non-nil, zero value otherwise.

### GetVapidSubjectOk

`func (o *WebPushConfigResponseData) GetVapidSubjectOk() (*string, bool)`

GetVapidSubjectOk returns a tuple with the VapidSubject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVapidSubject

`func (o *WebPushConfigResponseData) SetVapidSubject(v string)`

SetVapidSubject sets VapidSubject field to given value.

### HasVapidSubject

`func (o *WebPushConfigResponseData) HasVapidSubject() bool`

HasVapidSubject returns a boolean if a field has been set.

### SetVapidSubjectNil

`func (o *WebPushConfigResponseData) SetVapidSubjectNil(b bool)`

 SetVapidSubjectNil sets the value for VapidSubject to be an explicit nil

### UnsetVapidSubject
`func (o *WebPushConfigResponseData) UnsetVapidSubject()`

UnsetVapidSubject ensures that no value is present for VapidSubject, not even an explicit nil
### GetGeneratedAt

`func (o *WebPushConfigResponseData) GetGeneratedAt() time.Time`

GetGeneratedAt returns the GeneratedAt field if non-nil, zero value otherwise.

### GetGeneratedAtOk

`func (o *WebPushConfigResponseData) GetGeneratedAtOk() (*time.Time, bool)`

GetGeneratedAtOk returns a tuple with the GeneratedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGeneratedAt

`func (o *WebPushConfigResponseData) SetGeneratedAt(v time.Time)`

SetGeneratedAt sets GeneratedAt field to given value.

### HasGeneratedAt

`func (o *WebPushConfigResponseData) HasGeneratedAt() bool`

HasGeneratedAt returns a boolean if a field has been set.

### SetGeneratedAtNil

`func (o *WebPushConfigResponseData) SetGeneratedAtNil(b bool)`

 SetGeneratedAtNil sets the value for GeneratedAt to be an explicit nil

### UnsetGeneratedAt
`func (o *WebPushConfigResponseData) UnsetGeneratedAt()`

UnsetGeneratedAt ensures that no value is present for GeneratedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



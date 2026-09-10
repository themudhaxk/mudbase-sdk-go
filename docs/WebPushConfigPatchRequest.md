# WebPushConfigPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**RotateKeys** | Pointer to **bool** |  | [optional] 
**Subject** | Pointer to **string** | A &#x60;mailto:&#x60; address or an &#x60;https&#x60; URL. | [optional] 

## Methods

### NewWebPushConfigPatchRequest

`func NewWebPushConfigPatchRequest() *WebPushConfigPatchRequest`

NewWebPushConfigPatchRequest instantiates a new WebPushConfigPatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushConfigPatchRequestWithDefaults

`func NewWebPushConfigPatchRequestWithDefaults() *WebPushConfigPatchRequest`

NewWebPushConfigPatchRequestWithDefaults instantiates a new WebPushConfigPatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *WebPushConfigPatchRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *WebPushConfigPatchRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *WebPushConfigPatchRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *WebPushConfigPatchRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetRotateKeys

`func (o *WebPushConfigPatchRequest) GetRotateKeys() bool`

GetRotateKeys returns the RotateKeys field if non-nil, zero value otherwise.

### GetRotateKeysOk

`func (o *WebPushConfigPatchRequest) GetRotateKeysOk() (*bool, bool)`

GetRotateKeysOk returns a tuple with the RotateKeys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRotateKeys

`func (o *WebPushConfigPatchRequest) SetRotateKeys(v bool)`

SetRotateKeys sets RotateKeys field to given value.

### HasRotateKeys

`func (o *WebPushConfigPatchRequest) HasRotateKeys() bool`

HasRotateKeys returns a boolean if a field has been set.

### GetSubject

`func (o *WebPushConfigPatchRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *WebPushConfigPatchRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *WebPushConfigPatchRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *WebPushConfigPatchRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



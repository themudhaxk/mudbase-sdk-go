# WebPushSubscribeResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Endpoint** | Pointer to **string** |  | [optional] 
**UserId** | Pointer to **NullableString** |  | [optional] 
**LastSeenAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewWebPushSubscribeResponseData

`func NewWebPushSubscribeResponseData() *WebPushSubscribeResponseData`

NewWebPushSubscribeResponseData instantiates a new WebPushSubscribeResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebPushSubscribeResponseDataWithDefaults

`func NewWebPushSubscribeResponseDataWithDefaults() *WebPushSubscribeResponseData`

NewWebPushSubscribeResponseDataWithDefaults instantiates a new WebPushSubscribeResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEndpoint

`func (o *WebPushSubscribeResponseData) GetEndpoint() string`

GetEndpoint returns the Endpoint field if non-nil, zero value otherwise.

### GetEndpointOk

`func (o *WebPushSubscribeResponseData) GetEndpointOk() (*string, bool)`

GetEndpointOk returns a tuple with the Endpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoint

`func (o *WebPushSubscribeResponseData) SetEndpoint(v string)`

SetEndpoint sets Endpoint field to given value.

### HasEndpoint

`func (o *WebPushSubscribeResponseData) HasEndpoint() bool`

HasEndpoint returns a boolean if a field has been set.

### GetUserId

`func (o *WebPushSubscribeResponseData) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *WebPushSubscribeResponseData) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *WebPushSubscribeResponseData) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *WebPushSubscribeResponseData) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### SetUserIdNil

`func (o *WebPushSubscribeResponseData) SetUserIdNil(b bool)`

 SetUserIdNil sets the value for UserId to be an explicit nil

### UnsetUserId
`func (o *WebPushSubscribeResponseData) UnsetUserId()`

UnsetUserId ensures that no value is present for UserId, not even an explicit nil
### GetLastSeenAt

`func (o *WebPushSubscribeResponseData) GetLastSeenAt() time.Time`

GetLastSeenAt returns the LastSeenAt field if non-nil, zero value otherwise.

### GetLastSeenAtOk

`func (o *WebPushSubscribeResponseData) GetLastSeenAtOk() (*time.Time, bool)`

GetLastSeenAtOk returns a tuple with the LastSeenAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenAt

`func (o *WebPushSubscribeResponseData) SetLastSeenAt(v time.Time)`

SetLastSeenAt sets LastSeenAt field to given value.

### HasLastSeenAt

`func (o *WebPushSubscribeResponseData) HasLastSeenAt() bool`

HasLastSeenAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



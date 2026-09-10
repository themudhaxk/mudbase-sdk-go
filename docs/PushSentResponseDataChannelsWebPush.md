# PushSentResponseDataChannelsWebPush

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SuccessCount** | Pointer to **int32** |  | [optional] 
**FailureCount** | Pointer to **int32** |  | [optional] 
**Pruned** | Pointer to **int32** | Subscriptions the push service reported as gone (404/410) and that were pruned during this send.  | [optional] 

## Methods

### NewPushSentResponseDataChannelsWebPush

`func NewPushSentResponseDataChannelsWebPush() *PushSentResponseDataChannelsWebPush`

NewPushSentResponseDataChannelsWebPush instantiates a new PushSentResponseDataChannelsWebPush object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPushSentResponseDataChannelsWebPushWithDefaults

`func NewPushSentResponseDataChannelsWebPushWithDefaults() *PushSentResponseDataChannelsWebPush`

NewPushSentResponseDataChannelsWebPushWithDefaults instantiates a new PushSentResponseDataChannelsWebPush object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccessCount

`func (o *PushSentResponseDataChannelsWebPush) GetSuccessCount() int32`

GetSuccessCount returns the SuccessCount field if non-nil, zero value otherwise.

### GetSuccessCountOk

`func (o *PushSentResponseDataChannelsWebPush) GetSuccessCountOk() (*int32, bool)`

GetSuccessCountOk returns a tuple with the SuccessCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccessCount

`func (o *PushSentResponseDataChannelsWebPush) SetSuccessCount(v int32)`

SetSuccessCount sets SuccessCount field to given value.

### HasSuccessCount

`func (o *PushSentResponseDataChannelsWebPush) HasSuccessCount() bool`

HasSuccessCount returns a boolean if a field has been set.

### GetFailureCount

`func (o *PushSentResponseDataChannelsWebPush) GetFailureCount() int32`

GetFailureCount returns the FailureCount field if non-nil, zero value otherwise.

### GetFailureCountOk

`func (o *PushSentResponseDataChannelsWebPush) GetFailureCountOk() (*int32, bool)`

GetFailureCountOk returns a tuple with the FailureCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailureCount

`func (o *PushSentResponseDataChannelsWebPush) SetFailureCount(v int32)`

SetFailureCount sets FailureCount field to given value.

### HasFailureCount

`func (o *PushSentResponseDataChannelsWebPush) HasFailureCount() bool`

HasFailureCount returns a boolean if a field has been set.

### GetPruned

`func (o *PushSentResponseDataChannelsWebPush) GetPruned() int32`

GetPruned returns the Pruned field if non-nil, zero value otherwise.

### GetPrunedOk

`func (o *PushSentResponseDataChannelsWebPush) GetPrunedOk() (*int32, bool)`

GetPrunedOk returns a tuple with the Pruned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPruned

`func (o *PushSentResponseDataChannelsWebPush) SetPruned(v int32)`

SetPruned sets Pruned field to given value.

### HasPruned

`func (o *PushSentResponseDataChannelsWebPush) HasPruned() bool`

HasPruned returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



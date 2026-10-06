# PushSentResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** | True when at least one recipient across any channel was delivered to. | [optional] 
**MessageId** | Pointer to **string** |  | [optional] 
**SuccessCount** | Pointer to **int32** |  | [optional] 
**FailureCount** | Pointer to **int32** |  | [optional] 
**Channels** | Pointer to [**PushSentResponseDataChannels**](PushSentResponseDataChannels.md) |  | [optional] 
**RejectedTokens** | Pointer to **[]string** | Device tokens that were passed but are not registered to the project, and so were dropped. Omitted when empty.  | [optional] 

## Methods

### NewPushSentResponseData

`func NewPushSentResponseData() *PushSentResponseData`

NewPushSentResponseData instantiates a new PushSentResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPushSentResponseDataWithDefaults

`func NewPushSentResponseDataWithDefaults() *PushSentResponseData`

NewPushSentResponseDataWithDefaults instantiates a new PushSentResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *PushSentResponseData) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *PushSentResponseData) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *PushSentResponseData) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *PushSentResponseData) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetMessageId

`func (o *PushSentResponseData) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *PushSentResponseData) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *PushSentResponseData) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *PushSentResponseData) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetSuccessCount

`func (o *PushSentResponseData) GetSuccessCount() int32`

GetSuccessCount returns the SuccessCount field if non-nil, zero value otherwise.

### GetSuccessCountOk

`func (o *PushSentResponseData) GetSuccessCountOk() (*int32, bool)`

GetSuccessCountOk returns a tuple with the SuccessCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccessCount

`func (o *PushSentResponseData) SetSuccessCount(v int32)`

SetSuccessCount sets SuccessCount field to given value.

### HasSuccessCount

`func (o *PushSentResponseData) HasSuccessCount() bool`

HasSuccessCount returns a boolean if a field has been set.

### GetFailureCount

`func (o *PushSentResponseData) GetFailureCount() int32`

GetFailureCount returns the FailureCount field if non-nil, zero value otherwise.

### GetFailureCountOk

`func (o *PushSentResponseData) GetFailureCountOk() (*int32, bool)`

GetFailureCountOk returns a tuple with the FailureCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailureCount

`func (o *PushSentResponseData) SetFailureCount(v int32)`

SetFailureCount sets FailureCount field to given value.

### HasFailureCount

`func (o *PushSentResponseData) HasFailureCount() bool`

HasFailureCount returns a boolean if a field has been set.

### GetChannels

`func (o *PushSentResponseData) GetChannels() PushSentResponseDataChannels`

GetChannels returns the Channels field if non-nil, zero value otherwise.

### GetChannelsOk

`func (o *PushSentResponseData) GetChannelsOk() (*PushSentResponseDataChannels, bool)`

GetChannelsOk returns a tuple with the Channels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannels

`func (o *PushSentResponseData) SetChannels(v PushSentResponseDataChannels)`

SetChannels sets Channels field to given value.

### HasChannels

`func (o *PushSentResponseData) HasChannels() bool`

HasChannels returns a boolean if a field has been set.

### GetRejectedTokens

`func (o *PushSentResponseData) GetRejectedTokens() []string`

GetRejectedTokens returns the RejectedTokens field if non-nil, zero value otherwise.

### GetRejectedTokensOk

`func (o *PushSentResponseData) GetRejectedTokensOk() (*[]string, bool)`

GetRejectedTokensOk returns a tuple with the RejectedTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRejectedTokens

`func (o *PushSentResponseData) SetRejectedTokens(v []string)`

SetRejectedTokens sets RejectedTokens field to given value.

### HasRejectedTokens

`func (o *PushSentResponseData) HasRejectedTokens() bool`

HasRejectedTokens returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ChatAddParticipantRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | **string** |  | 
**Role** | Pointer to **string** |  | [optional] 

## Methods

### NewChatAddParticipantRequest

`func NewChatAddParticipantRequest(userId string, ) *ChatAddParticipantRequest`

NewChatAddParticipantRequest instantiates a new ChatAddParticipantRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatAddParticipantRequestWithDefaults

`func NewChatAddParticipantRequestWithDefaults() *ChatAddParticipantRequest`

NewChatAddParticipantRequestWithDefaults instantiates a new ChatAddParticipantRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *ChatAddParticipantRequest) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ChatAddParticipantRequest) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ChatAddParticipantRequest) SetUserId(v string)`

SetUserId sets UserId field to given value.


### GetRole

`func (o *ChatAddParticipantRequest) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *ChatAddParticipantRequest) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *ChatAddParticipantRequest) SetRole(v string)`

SetRole sets Role field to given value.

### HasRole

`func (o *ChatAddParticipantRequest) HasRole() bool`

HasRole returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# UsersEraseDataRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Confirmation** | **string** |  | 
**Reason** | Pointer to **string** | Optional reason for account deletion | [optional] 

## Methods

### NewUsersEraseDataRequest

`func NewUsersEraseDataRequest(confirmation string, ) *UsersEraseDataRequest`

NewUsersEraseDataRequest instantiates a new UsersEraseDataRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsersEraseDataRequestWithDefaults

`func NewUsersEraseDataRequestWithDefaults() *UsersEraseDataRequest`

NewUsersEraseDataRequestWithDefaults instantiates a new UsersEraseDataRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConfirmation

`func (o *UsersEraseDataRequest) GetConfirmation() string`

GetConfirmation returns the Confirmation field if non-nil, zero value otherwise.

### GetConfirmationOk

`func (o *UsersEraseDataRequest) GetConfirmationOk() (*string, bool)`

GetConfirmationOk returns a tuple with the Confirmation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfirmation

`func (o *UsersEraseDataRequest) SetConfirmation(v string)`

SetConfirmation sets Confirmation field to given value.


### GetReason

`func (o *UsersEraseDataRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *UsersEraseDataRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *UsersEraseDataRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *UsersEraseDataRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



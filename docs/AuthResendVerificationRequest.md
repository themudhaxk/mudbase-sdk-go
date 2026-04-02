# AuthResendVerificationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**ProjectId** | Pointer to **string** | Optional; for project-scoped signup (sends link with project context) | [optional] 

## Methods

### NewAuthResendVerificationRequest

`func NewAuthResendVerificationRequest(email string, ) *AuthResendVerificationRequest`

NewAuthResendVerificationRequest instantiates a new AuthResendVerificationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthResendVerificationRequestWithDefaults

`func NewAuthResendVerificationRequestWithDefaults() *AuthResendVerificationRequest`

NewAuthResendVerificationRequestWithDefaults instantiates a new AuthResendVerificationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *AuthResendVerificationRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AuthResendVerificationRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AuthResendVerificationRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetProjectId

`func (o *AuthResendVerificationRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *AuthResendVerificationRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *AuthResendVerificationRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *AuthResendVerificationRequest) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



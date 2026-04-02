# AuthConfirmPasswordResetRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**ProjectId** | **string** |  | 
**Otp** | **string** |  | 
**NewPassword** | **string** |  | 

## Methods

### NewAuthConfirmPasswordResetRequest

`func NewAuthConfirmPasswordResetRequest(email string, projectId string, otp string, newPassword string, ) *AuthConfirmPasswordResetRequest`

NewAuthConfirmPasswordResetRequest instantiates a new AuthConfirmPasswordResetRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthConfirmPasswordResetRequestWithDefaults

`func NewAuthConfirmPasswordResetRequestWithDefaults() *AuthConfirmPasswordResetRequest`

NewAuthConfirmPasswordResetRequestWithDefaults instantiates a new AuthConfirmPasswordResetRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *AuthConfirmPasswordResetRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AuthConfirmPasswordResetRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AuthConfirmPasswordResetRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetProjectId

`func (o *AuthConfirmPasswordResetRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *AuthConfirmPasswordResetRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *AuthConfirmPasswordResetRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetOtp

`func (o *AuthConfirmPasswordResetRequest) GetOtp() string`

GetOtp returns the Otp field if non-nil, zero value otherwise.

### GetOtpOk

`func (o *AuthConfirmPasswordResetRequest) GetOtpOk() (*string, bool)`

GetOtpOk returns a tuple with the Otp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOtp

`func (o *AuthConfirmPasswordResetRequest) SetOtp(v string)`

SetOtp sets Otp field to given value.


### GetNewPassword

`func (o *AuthConfirmPasswordResetRequest) GetNewPassword() string`

GetNewPassword returns the NewPassword field if non-nil, zero value otherwise.

### GetNewPasswordOk

`func (o *AuthConfirmPasswordResetRequest) GetNewPasswordOk() (*string, bool)`

GetNewPasswordOk returns a tuple with the NewPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewPassword

`func (o *AuthConfirmPasswordResetRequest) SetNewPassword(v string)`

SetNewPassword sets NewPassword field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AuthRegister201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | Pointer to **string** |  | [optional] 
**RequireVerification** | Pointer to **bool** | true when email verification is required; no token in response | [optional] 
**Token** | Pointer to **string** | Present only when requireEmailVerification is false | [optional] 
**RefreshToken** | Pointer to **string** | Present only when requireEmailVerification is false | [optional] 
**ExpiresIn** | Pointer to **int32** | Present only when token is returned | [optional] 
**User** | Pointer to [**AuthRegister201ResponseUser**](AuthRegister201ResponseUser.md) |  | [optional] 

## Methods

### NewAuthRegister201Response

`func NewAuthRegister201Response() *AuthRegister201Response`

NewAuthRegister201Response instantiates a new AuthRegister201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthRegister201ResponseWithDefaults

`func NewAuthRegister201ResponseWithDefaults() *AuthRegister201Response`

NewAuthRegister201ResponseWithDefaults instantiates a new AuthRegister201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *AuthRegister201Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *AuthRegister201Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *AuthRegister201Response) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *AuthRegister201Response) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetRequireVerification

`func (o *AuthRegister201Response) GetRequireVerification() bool`

GetRequireVerification returns the RequireVerification field if non-nil, zero value otherwise.

### GetRequireVerificationOk

`func (o *AuthRegister201Response) GetRequireVerificationOk() (*bool, bool)`

GetRequireVerificationOk returns a tuple with the RequireVerification field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequireVerification

`func (o *AuthRegister201Response) SetRequireVerification(v bool)`

SetRequireVerification sets RequireVerification field to given value.

### HasRequireVerification

`func (o *AuthRegister201Response) HasRequireVerification() bool`

HasRequireVerification returns a boolean if a field has been set.

### GetToken

`func (o *AuthRegister201Response) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *AuthRegister201Response) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *AuthRegister201Response) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *AuthRegister201Response) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetRefreshToken

`func (o *AuthRegister201Response) GetRefreshToken() string`

GetRefreshToken returns the RefreshToken field if non-nil, zero value otherwise.

### GetRefreshTokenOk

`func (o *AuthRegister201Response) GetRefreshTokenOk() (*string, bool)`

GetRefreshTokenOk returns a tuple with the RefreshToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshToken

`func (o *AuthRegister201Response) SetRefreshToken(v string)`

SetRefreshToken sets RefreshToken field to given value.

### HasRefreshToken

`func (o *AuthRegister201Response) HasRefreshToken() bool`

HasRefreshToken returns a boolean if a field has been set.

### GetExpiresIn

`func (o *AuthRegister201Response) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *AuthRegister201Response) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *AuthRegister201Response) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *AuthRegister201Response) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.

### GetUser

`func (o *AuthRegister201Response) GetUser() AuthRegister201ResponseUser`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *AuthRegister201Response) GetUserOk() (*AuthRegister201ResponseUser, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *AuthRegister201Response) SetUser(v AuthRegister201ResponseUser)`

SetUser sets User field to given value.

### HasUser

`func (o *AuthRegister201Response) HasUser() bool`

HasUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



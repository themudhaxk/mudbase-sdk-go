# AuthLogin403Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **string** |  | [optional] 
**Code** | Pointer to **string** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 

## Methods

### NewAuthLogin403Response

`func NewAuthLogin403Response() *AuthLogin403Response`

NewAuthLogin403Response instantiates a new AuthLogin403Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthLogin403ResponseWithDefaults

`func NewAuthLogin403ResponseWithDefaults() *AuthLogin403Response`

NewAuthLogin403ResponseWithDefaults instantiates a new AuthLogin403Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *AuthLogin403Response) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *AuthLogin403Response) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *AuthLogin403Response) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *AuthLogin403Response) HasError() bool`

HasError returns a boolean if a field has been set.

### GetCode

`func (o *AuthLogin403Response) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *AuthLogin403Response) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *AuthLogin403Response) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *AuthLogin403Response) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetMessage

`func (o *AuthLogin403Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *AuthLogin403Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *AuthLogin403Response) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *AuthLogin403Response) HasMessage() bool`

HasMessage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



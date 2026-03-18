# AuthRegister429Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | **string** | Exact error message from the backend | 
**Code** | Pointer to **string** |  | [optional] 
**Details** | Pointer to [**ErrorDetails**](ErrorDetails.md) |  | [optional] 
**Timestamp** | Pointer to **time.Time** |  | [optional] 
**Path** | Pointer to **string** |  | [optional] 
**RequestId** | Pointer to **string** |  | [optional] 
**RetryAfter** | Pointer to **int32** |  | [optional] 

## Methods

### NewAuthRegister429Response

`func NewAuthRegister429Response(error_ string, ) *AuthRegister429Response`

NewAuthRegister429Response instantiates a new AuthRegister429Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthRegister429ResponseWithDefaults

`func NewAuthRegister429ResponseWithDefaults() *AuthRegister429Response`

NewAuthRegister429ResponseWithDefaults instantiates a new AuthRegister429Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *AuthRegister429Response) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *AuthRegister429Response) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *AuthRegister429Response) SetError(v string)`

SetError sets Error field to given value.


### GetCode

`func (o *AuthRegister429Response) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *AuthRegister429Response) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *AuthRegister429Response) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *AuthRegister429Response) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetDetails

`func (o *AuthRegister429Response) GetDetails() ErrorDetails`

GetDetails returns the Details field if non-nil, zero value otherwise.

### GetDetailsOk

`func (o *AuthRegister429Response) GetDetailsOk() (*ErrorDetails, bool)`

GetDetailsOk returns a tuple with the Details field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetails

`func (o *AuthRegister429Response) SetDetails(v ErrorDetails)`

SetDetails sets Details field to given value.

### HasDetails

`func (o *AuthRegister429Response) HasDetails() bool`

HasDetails returns a boolean if a field has been set.

### GetTimestamp

`func (o *AuthRegister429Response) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *AuthRegister429Response) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *AuthRegister429Response) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *AuthRegister429Response) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetPath

`func (o *AuthRegister429Response) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *AuthRegister429Response) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *AuthRegister429Response) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *AuthRegister429Response) HasPath() bool`

HasPath returns a boolean if a field has been set.

### GetRequestId

`func (o *AuthRegister429Response) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *AuthRegister429Response) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *AuthRegister429Response) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.

### HasRequestId

`func (o *AuthRegister429Response) HasRequestId() bool`

HasRequestId returns a boolean if a field has been set.

### GetRetryAfter

`func (o *AuthRegister429Response) GetRetryAfter() int32`

GetRetryAfter returns the RetryAfter field if non-nil, zero value otherwise.

### GetRetryAfterOk

`func (o *AuthRegister429Response) GetRetryAfterOk() (*int32, bool)`

GetRetryAfterOk returns a tuple with the RetryAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryAfter

`func (o *AuthRegister429Response) SetRetryAfter(v int32)`

SetRetryAfter sets RetryAfter field to given value.

### HasRetryAfter

`func (o *AuthRegister429Response) HasRetryAfter() bool`

HasRetryAfter returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



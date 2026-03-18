# FunctionExecutionResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Result** | Pointer to **map[string]interface{}** |  | [optional] 
**Error** | Pointer to **string** |  | [optional] 
**ExecutionTime** | Pointer to **int32** | Duration in milliseconds | [optional] 

## Methods

### NewFunctionExecutionResponseData

`func NewFunctionExecutionResponseData() *FunctionExecutionResponseData`

NewFunctionExecutionResponseData instantiates a new FunctionExecutionResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFunctionExecutionResponseDataWithDefaults

`func NewFunctionExecutionResponseDataWithDefaults() *FunctionExecutionResponseData`

NewFunctionExecutionResponseDataWithDefaults instantiates a new FunctionExecutionResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *FunctionExecutionResponseData) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *FunctionExecutionResponseData) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *FunctionExecutionResponseData) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *FunctionExecutionResponseData) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetResult

`func (o *FunctionExecutionResponseData) GetResult() map[string]interface{}`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *FunctionExecutionResponseData) GetResultOk() (*map[string]interface{}, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *FunctionExecutionResponseData) SetResult(v map[string]interface{})`

SetResult sets Result field to given value.

### HasResult

`func (o *FunctionExecutionResponseData) HasResult() bool`

HasResult returns a boolean if a field has been set.

### GetError

`func (o *FunctionExecutionResponseData) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *FunctionExecutionResponseData) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *FunctionExecutionResponseData) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *FunctionExecutionResponseData) HasError() bool`

HasError returns a boolean if a field has been set.

### GetExecutionTime

`func (o *FunctionExecutionResponseData) GetExecutionTime() int32`

GetExecutionTime returns the ExecutionTime field if non-nil, zero value otherwise.

### GetExecutionTimeOk

`func (o *FunctionExecutionResponseData) GetExecutionTimeOk() (*int32, bool)`

GetExecutionTimeOk returns a tuple with the ExecutionTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutionTime

`func (o *FunctionExecutionResponseData) SetExecutionTime(v int32)`

SetExecutionTime sets ExecutionTime field to given value.

### HasExecutionTime

`func (o *FunctionExecutionResponseData) HasExecutionTime() bool`

HasExecutionTime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



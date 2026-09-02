# ApiKycWorkflowsGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Workflows** | Pointer to [**[]ApiKycWorkflowsGet200ResponseWorkflowsInner**](ApiKycWorkflowsGet200ResponseWorkflowsInner.md) |  | [optional] 
**Kyc** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Kyb** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewApiKycWorkflowsGet200Response

`func NewApiKycWorkflowsGet200Response() *ApiKycWorkflowsGet200Response`

NewApiKycWorkflowsGet200Response instantiates a new ApiKycWorkflowsGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiKycWorkflowsGet200ResponseWithDefaults

`func NewApiKycWorkflowsGet200ResponseWithDefaults() *ApiKycWorkflowsGet200Response`

NewApiKycWorkflowsGet200ResponseWithDefaults instantiates a new ApiKycWorkflowsGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetWorkflows

`func (o *ApiKycWorkflowsGet200Response) GetWorkflows() []ApiKycWorkflowsGet200ResponseWorkflowsInner`

GetWorkflows returns the Workflows field if non-nil, zero value otherwise.

### GetWorkflowsOk

`func (o *ApiKycWorkflowsGet200Response) GetWorkflowsOk() (*[]ApiKycWorkflowsGet200ResponseWorkflowsInner, bool)`

GetWorkflowsOk returns a tuple with the Workflows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkflows

`func (o *ApiKycWorkflowsGet200Response) SetWorkflows(v []ApiKycWorkflowsGet200ResponseWorkflowsInner)`

SetWorkflows sets Workflows field to given value.

### HasWorkflows

`func (o *ApiKycWorkflowsGet200Response) HasWorkflows() bool`

HasWorkflows returns a boolean if a field has been set.

### GetKyc

`func (o *ApiKycWorkflowsGet200Response) GetKyc() []map[string]interface{}`

GetKyc returns the Kyc field if non-nil, zero value otherwise.

### GetKycOk

`func (o *ApiKycWorkflowsGet200Response) GetKycOk() (*[]map[string]interface{}, bool)`

GetKycOk returns a tuple with the Kyc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKyc

`func (o *ApiKycWorkflowsGet200Response) SetKyc(v []map[string]interface{})`

SetKyc sets Kyc field to given value.

### HasKyc

`func (o *ApiKycWorkflowsGet200Response) HasKyc() bool`

HasKyc returns a boolean if a field has been set.

### GetKyb

`func (o *ApiKycWorkflowsGet200Response) GetKyb() []map[string]interface{}`

GetKyb returns the Kyb field if non-nil, zero value otherwise.

### GetKybOk

`func (o *ApiKycWorkflowsGet200Response) GetKybOk() (*[]map[string]interface{}, bool)`

GetKybOk returns a tuple with the Kyb field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKyb

`func (o *ApiKycWorkflowsGet200Response) SetKyb(v []map[string]interface{})`

SetKyb sets Kyb field to given value.

### HasKyb

`func (o *ApiKycWorkflowsGet200Response) HasKyb() bool`

HasKyb returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



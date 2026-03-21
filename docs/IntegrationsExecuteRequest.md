# IntegrationsExecuteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Endpoint** | **string** |  | 
**Method** | **string** |  | 
**Params** | Pointer to **map[string]interface{}** |  | [optional] 
**Body** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewIntegrationsExecuteRequest

`func NewIntegrationsExecuteRequest(endpoint string, method string, ) *IntegrationsExecuteRequest`

NewIntegrationsExecuteRequest instantiates a new IntegrationsExecuteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIntegrationsExecuteRequestWithDefaults

`func NewIntegrationsExecuteRequestWithDefaults() *IntegrationsExecuteRequest`

NewIntegrationsExecuteRequestWithDefaults instantiates a new IntegrationsExecuteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEndpoint

`func (o *IntegrationsExecuteRequest) GetEndpoint() string`

GetEndpoint returns the Endpoint field if non-nil, zero value otherwise.

### GetEndpointOk

`func (o *IntegrationsExecuteRequest) GetEndpointOk() (*string, bool)`

GetEndpointOk returns a tuple with the Endpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoint

`func (o *IntegrationsExecuteRequest) SetEndpoint(v string)`

SetEndpoint sets Endpoint field to given value.


### GetMethod

`func (o *IntegrationsExecuteRequest) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *IntegrationsExecuteRequest) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *IntegrationsExecuteRequest) SetMethod(v string)`

SetMethod sets Method field to given value.


### GetParams

`func (o *IntegrationsExecuteRequest) GetParams() map[string]interface{}`

GetParams returns the Params field if non-nil, zero value otherwise.

### GetParamsOk

`func (o *IntegrationsExecuteRequest) GetParamsOk() (*map[string]interface{}, bool)`

GetParamsOk returns a tuple with the Params field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParams

`func (o *IntegrationsExecuteRequest) SetParams(v map[string]interface{})`

SetParams sets Params field to given value.

### HasParams

`func (o *IntegrationsExecuteRequest) HasParams() bool`

HasParams returns a boolean if a field has been set.

### GetBody

`func (o *IntegrationsExecuteRequest) GetBody() map[string]interface{}`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *IntegrationsExecuteRequest) GetBodyOk() (*map[string]interface{}, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *IntegrationsExecuteRequest) SetBody(v map[string]interface{})`

SetBody sets Body field to given value.

### HasBody

`func (o *IntegrationsExecuteRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



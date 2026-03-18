# FunctionsSimulateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Trigger** | Pointer to **map[string]interface{}** | Simulated trigger (type, event) | [optional] 
**EventContext** | Pointer to **map[string]interface{}** | Simulated event context (document, file, webhook, wallet, message) | [optional] 
**Payload** | Pointer to **map[string]interface{}** | Additional payload | [optional] 

## Methods

### NewFunctionsSimulateRequest

`func NewFunctionsSimulateRequest() *FunctionsSimulateRequest`

NewFunctionsSimulateRequest instantiates a new FunctionsSimulateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFunctionsSimulateRequestWithDefaults

`func NewFunctionsSimulateRequestWithDefaults() *FunctionsSimulateRequest`

NewFunctionsSimulateRequestWithDefaults instantiates a new FunctionsSimulateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTrigger

`func (o *FunctionsSimulateRequest) GetTrigger() map[string]interface{}`

GetTrigger returns the Trigger field if non-nil, zero value otherwise.

### GetTriggerOk

`func (o *FunctionsSimulateRequest) GetTriggerOk() (*map[string]interface{}, bool)`

GetTriggerOk returns a tuple with the Trigger field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrigger

`func (o *FunctionsSimulateRequest) SetTrigger(v map[string]interface{})`

SetTrigger sets Trigger field to given value.

### HasTrigger

`func (o *FunctionsSimulateRequest) HasTrigger() bool`

HasTrigger returns a boolean if a field has been set.

### GetEventContext

`func (o *FunctionsSimulateRequest) GetEventContext() map[string]interface{}`

GetEventContext returns the EventContext field if non-nil, zero value otherwise.

### GetEventContextOk

`func (o *FunctionsSimulateRequest) GetEventContextOk() (*map[string]interface{}, bool)`

GetEventContextOk returns a tuple with the EventContext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventContext

`func (o *FunctionsSimulateRequest) SetEventContext(v map[string]interface{})`

SetEventContext sets EventContext field to given value.

### HasEventContext

`func (o *FunctionsSimulateRequest) HasEventContext() bool`

HasEventContext returns a boolean if a field has been set.

### GetPayload

`func (o *FunctionsSimulateRequest) GetPayload() map[string]interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *FunctionsSimulateRequest) GetPayloadOk() (*map[string]interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *FunctionsSimulateRequest) SetPayload(v map[string]interface{})`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *FunctionsSimulateRequest) HasPayload() bool`

HasPayload returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



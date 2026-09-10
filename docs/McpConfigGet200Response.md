# McpConfigGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**Plan** | Pointer to **string** |  | [optional] 
**AllowedPlans** | Pointer to **[]string** |  | [optional] 
**FreePromoActive** | Pointer to **bool** | True if this org is on the free plan and MCP is temporarily enabled via the launch promo | [optional] 
**FreePromoEndsAt** | Pointer to **NullableTime** | When the free-plan MCP promo ends (null if not active) | [optional] 
**Endpoint** | Pointer to **string** |  | [optional] 
**Tools** | Pointer to [**[]McpConfigGet200ResponseToolsInner**](McpConfigGet200ResponseToolsInner.md) |  | [optional] 

## Methods

### NewMcpConfigGet200Response

`func NewMcpConfigGet200Response() *McpConfigGet200Response`

NewMcpConfigGet200Response instantiates a new McpConfigGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMcpConfigGet200ResponseWithDefaults

`func NewMcpConfigGet200ResponseWithDefaults() *McpConfigGet200Response`

NewMcpConfigGet200ResponseWithDefaults instantiates a new McpConfigGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *McpConfigGet200Response) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *McpConfigGet200Response) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *McpConfigGet200Response) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *McpConfigGet200Response) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetPlan

`func (o *McpConfigGet200Response) GetPlan() string`

GetPlan returns the Plan field if non-nil, zero value otherwise.

### GetPlanOk

`func (o *McpConfigGet200Response) GetPlanOk() (*string, bool)`

GetPlanOk returns a tuple with the Plan field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlan

`func (o *McpConfigGet200Response) SetPlan(v string)`

SetPlan sets Plan field to given value.

### HasPlan

`func (o *McpConfigGet200Response) HasPlan() bool`

HasPlan returns a boolean if a field has been set.

### GetAllowedPlans

`func (o *McpConfigGet200Response) GetAllowedPlans() []string`

GetAllowedPlans returns the AllowedPlans field if non-nil, zero value otherwise.

### GetAllowedPlansOk

`func (o *McpConfigGet200Response) GetAllowedPlansOk() (*[]string, bool)`

GetAllowedPlansOk returns a tuple with the AllowedPlans field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedPlans

`func (o *McpConfigGet200Response) SetAllowedPlans(v []string)`

SetAllowedPlans sets AllowedPlans field to given value.

### HasAllowedPlans

`func (o *McpConfigGet200Response) HasAllowedPlans() bool`

HasAllowedPlans returns a boolean if a field has been set.

### GetFreePromoActive

`func (o *McpConfigGet200Response) GetFreePromoActive() bool`

GetFreePromoActive returns the FreePromoActive field if non-nil, zero value otherwise.

### GetFreePromoActiveOk

`func (o *McpConfigGet200Response) GetFreePromoActiveOk() (*bool, bool)`

GetFreePromoActiveOk returns a tuple with the FreePromoActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFreePromoActive

`func (o *McpConfigGet200Response) SetFreePromoActive(v bool)`

SetFreePromoActive sets FreePromoActive field to given value.

### HasFreePromoActive

`func (o *McpConfigGet200Response) HasFreePromoActive() bool`

HasFreePromoActive returns a boolean if a field has been set.

### GetFreePromoEndsAt

`func (o *McpConfigGet200Response) GetFreePromoEndsAt() time.Time`

GetFreePromoEndsAt returns the FreePromoEndsAt field if non-nil, zero value otherwise.

### GetFreePromoEndsAtOk

`func (o *McpConfigGet200Response) GetFreePromoEndsAtOk() (*time.Time, bool)`

GetFreePromoEndsAtOk returns a tuple with the FreePromoEndsAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFreePromoEndsAt

`func (o *McpConfigGet200Response) SetFreePromoEndsAt(v time.Time)`

SetFreePromoEndsAt sets FreePromoEndsAt field to given value.

### HasFreePromoEndsAt

`func (o *McpConfigGet200Response) HasFreePromoEndsAt() bool`

HasFreePromoEndsAt returns a boolean if a field has been set.

### SetFreePromoEndsAtNil

`func (o *McpConfigGet200Response) SetFreePromoEndsAtNil(b bool)`

 SetFreePromoEndsAtNil sets the value for FreePromoEndsAt to be an explicit nil

### UnsetFreePromoEndsAt
`func (o *McpConfigGet200Response) UnsetFreePromoEndsAt()`

UnsetFreePromoEndsAt ensures that no value is present for FreePromoEndsAt, not even an explicit nil
### GetEndpoint

`func (o *McpConfigGet200Response) GetEndpoint() string`

GetEndpoint returns the Endpoint field if non-nil, zero value otherwise.

### GetEndpointOk

`func (o *McpConfigGet200Response) GetEndpointOk() (*string, bool)`

GetEndpointOk returns a tuple with the Endpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoint

`func (o *McpConfigGet200Response) SetEndpoint(v string)`

SetEndpoint sets Endpoint field to given value.

### HasEndpoint

`func (o *McpConfigGet200Response) HasEndpoint() bool`

HasEndpoint returns a boolean if a field has been set.

### GetTools

`func (o *McpConfigGet200Response) GetTools() []McpConfigGet200ResponseToolsInner`

GetTools returns the Tools field if non-nil, zero value otherwise.

### GetToolsOk

`func (o *McpConfigGet200Response) GetToolsOk() (*[]McpConfigGet200ResponseToolsInner, bool)`

GetToolsOk returns a tuple with the Tools field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTools

`func (o *McpConfigGet200Response) SetTools(v []McpConfigGet200ResponseToolsInner)`

SetTools sets Tools field to given value.

### HasTools

`func (o *McpConfigGet200Response) HasTools() bool`

HasTools returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



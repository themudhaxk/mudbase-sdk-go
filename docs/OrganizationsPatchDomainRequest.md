# OrganizationsPatchDomainRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | Pointer to **string** | Org self-serve only pending or failed. Live (active) is set by platform admin. | [optional] 
**RegenerateToken** | Pointer to **bool** |  | [optional] 

## Methods

### NewOrganizationsPatchDomainRequest

`func NewOrganizationsPatchDomainRequest() *OrganizationsPatchDomainRequest`

NewOrganizationsPatchDomainRequest instantiates a new OrganizationsPatchDomainRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationsPatchDomainRequestWithDefaults

`func NewOrganizationsPatchDomainRequestWithDefaults() *OrganizationsPatchDomainRequest`

NewOrganizationsPatchDomainRequestWithDefaults instantiates a new OrganizationsPatchDomainRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *OrganizationsPatchDomainRequest) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *OrganizationsPatchDomainRequest) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *OrganizationsPatchDomainRequest) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *OrganizationsPatchDomainRequest) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetRegenerateToken

`func (o *OrganizationsPatchDomainRequest) GetRegenerateToken() bool`

GetRegenerateToken returns the RegenerateToken field if non-nil, zero value otherwise.

### GetRegenerateTokenOk

`func (o *OrganizationsPatchDomainRequest) GetRegenerateTokenOk() (*bool, bool)`

GetRegenerateTokenOk returns a tuple with the RegenerateToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegenerateToken

`func (o *OrganizationsPatchDomainRequest) SetRegenerateToken(v bool)`

SetRegenerateToken sets RegenerateToken field to given value.

### HasRegenerateToken

`func (o *OrganizationsPatchDomainRequest) HasRegenerateToken() bool`

HasRegenerateToken returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



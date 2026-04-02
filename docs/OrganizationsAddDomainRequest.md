# OrganizationsAddDomainRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Hostname** | **string** |  | 
**SetPrimary** | Pointer to **bool** |  | [optional] 

## Methods

### NewOrganizationsAddDomainRequest

`func NewOrganizationsAddDomainRequest(hostname string, ) *OrganizationsAddDomainRequest`

NewOrganizationsAddDomainRequest instantiates a new OrganizationsAddDomainRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationsAddDomainRequestWithDefaults

`func NewOrganizationsAddDomainRequestWithDefaults() *OrganizationsAddDomainRequest`

NewOrganizationsAddDomainRequestWithDefaults instantiates a new OrganizationsAddDomainRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHostname

`func (o *OrganizationsAddDomainRequest) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *OrganizationsAddDomainRequest) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *OrganizationsAddDomainRequest) SetHostname(v string)`

SetHostname sets Hostname field to given value.


### GetSetPrimary

`func (o *OrganizationsAddDomainRequest) GetSetPrimary() bool`

GetSetPrimary returns the SetPrimary field if non-nil, zero value otherwise.

### GetSetPrimaryOk

`func (o *OrganizationsAddDomainRequest) GetSetPrimaryOk() (*bool, bool)`

GetSetPrimaryOk returns a tuple with the SetPrimary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSetPrimary

`func (o *OrganizationsAddDomainRequest) SetSetPrimary(v bool)`

SetSetPrimary sets SetPrimary field to given value.

### HasSetPrimary

`func (o *OrganizationsAddDomainRequest) HasSetPrimary() bool`

HasSetPrimary returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# RoleElevationUploadDocumentsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RoleSlug** | **string** |  | 
**Documents** | [**[]RoleElevationUploadDocumentsRequestDocumentsInner**](RoleElevationUploadDocumentsRequestDocumentsInner.md) |  | 

## Methods

### NewRoleElevationUploadDocumentsRequest

`func NewRoleElevationUploadDocumentsRequest(roleSlug string, documents []RoleElevationUploadDocumentsRequestDocumentsInner, ) *RoleElevationUploadDocumentsRequest`

NewRoleElevationUploadDocumentsRequest instantiates a new RoleElevationUploadDocumentsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoleElevationUploadDocumentsRequestWithDefaults

`func NewRoleElevationUploadDocumentsRequestWithDefaults() *RoleElevationUploadDocumentsRequest`

NewRoleElevationUploadDocumentsRequestWithDefaults instantiates a new RoleElevationUploadDocumentsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRoleSlug

`func (o *RoleElevationUploadDocumentsRequest) GetRoleSlug() string`

GetRoleSlug returns the RoleSlug field if non-nil, zero value otherwise.

### GetRoleSlugOk

`func (o *RoleElevationUploadDocumentsRequest) GetRoleSlugOk() (*string, bool)`

GetRoleSlugOk returns a tuple with the RoleSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoleSlug

`func (o *RoleElevationUploadDocumentsRequest) SetRoleSlug(v string)`

SetRoleSlug sets RoleSlug field to given value.


### GetDocuments

`func (o *RoleElevationUploadDocumentsRequest) GetDocuments() []RoleElevationUploadDocumentsRequestDocumentsInner`

GetDocuments returns the Documents field if non-nil, zero value otherwise.

### GetDocumentsOk

`func (o *RoleElevationUploadDocumentsRequest) GetDocumentsOk() (*[]RoleElevationUploadDocumentsRequestDocumentsInner, bool)`

GetDocumentsOk returns a tuple with the Documents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocuments

`func (o *RoleElevationUploadDocumentsRequest) SetDocuments(v []RoleElevationUploadDocumentsRequestDocumentsInner)`

SetDocuments sets Documents field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



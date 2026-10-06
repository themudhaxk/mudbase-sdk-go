# CreateBackupRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Description** | Pointer to **string** |  | [optional] 
**IncludeFiles** | Pointer to **bool** |  | [optional] [default to true]

## Methods

### NewCreateBackupRequest

`func NewCreateBackupRequest() *CreateBackupRequest`

NewCreateBackupRequest instantiates a new CreateBackupRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateBackupRequestWithDefaults

`func NewCreateBackupRequestWithDefaults() *CreateBackupRequest`

NewCreateBackupRequestWithDefaults instantiates a new CreateBackupRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDescription

`func (o *CreateBackupRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateBackupRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateBackupRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateBackupRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetIncludeFiles

`func (o *CreateBackupRequest) GetIncludeFiles() bool`

GetIncludeFiles returns the IncludeFiles field if non-nil, zero value otherwise.

### GetIncludeFilesOk

`func (o *CreateBackupRequest) GetIncludeFilesOk() (*bool, bool)`

GetIncludeFilesOk returns a tuple with the IncludeFiles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeFiles

`func (o *CreateBackupRequest) SetIncludeFiles(v bool)`

SetIncludeFiles sets IncludeFiles field to given value.

### HasIncludeFiles

`func (o *CreateBackupRequest) HasIncludeFiles() bool`

HasIncludeFiles returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



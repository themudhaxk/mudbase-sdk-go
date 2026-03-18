# StorageConfirmUploadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | **string** | The S3 object key returned when the presigned POST was issued | 
**ProjectId** | **string** |  | 
**OriginalName** | Pointer to **string** |  | [optional] 
**ContentType** | Pointer to **string** |  | [optional] 
**Size** | Pointer to **int32** |  | [optional] 
**Bucket** | Pointer to **string** |  | [optional] 
**IsPublic** | Pointer to **bool** |  | [optional] 

## Methods

### NewStorageConfirmUploadRequest

`func NewStorageConfirmUploadRequest(key string, projectId string, ) *StorageConfirmUploadRequest`

NewStorageConfirmUploadRequest instantiates a new StorageConfirmUploadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStorageConfirmUploadRequestWithDefaults

`func NewStorageConfirmUploadRequestWithDefaults() *StorageConfirmUploadRequest`

NewStorageConfirmUploadRequestWithDefaults instantiates a new StorageConfirmUploadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *StorageConfirmUploadRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *StorageConfirmUploadRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *StorageConfirmUploadRequest) SetKey(v string)`

SetKey sets Key field to given value.


### GetProjectId

`func (o *StorageConfirmUploadRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *StorageConfirmUploadRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *StorageConfirmUploadRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetOriginalName

`func (o *StorageConfirmUploadRequest) GetOriginalName() string`

GetOriginalName returns the OriginalName field if non-nil, zero value otherwise.

### GetOriginalNameOk

`func (o *StorageConfirmUploadRequest) GetOriginalNameOk() (*string, bool)`

GetOriginalNameOk returns a tuple with the OriginalName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalName

`func (o *StorageConfirmUploadRequest) SetOriginalName(v string)`

SetOriginalName sets OriginalName field to given value.

### HasOriginalName

`func (o *StorageConfirmUploadRequest) HasOriginalName() bool`

HasOriginalName returns a boolean if a field has been set.

### GetContentType

`func (o *StorageConfirmUploadRequest) GetContentType() string`

GetContentType returns the ContentType field if non-nil, zero value otherwise.

### GetContentTypeOk

`func (o *StorageConfirmUploadRequest) GetContentTypeOk() (*string, bool)`

GetContentTypeOk returns a tuple with the ContentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentType

`func (o *StorageConfirmUploadRequest) SetContentType(v string)`

SetContentType sets ContentType field to given value.

### HasContentType

`func (o *StorageConfirmUploadRequest) HasContentType() bool`

HasContentType returns a boolean if a field has been set.

### GetSize

`func (o *StorageConfirmUploadRequest) GetSize() int32`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *StorageConfirmUploadRequest) GetSizeOk() (*int32, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *StorageConfirmUploadRequest) SetSize(v int32)`

SetSize sets Size field to given value.

### HasSize

`func (o *StorageConfirmUploadRequest) HasSize() bool`

HasSize returns a boolean if a field has been set.

### GetBucket

`func (o *StorageConfirmUploadRequest) GetBucket() string`

GetBucket returns the Bucket field if non-nil, zero value otherwise.

### GetBucketOk

`func (o *StorageConfirmUploadRequest) GetBucketOk() (*string, bool)`

GetBucketOk returns a tuple with the Bucket field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucket

`func (o *StorageConfirmUploadRequest) SetBucket(v string)`

SetBucket sets Bucket field to given value.

### HasBucket

`func (o *StorageConfirmUploadRequest) HasBucket() bool`

HasBucket returns a boolean if a field has been set.

### GetIsPublic

`func (o *StorageConfirmUploadRequest) GetIsPublic() bool`

GetIsPublic returns the IsPublic field if non-nil, zero value otherwise.

### GetIsPublicOk

`func (o *StorageConfirmUploadRequest) GetIsPublicOk() (*bool, bool)`

GetIsPublicOk returns a tuple with the IsPublic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPublic

`func (o *StorageConfirmUploadRequest) SetIsPublic(v bool)`

SetIsPublic sets IsPublic field to given value.

### HasIsPublic

`func (o *StorageConfirmUploadRequest) HasIsPublic() bool`

HasIsPublic returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



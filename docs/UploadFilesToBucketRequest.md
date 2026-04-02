# UploadFilesToBucketRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Files** | **[]*os.File** |  | 
**Folder** | Pointer to **string** |  | [optional] 
**Tags** | Pointer to **[]string** |  | [optional] 

## Methods

### NewUploadFilesToBucketRequest

`func NewUploadFilesToBucketRequest(files []*os.File, ) *UploadFilesToBucketRequest`

NewUploadFilesToBucketRequest instantiates a new UploadFilesToBucketRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUploadFilesToBucketRequestWithDefaults

`func NewUploadFilesToBucketRequestWithDefaults() *UploadFilesToBucketRequest`

NewUploadFilesToBucketRequestWithDefaults instantiates a new UploadFilesToBucketRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFiles

`func (o *UploadFilesToBucketRequest) GetFiles() []*os.File`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *UploadFilesToBucketRequest) GetFilesOk() (*[]*os.File, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *UploadFilesToBucketRequest) SetFiles(v []*os.File)`

SetFiles sets Files field to given value.


### GetFolder

`func (o *UploadFilesToBucketRequest) GetFolder() string`

GetFolder returns the Folder field if non-nil, zero value otherwise.

### GetFolderOk

`func (o *UploadFilesToBucketRequest) GetFolderOk() (*string, bool)`

GetFolderOk returns a tuple with the Folder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolder

`func (o *UploadFilesToBucketRequest) SetFolder(v string)`

SetFolder sets Folder field to given value.

### HasFolder

`func (o *UploadFilesToBucketRequest) HasFolder() bool`

HasFolder returns a boolean if a field has been set.

### GetTags

`func (o *UploadFilesToBucketRequest) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *UploadFilesToBucketRequest) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *UploadFilesToBucketRequest) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *UploadFilesToBucketRequest) HasTags() bool`

HasTags returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



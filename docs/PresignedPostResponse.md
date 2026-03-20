# PresignedPostResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | Pointer to **string** | Object key (S3) clients should upload to | [optional] 
**Url** | Pointer to **string** | URL to POST the multipart form to | [optional] 
**Fields** | Pointer to **map[string]interface{}** | Form fields required for the presigned POST (Policy, X-Amz-Signature, etc.) | [optional] 
**ExpiresIn** | Pointer to **int32** | Expiration of the presigned POST in seconds | [optional] 

## Methods

### NewPresignedPostResponse

`func NewPresignedPostResponse() *PresignedPostResponse`

NewPresignedPostResponse instantiates a new PresignedPostResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPresignedPostResponseWithDefaults

`func NewPresignedPostResponseWithDefaults() *PresignedPostResponse`

NewPresignedPostResponseWithDefaults instantiates a new PresignedPostResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *PresignedPostResponse) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *PresignedPostResponse) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *PresignedPostResponse) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *PresignedPostResponse) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetUrl

`func (o *PresignedPostResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *PresignedPostResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *PresignedPostResponse) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *PresignedPostResponse) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetFields

`func (o *PresignedPostResponse) GetFields() map[string]interface{}`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *PresignedPostResponse) GetFieldsOk() (*map[string]interface{}, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *PresignedPostResponse) SetFields(v map[string]interface{})`

SetFields sets Fields field to given value.

### HasFields

`func (o *PresignedPostResponse) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetExpiresIn

`func (o *PresignedPostResponse) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *PresignedPostResponse) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *PresignedPostResponse) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *PresignedPostResponse) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



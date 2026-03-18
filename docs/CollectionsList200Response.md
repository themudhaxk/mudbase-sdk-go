# CollectionsList200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Collections** | Pointer to [**[]Collection**](Collection.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewCollectionsList200Response

`func NewCollectionsList200Response() *CollectionsList200Response`

NewCollectionsList200Response instantiates a new CollectionsList200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCollectionsList200ResponseWithDefaults

`func NewCollectionsList200ResponseWithDefaults() *CollectionsList200Response`

NewCollectionsList200ResponseWithDefaults instantiates a new CollectionsList200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCollections

`func (o *CollectionsList200Response) GetCollections() []Collection`

GetCollections returns the Collections field if non-nil, zero value otherwise.

### GetCollectionsOk

`func (o *CollectionsList200Response) GetCollectionsOk() (*[]Collection, bool)`

GetCollectionsOk returns a tuple with the Collections field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCollections

`func (o *CollectionsList200Response) SetCollections(v []Collection)`

SetCollections sets Collections field to given value.

### HasCollections

`func (o *CollectionsList200Response) HasCollections() bool`

HasCollections returns a boolean if a field has been set.

### GetTotal

`func (o *CollectionsList200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *CollectionsList200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *CollectionsList200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *CollectionsList200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



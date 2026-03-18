# SearchGetAnalytics200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalSearches** | Pointer to **int32** |  | [optional] 
**TopQueries** | Pointer to [**[]SearchGetAnalytics200ResponseTopQueriesInner**](SearchGetAnalytics200ResponseTopQueriesInner.md) |  | [optional] 
**SearchesByCollection** | Pointer to **map[string]interface{}** |  | [optional] 
**AverageResponseTime** | Pointer to **float32** |  | [optional] 

## Methods

### NewSearchGetAnalytics200Response

`func NewSearchGetAnalytics200Response() *SearchGetAnalytics200Response`

NewSearchGetAnalytics200Response instantiates a new SearchGetAnalytics200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchGetAnalytics200ResponseWithDefaults

`func NewSearchGetAnalytics200ResponseWithDefaults() *SearchGetAnalytics200Response`

NewSearchGetAnalytics200ResponseWithDefaults instantiates a new SearchGetAnalytics200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalSearches

`func (o *SearchGetAnalytics200Response) GetTotalSearches() int32`

GetTotalSearches returns the TotalSearches field if non-nil, zero value otherwise.

### GetTotalSearchesOk

`func (o *SearchGetAnalytics200Response) GetTotalSearchesOk() (*int32, bool)`

GetTotalSearchesOk returns a tuple with the TotalSearches field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalSearches

`func (o *SearchGetAnalytics200Response) SetTotalSearches(v int32)`

SetTotalSearches sets TotalSearches field to given value.

### HasTotalSearches

`func (o *SearchGetAnalytics200Response) HasTotalSearches() bool`

HasTotalSearches returns a boolean if a field has been set.

### GetTopQueries

`func (o *SearchGetAnalytics200Response) GetTopQueries() []SearchGetAnalytics200ResponseTopQueriesInner`

GetTopQueries returns the TopQueries field if non-nil, zero value otherwise.

### GetTopQueriesOk

`func (o *SearchGetAnalytics200Response) GetTopQueriesOk() (*[]SearchGetAnalytics200ResponseTopQueriesInner, bool)`

GetTopQueriesOk returns a tuple with the TopQueries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopQueries

`func (o *SearchGetAnalytics200Response) SetTopQueries(v []SearchGetAnalytics200ResponseTopQueriesInner)`

SetTopQueries sets TopQueries field to given value.

### HasTopQueries

`func (o *SearchGetAnalytics200Response) HasTopQueries() bool`

HasTopQueries returns a boolean if a field has been set.

### GetSearchesByCollection

`func (o *SearchGetAnalytics200Response) GetSearchesByCollection() map[string]interface{}`

GetSearchesByCollection returns the SearchesByCollection field if non-nil, zero value otherwise.

### GetSearchesByCollectionOk

`func (o *SearchGetAnalytics200Response) GetSearchesByCollectionOk() (*map[string]interface{}, bool)`

GetSearchesByCollectionOk returns a tuple with the SearchesByCollection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchesByCollection

`func (o *SearchGetAnalytics200Response) SetSearchesByCollection(v map[string]interface{})`

SetSearchesByCollection sets SearchesByCollection field to given value.

### HasSearchesByCollection

`func (o *SearchGetAnalytics200Response) HasSearchesByCollection() bool`

HasSearchesByCollection returns a boolean if a field has been set.

### GetAverageResponseTime

`func (o *SearchGetAnalytics200Response) GetAverageResponseTime() float32`

GetAverageResponseTime returns the AverageResponseTime field if non-nil, zero value otherwise.

### GetAverageResponseTimeOk

`func (o *SearchGetAnalytics200Response) GetAverageResponseTimeOk() (*float32, bool)`

GetAverageResponseTimeOk returns a tuple with the AverageResponseTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverageResponseTime

`func (o *SearchGetAnalytics200Response) SetAverageResponseTime(v float32)`

SetAverageResponseTime sets AverageResponseTime field to given value.

### HasAverageResponseTime

`func (o *SearchGetAnalytics200Response) HasAverageResponseTime() bool`

HasAverageResponseTime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



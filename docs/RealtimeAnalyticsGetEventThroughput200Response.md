# RealtimeAnalyticsGetEventThroughput200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**WindowMs** | Pointer to **int32** |  | [optional] 
**TotalEvents** | Pointer to **int32** |  | [optional] 
**EventsPerSecond** | Pointer to **float32** |  | [optional] 
**ByType** | Pointer to **map[string]int32** |  | [optional] 
**Timestamp** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewRealtimeAnalyticsGetEventThroughput200Response

`func NewRealtimeAnalyticsGetEventThroughput200Response() *RealtimeAnalyticsGetEventThroughput200Response`

NewRealtimeAnalyticsGetEventThroughput200Response instantiates a new RealtimeAnalyticsGetEventThroughput200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRealtimeAnalyticsGetEventThroughput200ResponseWithDefaults

`func NewRealtimeAnalyticsGetEventThroughput200ResponseWithDefaults() *RealtimeAnalyticsGetEventThroughput200Response`

NewRealtimeAnalyticsGetEventThroughput200ResponseWithDefaults instantiates a new RealtimeAnalyticsGetEventThroughput200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetWindowMs

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetWindowMs() int32`

GetWindowMs returns the WindowMs field if non-nil, zero value otherwise.

### GetWindowMsOk

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetWindowMsOk() (*int32, bool)`

GetWindowMsOk returns a tuple with the WindowMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWindowMs

`func (o *RealtimeAnalyticsGetEventThroughput200Response) SetWindowMs(v int32)`

SetWindowMs sets WindowMs field to given value.

### HasWindowMs

`func (o *RealtimeAnalyticsGetEventThroughput200Response) HasWindowMs() bool`

HasWindowMs returns a boolean if a field has been set.

### GetTotalEvents

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetTotalEvents() int32`

GetTotalEvents returns the TotalEvents field if non-nil, zero value otherwise.

### GetTotalEventsOk

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetTotalEventsOk() (*int32, bool)`

GetTotalEventsOk returns a tuple with the TotalEvents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalEvents

`func (o *RealtimeAnalyticsGetEventThroughput200Response) SetTotalEvents(v int32)`

SetTotalEvents sets TotalEvents field to given value.

### HasTotalEvents

`func (o *RealtimeAnalyticsGetEventThroughput200Response) HasTotalEvents() bool`

HasTotalEvents returns a boolean if a field has been set.

### GetEventsPerSecond

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetEventsPerSecond() float32`

GetEventsPerSecond returns the EventsPerSecond field if non-nil, zero value otherwise.

### GetEventsPerSecondOk

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetEventsPerSecondOk() (*float32, bool)`

GetEventsPerSecondOk returns a tuple with the EventsPerSecond field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventsPerSecond

`func (o *RealtimeAnalyticsGetEventThroughput200Response) SetEventsPerSecond(v float32)`

SetEventsPerSecond sets EventsPerSecond field to given value.

### HasEventsPerSecond

`func (o *RealtimeAnalyticsGetEventThroughput200Response) HasEventsPerSecond() bool`

HasEventsPerSecond returns a boolean if a field has been set.

### GetByType

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetByType() map[string]int32`

GetByType returns the ByType field if non-nil, zero value otherwise.

### GetByTypeOk

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetByTypeOk() (*map[string]int32, bool)`

GetByTypeOk returns a tuple with the ByType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByType

`func (o *RealtimeAnalyticsGetEventThroughput200Response) SetByType(v map[string]int32)`

SetByType sets ByType field to given value.

### HasByType

`func (o *RealtimeAnalyticsGetEventThroughput200Response) HasByType() bool`

HasByType returns a boolean if a field has been set.

### GetTimestamp

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *RealtimeAnalyticsGetEventThroughput200Response) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *RealtimeAnalyticsGetEventThroughput200Response) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *RealtimeAnalyticsGetEventThroughput200Response) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



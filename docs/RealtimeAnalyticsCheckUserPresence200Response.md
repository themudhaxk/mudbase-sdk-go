# RealtimeAnalyticsCheckUserPresence200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Presence** | Pointer to [**map[string]RealtimeAnalyticsCheckUserPresence200ResponsePresenceValue**](RealtimeAnalyticsCheckUserPresence200ResponsePresenceValue.md) |  | [optional] 
**Timestamp** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewRealtimeAnalyticsCheckUserPresence200Response

`func NewRealtimeAnalyticsCheckUserPresence200Response() *RealtimeAnalyticsCheckUserPresence200Response`

NewRealtimeAnalyticsCheckUserPresence200Response instantiates a new RealtimeAnalyticsCheckUserPresence200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRealtimeAnalyticsCheckUserPresence200ResponseWithDefaults

`func NewRealtimeAnalyticsCheckUserPresence200ResponseWithDefaults() *RealtimeAnalyticsCheckUserPresence200Response`

NewRealtimeAnalyticsCheckUserPresence200ResponseWithDefaults instantiates a new RealtimeAnalyticsCheckUserPresence200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPresence

`func (o *RealtimeAnalyticsCheckUserPresence200Response) GetPresence() map[string]RealtimeAnalyticsCheckUserPresence200ResponsePresenceValue`

GetPresence returns the Presence field if non-nil, zero value otherwise.

### GetPresenceOk

`func (o *RealtimeAnalyticsCheckUserPresence200Response) GetPresenceOk() (*map[string]RealtimeAnalyticsCheckUserPresence200ResponsePresenceValue, bool)`

GetPresenceOk returns a tuple with the Presence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresence

`func (o *RealtimeAnalyticsCheckUserPresence200Response) SetPresence(v map[string]RealtimeAnalyticsCheckUserPresence200ResponsePresenceValue)`

SetPresence sets Presence field to given value.

### HasPresence

`func (o *RealtimeAnalyticsCheckUserPresence200Response) HasPresence() bool`

HasPresence returns a boolean if a field has been set.

### GetTimestamp

`func (o *RealtimeAnalyticsCheckUserPresence200Response) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *RealtimeAnalyticsCheckUserPresence200Response) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *RealtimeAnalyticsCheckUserPresence200Response) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *RealtimeAnalyticsCheckUserPresence200Response) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



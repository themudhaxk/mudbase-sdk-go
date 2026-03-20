# WebhookLog

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Url** | Pointer to **string** |  | [optional] 
**Method** | Pointer to **string** |  | [optional] 
**Event** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**StatusCode** | Pointer to **int32** |  | [optional] 
**Payload** | Pointer to **map[string]interface{}** |  | [optional] 
**Response** | Pointer to **map[string]interface{}** |  | [optional] 
**Duration** | Pointer to **int32** |  | [optional] 
**Attempts** | Pointer to **int32** |  | [optional] 
**Error** | Pointer to **string** |  | [optional] 
**NextRetry** | Pointer to **time.Time** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewWebhookLog

`func NewWebhookLog() *WebhookLog`

NewWebhookLog instantiates a new WebhookLog object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookLogWithDefaults

`func NewWebhookLogWithDefaults() *WebhookLog`

NewWebhookLogWithDefaults instantiates a new WebhookLog object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WebhookLog) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WebhookLog) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WebhookLog) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *WebhookLog) HasId() bool`

HasId returns a boolean if a field has been set.

### GetUrl

`func (o *WebhookLog) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WebhookLog) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WebhookLog) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *WebhookLog) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetMethod

`func (o *WebhookLog) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *WebhookLog) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *WebhookLog) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *WebhookLog) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### GetEvent

`func (o *WebhookLog) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WebhookLog) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WebhookLog) SetEvent(v string)`

SetEvent sets Event field to given value.

### HasEvent

`func (o *WebhookLog) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetStatus

`func (o *WebhookLog) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *WebhookLog) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *WebhookLog) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *WebhookLog) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetStatusCode

`func (o *WebhookLog) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *WebhookLog) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *WebhookLog) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *WebhookLog) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetPayload

`func (o *WebhookLog) GetPayload() map[string]interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *WebhookLog) GetPayloadOk() (*map[string]interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *WebhookLog) SetPayload(v map[string]interface{})`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *WebhookLog) HasPayload() bool`

HasPayload returns a boolean if a field has been set.

### GetResponse

`func (o *WebhookLog) GetResponse() map[string]interface{}`

GetResponse returns the Response field if non-nil, zero value otherwise.

### GetResponseOk

`func (o *WebhookLog) GetResponseOk() (*map[string]interface{}, bool)`

GetResponseOk returns a tuple with the Response field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponse

`func (o *WebhookLog) SetResponse(v map[string]interface{})`

SetResponse sets Response field to given value.

### HasResponse

`func (o *WebhookLog) HasResponse() bool`

HasResponse returns a boolean if a field has been set.

### GetDuration

`func (o *WebhookLog) GetDuration() int32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *WebhookLog) GetDurationOk() (*int32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *WebhookLog) SetDuration(v int32)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *WebhookLog) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### GetAttempts

`func (o *WebhookLog) GetAttempts() int32`

GetAttempts returns the Attempts field if non-nil, zero value otherwise.

### GetAttemptsOk

`func (o *WebhookLog) GetAttemptsOk() (*int32, bool)`

GetAttemptsOk returns a tuple with the Attempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttempts

`func (o *WebhookLog) SetAttempts(v int32)`

SetAttempts sets Attempts field to given value.

### HasAttempts

`func (o *WebhookLog) HasAttempts() bool`

HasAttempts returns a boolean if a field has been set.

### GetError

`func (o *WebhookLog) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *WebhookLog) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *WebhookLog) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *WebhookLog) HasError() bool`

HasError returns a boolean if a field has been set.

### GetNextRetry

`func (o *WebhookLog) GetNextRetry() time.Time`

GetNextRetry returns the NextRetry field if non-nil, zero value otherwise.

### GetNextRetryOk

`func (o *WebhookLog) GetNextRetryOk() (*time.Time, bool)`

GetNextRetryOk returns a tuple with the NextRetry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextRetry

`func (o *WebhookLog) SetNextRetry(v time.Time)`

SetNextRetry sets NextRetry field to given value.

### HasNextRetry

`func (o *WebhookLog) HasNextRetry() bool`

HasNextRetry returns a boolean if a field has been set.

### GetCreatedAt

`func (o *WebhookLog) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WebhookLog) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WebhookLog) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *WebhookLog) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



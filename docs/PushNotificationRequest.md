# PushNotificationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tokens** | Pointer to **[]string** | Registered device push tokens to deliver to (device-token channel). | [optional] 
**Endpoints** | Pointer to **[]string** | Registered Web Push subscription endpoints to deliver to (native Web Push channel).  | [optional] 
**UserIds** | Pointer to **[]string** | Deliver to every Web Push subscription registered under these user ids (native Web Push channel).  | [optional] 
**WebPushBroadcast** | Pointer to **bool** | When true, deliver to every enabled Web Push subscription registered to the project (native Web Push channel). Ignored when the project has not enabled native Web Push.  | [optional] 
**Title** | **string** |  | 
**Body** | **string** |  | 
**Data** | Pointer to **map[string]interface{}** |  | [optional] 
**ImageUrl** | Pointer to **string** |  | [optional] 

## Methods

### NewPushNotificationRequest

`func NewPushNotificationRequest(title string, body string, ) *PushNotificationRequest`

NewPushNotificationRequest instantiates a new PushNotificationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPushNotificationRequestWithDefaults

`func NewPushNotificationRequestWithDefaults() *PushNotificationRequest`

NewPushNotificationRequestWithDefaults instantiates a new PushNotificationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTokens

`func (o *PushNotificationRequest) GetTokens() []string`

GetTokens returns the Tokens field if non-nil, zero value otherwise.

### GetTokensOk

`func (o *PushNotificationRequest) GetTokensOk() (*[]string, bool)`

GetTokensOk returns a tuple with the Tokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokens

`func (o *PushNotificationRequest) SetTokens(v []string)`

SetTokens sets Tokens field to given value.

### HasTokens

`func (o *PushNotificationRequest) HasTokens() bool`

HasTokens returns a boolean if a field has been set.

### GetEndpoints

`func (o *PushNotificationRequest) GetEndpoints() []string`

GetEndpoints returns the Endpoints field if non-nil, zero value otherwise.

### GetEndpointsOk

`func (o *PushNotificationRequest) GetEndpointsOk() (*[]string, bool)`

GetEndpointsOk returns a tuple with the Endpoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoints

`func (o *PushNotificationRequest) SetEndpoints(v []string)`

SetEndpoints sets Endpoints field to given value.

### HasEndpoints

`func (o *PushNotificationRequest) HasEndpoints() bool`

HasEndpoints returns a boolean if a field has been set.

### GetUserIds

`func (o *PushNotificationRequest) GetUserIds() []string`

GetUserIds returns the UserIds field if non-nil, zero value otherwise.

### GetUserIdsOk

`func (o *PushNotificationRequest) GetUserIdsOk() (*[]string, bool)`

GetUserIdsOk returns a tuple with the UserIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserIds

`func (o *PushNotificationRequest) SetUserIds(v []string)`

SetUserIds sets UserIds field to given value.

### HasUserIds

`func (o *PushNotificationRequest) HasUserIds() bool`

HasUserIds returns a boolean if a field has been set.

### GetWebPushBroadcast

`func (o *PushNotificationRequest) GetWebPushBroadcast() bool`

GetWebPushBroadcast returns the WebPushBroadcast field if non-nil, zero value otherwise.

### GetWebPushBroadcastOk

`func (o *PushNotificationRequest) GetWebPushBroadcastOk() (*bool, bool)`

GetWebPushBroadcastOk returns a tuple with the WebPushBroadcast field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebPushBroadcast

`func (o *PushNotificationRequest) SetWebPushBroadcast(v bool)`

SetWebPushBroadcast sets WebPushBroadcast field to given value.

### HasWebPushBroadcast

`func (o *PushNotificationRequest) HasWebPushBroadcast() bool`

HasWebPushBroadcast returns a boolean if a field has been set.

### GetTitle

`func (o *PushNotificationRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *PushNotificationRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *PushNotificationRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetBody

`func (o *PushNotificationRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *PushNotificationRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *PushNotificationRequest) SetBody(v string)`

SetBody sets Body field to given value.


### GetData

`func (o *PushNotificationRequest) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PushNotificationRequest) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PushNotificationRequest) SetData(v map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *PushNotificationRequest) HasData() bool`

HasData returns a boolean if a field has been set.

### GetImageUrl

`func (o *PushNotificationRequest) GetImageUrl() string`

GetImageUrl returns the ImageUrl field if non-nil, zero value otherwise.

### GetImageUrlOk

`func (o *PushNotificationRequest) GetImageUrlOk() (*string, bool)`

GetImageUrlOk returns a tuple with the ImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl

`func (o *PushNotificationRequest) SetImageUrl(v string)`

SetImageUrl sets ImageUrl field to given value.

### HasImageUrl

`func (o *PushNotificationRequest) HasImageUrl() bool`

HasImageUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



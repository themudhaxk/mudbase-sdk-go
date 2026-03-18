# WalletCreateWebhookRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** |  | 
**Events** | **[]string** |  | 
**Secret** | Pointer to **string** | Optional webhook secret for HMAC signing | [optional] 
**Filters** | Pointer to [**WalletCreateWebhookRequestFilters**](WalletCreateWebhookRequestFilters.md) |  | [optional] 
**ProjectId** | Pointer to **string** | Optional project ID | [optional] 

## Methods

### NewWalletCreateWebhookRequest

`func NewWalletCreateWebhookRequest(url string, events []string, ) *WalletCreateWebhookRequest`

NewWalletCreateWebhookRequest instantiates a new WalletCreateWebhookRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletCreateWebhookRequestWithDefaults

`func NewWalletCreateWebhookRequestWithDefaults() *WalletCreateWebhookRequest`

NewWalletCreateWebhookRequestWithDefaults instantiates a new WalletCreateWebhookRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *WalletCreateWebhookRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WalletCreateWebhookRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WalletCreateWebhookRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetEvents

`func (o *WalletCreateWebhookRequest) GetEvents() []string`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *WalletCreateWebhookRequest) GetEventsOk() (*[]string, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *WalletCreateWebhookRequest) SetEvents(v []string)`

SetEvents sets Events field to given value.


### GetSecret

`func (o *WalletCreateWebhookRequest) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *WalletCreateWebhookRequest) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *WalletCreateWebhookRequest) SetSecret(v string)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *WalletCreateWebhookRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetFilters

`func (o *WalletCreateWebhookRequest) GetFilters() WalletCreateWebhookRequestFilters`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *WalletCreateWebhookRequest) GetFiltersOk() (*WalletCreateWebhookRequestFilters, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *WalletCreateWebhookRequest) SetFilters(v WalletCreateWebhookRequestFilters)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *WalletCreateWebhookRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### GetProjectId

`func (o *WalletCreateWebhookRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *WalletCreateWebhookRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *WalletCreateWebhookRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *WalletCreateWebhookRequest) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WalletTransactionWebhookPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | Pointer to **string** |  | [optional] 
**Data** | Pointer to **map[string]interface{}** | Payload data (addressId, address, chain, txHash, transaction, etc.) | [optional] 
**Timestamp** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewWalletTransactionWebhookPayload

`func NewWalletTransactionWebhookPayload() *WalletTransactionWebhookPayload`

NewWalletTransactionWebhookPayload instantiates a new WalletTransactionWebhookPayload object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletTransactionWebhookPayloadWithDefaults

`func NewWalletTransactionWebhookPayloadWithDefaults() *WalletTransactionWebhookPayload`

NewWalletTransactionWebhookPayloadWithDefaults instantiates a new WalletTransactionWebhookPayload object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *WalletTransactionWebhookPayload) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WalletTransactionWebhookPayload) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WalletTransactionWebhookPayload) SetEvent(v string)`

SetEvent sets Event field to given value.

### HasEvent

`func (o *WalletTransactionWebhookPayload) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetData

`func (o *WalletTransactionWebhookPayload) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletTransactionWebhookPayload) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletTransactionWebhookPayload) SetData(v map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *WalletTransactionWebhookPayload) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTimestamp

`func (o *WalletTransactionWebhookPayload) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *WalletTransactionWebhookPayload) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *WalletTransactionWebhookPayload) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *WalletTransactionWebhookPayload) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



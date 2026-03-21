# BillingHandleCryptoWebhookRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | **string** |  | 
**Data** | [**BillingHandleCryptoWebhookRequestData**](BillingHandleCryptoWebhookRequestData.md) |  | 

## Methods

### NewBillingHandleCryptoWebhookRequest

`func NewBillingHandleCryptoWebhookRequest(event string, data BillingHandleCryptoWebhookRequestData, ) *BillingHandleCryptoWebhookRequest`

NewBillingHandleCryptoWebhookRequest instantiates a new BillingHandleCryptoWebhookRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingHandleCryptoWebhookRequestWithDefaults

`func NewBillingHandleCryptoWebhookRequestWithDefaults() *BillingHandleCryptoWebhookRequest`

NewBillingHandleCryptoWebhookRequestWithDefaults instantiates a new BillingHandleCryptoWebhookRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *BillingHandleCryptoWebhookRequest) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *BillingHandleCryptoWebhookRequest) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *BillingHandleCryptoWebhookRequest) SetEvent(v string)`

SetEvent sets Event field to given value.


### GetData

`func (o *BillingHandleCryptoWebhookRequest) GetData() BillingHandleCryptoWebhookRequestData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BillingHandleCryptoWebhookRequest) GetDataOk() (*BillingHandleCryptoWebhookRequestData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BillingHandleCryptoWebhookRequest) SetData(v BillingHandleCryptoWebhookRequestData)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



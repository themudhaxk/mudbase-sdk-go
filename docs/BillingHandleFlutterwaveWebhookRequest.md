# BillingHandleFlutterwaveWebhookRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | Pointer to **string** | Event type (e.g. charge.completed, payment.successful) | [optional] 
**Data** | Pointer to [**BillingHandleFlutterwaveWebhookRequestData**](BillingHandleFlutterwaveWebhookRequestData.md) |  | [optional] 

## Methods

### NewBillingHandleFlutterwaveWebhookRequest

`func NewBillingHandleFlutterwaveWebhookRequest() *BillingHandleFlutterwaveWebhookRequest`

NewBillingHandleFlutterwaveWebhookRequest instantiates a new BillingHandleFlutterwaveWebhookRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingHandleFlutterwaveWebhookRequestWithDefaults

`func NewBillingHandleFlutterwaveWebhookRequestWithDefaults() *BillingHandleFlutterwaveWebhookRequest`

NewBillingHandleFlutterwaveWebhookRequestWithDefaults instantiates a new BillingHandleFlutterwaveWebhookRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *BillingHandleFlutterwaveWebhookRequest) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *BillingHandleFlutterwaveWebhookRequest) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *BillingHandleFlutterwaveWebhookRequest) SetEvent(v string)`

SetEvent sets Event field to given value.

### HasEvent

`func (o *BillingHandleFlutterwaveWebhookRequest) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetData

`func (o *BillingHandleFlutterwaveWebhookRequest) GetData() BillingHandleFlutterwaveWebhookRequestData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BillingHandleFlutterwaveWebhookRequest) GetDataOk() (*BillingHandleFlutterwaveWebhookRequestData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BillingHandleFlutterwaveWebhookRequest) SetData(v BillingHandleFlutterwaveWebhookRequestData)`

SetData sets Data field to given value.

### HasData

`func (o *BillingHandleFlutterwaveWebhookRequest) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



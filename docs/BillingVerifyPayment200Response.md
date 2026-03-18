# BillingVerifyPayment200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | Pointer to **bool** |  | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Data** | Pointer to [**BillingVerifyPayment200ResponseData**](BillingVerifyPayment200ResponseData.md) |  | [optional] 

## Methods

### NewBillingVerifyPayment200Response

`func NewBillingVerifyPayment200Response() *BillingVerifyPayment200Response`

NewBillingVerifyPayment200Response instantiates a new BillingVerifyPayment200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingVerifyPayment200ResponseWithDefaults

`func NewBillingVerifyPayment200ResponseWithDefaults() *BillingVerifyPayment200Response`

NewBillingVerifyPayment200ResponseWithDefaults instantiates a new BillingVerifyPayment200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *BillingVerifyPayment200Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *BillingVerifyPayment200Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *BillingVerifyPayment200Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *BillingVerifyPayment200Response) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetMessage

`func (o *BillingVerifyPayment200Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *BillingVerifyPayment200Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *BillingVerifyPayment200Response) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *BillingVerifyPayment200Response) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetData

`func (o *BillingVerifyPayment200Response) GetData() BillingVerifyPayment200ResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BillingVerifyPayment200Response) GetDataOk() (*BillingVerifyPayment200ResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BillingVerifyPayment200Response) SetData(v BillingVerifyPayment200ResponseData)`

SetData sets Data field to given value.

### HasData

`func (o *BillingVerifyPayment200Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



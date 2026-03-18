# PaymentRefund

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**PaymentIntent** | Pointer to **string** | Payment intent ID | [optional] 
**Merchant** | Pointer to **string** | Merchant ID | [optional] 
**Amount** | Pointer to **float32** | Refund amount | [optional] 
**Reason** | Pointer to **string** | Refund reason | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**IsCrossChain** | Pointer to **bool** | True if cross-chain refund | [optional] [default to false]
**SourceNetwork** | Pointer to **string** | Source network for refund | [optional] 
**TargetNetwork** | Pointer to **string** | Target network for cross-chain refund | [optional] 
**ApprovedBy** | Pointer to **string** | User ID who approved | [optional] 
**ApprovedAt** | Pointer to **time.Time** |  | [optional] 
**RefundTx** | Pointer to **string** | Refund transaction hash | [optional] 
**RefundedAt** | Pointer to **time.Time** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewPaymentRefund

`func NewPaymentRefund() *PaymentRefund`

NewPaymentRefund instantiates a new PaymentRefund object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentRefundWithDefaults

`func NewPaymentRefundWithDefaults() *PaymentRefund`

NewPaymentRefundWithDefaults instantiates a new PaymentRefund object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PaymentRefund) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PaymentRefund) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PaymentRefund) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *PaymentRefund) HasId() bool`

HasId returns a boolean if a field has been set.

### GetPaymentIntent

`func (o *PaymentRefund) GetPaymentIntent() string`

GetPaymentIntent returns the PaymentIntent field if non-nil, zero value otherwise.

### GetPaymentIntentOk

`func (o *PaymentRefund) GetPaymentIntentOk() (*string, bool)`

GetPaymentIntentOk returns a tuple with the PaymentIntent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentIntent

`func (o *PaymentRefund) SetPaymentIntent(v string)`

SetPaymentIntent sets PaymentIntent field to given value.

### HasPaymentIntent

`func (o *PaymentRefund) HasPaymentIntent() bool`

HasPaymentIntent returns a boolean if a field has been set.

### GetMerchant

`func (o *PaymentRefund) GetMerchant() string`

GetMerchant returns the Merchant field if non-nil, zero value otherwise.

### GetMerchantOk

`func (o *PaymentRefund) GetMerchantOk() (*string, bool)`

GetMerchantOk returns a tuple with the Merchant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMerchant

`func (o *PaymentRefund) SetMerchant(v string)`

SetMerchant sets Merchant field to given value.

### HasMerchant

`func (o *PaymentRefund) HasMerchant() bool`

HasMerchant returns a boolean if a field has been set.

### GetAmount

`func (o *PaymentRefund) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentRefund) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentRefund) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *PaymentRefund) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetReason

`func (o *PaymentRefund) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *PaymentRefund) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *PaymentRefund) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *PaymentRefund) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetStatus

`func (o *PaymentRefund) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PaymentRefund) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PaymentRefund) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PaymentRefund) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetIsCrossChain

`func (o *PaymentRefund) GetIsCrossChain() bool`

GetIsCrossChain returns the IsCrossChain field if non-nil, zero value otherwise.

### GetIsCrossChainOk

`func (o *PaymentRefund) GetIsCrossChainOk() (*bool, bool)`

GetIsCrossChainOk returns a tuple with the IsCrossChain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCrossChain

`func (o *PaymentRefund) SetIsCrossChain(v bool)`

SetIsCrossChain sets IsCrossChain field to given value.

### HasIsCrossChain

`func (o *PaymentRefund) HasIsCrossChain() bool`

HasIsCrossChain returns a boolean if a field has been set.

### GetSourceNetwork

`func (o *PaymentRefund) GetSourceNetwork() string`

GetSourceNetwork returns the SourceNetwork field if non-nil, zero value otherwise.

### GetSourceNetworkOk

`func (o *PaymentRefund) GetSourceNetworkOk() (*string, bool)`

GetSourceNetworkOk returns a tuple with the SourceNetwork field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceNetwork

`func (o *PaymentRefund) SetSourceNetwork(v string)`

SetSourceNetwork sets SourceNetwork field to given value.

### HasSourceNetwork

`func (o *PaymentRefund) HasSourceNetwork() bool`

HasSourceNetwork returns a boolean if a field has been set.

### GetTargetNetwork

`func (o *PaymentRefund) GetTargetNetwork() string`

GetTargetNetwork returns the TargetNetwork field if non-nil, zero value otherwise.

### GetTargetNetworkOk

`func (o *PaymentRefund) GetTargetNetworkOk() (*string, bool)`

GetTargetNetworkOk returns a tuple with the TargetNetwork field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetNetwork

`func (o *PaymentRefund) SetTargetNetwork(v string)`

SetTargetNetwork sets TargetNetwork field to given value.

### HasTargetNetwork

`func (o *PaymentRefund) HasTargetNetwork() bool`

HasTargetNetwork returns a boolean if a field has been set.

### GetApprovedBy

`func (o *PaymentRefund) GetApprovedBy() string`

GetApprovedBy returns the ApprovedBy field if non-nil, zero value otherwise.

### GetApprovedByOk

`func (o *PaymentRefund) GetApprovedByOk() (*string, bool)`

GetApprovedByOk returns a tuple with the ApprovedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApprovedBy

`func (o *PaymentRefund) SetApprovedBy(v string)`

SetApprovedBy sets ApprovedBy field to given value.

### HasApprovedBy

`func (o *PaymentRefund) HasApprovedBy() bool`

HasApprovedBy returns a boolean if a field has been set.

### GetApprovedAt

`func (o *PaymentRefund) GetApprovedAt() time.Time`

GetApprovedAt returns the ApprovedAt field if non-nil, zero value otherwise.

### GetApprovedAtOk

`func (o *PaymentRefund) GetApprovedAtOk() (*time.Time, bool)`

GetApprovedAtOk returns a tuple with the ApprovedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApprovedAt

`func (o *PaymentRefund) SetApprovedAt(v time.Time)`

SetApprovedAt sets ApprovedAt field to given value.

### HasApprovedAt

`func (o *PaymentRefund) HasApprovedAt() bool`

HasApprovedAt returns a boolean if a field has been set.

### GetRefundTx

`func (o *PaymentRefund) GetRefundTx() string`

GetRefundTx returns the RefundTx field if non-nil, zero value otherwise.

### GetRefundTxOk

`func (o *PaymentRefund) GetRefundTxOk() (*string, bool)`

GetRefundTxOk returns a tuple with the RefundTx field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefundTx

`func (o *PaymentRefund) SetRefundTx(v string)`

SetRefundTx sets RefundTx field to given value.

### HasRefundTx

`func (o *PaymentRefund) HasRefundTx() bool`

HasRefundTx returns a boolean if a field has been set.

### GetRefundedAt

`func (o *PaymentRefund) GetRefundedAt() time.Time`

GetRefundedAt returns the RefundedAt field if non-nil, zero value otherwise.

### GetRefundedAtOk

`func (o *PaymentRefund) GetRefundedAtOk() (*time.Time, bool)`

GetRefundedAtOk returns a tuple with the RefundedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefundedAt

`func (o *PaymentRefund) SetRefundedAt(v time.Time)`

SetRefundedAt sets RefundedAt field to given value.

### HasRefundedAt

`func (o *PaymentRefund) HasRefundedAt() bool`

HasRefundedAt returns a boolean if a field has been set.

### GetCreatedAt

`func (o *PaymentRefund) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PaymentRefund) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PaymentRefund) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *PaymentRefund) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *PaymentRefund) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *PaymentRefund) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *PaymentRefund) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *PaymentRefund) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



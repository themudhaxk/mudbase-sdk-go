# PaymentIntent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**PaymentId** | Pointer to **string** | Unique payment identifier | [optional] 
**Merchant** | Pointer to **string** | Merchant ID | [optional] 
**Project** | Pointer to **string** | Project ID | [optional] 
**Amount** | Pointer to **float32** | Payment amount | [optional] 
**Currency** | Pointer to **string** |  | [optional] [default to "USD"]
**Network** | Pointer to **string** |  | [optional] 
**Token** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**FinalityStatus** | Pointer to **string** |  | [optional] 
**TotalDue** | Pointer to **float32** | Total amount due including fees | [optional] 
**Commission** | Pointer to **float32** | Platform commission | [optional] 
**MerchantReceives** | Pointer to **float32** | Amount merchant receives after commission | [optional] 
**ExpiresAt** | Pointer to **time.Time** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** | Additional metadata | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewPaymentIntent

`func NewPaymentIntent() *PaymentIntent`

NewPaymentIntent instantiates a new PaymentIntent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentIntentWithDefaults

`func NewPaymentIntentWithDefaults() *PaymentIntent`

NewPaymentIntentWithDefaults instantiates a new PaymentIntent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PaymentIntent) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PaymentIntent) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PaymentIntent) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *PaymentIntent) HasId() bool`

HasId returns a boolean if a field has been set.

### GetPaymentId

`func (o *PaymentIntent) GetPaymentId() string`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *PaymentIntent) GetPaymentIdOk() (*string, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *PaymentIntent) SetPaymentId(v string)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *PaymentIntent) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetMerchant

`func (o *PaymentIntent) GetMerchant() string`

GetMerchant returns the Merchant field if non-nil, zero value otherwise.

### GetMerchantOk

`func (o *PaymentIntent) GetMerchantOk() (*string, bool)`

GetMerchantOk returns a tuple with the Merchant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMerchant

`func (o *PaymentIntent) SetMerchant(v string)`

SetMerchant sets Merchant field to given value.

### HasMerchant

`func (o *PaymentIntent) HasMerchant() bool`

HasMerchant returns a boolean if a field has been set.

### GetProject

`func (o *PaymentIntent) GetProject() string`

GetProject returns the Project field if non-nil, zero value otherwise.

### GetProjectOk

`func (o *PaymentIntent) GetProjectOk() (*string, bool)`

GetProjectOk returns a tuple with the Project field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProject

`func (o *PaymentIntent) SetProject(v string)`

SetProject sets Project field to given value.

### HasProject

`func (o *PaymentIntent) HasProject() bool`

HasProject returns a boolean if a field has been set.

### GetAmount

`func (o *PaymentIntent) GetAmount() float32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentIntent) GetAmountOk() (*float32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentIntent) SetAmount(v float32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *PaymentIntent) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *PaymentIntent) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *PaymentIntent) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *PaymentIntent) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *PaymentIntent) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetNetwork

`func (o *PaymentIntent) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *PaymentIntent) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *PaymentIntent) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *PaymentIntent) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetToken

`func (o *PaymentIntent) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *PaymentIntent) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *PaymentIntent) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *PaymentIntent) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetType

`func (o *PaymentIntent) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *PaymentIntent) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *PaymentIntent) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *PaymentIntent) HasType() bool`

HasType returns a boolean if a field has been set.

### GetStatus

`func (o *PaymentIntent) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PaymentIntent) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PaymentIntent) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PaymentIntent) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetFinalityStatus

`func (o *PaymentIntent) GetFinalityStatus() string`

GetFinalityStatus returns the FinalityStatus field if non-nil, zero value otherwise.

### GetFinalityStatusOk

`func (o *PaymentIntent) GetFinalityStatusOk() (*string, bool)`

GetFinalityStatusOk returns a tuple with the FinalityStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalityStatus

`func (o *PaymentIntent) SetFinalityStatus(v string)`

SetFinalityStatus sets FinalityStatus field to given value.

### HasFinalityStatus

`func (o *PaymentIntent) HasFinalityStatus() bool`

HasFinalityStatus returns a boolean if a field has been set.

### GetTotalDue

`func (o *PaymentIntent) GetTotalDue() float32`

GetTotalDue returns the TotalDue field if non-nil, zero value otherwise.

### GetTotalDueOk

`func (o *PaymentIntent) GetTotalDueOk() (*float32, bool)`

GetTotalDueOk returns a tuple with the TotalDue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalDue

`func (o *PaymentIntent) SetTotalDue(v float32)`

SetTotalDue sets TotalDue field to given value.

### HasTotalDue

`func (o *PaymentIntent) HasTotalDue() bool`

HasTotalDue returns a boolean if a field has been set.

### GetCommission

`func (o *PaymentIntent) GetCommission() float32`

GetCommission returns the Commission field if non-nil, zero value otherwise.

### GetCommissionOk

`func (o *PaymentIntent) GetCommissionOk() (*float32, bool)`

GetCommissionOk returns a tuple with the Commission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommission

`func (o *PaymentIntent) SetCommission(v float32)`

SetCommission sets Commission field to given value.

### HasCommission

`func (o *PaymentIntent) HasCommission() bool`

HasCommission returns a boolean if a field has been set.

### GetMerchantReceives

`func (o *PaymentIntent) GetMerchantReceives() float32`

GetMerchantReceives returns the MerchantReceives field if non-nil, zero value otherwise.

### GetMerchantReceivesOk

`func (o *PaymentIntent) GetMerchantReceivesOk() (*float32, bool)`

GetMerchantReceivesOk returns a tuple with the MerchantReceives field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMerchantReceives

`func (o *PaymentIntent) SetMerchantReceives(v float32)`

SetMerchantReceives sets MerchantReceives field to given value.

### HasMerchantReceives

`func (o *PaymentIntent) HasMerchantReceives() bool`

HasMerchantReceives returns a boolean if a field has been set.

### GetExpiresAt

`func (o *PaymentIntent) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *PaymentIntent) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *PaymentIntent) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *PaymentIntent) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetMetadata

`func (o *PaymentIntent) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *PaymentIntent) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *PaymentIntent) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *PaymentIntent) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetCreatedAt

`func (o *PaymentIntent) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PaymentIntent) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PaymentIntent) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *PaymentIntent) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *PaymentIntent) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *PaymentIntent) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *PaymentIntent) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *PaymentIntent) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



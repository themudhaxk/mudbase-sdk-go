# WalletEstimateGasRequestTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | Sender address | 
**To** | Pointer to **string** | For native transfers: recipient address. For token transfers: recipient address (tokenAddress must be provided separately). For raw format: contract or recipient address.  | [optional] 
**Value** | Pointer to **string** | Amount in native currency (ETH/BNB/MATIC). Can be provided as decimal string (e.g., \&quot;1.0\&quot;) or wei string. Required for native transfers.  | [optional] 
**Data** | Pointer to **string** | Raw transaction data (hex string starting with 0x). Used for raw format or contract calls. For token transfers, this is auto-generated from tokenAddress, to, and amount.  | [optional] 
**TokenAddress** | Pointer to **string** | Token contract address (for token transfers). When provided with &#39;amount&#39;, automatically encodes the transfer.  | [optional] 
**Amount** | Pointer to **string** | Token amount in human-readable format (e.g., \&quot;1.0\&quot; for 1 token). Used with tokenAddress for user-friendly token transfers. Automatically converted to token units based on token decimals.  | [optional] 

## Methods

### NewWalletEstimateGasRequestTransaction

`func NewWalletEstimateGasRequestTransaction(from string, ) *WalletEstimateGasRequestTransaction`

NewWalletEstimateGasRequestTransaction instantiates a new WalletEstimateGasRequestTransaction object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletEstimateGasRequestTransactionWithDefaults

`func NewWalletEstimateGasRequestTransactionWithDefaults() *WalletEstimateGasRequestTransaction`

NewWalletEstimateGasRequestTransactionWithDefaults instantiates a new WalletEstimateGasRequestTransaction object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *WalletEstimateGasRequestTransaction) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *WalletEstimateGasRequestTransaction) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *WalletEstimateGasRequestTransaction) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *WalletEstimateGasRequestTransaction) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *WalletEstimateGasRequestTransaction) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *WalletEstimateGasRequestTransaction) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *WalletEstimateGasRequestTransaction) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetValue

`func (o *WalletEstimateGasRequestTransaction) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *WalletEstimateGasRequestTransaction) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *WalletEstimateGasRequestTransaction) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *WalletEstimateGasRequestTransaction) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetData

`func (o *WalletEstimateGasRequestTransaction) GetData() string`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WalletEstimateGasRequestTransaction) GetDataOk() (*string, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WalletEstimateGasRequestTransaction) SetData(v string)`

SetData sets Data field to given value.

### HasData

`func (o *WalletEstimateGasRequestTransaction) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTokenAddress

`func (o *WalletEstimateGasRequestTransaction) GetTokenAddress() string`

GetTokenAddress returns the TokenAddress field if non-nil, zero value otherwise.

### GetTokenAddressOk

`func (o *WalletEstimateGasRequestTransaction) GetTokenAddressOk() (*string, bool)`

GetTokenAddressOk returns a tuple with the TokenAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenAddress

`func (o *WalletEstimateGasRequestTransaction) SetTokenAddress(v string)`

SetTokenAddress sets TokenAddress field to given value.

### HasTokenAddress

`func (o *WalletEstimateGasRequestTransaction) HasTokenAddress() bool`

HasTokenAddress returns a boolean if a field has been set.

### GetAmount

`func (o *WalletEstimateGasRequestTransaction) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *WalletEstimateGasRequestTransaction) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *WalletEstimateGasRequestTransaction) SetAmount(v string)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *WalletEstimateGasRequestTransaction) HasAmount() bool`

HasAmount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WalletEstimateGas200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Chain** | Pointer to **string** | Chain id (e.g. bsc, ethereum, bitcoin) | [optional] 
**GasLimit** | Pointer to **string** | (EVM only) Estimated gas limit from RPC eth_estimateGas | [optional] 
**GasPrice** | Pointer to **string** | (EVM only) Gas price in wei | [optional] 
**GasPriceGwei** | Pointer to **float32** | (EVM only) Gas price in Gwei | [optional] 
**EstimatedCost** | Pointer to **string** | (EVM only) Total cost in wei (gasLimit * gasPrice) | [optional] 
**NetworkFee** | Pointer to **string** | Human-readable network fee from blockchain (e.g. \&quot;0.00063 ETH\&quot;, \&quot;0.00001 BTC\&quot;) | [optional] 
**EstimatedTime** | Pointer to **string** | Estimated confirmation time when available | [optional] 
**Currency** | Pointer to **string** | Native currency for the chain (ETH, BNB, MATIC, BTC, SOL, TRX, etc.) | [optional] 
**SatPerVb** | Pointer to **int32** | (UTXO only) Satoshis per virtual byte | [optional] 
**FeeSat** | Pointer to **int32** | (UTXO only) Estimated fee in satoshis | [optional] 
**Lamports** | Pointer to **int32** | (Solana only) Fee in lamports | [optional] 

## Methods

### NewWalletEstimateGas200ResponseData

`func NewWalletEstimateGas200ResponseData() *WalletEstimateGas200ResponseData`

NewWalletEstimateGas200ResponseData instantiates a new WalletEstimateGas200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWalletEstimateGas200ResponseDataWithDefaults

`func NewWalletEstimateGas200ResponseDataWithDefaults() *WalletEstimateGas200ResponseData`

NewWalletEstimateGas200ResponseDataWithDefaults instantiates a new WalletEstimateGas200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChain

`func (o *WalletEstimateGas200ResponseData) GetChain() string`

GetChain returns the Chain field if non-nil, zero value otherwise.

### GetChainOk

`func (o *WalletEstimateGas200ResponseData) GetChainOk() (*string, bool)`

GetChainOk returns a tuple with the Chain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChain

`func (o *WalletEstimateGas200ResponseData) SetChain(v string)`

SetChain sets Chain field to given value.

### HasChain

`func (o *WalletEstimateGas200ResponseData) HasChain() bool`

HasChain returns a boolean if a field has been set.

### GetGasLimit

`func (o *WalletEstimateGas200ResponseData) GetGasLimit() string`

GetGasLimit returns the GasLimit field if non-nil, zero value otherwise.

### GetGasLimitOk

`func (o *WalletEstimateGas200ResponseData) GetGasLimitOk() (*string, bool)`

GetGasLimitOk returns a tuple with the GasLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGasLimit

`func (o *WalletEstimateGas200ResponseData) SetGasLimit(v string)`

SetGasLimit sets GasLimit field to given value.

### HasGasLimit

`func (o *WalletEstimateGas200ResponseData) HasGasLimit() bool`

HasGasLimit returns a boolean if a field has been set.

### GetGasPrice

`func (o *WalletEstimateGas200ResponseData) GetGasPrice() string`

GetGasPrice returns the GasPrice field if non-nil, zero value otherwise.

### GetGasPriceOk

`func (o *WalletEstimateGas200ResponseData) GetGasPriceOk() (*string, bool)`

GetGasPriceOk returns a tuple with the GasPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGasPrice

`func (o *WalletEstimateGas200ResponseData) SetGasPrice(v string)`

SetGasPrice sets GasPrice field to given value.

### HasGasPrice

`func (o *WalletEstimateGas200ResponseData) HasGasPrice() bool`

HasGasPrice returns a boolean if a field has been set.

### GetGasPriceGwei

`func (o *WalletEstimateGas200ResponseData) GetGasPriceGwei() float32`

GetGasPriceGwei returns the GasPriceGwei field if non-nil, zero value otherwise.

### GetGasPriceGweiOk

`func (o *WalletEstimateGas200ResponseData) GetGasPriceGweiOk() (*float32, bool)`

GetGasPriceGweiOk returns a tuple with the GasPriceGwei field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGasPriceGwei

`func (o *WalletEstimateGas200ResponseData) SetGasPriceGwei(v float32)`

SetGasPriceGwei sets GasPriceGwei field to given value.

### HasGasPriceGwei

`func (o *WalletEstimateGas200ResponseData) HasGasPriceGwei() bool`

HasGasPriceGwei returns a boolean if a field has been set.

### GetEstimatedCost

`func (o *WalletEstimateGas200ResponseData) GetEstimatedCost() string`

GetEstimatedCost returns the EstimatedCost field if non-nil, zero value otherwise.

### GetEstimatedCostOk

`func (o *WalletEstimateGas200ResponseData) GetEstimatedCostOk() (*string, bool)`

GetEstimatedCostOk returns a tuple with the EstimatedCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimatedCost

`func (o *WalletEstimateGas200ResponseData) SetEstimatedCost(v string)`

SetEstimatedCost sets EstimatedCost field to given value.

### HasEstimatedCost

`func (o *WalletEstimateGas200ResponseData) HasEstimatedCost() bool`

HasEstimatedCost returns a boolean if a field has been set.

### GetNetworkFee

`func (o *WalletEstimateGas200ResponseData) GetNetworkFee() string`

GetNetworkFee returns the NetworkFee field if non-nil, zero value otherwise.

### GetNetworkFeeOk

`func (o *WalletEstimateGas200ResponseData) GetNetworkFeeOk() (*string, bool)`

GetNetworkFeeOk returns a tuple with the NetworkFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetworkFee

`func (o *WalletEstimateGas200ResponseData) SetNetworkFee(v string)`

SetNetworkFee sets NetworkFee field to given value.

### HasNetworkFee

`func (o *WalletEstimateGas200ResponseData) HasNetworkFee() bool`

HasNetworkFee returns a boolean if a field has been set.

### GetEstimatedTime

`func (o *WalletEstimateGas200ResponseData) GetEstimatedTime() string`

GetEstimatedTime returns the EstimatedTime field if non-nil, zero value otherwise.

### GetEstimatedTimeOk

`func (o *WalletEstimateGas200ResponseData) GetEstimatedTimeOk() (*string, bool)`

GetEstimatedTimeOk returns a tuple with the EstimatedTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimatedTime

`func (o *WalletEstimateGas200ResponseData) SetEstimatedTime(v string)`

SetEstimatedTime sets EstimatedTime field to given value.

### HasEstimatedTime

`func (o *WalletEstimateGas200ResponseData) HasEstimatedTime() bool`

HasEstimatedTime returns a boolean if a field has been set.

### GetCurrency

`func (o *WalletEstimateGas200ResponseData) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *WalletEstimateGas200ResponseData) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *WalletEstimateGas200ResponseData) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *WalletEstimateGas200ResponseData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetSatPerVb

`func (o *WalletEstimateGas200ResponseData) GetSatPerVb() int32`

GetSatPerVb returns the SatPerVb field if non-nil, zero value otherwise.

### GetSatPerVbOk

`func (o *WalletEstimateGas200ResponseData) GetSatPerVbOk() (*int32, bool)`

GetSatPerVbOk returns a tuple with the SatPerVb field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSatPerVb

`func (o *WalletEstimateGas200ResponseData) SetSatPerVb(v int32)`

SetSatPerVb sets SatPerVb field to given value.

### HasSatPerVb

`func (o *WalletEstimateGas200ResponseData) HasSatPerVb() bool`

HasSatPerVb returns a boolean if a field has been set.

### GetFeeSat

`func (o *WalletEstimateGas200ResponseData) GetFeeSat() int32`

GetFeeSat returns the FeeSat field if non-nil, zero value otherwise.

### GetFeeSatOk

`func (o *WalletEstimateGas200ResponseData) GetFeeSatOk() (*int32, bool)`

GetFeeSatOk returns a tuple with the FeeSat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeeSat

`func (o *WalletEstimateGas200ResponseData) SetFeeSat(v int32)`

SetFeeSat sets FeeSat field to given value.

### HasFeeSat

`func (o *WalletEstimateGas200ResponseData) HasFeeSat() bool`

HasFeeSat returns a boolean if a field has been set.

### GetLamports

`func (o *WalletEstimateGas200ResponseData) GetLamports() int32`

GetLamports returns the Lamports field if non-nil, zero value otherwise.

### GetLamportsOk

`func (o *WalletEstimateGas200ResponseData) GetLamportsOk() (*int32, bool)`

GetLamportsOk returns a tuple with the Lamports field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLamports

`func (o *WalletEstimateGas200ResponseData) SetLamports(v int32)`

SetLamports sets Lamports field to given value.

### HasLamports

`func (o *WalletEstimateGas200ResponseData) HasLamports() bool`

HasLamports returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



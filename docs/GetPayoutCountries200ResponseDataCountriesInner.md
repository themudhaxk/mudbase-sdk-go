# GetPayoutCountries200ResponseDataCountriesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | Pointer to **string** | ISO-3166 alpha-2 country code (e.g. NG, GH, KE, US, GB). | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**BanksListSupported** | Pointer to **bool** | Whether GET /payment-processing/banks returns a live bank list for this country. | [optional] 
**MobileMoney** | Pointer to **bool** |  | [optional] 
**International** | Pointer to **bool** | True for a market whose settlement rail requires an account-level capability beyond the standard local-rail onboarding (currently US, GB). | [optional] 
**Fields** | Pointer to [**[]GetPayoutCountries200ResponseDataCountriesInnerFieldsInner**](GetPayoutCountries200ResponseDataCountriesInnerFieldsInner.md) |  | [optional] 

## Methods

### NewGetPayoutCountries200ResponseDataCountriesInner

`func NewGetPayoutCountries200ResponseDataCountriesInner() *GetPayoutCountries200ResponseDataCountriesInner`

NewGetPayoutCountries200ResponseDataCountriesInner instantiates a new GetPayoutCountries200ResponseDataCountriesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetPayoutCountries200ResponseDataCountriesInnerWithDefaults

`func NewGetPayoutCountries200ResponseDataCountriesInnerWithDefaults() *GetPayoutCountries200ResponseDataCountriesInner`

NewGetPayoutCountries200ResponseDataCountriesInnerWithDefaults instantiates a new GetPayoutCountries200ResponseDataCountriesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetName

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCurrency

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetBanksListSupported

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetBanksListSupported() bool`

GetBanksListSupported returns the BanksListSupported field if non-nil, zero value otherwise.

### GetBanksListSupportedOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetBanksListSupportedOk() (*bool, bool)`

GetBanksListSupportedOk returns a tuple with the BanksListSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanksListSupported

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetBanksListSupported(v bool)`

SetBanksListSupported sets BanksListSupported field to given value.

### HasBanksListSupported

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasBanksListSupported() bool`

HasBanksListSupported returns a boolean if a field has been set.

### GetMobileMoney

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetMobileMoney() bool`

GetMobileMoney returns the MobileMoney field if non-nil, zero value otherwise.

### GetMobileMoneyOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetMobileMoneyOk() (*bool, bool)`

GetMobileMoneyOk returns a tuple with the MobileMoney field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMobileMoney

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetMobileMoney(v bool)`

SetMobileMoney sets MobileMoney field to given value.

### HasMobileMoney

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasMobileMoney() bool`

HasMobileMoney returns a boolean if a field has been set.

### GetInternational

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetInternational() bool`

GetInternational returns the International field if non-nil, zero value otherwise.

### GetInternationalOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetInternationalOk() (*bool, bool)`

GetInternationalOk returns a tuple with the International field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInternational

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetInternational(v bool)`

SetInternational sets International field to given value.

### HasInternational

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasInternational() bool`

HasInternational returns a boolean if a field has been set.

### GetFields

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetFields() []GetPayoutCountries200ResponseDataCountriesInnerFieldsInner`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *GetPayoutCountries200ResponseDataCountriesInner) GetFieldsOk() (*[]GetPayoutCountries200ResponseDataCountriesInnerFieldsInner, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *GetPayoutCountries200ResponseDataCountriesInner) SetFields(v []GetPayoutCountries200ResponseDataCountriesInnerFieldsInner)`

SetFields sets Fields field to given value.

### HasFields

`func (o *GetPayoutCountries200ResponseDataCountriesInner) HasFields() bool`

HasFields returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



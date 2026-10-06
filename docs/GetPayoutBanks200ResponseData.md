# GetPayoutBanks200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BanksListSupported** | Pointer to **bool** |  | [optional] 
**Banks** | Pointer to [**[]GetPayoutBanks200ResponseDataBanksInner**](GetPayoutBanks200ResponseDataBanksInner.md) |  | [optional] 

## Methods

### NewGetPayoutBanks200ResponseData

`func NewGetPayoutBanks200ResponseData() *GetPayoutBanks200ResponseData`

NewGetPayoutBanks200ResponseData instantiates a new GetPayoutBanks200ResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetPayoutBanks200ResponseDataWithDefaults

`func NewGetPayoutBanks200ResponseDataWithDefaults() *GetPayoutBanks200ResponseData`

NewGetPayoutBanks200ResponseDataWithDefaults instantiates a new GetPayoutBanks200ResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBanksListSupported

`func (o *GetPayoutBanks200ResponseData) GetBanksListSupported() bool`

GetBanksListSupported returns the BanksListSupported field if non-nil, zero value otherwise.

### GetBanksListSupportedOk

`func (o *GetPayoutBanks200ResponseData) GetBanksListSupportedOk() (*bool, bool)`

GetBanksListSupportedOk returns a tuple with the BanksListSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanksListSupported

`func (o *GetPayoutBanks200ResponseData) SetBanksListSupported(v bool)`

SetBanksListSupported sets BanksListSupported field to given value.

### HasBanksListSupported

`func (o *GetPayoutBanks200ResponseData) HasBanksListSupported() bool`

HasBanksListSupported returns a boolean if a field has been set.

### GetBanks

`func (o *GetPayoutBanks200ResponseData) GetBanks() []GetPayoutBanks200ResponseDataBanksInner`

GetBanks returns the Banks field if non-nil, zero value otherwise.

### GetBanksOk

`func (o *GetPayoutBanks200ResponseData) GetBanksOk() (*[]GetPayoutBanks200ResponseDataBanksInner, bool)`

GetBanksOk returns a tuple with the Banks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanks

`func (o *GetPayoutBanks200ResponseData) SetBanks(v []GetPayoutBanks200ResponseDataBanksInner)`

SetBanks sets Banks field to given value.

### HasBanks

`func (o *GetPayoutBanks200ResponseData) HasBanks() bool`

HasBanks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



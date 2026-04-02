# UsersExportData200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ExportedAt** | Pointer to **time.Time** |  | [optional] 
**User** | Pointer to [**User**](User.md) |  | [optional] 
**Projects** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Wallets** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Transactions** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Files** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Integrations** | Pointer to **[]map[string]interface{}** |  | [optional] 
**ApiKeys** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewUsersExportData200Response

`func NewUsersExportData200Response() *UsersExportData200Response`

NewUsersExportData200Response instantiates a new UsersExportData200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsersExportData200ResponseWithDefaults

`func NewUsersExportData200ResponseWithDefaults() *UsersExportData200Response`

NewUsersExportData200ResponseWithDefaults instantiates a new UsersExportData200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetExportedAt

`func (o *UsersExportData200Response) GetExportedAt() time.Time`

GetExportedAt returns the ExportedAt field if non-nil, zero value otherwise.

### GetExportedAtOk

`func (o *UsersExportData200Response) GetExportedAtOk() (*time.Time, bool)`

GetExportedAtOk returns a tuple with the ExportedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportedAt

`func (o *UsersExportData200Response) SetExportedAt(v time.Time)`

SetExportedAt sets ExportedAt field to given value.

### HasExportedAt

`func (o *UsersExportData200Response) HasExportedAt() bool`

HasExportedAt returns a boolean if a field has been set.

### GetUser

`func (o *UsersExportData200Response) GetUser() User`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *UsersExportData200Response) GetUserOk() (*User, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *UsersExportData200Response) SetUser(v User)`

SetUser sets User field to given value.

### HasUser

`func (o *UsersExportData200Response) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetProjects

`func (o *UsersExportData200Response) GetProjects() []map[string]interface{}`

GetProjects returns the Projects field if non-nil, zero value otherwise.

### GetProjectsOk

`func (o *UsersExportData200Response) GetProjectsOk() (*[]map[string]interface{}, bool)`

GetProjectsOk returns a tuple with the Projects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjects

`func (o *UsersExportData200Response) SetProjects(v []map[string]interface{})`

SetProjects sets Projects field to given value.

### HasProjects

`func (o *UsersExportData200Response) HasProjects() bool`

HasProjects returns a boolean if a field has been set.

### GetWallets

`func (o *UsersExportData200Response) GetWallets() []map[string]interface{}`

GetWallets returns the Wallets field if non-nil, zero value otherwise.

### GetWalletsOk

`func (o *UsersExportData200Response) GetWalletsOk() (*[]map[string]interface{}, bool)`

GetWalletsOk returns a tuple with the Wallets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWallets

`func (o *UsersExportData200Response) SetWallets(v []map[string]interface{})`

SetWallets sets Wallets field to given value.

### HasWallets

`func (o *UsersExportData200Response) HasWallets() bool`

HasWallets returns a boolean if a field has been set.

### GetTransactions

`func (o *UsersExportData200Response) GetTransactions() []map[string]interface{}`

GetTransactions returns the Transactions field if non-nil, zero value otherwise.

### GetTransactionsOk

`func (o *UsersExportData200Response) GetTransactionsOk() (*[]map[string]interface{}, bool)`

GetTransactionsOk returns a tuple with the Transactions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactions

`func (o *UsersExportData200Response) SetTransactions(v []map[string]interface{})`

SetTransactions sets Transactions field to given value.

### HasTransactions

`func (o *UsersExportData200Response) HasTransactions() bool`

HasTransactions returns a boolean if a field has been set.

### GetFiles

`func (o *UsersExportData200Response) GetFiles() []map[string]interface{}`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *UsersExportData200Response) GetFilesOk() (*[]map[string]interface{}, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *UsersExportData200Response) SetFiles(v []map[string]interface{})`

SetFiles sets Files field to given value.

### HasFiles

`func (o *UsersExportData200Response) HasFiles() bool`

HasFiles returns a boolean if a field has been set.

### GetIntegrations

`func (o *UsersExportData200Response) GetIntegrations() []map[string]interface{}`

GetIntegrations returns the Integrations field if non-nil, zero value otherwise.

### GetIntegrationsOk

`func (o *UsersExportData200Response) GetIntegrationsOk() (*[]map[string]interface{}, bool)`

GetIntegrationsOk returns a tuple with the Integrations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegrations

`func (o *UsersExportData200Response) SetIntegrations(v []map[string]interface{})`

SetIntegrations sets Integrations field to given value.

### HasIntegrations

`func (o *UsersExportData200Response) HasIntegrations() bool`

HasIntegrations returns a boolean if a field has been set.

### GetApiKeys

`func (o *UsersExportData200Response) GetApiKeys() []map[string]interface{}`

GetApiKeys returns the ApiKeys field if non-nil, zero value otherwise.

### GetApiKeysOk

`func (o *UsersExportData200Response) GetApiKeysOk() (*[]map[string]interface{}, bool)`

GetApiKeysOk returns a tuple with the ApiKeys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKeys

`func (o *UsersExportData200Response) SetApiKeys(v []map[string]interface{})`

SetApiKeys sets ApiKeys field to given value.

### HasApiKeys

`func (o *UsersExportData200Response) HasApiKeys() bool`

HasApiKeys returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



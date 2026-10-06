# RegisterRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**Password** | **string** |  | 
**FirstName** | **string** |  | 
**LastName** | **string** |  | 
**OrgName** | Pointer to **string** |  | [optional] 
**AgreedToTerms** | **bool** | Must be &#x60;true&#x60; - the server rejects the request otherwise. Required to stop a direct API call from creating an account without accepting the Terms of Service and Privacy Policy. | 
**Captcha** | Pointer to **string** | Google reCAPTCHA v3 response token, required only when the platform&#39;s anti-bot CAPTCHA gate is enabled. A missing token then gets a 400 with &#x60;captchaRequired: true&#x60; and a &#x60;siteKey&#x60;. Solving this needs a real browser, so this endpoint backs the web console&#39;s own signup form (&#x60;https://www.mudbase.dev/console/register&#x60;) and is not meant for scripted/server-to-server account creation. To integrate: create your Mudbase account once through the console, then use the API key from Settings -&gt; API Keys for everything else - collections, documents, storage, and the rest of the API are all fully scriptable from there. | [optional] 

## Methods

### NewRegisterRequest

`func NewRegisterRequest(email string, password string, firstName string, lastName string, agreedToTerms bool, ) *RegisterRequest`

NewRegisterRequest instantiates a new RegisterRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterRequestWithDefaults

`func NewRegisterRequestWithDefaults() *RegisterRequest`

NewRegisterRequestWithDefaults instantiates a new RegisterRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *RegisterRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *RegisterRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *RegisterRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetPassword

`func (o *RegisterRequest) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *RegisterRequest) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *RegisterRequest) SetPassword(v string)`

SetPassword sets Password field to given value.


### GetFirstName

`func (o *RegisterRequest) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *RegisterRequest) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *RegisterRequest) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.


### GetLastName

`func (o *RegisterRequest) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *RegisterRequest) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *RegisterRequest) SetLastName(v string)`

SetLastName sets LastName field to given value.


### GetOrgName

`func (o *RegisterRequest) GetOrgName() string`

GetOrgName returns the OrgName field if non-nil, zero value otherwise.

### GetOrgNameOk

`func (o *RegisterRequest) GetOrgNameOk() (*string, bool)`

GetOrgNameOk returns a tuple with the OrgName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrgName

`func (o *RegisterRequest) SetOrgName(v string)`

SetOrgName sets OrgName field to given value.

### HasOrgName

`func (o *RegisterRequest) HasOrgName() bool`

HasOrgName returns a boolean if a field has been set.

### GetAgreedToTerms

`func (o *RegisterRequest) GetAgreedToTerms() bool`

GetAgreedToTerms returns the AgreedToTerms field if non-nil, zero value otherwise.

### GetAgreedToTermsOk

`func (o *RegisterRequest) GetAgreedToTermsOk() (*bool, bool)`

GetAgreedToTermsOk returns a tuple with the AgreedToTerms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAgreedToTerms

`func (o *RegisterRequest) SetAgreedToTerms(v bool)`

SetAgreedToTerms sets AgreedToTerms field to given value.


### GetCaptcha

`func (o *RegisterRequest) GetCaptcha() string`

GetCaptcha returns the Captcha field if non-nil, zero value otherwise.

### GetCaptchaOk

`func (o *RegisterRequest) GetCaptchaOk() (*string, bool)`

GetCaptchaOk returns a tuple with the Captcha field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCaptcha

`func (o *RegisterRequest) SetCaptcha(v string)`

SetCaptcha sets Captcha field to given value.

### HasCaptcha

`func (o *RegisterRequest) HasCaptcha() bool`

HasCaptcha returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ChatSendMessageRequestE2ee

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | Pointer to **int32** |  | [optional] [default to 1]
**Scheme** | Pointer to **string** |  | [optional] 
**Ciphertext** | Pointer to **string** | Base64-encoded ciphertext. | [optional] 
**Nonce** | Pointer to **string** |  | [optional] 
**EphemeralPublicKey** | Pointer to **string** |  | [optional] 
**SenderKeyId** | Pointer to **string** |  | [optional] 

## Methods

### NewChatSendMessageRequestE2ee

`func NewChatSendMessageRequestE2ee() *ChatSendMessageRequestE2ee`

NewChatSendMessageRequestE2ee instantiates a new ChatSendMessageRequestE2ee object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatSendMessageRequestE2eeWithDefaults

`func NewChatSendMessageRequestE2eeWithDefaults() *ChatSendMessageRequestE2ee`

NewChatSendMessageRequestE2eeWithDefaults instantiates a new ChatSendMessageRequestE2ee object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *ChatSendMessageRequestE2ee) GetVersion() int32`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ChatSendMessageRequestE2ee) GetVersionOk() (*int32, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ChatSendMessageRequestE2ee) SetVersion(v int32)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *ChatSendMessageRequestE2ee) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetScheme

`func (o *ChatSendMessageRequestE2ee) GetScheme() string`

GetScheme returns the Scheme field if non-nil, zero value otherwise.

### GetSchemeOk

`func (o *ChatSendMessageRequestE2ee) GetSchemeOk() (*string, bool)`

GetSchemeOk returns a tuple with the Scheme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheme

`func (o *ChatSendMessageRequestE2ee) SetScheme(v string)`

SetScheme sets Scheme field to given value.

### HasScheme

`func (o *ChatSendMessageRequestE2ee) HasScheme() bool`

HasScheme returns a boolean if a field has been set.

### GetCiphertext

`func (o *ChatSendMessageRequestE2ee) GetCiphertext() string`

GetCiphertext returns the Ciphertext field if non-nil, zero value otherwise.

### GetCiphertextOk

`func (o *ChatSendMessageRequestE2ee) GetCiphertextOk() (*string, bool)`

GetCiphertextOk returns a tuple with the Ciphertext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCiphertext

`func (o *ChatSendMessageRequestE2ee) SetCiphertext(v string)`

SetCiphertext sets Ciphertext field to given value.

### HasCiphertext

`func (o *ChatSendMessageRequestE2ee) HasCiphertext() bool`

HasCiphertext returns a boolean if a field has been set.

### GetNonce

`func (o *ChatSendMessageRequestE2ee) GetNonce() string`

GetNonce returns the Nonce field if non-nil, zero value otherwise.

### GetNonceOk

`func (o *ChatSendMessageRequestE2ee) GetNonceOk() (*string, bool)`

GetNonceOk returns a tuple with the Nonce field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNonce

`func (o *ChatSendMessageRequestE2ee) SetNonce(v string)`

SetNonce sets Nonce field to given value.

### HasNonce

`func (o *ChatSendMessageRequestE2ee) HasNonce() bool`

HasNonce returns a boolean if a field has been set.

### GetEphemeralPublicKey

`func (o *ChatSendMessageRequestE2ee) GetEphemeralPublicKey() string`

GetEphemeralPublicKey returns the EphemeralPublicKey field if non-nil, zero value otherwise.

### GetEphemeralPublicKeyOk

`func (o *ChatSendMessageRequestE2ee) GetEphemeralPublicKeyOk() (*string, bool)`

GetEphemeralPublicKeyOk returns a tuple with the EphemeralPublicKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEphemeralPublicKey

`func (o *ChatSendMessageRequestE2ee) SetEphemeralPublicKey(v string)`

SetEphemeralPublicKey sets EphemeralPublicKey field to given value.

### HasEphemeralPublicKey

`func (o *ChatSendMessageRequestE2ee) HasEphemeralPublicKey() bool`

HasEphemeralPublicKey returns a boolean if a field has been set.

### GetSenderKeyId

`func (o *ChatSendMessageRequestE2ee) GetSenderKeyId() string`

GetSenderKeyId returns the SenderKeyId field if non-nil, zero value otherwise.

### GetSenderKeyIdOk

`func (o *ChatSendMessageRequestE2ee) GetSenderKeyIdOk() (*string, bool)`

GetSenderKeyIdOk returns a tuple with the SenderKeyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderKeyId

`func (o *ChatSendMessageRequestE2ee) SetSenderKeyId(v string)`

SetSenderKeyId sets SenderKeyId field to given value.

### HasSenderKeyId

`func (o *ChatSendMessageRequestE2ee) HasSenderKeyId() bool`

HasSenderKeyId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ComplianceLogSecurityEventRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EventType** | **string** |  | 
**Severity** | **string** |  | 
**Details** | Pointer to [**ComplianceLogSecurityEventRequestDetails**](ComplianceLogSecurityEventRequestDetails.md) |  | [optional] 

## Methods

### NewComplianceLogSecurityEventRequest

`func NewComplianceLogSecurityEventRequest(eventType string, severity string, ) *ComplianceLogSecurityEventRequest`

NewComplianceLogSecurityEventRequest instantiates a new ComplianceLogSecurityEventRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComplianceLogSecurityEventRequestWithDefaults

`func NewComplianceLogSecurityEventRequestWithDefaults() *ComplianceLogSecurityEventRequest`

NewComplianceLogSecurityEventRequestWithDefaults instantiates a new ComplianceLogSecurityEventRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEventType

`func (o *ComplianceLogSecurityEventRequest) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *ComplianceLogSecurityEventRequest) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *ComplianceLogSecurityEventRequest) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetSeverity

`func (o *ComplianceLogSecurityEventRequest) GetSeverity() string`

GetSeverity returns the Severity field if non-nil, zero value otherwise.

### GetSeverityOk

`func (o *ComplianceLogSecurityEventRequest) GetSeverityOk() (*string, bool)`

GetSeverityOk returns a tuple with the Severity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeverity

`func (o *ComplianceLogSecurityEventRequest) SetSeverity(v string)`

SetSeverity sets Severity field to given value.


### GetDetails

`func (o *ComplianceLogSecurityEventRequest) GetDetails() ComplianceLogSecurityEventRequestDetails`

GetDetails returns the Details field if non-nil, zero value otherwise.

### GetDetailsOk

`func (o *ComplianceLogSecurityEventRequest) GetDetailsOk() (*ComplianceLogSecurityEventRequestDetails, bool)`

GetDetailsOk returns a tuple with the Details field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetails

`func (o *ComplianceLogSecurityEventRequest) SetDetails(v ComplianceLogSecurityEventRequestDetails)`

SetDetails sets Details field to given value.

### HasDetails

`func (o *ComplianceLogSecurityEventRequest) HasDetails() bool`

HasDetails returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



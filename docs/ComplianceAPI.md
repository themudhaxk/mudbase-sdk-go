# \ComplianceAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ComplianceLogSecurityEvent**](ComplianceAPI.md#ComplianceLogSecurityEvent) | **Post** /api/compliance/security-event | Log security event



## ComplianceLogSecurityEvent

> ComplianceLogSecurityEvent200Response ComplianceLogSecurityEvent(ctx).ComplianceLogSecurityEventRequest(complianceLogSecurityEventRequest).Execute()

Log security event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	complianceLogSecurityEventRequest := *openapiclient.NewComplianceLogSecurityEventRequest("unauthorized_access_attempt", "high") // ComplianceLogSecurityEventRequest | Event type (e.g. unauthorized_access_attempt, brute_force_attempt), severity (low–critical), and optional details object for context.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ComplianceAPI.ComplianceLogSecurityEvent(context.Background()).ComplianceLogSecurityEventRequest(complianceLogSecurityEventRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ComplianceAPI.ComplianceLogSecurityEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ComplianceLogSecurityEvent`: ComplianceLogSecurityEvent200Response
	fmt.Fprintf(os.Stdout, "Response from `ComplianceAPI.ComplianceLogSecurityEvent`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiComplianceLogSecurityEventRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **complianceLogSecurityEventRequest** | [**ComplianceLogSecurityEventRequest**](ComplianceLogSecurityEventRequest.md) | Event type (e.g. unauthorized_access_attempt, brute_force_attempt), severity (low–critical), and optional details object for context. | 

### Return type

[**ComplianceLogSecurityEvent200Response**](ComplianceLogSecurityEvent200Response.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


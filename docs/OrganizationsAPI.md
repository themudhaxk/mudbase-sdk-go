# \OrganizationsAPI

All URIs are relative to *https://cloud.mudbase.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**OrganizationsAddDomain**](OrganizationsAPI.md#OrganizationsAddDomain) | **Post** /api/orgs/{orgId}/projects/{projectId}/domains | Add custom domain
[**OrganizationsListDomains**](OrganizationsAPI.md#OrganizationsListDomains) | **Get** /api/orgs/{orgId}/projects/{projectId}/domains | List custom domains and DNS TXT hints
[**OrganizationsPatchDomain**](OrganizationsAPI.md#OrganizationsPatchDomain) | **Patch** /api/orgs/{orgId}/projects/{projectId}/domains/{hostname} | Patch domain status or regenerate token
[**OrganizationsRemoveDomain**](OrganizationsAPI.md#OrganizationsRemoveDomain) | **Delete** /api/orgs/{orgId}/projects/{projectId}/domains/{hostname} | Remove custom domain
[**OrganizationsReportDomainPlatformReady**](OrganizationsAPI.md#OrganizationsReportDomainPlatformReady) | **Post** /api/orgs/{orgId}/projects/{projectId}/domains/{hostname}/platform-ready | Notify platform ops hosting / edge ready
[**OrganizationsSetPrimaryDomain**](OrganizationsAPI.md#OrganizationsSetPrimaryDomain) | **Patch** /api/orgs/{orgId}/projects/{projectId}/domains/primary | Set primary custom domain
[**OrganizationsVerifyDomainDns**](OrganizationsAPI.md#OrganizationsVerifyDomainDns) | **Post** /api/orgs/{orgId}/projects/{projectId}/domains/{hostname}/verify-dns | Verify domain via DNS TXT



## OrganizationsAddDomain

> OrganizationsAddDomain(ctx, orgId, projectId).OrganizationsAddDomainRequest(organizationsAddDomainRequest).Execute()

Add custom domain

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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	organizationsAddDomainRequest := *openapiclient.NewOrganizationsAddDomainRequest("Hostname_example") // OrganizationsAddDomainRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsAddDomain(context.Background(), orgId, projectId).OrganizationsAddDomainRequest(organizationsAddDomainRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsAddDomain``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsAddDomainRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **organizationsAddDomainRequest** | [**OrganizationsAddDomainRequest**](OrganizationsAddDomainRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsListDomains

> OrganizationsListDomains(ctx, orgId, projectId).Execute()

List custom domains and DNS TXT hints



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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsListDomains(context.Background(), orgId, projectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsListDomains``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsListDomainsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsPatchDomain

> OrganizationsPatchDomain(ctx, orgId, projectId, hostname).OrganizationsPatchDomainRequest(organizationsPatchDomainRequest).Execute()

Patch domain status or regenerate token

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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	hostname := "hostname_example" // string | 
	organizationsPatchDomainRequest := *openapiclient.NewOrganizationsPatchDomainRequest() // OrganizationsPatchDomainRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsPatchDomain(context.Background(), orgId, projectId, hostname).OrganizationsPatchDomainRequest(organizationsPatchDomainRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsPatchDomain``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 
**hostname** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsPatchDomainRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **organizationsPatchDomainRequest** | [**OrganizationsPatchDomainRequest**](OrganizationsPatchDomainRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsRemoveDomain

> OrganizationsRemoveDomain(ctx, orgId, projectId, hostname).Execute()

Remove custom domain

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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	hostname := "hostname_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsRemoveDomain(context.Background(), orgId, projectId, hostname).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsRemoveDomain``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 
**hostname** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsRemoveDomainRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsReportDomainPlatformReady

> OrganizationsReportDomainPlatformReady(ctx, orgId, projectId, hostname).OrganizationsReportDomainPlatformReadyRequest(organizationsReportDomainPlatformReadyRequest).Execute()

Notify platform ops hosting / edge ready



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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	hostname := "hostname_example" // string | 
	organizationsReportDomainPlatformReadyRequest := *openapiclient.NewOrganizationsReportDomainPlatformReadyRequest() // OrganizationsReportDomainPlatformReadyRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsReportDomainPlatformReady(context.Background(), orgId, projectId, hostname).OrganizationsReportDomainPlatformReadyRequest(organizationsReportDomainPlatformReadyRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsReportDomainPlatformReady``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 
**hostname** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsReportDomainPlatformReadyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **organizationsReportDomainPlatformReadyRequest** | [**OrganizationsReportDomainPlatformReadyRequest**](OrganizationsReportDomainPlatformReadyRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsSetPrimaryDomain

> OrganizationsSetPrimaryDomain(ctx, orgId, projectId).OrganizationsSetPrimaryDomainRequest(organizationsSetPrimaryDomainRequest).Execute()

Set primary custom domain

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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	organizationsSetPrimaryDomainRequest := *openapiclient.NewOrganizationsSetPrimaryDomainRequest("Hostname_example") // OrganizationsSetPrimaryDomainRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsSetPrimaryDomain(context.Background(), orgId, projectId).OrganizationsSetPrimaryDomainRequest(organizationsSetPrimaryDomainRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsSetPrimaryDomain``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsSetPrimaryDomainRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **organizationsSetPrimaryDomainRequest** | [**OrganizationsSetPrimaryDomainRequest**](OrganizationsSetPrimaryDomainRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrganizationsVerifyDomainDns

> OrganizationsVerifyDomainDns(ctx, orgId, projectId, hostname).Execute()

Verify domain via DNS TXT



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
	orgId := "orgId_example" // string | 
	projectId := "projectId_example" // string | 
	hostname := "hostname_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.OrganizationsVerifyDomainDns(context.Background(), orgId, projectId, hostname).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.OrganizationsVerifyDomainDns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**orgId** | **string** |  | 
**projectId** | **string** |  | 
**hostname** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrganizationsVerifyDomainDnsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

 (empty response body)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


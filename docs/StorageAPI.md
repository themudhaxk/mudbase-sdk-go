# \StorageAPI

All URIs are relative to *https://cloud.dev.mudbase*

Method | HTTP request | Description
------------- | ------------- | -------------
[**StorageConfirmUpload**](StorageAPI.md#StorageConfirmUpload) | **Post** /api/files/upload/confirm | Confirm direct upload (scan + finalize metadata)
[**StorageCreateBucket**](StorageAPI.md#StorageCreateBucket) | **Post** /api/bucket/projects/{projectId}/buckets | Create a new bucket
[**StorageDeleteBucket**](StorageAPI.md#StorageDeleteBucket) | **Delete** /api/bucket/projects/{projectId}/buckets/{bucketId} | Delete bucket
[**StorageDeleteFile**](StorageAPI.md#StorageDeleteFile) | **Delete** /api/bucket/projects/{projectId}/buckets/{bucketId}/files/{fileId} | Delete file
[**StorageDownloadBucketFile**](StorageAPI.md#StorageDownloadBucketFile) | **Get** /api/bucket/files/{fileId}/download | Download file from bucket
[**StorageDownloadFile**](StorageAPI.md#StorageDownloadFile) | **Get** /api/files/{fileId}/download | Generate a presigned URL for downloading a file
[**StorageGetBucket**](StorageAPI.md#StorageGetBucket) | **Get** /api/bucket/projects/{projectId}/buckets/{bucketId} | Get bucket details
[**StorageGetFile**](StorageAPI.md#StorageGetFile) | **Get** /api/bucket/projects/{projectId}/buckets/{bucketId}/files/{fileId} | Get file metadata
[**StorageGetPresignedUpload**](StorageAPI.md#StorageGetPresignedUpload) | **Post** /api/files/upload/presigned | Generate presigned POST data for direct browser upload
[**StorageGetSignedUrl**](StorageAPI.md#StorageGetSignedUrl) | **Post** /api/bucket/projects/{projectId}/buckets/{bucketId}/files/{fileId}/signed-url | Generate signed URL for file
[**StorageListBuckets**](StorageAPI.md#StorageListBuckets) | **Get** /api/bucket/projects/{projectId}/buckets | List buckets in a project
[**StorageListFiles**](StorageAPI.md#StorageListFiles) | **Get** /api/bucket/projects/{projectId}/buckets/{bucketId}/files | List files in bucket
[**StorageUpdateBucket**](StorageAPI.md#StorageUpdateBucket) | **Patch** /api/bucket/projects/{projectId}/buckets/{bucketId} | Update bucket
[**StorageUploadFiles**](StorageAPI.md#StorageUploadFiles) | **Post** /api/bucket/projects/{projectId}/buckets/{bucketId}/files | Upload files to bucket



## StorageConfirmUpload

> ConfirmUploadResponse StorageConfirmUpload(ctx).StorageConfirmUploadRequest(storageConfirmUploadRequest).Execute()

Confirm direct upload (scan + finalize metadata)



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
	storageConfirmUploadRequest := *openapiclient.NewStorageConfirmUploadRequest("Key_example", "ProjectId_example") // StorageConfirmUploadRequest | S3 key from presigned response, projectId, and optional originalName, contentType, size, bucket, isPublic.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageConfirmUpload(context.Background()).StorageConfirmUploadRequest(storageConfirmUploadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageConfirmUpload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageConfirmUpload`: ConfirmUploadResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageConfirmUpload`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStorageConfirmUploadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storageConfirmUploadRequest** | [**StorageConfirmUploadRequest**](StorageConfirmUploadRequest.md) | S3 key from presigned response, projectId, and optional originalName, contentType, size, bucket, isPublic. | 

### Return type

[**ConfirmUploadResponse**](ConfirmUploadResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageCreateBucket

> BucketResponse StorageCreateBucket(ctx, projectId).CreateBucketRequest(createBucketRequest).Execute()

Create a new bucket



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
	projectId := "projectId_example" // string | Project ID.
	createBucketRequest := *openapiclient.NewCreateBucketRequest("Name_example") // CreateBucketRequest | Bucket name, isPublic flag, and optional settings.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageCreateBucket(context.Background(), projectId).CreateBucketRequest(createBucketRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageCreateBucket``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageCreateBucket`: BucketResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageCreateBucket`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageCreateBucketRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createBucketRequest** | [**CreateBucketRequest**](CreateBucketRequest.md) | Bucket name, isPublic flag, and optional settings. | 

### Return type

[**BucketResponse**](BucketResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageDeleteBucket

> MessageResponse StorageDeleteBucket(ctx, projectId, bucketId).Execute()

Delete bucket



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageDeleteBucket(context.Background(), projectId, bucketId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageDeleteBucket``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageDeleteBucket`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageDeleteBucket`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageDeleteBucketRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageDeleteFile

> MessageResponse StorageDeleteFile(ctx, projectId, bucketId, fileId).Execute()

Delete file



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	fileId := "fileId_example" // string | File ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageDeleteFile(context.Background(), projectId, bucketId, fileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageDeleteFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageDeleteFile`: MessageResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageDeleteFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 
**fileId** | **string** | File ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageDeleteFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**MessageResponse**](MessageResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageDownloadBucketFile

> *os.File StorageDownloadBucketFile(ctx, fileId).Token(token).Execute()

Download file from bucket



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
	fileId := "685af8b85d73a104065b6a77" // string | File ID to download.
	token := "token_example" // string | Download token for private files (from signed URL endpoint). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageDownloadBucketFile(context.Background(), fileId).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageDownloadBucketFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageDownloadBucketFile`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageDownloadBucketFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**fileId** | **string** | File ID to download. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageDownloadBucketFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **token** | **string** | Download token for private files (from signed URL endpoint). | 

### Return type

[***os.File**](*os.File.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageDownloadFile

> SignedUrlResponse StorageDownloadFile(ctx, fileId).Token(token).Execute()

Generate a presigned URL for downloading a file



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
	fileId := "fileId_example" // string | File ID.
	token := "token_example" // string | Optional one-time download token (if provided by upload flow). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageDownloadFile(context.Background(), fileId).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageDownloadFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageDownloadFile`: SignedUrlResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageDownloadFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**fileId** | **string** | File ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageDownloadFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **token** | **string** | Optional one-time download token (if provided by upload flow). | 

### Return type

[**SignedUrlResponse**](SignedUrlResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageGetBucket

> BucketResponse StorageGetBucket(ctx, projectId, bucketId).Execute()

Get bucket details



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageGetBucket(context.Background(), projectId, bucketId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageGetBucket``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageGetBucket`: BucketResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageGetBucket`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageGetBucketRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**BucketResponse**](BucketResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageGetFile

> FileResponse StorageGetFile(ctx, projectId, bucketId, fileId).Execute()

Get file metadata



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	fileId := "fileId_example" // string | File ID.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageGetFile(context.Background(), projectId, bucketId, fileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageGetFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageGetFile`: FileResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageGetFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 
**fileId** | **string** | File ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageGetFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**FileResponse**](FileResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageGetPresignedUpload

> PresignedPostResponse StorageGetPresignedUpload(ctx).StorageGetPresignedUploadRequest(storageGetPresignedUploadRequest).Execute()

Generate presigned POST data for direct browser upload



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
	storageGetPresignedUploadRequest := *openapiclient.NewStorageGetPresignedUploadRequest("ProjectId_example", "OriginalName_example") // StorageGetPresignedUploadRequest | projectId, originalName, optional bucket, contentType, isPublic.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageGetPresignedUpload(context.Background()).StorageGetPresignedUploadRequest(storageGetPresignedUploadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageGetPresignedUpload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageGetPresignedUpload`: PresignedPostResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageGetPresignedUpload`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStorageGetPresignedUploadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storageGetPresignedUploadRequest** | [**StorageGetPresignedUploadRequest**](StorageGetPresignedUploadRequest.md) | projectId, originalName, optional bucket, contentType, isPublic. | 

### Return type

[**PresignedPostResponse**](PresignedPostResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageGetSignedUrl

> SignedUrlResponse StorageGetSignedUrl(ctx, projectId, bucketId, fileId).StorageGetSignedUrlRequest(storageGetSignedUrlRequest).Execute()

Generate signed URL for file



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	fileId := "fileId_example" // string | File ID.
	storageGetSignedUrlRequest := *openapiclient.NewStorageGetSignedUrlRequest() // StorageGetSignedUrlRequest | Optional expiresIn (seconds) for the signed URL. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageGetSignedUrl(context.Background(), projectId, bucketId, fileId).StorageGetSignedUrlRequest(storageGetSignedUrlRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageGetSignedUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageGetSignedUrl`: SignedUrlResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageGetSignedUrl`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 
**fileId** | **string** | File ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageGetSignedUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **storageGetSignedUrlRequest** | [**StorageGetSignedUrlRequest**](StorageGetSignedUrlRequest.md) | Optional expiresIn (seconds) for the signed URL. | 

### Return type

[**SignedUrlResponse**](SignedUrlResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageListBuckets

> BucketListResponse StorageListBuckets(ctx, projectId).Page(page).Limit(limit).Search(search).Execute()

List buckets in a project



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
	projectId := "projectId_example" // string | Project ID.
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Number of buckets per page. (optional) (default to 20)
	search := "search_example" // string | Search by bucket name. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageListBuckets(context.Background(), projectId).Page(page).Limit(limit).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageListBuckets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageListBuckets`: BucketListResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageListBuckets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageListBucketsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of buckets per page. | [default to 20]
 **search** | **string** | Search by bucket name. | 

### Return type

[**BucketListResponse**](BucketListResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageListFiles

> FileListResponse StorageListFiles(ctx, projectId, bucketId).Page(page).Limit(limit).Search(search).Type_(type_).Execute()

List files in bucket



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	page := int32(56) // int32 | Page number (1-based). (optional) (default to 1)
	limit := int32(56) // int32 | Number of files per page. (optional) (default to 20)
	search := "search_example" // string | Search by filename. (optional)
	type_ := "type__example" // string | Filter by MIME type or file type. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageListFiles(context.Background(), projectId, bucketId).Page(page).Limit(limit).Search(search).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageListFiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageListFiles`: FileListResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageListFiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageListFilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **page** | **int32** | Page number (1-based). | [default to 1]
 **limit** | **int32** | Number of files per page. | [default to 20]
 **search** | **string** | Search by filename. | 
 **type_** | **string** | Filter by MIME type or file type. | 

### Return type

[**FileListResponse**](FileListResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageUpdateBucket

> BucketResponse StorageUpdateBucket(ctx, projectId, bucketId).UpdateBucketRequest(updateBucketRequest).Execute()

Update bucket



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	updateBucketRequest := *openapiclient.NewUpdateBucketRequest() // UpdateBucketRequest | Fields to update (name, isPublic, settings).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageUpdateBucket(context.Background(), projectId, bucketId).UpdateBucketRequest(updateBucketRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageUpdateBucket``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageUpdateBucket`: BucketResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageUpdateBucket`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageUpdateBucketRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateBucketRequest** | [**UpdateBucketRequest**](UpdateBucketRequest.md) | Fields to update (name, isPublic, settings). | 

### Return type

[**BucketResponse**](BucketResponse.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StorageUploadFiles

> FileUploadResponse StorageUploadFiles(ctx, projectId, bucketId).UploadFilesToBucketRequest(uploadFilesToBucketRequest).Execute()

Upload files to bucket



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
	projectId := "projectId_example" // string | Project ID.
	bucketId := "bucketId_example" // string | Bucket ID.
	uploadFilesToBucketRequest := *openapiclient.NewUploadFilesToBucketRequest([]*os.File{"TODO"}) // UploadFilesToBucketRequest | Use multipart/form-data for file upload (files required; optional folder, tags). application/json uses the same schema for metadata-only or tooling that prefers JSON.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageAPI.StorageUploadFiles(context.Background(), projectId, bucketId).UploadFilesToBucketRequest(uploadFilesToBucketRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageAPI.StorageUploadFiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StorageUploadFiles`: FileUploadResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageAPI.StorageUploadFiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project ID. | 
**bucketId** | **string** | Bucket ID. | 

### Other Parameters

Other parameters are passed through a pointer to a apiStorageUploadFilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **uploadFilesToBucketRequest** | [**UploadFilesToBucketRequest**](UploadFilesToBucketRequest.md) | Use multipart/form-data for file upload (files required; optional folder, tags). application/json uses the same schema for metadata-only or tooling that prefers JSON. | 

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: application/json, multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


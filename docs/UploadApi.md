# \UploadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_files**](UploadApi.md#create_files) | **POST** /api/v1/files | Upload@upload
[**delete_files_processed**](UploadApi.md#delete_files_processed) | **DELETE** /api/v1/files/processed/{id} | Upload@destroy
[**fetch_files**](UploadApi.md#fetch_files) | **GET** /api/v1/files/{uuid} | Upload@show
[**fetch_files_processed_content**](UploadApi.md#fetch_files_processed_content) | **GET** /api/v1/files/processed/{uuid}/download | Upload@content



## create_files

> models::CreateFiles200Response create_files(entity_flag, team_id, application_id, question_id)
Upload@upload

Upload a file to the gateway-api via scanning sub-service

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**entity_flag** | Option<**String**> | Flag to indicate the purpose of the file upload e.g. dur-from-upload |  |
**team_id** | Option<**i32**> | Id of team associated with the file upload |  |
**application_id** | Option<**i32**> | Id of dar application associated with the file upload |  |
**question_id** | Option<**i32**> | Id of the question in the dar application associated with the file upload |  |

### Return type

[**models::CreateFiles200Response**](create_files_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_files_processed

> models::DeleteAliases200Response delete_files_processed(id)
Upload@destroy

Delete a processed file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | file uuid | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_files

> models::FetchFiles200Response fetch_files(uuid)
Upload@show

Get the scanning status of an upload

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | upload id | [required] |

### Return type

[**models::FetchFiles200Response**](fetch_files_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_files_processed_content

> models::FetchFilesProcessedContent200Response fetch_files_processed_content(uuid)
Upload@content

Get the content of a processed file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | upload id | [required] |

### Return type

[**models::FetchFilesProcessedContent200Response**](fetch_files_processed_content_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


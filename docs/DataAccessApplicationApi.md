# \DataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_dar_application_files**](DataAccessApplicationApi.md#delete_dar_application_files) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**delete_dar_applications**](DataAccessApplicationApi.md#delete_dar_applications) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy
[**delete_team_dar_application_file**](DataAccessApplicationApi.md#delete_team_dar_application_file) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**fetch_team_dar_application_answers**](DataAccessApplicationApi.md#fetch_team_dar_application_answers) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers
[**fetch_team_dar_application_download_zip**](DataAccessApplicationApi.md#fetch_team_dar_application_download_zip) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download
[**fetch_team_dar_application_file**](DataAccessApplicationApi.md#fetch_team_dar_application_file) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**fetch_team_dar_application_files**](DataAccessApplicationApi.md#fetch_team_dar_application_files) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**fetch_team_dar_application_status_history**](DataAccessApplicationApi.md#fetch_team_dar_application_status_history) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status
[**update_team_dar_application**](DataAccessApplicationApi.md#update_team_dar_application) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update



## delete_dar_application_files

> models::DeleteApplications200Response delete_dar_application_files(id, file_id)
DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |
**file_id** | **String** | File id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_applications

> models::DeleteApplications200Response delete_dar_applications(id)
DataAccessApplication@destroy

Delete a system DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_dar_application_file

> models::DeleteApplications200Response delete_team_dar_application_file(team_id, id, file_id)
DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**file_id** | **i32** | File id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_answers

> models::FetchTeamDarApplicationAnswers200Response fetch_team_dar_application_answers(team_id, id)
DataAccessApplication@showAnswers

Return answers from a single DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationAnswers200Response**](fetch_team_dar_application_answers_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_download_zip

> fetch_team_dar_application_download_zip(team_id, id)
DataAccessApplication@download

Returns a DAR form as a CSV with attached files as a zip

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_file

> fetch_team_dar_application_file(team_id, id, file_id)
DataAccessApplication@downloadFile

Download a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**file_id** | **String** | File uuid | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_files

> models::FetchTeamDarApplicationFiles200Response fetch_team_dar_application_files(team_id, id)
DataAccessApplication@showFiles

Return a list of files associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationFiles200Response**](fetch_team_dar_application_files_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_status_history

> models::FetchTeamDarApplicationStatusHistory200Response fetch_team_dar_application_status_history(team_id, id)
DataAccessApplication@status

Return the status history of a single DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationStatusHistory200Response**](fetch_team_dar_application_status_history_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_team_dar_application

> models::FetchTeamDarApplication200Response update_team_dar_application(team_id, id, update_team_dar_application_request)
DataAccessApplication@update

Edit a system DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**update_team_dar_application_request** | [**UpdateTeamDarApplicationRequest**](UpdateTeamDarApplicationRequest.md) | DataAccessApplication definition | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


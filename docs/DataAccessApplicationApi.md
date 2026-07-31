# \DataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_applications**](DataAccessApplicationApi.md#create_dar_applications) | **POST** /api/v1/dar/applications | DataAccessApplication@store
[**delete_dar_application_files**](DataAccessApplicationApi.md#delete_dar_application_files) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**delete_dar_applications**](DataAccessApplicationApi.md#delete_dar_applications) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy
[**delete_team_dar_application_file**](DataAccessApplicationApi.md#delete_team_dar_application_file) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**delete_user_dar_application**](DataAccessApplicationApi.md#delete_user_dar_application) | **DELETE** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@destroy
[**delete_user_dar_application_file**](DataAccessApplicationApi.md#delete_user_dar_application_file) | **DELETE** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**fetch_team_dar_application_answers**](DataAccessApplicationApi.md#fetch_team_dar_application_answers) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers
[**fetch_team_dar_application_download_zip**](DataAccessApplicationApi.md#fetch_team_dar_application_download_zip) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download
[**fetch_team_dar_application_file**](DataAccessApplicationApi.md#fetch_team_dar_application_file) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**fetch_team_dar_application_files**](DataAccessApplicationApi.md#fetch_team_dar_application_files) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**fetch_team_dar_application_status_history**](DataAccessApplicationApi.md#fetch_team_dar_application_status_history) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status
[**fetch_user_dar_application_file**](DataAccessApplicationApi.md#fetch_user_dar_application_file) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**fetch_user_dar_application_files**](DataAccessApplicationApi.md#fetch_user_dar_application_files) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**patch_user_dar_application**](DataAccessApplicationApi.md#patch_user_dar_application) | **PATCH** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update
[**update_team_dar_application**](DataAccessApplicationApi.md#update_team_dar_application) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update
[**update_user_dar_application**](DataAccessApplicationApi.md#update_user_dar_application) | **PUT** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update



## create_dar_applications

> models::CreateCategories200Response create_dar_applications(create_dar_applications_request)
DataAccessApplication@store

Creates a new DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_dar_applications_request** | [**CreateDarApplicationsRequest**](CreateDarApplicationsRequest.md) | DataAccessApplication definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_application_files

> models::DeleteAliases200Response delete_dar_application_files(id, file_id)
DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |
**file_id** | **String** | File id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_applications

> models::DeleteAliases200Response delete_dar_applications(id)
DataAccessApplication@destroy

Delete a system DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_dar_application_file

> models::DeleteAliases200Response delete_team_dar_application_file(team_id, id, file_id)
DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**file_id** | **i32** | File id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_user_dar_application

> models::DeleteAliases200Response delete_user_dar_application(user_id, id)
DataAccessApplication@destroy

Delete a users DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_user_dar_application_file

> models::DeleteAliases200Response delete_user_dar_application_file(id, user_id, file_id)
DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |
**user_id** | **i32** | User id | [required] |
**file_id** | **String** | File uuid | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

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


## fetch_user_dar_application_file

> fetch_user_dar_application_file(id, user_id, file_id)
DataAccessApplication@downloadFile

Download a file associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |
**user_id** | **i32** | User id | [required] |
**file_id** | **String** | File id | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_files

> models::FetchTeamDarApplicationFiles200Response fetch_user_dar_application_files(id, user_id)
DataAccessApplication@showFiles

Return a list of files associated with a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR application id | [required] |
**user_id** | **i32** | User id | [required] |

### Return type

[**models::FetchTeamDarApplicationFiles200Response**](fetch_team_dar_application_files_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_user_dar_application

> models::FetchTeamDarApplication200Response patch_user_dar_application(user_id, id, patch_user_dar_application_request)
DataAccessApplication@update

Edit a system DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**patch_user_dar_application_request** | [**PatchUserDarApplicationRequest**](PatchUserDarApplicationRequest.md) | DataAccessApplication definition | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
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


## update_user_dar_application

> models::FetchTeamDarApplication200Response update_user_dar_application(user_id, id, update_user_dar_application_request)
DataAccessApplication@update

Update a system DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**update_user_dar_application_request** | [**UpdateUserDarApplicationRequest**](UpdateUserDarApplicationRequest.md) | DataAccessApplication definition | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \ProgrammingLanguageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_languages**](ProgrammingLanguageApi.md#create_programming_languages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
[**delete_programming_languages**](ProgrammingLanguageApi.md#delete_programming_languages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
[**edit_programming_languages**](ProgrammingLanguageApi.md#edit_programming_languages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
[**update_programming_languages**](ProgrammingLanguageApi.md#update_programming_languages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update



## create_programming_languages

> models::CreateDarIntegration201Response create_programming_languages(create_programming_languages_request)
ProgrammingLanguage@store

Creates a new system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_programming_languages_request** | [**CreateProgrammingLanguagesRequest**](CreateProgrammingLanguagesRequest.md) | Programming language definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_programming_languages

> models::DeleteApplications200Response delete_programming_languages(id)
ProgrammingLanguage@destroy

Delete a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_programming_languages

> models::UpdateProgrammingLanguages200Response edit_programming_languages(id, edit_programming_languages_request)
ProgrammingLanguage@update

Edit a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |
**edit_programming_languages_request** | [**EditProgrammingLanguagesRequest**](EditProgrammingLanguagesRequest.md) | ProgrammingLanguage definition | [required] |

### Return type

[**models::UpdateProgrammingLanguages200Response**](update_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_programming_languages

> models::UpdateProgrammingLanguages200Response update_programming_languages(id, update_programming_languages_request)
ProgrammingLanguage@update

Update a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |
**update_programming_languages_request** | [**UpdateProgrammingLanguagesRequest**](UpdateProgrammingLanguagesRequest.md) | ProgrammingLanguage definition | [required] |

### Return type

[**models::UpdateProgrammingLanguages200Response**](update_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


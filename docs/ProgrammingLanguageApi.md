# \ProgrammingLanguageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_languages**](ProgrammingLanguageApi.md#create_programming_languages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
[**delete_programming_languages**](ProgrammingLanguageApi.md#delete_programming_languages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
[**edit_programming_languages**](ProgrammingLanguageApi.md#edit_programming_languages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
[**fetch_all_programming_languages**](ProgrammingLanguageApi.md#fetch_all_programming_languages) | **GET** /api/v1/programming_languages | ProgrammingLanguage@index
[**fetch_programming_languages**](ProgrammingLanguageApi.md#fetch_programming_languages) | **GET** /api/v1/programming_languages/{id} | ProgrammingLanguage@show
[**update_programming_languages**](ProgrammingLanguageApi.md#update_programming_languages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update



## create_programming_languages

> models::CreateCategories200Response create_programming_languages(create_categories_request)
ProgrammingLanguage@store

Creates a new system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md) | Programming language definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_programming_languages

> models::DeleteAliases200Response delete_programming_languages(id)
ProgrammingLanguage@destroy

Delete a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_programming_languages

> models::UpdateProgrammingLanguages200Response edit_programming_languages(id, edit_categories_request)
ProgrammingLanguage@update

Edit a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |
**edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md) | ProgrammingLanguage definition | [required] |

### Return type

[**models::UpdateProgrammingLanguages200Response**](update_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_programming_languages

> models::FetchAllProgrammingLanguages200Response fetch_all_programming_languages()
ProgrammingLanguage@index

Returns a list of programming languages enabled on the system

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllProgrammingLanguages200Response**](fetch_all_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_programming_languages

> models::FetchProgrammingLanguages200Response fetch_programming_languages(id)
ProgrammingLanguage@show

Return a single system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |

### Return type

[**models::FetchProgrammingLanguages200Response**](fetch_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_programming_languages

> models::UpdateProgrammingLanguages200Response update_programming_languages(id, update_categories_request)
ProgrammingLanguage@update

Update a system programming language

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming language id | [required] |
**update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md) | ProgrammingLanguage definition | [required] |

### Return type

[**models::UpdateProgrammingLanguages200Response**](update_programming_languages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


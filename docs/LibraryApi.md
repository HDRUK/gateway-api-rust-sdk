# \LibraryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_libraries**](LibraryApi.md#create_libraries) | **POST** /api/v1/libraries | Library@store
[**delete_libraries**](LibraryApi.md#delete_libraries) | **DELETE** /api/v1/libraries/{id} | Library@destroy
[**edit_libraries**](LibraryApi.md#edit_libraries) | **PATCH** /api/v1/libraries/{id} | Library@update
[**fetch_libraries**](LibraryApi.md#fetch_libraries) | **GET** /api/v1/libraries/{id} | Return a single library
[**list_libraries**](LibraryApi.md#list_libraries) | **GET** /api/v1/libraries | Retrieve a list of libraries
[**update_libraries**](LibraryApi.md#update_libraries) | **PUT** /api/v1/libraries/{id} | Library@update



## create_libraries

> models::CreateCategories200Response create_libraries(create_libraries_request)
Library@store

Creates a new library

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md) | library definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_libraries

> models::DeleteAliases200Response delete_libraries(id)
Library@destroy

Delete a library

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | library id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_libraries

> models::UpdateLibraries200Response edit_libraries(id, create_libraries_request)
Library@update

Edit a library

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | library id | [required] |
**create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md) | library definition | [required] |

### Return type

[**models::UpdateLibraries200Response**](update_libraries_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_libraries

> models::FetchLibraries200Response fetch_libraries(id)
Return a single library

Return a single library

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | library id | [required] |

### Return type

[**models::FetchLibraries200Response**](fetch_libraries_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_libraries

> models::ListLibraries200Response list_libraries(per_page)
Retrieve a list of libraries

Returns a paginated list of libraries along with associated datasets and teams.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | Specify the number of libraries per page |  |[default to 10]

### Return type

[**models::ListLibraries200Response**](listLibraries_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_libraries

> models::UpdateLibraries200Response update_libraries(id, create_libraries_request)
Library@update

Update a library

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | library id | [required] |
**create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md) | library definition | [required] |

### Return type

[**models::UpdateLibraries200Response**](update_libraries_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


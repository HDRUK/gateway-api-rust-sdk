# \KeywordApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_keywords**](KeywordApi.md#create_keywords) | **POST** /api/v1/keywords | KeywordController@store
[**delete_keywords**](KeywordApi.md#delete_keywords) | **DELETE** /api/v1/keywords/{id} | KeywordController@destroy
[**edit_keywords**](KeywordApi.md#edit_keywords) | **PATCH** /api/v1/keywords/{id} | KeywordController@update
[**fetch_all_keywords**](KeywordApi.md#fetch_all_keywords) | **GET** /api/v1/keywords | KeywordController@index
[**fetch_keywords**](KeywordApi.md#fetch_keywords) | **GET** /api/v1/keywords/{id} | KeywordController@show
[**update_keywords**](KeywordApi.md#update_keywords) | **PUT** /api/v1/keywords/{id} | KeywordController@update



## create_keywords

> models::CreateCategories200Response create_keywords(create_categories_request)
KeywordController@store

Creates a new keyword

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md) | Keyword definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_keywords

> models::DeleteAliases200Response delete_keywords(id)
KeywordController@destroy

Delete a keyword by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | keyword id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_keywords

> models::UpdateKeywords200Response edit_keywords(id, edit_categories_request)
KeywordController@update

Edit a keyword by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | keyword id | [required] |
**edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md) | Category definition | [required] |

### Return type

[**models::UpdateKeywords200Response**](update_keywords_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_keywords

> models::FetchAllKeywords200Response fetch_all_keywords(per_page)
KeywordController@index

Returns a list of keywords

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | Alternative output schema version. |  |

### Return type

[**models::FetchAllKeywords200Response**](fetch_all_keywords_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_keywords

> models::FetchKeywords200Response fetch_keywords(id)
KeywordController@show

Return a single keyword

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | keyword id | [required] |

### Return type

[**models::FetchKeywords200Response**](fetch_keywords_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_keywords

> models::UpdateKeywords200Response update_keywords(id, update_categories_request)
KeywordController@update

Update a keyword by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | keyword id | [required] |
**update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md) | Keyword definition | [required] |

### Return type

[**models::UpdateKeywords200Response**](update_keywords_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


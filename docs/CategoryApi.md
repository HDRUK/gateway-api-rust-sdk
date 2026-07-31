# \CategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_categories**](CategoryApi.md#create_categories) | **POST** /api/v1/categories | Category@store
[**delete_categories**](CategoryApi.md#delete_categories) | **DELETE** /api/v1/categories/{id} | Category@destroy
[**edit_categories**](CategoryApi.md#edit_categories) | **PATCH** /api/v1/categories/{id} | Category@update
[**fetch_all_categories**](CategoryApi.md#fetch_all_categories) | **GET** /api/v1/categories | Category@index
[**fetch_categories**](CategoryApi.md#fetch_categories) | **GET** /api/v1/categories/{id} | Category@show
[**update_categories**](CategoryApi.md#update_categories) | **PUT** /api/v1/categories/{id} | Category@update



## create_categories

> models::CreateCategories200Response create_categories(create_categories_request)
Category@store

Creates a new tool category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md) | Category definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_categories

> models::DeleteAliases200Response delete_categories(id)
Category@destroy

Delete a tool category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | category id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_categories

> models::UpdateCategories200Response edit_categories(id, edit_categories_request)
Category@update

Edit a tool category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | category id | [required] |
**edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md) | Category definition | [required] |

### Return type

[**models::UpdateCategories200Response**](update_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_categories

> models::FetchAllCategories200Response fetch_all_categories(per_page)
Category@index

Returns a list of categories enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllCategories200Response**](fetch_all_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_categories

> models::FetchAllCategories200Response fetch_categories(id)
Category@show

Return a single tool category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | category id | [required] |

### Return type

[**models::FetchAllCategories200Response**](fetch_all_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_categories

> models::UpdateCategories200Response update_categories(id, update_categories_request)
Category@update

Update a tool category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | category id | [required] |
**update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md) | Category definition | [required] |

### Return type

[**models::UpdateCategories200Response**](update_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


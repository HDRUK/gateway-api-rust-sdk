# \TypeCategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_type_categories**](TypeCategoryApi.md#create_type_categories) | **POST** /api/v1/type_categories | TypeCategory@store
[**delete_type_categories**](TypeCategoryApi.md#delete_type_categories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy
[**edit_type_categories**](TypeCategoryApi.md#edit_type_categories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update
[**fetch_all_type_categories**](TypeCategoryApi.md#fetch_all_type_categories) | **GET** /api/v1/type_categories | TypeCategory@index
[**fetch_type_categories**](TypeCategoryApi.md#fetch_type_categories) | **GET** /api/v1/type_categories/{id} | TypeCategory@show
[**update_type_categories**](TypeCategoryApi.md#update_type_categories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update



## create_type_categories

> models::CreateCategories200Response create_type_categories(create_type_categories_request)
TypeCategory@store

Creates a new system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_type_categories_request** | [**CreateTypeCategoriesRequest**](CreateTypeCategoriesRequest.md) | Programming language definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_type_categories

> models::DeleteAliases200Response delete_type_categories(id)
TypeCategory@destroy

Delete a system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_type_categories

> models::UpdateTypeCategories200Response edit_type_categories(id, edit_categories_request)
TypeCategory@update

Edit a system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |
**edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md) | TypeCategory definition | [required] |

### Return type

[**models::UpdateTypeCategories200Response**](update_type_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_type_categories

> models::FetchAllTypeCategories200Response fetch_all_type_categories()
TypeCategory@index

Returns a list of type categories enabled on the system

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllTypeCategories200Response**](fetch_all_type_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_type_categories

> models::FetchTypeCategories200Response fetch_type_categories(id)
TypeCategory@show

Return a single system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |

### Return type

[**models::FetchTypeCategories200Response**](fetch_type_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_type_categories

> models::UpdateTypeCategories200Response update_type_categories(id, update_type_categories_request)
TypeCategory@update

Update a system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |
**update_type_categories_request** | [**UpdateTypeCategoriesRequest**](UpdateTypeCategoriesRequest.md) | TypeCategory definition | [required] |

### Return type

[**models::UpdateTypeCategories200Response**](update_type_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


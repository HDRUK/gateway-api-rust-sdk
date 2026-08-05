# \TypeCategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_type_categories**](TypeCategoryApi.md#create_type_categories) | **POST** /api/v1/type_categories | TypeCategory@store
[**delete_type_categories**](TypeCategoryApi.md#delete_type_categories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy
[**edit_type_categories**](TypeCategoryApi.md#edit_type_categories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update
[**update_type_categories**](TypeCategoryApi.md#update_type_categories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update



## create_type_categories

> models::CreateDarIntegration201Response create_type_categories(create_type_categories_request)
TypeCategory@store

Creates a new system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_type_categories_request** | [**CreateTypeCategoriesRequest**](CreateTypeCategoriesRequest.md) | Programming language definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_type_categories

> models::DeleteApplications200Response delete_type_categories(id)
TypeCategory@destroy

Delete a system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_type_categories

> models::UpdateTypeCategories200Response edit_type_categories(id, edit_programming_languages_request)
TypeCategory@update

Edit a system type category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | type category id | [required] |
**edit_programming_languages_request** | [**EditProgrammingLanguagesRequest**](EditProgrammingLanguagesRequest.md) | TypeCategory definition | [required] |

### Return type

[**models::UpdateTypeCategories200Response**](update_type_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
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


# \ProgrammingPackageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_packages**](ProgrammingPackageApi.md#create_programming_packages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store
[**delete_programming_packages**](ProgrammingPackageApi.md#delete_programming_packages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy
[**edit_programming_packages**](ProgrammingPackageApi.md#edit_programming_packages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update
[**fetch_all_programming_packages**](ProgrammingPackageApi.md#fetch_all_programming_packages) | **GET** /api/v1/programming_packages | ProgrammingPackage@index
[**fetch_programming_packages**](ProgrammingPackageApi.md#fetch_programming_packages) | **GET** /api/v1/programming_packages/{id} | ProgrammingPackage@show
[**update_programming_packages**](ProgrammingPackageApi.md#update_programming_packages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update



## create_programming_packages

> models::CreateCategories200Response create_programming_packages(create_categories_request)
ProgrammingPackage@store

Creates a new system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md) | Programming package definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_programming_packages

> models::DeleteAliases200Response delete_programming_packages(id)
ProgrammingPackage@destroy

Delete a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_programming_packages

> models::UpdateProgrammingPackages200Response edit_programming_packages(id, edit_categories_request)
ProgrammingPackage@update

Edit a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |
**edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md) | ProgrammingPackage definition | [required] |

### Return type

[**models::UpdateProgrammingPackages200Response**](update_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_programming_packages

> models::FetchAllProgrammingPackages200Response fetch_all_programming_packages()
ProgrammingPackage@index

Returns a list of programming packages enabled on the system

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllProgrammingPackages200Response**](fetch_all_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_programming_packages

> models::FetchProgrammingPackages200Response fetch_programming_packages(id)
ProgrammingPackage@show

Return a single system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |

### Return type

[**models::FetchProgrammingPackages200Response**](fetch_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_programming_packages

> models::UpdateProgrammingPackages200Response update_programming_packages(id, update_categories_request)
ProgrammingPackage@update

Update a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |
**update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md) | ProgrammingPackage definition | [required] |

### Return type

[**models::UpdateProgrammingPackages200Response**](update_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


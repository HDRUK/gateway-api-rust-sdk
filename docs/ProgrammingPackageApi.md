# \ProgrammingPackageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_packages**](ProgrammingPackageApi.md#create_programming_packages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store
[**delete_programming_packages**](ProgrammingPackageApi.md#delete_programming_packages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy
[**edit_programming_packages**](ProgrammingPackageApi.md#edit_programming_packages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update
[**update_programming_packages**](ProgrammingPackageApi.md#update_programming_packages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update



## create_programming_packages

> models::CreateDarIntegration201Response create_programming_packages(create_programming_languages_request)
ProgrammingPackage@store

Creates a new system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_programming_languages_request** | [**CreateProgrammingLanguagesRequest**](CreateProgrammingLanguagesRequest.md) | Programming package definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_programming_packages

> models::DeleteApplications200Response delete_programming_packages(id)
ProgrammingPackage@destroy

Delete a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_programming_packages

> models::UpdateProgrammingPackages200Response edit_programming_packages(id, edit_programming_languages_request)
ProgrammingPackage@update

Edit a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |
**edit_programming_languages_request** | [**EditProgrammingLanguagesRequest**](EditProgrammingLanguagesRequest.md) | ProgrammingPackage definition | [required] |

### Return type

[**models::UpdateProgrammingPackages200Response**](update_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_programming_packages

> models::UpdateProgrammingPackages200Response update_programming_packages(id, update_programming_languages_request)
ProgrammingPackage@update

Update a system programming package

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | programming package id | [required] |
**update_programming_languages_request** | [**UpdateProgrammingLanguagesRequest**](UpdateProgrammingLanguagesRequest.md) | ProgrammingPackage definition | [required] |

### Return type

[**models::UpdateProgrammingPackages200Response**](update_programming_packages_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


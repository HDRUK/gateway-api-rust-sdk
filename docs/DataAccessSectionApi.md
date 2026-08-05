# \DataAccessSectionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_section**](DataAccessSectionApi.md#create_dar_section) | **POST** /api/v1/dar/sections | DataAccessSection@store
[**delete_dar_section**](DataAccessSectionApi.md#delete_dar_section) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy
[**patch_dar_section**](DataAccessSectionApi.md#patch_dar_section) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update
[**update_dar_section**](DataAccessSectionApi.md#update_dar_section) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update



## create_dar_section

> models::CreateDarIntegration201Response create_dar_section(create_dar_section_request)
DataAccessSection@store

Creates a new DAR section

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_dar_section_request** | [**CreateDarSectionRequest**](CreateDarSectionRequest.md) | DataAccessSection definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_section

> models::DeleteApplications200Response delete_dar_section(id)
DataAccessSection@destroy

Delete a system DAR section

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR section id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_dar_section

> models::UpdateDarSection200Response patch_dar_section(id, patch_dar_section_request)
DataAccessSection@update

Edit a system DAR section

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR section id | [required] |
**patch_dar_section_request** | [**PatchDarSectionRequest**](PatchDarSectionRequest.md) | DataAccessSection definition | [required] |

### Return type

[**models::UpdateDarSection200Response**](update_dar_section_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dar_section

> models::UpdateDarSection200Response update_dar_section(id, create_dar_section_request)
DataAccessSection@update

Update a system DAR section

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR section id | [required] |
**create_dar_section_request** | [**CreateDarSectionRequest**](CreateDarSectionRequest.md) | DataAccessSection definition | [required] |

### Return type

[**models::UpdateDarSection200Response**](update_dar_section_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


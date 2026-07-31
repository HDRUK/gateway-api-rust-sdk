# \DataAccessTemplateApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_template**](DataAccessTemplateApi.md#create_dar_template) | **POST** /api/v1/dar/templates | DataAccessTemplate@store
[**delete_dar_template**](DataAccessTemplateApi.md#delete_dar_template) | **DELETE** /api/v1/dar/templates/{id} | DataAccessTemplate@destroy
[**download_dar_template_file**](DataAccessTemplateApi.md#download_dar_template_file) | **GET** /api/v1/dar/templates/{id}/download | DataAccessTemplate@downloadFile
[**fetch_dar_template**](DataAccessTemplateApi.md#fetch_dar_template) | **GET** /api/v1/dar/templates/{id} | DataAccessTemplate@show
[**fetch_dar_templates**](DataAccessTemplateApi.md#fetch_dar_templates) | **GET** /api/v1/dar/templates | DataAccessTemplate@index
[**patch_dar_template**](DataAccessTemplateApi.md#patch_dar_template) | **PATCH** /api/v1/dar/templates/{id} | DataAccessTemplate@update
[**update_dar_template**](DataAccessTemplateApi.md#update_dar_template) | **PUT** /api/v1/dar/templates/{id} | DataAccessTemplate@update



## create_dar_template

> models::CreateCategories200Response create_dar_template(create_dar_template_request)
DataAccessTemplate@store

Creates a new DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_dar_template_request** | [**CreateDarTemplateRequest**](CreateDarTemplateRequest.md) | DataAccessTemplate definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_template

> models::DeleteAliases200Response delete_dar_template(id)
DataAccessTemplate@destroy

Delete a system DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR template id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## download_dar_template_file

> download_dar_template_file(id)
DataAccessTemplate@downloadFile

Download the template for a file based DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR template id | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_template

> models::FetchDarTemplate200Response fetch_dar_template(id)
DataAccessTemplate@show

Return a single DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR template id | [required] |

### Return type

[**models::FetchDarTemplate200Response**](fetch_dar_template_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_templates

> models::FetchDarTemplates200Response fetch_dar_templates(with_questions, published)
DataAccessTemplate@index

List of DAR templates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**with_questions** | Option<**i32**> | Include questions in response |  |
**published** | Option<**String**> | Template publication status to filter by (true, false) |  |

### Return type

[**models::FetchDarTemplates200Response**](fetch_dar_templates_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_dar_template

> models::PatchDarTemplate200Response patch_dar_template(id, patch_dar_template_request, section_id)
DataAccessTemplate@update

Edit a system DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR template id | [required] |
**patch_dar_template_request** | [**PatchDarTemplateRequest**](PatchDarTemplateRequest.md) | DataAccessTemplate definition | [required] |
**section_id** | Option<**i32**> | Section id |  |

### Return type

[**models::PatchDarTemplate200Response**](patch_dar_template_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dar_template

> models::FetchDarTemplate200Response update_dar_template(id, update_dar_template_request)
DataAccessTemplate@update

Update a system DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DAR template id | [required] |
**update_dar_template_request** | [**UpdateDarTemplateRequest**](UpdateDarTemplateRequest.md) | DataAccessTemplate definition | [required] |

### Return type

[**models::FetchDarTemplate200Response**](fetch_dar_template_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


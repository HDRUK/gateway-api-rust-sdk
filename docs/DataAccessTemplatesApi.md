# \DataAccessTemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dar_template_count_unique_fields**](DataAccessTemplatesApi.md#dar_template_count_unique_fields) | **GET** /api/v1/dar/templates/count/{field} | DataAccessTemplateController@count



## dar_template_count_unique_fields

> models::CountUniqueFieldsCollections200Response dar_template_count_unique_fields(field)
DataAccessTemplateController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \SearchDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_datasets**](SearchDatasetsApi.md#search_datasets) | **POST** /api/v1/search/datasets | Search@datasets



## search_datasets

> models::SearchDatasets200Response search_datasets(search_datasets_request)
Search@datasets

Returns gateway datasets related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_datasets_request** | [**SearchDatasetsRequest**](SearchDatasetsRequest.md) | Submit search query | [required] |

### Return type

[**models::SearchDatasets200Response**](search_datasets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


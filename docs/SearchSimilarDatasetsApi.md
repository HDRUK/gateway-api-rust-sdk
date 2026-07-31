# \SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_similar_datasets**](SearchSimilarDatasetsApi.md#search_similar_datasets) | **POST** /api/v1/search/similar/datasets | Search@similarDatasets



## search_similar_datasets

> models::SearchSimilarDatasets200Response search_similar_datasets(search_similar_datasets_request)
Search@similarDatasets

Returns top three gateway datasets most similar to the provided dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_similar_datasets_request** | [**SearchSimilarDatasetsRequest**](SearchSimilarDatasetsRequest.md) | Submit dataset id | [required] |

### Return type

[**models::SearchSimilarDatasets200Response**](search_similar_datasets_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


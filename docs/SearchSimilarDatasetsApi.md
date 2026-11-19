# \SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_similar_datasets**](SearchSimilarDatasetsApi.md#search_similar_datasets) | **POST** /api/v1/search/similar/datasets | Search for similar datasets (deprecated)
[**search_similar_datasets_v2**](SearchSimilarDatasetsApi.md#search_similar_datasets_v2) | **POST** /api/v2/search/similar/datasets | Search for similar datasets



## search_similar_datasets

> search_similar_datasets(search_similar_datasets_v2_request)
Search for similar datasets (deprecated)

Deprecated: use /api/v2/search/similar/datasets, which this endpoint now serves. Responses carry Deprecation, Sunset and Link headers; it stops working after the Sunset date (17 May 2027).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_similar_datasets_v2_request** | [**SearchSimilarDatasetsV2Request**](SearchSimilarDatasetsV2Request.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_similar_datasets_v2

> models::SearchSimilarDatasetsV2200Response search_similar_datasets_v2(search_similar_datasets_v2_request)
Search for similar datasets

Returns up to three gateway datasets sharing the most terms with the provided dataset's keywords and title. The provided dataset is never included.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_similar_datasets_v2_request** | [**SearchSimilarDatasetsV2Request**](SearchSimilarDatasetsV2Request.md) |  | [required] |

### Return type

[**models::SearchSimilarDatasetsV2200Response**](search_similar_datasets_v2_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


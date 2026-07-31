# \SearchDataUsesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_data_uses**](SearchDataUsesApi.md#search_data_uses) | **POST** /api/v1/search/dur | Search@data_uses



## search_data_uses

> models::SearchDataUses200Response search_data_uses(search_data_uses_request, sort, direction, download)
Search@data_uses

Returns gateway data uses related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_data_uses_request** | [**SearchDataUsesRequest**](SearchDataUsesRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |
**download** | Option<**bool**> | Download a csv of the results (default: false) |  |

### Return type

[**models::SearchDataUses200Response**](search_data_uses_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


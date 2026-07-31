# \SearchDataCustodiansApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_data_custodians**](SearchDataCustodiansApi.md#search_data_custodians) | **POST** /api/v1/search/data_custodians | Search@data_custodians



## search_data_custodians

> models::SearchDataCustodians200Response search_data_custodians(search_data_custodians_request, sort, direction, per_page)
Search@data_custodians

Returns gateway data custodians related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_data_custodians_request** | [**SearchDataCustodiansRequest**](SearchDataCustodiansRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |
**per_page** | Option<**i32**> | Number of results to return per page |  |

### Return type

[**models::SearchDataCustodians200Response**](search_data_custodians_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


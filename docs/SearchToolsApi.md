# \SearchToolsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_tools**](SearchToolsApi.md#search_tools) | **POST** /api/v1/search/tools | Search@tools



## search_tools

> models::SearchTools200Response search_tools(search_tools_request, sort, direction)
Search@tools

Returns gateway tools related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_tools_request** | [**SearchToolsRequest**](SearchToolsRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |

### Return type

[**models::SearchTools200Response**](search_tools_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \SearchCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_collections**](SearchCollectionsApi.md#search_collections) | **POST** /api/v1/search/collections | Search@collections



## search_collections

> models::SearchCollections200Response search_collections(search_collections_request, sort, direction)
Search@collections

Returns gateway collections related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_collections_request** | [**SearchCollectionsRequest**](SearchCollectionsRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |

### Return type

[**models::SearchCollections200Response**](search_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


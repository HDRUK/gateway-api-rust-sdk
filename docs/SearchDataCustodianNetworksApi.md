# \SearchDataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_data_custodian_networks**](SearchDataCustodianNetworksApi.md#search_data_custodian_networks) | **POST** /api/v1/search/data_custodian_networks | Search@data_custodian_networks



## search_data_custodian_networks

> models::SearchDataCustodianNetworks200Response search_data_custodian_networks(search_data_custodian_networks_request, sort, direction)
Search@data_custodian_networks

Returns gateway data custodian networks related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_data_custodian_networks_request** | [**SearchDataCustodianNetworksRequest**](SearchDataCustodianNetworksRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |

### Return type

[**models::SearchDataCustodianNetworks200Response**](search_data_custodian_networks_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


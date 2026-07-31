# \CancerTypeFilterApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cancer_type_filter**](CancerTypeFilterApi.md#get_cancer_type_filter) | **GET** /api/v1/cancer-type-filters/{filter_id} | Get a single cancer type filter
[**get_cancer_type_filters**](CancerTypeFilterApi.md#get_cancer_type_filters) | **GET** /api/v1/cancer-type-filters | Get all cancer type filters



## get_cancer_type_filter

> models::GetCancerTypeFilter200Response get_cancer_type_filter(filter_id)
Get a single cancer type filter

Returns a single cancer type filter with its children by filter_id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**filter_id** | **String** | Filter ID (e.g., 0_0, 0_0_2_59) | [required] |

### Return type

[**models::GetCancerTypeFilter200Response**](getCancerTypeFilter_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cancer_type_filters

> models::GetCancerTypeFilters200Response get_cancer_type_filters(parent_id, level)
Get all cancer type filters

Returns a hierarchical tree of cancer type filters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**parent_id** | Option<**i32**> | Filter by parent ID |  |
**level** | Option<**i32**> | Filter by hierarchy level |  |

### Return type

[**models::GetCancerTypeFilters200Response**](getCancerTypeFilters_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


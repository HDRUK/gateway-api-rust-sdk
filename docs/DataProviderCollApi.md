# \DataProviderCollApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_data_provider_coll**](DataProviderCollApi.md#fetch_data_provider_coll) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show
[**fetch_data_provider_coll_summary**](DataProviderCollApi.md#fetch_data_provider_coll_summary) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary
[**fetch_data_provider_colls**](DataProviderCollApi.md#fetch_data_provider_colls) | **GET** /api/v1/data_provider_colls | DataProviderColl@index



## fetch_data_provider_coll

> models::FetchDataProviderColl200Response fetch_data_provider_coll(id)
DataProviderColl@show

Return a single DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID | [required] |

### Return type

[**models::FetchDataProviderColl200Response**](fetch_data_provider_coll_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_provider_coll_summary

> models::FetchDataProviderCollSummary200Response fetch_data_provider_coll_summary(id)
DataProviderColl@showSummary

Return a single DataProviderColl - summary

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID - summary | [required] |

### Return type

[**models::FetchDataProviderCollSummary200Response**](fetch_data_provider_coll_summary_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_provider_colls

> models::FetchDataProviderColls200Response fetch_data_provider_colls(per_page)
DataProviderColl@index

Returns a list of DataProviderColls enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchDataProviderColls200Response**](fetch_data_provider_colls_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


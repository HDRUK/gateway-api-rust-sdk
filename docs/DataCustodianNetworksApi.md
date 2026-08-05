# \DataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_data_custodian_network**](DataCustodianNetworksApi.md#fetch_data_custodian_network) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show
[**fetch_data_custodian_network_custodians_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_custodians_summary) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary
[**fetch_data_custodian_network_datasets_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_datasets_summary) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary
[**fetch_data_custodian_network_entities_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_entities_summary) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary
[**fetch_data_custodian_network_info**](DataCustodianNetworksApi.md#fetch_data_custodian_network_info) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary
[**fetch_data_custodian_networks**](DataCustodianNetworksApi.md#fetch_data_custodian_networks) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index



## fetch_data_custodian_network

> models::FetchDataCustodianNetwork200Response fetch_data_custodian_network(id)
DataCustodianNetworks@show

Return a single DataCustodianNetwork

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataCustodianNetwork ID | [required] |

### Return type

[**models::FetchDataCustodianNetwork200Response**](fetch_data_custodian_network_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodian_network_custodians_summary

> models::FetchDataCustodianNetworkCustodiansSummary200Response fetch_data_custodian_network_custodians_summary(id)
DataCustodianNetworks@showCustodiansSummary

Return a single DataCustodianNetwork - custodians summary

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataCustodianNetwork ID - summary | [required] |

### Return type

[**models::FetchDataCustodianNetworkCustodiansSummary200Response**](fetch_data_custodian_network_custodians_summary_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodian_network_datasets_summary

> models::FetchDataCustodianNetworkDatasetsSummary200Response fetch_data_custodian_network_datasets_summary(id)
DataCustodianNetworks@showDatasetsSummary

Return a single DataCustodianNetwork - summary of datasets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataCustodianNetwork ID - summary | [required] |

### Return type

[**models::FetchDataCustodianNetworkDatasetsSummary200Response**](fetch_data_custodian_network_datasets_summary_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodian_network_entities_summary

> models::FetchDataCustodianNetworkEntitiesSummary200Response fetch_data_custodian_network_entities_summary(id)
DataCustodianNetworks@showSummary

Return a single DataCustodianNetwork - summary of entities

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataCustodianNetwork ID - summary | [required] |

### Return type

[**models::FetchDataCustodianNetworkEntitiesSummary200Response**](fetch_data_custodian_network_entities_summary_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodian_network_info

> models::FetchDataCustodianNetworkInfo200Response fetch_data_custodian_network_info(id)
DataCustodianNetworks@showInfoSummary

Return a single DataCustodianNetwork - basic information

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataCustodianNetwork ID - summary | [required] |

### Return type

[**models::FetchDataCustodianNetworkInfo200Response**](fetch_data_custodian_network_info_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodian_networks

> models::FetchDataCustodianNetworks200Response fetch_data_custodian_networks(per_page)
DataCustodianNetworks@index

Returns a list of DataCustodianNetworks enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchDataCustodianNetworks200Response**](fetch_data_custodian_networks_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


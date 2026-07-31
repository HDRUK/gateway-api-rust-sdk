# \AdminSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_admin_search_reindex**](AdminSearchApi.md#create_admin_search_reindex) | **POST** /api/v1/admin/search/reindex | Queue a drop+recreate+import of a search entity's Typesense collection
[**fetch_admin_search_status**](AdminSearchApi.md#fetch_admin_search_status) | **GET** /api/v1/admin/search/status | Get Typesense collection status for every onboarded search entity
[**update_admin_search_feature**](AdminSearchApi.md#update_admin_search_feature) | **POST** /api/v1/admin/search/feature | Activate or deactivate a search-related Pennant feature flag



## create_admin_search_reindex

> create_admin_search_reindex(create_admin_search_reindex_request)
Queue a drop+recreate+import of a search entity's Typesense collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_admin_search_reindex_request** | [**CreateAdminSearchReindexRequest**](CreateAdminSearchReindexRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_admin_search_status

> fetch_admin_search_status()
Get Typesense collection status for every onboarded search entity

### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_admin_search_feature

> update_admin_search_feature(update_admin_search_feature_request)
Activate or deactivate a search-related Pennant feature flag

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_admin_search_feature_request** | [**UpdateAdminSearchFeatureRequest**](UpdateAdminSearchFeatureRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


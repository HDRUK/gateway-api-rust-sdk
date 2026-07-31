# \AdminDataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_admin_data_custodian_networks**](AdminDataCustodianNetworksApi.md#fetch_admin_data_custodian_networks) | **GET** /api/v2/admin/data_custodian_networks | DataCustodianNetworks@adminIndex



## fetch_admin_data_custodian_networks

> fetch_admin_data_custodian_networks(per_page)
DataCustodianNetworks@adminIndex

Superadmin-only listing used by the network management admin screen — unlike index(), this is not filtered to enabled=1, so disabled networks remain visible/manageable.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


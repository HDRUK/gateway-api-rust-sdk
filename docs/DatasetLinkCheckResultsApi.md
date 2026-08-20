# \DatasetLinkCheckResultsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_dataset_link_check_results_v2**](DatasetLinkCheckResultsApi.md#fetch_dataset_link_check_results_v2) | **GET** /api/v2/dataset_link_check_results | DatasetLinkCheckResultController@index



## fetch_dataset_link_check_results_v2

> models::FetchDatasetLinkCheckResultsV2200Response fetch_dataset_link_check_results_v2()
DatasetLinkCheckResultController@index

Get the confirmed dead links (HTTP 404, verified across multiple checks) found in active dataset metadata by the nightly link check

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchDatasetLinkCheckResultsV2200Response**](fetch_dataset_link_check_results_v2_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


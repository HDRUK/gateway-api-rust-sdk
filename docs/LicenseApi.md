# \LicenseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_all_licenses**](LicenseApi.md#fetch_all_licenses) | **GET** /api/v1/licenses | License@index
[**fetch_licenses**](LicenseApi.md#fetch_licenses) | **GET** /api/v1/licenses/{id} | License@show



## fetch_all_licenses

> models::FetchAllLicenses200Response fetch_all_licenses()
License@index

Returns a list of licenses available

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllLicenses200Response**](fetch_all_licenses_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_licenses

> models::FetchLicenses200Response fetch_licenses(id)
License@show

Return a single license

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | License ID | [required] |

### Return type

[**models::FetchLicenses200Response**](fetch_licenses_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


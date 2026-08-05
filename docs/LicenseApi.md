# \LicenseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_licenses**](LicenseApi.md#create_licenses) | **POST** /api/v1/licenses | License@store
[**delete_licenses**](LicenseApi.md#delete_licenses) | **DELETE** /api/v1/licenses/{id} | License@destroy
[**edit_licenses**](LicenseApi.md#edit_licenses) | **PATCH** /api/v1/licenses/{id} | License@edit
[**fetch_all_licenses**](LicenseApi.md#fetch_all_licenses) | **GET** /api/v1/licenses | License@index
[**fetch_licenses**](LicenseApi.md#fetch_licenses) | **GET** /api/v1/licenses/{id} | License@show
[**update_licenses**](LicenseApi.md#update_licenses) | **PUT** /api/v1/licenses/{id} | License@update



## create_licenses

> models::CreateDarIntegration201Response create_licenses(create_licenses_request)
License@store

Creates a new license

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md) | License definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_licenses

> models::DeleteApplications200Response delete_licenses(id)
License@destroy

Delete a License

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | License id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_licenses

> models::UpdateLicenses200Response edit_licenses(id, create_licenses_request)
License@edit

Edit a tool license

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | license id | [required] |
**create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md) | Category definition | [required] |

### Return type

[**models::UpdateLicenses200Response**](update_licenses_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


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


## update_licenses

> models::UpdateLicenses200Response update_licenses(id, create_licenses_request)
License@update

Update a tool license

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | license id | [required] |
**create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md) | Category definition | [required] |

### Return type

[**models::UpdateLicenses200Response**](update_licenses_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


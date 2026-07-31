# \ApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_applications**](ApplicationApi.md#create_applications) | **POST** /api/v1/applications | ApplicationController@store
[**delete_applications**](ApplicationApi.md#delete_applications) | **DELETE** /api/v1/applications/{id} | ApplicationController@delete
[**edit_applications**](ApplicationApi.md#edit_applications) | **PATCH** /api/v1/applications/{id} | ApplicationController@edit
[**fetch_all_applications**](ApplicationApi.md#fetch_all_applications) | **GET** /api/v1/applications | ApplicationController@index
[**fetch_all_sitemap**](ApplicationApi.md#fetch_all_sitemap) | **GET** /api/v1/sitemap | SiteMapController@index
[**fetch_applications**](ApplicationApi.md#fetch_applications) | **GET** /api/v1/applications/{id} | ApplicationController@show
[**patch_applications_client_id**](ApplicationApi.md#patch_applications_client_id) | **PATCH** /api/v1/applications/{id}/clientid | ApplicationController@generateClientIdById
[**update_applications**](ApplicationApi.md#update_applications) | **PUT** /api/v1/applications/{id} | ApplicationController@update



## create_applications

> models::CreateApplications200Response create_applications(create_applications_request)
ApplicationController@store

Creates application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_applications_request** | [**CreateApplicationsRequest**](CreateApplicationsRequest.md) | Application definition | [required] |

### Return type

[**models::CreateApplications200Response**](create_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_applications

> models::DeleteAliases200Response delete_applications(id)
ApplicationController@delete

Delete application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | application id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_applications

> models::UpdateApplications200Response edit_applications(id, edit_applications_request)
ApplicationController@edit

Edit application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | application id | [required] |
**edit_applications_request** | [**EditApplicationsRequest**](EditApplicationsRequest.md) | ActivityLog definition | [required] |

### Return type

[**models::UpdateApplications200Response**](update_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_applications

> models::FetchAllApplications200Response fetch_all_applications(team_id, text, status)
ApplicationController@index

Returns a list of applications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | Option<**i32**> | Filter Apps by the teamId |  |
**text** | Option<**String**> | Search term to filter by application name or description. |  |
**status** | Option<**String**> | Filter by application status is enabled or not (true or false). |  |

### Return type

[**models::FetchAllApplications200Response**](fetch_all_applications_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_sitemap

> models::FetchAllSitemap200Response fetch_all_sitemap()
SiteMapController@index

Returns a list of all ids and last updated date for Collections, Data Custodians, Data Custodian Networks, Durs, DataSets, Tools

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllSitemap200Response**](fetch_all_sitemap_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_applications

> models::FetchApplications200Response fetch_applications(id)
ApplicationController@show

Get application by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | application id | [required] |

### Return type

[**models::FetchApplications200Response**](fetch_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_applications_client_id

> models::UpdateApplications200Response patch_applications_client_id(id)
ApplicationController@generateClientIdById

Generate Client ID application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | application id | [required] |

### Return type

[**models::UpdateApplications200Response**](update_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_applications

> models::UpdateApplications200Response update_applications(id, update_applications_request)
ApplicationController@update

Update application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | application id | [required] |
**update_applications_request** | [**UpdateApplicationsRequest**](UpdateApplicationsRequest.md) | ActivityLog definition | [required] |

### Return type

[**models::UpdateApplications200Response**](update_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


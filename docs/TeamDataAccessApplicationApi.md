# \TeamDataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_team_dar_applications**](TeamDataAccessApplicationApi.md#count_team_dar_applications) | **GET** /api/v1/teams/{teamId}/dar/applications/count | TeamDataAccessApplicationController@allCounts
[**count_unique_fields_dar_applications**](TeamDataAccessApplicationApi.md#count_unique_fields_dar_applications) | **GET** /api/v1/teams/{teamId}/dar/applications/count/{field} | TeamDataAccessApplicationController@count
[**fetch_team_dar_application**](TeamDataAccessApplicationApi.md#fetch_team_dar_application) | **GET** /api/v1/teams/{teamId}/dar/applications/{id} | TeamDataAccessApplicationController@show
[**fetch_team_dar_application_header**](TeamDataAccessApplicationApi.md#fetch_team_dar_application_header) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/showHeader | TeamDataAccessApplicationController@showHeader
[**fetch_team_dar_applications**](TeamDataAccessApplicationApi.md#fetch_team_dar_applications) | **GET** /api/v1/teams/{teamId}/dar/applications | TeamDataAccessApplicationController@index



## count_team_dar_applications

> models::CountUniqueFieldsCollections200Response count_team_dar_applications(team_id)
TeamDataAccessApplicationController@allCounts

Get Counts for all status fields in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_unique_fields_dar_applications

> models::CountUniqueFieldsCollections200Response count_unique_fields_dar_applications(team_id, field)
TeamDataAccessApplicationController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application

> models::FetchTeamDarApplication200Response fetch_team_dar_application(team_id, id)
TeamDataAccessApplicationController@show

Return a single DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_header

> models::FetchTeamDarApplicationHeader200Response fetch_team_dar_application_header(team_id, id)
TeamDataAccessApplicationController@showHeader

Get header information about a specific DAR

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationHeader200Response**](fetch_team_dar_application_header_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_applications

> models::FetchTeamDarApplications200Response fetch_team_dar_applications(team_id)
TeamDataAccessApplicationController@index

List of dar applications belonging to a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |

### Return type

[**models::FetchTeamDarApplications200Response**](fetch_team_dar_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


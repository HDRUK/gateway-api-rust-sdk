# \ProjectGrantApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_project_grant**](ProjectGrantApi.md#create_project_grant) | **POST** /api/v1/project_grants | ProjectGrantController@store
[**fetch_all_project_grants**](ProjectGrantApi.md#fetch_all_project_grants) | **GET** /api/v1/project_grants | ProjectGrantController@index
[**fetch_project_grant**](ProjectGrantApi.md#fetch_project_grant) | **GET** /api/v1/project_grants/{id} | ProjectGrantController@show



## create_project_grant

> models::CreateProjectGrant201Response create_project_grant()
ProjectGrantController@store

Create a project grant (and initial version)

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::CreateProjectGrant201Response**](create_project_grant_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_project_grants

> models::FetchAllProjectGrants200Response fetch_all_project_grants(pid, version, project_grant_name, user_id, team_id, with_related)
ProjectGrantController@index

Get all project grants

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | Option<**String**> | Filter by dataset pid |  |
**version** | Option<**i32**> | Filter by dataset version number |  |
**project_grant_name** | Option<**String**> | Filter by project grant name |  |
**user_id** | Option<**i32**> | Filter by owning user id |  |
**team_id** | Option<**i32**> | Filter by owning team id |  |
**with_related** | Option<**bool**> |  |  |

### Return type

[**models::FetchAllProjectGrants200Response**](fetch_all_project_grants_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_project_grant

> models::CountUniqueFieldsCollections200Response fetch_project_grant(id, with_related)
ProjectGrantController@show

Get a single project grant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** |  | [required] |
**with_related** | Option<**bool**> |  |  |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


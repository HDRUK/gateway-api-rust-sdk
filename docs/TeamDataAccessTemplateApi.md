# \TeamDataAccessTemplateApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_team_dar_template_file**](TeamDataAccessTemplateApi.md#delete_team_dar_template_file) | **DELETE** /api/v1/teams/{teamId}/dar/templates/{id}/files/{fileId} | TeamDataAccessTemplateController@destroyFile
[**fetch_team_dar_templates**](TeamDataAccessTemplateApi.md#fetch_team_dar_templates) | **GET** /api/v1/teams/{teamId}/dar/templates | TeamDataAccessTemplateController@index
[**team_dar_template_count_unique_fields**](TeamDataAccessTemplateApi.md#team_dar_template_count_unique_fields) | **GET** /api/v1/teams/{teamId}/dar/templates/count/{field} | TeamDataAccessTemplateController@count



## delete_team_dar_template_file

> models::DeleteAliases200Response delete_team_dar_template_file(team_id, id, file_id)
TeamDataAccessTemplateController@destroyFile

Delete a file associated with a DAR template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR template id | [required] |
**file_id** | **String** | File id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_templates

> models::FetchDarTemplates200Response fetch_team_dar_templates(team_id, published)
TeamDataAccessTemplateController@index

List of dar templates belonging to a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**published** | Option<**String**> | Template publication status to filter by (true, false) |  |

### Return type

[**models::FetchDarTemplates200Response**](fetch_dar_templates_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## team_dar_template_count_unique_fields

> models::CountUniqueFieldsCollections200Response team_dar_template_count_unique_fields(team_id, field)
TeamDataAccessTemplateController@count

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


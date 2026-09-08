# \ToolsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_unique_fields_tools**](ToolsApi.md#count_unique_fields_tools) | **GET** /api/v1/tools/count/{field} | ToolController@count
[**create_tools**](ToolsApi.md#create_tools) | **POST** /api/v1/tools | ToolController@store
[**create_tools_by_team_v2**](ToolsApi.md#create_tools_by_team_v2) | **POST** /api/v2/teams/{teamId}/tools | ToolController@store
[**create_tools_integrations**](ToolsApi.md#create_tools_integrations) | **POST** /api/v1/integrations/tools | IntegrationToolController@store
[**delete_tools**](ToolsApi.md#delete_tools) | **DELETE** /api/v1/tools/{id} | ToolController@destroy
[**delete_tools_by_teamid_v2**](ToolsApi.md#delete_tools_by_teamid_v2) | **DELETE** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@destroy
[**delete_tools_integrations**](ToolsApi.md#delete_tools_integrations) | **DELETE** /api/v1/integrations/tools/{id} | IntegrationToolController@destroy
[**edit_tools**](ToolsApi.md#edit_tools) | **PATCH** /api/v1/tools/{id} | ToolController@edit
[**edit_tools_by_teamid_v2**](ToolsApi.md#edit_tools_by_teamid_v2) | **PATCH** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@edit
[**edit_tools_integrations**](ToolsApi.md#edit_tools_integrations) | **PATCH** /api/v1/integrations/tools/{id} | IntegrationToolController@edit
[**fetch_all_tools**](ToolsApi.md#fetch_all_tools) | **GET** /api/v1/tools | Fetch all tools
[**fetch_all_tools_integrations**](ToolsApi.md#fetch_all_tools_integrations) | **GET** /api/v1/integrations/tools | IntegrationToolController@index
[**fetch_all_tools_v2**](ToolsApi.md#fetch_all_tools_v2) | **GET** /api/v2/tools | ToolController@indexActive
[**fetch_tools**](ToolsApi.md#fetch_tools) | **GET** /api/v1/tools/{id} | ToolController@show
[**fetch_tools_integrations**](ToolsApi.md#fetch_tools_integrations) | **GET** /api/v1/integrations/tools/{id} | IntegrationToolController@show
[**fetch_tools_v2**](ToolsApi.md#fetch_tools_v2) | **GET** /api/v2/tools/{id} | ToolController@showActive
[**update_tools**](ToolsApi.md#update_tools) | **PUT** /api/v1/tools/{id} | ToolController@update
[**update_tools_by_teamid_v2**](ToolsApi.md#update_tools_by_teamid_v2) | **PUT** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@update
[**update_tools_integrations**](ToolsApi.md#update_tools_integrations) | **PUT** /api/v1/integrations/tools/{id} | IntegrationToolController@update



## count_unique_fields_tools

> models::CountUniqueFieldsCollections200Response count_unique_fields_tools(field, team_id)
ToolController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**field** | **String** | name of the field to perform a count on | [required] |
**team_id** | **i32** | team id | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tools

> models::CreateDarIntegration201Response create_tools(create_tools_request)
ToolController@store

Create a new tool

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_tools_request** | [**CreateToolsRequest**](CreateToolsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tools_by_team_v2

> models::CreateDarIntegration201Response create_tools_by_team_v2(team_id, create_tools_request)
ToolController@store

Create a new tool by team v2

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_tools_request** | [**CreateToolsRequest**](CreateToolsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tools_integrations

> models::CreateDarIntegration201Response create_tools_integrations(create_tools_integrations_request)
IntegrationToolController@store

Create a new tool

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_tools_integrations_request** | [**CreateToolsIntegrationsRequest**](CreateToolsIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tools

> models::DeleteFederation200Response delete_tools(id)
ToolController@destroy

Delete tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tools_by_teamid_v2

> models::DeleteFederation200Response delete_tools_by_teamid_v2(team_id, id)
TeamToolController@destroy

Delete tool by id and by team_id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | tool id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tools_integrations

> models::DeleteFederation200Response delete_tools_integrations(id)
IntegrationToolController@destroy

Delete tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_tools

> models::FetchToolsIntegrations200Response edit_tools(id, update_tools_request, unarchive)
ToolController@edit

Edit tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |
**update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md) | Pass user credentials | [required] |
**unarchive** | Option<**String**> | Unarchive a tool |  |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_tools_by_teamid_v2

> models::FetchToolsIntegrations200Response edit_tools_by_teamid_v2(team_id, id, update_tools_request)
TeamToolController@edit

Edit tool by id and by teamid

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | tool id | [required] |
**update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_tools_integrations

> models::FetchToolsIntegrations200Response edit_tools_integrations(id, update_tools_integrations_request)
IntegrationToolController@edit

Edit tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |
**update_tools_integrations_request** | [**UpdateToolsIntegrationsRequest**](UpdateToolsIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_tools

> models::FetchAllTools200Response fetch_all_tools(team_id, user_id, title, sort)
Fetch all tools

Get all tools with optional filters and sorting

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | Option<**i32**> | Filter tools by team ID |  |
**user_id** | Option<**i32**> | Filter tools by user ID |  |
**title** | Option<**String**> | Filter tools by title |  |
**sort** | Option<**String**> | Sort tools by a specific field and direction, e.g., 'name:asc' or 'created_at:desc' |  |

### Return type

[**models::FetchAllTools200Response**](fetch_all_tools_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_tools_integrations

> models::FetchAllToolsIntegrations200Response fetch_all_tools_integrations()
IntegrationToolController@index

Get All Tools

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllToolsIntegrations200Response**](fetch_all_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_tools_v2

> models::FetchAllTools200Response fetch_all_tools_v2(name, sort)
ToolController@indexActive

Get all tools with optional filters and sorting

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | Filter tools by name |  |
**sort** | Option<**String**> | Sort tools by a specific field and direction, e.g., 'name:asc' or 'created_at:desc' |  |

### Return type

[**models::FetchAllTools200Response**](fetch_all_tools_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_tools

> models::FetchToolsIntegrations200Response fetch_tools(id, view_type)
ToolController@show

Get tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |
**view_type** | Option<**String**> | Query flag to show full tool data or a trimmed version (defaults to full). |  |[default to full]

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_tools_integrations

> models::FetchToolsIntegrations200Response fetch_tools_integrations(id)
IntegrationToolController@show

Get tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_tools_v2

> models::FetchToolsIntegrations200Response fetch_tools_v2(id)
ToolController@showActive

Get tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tools

> models::FetchToolsIntegrations200Response update_tools(id, update_tools_request)
ToolController@update

Update tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |
**update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tools_by_teamid_v2

> models::FetchToolsIntegrations200Response update_tools_by_teamid_v2(team_id, id, update_tools_request)
TeamToolController@update

Update tools by team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | tool id | [required] |
**update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tools_integrations

> models::FetchToolsIntegrations200Response update_tools_integrations(id, update_tools_integrations_request)
IntegrationToolController@update

Update tool by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | tool id | [required] |
**update_tools_integrations_request** | [**UpdateToolsIntegrationsRequest**](UpdateToolsIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchToolsIntegrations200Response**](fetch_tools_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \DatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_unique_fields**](DatasetsApi.md#count_unique_fields) | **GET** /api/v1/datasets/count/{field} | DatasetController@count
[**create_datasets**](DatasetsApi.md#create_datasets) | **POST** /api/v1/datasets | DatasetController@store
[**create_datasets_v2**](DatasetsApi.md#create_datasets_v2) | **POST** /api/v2/datasets | DatasetController@store
[**create_team_datasets_v2**](DatasetsApi.md#create_team_datasets_v2) | **POST** /api/v2/teams/{teamId}/datasets | TeamDatasetController@store
[**delete_datasets**](DatasetsApi.md#delete_datasets) | **DELETE** /api/v1/datasets/{id} | DatasetController@destroy
[**delete_datasets_v2**](DatasetsApi.md#delete_datasets_v2) | **DELETE** /api/v2/datasets/{id} | Delete a dataset
[**delete_team_datasets_v2**](DatasetsApi.md#delete_team_datasets_v2) | **DELETE** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@destroy
[**export_dataset_metadata**](DatasetsApi.md#export_dataset_metadata) | **GET** /api/v1/datasets/export_metadata/{id} | DatasetController@exportMetadata
[**export_datasets**](DatasetsApi.md#export_datasets) | **GET** /api/v1/datasets/export | DatasetController@export
[**export_dur**](DatasetsApi.md#export_dur) | **GET** /api/v1/dur/export | DurController@export
[**export_mock_dataset**](DatasetsApi.md#export_mock_dataset) | **GET** /api/v1/datasets/export/mock | DatasetController@exportMock
[**export_mock_dataset_v2**](DatasetsApi.md#export_mock_dataset_v2) | **GET** /api/v2/datasets/export/mock | DatasetController@exportMock
[**fetch_all_datasets**](DatasetsApi.md#fetch_all_datasets) | **GET** /api/v1/datasets | DatasetController@index
[**fetch_all_datasets_v2**](DatasetsApi.md#fetch_all_datasets_v2) | **GET** /api/v2/datasets | DatasetController@index
[**fetch_datasets**](DatasetsApi.md#fetch_datasets) | **GET** /api/v1/datasets/{id} | DatasetController@show
[**fetch_datasets_v2**](DatasetsApi.md#fetch_datasets_v2) | **GET** /api/v2/datasets/{id} | DatasetController@showActive
[**patch_datasets**](DatasetsApi.md#patch_datasets) | **PATCH** /api/v1/datasets/{id} | DatasetController@edit
[**patch_datasets_v2**](DatasetsApi.md#patch_datasets_v2) | **PATCH** /api/v2/datasets/{id} | DatasetController@edit
[**patch_team_datasets_v2**](DatasetsApi.md#patch_team_datasets_v2) | **PATCH** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@edit
[**update_datasets**](DatasetsApi.md#update_datasets) | **PUT** /api/v1/datasets/{id} | DatasetController@update
[**update_datasets_v2**](DatasetsApi.md#update_datasets_v2) | **PUT** /api/v2/datasets/{id} | DatasetController@update
[**update_team_datasets_v2**](DatasetsApi.md#update_team_datasets_v2) | **PUT** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@update



## count_unique_fields

> models::CountUniqueFieldsCollections200Response count_unique_fields(field, team_id)
DatasetController@count

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


## create_datasets

> models::CreateDarIntegration201Response create_datasets(create_datasets_request)
DatasetController@store

Create a new dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_datasets_request** | [**CreateDatasetsRequest**](CreateDatasetsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_datasets_v2

> models::CreateDarIntegration201Response create_datasets_v2(create_datasets_v2_request)
DatasetController@store

Create a new dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_datasets_v2_request** | [**CreateDatasetsV2Request**](CreateDatasetsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_team_datasets_v2

> models::CreateDarIntegration201Response create_team_datasets_v2(team_id, create_team_datasets_v2_request)
TeamDatasetController@store

Create a new dataset for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_team_datasets_v2_request** | [**CreateTeamDatasetsV2Request**](CreateTeamDatasetsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_datasets

> models::DeleteApplications200Response delete_datasets(id)
DatasetController@destroy

Delete a dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_datasets_v2

> models::DeleteApplications200Response delete_datasets_v2(id)
Delete a dataset

Delete a dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_datasets_v2

> models::DeleteApplications200Response delete_team_datasets_v2(team_id, id)
TeamDatasetController@destroy

Delete a team's dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dataset id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_dataset_metadata

> String export_dataset_metadata(id, download_type)
DatasetController@exportMetadata

Export Structural Metadata CSV of a single dataset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**download_type** | **String** | download type | [required] |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_datasets

> String export_datasets(team_id, dataset_id)
DatasetController@export

Export CSV Of All Datasets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**dataset_id** | Option<**i32**> | dataset id |  |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_dur

> String export_dur(team_id, dur_id)
DurController@export

Export CSV Of All Dur's

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**dur_id** | Option<**i32**> | dur id |  |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_mock_dataset

> String export_mock_dataset(r#type)
DatasetController@exportMock

Export Mock

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**r#type** | **String** | type export | [required] |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_mock_dataset_v2

> String export_mock_dataset_v2(r#type)
DatasetController@exportMock

Export Mock

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**r#type** | **String** |  | [required] |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_datasets

> models::FetchAllDatasets200Response fetch_all_datasets(team_id, pid, sort, title, status)
DatasetController@index

Get All Datasets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**pid** | Option<**String**> | get based on a pid |  |
**sort** | Option<**String**> | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> |  |
**title** | Option<**String**> | Three or more characters to filter dataset titles by |  |
**status** | Option<**String**> | Dataset status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') |  |

### Return type

[**models::FetchAllDatasets200Response**](fetch_all_datasets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_datasets_v2

> models::FetchAllDatasets200Response fetch_all_datasets_v2(sort, title, status, with_metadata)
DatasetController@index

Returns a list of all datasets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sort** | Option<**String**> | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> |  |
**title** | Option<**String**> | Three or more characters to filter dataset titles by |  |
**status** | Option<**String**> | Dataset status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') |  |
**with_metadata** | Option<**String**> | Boolean whether to return dataset metadata |  |

### Return type

[**models::FetchAllDatasets200Response**](fetch_all_datasets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_datasets

> models::FetchDatasets200Response fetch_datasets(id, export, schema_model, schema_version)
DatasetController@show

Get dataset by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**export** | Option<**String**> | Alternative output schema model. |  |
**schema_model** | Option<**String**> | Alternative output schema model. |  |
**schema_version** | Option<**String**> | Alternative output schema version. |  |

### Return type

[**models::FetchDatasets200Response**](fetch_datasets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_datasets_v2

> models::FetchDatasets200Response fetch_datasets_v2(id, export, schema_model, schema_version)
DatasetController@showActive

Get publicly visible dataset by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**export** | Option<**String**> | Set to 'structuralMetadata' to download as CSV. |  |
**schema_model** | Option<**String**> | Alternative output schema model. |  |
**schema_version** | Option<**String**> | Alternative output schema version. |  |

### Return type

[**models::FetchDatasets200Response**](fetch_datasets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_datasets

> models::DeleteApplications200Response patch_datasets(id, unarchive)
DatasetController@edit

Patch dataset by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**unarchive** | Option<**String**> | Unarchive a dataset |  |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_datasets_v2

> models::DeleteApplications200Response patch_datasets_v2(id, patch_datasets_v2_request)
DatasetController@edit

Patch dataset by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md) |  | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_team_datasets_v2

> models::DeleteApplications200Response patch_team_datasets_v2(team_id, id, patch_datasets_v2_request)
TeamDatasetController@edit

Edit a dataset owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dataset id | [required] |
**patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_datasets

> models::CreateDarIntegration201Response update_datasets(id, update_datasets_request)
DatasetController@update

Update a dataset with a new dataset version

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**update_datasets_request** | [**UpdateDatasetsRequest**](UpdateDatasetsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_datasets_v2

> models::CreateDarIntegration201Response update_datasets_v2(id, update_datasets_request)
DatasetController@update

Update a dataset with a new dataset version

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dataset id | [required] |
**update_datasets_request** | [**UpdateDatasetsRequest**](UpdateDatasetsRequest.md) |  | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_team_datasets_v2

> models::CreateDarIntegration201Response update_team_datasets_v2(team_id, id, patch_datasets_v2_request)
TeamDatasetController@update

Update a team dataset with a new dataset version

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dataset id | [required] |
**patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


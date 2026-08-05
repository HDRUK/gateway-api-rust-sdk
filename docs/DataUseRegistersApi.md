# \DataUseRegistersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dur**](DataUseRegistersApi.md#create_dur) | **POST** /api/v1/dur | DurController@store
[**create_dur_by_team_v2**](DataUseRegistersApi.md#create_dur_by_team_v2) | **POST** /api/v2/teams/{teamId}/dur | TeamDurController@store
[**delete_dur**](DataUseRegistersApi.md#delete_dur) | **DELETE** /api/v1/dur/{id} | Delete a dur
[**delete_durs_v2_by_team_id**](DataUseRegistersApi.md#delete_durs_v2_by_team_id) | **DELETE** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@destroy
[**edit_dur**](DataUseRegistersApi.md#edit_dur) | **PATCH** /api/v1/dur/{id} | Edit a dur
[**edit_durs_v2_by_team_id**](DataUseRegistersApi.md#edit_durs_v2_by_team_id) | **PATCH** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@edit
[**export_dur_template**](DataUseRegistersApi.md#export_dur_template) | **GET** /api/v1/dur/template | DurController@exportTemplate
[**export_dur_template_v2**](DataUseRegistersApi.md#export_dur_template_v2) | **GET** /api/v2/dur/template | DurController@exportTemplate
[**export_dur_v2**](DataUseRegistersApi.md#export_dur_v2) | **GET** /api/v2/dur/export | DurController@export
[**fetch_all_dur**](DataUseRegistersApi.md#fetch_all_dur) | **GET** /api/v1/dur | DurController@index
[**fetch_all_dur_v2**](DataUseRegistersApi.md#fetch_all_dur_v2) | **GET** /api/v2/dur | DurController@indexActive
[**fetch_dur_by_id**](DataUseRegistersApi.md#fetch_dur_by_id) | **GET** /api/v1/dur/{id} | DurController@show
[**fetch_dur_by_id_v2**](DataUseRegistersApi.md#fetch_dur_by_id_v2) | **GET** /api/v2/dur/{id} | DurController@showActive
[**update_dur**](DataUseRegistersApi.md#update_dur) | **PUT** /api/v1/dur/{id} | Update a dur by id
[**update_dur_v2_by_team_id**](DataUseRegistersApi.md#update_dur_v2_by_team_id) | **PUT** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@update
[**upload_dur**](DataUseRegistersApi.md#upload_dur) | **POST** /api/v1/dur/upload | DurController@upload



## create_dur

> models::CreateDarIntegration201Response create_dur(create_dur_request)
DurController@store

Create a new dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_dur_by_team_v2

> models::CreateDarIntegration201Response create_dur_by_team_v2(team_id, create_dur_request)
TeamDurController@store

Create a new dur by team v2

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dur

> models::DeleteApplications200Response delete_dur(id)
Delete a dur

Delete a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_durs_v2_by_team_id

> models::DeleteApplications200Response delete_durs_v2_by_team_id(team_id, id)
TeamDurController@destroy

Delete a dur by team and id v2

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dur id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_dur

> models::UpdateDur200Response edit_dur(id, create_dur_request, unarchive)
Edit a dur

Edit a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |
**unarchive** | Option<**String**> | Unarchive a dur |  |

### Return type

[**models::UpdateDur200Response**](update_dur_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_durs_v2_by_team_id

> models::UpdateDur200Response edit_durs_v2_by_team_id(team_id, id, create_dur_request)
TeamDurController@edit

Edit a dur by team v2

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dur id | [required] |
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateDur200Response**](update_dur_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_dur_template

> serde_json::Value export_dur_template()
DurController@exportTemplate

Export Dur upload template

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_dur_template_v2

> serde_json::Value export_dur_template_v2()
DurController@exportTemplate

Export Dur upload template

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_dur_v2

> String export_dur_v2(id)
DurController@export

Export CSV of one or more DURs

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | Option<**i32**> | dur id |  |

### Return type

**String**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_dur

> models::FetchAllDur200Response fetch_all_dur(sort, project_title, per_page)
DurController@index

Returns a list of dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sort** | Option<[**models::ProjectTitleColonAscCommaUpdatedAtColonAsc**](Models__ProjectTitleColonAscCommaUpdatedAtColonAsc.md)> | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc |  |
**project_title** | Option<**String**> | Filter tools by project title |  |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllDur200Response**](fetch_all_dur_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_dur_v2

> models::FetchAllDurV2200Response fetch_all_dur_v2(sort, project_title, per_page, with_related)
DurController@indexActive

Returns a list of active dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sort** | Option<[**models::ProjectTitleColonAscCommaUpdatedAtColonAsc**](Models__ProjectTitleColonAscCommaUpdatedAtColonAsc.md)> | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc |  |
**project_title** | Option<**String**> | Filter tools by project title |  |
**per_page** | Option<**i32**> | per page |  |
**with_related** | Option<**bool**> | Show related entities |  |

### Return type

[**models::FetchAllDurV2200Response**](fetch_all_dur_v2_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dur_by_id

> models::FetchDurById200Response fetch_dur_by_id(id)
DurController@show

Get dur by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | data use register id | [required] |

### Return type

[**models::FetchDurById200Response**](fetch_dur_by_id_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dur_by_id_v2

> models::UpdateDur200Response fetch_dur_by_id_v2(id)
DurController@showActive

Get dur by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | data use register id | [required] |

### Return type

[**models::UpdateDur200Response**](update_dur_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dur

> models::UpdateDur200Response update_dur(id, create_dur_request)
Update a dur by id

Update a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateDur200Response**](update_dur_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dur_v2_by_team_id

> models::UpdateDur200Response update_dur_v2_by_team_id(team_id, id, create_dur_request)
TeamDurController@update

Update a dur by team and id v2

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | dur id | [required] |
**create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateDur200Response**](update_dur_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upload_dur

> models::CreateDarIntegration201Response upload_dur(upload_dur_request)
DurController@upload

Create a new dur with upload data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**upload_dur_request** | [**UploadDurRequest**](UploadDurRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


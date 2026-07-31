# \IntegrationDataUseRegistersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dur_integrations**](IntegrationDataUseRegistersApi.md#create_dur_integrations) | **POST** /api/v1/integrations/dur | IntegrationDurController@store
[**delete_dur_integrations**](IntegrationDataUseRegistersApi.md#delete_dur_integrations) | **DELETE** /api/v1/integrations/dur/{id} | Delete a dur
[**edit_dur_integrations**](IntegrationDataUseRegistersApi.md#edit_dur_integrations) | **PATCH** /api/v1/integrations/dur/{id} | Edit a dur
[**fetch_all_dur_integrations**](IntegrationDataUseRegistersApi.md#fetch_all_dur_integrations) | **GET** /api/v1/integrations/dur | IntegrationDurController@index
[**fetch_dur_by_id_integrations**](IntegrationDataUseRegistersApi.md#fetch_dur_by_id_integrations) | **GET** /api/v1/integrations/dur/{id} | IntegrationDurController@show
[**update_dur_integrations**](IntegrationDataUseRegistersApi.md#update_dur_integrations) | **PUT** /api/v1/integrations/dur/{id} | Update a dur by id



## create_dur_integrations

> models::CreateCategories200Response create_dur_integrations(create_dur_integrations_request)
IntegrationDurController@store

Create a new dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dur_integrations

> models::DeleteAliases200Response delete_dur_integrations(id)
Delete a dur

Delete a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_dur_integrations

> models::UpdateDurIntegrations200Response edit_dur_integrations(id, create_dur_integrations_request)
Edit a dur

Edit a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |
**create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateDurIntegrations200Response**](update_dur_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_dur_integrations

> models::FetchAllDurIntegrations200Response fetch_all_dur_integrations(sort, per_page)
IntegrationDurController@index

Returns a list of dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sort** | Option<[**models::ProjectTitleColonAscCommaUpdatedAtColonAsc**](Models__ProjectTitleColonAscCommaUpdatedAtColonAsc.md)> | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc |  |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllDurIntegrations200Response**](fetch_all_dur_integrations_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dur_by_id_integrations

> models::FetchDurByIdIntegrations200Response fetch_dur_by_id_integrations(id)
IntegrationDurController@show

Get dur by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | data use register id | [required] |

### Return type

[**models::FetchDurByIdIntegrations200Response**](fetch_dur_by_id_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dur_integrations

> models::UpdateDurIntegrations200Response update_dur_integrations(id, create_dur_integrations_request)
Update a dur by id

Update a dur

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dur id | [required] |
**create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateDurIntegrations200Response**](update_dur_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \DarIntegrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_integration**](DarIntegrationApi.md#create_dar_integration) | **POST** /api/v1/dar-integration/{id} | DarIntegration@store
[**delete_dar_integration**](DarIntegrationApi.md#delete_dar_integration) | **DELETE** /api/v1/dar-integrations/{id} | DarIntegration@destroy
[**edit_dar_integration**](DarIntegrationApi.md#edit_dar_integration) | **PATCH** /api/v1/dar-integration/{id} | DarIntegration@edit
[**fetch_all_dar_integrations**](DarIntegrationApi.md#fetch_all_dar_integrations) | **GET** /api/v1/dar-integration | DarIntegration@index
[**fetch_dar_integration**](DarIntegrationApi.md#fetch_dar_integration) | **GET** /api/v1/dar-integration/{id} | DarIntegration@show
[**update_dar_integration**](DarIntegrationApi.md#update_dar_integration) | **PUT** /api/v1/dar-integration/{id} | DarIntegration@update



## create_dar_integration

> models::CreateCategories200Response create_dar_integration(id, update_dar_integration_request)
DarIntegration@store

Creates a new DAR integration enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dar integration id | [required] |
**update_dar_integration_request** | [**UpdateDarIntegrationRequest**](UpdateDarIntegrationRequest.md) | DarIntegration definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_dar_integration

> models::DeleteAliases200Response delete_dar_integration(id)
DarIntegration@destroy

Delete a system Dar Integration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dar integration id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_dar_integration

> models::UpdateDarIntegration200Response edit_dar_integration(id, edit_dar_integration_request)
DarIntegration@edit

Edit a DAR integration enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dar integration id | [required] |
**edit_dar_integration_request** | [**EditDarIntegrationRequest**](EditDarIntegrationRequest.md) | DarIntegration definition | [required] |

### Return type

[**models::UpdateDarIntegration200Response**](update_dar_integration_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_dar_integrations

> models::FetchAllDarIntegrations200Response fetch_all_dar_integrations()
DarIntegration@index

Returns a list of DAR integrations enabled on the system

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllDarIntegrations200Response**](fetch_all_dar_integrations_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_integration

> models::FetchAllDarIntegrations200ResponseDataInner fetch_dar_integration(id)
DarIntegration@show

Returns a single DAR integration enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dar integration id | [required] |

### Return type

[**models::FetchAllDarIntegrations200ResponseDataInner**](fetch_all_dar_integrations_200_response_data_inner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_dar_integration

> models::UpdateDarIntegration200Response update_dar_integration(id, update_dar_integration_request)
DarIntegration@update

Updates a DAR integration enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | dar integration id | [required] |
**update_dar_integration_request** | [**UpdateDarIntegrationRequest**](UpdateDarIntegrationRequest.md) | DarIntegration definition | [required] |

### Return type

[**models::UpdateDarIntegration200Response**](update_dar_integration_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


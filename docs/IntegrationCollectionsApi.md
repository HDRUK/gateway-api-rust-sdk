# \IntegrationCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_collections_integrations**](IntegrationCollectionsApi.md#create_collections_integrations) | **POST** /api/v1/integrations/collections | IntegrationCollectionController@store
[**delete_collections_integrations**](IntegrationCollectionsApi.md#delete_collections_integrations) | **DELETE** /api/v1/integrations/collections/{id} | Delete a collection
[**edit_collections_integrations**](IntegrationCollectionsApi.md#edit_collections_integrations) | **PATCH** /api/v1/integrations/collections/{id} | Edit a collection
[**fetch_all_collections_integrations**](IntegrationCollectionsApi.md#fetch_all_collections_integrations) | **GET** /api/v1/integrations/collections | IntegrationCollectionController@index
[**fetch_collections_integrations**](IntegrationCollectionsApi.md#fetch_collections_integrations) | **GET** /api/v1/integrations/collections/{id} | IntegrationCollectionController@show
[**update_collections_integrations**](IntegrationCollectionsApi.md#update_collections_integrations) | **PUT** /api/v1/integrations/collections/{id} | Update a collection



## create_collections_integrations

> models::CreateCategories200Response create_collections_integrations(update_team_collections_request)
IntegrationCollectionController@store

Create a new collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_team_collections_request** | [**UpdateTeamCollectionsRequest**](UpdateTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_collections_integrations

> models::DeleteAliases200Response delete_collections_integrations(id)
Delete a collection

Delete a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_collections_integrations

> models::FetchCollections200Response edit_collections_integrations(id, update_team_collections_request)
Edit a collection

Edit a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**update_team_collections_request** | [**UpdateTeamCollectionsRequest**](UpdateTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_collections_integrations

> models::FetchAllCollections200Response fetch_all_collections_integrations(name, per_page)
IntegrationCollectionController@index

Returns a list of collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | Filter collections by name |  |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_collections_integrations

> models::FetchCollections200Response fetch_collections_integrations(id)
IntegrationCollectionController@show

Get collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_collections_integrations

> models::FetchCollections200Response update_collections_integrations(id, update_team_collections_request)
Update a collection

Update a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**update_team_collections_request** | [**UpdateTeamCollectionsRequest**](UpdateTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


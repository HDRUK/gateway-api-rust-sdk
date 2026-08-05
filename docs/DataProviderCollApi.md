# \DataProviderCollApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_data_provider_coll**](DataProviderCollApi.md#create_data_provider_coll) | **POST** /api/v1/data_provider_colls | DataProviderColl@store
[**delete_data_provider_coll**](DataProviderCollApi.md#delete_data_provider_coll) | **DELETE** /api/v1/data_provider_colls/{id} | DataProviderColl@destroy
[**edit_data_provider_coll**](DataProviderCollApi.md#edit_data_provider_coll) | **PATCH** /api/v1/data_provider_colls/{id} | DataProviderColl@edit
[**fetch_data_provider_coll**](DataProviderCollApi.md#fetch_data_provider_coll) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show
[**fetch_data_provider_coll_summary**](DataProviderCollApi.md#fetch_data_provider_coll_summary) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary
[**fetch_data_provider_colls**](DataProviderCollApi.md#fetch_data_provider_colls) | **GET** /api/v1/data_provider_colls | DataProviderColl@index
[**update_data_provider_coll**](DataProviderCollApi.md#update_data_provider_coll) | **PUT** /api/v1/data_provider_colls/{id} | DataProviderColl@update



## create_data_provider_coll

> models::CreateDarIntegration201Response create_data_provider_coll(create_data_provider_coll_request)
DataProviderColl@store

Creates a new DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_data_provider_coll_request** | [**CreateDataProviderCollRequest**](CreateDataProviderCollRequest.md) | DataProviderColl definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_data_provider_coll

> models::DeleteApplications200Response delete_data_provider_coll(id)
DataProviderColl@destroy

Delete a DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_data_provider_coll

> models::UpdateDataProviderColl200Response edit_data_provider_coll(id, edit_data_provider_coll_request)
DataProviderColl@edit

Edit a DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID | [required] |
**edit_data_provider_coll_request** | [**EditDataProviderCollRequest**](EditDataProviderCollRequest.md) | DataProviderColl definition | [required] |

### Return type

[**models::UpdateDataProviderColl200Response**](update_data_provider_coll_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_provider_coll

> models::FetchDataProviderColl200Response fetch_data_provider_coll(id)
DataProviderColl@show

Return a single DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID | [required] |

### Return type

[**models::FetchDataProviderColl200Response**](fetch_data_provider_coll_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_provider_coll_summary

> models::FetchDataProviderCollSummary200Response fetch_data_provider_coll_summary(id)
DataProviderColl@showSummary

Return a single DataProviderColl - summary

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID - summary | [required] |

### Return type

[**models::FetchDataProviderCollSummary200Response**](fetch_data_provider_coll_summary_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_provider_colls

> models::FetchDataProviderColls200Response fetch_data_provider_colls(per_page)
DataProviderColl@index

Returns a list of DataProviderColls enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchDataProviderColls200Response**](fetch_data_provider_colls_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_data_provider_coll

> models::UpdateDataProviderColl200Response update_data_provider_coll(id, update_data_provider_coll_request)
DataProviderColl@update

Update a DataProviderColl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | DataProviderColl ID | [required] |
**update_data_provider_coll_request** | [**UpdateDataProviderCollRequest**](UpdateDataProviderCollRequest.md) | DataProviderColl definition | [required] |

### Return type

[**models::UpdateDataProviderColl200Response**](update_data_provider_coll_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \AliasApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_aliases**](AliasApi.md#create_aliases) | **POST** /api/v1/aliases | AliasController@store
[**delete_aliases**](AliasApi.md#delete_aliases) | **DELETE** /api/v1/aliases/{id} | AliasController@destroy
[**edit_aliases**](AliasApi.md#edit_aliases) | **PATCH** /api/v1/aliases/{id} | AliasController@edit
[**fetch_aliases**](AliasApi.md#fetch_aliases) | **GET** /api/v1/aliases/{id} | Return a single alias
[**fetch_all_aliases**](AliasApi.md#fetch_all_aliases) | **GET** /api/v1/aliases | List of aliases
[**update_aliases**](AliasApi.md#update_aliases) | **PUT** /api/v1/aliases/{id} | AliasController@update



## create_aliases

> models::CreateAliases200Response create_aliases(create_aliases_request)
AliasController@store

Creates a new alias

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_aliases_request** | [**CreateAliasesRequest**](CreateAliasesRequest.md) | Alias definition | [required] |

### Return type

[**models::CreateAliases200Response**](create_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_aliases

> models::DeleteAliases200Response delete_aliases(id)
AliasController@destroy

Delete an alias

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | alias id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_aliases

> models::UpdateAliases200Response edit_aliases(id, edit_aliases_request)
AliasController@edit

Edit a alias

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | alias id | [required] |
**edit_aliases_request** | [**EditAliasesRequest**](EditAliasesRequest.md) | Alias definition | [required] |

### Return type

[**models::UpdateAliases200Response**](update_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_aliases

> models::FetchAliases200Response fetch_aliases(id)
Return a single alias

Return a single alias

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | alias id | [required] |

### Return type

[**models::FetchAliases200Response**](fetch_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_aliases

> models::FetchAllAliases200Response fetch_all_aliases()
List of aliases

Returns a list of aliases

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllAliases200Response**](fetch_all_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_aliases

> models::UpdateAliases200Response update_aliases(id, create_aliases_request)
AliasController@update

Update a alias

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | alias id | [required] |
**create_aliases_request** | [**CreateAliasesRequest**](CreateAliasesRequest.md) | Alias definition | [required] |

### Return type

[**models::UpdateAliases200Response**](update_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \SavedSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_saved_searches**](SavedSearchApi.md#create_saved_searches) | **POST** /api/v1/saved_searches | SavedSearch@store
[**delete_saved_searches**](SavedSearchApi.md#delete_saved_searches) | **DELETE** /api/v1/saved_searches/{id} | SavedSearch@destroy
[**edit_saved_searches**](SavedSearchApi.md#edit_saved_searches) | **PATCH** /api/v1/saved_searches/{id} | SavedSearch@update
[**fetch_all_saved_searches**](SavedSearchApi.md#fetch_all_saved_searches) | **GET** /api/v1/saved_searches | SavedSearch@index
[**fetch_saved_searches**](SavedSearchApi.md#fetch_saved_searches) | **GET** /api/v1/saved_searches/{id} | SavedSearch@show
[**update_saved_searches**](SavedSearchApi.md#update_saved_searches) | **PUT** /api/v1/saved_searches/{id} | SavedSearch@update



## create_saved_searches

> models::CreateCategories200Response create_saved_searches(create_saved_searches_request)
SavedSearch@store

Creates a new saved search

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_saved_searches_request** | [**CreateSavedSearchesRequest**](CreateSavedSearchesRequest.md) | Saved search definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_saved_searches

> models::DeleteAliases200Response delete_saved_searches(id)
SavedSearch@destroy

Delete a saved search

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | saved search id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_saved_searches

> models::UpdateSavedSearches200Response edit_saved_searches(id, edit_saved_searches_request)
SavedSearch@update

Edit a saved search

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | saved search id | [required] |
**edit_saved_searches_request** | [**EditSavedSearchesRequest**](EditSavedSearchesRequest.md) | Saved search definition | [required] |

### Return type

[**models::UpdateSavedSearches200Response**](update_saved_searches_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_saved_searches

> models::FetchAllSavedSearches200Response fetch_all_saved_searches(per_page)
SavedSearch@index

Returns a list of saved searches enabled on the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | Specify number of results per page |  |

### Return type

[**models::FetchAllSavedSearches200Response**](fetch_all_saved_searches_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_saved_searches

> models::FetchAllSavedSearches200Response fetch_saved_searches(id)
SavedSearch@show

Return a single saved search

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | saved search id | [required] |

### Return type

[**models::FetchAllSavedSearches200Response**](fetch_all_saved_searches_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_saved_searches

> models::UpdateSavedSearches200Response update_saved_searches(id, update_saved_searches_request)
SavedSearch@update

Update a saved search

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | saved search id | [required] |
**update_saved_searches_request** | [**UpdateSavedSearchesRequest**](UpdateSavedSearchesRequest.md) | Saved search definition | [required] |

### Return type

[**models::UpdateSavedSearches200Response**](update_saved_searches_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


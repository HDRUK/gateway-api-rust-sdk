# \CollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_team_unique_fields_collection_v2**](CollectionsApi.md#count_team_unique_fields_collection_v2) | **GET** /api/v2/teams/{teamId}/collections/count/{field} | TeamCollectionController@count
[**count_unique_fields_collections**](CollectionsApi.md#count_unique_fields_collections) | **GET** /api/v1/collections/count/{field} | CollectionController@count
[**count_unique_fields_collections_v2**](CollectionsApi.md#count_unique_fields_collections_v2) | **GET** /api/v2/collections/count/{field} | CollectionController@count
[**count_user_unique_fields_collection_v2**](CollectionsApi.md#count_user_unique_fields_collection_v2) | **GET** /api/v2/users/{userId}/collections/count/{field} | UserCollectionController@count
[**create_collections**](CollectionsApi.md#create_collections) | **POST** /api/v2/collections | CollectionController@store
[**create_team_collections**](CollectionsApi.md#create_team_collections) | **POST** /api/v1/teams/{teamId}/collections | CollectionController@store
[**create_team_collections_v2**](CollectionsApi.md#create_team_collections_v2) | **POST** /api/v2/teams/{teamId}/collections | TeamCollectionController@store
[**create_user_collections**](CollectionsApi.md#create_user_collections) | **POST** /api/v2/users/collections | UserCollectionController@store
[**delete_collections_v2**](CollectionsApi.md#delete_collections_v2) | **DELETE** /api/v2/collections/{id} | Delete a collection
[**delete_team_collections**](CollectionsApi.md#delete_team_collections) | **DELETE** /api/v1/teams/{teamId}/collections/{id} | Delete a collection
[**delete_team_collections_v2**](CollectionsApi.md#delete_team_collections_v2) | **DELETE** /api/v2/teams/{teamId}/collections/{id} | Delete a collection
[**delete_user_collections_v2**](CollectionsApi.md#delete_user_collections_v2) | **DELETE** /api/v2/users/{userId}/collections/{id} | Delete a collection
[**edit_collections_v2**](CollectionsApi.md#edit_collections_v2) | **PATCH** /api/v2/collections/{id} | Edit a collection
[**edit_team_collections**](CollectionsApi.md#edit_team_collections) | **PATCH** /api/v1/teams/{teamId}/collections/{id} | Edit a collection
[**edit_team_collections_v2**](CollectionsApi.md#edit_team_collections_v2) | **PATCH** /api/v2/teams/{teamId}/collections/{id} | Edit a collection
[**edit_user_collections_v2**](CollectionsApi.md#edit_user_collections_v2) | **PATCH** /api/v2/users/{userId}/collections/{id} | Edit a collection
[**fetch_all_collections**](CollectionsApi.md#fetch_all_collections) | **GET** /api/v1/collections | CollectionController@index
[**fetch_all_collections_v2**](CollectionsApi.md#fetch_all_collections_v2) | **GET** /api/v2/collections | CollectionController@index
[**fetch_collections**](CollectionsApi.md#fetch_collections) | **GET** /api/v1/collections/{id} | CollectionController@show
[**fetch_collections_v2**](CollectionsApi.md#fetch_collections_v2) | **GET** /api/v2/collections/{id} | CollectionController@show
[**fetch_team_active_collections_v2**](CollectionsApi.md#fetch_team_active_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/active | TeamCollectionController@indexActive
[**fetch_team_archived_collections_v2**](CollectionsApi.md#fetch_team_archived_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/archived | TeamCollectionController@indexArchived
[**fetch_team_collection_v2**](CollectionsApi.md#fetch_team_collection_v2) | **GET** /api/v2/teams/{teamId}/collections/{id} | TeamCollectionController@show
[**fetch_team_draft_collections_v2**](CollectionsApi.md#fetch_team_draft_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/draft | TeamCollectionController@indexDraft
[**fetch_user_archived_collections_v2**](CollectionsApi.md#fetch_user_archived_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/archived | UserCollectionController@indexArchived
[**fetch_user_collection_v2**](CollectionsApi.md#fetch_user_collection_v2) | **GET** /api/v2/users/{userId}/collections/{id} | CollectionController@show
[**fetch_user_collections_v2**](CollectionsApi.md#fetch_user_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/active | UserCollectionController@indexActive
[**fetch_user_draft_collections_v2**](CollectionsApi.md#fetch_user_draft_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/draft | UserCollectionController@indexDraft
[**update_collections_v2**](CollectionsApi.md#update_collections_v2) | **PUT** /api/v2/collections/{id} | Update a collection
[**update_team_collections**](CollectionsApi.md#update_team_collections) | **PUT** /api/v1/teams/{teamId}/collections/{id} | Update a collection
[**update_team_collections_v2**](CollectionsApi.md#update_team_collections_v2) | **PUT** /api/v2/teams/{teamId}/collections/{id} | Update a collection
[**update_user_collections_v2**](CollectionsApi.md#update_user_collections_v2) | **PUT** /api/v2/users/{userId}/collections/{id} | Update a collection



## count_team_unique_fields_collection_v2

> models::CountUniqueFieldsCollections200Response count_team_unique_fields_collection_v2(team_id, field)
TeamCollectionController@count

Get user counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_unique_fields_collections

> models::CountUniqueFieldsCollections200Response count_unique_fields_collections(field, team_id, user_id)
CollectionController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**field** | **String** | name of the field to perform a count on | [required] |
**team_id** | **i32** | team id | [required] |
**user_id** | **i32** | user id | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_unique_fields_collections_v2

> models::CountUniqueFieldsCollections200Response count_unique_fields_collections_v2(field)
CollectionController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_user_unique_fields_collection_v2

> models::CountUniqueFieldsCollections200Response count_user_unique_fields_collection_v2(user_id, field)
UserCollectionController@count

Get user counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_collections

> models::CreateCategories200Response create_collections(create_collections_request)
CollectionController@store

Create a new collection owned by an individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_collections_request** | [**CreateCollectionsRequest**](CreateCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_team_collections

> models::CreateCategories200Response create_team_collections(team_id, create_team_collections_request)
CollectionController@store

Create a new collection for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_team_collections_request** | [**CreateTeamCollectionsRequest**](CreateTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_team_collections_v2

> models::CreateCategories200Response create_team_collections_v2(team_id, create_team_collections_request)
TeamCollectionController@store

Create a new collection for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_team_collections_request** | [**CreateTeamCollectionsRequest**](CreateTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_user_collections

> models::CreateCategories200Response create_user_collections(create_collections_request)
UserCollectionController@store

Create a new collection owned by an individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_collections_request** | [**CreateCollectionsRequest**](CreateCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_collections_v2

> models::DeleteAliases200Response delete_collections_v2(id)
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


## delete_team_collections

> models::DeleteAliases200Response delete_team_collections(team_id, id)
Delete a collection

Delete a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | collection id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_collections_v2

> models::DeleteAliases200Response delete_team_collections_v2(team_id, id)
Delete a collection

Delete a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | collection id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_user_collections_v2

> models::DeleteAliases200Response delete_user_collections_v2(user_id, id)
Delete a collection

Delete a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**id** | **i32** | collection id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_collections_v2

> models::FetchCollections200Response edit_collections_v2(id, edit_collections_v2_request, unarchive)
Edit a collection

Edit a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**edit_collections_v2_request** | [**EditCollectionsV2Request**](EditCollectionsV2Request.md) | Pass user credentials | [required] |
**unarchive** | Option<**String**> | Unarchive a collection |  |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_team_collections

> models::FetchCollections200Response edit_team_collections(team_id, id, edit_team_collections_request, unarchive)
Edit a collection

Edit a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | collection id | [required] |
**edit_team_collections_request** | [**EditTeamCollectionsRequest**](EditTeamCollectionsRequest.md) | Pass user credentials | [required] |
**unarchive** | Option<**String**> | Unarchive a collection |  |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_team_collections_v2

> models::FetchCollections200Response edit_team_collections_v2(team_id, id, edit_team_collections_request)
Edit a collection

Edit a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | collection id | [required] |
**edit_team_collections_request** | [**EditTeamCollectionsRequest**](EditTeamCollectionsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_user_collections_v2

> models::FetchCollections200Response edit_user_collections_v2(user_id, id, edit_collections_v2_request)
Edit a collection

Edit a collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**id** | **i32** | collection id | [required] |
**edit_collections_v2_request** | [**EditCollectionsV2Request**](EditCollectionsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_collections

> models::FetchAllCollections200Response fetch_all_collections(name, team_id, user_id, title, status, per_page)
CollectionController@index

Returns a list of collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | Filter collections by name |  |
**team_id** | Option<**i32**> | Filter collections by team ID |  |
**user_id** | Option<**i32**> | Filter collections by user ID |  |
**title** | Option<**String**> | Filter collections by title |  |
**status** | Option<**String**> | Filter collections by status (DRAFT, ACTIVE, ARCHIVED) |  |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_collections_v2

> models::FetchAllCollections200Response fetch_all_collections_v2()
CollectionController@index

Returns a list of collections

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_collections

> models::FetchCollections200Response fetch_collections(id, view_type)
CollectionController@show

Get collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**view_type** | Option<**String**> | Query flag to show full collection data or a trimmed version (defaults to full). |  |[default to full]

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_collections_v2

> models::FetchCollections200Response fetch_collections_v2(id, view_type)
CollectionController@show

Get collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**view_type** | Option<**String**> | Query flag to show full collection data or a trimmed version (defaults to full). |  |[default to full]

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_active_collections_v2

> models::FetchAllCollections200Response fetch_team_active_collections_v2(team_id)
TeamCollectionController@indexActive

Returns a list of a teams collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_archived_collections_v2

> models::FetchAllCollections200Response fetch_team_archived_collections_v2(team_id)
TeamCollectionController@indexArchived

Returns a list of a teams archived collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_collection_v2

> models::FetchCollections200Response fetch_team_collection_v2(team_id, id)
TeamCollectionController@show

Get collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | collection id | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_draft_collections_v2

> models::FetchAllCollections200Response fetch_team_draft_collections_v2(team_id)
TeamCollectionController@indexDraft

Returns a list of a teams draft collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_archived_collections_v2

> models::FetchAllCollections200Response fetch_user_archived_collections_v2(user_id)
UserCollectionController@indexArchived

Returns a list of a users archived collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_collection_v2

> models::FetchCollections200Response fetch_user_collection_v2(user_id, id)
CollectionController@show

Get collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**id** | **i32** | collection id | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_collections_v2

> models::FetchAllCollections200Response fetch_user_collections_v2(user_id)
UserCollectionController@indexActive

Returns a list of a users collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_draft_collections_v2

> models::FetchAllCollections200Response fetch_user_draft_collections_v2(user_id)
UserCollectionController@indexDraft

Returns a list of a users draft collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |

### Return type

[**models::FetchAllCollections200Response**](fetch_all_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_collections_v2

> models::FetchCollections200Response update_collections_v2(id, update_collections_v2_request)
Update a collection

Update a collection owned by an individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | collection id | [required] |
**update_collections_v2_request** | [**UpdateCollectionsV2Request**](UpdateCollectionsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_team_collections

> models::FetchCollections200Response update_team_collections(team_id, id, update_team_collections_request)
Update a collection

Update a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
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


## update_team_collections_v2

> models::FetchCollections200Response update_team_collections_v2(team_id, id, update_team_collections_request)
Update a collection

Update a collection owned by a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
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


## update_user_collections_v2

> models::FetchCollections200Response update_user_collections_v2(user_id, id, update_collections_v2_request)
Update a collection

Update a collection owned by an individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**id** | **i32** | collection id | [required] |
**update_collections_v2_request** | [**UpdateCollectionsV2Request**](UpdateCollectionsV2Request.md) | Pass user credentials | [required] |

### Return type

[**models::FetchCollections200Response**](fetch_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


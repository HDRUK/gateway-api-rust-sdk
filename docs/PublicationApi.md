# \PublicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_team_unique_fields_publication_v2**](PublicationApi.md#count_team_unique_fields_publication_v2) | **GET** /api/v2/teams/{teamId}/publications/count/{field} | TeamPublicationController@count
[**count_unique_fields_publications**](PublicationApi.md#count_unique_fields_publications) | **GET** /api/v1/publication/count/{field} | PublicationController@count
[**count_user_unique_fields_publication_v2**](PublicationApi.md#count_user_unique_fields_publication_v2) | **GET** /api/v2/users/{userId}/publications/count/{field} | UserPublicationController@count
[**create_publications**](PublicationApi.md#create_publications) | **POST** /api/v1/publications | PublicationController@store
[**create_publications_v2_by_team_id**](PublicationApi.md#create_publications_v2_by_team_id) | **POST** /api/v2/teams/{teamId}/publications | TeamPublicationController@store
[**create_publications_v2_by_user_id**](PublicationApi.md#create_publications_v2_by_user_id) | **POST** /api/v2/users/{userId}/publications | UserPublicationController@store
[**delete_publications**](PublicationApi.md#delete_publications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy
[**delete_publications_v2_by_team_id**](PublicationApi.md#delete_publications_v2_by_team_id) | **DELETE** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@destroy
[**delete_publications_v2_by_user_id**](PublicationApi.md#delete_publications_v2_by_user_id) | **DELETE** /api/v2/users/{userId}/publications/{id} | UserPublicationController@destroy
[**edit_publications**](PublicationApi.md#edit_publications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit
[**edit_publications_v2_by_team_id**](PublicationApi.md#edit_publications_v2_by_team_id) | **PATCH** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@edit
[**edit_publications_v2_by_user_id**](PublicationApi.md#edit_publications_v2_by_user_id) | **PATCH** /api/v2/users/{userId}/publications/{id} | UserPublicationController@edit
[**fetch_all_publications**](PublicationApi.md#fetch_all_publications) | **GET** /api/v1/publications | PublicationController@index
[**fetch_all_publications_by_team_and_status_v2**](PublicationApi.md#fetch_all_publications_by_team_and_status_v2) | **GET** /api/v2/teams/{teamId}/publications/status/{status} | TeamPublicationController@indexStatus
[**fetch_all_publications_by_user_and_status_v2**](PublicationApi.md#fetch_all_publications_by_user_and_status_v2) | **GET** /api/v2/users/{userId}/publications/{status} | UserPublicationController@indexStatus
[**fetch_all_publications_v2**](PublicationApi.md#fetch_all_publications_v2) | **GET** /api/v2/publications | PublicationController@indexActive
[**fetch_publications**](PublicationApi.md#fetch_publications) | **GET** /api/v1/publications/{id} | PublicationController@show
[**fetch_publications_by_team_and_by_id_v2**](PublicationApi.md#fetch_publications_by_team_and_by_id_v2) | **GET** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@show
[**fetch_publications_by_user_and_by_id_v2**](PublicationApi.md#fetch_publications_by_user_and_by_id_v2) | **GET** /api/v2/users/{userId}/publications/{id} | UserPublicationController@show
[**fetch_publications_v2**](PublicationApi.md#fetch_publications_v2) | **GET** /api/v2/publications/{id} | PublicationController@showActive
[**update_publications**](PublicationApi.md#update_publications) | **PUT** /api/v1/publications/{id} | PublicationController@update
[**update_publications_v2_by_team_id**](PublicationApi.md#update_publications_v2_by_team_id) | **PUT** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@update
[**update_publications_v2_by_user_id**](PublicationApi.md#update_publications_v2_by_user_id) | **PUT** /api/v2/users/{userId}/publications/{id} | UserPublicationController@update



## count_team_unique_fields_publication_v2

> models::CountUniqueFieldsCollections200Response count_team_unique_fields_publication_v2(team_id, field)
TeamPublicationController@count

Get team counts for distinct entries of a field in the model

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


## count_unique_fields_publications

> models::CountUniqueFieldsCollections200Response count_unique_fields_publications(field, owner_id, team_id)
PublicationController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**field** | **String** | name of the field to perform a count on | [required] |
**owner_id** | **i32** | owner id | [required] |
**team_id** | Option<**i32**> |  |  |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_user_unique_fields_publication_v2

> models::CountUniqueFieldsCollections200Response count_user_unique_fields_publication_v2(user_id, field)
UserPublicationController@count

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


## create_publications

> models::CreateCategories200Response create_publications(create_publications_request)
PublicationController@store

Create a new publication

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_publications_v2_by_team_id

> models::CreateCategories200Response create_publications_v2_by_team_id(team_id, create_publications_request)
TeamPublicationController@store

Create a new publication by team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_publications_v2_by_user_id

> models::CreateCategories200Response create_publications_v2_by_user_id(user_id, create_publications_request)
UserPublicationController@store

Create a new publication by user id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_publications

> models::DeleteFederation200Response delete_publications(id)
PublicationController@destroy

Delete publication by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | publication id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_publications_v2_by_team_id

> models::DeleteFederation200Response delete_publications_v2_by_team_id(team_id, id)
TeamPublicationController@destroy

Delete publication by team id and id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | publication id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_publications_v2_by_user_id

> models::DeleteFederation200Response delete_publications_v2_by_user_id(user_id, id)
UserPublicationController@destroy

Delete publication by user id and id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**id** | **i32** | publication id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_publications

> models::FetchPublications200Response edit_publications(id, update_publications_request, unarchive)
PublicationController@edit

Edit publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | publications id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |
**unarchive** | Option<**String**> | Unarchive a publication |  |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_publications_v2_by_team_id

> models::FetchPublications200Response edit_publications_v2_by_team_id(team_id, id, update_publications_request)
TeamPublicationController@edit

Edit publications by team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | publications id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_publications_v2_by_user_id

> models::FetchPublications200Response edit_publications_v2_by_user_id(user_id, id, update_publications_request)
UserPublicationController@edit

Edit publications by user id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**id** | **i32** | publications id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_publications

> models::FetchAllPublications200Response fetch_all_publications(paper_title, owner_id, team_id, status)
PublicationController@index

Get All Publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**paper_title** | Option<**String**> | Filter tools by paper title |  |
**owner_id** | Option<[**models::Int**](Models__Int.md)> | Filter tools by owner id |  |
**team_id** | Option<[**models::Int**](Models__Int.md)> | Filter tools by team id |  |
**status** | Option<**String**> | Publication status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') |  |

### Return type

[**models::FetchAllPublications200Response**](fetch_all_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_publications_by_team_and_status_v2

> models::FetchAllPublications200Response fetch_all_publications_by_team_and_status_v2(team_id, status, paper_title)
TeamPublicationController@indexStatus

Returns a list of a teams publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i64** | ID of the team | [required] |
**status** | **String** | Status of the team (active, draft, or archived). Defaults to active if not provided. | [required] |[default to active]
**paper_title** | Option<**String**> | Filter Publication by title |  |

### Return type

[**models::FetchAllPublications200Response**](fetch_all_publications_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_publications_by_user_and_status_v2

> models::FetchAllPublications200Response fetch_all_publications_by_user_and_status_v2(user_id, status, paper_title)
UserPublicationController@indexStatus

Returns a list of a users publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**status** | **String** | Status of the team (active, draft, or archived). Defaults to active if not provided. | [required] |[default to active]
**paper_title** | Option<**String**> | Filter Publication by title |  |

### Return type

[**models::FetchAllPublications200Response**](fetch_all_publications_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_publications_v2

> models::FetchAllPublications200Response fetch_all_publications_v2(paper_title, with_related, per_page)
PublicationController@indexActive

Get All Publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**paper_title** | Option<**String**> | Filter tools by paper title |  |
**with_related** | Option<**bool**> | Return related datasets |  |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllPublications200Response**](fetch_all_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_publications

> models::FetchPublications200Response fetch_publications(id)
PublicationController@show

Get publication by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | publication id | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_publications_by_team_and_by_id_v2

> models::FetchPublications200Response fetch_publications_by_team_and_by_id_v2(team_id, id)
TeamPublicationController@show

Get publication by team id and by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | publication id | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_publications_by_user_and_by_id_v2

> models::FetchPublications200Response fetch_publications_by_user_and_by_id_v2(user_id, id)
UserPublicationController@show

Get publication by user id and by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**id** | **i32** | publication id | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_publications_v2

> models::FetchPublications200Response fetch_publications_v2(id)
PublicationController@showActive

Get publication by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | publication id | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_publications

> models::FetchPublications200Response update_publications(id, update_publications_request)
PublicationController@update

Update publications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | publication id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_publications_v2_by_team_id

> models::FetchPublications200Response update_publications_v2_by_team_id(team_id, id, update_publications_request)
TeamPublicationController@update

Update publications by team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**id** | **i32** | publication id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_publications_v2_by_user_id

> models::FetchPublications200Response update_publications_v2_by_user_id(user_id, id, update_publications_request)
UserPublicationController@update

Update publications by user id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i64** | ID of the user | [required] |
**id** | **i32** | publication id | [required] |
**update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchPublications200Response**](fetch_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


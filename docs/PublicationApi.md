# \PublicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_unique_fields_publications**](PublicationApi.md#count_unique_fields_publications) | **GET** /api/v1/publication/count/{field} | PublicationController@count
[**create_publications**](PublicationApi.md#create_publications) | **POST** /api/v1/publications | PublicationController@store
[**delete_publications**](PublicationApi.md#delete_publications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy
[**edit_publications**](PublicationApi.md#edit_publications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit
[**fetch_all_publications**](PublicationApi.md#fetch_all_publications) | **GET** /api/v1/publications | PublicationController@index
[**fetch_all_publications_v2**](PublicationApi.md#fetch_all_publications_v2) | **GET** /api/v2/publications | PublicationController@indexActive
[**fetch_publications**](PublicationApi.md#fetch_publications) | **GET** /api/v1/publications/{id} | PublicationController@show
[**fetch_publications_v2**](PublicationApi.md#fetch_publications_v2) | **GET** /api/v2/publications/{id} | PublicationController@showActive
[**update_publications**](PublicationApi.md#update_publications) | **PUT** /api/v1/publications/{id} | PublicationController@update



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


## create_publications

> models::CreateDarIntegration201Response create_publications(create_publications_request)
PublicationController@store

Create a new publication

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

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


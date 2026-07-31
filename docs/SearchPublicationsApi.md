# \SearchPublicationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_publications**](SearchPublicationsApi.md#search_publications) | **POST** /api/v1/search/publications | Search@publications
[**search_publications_by_doi**](SearchPublicationsApi.md#search_publications_by_doi) | **POST** /api/v1/search/doi | Search@publications



## search_publications

> models::SearchPublications200Response search_publications(search_publications_request, sort, direction, source)
Search@publications

Returns gateway publications related to the provided query term(s)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_publications_request** | [**SearchPublicationsRequest**](SearchPublicationsRequest.md) | Submit search query | [required] |
**sort** | Option<**String**> | Field to sort by (default: 'score') |  |
**direction** | Option<**String**> | Sort direction ('asc' or 'desc', default: 'desc') |  |
**source** | Option<**String**> | Which source to search ('GAT' or 'FED', default: 'GAT') |  |

### Return type

[**models::SearchPublications200Response**](search_publications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_publications_by_doi

> models::SearchPublicationsByDoi200Response search_publications_by_doi(search_publications_by_doi_request)
Search@publications

Returns publications from EuropePMC matching a give DOI

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_publications_by_doi_request** | [**SearchPublicationsByDoiRequest**](SearchPublicationsByDoiRequest.md) | Submit search query | [required] |

### Return type

[**models::SearchPublicationsByDoi200Response**](search_publications_by_doi_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


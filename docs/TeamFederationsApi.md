# \TeamFederationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_federation_team**](TeamFederationsApi.md#create_federation_team) | **POST** /api/v1/teams/{teamId}/federations | FederationController@store
[**delete_federation**](TeamFederationsApi.md#delete_federation) | **DELETE** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@destroy
[**get_federation_by_federation_id_and_team_id**](TeamFederationsApi.md#get_federation_by_federation_id_and_team_id) | **GET** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@show
[**get_federation_history**](TeamFederationsApi.md#get_federation_history) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/history | FederationController@history
[**get_federation_team_id**](TeamFederationsApi.md#get_federation_team_id) | **GET** /api/v1/teams/{teamId}/federations | FederationController@index
[**run_federation**](TeamFederationsApi.md#run_federation) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/run | FederationController@runNow
[**test_federation**](TeamFederationsApi.md#test_federation) | **POST** /api/v1/teams/{teamId}/federations/test | FederationController@testFederation
[**update_federation_team**](TeamFederationsApi.md#update_federation_team) | **PUT** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@update



## create_federation_team

> models::CreateDarIntegration201Response create_federation_team(team_id, create_federation_team_request)
FederationController@store

Create federation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**create_federation_team_request** | [**CreateFederationTeamRequest**](CreateFederationTeamRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_federation

> models::DeleteFederation200Response delete_federation(team_id, federation_id)
FederationController@destroy

Delete federation for team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**federation_id** | **i32** | federation id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_federation_by_federation_id_and_team_id

> models::GetFederationByFederationIdAndTeamId200Response get_federation_by_federation_id_and_team_id(team_id, federation_id)
FederationController@show

Get federation by federation id from team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**federation_id** | **i32** | federation id | [required] |

### Return type

[**models::GetFederationByFederationIdAndTeamId200Response**](get_federation_by_federation_id_and_team_id_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_federation_history

> models::GetFederationHistory200Response get_federation_history(team_id, federation_id, per_page)
FederationController@history

Get run history for a federation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**federation_id** | **i32** | federation id | [required] |
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::GetFederationHistory200Response**](get_federation_history_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_federation_team_id

> models::GetFederationTeamId200Response get_federation_team_id(team_id)
FederationController@index

Get federations by team id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |

### Return type

[**models::GetFederationTeamId200Response**](get_federation_team_id_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## run_federation

> models::TestFederation200Response run_federation(team_id, federation_id)
FederationController@runNow

Run federation immediately

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**federation_id** | **i32** | federation id | [required] |

### Return type

[**models::TestFederation200Response**](test_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## test_federation

> models::TestFederation200Response test_federation(team_id)
FederationController@testFederation

Test federation configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |

### Return type

[**models::TestFederation200Response**](test_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_federation_team

> models::CreateDarIntegration201Response update_federation_team(team_id, federation_id, update_federation_team_request)
FederationController@update

Update federation for team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | team id | [required] |
**federation_id** | **i32** | federation id | [required] |
**update_federation_team_request** | [**UpdateFederationTeamRequest**](UpdateFederationTeamRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


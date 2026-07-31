# \UserDataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_all_user_dar_applications**](UserDataAccessApplicationApi.md#count_all_user_dar_applications) | **GET** /api/v1/users/{userId}/dar/applications/count | UserDataAccessApplicationController@allCounts
[**count_user_dar_applications_by_field**](UserDataAccessApplicationApi.md#count_user_dar_applications_by_field) | **GET** /api/v1/users/{userId}/dar/applications/count/{field} | UserDataAccessApplicationController@count
[**create_user_dar_application_answers**](UserDataAccessApplicationApi.md#create_user_dar_application_answers) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplication@storeAnswers
[**fetch_user_dar_application_answers**](UserDataAccessApplicationApi.md#fetch_user_dar_application_answers) | **GET** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplicationController@showAnswers
[**fetch_user_dar_application_details**](UserDataAccessApplicationApi.md#fetch_user_dar_application_details) | **GET** /api/v1/users/{userId}/dar/applications/{id} | UserDataAccessApplicationController@show
[**fetch_user_dar_application_header**](UserDataAccessApplicationApi.md#fetch_user_dar_application_header) | **GET** /api/v1/users/{userId}/dar/applications/{id}/showHeader | UserDataAccessApplicationController@showHeader
[**fetch_user_dar_applications**](UserDataAccessApplicationApi.md#fetch_user_dar_applications) | **GET** /api/v1/users/{userId}/dar/applications | UserDataAccessApplicationController@index



## count_all_user_dar_applications

> models::CountUniqueFieldsCollections200Response count_all_user_dar_applications(user_id)
UserDataAccessApplicationController@allCounts

Get Counts for all status fields in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_user_dar_applications_by_field

> models::CountUniqueFieldsCollections200Response count_user_dar_applications_by_field(user_id, field)
UserDataAccessApplicationController@count

Get Counts for distinct entries of a field in the model

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**field** | **String** | name of the field to perform a count on | [required] |

### Return type

[**models::CountUniqueFieldsCollections200Response**](count_unique_fields_collections_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_user_dar_application_answers

> models::CreateCategories200Response create_user_dar_application_answers(user_id, id, create_user_dar_application_answers_request)
UserDataAccessApplication@storeAnswers

Add answers to the user's DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**create_user_dar_application_answers_request** | [**CreateUserDarApplicationAnswersRequest**](CreateUserDarApplicationAnswersRequest.md) | UserDataAccessApplication definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_answers

> models::FetchTeamDarApplicationAnswers200Response fetch_user_dar_application_answers(user_id, id)
UserDataAccessApplicationController@showAnswers

Return answers from the user's DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationAnswers200Response**](fetch_team_dar_application_answers_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_details

> models::FetchTeamDarApplication200Response fetch_user_dar_application_details(user_id, id)
UserDataAccessApplicationController@show

Return a DAR application belonging to the user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_header

> models::FetchTeamDarApplication200Response fetch_user_dar_application_header(user_id, id)
UserDataAccessApplicationController@showHeader

Get header information about a specific DAR

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplication200Response**](fetch_team_dar_application_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_applications

> models::FetchTeamDarApplications200Response fetch_user_dar_applications(user_id)
UserDataAccessApplicationController@index

List of dar applications belonging to a user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |

### Return type

[**models::FetchTeamDarApplications200Response**](fetch_team_dar_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


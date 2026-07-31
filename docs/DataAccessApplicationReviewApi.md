# \DataAccessApplicationReviewApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#create_team_dar_application_question_review) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews | DataAccessApplicationReview@store
[**create_team_dar_application_review**](DataAccessApplicationReviewApi.md#create_team_dar_application_review) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@storeGlobal
[**delete_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#delete_team_dar_application_question_review) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@destroy
[**delete_team_dar_application_review**](DataAccessApplicationReviewApi.md#delete_team_dar_application_review) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@destroyGlobal
[**delete_team_dar_application_review_file**](DataAccessApplicationReviewApi.md#delete_team_dar_application_review_file) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/files/{fileId} | DataAccessApplicationReview@destroyFile
[**fetch_team_dar_application_review_file**](DataAccessApplicationReviewApi.md#fetch_team_dar_application_review_file) | **GET** /ap1/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadFile
[**fetch_team_dar_application_reviews**](DataAccessApplicationReviewApi.md#fetch_team_dar_application_reviews) | **GET** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**fetch_user_dar_application_review_file**](DataAccessApplicationReviewApi.md#fetch_user_dar_application_review_file) | **GET** /ap1/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadUserFile
[**fetch_user_dar_application_reviews**](DataAccessApplicationReviewApi.md#fetch_user_dar_application_reviews) | **GET** /api/v1/users/{userId}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**update_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#update_team_dar_application_question_review) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@update
[**update_team_dar_application_review**](DataAccessApplicationReviewApi.md#update_team_dar_application_review) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@updateGlobal
[**update_user_dar_application_question_review**](DataAccessApplicationReviewApi.md#update_user_dar_application_question_review) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@userUpdate
[**update_user_dar_application_review**](DataAccessApplicationReviewApi.md#update_user_dar_application_review) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@userUpdateGlobal



## create_team_dar_application_question_review

> models::CreateCategories200Response create_team_dar_application_question_review(team_id, id, question_id, create_team_dar_application_review_request)
DataAccessApplicationReview@store

Create a new review comment on a question in a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**question_id** | **i32** | DAR application question id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_team_dar_application_review

> models::CreateCategories200Response create_team_dar_application_review(team_id, id, create_team_dar_application_review_request)
DataAccessApplicationReview@storeGlobal

Create a new review comment on a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_dar_application_question_review

> models::DeleteAliases200Response delete_team_dar_application_question_review(team_id, id, question_id, review_id)
DataAccessApplicationReview@destroy

Delete a review from a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**question_id** | **i32** | DAR application question id | [required] |
**review_id** | **i32** | DAR application review id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_dar_application_review

> models::DeleteAliases200Response delete_team_dar_application_review(team_id, id, review_id)
DataAccessApplicationReview@destroyGlobal

Delete a review from a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**review_id** | **i32** | DAR application review id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_team_dar_application_review_file

> models::DeleteAliases200Response delete_team_dar_application_review_file(team_id, id, review_id, file_id)
DataAccessApplicationReview@destroyFile

Delete a file associated with a DAR review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | Dar application id | [required] |
**review_id** | **i32** | Review id | [required] |
**file_id** | **String** | File uuid | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_review_file

> fetch_team_dar_application_review_file(team_id, id, review_id, file_id)
DataAccessApplicationReview@downloadFile

Download a file associated with a DAR application review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**file_id** | **String** | File uuid | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_dar_application_reviews

> models::FetchTeamDarApplicationReviews200Response fetch_team_dar_application_reviews(team_id, id)
DataAccessApplicationReview@index

Return all reviews on a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationReviews200Response**](fetch_team_dar_application_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_review_file

> fetch_user_dar_application_review_file(user_id, id, review_id, file_id)
DataAccessApplicationReview@downloadUserFile

Download a file associated with a DAR application review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**file_id** | **String** | File uuid | [required] |

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: file, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_user_dar_application_reviews

> models::FetchTeamDarApplicationReviews200Response fetch_user_dar_application_reviews(user_id, id)
DataAccessApplicationReview@index

Return all reviews on a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |

### Return type

[**models::FetchTeamDarApplicationReviews200Response**](fetch_team_dar_application_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_team_dar_application_question_review

> models::UpdateTeamDarApplicationQuestionReview200Response update_team_dar_application_question_review(team_id, id, question_id, review_id, create_team_dar_application_review_request)
DataAccessApplicationReview@update

Update a review comment on a question in a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**question_id** | **i32** | DAR application question id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::UpdateTeamDarApplicationQuestionReview200Response**](update_team_dar_application_question_review_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_team_dar_application_review

> models::UpdateTeamDarApplicationQuestionReview200Response update_team_dar_application_review(team_id, id, review_id, create_team_dar_application_review_request)
DataAccessApplicationReview@updateGlobal

Update a review comment on a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team id | [required] |
**id** | **i32** | DAR application id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::UpdateTeamDarApplicationQuestionReview200Response**](update_team_dar_application_question_review_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_user_dar_application_question_review

> models::UpdateTeamDarApplicationQuestionReview200Response update_user_dar_application_question_review(user_id, id, question_id, review_id, create_team_dar_application_review_request)
DataAccessApplicationReview@userUpdate

User endpoint to update a review comment on a question in a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**question_id** | **i32** | DAR application question id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::UpdateTeamDarApplicationQuestionReview200Response**](update_team_dar_application_question_review_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_user_dar_application_review

> models::UpdateTeamDarApplicationQuestionReview200Response update_user_dar_application_review(user_id, id, review_id, create_team_dar_application_review_request)
DataAccessApplicationReview@userUpdateGlobal

User endpoint to update a review comment on a DAR application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | User id | [required] |
**id** | **i32** | DAR application id | [required] |
**review_id** | **i32** | DAR application review id | [required] |
**create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md) | DataAccessApplicationReview definition | [required] |

### Return type

[**models::UpdateTeamDarApplicationQuestionReview200Response**](update_team_dar_application_question_review_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


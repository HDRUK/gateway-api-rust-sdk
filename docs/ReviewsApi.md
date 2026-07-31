# \ReviewsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_reviews**](ReviewsApi.md#create_reviews) | **POST** /api/v1/reviews | ReviewController@store
[**delete_reviews**](ReviewsApi.md#delete_reviews) | **DELETE** /api/v1/reviews/{id} | Delete a review
[**edit_reviews**](ReviewsApi.md#edit_reviews) | **PATCH** /api/v1/reviews/{id} | Edit a review
[**fetch_all_reviews**](ReviewsApi.md#fetch_all_reviews) | **GET** /api/v1/reviews | ReviewController@index
[**fetch_reviews**](ReviewsApi.md#fetch_reviews) | **GET** /api/v1/reviews/{id} | ReviewController@show
[**update_reviews**](ReviewsApi.md#update_reviews) | **PUT** /api/v1/reviews/{id} | Update a review



## create_reviews

> models::CreateCategories200Response create_reviews(create_reviews_request)
ReviewController@store

Create a new review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_reviews

> models::DeleteAliases200Response delete_reviews(id)
Delete a review

Delete a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_reviews

> models::UpdateReviews200Response edit_reviews(id, create_reviews_request)
Edit a review

Edit a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |
**create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateReviews200Response**](update_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_reviews

> models::FetchAllReviews200Response fetch_all_reviews()
ReviewController@index

Get All Reviews

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllReviews200Response**](fetch_all_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_reviews

> models::FetchAllReviews200Response fetch_reviews(id)
ReviewController@show

Get review by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |

### Return type

[**models::FetchAllReviews200Response**](fetch_all_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_reviews

> models::UpdateReviews200Response update_reviews(id, create_reviews_request)
Update a review

Update a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |
**create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateReviews200Response**](update_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


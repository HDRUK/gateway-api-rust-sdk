# \ReviewsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_reviews**](ReviewsApi.md#delete_reviews) | **DELETE** /api/v1/reviews/{id} | Delete a review
[**edit_reviews**](ReviewsApi.md#edit_reviews) | **PATCH** /api/v1/reviews/{id} | Edit a review
[**update_reviews**](ReviewsApi.md#update_reviews) | **PUT** /api/v1/reviews/{id} | Update a review



## delete_reviews

> models::DeleteApplications200Response delete_reviews(id)
Delete a review

Delete a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_reviews

> models::UpdateReviews200Response edit_reviews(id, update_reviews_request)
Edit a review

Edit a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |
**update_reviews_request** | [**UpdateReviewsRequest**](UpdateReviewsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateReviews200Response**](update_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_reviews

> models::UpdateReviews200Response update_reviews(id, update_reviews_request)
Update a review

Update a review

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | review id | [required] |
**update_reviews_request** | [**UpdateReviewsRequest**](UpdateReviewsRequest.md) | Pass user credentials | [required] |

### Return type

[**models::UpdateReviews200Response**](update_reviews_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


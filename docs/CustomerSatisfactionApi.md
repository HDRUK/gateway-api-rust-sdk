# \CustomerSatisfactionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_csat**](CustomerSatisfactionApi.md#create_csat) | **POST** /api/v1/csat | Create Customer Satisfaction Score
[**edit_csat**](CustomerSatisfactionApi.md#edit_csat) | **PATCH** /api/v1/csat/{id} | Update Customer Satisfaction Description



## create_csat

> models::DeleteApplications200Response create_csat(create_csat_request)
Create Customer Satisfaction Score

Creates a customer satisfaction score between 0 and 5

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_csat_request** | [**CreateCsatRequest**](CreateCsatRequest.md) | Customer Satisfaction score | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_csat

> models::EditCsat200Response edit_csat(id, edit_csat_request)
Update Customer Satisfaction Description

Update a description for a satisfaction score entry

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | ID of the CSAT entry | [required] |
**edit_csat_request** | [**EditCsatRequest**](EditCsatRequest.md) | Reason to update | [required] |

### Return type

[**models::EditCsat200Response**](edit_csat_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


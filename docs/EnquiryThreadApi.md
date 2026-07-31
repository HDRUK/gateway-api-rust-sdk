# \EnquiryThreadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_enquiry_threads**](EnquiryThreadApi.md#create_enquiry_threads) | **POST** /api/v1/enquiry_threads | EnquiryThread@store
[**fetch_all_enquiry_threads**](EnquiryThreadApi.md#fetch_all_enquiry_threads) | **GET** /api/v1/enquiry_threads | EnquiryThread@index
[**fetch_enquiry_threads**](EnquiryThreadApi.md#fetch_enquiry_threads) | **GET** /api/v1/enquiry_threads/{id} | EnquiryThread@show



## create_enquiry_threads

> models::CreateCategories200Response create_enquiry_threads(create_enquiry_threads_request)
EnquiryThread@store

Creates one or more new EnquiryThreads

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_enquiry_threads_request** | [**CreateEnquiryThreadsRequest**](CreateEnquiryThreadsRequest.md) | EnquiryThread definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_enquiry_threads

> models::FetchAllEnquiryThreads200Response fetch_all_enquiry_threads(per_page)
EnquiryThread@index

Returns a list of EnquiryThreads from the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**per_page** | Option<**i32**> | per page |  |

### Return type

[**models::FetchAllEnquiryThreads200Response**](fetch_all_enquiry_threads_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_enquiry_threads

> models::FetchAllEnquiryThreads200Response fetch_enquiry_threads(id)
EnquiryThread@show

Return a single EnquiryThread

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | EnquiryThread id | [required] |

### Return type

[**models::FetchAllEnquiryThreads200Response**](fetch_all_enquiry_threads_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


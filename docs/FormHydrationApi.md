# \FormHydrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_form_schema**](FormHydrationApi.md#get_form_schema) | **GET** /api/v1/form_hydration/schema | Retrieve form schema data
[**onboarding_form_hydration**](FormHydrationApi.md#onboarding_form_hydration) | **GET** /api/v1/form_hydration | Retrieve form schema data



## get_form_schema

> serde_json::Value get_form_schema(model, version)
Retrieve form schema data

Retrieves form schema data based on the provided model and version.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**model** | Option<**String**> | The model for which form schema is requested. |  |
**version** | Option<**String**> | The version of the model for which form schema is requested. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## onboarding_form_hydration

> serde_json::Value onboarding_form_hydration(name, version, data_types)
Retrieve form schema data

Retrieves form schema data based on the provided model and version.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | The model name for which form schema is requested. |  |
**version** | Option<**String**> | The version of the model for which form schema is requested. |  |
**data_types** | Option<**String**> | The data types of the dataset about to be onboarded. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


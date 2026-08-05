# \NotificationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_notifications**](NotificationApi.md#delete_notifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy



## delete_notifications

> models::DeleteApplications200Response delete_notifications(id)
Notification@destroy

Delete a notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | notification id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \NotificationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_notifications**](NotificationApi.md#create_notifications) | **POST** /api/v1/notifications | Notification@store
[**delete_notifications**](NotificationApi.md#delete_notifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy
[**edit_notifications**](NotificationApi.md#edit_notifications) | **PATCH** /api/v1/notifications/{id} | Notification@edit
[**fetch_all_notifications**](NotificationApi.md#fetch_all_notifications) | **GET** /api/v1/notifications | Notification@index
[**fetch_notifications**](NotificationApi.md#fetch_notifications) | **GET** /api/v1/notifications/{id} | Notification@show
[**update_notifications**](NotificationApi.md#update_notifications) | **PUT** /api/v1/notifications/{id} | Notification@update



## create_notifications

> models::CreateCategories200Response create_notifications(create_notifications_request)
Notification@store

Creates a new notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_notifications_request** | [**CreateNotificationsRequest**](CreateNotificationsRequest.md) | Notification definition | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_notifications

> models::DeleteAliases200Response delete_notifications(id)
Notification@destroy

Delete a notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | notification id | [required] |

### Return type

[**models::DeleteAliases200Response**](delete_aliases_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_notifications

> models::UpdateNotifications200Response edit_notifications(id, edit_notifications_request)
Notification@edit

Edit a notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | notification id | [required] |
**edit_notifications_request** | [**EditNotificationsRequest**](EditNotificationsRequest.md) | Notification definition | [required] |

### Return type

[**models::UpdateNotifications200Response**](update_notifications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_notifications

> models::FetchAllNotifications200Response fetch_all_notifications()
Notification@index

Returns a list of notifications enabled on the system

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::FetchAllNotifications200Response**](fetch_all_notifications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_notifications

> models::FetchNotifications200Response fetch_notifications(id)
Notification@show

Return a single notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | notification id | [required] |

### Return type

[**models::FetchNotifications200Response**](fetch_notifications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_notifications

> models::UpdateNotifications200Response update_notifications(id, create_notifications_request)
Notification@update

Update a notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | notification id | [required] |
**create_notifications_request** | [**CreateNotificationsRequest**](CreateNotificationsRequest.md) | Notification definition | [required] |

### Return type

[**models::UpdateNotifications200Response**](update_notifications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


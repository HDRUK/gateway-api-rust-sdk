# \UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_users**](UsersApi.md#create_users) | **POST** /api/v1/users | UserController@store
[**delete_users**](UsersApi.md#delete_users) | **DELETE** /api/v1/users/{id} | UserController@destroy
[**edit_users**](UsersApi.md#edit_users) | **PATCH** /api/v1/users/{id} | UserController@edit
[**verify_secondary_email**](UsersApi.md#verify_secondary_email) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user's secondary email using a UUID



## create_users

> models::CreateDarIntegration201Response create_users(create_users_request)
UserController@store

Create a new user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_users_request** | [**CreateUsersRequest**](CreateUsersRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_users

> models::DeleteFederation200Response delete_users(id)
UserController@destroy

Delete User based in id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | user id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_users

> models::EditUsers200Response edit_users(id, edit_users_request)
UserController@edit

Edit user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | user id | [required] |
**edit_users_request** | [**EditUsersRequest**](EditUsersRequest.md) | Pass user credentials | [required] |

### Return type

[**models::EditUsers200Response**](edit_users_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## verify_secondary_email

> models::VerifySecondaryEmail200Response verify_secondary_email(uuid)
Verify user's secondary email using a UUID

This endpoint verifies the secondary email for a user if the UUID is valid and not expired.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | Verification UUID | [required] |

### Return type

[**models::VerifySecondaryEmail200Response**](verify_secondary_email_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


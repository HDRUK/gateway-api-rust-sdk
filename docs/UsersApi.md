# \UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_users**](UsersApi.md#create_users) | **POST** /api/v1/users | UserController@store
[**delete_users**](UsersApi.md#delete_users) | **DELETE** /api/v1/users/{id} | UserController@destroy
[**edit_users**](UsersApi.md#edit_users) | **PATCH** /api/v1/users/{id} | UserController@edit
[**fetch_all_users**](UsersApi.md#fetch_all_users) | **GET** /api/v1/users | UserController@index
[**fetch_users**](UsersApi.md#fetch_users) | **GET** /api/v1/users/{id} | UserController@show
[**resend_secondary_verification_email**](UsersApi.md#resend_secondary_verification_email) | **POST** /api/v1/users/{id}/resend-secondary-verification | Resend secondary email verification
[**update_users**](UsersApi.md#update_users) | **PUT** /api/v1/users/{id} | UserController@update
[**verify_secondary_email**](UsersApi.md#verify_secondary_email) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user's secondary email using a UUID



## create_users

> models::CreateCategories200Response create_users(create_users_request)
UserController@store

Create a new user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_users_request** | [**CreateUsersRequest**](CreateUsersRequest.md) | Pass user credentials | [required] |

### Return type

[**models::CreateCategories200Response**](create_categories_200_response.md)

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

> models::FetchUsers200Response edit_users(id, update_users_request)
UserController@edit

Edit user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | user id | [required] |
**update_users_request** | [**UpdateUsersRequest**](UpdateUsersRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchUsers200Response**](fetch_users_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_users

> models::FetchAllUsers200Response fetch_all_users(filter_names)
UserController@index

Get All Users

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**filter_names** | Option<**String**> | Three or more characters to filter users names by |  |

### Return type

[**models::FetchAllUsers200Response**](fetch_all_users_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_users

> models::FetchUsers200Response fetch_users(id)
UserController@show

Get users by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | user id | [required] |

### Return type

[**models::FetchUsers200Response**](fetch_users_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## resend_secondary_verification_email

> models::ResendSecondaryVerificationEmail200Response resend_secondary_verification_email(id)
Resend secondary email verification

Resends the verification email for the secondary email address. Old tokens are expired.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | User ID | [required] |

### Return type

[**models::ResendSecondaryVerificationEmail200Response**](resendSecondaryVerificationEmail_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_users

> models::FetchUsers200Response update_users(id, update_users_request)
UserController@update

Update user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | user id | [required] |
**update_users_request** | [**UpdateUsersRequest**](UpdateUsersRequest.md) | Pass user credentials | [required] |

### Return type

[**models::FetchUsers200Response**](fetch_users_200_response.md)

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


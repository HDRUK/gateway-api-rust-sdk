# \UserRolesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_user_has_roles**](UserRolesApi.md#create_user_has_roles) | **POST** /api/v1/users/{userId}/roles | UserRoleController@store
[**delete_user_has_roles**](UserRolesApi.md#delete_user_has_roles) | **DELETE** /api/v1/users/{userId}/roles | UserRoleController@destroy
[**update_user_has_roles**](UserRolesApi.md#update_user_has_roles) | **PATCH** /api/v1/users/{userId}/roles | UserRoleController@edit



## create_user_has_roles

> models::DeleteApplications200Response create_user_has_roles(user_id, create_user_has_roles_request)
UserRoleController@store

Create user has roles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**create_user_has_roles_request** | [**CreateUserHasRolesRequest**](CreateUserHasRolesRequest.md) | Pass user credentials | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_user_has_roles

> models::DeleteFederation200Response delete_user_has_roles(user_id)
UserRoleController@destroy

Delete user - roles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |

### Return type

[**models::DeleteFederation200Response**](delete_federation_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_user_has_roles

> models::DeleteApplications200Response update_user_has_roles(user_id, update_user_has_roles_request)
UserRoleController@edit

Update user has roles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **i32** | user id | [required] |
**update_user_has_roles_request** | [**UpdateUserHasRolesRequest**](UpdateUserHasRolesRequest.md) | Pass user credentials | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


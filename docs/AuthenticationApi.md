# \AuthenticationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authentication**](AuthenticationApi.md#authentication) | **POST** /api/v1/auth | AuthController@checkAuthorization
[**login**](AuthenticationApi.md#login) | **POST** /api/v1/auth/login | AuthController@login
[**register**](AuthenticationApi.md#register) | **POST** /api/v1/auth/register | AuthController@register



## authentication

> models::Authentication200Response authentication(authentication_request)
AuthController@checkAuthorization

Generate Jwt based on email and password

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authentication_request** | [**AuthenticationRequest**](AuthenticationRequest.md) | Pass user credentials | [required] |

### Return type

[**models::Authentication200Response**](authentication_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## login

> models::Register200Response login(login_request)
AuthController@login

Login with email and password

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**login_request** | [**LoginRequest**](LoginRequest.md) | Pass user credentials | [required] |

### Return type

[**models::Register200Response**](register_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## register

> models::Register200Response register(register_request)
AuthController@register

Register a new user with email and password

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**register_request** | [**RegisterRequest**](RegisterRequest.md) | Pass user registration data | [required] |

### Return type

[**models::Register200Response**](register_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


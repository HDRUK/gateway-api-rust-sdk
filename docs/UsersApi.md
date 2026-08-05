# \UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**verify_secondary_email**](UsersApi.md#verify_secondary_email) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user's secondary email using a UUID



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


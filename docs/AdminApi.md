# \AdminApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**revoke_all_tokens_v2**](AdminApi.md#revoke_all_tokens_v2) | **POST** /api/v2/admin/tokens/revoke_all | TokenRevocationController@revokeAll



## revoke_all_tokens_v2

> models::RevokeAllTokensV2200Response revoke_all_tokens_v2()
TokenRevocationController@revokeAll

Revoke every Gateway JWT issued up to now, including the caller's own. All users must sign in again.

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::RevokeAllTokensV2200Response**](revoke_all_tokens_v2_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \QuestionBankApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_question_bank_question**](QuestionBankApi.md#create_question_bank_question) | **POST** /api/v1/questions | QuestionBank@store
[**delete_question_bank_question**](QuestionBankApi.md#delete_question_bank_question) | **DELETE** /api/v1/questions/{id} | QuestionBank@destroy
[**download_question_bank_question_file**](QuestionBankApi.md#download_question_bank_question_file) | **GET** /api/v1/questions/{id}/files/{fileId} | QuestionBank@destroyFile
[**edit_question_bank_question**](QuestionBankApi.md#edit_question_bank_question) | **PATCH** /api/v1/questions/{id} | QuestionBank@update
[**fetch_archived_question_bank_questions**](QuestionBankApi.md#fetch_archived_question_bank_questions) | **GET** /api/v1/questions/archived | QuestionBank@indexArchived
[**fetch_custom_question_bank_questions**](QuestionBankApi.md#fetch_custom_question_bank_questions) | **GET** /api/v1/questions/custom | QuestionBank@indexCustom
[**fetch_question_bank_question**](QuestionBankApi.md#fetch_question_bank_question) | **GET** /api/v1/questions/{id} | QuestionBank@show
[**fetch_question_bank_question_version**](QuestionBankApi.md#fetch_question_bank_question_version) | **GET** /api/v1/questions/version/{id} | QuestionBank@showVersion
[**fetch_question_bank_questions**](QuestionBankApi.md#fetch_question_bank_questions) | **GET** /api/v1/questions | QuestionBank@index
[**fetch_standard_question_bank_questions**](QuestionBankApi.md#fetch_standard_question_bank_questions) | **GET** /api/v1/questions/standard | QuestionBank@indexStandard
[**fetch_team_question_bank_questions_by_section**](QuestionBankApi.md#fetch_team_question_bank_questions_by_section) | **GET** /api/v1/teams/{teamId}/questions/section/{sectionId} | TeamQuestionBank@indexBySection
[**update_question_bank_question**](QuestionBankApi.md#update_question_bank_question) | **PUT** /api/v1/questions/{id} | QuestionBank@update
[**update_question_bank_question_status**](QuestionBankApi.md#update_question_bank_question_status) | **PATCH** /api/v1/questions/{id}/{status} | QuestionBank@updateStatus



## create_question_bank_question

> models::CreateDarIntegration201Response create_question_bank_question(create_question_bank_question_request)
QuestionBank@store

Create a new system question bank question with FE-helpful input format

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_question_bank_question_request** | [**CreateQuestionBankQuestionRequest**](CreateQuestionBankQuestionRequest.md) | QuestionBank definition | [required] |

### Return type

[**models::CreateDarIntegration201Response**](create_dar_integration_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_question_bank_question

> models::DeleteApplications200Response delete_question_bank_question(id)
QuestionBank@destroy

Delete a system question bank question

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## download_question_bank_question_file

> models::DeleteApplications200Response download_question_bank_question_file(id, file_id)
QuestionBank@destroyFile

Download a system question bank question

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |
**file_id** | **i32** | file uuid | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## edit_question_bank_question

> models::UpdateQuestionBankQuestion200Response edit_question_bank_question(id, edit_question_bank_question_request)
QuestionBank@update

Edit a system question bank question - use this for parents and children separately

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |
**edit_question_bank_question_request** | [**EditQuestionBankQuestionRequest**](EditQuestionBankQuestionRequest.md) | QuestionBank definition | [required] |

### Return type

[**models::UpdateQuestionBankQuestion200Response**](update_question_bank_question_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_archived_question_bank_questions

> models::FetchQuestionBankQuestions200Response fetch_archived_question_bank_questions(section_id, is_child, per_page, page)
QuestionBank@indexArchived

List of archived question bank questions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**section_id** | Option<**i32**> | section id |  |
**is_child** | Option<**i32**> | filter on is_child field |  |
**per_page** | Option<**i32**> | per page |  |
**page** | Option<**i32**> | page |  |

### Return type

[**models::FetchQuestionBankQuestions200Response**](fetch_question_bank_questions_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_custom_question_bank_questions

> models::FetchCustomQuestionBankQuestions200Response fetch_custom_question_bank_questions(section_id, is_child, per_page, page)
QuestionBank@indexCustom

List of custom question bank questions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**section_id** | Option<**i32**> | section id |  |
**is_child** | Option<**i32**> | filter on is_child field |  |
**per_page** | Option<**i32**> | per page |  |
**page** | Option<**i32**> | page |  |

### Return type

[**models::FetchCustomQuestionBankQuestions200Response**](fetch_custom_question_bank_questions_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_question_bank_question

> models::FetchQuestionBankQuestion200Response fetch_question_bank_question(id)
QuestionBank@show

Return the latest question bank question version for the supplied question id, in an FE-friendly format

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |

### Return type

[**models::FetchQuestionBankQuestion200Response**](fetch_question_bank_question_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_question_bank_question_version

> models::FetchQuestionBankQuestionVersion200Response fetch_question_bank_question_version(id)
QuestionBank@showVersion

Return a single system question bank question version

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question version id | [required] |

### Return type

[**models::FetchQuestionBankQuestionVersion200Response**](fetch_question_bank_question_version_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_question_bank_questions

> models::FetchQuestionBankQuestions200Response fetch_question_bank_questions(section_id, is_child, per_page, page)
QuestionBank@index

List of question bank questions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**section_id** | Option<**i32**> | section id |  |
**is_child** | Option<**i32**> | filter on is_child field |  |
**per_page** | Option<**i32**> | per page |  |
**page** | Option<**i32**> | page |  |

### Return type

[**models::FetchQuestionBankQuestions200Response**](fetch_question_bank_questions_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_standard_question_bank_questions

> models::FetchStandardQuestionBankQuestions200Response fetch_standard_question_bank_questions(section_id, is_child, per_page, page)
QuestionBank@indexStandard

List of standard question bank questions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**section_id** | Option<**i32**> | section id |  |
**is_child** | Option<**i32**> | filter on is_child field |  |
**per_page** | Option<**i32**> | per page |  |
**page** | Option<**i32**> | page |  |

### Return type

[**models::FetchStandardQuestionBankQuestions200Response**](fetch_standard_question_bank_questions_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_team_question_bank_questions_by_section

> models::FetchTeamQuestionBankQuestionsBySection200Response fetch_team_question_bank_questions_by_section(team_id, section_id, is_child)
TeamQuestionBank@indexBySection

List of question bank questions by section

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**section_id** | **i32** | section id | [required] |
**is_child** | Option<**i32**> | filter on is_child field |  |

### Return type

[**models::FetchTeamQuestionBankQuestionsBySection200Response**](fetch_team_question_bank_questions_by_section_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_question_bank_question

> models::UpdateQuestionBankQuestion200Response update_question_bank_question(id, update_question_bank_question_request)
QuestionBank@update

Update a system question bank question - children and their versions are updated through parents

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |
**update_question_bank_question_request** | [**UpdateQuestionBankQuestionRequest**](UpdateQuestionBankQuestionRequest.md) | QuestionBank definition | [required] |

### Return type

[**models::UpdateQuestionBankQuestion200Response**](update_question_bank_question_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_question_bank_question_status

> models::UpdateQuestionBankQuestionStatus200Response update_question_bank_question_status(id, status)
QuestionBank@updateStatus

Lock, unlock, archive or unarchive a question bank question

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | question bank question id | [required] |
**status** | **String** | lock or unlock | [required] |

### Return type

[**models::UpdateQuestionBankQuestionStatus200Response**](update_question_bank_question_status_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


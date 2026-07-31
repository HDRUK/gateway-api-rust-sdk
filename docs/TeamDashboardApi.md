# \TeamDashboardApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_collections_views_v3**](TeamDashboardApi.md#fetch_collections_views_v3) | **GET** /api/v3/teams/{id}/dashboard/collections/views | TeamDashboardController@collectionViews
[**fetch_dar_applications_application_timeline_v3**](TeamDashboardApi.md#fetch_dar_applications_application_timeline_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline | DataAccessDashboardController@getApplicationTimeline
[**fetch_dar_applications_average_time_to_approval_v3**](TeamDashboardApi.md#fetch_dar_applications_average_time_to_approval_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/average-time | DataAccessDashboardController@getAverageTimeToApproval
[**fetch_dar_applications_current_status_v3**](TeamDashboardApi.md#fetch_dar_applications_current_status_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/status | DataAccessDashboardController@getApplicationStatus
[**fetch_dar_applications_dashboard_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/export/csv | DataAccessDashboardController@exportDashboardCsv
[**fetch_dar_applications_dashboard_required_actions_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_required_actions_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions/export/csv | DataAccessDashboardController@exportRequiredActionsCsv
[**fetch_dar_applications_dashboard_timeline_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_timeline_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline/export/csv | DataAccessDashboardController@exportDashboardTimelineCsv
[**fetch_dar_applications_required_actions_v3**](TeamDashboardApi.md#fetch_dar_applications_required_actions_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions | DataAccessDashboardController@getRequiredActions
[**fetch_dar_my_applications_v3**](TeamDashboardApi.md#fetch_dar_my_applications_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/count | DataAccessDashboardController@getMyApplications
[**fetch_dashboard_download_csv_v3**](TeamDashboardApi.md#fetch_dashboard_download_csv_v3) | **GET** /api/v3/teams/{id}/dashboard/download/csv | TeamDashboardController@downloadCsv
[**fetch_data_custodians_views_v3**](TeamDashboardApi.md#fetch_data_custodians_views_v3) | **GET** /api/v3/teams/{id}/dashboard/datacustodians/views | TeamDashboardController@datacustodianViews
[**fetch_dataset_views360_v3**](TeamDashboardApi.md#fetch_dataset_views360_v3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/360 | TeamDashboardController@datasetViews360
[**fetch_dataset_views_top_v3**](TeamDashboardApi.md#fetch_dataset_views_top_v3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/top | TeamDashboardController@datasetViewsTop
[**fetch_entities_count_v3**](TeamDashboardApi.md#fetch_entities_count_v3) | **GET** /api/v3/teams/{id}/dashboard/{entity}/count | TeamDashboardController@entityCount



## fetch_collections_views_v3

> models::FetchCollectionsViewsV3200Response fetch_collections_views_v3(id, start_date, end_date)
TeamDashboardController@collectionViews

Get count of a collection views for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::FetchCollectionsViewsV3200Response**](fetch_collections_views_v3_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_application_timeline_v3

> models::CreateWidget201Response fetch_dar_applications_application_timeline_v3(id, start_date, end_date)
DataAccessDashboardController@getApplicationTimeline

Get Dar applications timeline for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_average_time_to_approval_v3

> models::CreateWidget201Response fetch_dar_applications_average_time_to_approval_v3(id, start_date, end_date)
DataAccessDashboardController@getAverageTimeToApproval

Get Dar applications average time to approval for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_current_status_v3

> models::CreateWidget201Response fetch_dar_applications_current_status_v3(id, start_date, end_date)
DataAccessDashboardController@getApplicationStatus

Get Dar applications current status for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_dashboard_export_csv_v3

> models::CreateWidget201Response fetch_dar_applications_dashboard_export_csv_v3(id, start_date, end_date)
DataAccessDashboardController@exportDashboardCsv

Get Dar applications dashboard export csv for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_dashboard_required_actions_export_csv_v3

> models::CreateWidget201Response fetch_dar_applications_dashboard_required_actions_export_csv_v3(id)
DataAccessDashboardController@exportRequiredActionsCsv

Get Dar applications dashboard timeline export csv for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_dashboard_timeline_export_csv_v3

> models::CreateWidget201Response fetch_dar_applications_dashboard_timeline_export_csv_v3(id, start_date, end_date)
DataAccessDashboardController@exportDashboardTimelineCsv

Get Dar applications dashboard timeline export csv for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_applications_required_actions_v3

> models::CreateWidget201Response fetch_dar_applications_required_actions_v3(id, start_date, end_date)
DataAccessDashboardController@getRequiredActions

Get Dar applications required actions for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dar_my_applications_v3

> models::CreateWidget201Response fetch_dar_my_applications_v3(id, start_date, end_date)
DataAccessDashboardController@getMyApplications

Get Dar applications for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dashboard_download_csv_v3

> std::path::PathBuf fetch_dashboard_download_csv_v3(id, start_date, end_date)
TeamDashboardController@downloadCsv

Download dashboard data custodian in csv format

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_data_custodians_views_v3

> models::FetchCollectionsViewsV3200Response fetch_data_custodians_views_v3(id, start_date, end_date)
TeamDashboardController@datacustodianViews

Get count of a data custodian views for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::FetchCollectionsViewsV3200Response**](fetch_collections_views_v3_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dataset_views360_v3

> models::FetchDatasetViews360V3200Response fetch_dataset_views360_v3(id, start_date, end_date)
TeamDashboardController@datasetViews360

Get count of a datasets views 360 for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::FetchDatasetViews360V3200Response**](fetch_dataset_views_360_v3_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_dataset_views_top_v3

> models::FetchDatasetViewsTopV3200Response fetch_dataset_views_top_v3(id, start_date, end_date)
TeamDashboardController@datasetViewsTop

Get count of a datasets views top for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::FetchDatasetViewsTopV3200Response**](fetch_dataset_views_top_v3_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_entities_count_v3

> models::FetchEntitiesCountV3200Response fetch_entities_count_v3(id, entity, start_date, end_date)
TeamDashboardController@entityCount

Get count of a specific entity for a team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i32** | Team ID | [required] |
**entity** | **String** | Entity type to count | [required] |
**start_date** | Option<**chrono::NaiveDate**> | Start date for the reporting interval (Y-m-d). Defaults to one year ago. |  |
**end_date** | Option<**chrono::NaiveDate**> | End date for the reporting interval (Y-m-d). Defaults to today. |  |

### Return type

[**models::FetchEntitiesCountV3200Response**](fetch_entities_count_v3_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


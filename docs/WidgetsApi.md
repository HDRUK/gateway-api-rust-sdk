# \WidgetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_widget**](WidgetsApi.md#create_widget) | **POST** /api/v1/teams/{teamId}/widgets | Create a new widget
[**delete_widget**](WidgetsApi.md#delete_widget) | **DELETE** /api/v1/teams/{teamId}/widgets/{id} | Delete a widget
[**fetch_all_widgets**](WidgetsApi.md#fetch_all_widgets) | **GET** /api/v1/teams/{teamId}/widgets | WidgetController@index
[**fetch_widget**](WidgetsApi.md#fetch_widget) | **GET** /api/v1/teams/{teamId}/widgets/{id} | WidgetController@retrieve
[**fetch_widget_data_sources**](WidgetsApi.md#fetch_widget_data_sources) | **GET** /api/v1/teams/{teamId}/widgets/data | WidgetController@getWidgetData
[**retrieve_widget_data**](WidgetsApi.md#retrieve_widget_data) | **GET** /api/v1/teams/{teamId}/widgets/{id}/data | Retrieve data related to a widget
[**track_widget_event**](WidgetsApi.md#track_widget_event) | **POST** /api/v1/teams/{teamId}/widgets/{id}/track | Record a widget analytics event
[**update_widget**](WidgetsApi.md#update_widget) | **PATCH** /api/v1/teams/{teamId}/widgets/{id} | Update an existing widget
[**widget_analytics**](WidgetsApi.md#widget_analytics) | **GET** /api/v1/teams/{teamId}/widgets/analytics | Get widget analytics for a team



## create_widget

> models::CreateWidget201Response create_widget(team_id, create_widget_request)
Create a new widget

Creates a new widget for a given team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID the widget belongs to | [required] |
**create_widget_request** | [**CreateWidgetRequest**](CreateWidgetRequest.md) |  | [required] |

### Return type

[**models::CreateWidget201Response**](create_widget_201_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_widget

> models::DeleteApplications200Response delete_widget(team_id, id)
Delete a widget

Soft delete a widget belonging to a specific team

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**id** | **i32** | Widget ID | [required] |

### Return type

[**models::DeleteApplications200Response**](delete_applications_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_all_widgets

> models::FetchAllWidgets200Response fetch_all_widgets(team_id)
WidgetController@index

Get All Widgets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |

### Return type

[**models::FetchAllWidgets200Response**](fetch_all_widgets_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_widget

> models::FetchWidget200Response fetch_widget(team_id, id)
WidgetController@retrieve

Get a single Widget

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**id** | **i32** | Widget ID | [required] |

### Return type

[**models::FetchWidget200Response**](fetch_widget_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fetch_widget_data_sources

> models::FetchWidgetDataSources200Response fetch_widget_data_sources(team_id, team_ids)
WidgetController@getWidgetData

Fetch lightweight data (id, name, etc.) for multiple teams across datasets, tools, collections, and DURS

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**team_ids** | **String** | Comma-separated list of team IDs to filter data | [required] |

### Return type

[**models::FetchWidgetDataSources200Response**](fetch_widget_data_sources_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## retrieve_widget_data

> models::RetrieveWidgetData200Response retrieve_widget_data(team_id, id, domain_origin)
Retrieve data related to a widget

Fetches datasets, data uses, scripts, and collections linked to a widget

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**id** | **i32** | Widget ID | [required] |
**domain_origin** | **String** | Optional domain URL to check against the widget's permitted_domains list | [required] |

### Return type

[**models::RetrieveWidgetData200Response**](retrieve_widget_data_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## track_widget_event

> track_widget_event(team_id, id, track_widget_event_request)
Record a widget analytics event

Public endpoint for frontend clients to record user interactions with a widget (page views, code copies, gateway clicks, searches). No authentication required.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** |  | [required] |
**id** | **i32** |  | [required] |
**track_widget_event_request** | [**TrackWidgetEventRequest**](TrackWidgetEventRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_widget

> models::UpdateWidget200Response update_widget(team_id, id, update_widget_request)
Update an existing widget

Updates an existing widget for a given team ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** | Team ID | [required] |
**id** | **i32** | Widget ID | [required] |
**update_widget_request** | Option<[**UpdateWidgetRequest**](UpdateWidgetRequest.md)> |  |  |

### Return type

[**models::UpdateWidget200Response**](update_widget_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## widget_analytics

> models::WidgetAnalytics200Response widget_analytics(team_id, from, to, group_by)
Get widget analytics for a team

Returns aggregated event counts per widget, per event type, and over time. Supports date range filtering and time-based grouping.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**team_id** | **i32** |  | [required] |
**from** | Option<**String**> | Start date (Y-m-d) |  |
**to** | Option<**String**> | End date (Y-m-d) |  |
**group_by** | Option<**String**> | Time granularity |  |[default to day]

### Return type

[**models::WidgetAnalytics200Response**](widget_analytics_200_response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


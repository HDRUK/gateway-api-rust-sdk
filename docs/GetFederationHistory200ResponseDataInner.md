# GetFederationHistory200ResponseDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_uuid** | Option<**String**> |  | [optional]
**started_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**finished_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**status** | Option<**Status**> |  (enum: success, failed, in_progress) | [optional]
**message** | Option<**String**> |  | [optional]
**failed_datasets** | Option<[**Vec<models::GetFederationHistory200ResponseDataInnerFailedDatasetsInner>**](GetFederationHistory200ResponseDataInnerFailedDatasetsInner.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



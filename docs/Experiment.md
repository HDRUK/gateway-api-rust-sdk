# Experiment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**i32**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**status** | Option<**Status**> |  (enum: draft, active, paused, archived) | [optional]
**definition** | Option<[**models::ExperimentDefinition**](ExperimentDefinition.md)> |  | [optional]
**targeting** | Option<[**models::ExperimentTargeting**](ExperimentTargeting.md)> |  | [optional]
**trigger** | Option<[**models::ExperimentTrigger**](ExperimentTrigger.md)> |  | [optional]
**starts_at** | Option<**chrono::NaiveDate**> |  | [optional]
**ends_at** | Option<**chrono::NaiveDate**> |  | [optional]
**created_by** | Option<**i32**> |  | [optional]
**responses_count** | Option<**i32**> |  | [optional]
**created_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**updated_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**deleted_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



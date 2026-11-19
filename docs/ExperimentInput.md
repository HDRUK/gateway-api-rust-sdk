# ExperimentInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** |  | 
**status** | **Status** |  (enum: draft, active, paused, archived) | 
**definition** | **serde_json::Value** | See Experiment.definition | 
**targeting** | **serde_json::Value** | See Experiment.targeting | 
**trigger** | **serde_json::Value** | See Experiment.trigger | 
**starts_at** | Option<**chrono::NaiveDate**> |  | [optional]
**ends_at** | Option<**chrono::NaiveDate**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



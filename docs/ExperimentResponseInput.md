# ExperimentResponseInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**answers** | **serde_json::Value** | Answers keyed by question block id; unknown ids are dropped | 
**path** | **String** |  | 
**variant** | Option<**String**> |  | [optional]
**contact** | Option<**bool**> |  | [optional]
**email** | Option<**String**> | Required when contact is true and not signed in | [optional]
**recaptcha** | **String** | reCAPTCHA v3 token for the experiment_response action | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



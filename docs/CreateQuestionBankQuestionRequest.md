# CreateQuestionBankQuestionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **i32** |  | 
**user_id** | Option<**i32**> |  | [optional]
**team_ids** | Option<**Vec<i32>**> |  | [optional]
**locked** | Option<**bool**> |  | [optional]
**archived** | Option<**bool**> |  | [optional]
**required** | Option<**bool**> |  | [optional]
**force_required** | **bool** |  | 
**allow_guidance_override** | **bool** |  | 
**default** | Option<**bool**> |  | [optional]
**guidance** | **String** |  | 
**title** | **String** |  | 
**field** | **Vec<serde_json::Value>** |  | 
**component** | **String** |  | 
**validations** | **Vec<serde_json::Value>** |  | 
**options** | [**Vec<models::CreateQuestionBankQuestionRequestOptionsInner>**](CreateQuestionBankQuestionRequestOptionsInner.md) |  | 
**is_child** | Option<**bool**> |  | [optional]
**question_type** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



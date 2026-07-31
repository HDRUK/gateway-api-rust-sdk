# CreateToolsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> |  | [optional]
**url** | Option<**String**> |  | [optional]
**description** | Option<**String**> |  | [optional]
**results_insights** | Option<**String**> |  | [optional]
**license** | Option<**i32**> |  | [optional]
**tech_stack** | Option<**String**> |  | [optional]
**category_id** | Option<**i32**> |  | [optional]
**user_id** | Option<**i32**> |  | [optional]
**team_id** | Option<**i32**> |  | [optional]
**tags** | Option<**Vec<i64>**> |  | [optional]
**dataset** | Option<[**Vec<models::CreateToolsIntegrationsRequestDatasetInner>**](CreateToolsIntegrationsRequestDatasetInner.md)> |  | [optional]
**enabled** | Option<**i32**> |  | [optional]
**programming_language** | Option<**Vec<i64>**> |  | [optional]
**programming_package** | Option<**Vec<i64>**> |  | [optional]
**type_category** | Option<**Vec<i64>**> |  | [optional]
**associated_authors** | Option<**String**> |  | [optional]
**contact_address** | Option<**String**> |  | [optional]
**publications** | Option<[**Vec<models::CreateToolsIntegrationsRequestPublicationsInner>**](CreateToolsIntegrationsRequestPublicationsInner.md)> |  | [optional]
**durs** | Option<**Vec<i64>**> |  | [optional]
**collections** | Option<[**Vec<models::CreateToolsRequestCollectionsInner>**](CreateToolsRequestCollectionsInner.md)> |  | [optional]
**any_dataset** | Option<**bool**> |  | [optional]
**status** | Option<**Status**> |  (enum: ACTIVE, DRAFT, ARCHIVED) | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



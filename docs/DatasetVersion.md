# DatasetVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**i32**> |  | [optional]
**dataset_id** | Option<**i32**> |  | [optional]
**version** | Option<**i32**> |  | [optional]
**title** | Option<**String**> |  | [optional]
**short_title** | Option<**String**> |  | [optional]
**metadata** | Option<**serde_json::Value**> | Full GWDM-format metadata document for this version | [optional]
**patch** | Option<**Vec<serde_json::Value>**> | RFC 6902 JSON Patch array used to reconstruct this version from the previous snapshot. Null for full snapshots (v1 and every 10th version). | [optional]
**created_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**updated_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



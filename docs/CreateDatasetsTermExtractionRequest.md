# CreateDatasetsTermExtractionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partial** | Option<**bool**> | Flag to determine if term extraction should be partial (true) or full (false) | [optional][default to true]
**min_id** | Option<**i32**> | Minimum dataset ID to include in the term extraction | [optional][default to 1]
**max_id** | Option<**i32**> | Maximum dataset ID to include in the term extraction. Defaults to the maximum dataset ID available. | [optional]
**index_elastic** | Option<**bool**> | Flag to determine if data should be indexed in Elasticsearch | [optional][default to true]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



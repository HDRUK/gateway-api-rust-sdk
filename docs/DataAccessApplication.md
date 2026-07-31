# DataAccessApplication

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**i32**> |  | [optional]
**applicant_id** | Option<**i32**> |  | [optional]
**project_title** | Option<**String**> |  | [optional]
**project_id** | Option<**String**> |  | [optional]
**application_type** | Option<**String**> |  | [optional]
**submission_status** | Option<**SubmissionStatus**> |  (enum: DRAFT, SUBMITTED, FEEDBACK) | [optional]
**approval_status** | Option<**ApprovalStatus**> |  (enum: APPROVED, APPROVED_COMMENTS, REJECTED, WITHDRAWN) | [optional]
**is_joint** | Option<**bool**> |  | [optional]
**status_review_id** | Option<**i32**> |  | [optional]
**created_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**updated_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]
**deleted_at** | Option<**chrono::DateTime<chrono::FixedOffset>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



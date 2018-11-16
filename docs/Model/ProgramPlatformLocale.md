# ProgramPlatformLocale

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id_program** | **string** | Program identifier | 
**id_platform** | **string** | Platform identifier | 
**id_locale** | **string** | Locale identifier | 
**legal_advisory** | **string** | Type of legal advisory. | [optional] [default to 'AUTO']
**legal_note** | **string** | Legal note, in case the advisory type is MANUAL. It can be up to 65535 bytes. | [optional] 
**dont_allow_download** | **bool** | If true no download button should be shown | [optional] [default to false]
**force_external_download** | **bool** | If the download for the program is forced to external | [optional] [default to false]
**is_sales_client** | **bool** | This program pays in some way to the company, affects compliance rules | [optional] [default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



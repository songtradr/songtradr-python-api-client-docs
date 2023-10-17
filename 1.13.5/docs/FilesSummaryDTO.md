# FilesSummaryDTO

Summary of content of files

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_details_summary** | [**List[FieldSummaryDTO]**](FieldSummaryDTO.md) |  | [optional] 
**genre_summary** | [**List[GenresSummaryDTO]**](GenresSummaryDTO.md) |  | [optional] 
**tag_summary** | [**List[TagsSummaryDTO]**](TagsSummaryDTO.md) |  | [optional] 
**musical_features_summary** | [**List[FieldSummaryDTO]**](FieldSummaryDTO.md) |  | [optional] 
**total_files** | **int** |  | 
**bpm_min** | **float** |  | [optional] 
**bpm_max** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FilesSummaryDTO from a JSON string
files_summary_dto_instance = FilesSummaryDTO.from_json(json)
# print the JSON string representation of the object
print FilesSummaryDTO.to_json()

# convert the object into a dict
files_summary_dto_dict = files_summary_dto_instance.to_dict()
# create an instance of FilesSummaryDTO from a dict
files_summary_dto_form_dict = files_summary_dto.from_dict(files_summary_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



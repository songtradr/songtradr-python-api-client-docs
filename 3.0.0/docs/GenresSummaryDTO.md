# GenresSummaryDTO

Summary of genres occuring in files.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**total** | **int** |  | 
**genre_type** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.genres_summary_dto import GenresSummaryDTO

# TODO update the JSON string below
json = "{}"
# create an instance of GenresSummaryDTO from a JSON string
genres_summary_dto_instance = GenresSummaryDTO.from_json(json)
# print the JSON string representation of the object
print(GenresSummaryDTO.to_json())

# convert the object into a dict
genres_summary_dto_dict = genres_summary_dto_instance.to_dict()
# create an instance of GenresSummaryDTO from a dict
genres_summary_dto_from_dict = GenresSummaryDTO.from_dict(genres_summary_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



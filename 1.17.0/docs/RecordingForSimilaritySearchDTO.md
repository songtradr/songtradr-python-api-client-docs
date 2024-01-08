# RecordingForSimilaritySearchDTO

List of recordings with with a mid-sized field set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recording** | [**RecordingSmallDTO**](RecordingSmallDTO.md) |  | 
**score** | **float** |  | 

## Example

```python
from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingForSimilaritySearchDTO from a JSON string
recording_for_similarity_search_dto_instance = RecordingForSimilaritySearchDTO.from_json(json)
# print the JSON string representation of the object
print RecordingForSimilaritySearchDTO.to_json()

# convert the object into a dict
recording_for_similarity_search_dto_dict = recording_for_similarity_search_dto_instance.to_dict()
# create an instance of RecordingForSimilaritySearchDTO from a dict
recording_for_similarity_search_dto_form_dict = recording_for_similarity_search_dto.from_dict(recording_for_similarity_search_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# RecordingListDTO

List of recordings with with a mid-sized field set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recordings** | [**List[RecordingMediumDTO]**](RecordingMediumDTO.md) |  | 
**has_next_page** | **bool** |  | 
**current_page_number** | **int** |  | 
**total_results** | **int** |  | 

## Example

```python
from songtradr_api_client_python.models.recording_list_dto import RecordingListDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingListDTO from a JSON string
recording_list_dto_instance = RecordingListDTO.from_json(json)
# print the JSON string representation of the object
print RecordingListDTO.to_json()

# convert the object into a dict
recording_list_dto_dict = recording_list_dto_instance.to_dict()
# create an instance of RecordingListDTO from a dict
recording_list_dto_form_dict = recording_list_dto.from_dict(recording_list_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



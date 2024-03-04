# RecordingGenrePredictionDTO

AI-predicted Genres for a recording

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**genre_type** | **str** |  | 
**genre** | [**GenreMinimalDTO**](GenreMinimalDTO.md) |  | 
**probability** | **float** |  | 

## Example

```python
from songtradr_api_client_python.models.recording_genre_prediction_dto import RecordingGenrePredictionDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingGenrePredictionDTO from a JSON string
recording_genre_prediction_dto_instance = RecordingGenrePredictionDTO.from_json(json)
# print the JSON string representation of the object
print(RecordingGenrePredictionDTO.to_json())

# convert the object into a dict
recording_genre_prediction_dto_dict = recording_genre_prediction_dto_instance.to_dict()
# create an instance of RecordingGenrePredictionDTO from a dict
recording_genre_prediction_dto_form_dict = recording_genre_prediction_dto.from_dict(recording_genre_prediction_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



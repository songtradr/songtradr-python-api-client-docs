# RecordingMediumDTO

Recording with a mid-sized field set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**isrc** | **str** |  | 
**recording_party_entities** | [**List[RecordingPartyDTO]**](RecordingPartyDTO.md) |  | [optional] 
**genres** | [**List[GenreDTO]**](GenreDTO.md) |  | [optional] 
**language_of_performance** | **str** |  | [optional] 
**release_date** | **datetime** |  | [optional] 
**titles** | [**List[TitleDTO]**](TitleDTO.md) |  | [optional] 
**tracks** | [**List[TrackDTO]**](TrackDTO.md) |  | [optional] 
**musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] 
**spotify_id** | **str** |  | [optional] 
**tags** | [**List[RecordingTagSmallDTO]**](RecordingTagSmallDTO.md) |  | [optional] 
**genre_predictions** | [**List[RecordingGenrePredictionDTO]**](RecordingGenrePredictionDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingMediumDTO from a JSON string
recording_medium_dto_instance = RecordingMediumDTO.from_json(json)
# print the JSON string representation of the object
print(RecordingMediumDTO.to_json())

# convert the object into a dict
recording_medium_dto_dict = recording_medium_dto_instance.to_dict()
# create an instance of RecordingMediumDTO from a dict
recording_medium_dto_from_dict = RecordingMediumDTO.from_dict(recording_medium_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



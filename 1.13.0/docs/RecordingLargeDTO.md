# RecordingLargeDTO

Recording with a large field set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**duration** | **int** |  | [optional] 
**parties** | [**List[RecordingPartyDTO]**](RecordingPartyDTO.md) |  | [optional] 
**genres** | [**List[GenreDTO]**](GenreDTO.md) |  | [optional] 
**language_of_performance** | **str** |  | [optional] 
**titles** | [**List[TitleDTO]**](TitleDTO.md) |  | [optional] 
**tracks** | [**List[TrackToMediumProductDTO]**](TrackToMediumProductDTO.md) |  | [optional] 
**musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] 
**isrc** | **str** |  | 
**tags** | [**List[RecordingTagSmallDTO]**](RecordingTagSmallDTO.md) |  | [optional] 
**spotify_id** | **str** |  | [optional] 
**pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] 
**genre_predictions** | [**List[RecordingGenrePredictionDTO]**](RecordingGenrePredictionDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_large_dto import RecordingLargeDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingLargeDTO from a JSON string
recording_large_dto_instance = RecordingLargeDTO.from_json(json)
# print the JSON string representation of the object
print RecordingLargeDTO.to_json()

# convert the object into a dict
recording_large_dto_dict = recording_large_dto_instance.to_dict()
# create an instance of RecordingLargeDTO from a dict
recording_large_dto_form_dict = recording_large_dto.from_dict(recording_large_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



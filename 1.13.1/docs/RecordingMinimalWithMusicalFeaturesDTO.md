# RecordingMinimalWithMusicalFeaturesDTO

Recording in its minimal form, but with AI-predicted musical features.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**musical_features** | [**List[MusicalFeaturesDTO]**](MusicalFeaturesDTO.md) |  | [optional] 
**isrc** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.recording_minimal_with_musical_features_dto import RecordingMinimalWithMusicalFeaturesDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingMinimalWithMusicalFeaturesDTO from a JSON string
recording_minimal_with_musical_features_dto_instance = RecordingMinimalWithMusicalFeaturesDTO.from_json(json)
# print the JSON string representation of the object
print RecordingMinimalWithMusicalFeaturesDTO.to_json()

# convert the object into a dict
recording_minimal_with_musical_features_dto_dict = recording_minimal_with_musical_features_dto_instance.to_dict()
# create an instance of RecordingMinimalWithMusicalFeaturesDTO from a dict
recording_minimal_with_musical_features_dto_form_dict = recording_minimal_with_musical_features_dto.from_dict(recording_minimal_with_musical_features_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



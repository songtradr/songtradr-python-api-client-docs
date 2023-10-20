# SaveRecordingPartyDTO

Recording-party-connection to be saved the API.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_name** | **str** |  | 
**contributor_type** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.save_recording_party_dto import SaveRecordingPartyDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveRecordingPartyDTO from a JSON string
save_recording_party_dto_instance = SaveRecordingPartyDTO.from_json(json)
# print the JSON string representation of the object
print SaveRecordingPartyDTO.to_json()

# convert the object into a dict
save_recording_party_dto_dict = save_recording_party_dto_instance.to_dict()
# create an instance of SaveRecordingPartyDTO from a dict
save_recording_party_dto_form_dict = save_recording_party_dto.from_dict(save_recording_party_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



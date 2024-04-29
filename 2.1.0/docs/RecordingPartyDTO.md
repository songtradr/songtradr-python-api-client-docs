# RecordingPartyDTO

Party (person, group or organization) that contributed to a recording.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**party** | [**PartySmallDTO**](PartySmallDTO.md) |  | 
**contributor_types** | [**List[ContributorTypeDTO]**](ContributorTypeDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingPartyDTO from a JSON string
recording_party_dto_instance = RecordingPartyDTO.from_json(json)
# print the JSON string representation of the object
print(RecordingPartyDTO.to_json())

# convert the object into a dict
recording_party_dto_dict = recording_party_dto_instance.to_dict()
# create an instance of RecordingPartyDTO from a dict
recording_party_dto_from_dict = RecordingPartyDTO.from_dict(recording_party_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PartySmallDTO

Party (person, group or organization) with a small field-set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**full_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.party_small_dto import PartySmallDTO

# TODO update the JSON string below
json = "{}"
# create an instance of PartySmallDTO from a JSON string
party_small_dto_instance = PartySmallDTO.from_json(json)
# print the JSON string representation of the object
print PartySmallDTO.to_json()

# convert the object into a dict
party_small_dto_dict = party_small_dto_instance.to_dict()
# create an instance of PartySmallDTO from a dict
party_small_dto_form_dict = party_small_dto.from_dict(party_small_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



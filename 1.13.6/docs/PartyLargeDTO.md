# PartyLargeDTO

Party (person, group or organization) with a large field-set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_name** | **str** |  | 
**birth_date** | **str** |  | [optional] 
**death_date** | **str** |  | [optional] 
**birth_year** | **str** |  | [optional] 
**death_year** | **str** |  | [optional] 
**birth_place** | **str** |  | [optional] 
**musicbrainz_type** | **str** |  | [optional] 
**area** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.party_large_dto import PartyLargeDTO

# TODO update the JSON string below
json = "{}"
# create an instance of PartyLargeDTO from a JSON string
party_large_dto_instance = PartyLargeDTO.from_json(json)
# print the JSON string representation of the object
print PartyLargeDTO.to_json()

# convert the object into a dict
party_large_dto_dict = party_large_dto_instance.to_dict()
# create an instance of PartyLargeDTO from a dict
party_large_dto_form_dict = party_large_dto.from_dict(party_large_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



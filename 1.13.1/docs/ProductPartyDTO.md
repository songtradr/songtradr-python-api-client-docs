# ProductPartyDTO

Parties (persons, groups or organizations) that have contributed to a product.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contributor_types** | [**List[ContributorTypeDTO]**](ContributorTypeDTO.md) |  | [optional] 
**party** | [**PartySmallDTO**](PartySmallDTO.md) |  | 

## Example

```python
from songtradr_api_client_python.models.product_party_dto import ProductPartyDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ProductPartyDTO from a JSON string
product_party_dto_instance = ProductPartyDTO.from_json(json)
# print the JSON string representation of the object
print ProductPartyDTO.to_json()

# convert the object into a dict
product_party_dto_dict = product_party_dto_instance.to_dict()
# create an instance of ProductPartyDTO from a dict
product_party_dto_form_dict = product_party_dto.from_dict(product_party_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



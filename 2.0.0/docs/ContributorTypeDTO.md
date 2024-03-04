# ContributorTypeDTO

A type of contribution a party (person, group or organization) had on a recording or product.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ContributorTypeDTO from a JSON string
contributor_type_dto_instance = ContributorTypeDTO.from_json(json)
# print the JSON string representation of the object
print(ContributorTypeDTO.to_json())

# convert the object into a dict
contributor_type_dto_dict = contributor_type_dto_instance.to_dict()
# create an instance of ContributorTypeDTO from a dict
contributor_type_dto_form_dict = contributor_type_dto.from_dict(contributor_type_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



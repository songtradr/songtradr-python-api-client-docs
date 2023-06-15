# UsageDTO

Details on a track's or playlist's usage permissions.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.usage_dto import UsageDTO

# TODO update the JSON string below
json = "{}"
# create an instance of UsageDTO from a JSON string
usage_dto_instance = UsageDTO.from_json(json)
# print the JSON string representation of the object
print UsageDTO.to_json()

# convert the object into a dict
usage_dto_dict = usage_dto_instance.to_dict()
# create an instance of UsageDTO from a dict
usage_dto_form_dict = usage_dto.from_dict(usage_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



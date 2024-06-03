# TitleDTO

A Title for recordings or products.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title_text** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.title_dto import TitleDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TitleDTO from a JSON string
title_dto_instance = TitleDTO.from_json(json)
# print the JSON string representation of the object
print(TitleDTO.to_json())

# convert the object into a dict
title_dto_dict = title_dto_instance.to_dict()
# create an instance of TitleDTO from a dict
title_dto_from_dict = TitleDTO.from_dict(title_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



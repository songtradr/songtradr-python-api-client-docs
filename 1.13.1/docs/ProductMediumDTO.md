# ProductMediumDTO

Product details with a mid-sized field-set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**duration** | **datetime** |  | [optional] 
**pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] 
**gtin** | **str** |  | [optional] 
**grid** | **str** |  | [optional] 
**release_date** | **datetime** |  | [optional] 
**takedown_date** | **datetime** |  | [optional] 
**parties** | [**List[ProductPartyDTO]**](ProductPartyDTO.md) |  | [optional] 
**genres** | [**List[GenreMinimalDTO]**](GenreMinimalDTO.md) |  | [optional] 
**titles** | [**List[TitleDTO]**](TitleDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.product_medium_dto import ProductMediumDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ProductMediumDTO from a JSON string
product_medium_dto_instance = ProductMediumDTO.from_json(json)
# print the JSON string representation of the object
print ProductMediumDTO.to_json()

# convert the object into a dict
product_medium_dto_dict = product_medium_dto_instance.to_dict()
# create an instance of ProductMediumDTO from a dict
product_medium_dto_form_dict = product_medium_dto.from_dict(product_medium_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



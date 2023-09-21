# TrackToMediumProductDTO

A track that connects from recording to a product with a mid-sized field set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product** | [**ProductMediumDTO**](ProductMediumDTO.md) |  | 
**track_no** | **str** |  | 
**set_no** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.track_to_medium_product_dto import TrackToMediumProductDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TrackToMediumProductDTO from a JSON string
track_to_medium_product_dto_instance = TrackToMediumProductDTO.from_json(json)
# print the JSON string representation of the object
print TrackToMediumProductDTO.to_json()

# convert the object into a dict
track_to_medium_product_dto_dict = track_to_medium_product_dto_instance.to_dict()
# create an instance of TrackToMediumProductDTO from a dict
track_to_medium_product_dto_form_dict = track_to_medium_product_dto.from_dict(track_to_medium_product_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



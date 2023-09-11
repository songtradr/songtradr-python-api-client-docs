# SaveReferrerDTO

URLs that are allowed to reffer to musicube Widgets

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_referrer_dto import SaveReferrerDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveReferrerDTO from a JSON string
save_referrer_dto_instance = SaveReferrerDTO.from_json(json)
# print the JSON string representation of the object
print SaveReferrerDTO.to_json()

# convert the object into a dict
save_referrer_dto_dict = save_referrer_dto_instance.to_dict()
# create an instance of SaveReferrerDTO from a dict
save_referrer_dto_form_dict = save_referrer_dto.from_dict(save_referrer_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AdminApiUpdateUserDTO


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**full_name** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**is_admin** | **bool** |  | [optional] 
**widgets_allowed** | **bool** |  | [optional] 
**full_search_allowed** | **bool** |  | [optional] 
**voice_search_allowed** | **bool** |  | [optional] 
**recording_detail_allowed** | **bool** |  | [optional] 
**artist_detail_allowed** | **bool** |  | [optional] 
**playlist_prediction_allowed** | **bool** |  | [optional] 
**signup_allowed** | **bool** |  | [optional] 
**upload_allowed** | **bool** |  | [optional] 
**fingerprint_allowed** | **bool** |  | [optional] 
**audiotagging_allowed** | **bool** |  | [optional] 
**insights_allowed** | **bool** |  | [optional] 
**genres_allowed** | **bool** |  | [optional] 
**moods_allowed** | **bool** |  | [optional] 
**instrumentation_allowed** | **bool** |  | [optional] 
**sound_features_allowed** | **bool** |  | [optional] 
**tonal_features_allowed** | **bool** |  | [optional] 
**rhythm_features_allowed** | **bool** |  | [optional] 
**audience_allowed** | **bool** |  | [optional] 
**origin_allowed** | **bool** |  | [optional] 
**quality_allowed** | **bool** |  | [optional] 
**b2b_allowed** | **bool** |  | [optional] 
**editor_allowed** | **bool** |  | [optional] 
**reduced_musical_features** | **bool** |  | [optional] 
**confirmed** | **bool** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.admin_api_update_user_dto import AdminApiUpdateUserDTO

# TODO update the JSON string below
json = "{}"
# create an instance of AdminApiUpdateUserDTO from a JSON string
admin_api_update_user_dto_instance = AdminApiUpdateUserDTO.from_json(json)
# print the JSON string representation of the object
print AdminApiUpdateUserDTO.to_json()

# convert the object into a dict
admin_api_update_user_dto_dict = admin_api_update_user_dto_instance.to_dict()
# create an instance of AdminApiUpdateUserDTO from a dict
admin_api_update_user_dto_form_dict = admin_api_update_user_dto.from_dict(admin_api_update_user_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



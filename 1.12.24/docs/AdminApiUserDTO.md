# AdminApiUserDTO


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**username** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
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
**b2b_allowed** | **bool** |  | [optional] 
**editor_allowed** | **bool** |  | [optional] 
**reduced_musical_features** | **bool** |  | [optional] 
**confirmed** | **bool** |  | [optional] 
**gdpr_confirmation_timestamp** | **datetime** |  | [optional] 
**last_login** | **datetime** |  | [optional] 
**total_logins** | **int** |  | [optional] 
**total_searches** | **int** |  | [optional] 
**total_uploads** | **int** |  | [optional] 
**total_downloads** | **int** |  | [optional] 
**total_updates** | **int** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.admin_api_user_dto import AdminApiUserDTO

# TODO update the JSON string below
json = "{}"
# create an instance of AdminApiUserDTO from a JSON string
admin_api_user_dto_instance = AdminApiUserDTO.from_json(json)
# print the JSON string representation of the object
print AdminApiUserDTO.to_json()

# convert the object into a dict
admin_api_user_dto_dict = admin_api_user_dto_instance.to_dict()
# create an instance of AdminApiUserDTO from a dict
admin_api_user_dto_form_dict = admin_api_user_dto.from_dict(admin_api_user_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



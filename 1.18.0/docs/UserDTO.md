# UserDTO

All details on a user.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | 
**email_address** | **str** |  | 
**company_name** | **str** |  | [optional] 
**is_admin** | **bool** |  | 
**full_search_allowed** | **bool** |  | 
**voice_search_allowed** | **bool** |  | 
**recording_detail_allowed** | **bool** |  | 
**artist_detail_allowed** | **bool** |  | 
**playlist_prediction_allowed** | **bool** |  | 
**widgets_allowed** | **bool** |  | 
**signup_allowed** | **bool** |  | 
**upload_allowed** | **bool** |  | 
**fingerprint_allowed** | **bool** |  | 
**audiotagging_allowed** | **bool** |  | 
**b2b_allowed** | **bool** |  | 
**editor_allowed** | **bool** |  | 
**insights_allowed** | **bool** |  | 
**genres_allowed** | **bool** |  | 
**moods_allowed** | **bool** |  | 
**instrumentation_allowed** | **bool** |  | 
**sound_features_allowed** | **bool** |  | 
**tonal_features_allowed** | **bool** |  | 
**rhythm_features_allowed** | **bool** |  | 
**audience_allowed** | **bool** |  | 
**origin_allowed** | **bool** |  | 
**quality_allowed** | **bool** |  | 
**reduced_musical_features** | **bool** |  | 
**confirmed** | **bool** |  | 
**language** | **str** |  | 
**recording_endpoints_allowed** | **bool** |  | 
**admin** | **bool** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.user_dto import UserDTO

# TODO update the JSON string below
json = "{}"
# create an instance of UserDTO from a JSON string
user_dto_instance = UserDTO.from_json(json)
# print the JSON string representation of the object
print UserDTO.to_json()

# convert the object into a dict
user_dto_dict = user_dto_instance.to_dict()
# create an instance of UserDTO from a dict
user_dto_form_dict = user_dto.from_dict(user_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



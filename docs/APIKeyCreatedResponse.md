# APIKeyCreatedResponse

Returned ONLY by create + rotate — contains the plaintext key. Frontend must show it once and warn the user to copy it now.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**prefix** | **str** |  | 
**last_used_at** | **str** |  | [optional] 
**revoked_at** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**full_key** | **str** | Plaintext key. Shown ONCE — store it immediately. | 

## Example

```python
from sensecore.models.api_key_created_response import APIKeyCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of APIKeyCreatedResponse from a JSON string
api_key_created_response_instance = APIKeyCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(APIKeyCreatedResponse.to_json())

# convert the object into a dict
api_key_created_response_dict = api_key_created_response_instance.to_dict()
# create an instance of APIKeyCreatedResponse from a dict
api_key_created_response_from_dict = APIKeyCreatedResponse.from_dict(api_key_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



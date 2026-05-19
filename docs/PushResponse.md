# PushResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**records_accepted** | **int** |  | 
**records_rejected** | **int** |  | 
**message** | **str** |  | 

## Example

```python
from sensecore.models.push_response import PushResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PushResponse from a JSON string
push_response_instance = PushResponse.from_json(json)
# print the JSON string representation of the object
print(PushResponse.to_json())

# convert the object into a dict
push_response_dict = push_response_instance.to_dict()
# create an instance of PushResponse from a dict
push_response_from_dict = PushResponse.from_dict(push_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



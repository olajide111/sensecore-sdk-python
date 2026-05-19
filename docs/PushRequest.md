# PushRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**readings** | [**List[AppRoutersReadingsPushReadingItem]**](AppRoutersReadingsPushReadingItem.md) |  | 
**building_id** | **str** |  | [optional] 

## Example

```python
from sensecore.models.push_request import PushRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PushRequest from a JSON string
push_request_instance = PushRequest.from_json(json)
# print the JSON string representation of the object
print(PushRequest.to_json())

# convert the object into a dict
push_request_dict = push_request_instance.to_dict()
# create an instance of PushRequest from a dict
push_request_from_dict = PushRequest.from_dict(push_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



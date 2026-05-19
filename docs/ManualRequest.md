# ManualRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**timestamp** | **str** |  | 
**kwh** | **float** |  | 
**building_id** | **str** |  | [optional] 

## Example

```python
from sensecore.models.manual_request import ManualRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ManualRequest from a JSON string
manual_request_instance = ManualRequest.from_json(json)
# print the JSON string representation of the object
print(ManualRequest.to_json())

# convert the object into a dict
manual_request_dict = manual_request_instance.to_dict()
# create an instance of ManualRequest from a dict
manual_request_from_dict = ManualRequest.from_dict(manual_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



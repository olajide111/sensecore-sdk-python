# OptimiseRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**readings** | [**List[AppSchemasReadingItem]**](AppSchemasReadingItem.md) |  | 
**tariffs** | **List[str]** |  | [optional] [default to [flat, tou, economy7]]
**sector** | **str** |  | [optional] 

## Example

```python
from sensecore.models.optimise_request import OptimiseRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OptimiseRequest from a JSON string
optimise_request_instance = OptimiseRequest.from_json(json)
# print the JSON string representation of the object
print(OptimiseRequest.to_json())

# convert the object into a dict
optimise_request_dict = optimise_request_instance.to_dict()
# create an instance of OptimiseRequest from a dict
optimise_request_from_dict = OptimiseRequest.from_dict(optimise_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CarbonRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**readings** | [**List[AppSchemasReadingItem]**](AppSchemasReadingItem.md) |  | 
**period** | **str** |  | [optional] [default to 'monthly']

## Example

```python
from sensecore.models.carbon_request import CarbonRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CarbonRequest from a JSON string
carbon_request_instance = CarbonRequest.from_json(json)
# print the JSON string representation of the object
print(CarbonRequest.to_json())

# convert the object into a dict
carbon_request_dict = carbon_request_instance.to_dict()
# create an instance of CarbonRequest from a dict
carbon_request_from_dict = CarbonRequest.from_dict(carbon_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



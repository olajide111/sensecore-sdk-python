# OptimiseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**current_tariff** | **str** |  | 
**current_tariff_cost_annual** | **float** |  | 
**best_tariff** | **str** |  | 
**best_tariff_cost_annual** | **float** |  | 
**annual_saving_gbp** | **float** |  | 
**recommendation** | **str** |  | 
**tariff_breakdown** | **object** |  | 

## Example

```python
from sensecore.models.optimise_response import OptimiseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OptimiseResponse from a JSON string
optimise_response_instance = OptimiseResponse.from_json(json)
# print the JSON string representation of the object
print(OptimiseResponse.to_json())

# convert the object into a dict
optimise_response_dict = optimise_response_instance.to_dict()
# create an instance of OptimiseResponse from a dict
optimise_response_from_dict = OptimiseResponse.from_dict(optimise_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



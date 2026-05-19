# ERICResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**report_type** | **str** |  | [optional] [default to 'NHS ERIC']
**organisation** | **str** |  | 
**period** | **str** |  | 
**year** | **int** |  | 
**generated_at** | **str** |  | 
**electricity_kwh** | **float** |  | 
**gas_kwh** | **float** |  | 
**oil_kwh** | **float** |  | 
**coal_kwh** | **float** |  | 
**steam_kwh** | **float** |  | 
**hot_water_kwh** | **float** |  | 
**total_energy_kwh** | **float** |  | 
**total_energy_gj** | **float** |  | 
**co2_emissions_tonnes** | **float** |  | 
**floor_area_m2** | **float** |  | [optional] 
**energy_cost_gbp** | **float** |  | [optional] 
**renewable_generation_kwh** | **float** |  | [optional] [default to 0]
**chp_kwh** | **float** |  | [optional] [default to 0]
**backlog_maintenance_gbp** | **float** |  | [optional] 
**status** | **str** |  | [optional] [default to 'complete']

## Example

```python
from sensecore.models.eric_response import ERICResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ERICResponse from a JSON string
eric_response_instance = ERICResponse.from_json(json)
# print the JSON string representation of the object
print(ERICResponse.to_json())

# convert the object into a dict
eric_response_dict = eric_response_instance.to_dict()
# create an instance of ERICResponse from a dict
eric_response_from_dict = ERICResponse.from_dict(eric_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



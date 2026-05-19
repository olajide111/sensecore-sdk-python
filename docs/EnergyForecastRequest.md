# EnergyForecastRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | [optional] [default to 'METER-BDG2-001']
**readings** | **List[object]** |  | [optional] 
**horizon** | **int** |  | [optional] [default to 48]
**include_uncertainty** | **bool** |  | [optional] [default to True]
**sector** | **str** |  | [optional] [default to 'commercial']

## Example

```python
from sensecore.models.energy_forecast_request import EnergyForecastRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EnergyForecastRequest from a JSON string
energy_forecast_request_instance = EnergyForecastRequest.from_json(json)
# print the JSON string representation of the object
print(EnergyForecastRequest.to_json())

# convert the object into a dict
energy_forecast_request_dict = energy_forecast_request_instance.to_dict()
# create an instance of EnergyForecastRequest from a dict
energy_forecast_request_from_dict = EnergyForecastRequest.from_dict(energy_forecast_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



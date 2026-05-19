# ForecastResponse

Full SenseCore AI intelligence bundle — one response per meter request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**forecast_kwh** | **List[float]** |  | 
**lower_80** | **List[float]** |  | 
**upper_80** | **List[float]** |  | 
**mape_benchmark** | **float** |  | 
**model_version** | **str** |  | 
**generated_at** | **datetime** |  | 
**carbon** | [**CarbonLayer**](CarbonLayer.md) |  | 
**anomaly** | [**AnomalyLayer**](AnomalyLayer.md) |  | 
**fuel_poverty** | [**FuelPovertyLayer**](FuelPovertyLayer.md) |  | 
**occupancy** | [**OccupancyLayer**](OccupancyLayer.md) |  | 
**estimated_cost_gbp** | **float** |  | 
**annual_cost_gbp** | **float** |  | 

## Example

```python
from sensecore.models.forecast_response import ForecastResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ForecastResponse from a JSON string
forecast_response_instance = ForecastResponse.from_json(json)
# print the JSON string representation of the object
print(ForecastResponse.to_json())

# convert the object into a dict
forecast_response_dict = forecast_response_instance.to_dict()
# create an instance of ForecastResponse from a dict
forecast_response_from_dict = ForecastResponse.from_dict(forecast_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



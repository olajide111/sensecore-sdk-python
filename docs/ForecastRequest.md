# ForecastRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**readings** | [**List[AppSchemasReadingItem]**](AppSchemasReadingItem.md) |  | 
**horizon** | **int** |  | [optional] [default to 48]
**include_uncertainty** | **bool** |  | [optional] [default to True]
**sector** | **str** |  | [optional] 

## Example

```python
from sensecore.models.forecast_request import ForecastRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ForecastRequest from a JSON string
forecast_request_instance = ForecastRequest.from_json(json)
# print the JSON string representation of the object
print(ForecastRequest.to_json())

# convert the object into a dict
forecast_request_dict = forecast_request_instance.to_dict()
# create an instance of ForecastRequest from a dict
forecast_request_from_dict = ForecastRequest.from_dict(forecast_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# EngRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | [optional] 
**readings** | **List[object]** |  | [optional] 
**annual_kwh** | **float** |  | [optional] 
**floor_area_m2** | **float** |  | [optional] 
**building_type** | **str** |  | [optional] 
**revenue_gbp** | **float** |  | [optional] 
**fte_count** | **int** |  | [optional] 
**outdoor_temps_c** | **List[float]** |  | [optional] 
**base_temp_c** | **float** |  | [optional] [default to 15.5]
**fuel_type** | **str** |  | [optional] [default to 'electricity']
**investment_gbp** | **float** |  | [optional] 
**annual_saving_gbp** | **float** |  | [optional] 
**discount_rate** | **float** |  | [optional] [default to 0.035]
**project_years** | **int** |  | [optional] [default to 10]
**inflation_rate** | **float** |  | [optional] [default to 0.03]
**wall_area_m2** | **float** |  | [optional] 
**wall_u_value** | **float** |  | [optional] 
**roof_area_m2** | **float** |  | [optional] 
**roof_u_value** | **float** |  | [optional] 
**window_area_m2** | **float** |  | [optional] 
**window_u_value** | **float** |  | [optional] 
**floor_area_ground_m2** | **float** |  | [optional] 
**floor_u_value** | **float** |  | [optional] 
**ventilation_rate** | **float** |  | [optional] 
**indoor_temp_c** | **float** |  | [optional] [default to 21.0]
**outdoor_temp_c** | **float** |  | [optional] [default to 5.0]

## Example

```python
from sensecore.models.eng_request import EngRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EngRequest from a JSON string
eng_request_instance = EngRequest.from_json(json)
# print the JSON string representation of the object
print(EngRequest.to_json())

# convert the object into a dict
eng_request_dict = eng_request_instance.to_dict()
# create an instance of EngRequest from a dict
eng_request_from_dict = EngRequest.from_dict(eng_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



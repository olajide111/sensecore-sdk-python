# FuelPovertyLayer

Fuel poverty risk scoring (FPRS) — 5-signal index

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fprs_score** | **float** |  | 
**risk_level** | **str** |  | 
**signal_safe_heating** | **float** |  | 
**signal_self_rationing** | **float** |  | 
**signal_evening_suppression** | **float** |  | 
**signal_weekend_pattern** | **float** |  | 
**signal_long_absence** | **float** |  | 
**flagged_for_review** | **bool** |  | 

## Example

```python
from sensecore.models.fuel_poverty_layer import FuelPovertyLayer

# TODO update the JSON string below
json = "{}"
# create an instance of FuelPovertyLayer from a JSON string
fuel_poverty_layer_instance = FuelPovertyLayer.from_json(json)
# print the JSON string representation of the object
print(FuelPovertyLayer.to_json())

# convert the object into a dict
fuel_poverty_layer_dict = fuel_poverty_layer_instance.to_dict()
# create an instance of FuelPovertyLayer from a dict
fuel_poverty_layer_from_dict = FuelPovertyLayer.from_dict(fuel_poverty_layer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



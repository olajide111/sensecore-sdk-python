# CarbonLayer

Scope 2 carbon output per forecast period

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**forecast_kgco2** | **List[float]** |  | 
**carbon_intensity_gco2_kwh** | **float** |  | 
**annual_kgco2_estimate** | **float** |  | 

## Example

```python
from sensecore.models.carbon_layer import CarbonLayer

# TODO update the JSON string below
json = "{}"
# create an instance of CarbonLayer from a JSON string
carbon_layer_instance = CarbonLayer.from_json(json)
# print the JSON string representation of the object
print(CarbonLayer.to_json())

# convert the object into a dict
carbon_layer_dict = carbon_layer_instance.to_dict()
# create an instance of CarbonLayer from a dict
carbon_layer_from_dict = CarbonLayer.from_dict(carbon_layer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



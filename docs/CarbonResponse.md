# CarbonResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**period** | **str** |  | 
**total_kgco2** | **float** |  | 
**total_kwh** | **float** |  | 
**carbon_intensity_gco2_kwh** | **float** |  | 
**scope** | **str** |  | [optional] [default to 'Scope 2']
**reporting_standard** | **str** |  | [optional] [default to 'SECR / EU EED']
**generated_at** | **datetime** |  | 

## Example

```python
from sensecore.models.carbon_response import CarbonResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CarbonResponse from a JSON string
carbon_response_instance = CarbonResponse.from_json(json)
# print the JSON string representation of the object
print(CarbonResponse.to_json())

# convert the object into a dict
carbon_response_dict = carbon_response_instance.to_dict()
# create an instance of CarbonResponse from a dict
carbon_response_from_dict = CarbonResponse.from_dict(carbon_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



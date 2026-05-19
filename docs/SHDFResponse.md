# SHDFResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**report_type** | **str** |  | [optional] [default to 'SHDF Wave 2']
**organisation** | **str** |  | 
**generated_at** | **str** |  | 
**properties_assessed** | **int** |  | 
**average_fprs** | **float** |  | 
**high_risk_count** | **int** |  | 
**medium_risk_count** | **int** |  | 
**low_risk_count** | **int** |  | 
**epc_distribution** | **object** |  | 
**below_band_c_count** | **int** |  | 
**shdf_eligible_count** | **int** |  | 
**estimated_funding_gbp** | **float** |  | 
**retrofit_measures** | **List[object]** |  | 
**estimated_carbon_saving_tco2e** | **float** |  | 
**estimated_cost_saving_gbp** | **float** |  | 
**status** | **str** |  | [optional] [default to 'assessment']

## Example

```python
from sensecore.models.shdf_response import SHDFResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SHDFResponse from a JSON string
shdf_response_instance = SHDFResponse.from_json(json)
# print the JSON string representation of the object
print(SHDFResponse.to_json())

# convert the object into a dict
shdf_response_dict = shdf_response_instance.to_dict()
# create an instance of SHDFResponse from a dict
shdf_response_from_dict = SHDFResponse.from_dict(shdf_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



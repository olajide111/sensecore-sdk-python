# SECRResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**report_type** | **str** |  | [optional] [default to 'SECR']
**organisation** | **str** |  | 
**period** | **str** |  | 
**year** | **int** |  | 
**generated_at** | **str** |  | 
**scope1_kgco2e** | **float** |  | 
**scope1_source** | **str** |  | 
**scope2_kgco2e** | **float** |  | 
**scope2_source** | **str** |  | 
**total_kgco2e** | **float** |  | 
**total_tco2e** | **float** |  | 
**total_kwh** | **float** |  | 
**intensity_revenue** | **float** |  | [optional] 
**intensity_area** | **float** |  | [optional] 
**intensity_fte** | **float** |  | [optional] 
**previous_year_tco2e** | **float** |  | [optional] 
**yoy_change_pct** | **float** |  | [optional] 
**defra_year** | **int** |  | 
**defra_electricity_factor** | **float** |  | 
**defra_gas_factor** | **float** |  | 
**methodology** | **str** |  | 
**recommendations** | **List[object]** |  | 
**status** | **str** |  | [optional] [default to 'complete']

## Example

```python
from sensecore.models.secr_response import SECRResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SECRResponse from a JSON string
secr_response_instance = SECRResponse.from_json(json)
# print the JSON string representation of the object
print(SECRResponse.to_json())

# convert the object into a dict
secr_response_dict = secr_response_instance.to_dict()
# create an instance of SECRResponse from a dict
secr_response_from_dict = SECRResponse.from_dict(secr_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



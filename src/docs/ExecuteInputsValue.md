# ExecuteInputsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bbox** | **List[float]** |  | 
**crs** | **str** |  | [optional] [default to 'http://www.opengis.net/def/crs/OGC/1.3/CRS84']
**media_type** | **str** |  | [optional] 
**encoding** | **str** |  | [optional] 
**var_schema** | [**FormatSchema**](FormatSchema.md) |  | [optional] 
**value** | [**InputValue**](InputValue.md) |  | 
**href** | **str** |  | 
**rel** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**hreflang** | **str** |  | [optional] 
**title** | **str** |  | [optional] 

## Example

```python
from ogc_api_client.models.execute_inputs_value import ExecuteInputsValue

# TODO update the JSON string below
json = "{}"
# create an instance of ExecuteInputsValue from a JSON string
execute_inputs_value_instance = ExecuteInputsValue.from_json(json)
# print the JSON string representation of the object
print(ExecuteInputsValue.to_json())

# convert the object into a dict
execute_inputs_value_dict = execute_inputs_value_instance.to_dict()
# create an instance of ExecuteInputsValue from a dict
execute_inputs_value_from_dict = ExecuteInputsValue.from_dict(execute_inputs_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# QualifiedInputValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**media_type** | **str** |  | [optional] 
**encoding** | **str** |  | [optional] 
**var_schema** | [**FormatSchema**](FormatSchema.md) |  | [optional] 
**value** | [**InputValue**](InputValue.md) |  | 

## Example

```python
from ogc_api_client.models.qualified_input_value import QualifiedInputValue

# TODO update the JSON string below
json = "{}"
# create an instance of QualifiedInputValue from a JSON string
qualified_input_value_instance = QualifiedInputValue.from_json(json)
# print the JSON string representation of the object
print(QualifiedInputValue.to_json())

# convert the object into a dict
qualified_input_value_dict = qualified_input_value_instance.to_dict()
# create an instance of QualifiedInputValue from a dict
qualified_input_value_from_dict = QualifiedInputValue.from_dict(qualified_input_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



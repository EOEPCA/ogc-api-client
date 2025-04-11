# AdditionalParameter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**value** | [**List[AdditionalParameterValueInner]**](AdditionalParameterValueInner.md) |  | 

## Example

```python
from ogc_api_client.models.additional_parameter import AdditionalParameter

# TODO update the JSON string below
json = "{}"
# create an instance of AdditionalParameter from a JSON string
additional_parameter_instance = AdditionalParameter.from_json(json)
# print the JSON string representation of the object
print(AdditionalParameter.to_json())

# convert the object into a dict
additional_parameter_dict = additional_parameter_instance.to_dict()
# create an instance of AdditionalParameter from a dict
additional_parameter_from_dict = AdditionalParameter.from_dict(additional_parameter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



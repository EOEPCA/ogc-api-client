# OutputDescription


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**metadata** | [**List[Metadata]**](Metadata.md) |  | [optional] 
**additional_parameters** | [**DescriptionTypeAdditionalParameters**](DescriptionTypeAdditionalParameters.md) |  | [optional] 
**var_schema** | [**ModelSchema**](ModelSchema.md) |  | 

## Example

```python
from ogcapi_processes_client.models.output_description import OutputDescription

# TODO update the JSON string below
json = "{}"
# create an instance of OutputDescription from a JSON string
output_description_instance = OutputDescription.from_json(json)
# print the JSON string representation of the object
print(OutputDescription.to_json())

# convert the object into a dict
output_description_dict = output_description_instance.to_dict()
# create an instance of OutputDescription from a dict
output_description_from_dict = OutputDescription.from_dict(output_description_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# DescriptionType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**metadata** | [**List[Metadata]**](Metadata.md) |  | [optional] 
**additional_parameters** | [**DescriptionTypeAdditionalParameters**](DescriptionTypeAdditionalParameters.md) |  | [optional] 

## Example

```python
from ogcapi_processes_client.models.description_type import DescriptionType

# TODO update the JSON string below
json = "{}"
# create an instance of DescriptionType from a JSON string
description_type_instance = DescriptionType.from_json(json)
# print the JSON string representation of the object
print(DescriptionType.to_json())

# convert the object into a dict
description_type_dict = description_type_instance.to_dict()
# create an instance of DescriptionType from a dict
description_type_from_dict = DescriptionType.from_dict(description_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



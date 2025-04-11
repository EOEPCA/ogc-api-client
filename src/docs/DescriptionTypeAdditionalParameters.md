# DescriptionTypeAdditionalParameters


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**role** | **str** |  | [optional] 
**href** | **str** |  | [optional] 
**parameters** | [**List[AdditionalParameter]**](AdditionalParameter.md) |  | [optional] 

## Example

```python
from ogc_api_client.models.description_type_additional_parameters import DescriptionTypeAdditionalParameters

# TODO update the JSON string below
json = "{}"
# create an instance of DescriptionTypeAdditionalParameters from a JSON string
description_type_additional_parameters_instance = DescriptionTypeAdditionalParameters.from_json(json)
# print the JSON string representation of the object
print(DescriptionTypeAdditionalParameters.to_json())

# convert the object into a dict
description_type_additional_parameters_dict = description_type_additional_parameters_instance.to_dict()
# create an instance of DescriptionTypeAdditionalParameters from a dict
description_type_additional_parameters_from_dict = DescriptionTypeAdditionalParameters.from_dict(description_type_additional_parameters_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



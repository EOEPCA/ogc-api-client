# InputDescription


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**metadata** | [**List[Metadata]**](Metadata.md) |  | [optional] 
**additional_parameters** | [**DescriptionTypeAdditionalParameters**](DescriptionTypeAdditionalParameters.md) |  | [optional] 
**min_occurs** | **int** |  | [optional] [default to 1]
**max_occurs** | [**InputDescriptionAllOfMaxOccurs**](InputDescriptionAllOfMaxOccurs.md) |  | [optional] 
**var_schema** | [**ModelSchema**](ModelSchema.md) |  | 

## Example

```python
from ogc_api_client.models.input_description import InputDescription

# TODO update the JSON string below
json = "{}"
# create an instance of InputDescription from a JSON string
input_description_instance = InputDescription.from_json(json)
# print the JSON string representation of the object
print(InputDescription.to_json())

# convert the object into a dict
input_description_dict = input_description_instance.to_dict()
# create an instance of InputDescription from a dict
input_description_from_dict = InputDescription.from_dict(input_description_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



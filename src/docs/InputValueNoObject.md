# InputValueNoObject


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bbox** | **List[float]** |  | 
**crs** | **str** |  | [optional] [default to 'http://www.opengis.net/def/crs/OGC/1.3/CRS84']

## Example

```python
from ogc_api_client.models.input_value_no_object import InputValueNoObject

# TODO update the JSON string below
json = "{}"
# create an instance of InputValueNoObject from a JSON string
input_value_no_object_instance = InputValueNoObject.from_json(json)
# print the JSON string representation of the object
print(InputValueNoObject.to_json())

# convert the object into a dict
input_value_no_object_dict = input_value_no_object_instance.to_dict()
# create an instance of InputValueNoObject from a dict
input_value_no_object_from_dict = InputValueNoObject.from_dict(input_value_no_object_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



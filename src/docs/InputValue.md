# InputValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bbox** | **List[float]** |  | 
**crs** | **str** |  | [optional] [default to 'http://www.opengis.net/def/crs/OGC/1.3/CRS84']

## Example

```python
from ogcapi_processes_client.models.input_value import InputValue

# TODO update the JSON string below
json = "{}"
# create an instance of InputValue from a JSON string
input_value_instance = InputValue.from_json(json)
# print the JSON string representation of the object
print(InputValue.to_json())

# convert the object into a dict
input_value_dict = input_value_instance.to_dict()
# create an instance of InputValue from a dict
input_value_from_dict = InputValue.from_dict(input_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



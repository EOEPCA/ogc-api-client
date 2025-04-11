# ProcessList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**processes** | [**List[ProcessSummary]**](ProcessSummary.md) |  | 
**links** | [**List[Link]**](Link.md) |  | 

## Example

```python
from ogc_api_client.models.process_list import ProcessList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessList from a JSON string
process_list_instance = ProcessList.from_json(json)
# print the JSON string representation of the object
print(ProcessList.to_json())

# convert the object into a dict
process_list_dict = process_list_instance.to_dict()
# create an instance of ProcessList from a dict
process_list_from_dict = ProcessList.from_dict(process_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# StatusInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**process_id** | **str** |  | [optional] 
**type** | **str** |  | 
**job_id** | **str** |  | 
**status** | [**StatusCode**](StatusCode.md) |  | 
**message** | **str** |  | [optional] 
**created** | **datetime** |  | [optional] 
**started** | **datetime** |  | [optional] 
**finished** | **datetime** |  | [optional] 
**updated** | **datetime** |  | [optional] 
**progress** | **int** |  | [optional] 
**links** | [**List[Link]**](Link.md) |  | [optional] 

## Example

```python
from ogcapi_processes_client.models.status_info import StatusInfo

# TODO update the JSON string below
json = "{}"
# create an instance of StatusInfo from a JSON string
status_info_instance = StatusInfo.from_json(json)
# print the JSON string representation of the object
print(StatusInfo.to_json())

# convert the object into a dict
status_info_dict = status_info_instance.to_dict()
# create an instance of StatusInfo from a dict
status_info_from_dict = StatusInfo.from_dict(status_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



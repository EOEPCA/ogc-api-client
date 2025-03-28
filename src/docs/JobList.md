# JobList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jobs** | [**List[StatusInfo]**](StatusInfo.md) |  | 
**links** | [**List[Link]**](Link.md) |  | 

## Example

```python
from ogcapi_processes_client.models.job_list import JobList

# TODO update the JSON string below
json = "{}"
# create an instance of JobList from a JSON string
job_list_instance = JobList.from_json(json)
# print the JSON string representation of the object
print(JobList.to_json())

# convert the object into a dict
job_list_dict = job_list_instance.to_dict()
# create an instance of JobList from a dict
job_list_from_dict = JobList.from_dict(job_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Process


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**metadata** | [**List[Metadata]**](Metadata.md) |  | [optional] 
**additional_parameters** | [**DescriptionTypeAdditionalParameters**](DescriptionTypeAdditionalParameters.md) |  | [optional] 
**id** | **str** |  | 
**version** | **str** |  | 
**job_control_options** | [**List[JobControlOptions]**](JobControlOptions.md) |  | [optional] 
**output_transmission** | [**List[TransmissionMode]**](TransmissionMode.md) |  | [optional] 
**links** | [**List[Link]**](Link.md) |  | [optional] 
**inputs** | [**Dict[str, InputDescription]**](InputDescription.md) |  | [optional] 
**outputs** | [**Dict[str, OutputDescription]**](OutputDescription.md) |  | [optional] 

## Example

```python
from ogcapi_processes_client.models.process import Process

# TODO update the JSON string below
json = "{}"
# create an instance of Process from a JSON string
process_instance = Process.from_json(json)
# print the JSON string representation of the object
print(Process.to_json())

# convert the object into a dict
process_dict = process_instance.to_dict()
# create an instance of Process from a dict
process_from_dict = Process.from_dict(process_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



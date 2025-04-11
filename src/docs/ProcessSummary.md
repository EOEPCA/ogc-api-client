# ProcessSummary


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

## Example

```python
from ogc_api_client.models.process_summary import ProcessSummary

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessSummary from a JSON string
process_summary_instance = ProcessSummary.from_json(json)
# print the JSON string representation of the object
print(ProcessSummary.to_json())

# convert the object into a dict
process_summary_dict = process_summary_instance.to_dict()
# create an instance of ProcessSummary from a dict
process_summary_from_dict = ProcessSummary.from_dict(process_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



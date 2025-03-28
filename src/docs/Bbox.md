# Bbox


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bbox** | **List[float]** |  | 
**crs** | **str** |  | [optional] [default to 'http://www.opengis.net/def/crs/OGC/1.3/CRS84']

## Example

```python
from ogcapi_processes_client.models.bbox import Bbox

# TODO update the JSON string below
json = "{}"
# create an instance of Bbox from a JSON string
bbox_instance = Bbox.from_json(json)
# print the JSON string representation of the object
print(Bbox.to_json())

# convert the object into a dict
bbox_dict = bbox_instance.to_dict()
# create an instance of Bbox from a dict
bbox_from_dict = Bbox.from_dict(bbox_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InlineOrRefData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bbox** | **List[float]** |  | 
**crs** | **str** |  | [optional] [default to 'http://www.opengis.net/def/crs/OGC/1.3/CRS84']
**media_type** | **str** |  | [optional] 
**encoding** | **str** |  | [optional] 
**var_schema** | [**FormatSchema**](FormatSchema.md) |  | [optional] 
**value** | [**InputValue**](InputValue.md) |  | 
**href** | **str** |  | 
**rel** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**hreflang** | **str** |  | [optional] 
**title** | **str** |  | [optional] 

## Example

```python
from ogc_api_client.models.inline_or_ref_data import InlineOrRefData

# TODO update the JSON string below
json = "{}"
# create an instance of InlineOrRefData from a JSON string
inline_or_ref_data_instance = InlineOrRefData.from_json(json)
# print the JSON string representation of the object
print(InlineOrRefData.to_json())

# convert the object into a dict
inline_or_ref_data_dict = inline_or_ref_data_instance.to_dict()
# create an instance of InlineOrRefData from a dict
inline_or_ref_data_from_dict = InlineOrRefData.from_dict(inline_or_ref_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# jq

Parse, manipulate and output JSON data.

## Examples

```bash
list_devices.sh | jq '.[] | {uuid:.Uuid,mode:.Model,name:.Name,type:.Type}'
```

```bash
list_devices.sh | jq '.[] | {uuid:.Uuid,mode:.Model,name:.Name,type:.Type,tech:.Technology,online:.Online,appliance:.Parameters[]|select(has("MeasuredApplianceType"))|.MeasuredApplianceType} | select(.type | contains("meter"))'
```

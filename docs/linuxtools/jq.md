# jq

Parse, manipulate and output JSON data.

## Examples

```bash
list_devices.sh | jq '.[] | {uuid:.Uuid,mode:.Model,name:.Name,type:.Type}'
```

```bash
list_devices.sh | jq '.[] | {uuid:.Uuid,mode:.Model,name:.Name,type:.Type,online:.Online,properties:.Properties} | select(.type | contains("meter"))'
```

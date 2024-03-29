
# Observation Request

Used to define callbacks including the device identity, the attribute names, corresponding attribute values and the date/timestamp of when the observation was made.

## Structure

`ObservationRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AccountName` | `string` | Required | Account identifier in "##########-#####". |
| `Devices` | [`List<Device>`](../../doc/models/device.md) | Required | List of devices. |
| `Attributes` | [`List<ObservationRequestAttribute>`](../../doc/models/observation-request-attribute.md) | Required | Attributes are streaming RF parameters that you want to observe. |
| `Frequency` | [`NumericalData`](../../doc/models/numerical-data.md) | Optional | Describes value and unit of time. |
| `Duration` | [`NumericalData`](../../doc/models/numerical-data.md) | Optional | Describes value and unit of time. |

## Example (as JSON)

```json
{
  "accountName": "0000123456-00001",
  "attributes": [
    {
      "name": "RADIO_SIGNAL_STRENGTH"
    },
    {
      "name": "LINK_QUALITY"
    },
    {
      "name": "NETWORK_BEARER"
    },
    {
      "name": "CELL_ID"
    }
  ],
  "devices": [
    {
      "id": "864508030026238",
      "kind": "IMEI"
    }
  ],
  "frequency": {
    "value": 76,
    "unit": "SECOND"
  },
  "duration": {
    "value": 176,
    "unit": "SECOND"
  }
}
```


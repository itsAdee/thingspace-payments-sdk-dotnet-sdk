
# Change Pmec Device Profile Bulk Request

## Structure

`ChangePmecDeviceProfileBulkRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AccountName` | `string` | Required | - |
| `DeviceList` | [`List<MECDeviceList>`](../../doc/models/mec-device-list.md) | Required | - |
| `NewProfile` | `string` | Required | - |

## Example (as JSON)

```json
{
  "accountName": "0342351414-00001",
  "deviceList": [
    {
      "deviceIds": [
        {
          "id": "99948099913032000000",
          "kind": "iccid"
        }
      ]
    },
    {
      "deviceIds": [
        {
          "id": "99948099913032100000",
          "kind": "iccid"
        }
      ]
    }
  ],
  "newProfile": "HSS EsmProfile Enterprise 5G"
}
```


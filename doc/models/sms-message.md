
# SMS Message

SMS messages sent by all M2M devices associated with a billing account.

## Structure

`SMSMessage`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `DeviceIds` | [`List<DeviceId>`](../../doc/models/device-id.md) | Optional | One or more IDs of the device that sent the message. |
| `Message` | `string` | Optional | The contents of the SMS message. |
| `Timestamp` | `string` | Optional | The date and time that the message was received by the Verizon ThingSpace Platform. |

## Example (as JSON)

```json
{
  "deviceIds": [
    {
      "id": "09623489171",
      "kind": "esn"
    }
  ],
  "message": "testmessage1",
  "timestamp": "2016-01-01T12:29:49-08:00"
}
```



# Date Filter

Filter out the dates.

## Structure

`DateFilter`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Earliest` | `string` | Required | Only include devices that were added after this date and time. |
| `Latest` | `string` | Required | Only include devices that were added before this date and time. |

## Example (as JSON)

```json
{
  "earliest": "2020-05-01T15:00:00-08:00Z",
  "latest": "2020-07-30T15:00:00-08:00Z"
}
```


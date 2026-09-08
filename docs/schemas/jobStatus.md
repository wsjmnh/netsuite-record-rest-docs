# Schemas: jobStatus

Property tables for definitions owned by `jobStatus`.

Record page: [jobStatus](../records/jobStatus.md).

## Index

- [jobStatus](#jobstatus) — 12 properties
- [jobStatusCollection](#jobstatuscollection) — 6 properties

## jobStatus

Browser definition `jobStatus`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allowCompletelyBilledOnProject` | Completely billed | boolean |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Status | string |  |  |  |  |
| `percentCompleteAutomaticRecalculation` | Percent Complete Automatic Recalculation | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `scheduleActualChargeRunOnMidnight` | Create actual charges during midnight run | boolean |  |  |  |  |
| `scheduleForecastChargeRunOnMidnight` | Create forecast charges during midnight run | boolean |  |  |  |  |

## jobStatusCollection

Browser definition `jobStatusCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | jobStatus[] |  |  | [`jobStatus`](#jobstatus) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

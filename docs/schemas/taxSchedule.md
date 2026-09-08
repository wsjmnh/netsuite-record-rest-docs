# Schemas: taxSchedule

Property tables for definitions owned by `taxSchedule`.

Record page: [taxSchedule](../records/taxSchedule.md).

## Index

- [taxSchedule](#taxschedule) — 9 properties
- [taxSchedule-nexusesCollection](#taxschedule-nexusescollection) — 6 properties
- [taxSchedule-nexusesElement](#taxschedule-nexuseselement) — 7 properties
- [taxSchedule-usNexusesCollection](#taxschedule-usnexusescollection) — 6 properties
- [taxSchedule-usNexusesElement](#taxschedule-usnexuseselement) — 4 properties
- [taxScheduleCollection](#taxschedulecollection) — 6 properties

## taxSchedule

Browser definition `taxSchedule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `nexuses` |  | taxSchedule-nexusesCollection |  |  | [`taxSchedule-nexusesCollection`](#taxschedule-nexusescollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `usNexuses` |  | taxSchedule-usNexusesCollection |  |  | [`taxSchedule-usNexusesCollection`](#taxschedule-usnexusescollection) |  |

## taxSchedule-nexusesCollection

Browser definition `taxSchedule-nexusesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | taxSchedule-nexusesElement[] |  |  | [`taxSchedule-nexusesElement`](#taxschedule-nexuseselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## taxSchedule-nexusesElement

Browser definition `taxSchedule-nexusesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `nexusCountry` | Country | string |  |  |  |  |
| `purchaseTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxCodeInclude` | Tax Code Lists Include | string |  |  |  |  |

## taxSchedule-usNexusesCollection

Browser definition `taxSchedule-usNexusesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | taxSchedule-usNexusesElement[] |  |  | [`taxSchedule-usNexusesElement`](#taxschedule-usnexuseselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## taxSchedule-usNexusesElement

Browser definition `taxSchedule-usNexusesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxable` | Taxable | boolean |  |  |  |  |

## taxScheduleCollection

Browser definition `taxScheduleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | taxSchedule[] |  |  | [`taxSchedule`](#taxschedule) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

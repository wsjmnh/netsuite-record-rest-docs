# Schemas: unitsType

Property tables for definitions owned by `unitsType`.

Record page: [unitsType](../records/unitsType.md).

## Index

- [unitsType](#unitstype) — 8 properties
- [unitsType-uomCollection](#unitstype-uomcollection) — 6 properties
- [unitsType-uomElement](#unitstype-uomelement) — 10 properties
- [unitsTypeCollection](#unitstypecollection) — 6 properties

## unitsType

Browser definition `unitsType`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Type Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `uom` |  | unitsType-uomCollection |  |  | [`unitsType-uomCollection`](#unitstype-uomcollection) |  |

## unitsType-uomCollection

Browser definition `unitsType-uomCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | unitsType-uomElement[] |  |  | [`unitsType-uomElement`](#unitstype-uomelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## unitsType-uomElement

Browser definition `unitsType-uomElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `abbreviation` | Abbreviation | string |  |  |  |  |
| `baseUnit` | Base Unit | boolean |  |  |  |  |
| `conversionRate` | Conversion Rate {1} | number | float |  |  |  |
| `inUse` | Used | boolean |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `pluralAbbreviation` | Plural Abbreviation | string |  |  |  |  |
| `pluralName` | Plural Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `unitName` | Name | string |  |  |  |  |

## unitsTypeCollection

Browser definition `unitsTypeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | unitsType[] |  |  | [`unitsType`](#unitstype) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

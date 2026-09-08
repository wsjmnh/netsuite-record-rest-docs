# Schemas: manufacturingCostTemplate

Property tables for definitions owned by `manufacturingCostTemplate`.

Record page: [manufacturingCostTemplate](../records/manufacturingCostTemplate.md).

## Index

- [manufacturingCostTemplate](#manufacturingcosttemplate) — 11 properties
- [manufacturingCostTemplate-costDetailCollection](#manufacturingcosttemplate-costdetailcollection) — 6 properties
- [manufacturingCostTemplate-costDetailElement](#manufacturingcosttemplate-costdetailelement) — 6 properties
- [manufacturingCostTemplateCollection](#manufacturingcosttemplatecollection) — 6 properties
- [manufacturingCostTemplateSelectOptions](#manufacturingcosttemplateselectoptions) — 2 properties

## manufacturingCostTemplate

Browser definition `manufacturingCostTemplate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `costDetail` |  | manufacturingCostTemplate-costDetailCollection |  |  | [`manufacturingCostTemplate-costDetailCollection`](#manufacturingcosttemplate-costdetailcollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## manufacturingCostTemplate-costDetailCollection

Browser definition `manufacturingCostTemplate-costDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | manufacturingCostTemplate-costDetailElement[] |  |  | [`manufacturingCostTemplate-costDetailElement`](#manufacturingcosttemplate-costdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingCostTemplate-costDetailElement

Browser definition `manufacturingCostTemplate-costDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `fixedRate` | Fixed Rate | number | double |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `runRate` | Run Rate | number | double |  |  |  |

## manufacturingCostTemplateCollection

Browser definition `manufacturingCostTemplateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | manufacturingCostTemplate[] |  |  | [`manufacturingCostTemplate`](#manufacturingcosttemplate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingCostTemplateSelectOptions

Browser definition `manufacturingCostTemplateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

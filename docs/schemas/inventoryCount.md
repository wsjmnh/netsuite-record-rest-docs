# Schemas: inventoryCount

Property tables for definitions owned by `inventoryCount`.

Record page: [inventoryCount](../records/inventoryCount.md).

## Index

- [inventoryCount](#inventorycount) — 28 properties
- [inventoryCount-item-countDetail](#inventorycount-item-countdetail) — 8 properties
- [inventoryCount-item-countDetail-inventoryDetailCollection](#inventorycount-item-countdetail-inventorydetailcollection) — 6 properties
- [inventoryCount-item-countDetail-inventoryDetailElement](#inventorycount-item-countdetail-inventorydetailelement) — 6 properties
- [inventoryCount-itemCollection](#inventorycount-itemcollection) — 6 properties
- [inventoryCount-itemElement](#inventorycount-itemelement) — 14 properties
- [inventoryCountCollection](#inventorycountcollection) — 6 properties
- [inventoryCountSelectOptions](#inventorycountselectoptions) — 9 properties

## inventoryCount

Browser definition `inventoryCount`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `countDate` | Count Start Date | string | date |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | inventoryCount-itemCollection |  |  | [`inventoryCount-itemCollection`](#inventorycount-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `selStatus` |  | object |  |  |  |  |
| `selStatus.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D` |
| `selStatus.refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## inventoryCount-item-countDetail

Browser definition `inventoryCount-item-countDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `bin` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `inventoryDetail` |  | inventoryCount-item-countDetail-inventoryDetailCollection |  |  | [`inventoryCount-item-countDetail-inventoryDetailCollection`](#inventorycount-item-countdetail-inventorydetailcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |

## inventoryCount-item-countDetail-inventoryDetailCollection

Browser definition `inventoryCount-item-countDetail-inventoryDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryCount-item-countDetail-inventoryDetailElement[] |  |  | [`inventoryCount-item-countDetail-inventoryDetailElement`](#inventorycount-item-countdetail-inventorydetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCount-item-countDetail-inventoryDetailElement

Browser definition `inventoryCount-item-countDetail-inventoryDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | Internal ID | integer | int64 |  |  |  |
| `inventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## inventoryCount-itemCollection

Browser definition `inventoryCount-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryCount-itemElement[] |  |  | [`inventoryCount-itemElement`](#inventorycount-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCount-itemElement

Browser definition `inventoryCount-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `adjustedQuantity` | Adjusted Quantity | number | double |  |  |  |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `countDetail` |  | inventoryCount-item-countDetail |  |  | [`inventoryCount-item-countDetail`](#inventorycount-item-countdetail) |  |
| `countLine` | Line | integer | int64 |  |  |  |
| `countQuantity` | Count Quantity | number | double |  |  |  |
| `item` |  | inventoryItem |  |  | [`inventoryItem`](inventoryItem.md#inventoryitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `snapshotQuantity` | Snapshot Quantity | number | double |  |  |  |
| `units` | Units | string |  |  |  |  |
| `viewAdjustment` | Variance Detail | string |  |  |  |  |
| `viewSnapshot` | Snapshot Detail | string |  |  |  |  |

## inventoryCountCollection

Browser definition `inventoryCountCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inventoryCount[] |  |  | [`inventoryCount`](#inventorycount) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryCountSelectOptions

Browser definition `inventoryCountSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `selStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

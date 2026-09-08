# Schemas: payrollItem

Property tables for definitions owned by `payrollItem`.

Record page: [payrollItem](../records/payrollItem.md).

## Index

- [payrollItem](#payrollitem) — 38 properties
- [payrollItemCollection](#payrollitemcollection) — 6 properties
- [payrollItemSelectOptions](#payrollitemselectoptions) — 13 properties

## payrollItem

Browser definition `payrollItem`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountcategory` |  | object |  |  |  |  |
| `accountcategory.id` | Internal identifier | string |  |  |  | `Expense`, `Liability`, `Asset` |
| `accountcategory.refName` | Reference Name | string |  |  |  |  |
| `assetaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `defaultRate` | Default Rate | number | double |  |  |  |
| `deriveRateFromRetirementPlan` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `derivedratemultiplier` | Rate Multiplier | number | float |  |  |  |
| `deriveratefrompayrollitem` |  | payrollItem |  |  | [`payrollItem`](#payrollitem) |  |
| `deriveratefrompayrollitemgroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deriveratefromtype` |  | object |  |  |  |  |
| `deriveratefromtype.id` | Internal identifier | string |  |  |  | `payrollitem`, `payrollitemgroup`, `retirementplan` |
| `deriveratefromtype.refName` | Reference Name | string |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `employeePaid` | Employee Paid | boolean |  |  |  |  |
| `expenseAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `liabilityAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `limit` | Limit | number | double |  |  |  |
| `limitiswithholding` |  | object |  |  |  |  |
| `limitiswithholding.id` | Internal identifier | string |  |  |  | `wage`, `withholding` |
| `limitiswithholding.refName` | Reference Name | string |  |  |  |  |
| `limittype` | Limit Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locality` | Locality | string |  |  |  |  |
| `name` | Item Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reportingSection` |  | object |  |  |  |  |
| `reportingSection.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `reportingSection.refName` | Reference Name | string |  |  |  |  |
| `state` | State | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |

## payrollItemCollection

Browser definition `payrollItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | payrollItem[] |  |  | [`payrollItem`](#payrollitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## payrollItemSelectOptions

Browser definition `payrollItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountcategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `assetaccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deriveRateFromRetirementPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deriveratefrompayrollitem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deriveratefrompayrollitemgroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deriveratefromtype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `liabilityAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `limitiswithholding` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reportingSection` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: paymentMethod

Property tables for definitions owned by `paymentMethod`.

Record page: [paymentMethod](../records/paymentMethod.md).

## Index

- [paymentMethod](#paymentmethod) — 23 properties
- [paymentMethod-visualsCollection](#paymentmethod-visualscollection) — 6 properties
- [paymentMethod-visualsElement](#paymentmethod-visualselement) — 4 properties
- [paymentMethodCollection](#paymentmethodcollection) — 6 properties
- [paymentMethodSelectOptions](#paymentmethodselectoptions) — 6 properties

## paymentMethod

Browser definition `paymentMethod`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `cardBrands` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `countries` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isDebitCard` | Debit Card | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isLineLevelDataRequired` | Requires Line-Level Data | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `longitemtype` |  | string |  |  |  |  |
| `merchantAccounts` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `methodType` |  | object |  |  |  |  |
| `methodType.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `methodType.refName` | Reference Name | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tname` |  | string |  |  |  |  |
| `undepFunds` |  | object |  |  |  |  |
| `undepFunds.id` | Internal identifier | string |  |  |  |  |
| `undepFunds.refName` | Reference Name | string |  |  |  |  |
| `visuals` |  | paymentMethod-visualsCollection |  |  | [`paymentMethod-visualsCollection`](#paymentmethod-visualscollection) |  |

## paymentMethod-visualsCollection

Browser definition `paymentMethod-visualsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paymentMethod-visualsElement[] |  |  | [`paymentMethod-visualsElement`](#paymentmethod-visualselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paymentMethod-visualsElement

Browser definition `paymentMethod-visualsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `flags` | Flags | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` | URL | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## paymentMethodCollection

Browser definition `paymentMethodCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | paymentMethod[] |  |  | [`paymentMethod`](#paymentmethod) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paymentMethodSelectOptions

Browser definition `paymentMethodSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardBrands` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `countries` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `merchantAccounts` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `methodType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `undepFunds` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: generalToken

Property tables for definitions owned by `generalToken`.

Record page: [generalToken](../records/generalToken.md).

## Index

- [generalToken](#generaltoken) — 25 properties
- [generalTokenCollection](#generaltokencollection) — 6 properties
- [generalTokenSelectOptions](#generaltokenselectoptions) — 6 properties

## generalToken

Browser definition `generalToken`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `instrumentType` |  | object |  |  |  |  |
| `instrumentType.id` | Internal identifier | string |  |  |  | `1`, `2`, `13`, `3` |
| `instrumentType.refName` | Reference Name | string |  |  |  |  |
| `isDefault` | Default | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mask` | Mask | string |  |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `paymentMethod` |  | paymentMethod |  |  | [`paymentMethod`](paymentMethod.md#paymentmethod) |  |
| `preserveOnFile` | Preserve on File | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `state` |  | object |  |  |  |  |
| `state.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `state.refName` | Reference Name | string |  |  |  |  |
| `supportedOperations` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `token` | Token | string |  |  |  |  |
| `tokenExpirationDate` | Token Expiration Date | object |  |  |  |  |
| `tokenFamily` |  | object |  |  |  |  |
| `tokenFamily.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `10`, `21` |
| `tokenFamily.refName` | Reference Name | string |  |  |  |  |
| `tokenNamespace` | Token Namespace | string |  |  |  |  |

## generalTokenCollection

Browser definition `generalTokenCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | generalToken[] |  |  | [`generalToken`](#generaltoken) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## generalTokenSelectOptions

Browser definition `generalTokenSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `instrumentType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportedOperations` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `tokenFamily` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

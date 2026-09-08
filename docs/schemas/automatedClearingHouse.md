# Schemas: automatedClearingHouse

Property tables for definitions owned by `automatedClearingHouse`.

Record page: [automatedClearingHouse](../records/automatedClearingHouse.md).

## Index

- [automatedClearingHouse](#automatedclearinghouse) — 28 properties
- [automatedClearingHouseCollection](#automatedclearinghousecollection) — 6 properties
- [automatedClearingHouseSelectOptions](#automatedclearinghouseselectoptions) — 6 properties

## automatedClearingHouse

Browser definition `automatedClearingHouse`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountOwnerName` | Account owner name | string |  |  |  |  |
| `accountType` |  | object |  |  |  |  |
| `accountType.id` | Internal identifier | string |  |  |  | `CORPORATE_CHECKING`, `SAVING`, `CHECKING` |
| `accountType.refName` | Reference Name | string |  |  |  |  |
| `bankAccountNumber` | Bank Account Number | string |  |  |  |  |
| `bankName` | Bank Name | string |  |  |  |  |
| `customerConsent` | Customer Consent | string |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `instrumentType` |  | object |  |  |  |  |
| `instrumentType.id` | Internal identifier | string |  |  |  | `1`, `2`, `13`, `3` |
| `instrumentType.refName` | Reference Name | string |  |  |  |  |
| `isDefault` | Default | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `limit` | Limit | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mask` | Mask | string |  |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `paymentMethod` |  | paymentMethod |  |  | [`paymentMethod`](paymentMethod.md#paymentmethod) |  |
| `preserveOnFile` | Preserve on File | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `routingNumber` | Routing Number | string |  |  |  |  |
| `state` |  | object |  |  |  |  |
| `state.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `state.refName` | Reference Name | string |  |  |  |  |
| `supportedOperations` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |

## automatedClearingHouseCollection

Browser definition `automatedClearingHouseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | automatedClearingHouse[] |  |  | [`automatedClearingHouse`](#automatedclearinghouse) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## automatedClearingHouseSelectOptions

Browser definition `automatedClearingHouseSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `instrumentType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportedOperations` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: paymentCard

Property tables for definitions owned by `paymentCard`.

Record page: [paymentCard](../records/paymentCard.md).

## Index

- [paymentCard](#paymentcard) — 35 properties
- [paymentCardCollection](#paymentcardcollection) — 6 properties
- [paymentCardSelectOptions](#paymentcardselectoptions) — 7 properties

## paymentCard

Browser definition `paymentCard`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cardBrand` |  | object |  |  |  |  |
| `cardBrand.id` | Internal identifier | string |  |  |  | `11`, `12`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `cardBrand.refName` | Reference Name | string |  |  |  |  |
| `cardNumber` | Payment Card Number | string |  |  |  |  |
| `cardType` |  | object |  |  |  |  |
| `cardType.id` | Internal identifier | string |  |  |  | `CREDIT`, `DEBIT` |
| `cardType.refName` | Reference Name | string |  |  |  |  |
| `customerCode` | Customer Code | string |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `expirationDate` | Expiration Date | object |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `instrumentType` |  | object |  |  |  |  |
| `instrumentType.id` | Internal identifier | string |  |  |  | `1`, `2`, `13`, `3` |
| `instrumentType.refName` | Reference Name | string |  |  |  |  |
| `isDefault` | Default | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `issueNumber` | Issue No. | string |  |  |  |  |
| `issuerIdNumber` | Issuer Identification Number | string |  |  |  |  |
| `lastFourDigits` | Last Four Digits | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mask` | Mask | string |  |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `nameOnCard` | Cardholder Name | string |  |  |  |  |
| `paymentMethod` |  | paymentMethod |  |  | [`paymentMethod`](paymentMethod.md#paymentmethod) |  |
| `preserveOnFile` | Preserve on File | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `state` |  | object |  |  |  |  |
| `state.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `state.refName` | Reference Name | string |  |  |  |  |
| `street` | Card Street | string |  |  |  |  |
| `supportedOperations` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `validFromDate` | Valid From / Start Date (MM/YYYY) | object |  |  |  |  |
| `zipCode` | Card Zip Code | string |  |  |  |  |

## paymentCardCollection

Browser definition `paymentCardCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | paymentCard[] |  |  | [`paymentCard`](#paymentcard) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paymentCardSelectOptions

Browser definition `paymentCardSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cardBrand` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `instrumentType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportedOperations` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

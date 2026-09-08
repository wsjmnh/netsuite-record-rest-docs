# Schemas: paymentCardToken

Property tables for definitions owned by `paymentCardToken`.

Record page: [paymentCardToken](../records/paymentCardToken.md).

## Index

- [paymentCardToken](#paymentcardtoken) — 35 properties
- [paymentCardTokenCollection](#paymentcardtokencollection) — 6 properties
- [paymentCardTokenSelectOptions](#paymentcardtokenselectoptions) — 8 properties

## paymentCardToken

Browser definition `paymentCardToken`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cardBrand` |  | object |  |  |  |  |
| `cardBrand.id` | Internal identifier | string |  |  |  | `11`, `12`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `cardBrand.refName` | Reference Name | string |  |  |  |  |
| `cardExpirationDate` | Expiration Date | object |  |  |  |  |
| `cardIssuerIdNumber` | Issuer Identification Number | string |  |  |  |  |
| `cardLastFourDigits` | Last Four Digits | string |  |  |  |  |
| `cardNameOnCard` | Cardholder Name | string |  |  |  |  |
| `cardType` |  | object |  |  |  |  |
| `cardType.id` | Internal identifier | string |  |  |  | `CREDIT`, `DEBIT` |
| `cardType.refName` | Reference Name | string |  |  |  |  |
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

## paymentCardTokenCollection

Browser definition `paymentCardTokenCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | paymentCardToken[] |  |  | [`paymentCardToken`](#paymentcardtoken) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paymentCardTokenSelectOptions

Browser definition `paymentCardTokenSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cardBrand` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `instrumentType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supportedOperations` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `tokenFamily` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: currencyRate

Property tables for definitions owned by `currencyRate`.

Record page: [currencyRate](../records/currencyRate.md).

## Index

- [currencyRate](#currencyrate) — 11 properties
- [currencyRateCollection](#currencyratecollection) — 6 properties
- [currencyRateSelectOptions](#currencyrateselectoptions) — 3 properties

## currencyRate

Browser definition `currencyRate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currencyRateType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fxSourceMethod` | Method | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `transactionCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |

## currencyRateCollection

Browser definition `currencyRateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | currencyRate[] |  |  | [`currencyRate`](#currencyrate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## currencyRateSelectOptions

Browser definition `currencyRateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currencyRateType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

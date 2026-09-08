# Schemas: budgetExchangeRate

Property tables for definitions owned by `budgetExchangeRate`.

Record page: [budgetExchangeRate](../records/budgetExchangeRate.md).

## Index

- [budgetExchangeRate](#budgetexchangerate) — 18 properties
- [budgetExchangeRateCollection](#budgetexchangeratecollection) — 6 properties
- [budgetExchangeRateSelectOptions](#budgetexchangerateselectoptions) — 6 properties

## budgetExchangeRate

Browser definition `budgetExchangeRate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `averageRate` | Average Exchange Rate | number | double |  |  |  |
| `currentRate` | Current Exchange Rate | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fromCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `fromSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `historicalRate` | Historical Exchange Rate | number | double |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isDerived` | Exchange Rate Derived | boolean |  |  |  |  |
| `isEliminationSubsidiary` | Is Elimination Subsidiary | boolean |  |  |  |  |
| `isPeriodClosed` | Period Closed | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `periodEndDate` | Period End Date | string | date |  |  |  |
| `periodStartDate` | Period Start Date | string | date |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `toSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## budgetExchangeRateCollection

Browser definition `budgetExchangeRateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | budgetExchangeRate[] |  |  | [`budgetExchangeRate`](#budgetexchangerate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## budgetExchangeRateSelectOptions

Browser definition `budgetExchangeRateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fromCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fromSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `toCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `toSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

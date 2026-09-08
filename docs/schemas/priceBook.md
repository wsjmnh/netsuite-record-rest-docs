# Schemas: priceBook

Property tables for definitions owned by `priceBook`.

Record page: [priceBook](../records/priceBook.md).

## Index

- [priceBook](#pricebook) — 9 properties
- [priceBook-priceIntervalCollection](#pricebook-priceintervalcollection) — 6 properties
- [priceBook-priceIntervalElement](#pricebook-priceintervalelement) — 40 properties
- [priceBookCollection](#pricebookcollection) — 6 properties
- [priceBookSelectOptions](#pricebookselectoptions) — 3 properties

## priceBook

Browser definition `priceBook`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `priceInterval` |  | priceBook-priceIntervalCollection |  |  | [`priceBook-priceIntervalCollection`](#pricebook-priceintervalcollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscriptionPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |

## priceBook-priceIntervalCollection

Browser definition `priceBook-priceIntervalCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | priceBook-priceIntervalElement[] |  |  | [`priceBook-priceIntervalElement`](#pricebook-priceintervalelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## priceBook-priceIntervalElement

Browser definition `priceBook-priceIntervalElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `chargeType` |  | object |  |  |  |  |
| `chargeType.id` | Internal identifier | string |  |  |  |  |
| `chargeType.refName` | Reference Name | string |  |  |  |  |
| `commitmentService` | Commitment Service | string |  |  |  |  |
| `discount` | Discount | number | double |  |  |  |
| `frequency` |  | object |  |  |  |  |
| `frequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `frequency.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `isRequired` | Required | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `multiplierLine` | Included Quantity Multiplier | string |  |  |  |  |
| `overageDiscount` | Overage Discount | number | double |  |  |  |
| `overageFrequency` |  | object |  |  |  |  |
| `overageFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `overageFrequency.refName` | Reference Name | string |  |  |  |  |
| `overagePricePlan` |  | pricePlan |  |  | [`pricePlan`](pricePlan.md#priceplan) |  |
| `overagePricingFrequency` |  | object |  |  |  |  |
| `overagePricingFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `overagePricingFrequency.refName` | Reference Name | string |  |  |  |  |
| `overagePricingRepeatEvery` | Overage Pricing Repeat Every | integer | int64 |  |  |  |
| `overageRepeatEvery` | Overage Repeat Every | integer | int64 |  |  |  |
| `prepayLine` | Prepay Line | string |  |  |  |  |
| `pricePlan` |  | pricePlan |  |  | [`pricePlan`](pricePlan.md#priceplan) |  |
| `pricingFrequency` |  | object |  |  |  |  |
| `pricingFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `pricingFrequency.refName` | Reference Name | string |  |  |  |  |
| `pricingRepeatEvery` | Pricing Repeat Every | integer | int64 |  |  |  |
| `prorateBy` |  | object |  |  |  |  |
| `prorateBy.id` | Internal identifier | string |  |  |  | `MONTH`, `DAY` |
| `prorateBy.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `repeatEvery` | Repeat Every | integer | int64 |  |  |  |
| `startOffsetUnit` |  | object |  |  |  |  |
| `startOffsetUnit.id` | Internal identifier | string |  |  |  | `MONTH`, `YEAR`, `WEEK` |
| `startOffsetUnit.refName` | Reference Name | string |  |  |  |  |
| `startOffsetValue` | Start On | integer | int64 |  |  |  |
| `subscriptionPlanLineNumber` | Line Number | integer | int64 |  |  |  |

## priceBookCollection

Browser definition `priceBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | priceBook[] |  |  | [`priceBook`](#pricebook) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## priceBookSelectOptions

Browser definition `priceBookSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

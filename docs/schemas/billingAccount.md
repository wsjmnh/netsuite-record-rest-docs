# Schemas: billingAccount

Property tables for definitions owned by `billingAccount`.

Record page: [billingAccount](../records/billingAccount.md).

## Index

- [billingAccount](#billingaccount) — 38 properties
- [billingAccountCollection](#billingaccountcollection) — 6 properties
- [billingAccountSelectOptions](#billingaccountselectoptions) — 14 properties

## billingAccount

Browser definition `billingAccount`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `autoName` | Auto | boolean |  |  |  |  |
| `billAddress` | Bill To | string |  |  |  |  |
| `billAddressList` | Bill To Select | string |  |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `cashSaleForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdBy` | Created By | string |  |  |  |  |
| `createdDate` | Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `customerDefault` | Customer Default | boolean |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `displayName` | Display Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `frequency` |  | object |  |  |  |  |
| `frequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `frequency.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `idNumber` | Account Number | string |  |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `invoiceForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lastBillCycleDate` | Last Bill Cycle Date | string | date |  |  |  |
| `lastBillDate` | Last Bill Date | string | date |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Account Description | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `nextBillCycleDate` |  | object |  |  |  |  |
| `nextBillCycleDate.id` | Internal identifier | string |  |  |  |  |
| `nextBillCycleDate.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `requestOffCycleInvoice` | Use Off-Cycle Invoice for Advance Charges | boolean |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` | Ship To Select | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## billingAccountCollection

Browser definition `billingAccountCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | billingAccount[] |  |  | [`billingAccount`](#billingaccount) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## billingAccountSelectOptions

Browser definition `billingAccountSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cashSaleForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `frequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `invoiceForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextBillCycleDate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

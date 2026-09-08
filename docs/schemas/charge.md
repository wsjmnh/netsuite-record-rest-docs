# Schemas: charge

Property tables for definitions owned by `charge`.

Record page: [charge](../records/charge.md).

## Index

- [charge](#charge) — 53 properties
- [chargeCollection](#chargecollection) — 6 properties
- [chargeSelectOptions](#chargeselectoptions) — 26 properties

## charge

Browser definition `charge`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `amountDetail` | Amount Detail | string |  |  |  |  |
| `billDate` | Bill Date | string | date |  |  |  |
| `billTo` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `billingAccount` |  | billingAccount |  |  | [`billingAccount`](billingAccount.md#billingaccount) |  |
| `billingItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `billingMode` |  | object |  |  |  |  |
| `billingMode.id` | Internal identifier | string |  |  |  | `IN_ARREARS`, `IN_ADVANCE`, `IMMEDIATE` |
| `billingMode.refName` | Reference Name | string |  |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `chargeDate` | Date | string | date |  |  |  |
| `chargeEmployee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `chargeType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `creditMemo` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `creditMemoLine` | Credit Memo Item Line | string |  |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `discountAmount` | Discount Amount | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `groupOrder` | Group Order | integer | int64 |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `invoice` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `invoiceLine` | Invoice Item Line | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `projectTask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `rule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `runId` | Charge Run ID | string |  |  |  |  |
| `salesOrder` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `salesOrderLine` | Sales Order Line | string |  |  |  |  |
| `serviceEndDate` | Service End Date | string | date |  |  |  |
| `serviceStartDate` | Service Start Date | string | date |  |  |  |
| `stage` |  | object |  |  |  |  |
| `stage.id` | Internal identifier | string |  |  |  | `NON_BILLABLE`, `READY_FOR_BILLING`, `HOLD_FOR_BILLING` |
| `stage.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `timeRecord` |  | timeBill |  |  | [`timeBill`](timeBill.md#timebill) |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `transactionLine` | Transaction Line | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |
| `use` |  | object |  |  |  |  |
| `use.id` | Internal identifier | string |  |  |  | `Forecast`, `Actual` |
| `use.refName` | Reference Name | string |  |  |  |  |

## chargeCollection

Browser definition `chargeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | charge[] |  |  | [`charge`](#charge) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## chargeSelectOptions

Browser definition `chargeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billTo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `chargeEmployee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `chargeType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `creditMemo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `invoice` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `projectTask` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `rule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrderLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `stage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeRecord` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `use` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

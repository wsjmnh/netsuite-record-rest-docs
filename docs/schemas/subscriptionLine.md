# Schemas: subscriptionLine

Property tables for definitions owned by `subscriptionLine`.

Record page: [subscriptionLine](../records/subscriptionLine.md).

## Index

- [subscriptionLine](#subscriptionline) — 54 properties
- [subscriptionLineCollection](#subscriptionlinecollection) — 6 properties
- [subscriptionLineSelectOptions](#subscriptionlineselectoptions) — 14 properties

## subscriptionLine

Browser definition `subscriptionLine`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `alignChargeWithSub` | Align Charge amounts with Subscription | boolean |  |  |  |  |
| `billingMode` |  | object |  |  |  |  |
| `billingMode.id` | Internal identifier | string |  |  |  | `IN_ARREARS`, `IN_ADVANCE`, `IMMEDIATE` |
| `billingMode.refName` | Reference Name | string |  |  |  |  |
| `catalogType` |  | object |  |  |  |  |
| `catalogType.id` | Internal identifier | string |  |  |  | `ADD_ON`, `OPTIONAL`, `REQUIRED` |
| `catalogType.refName` | Reference Name | string |  |  |  |  |
| `chargeCommitOnUsage` | Charge Commit On Usage | boolean |  |  |  |  |
| `chargePerUsageRecord` | Charge Per Usage Record | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Created Date | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `endDate` | End Date | string | date |  |  |  |
| `estimatedRevRecEndDate` | Estimated Revenue Recognition End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `firstBillDate` | First Bill Date | string | date |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeInRenewal` | Include In Renewal Subscription | boolean |  |  |  |  |
| `isIncluded` | Include | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `poNumber` | PO # | string |  |  |  |  |
| `prepaymentRemaining` | Prepayment Remaining | number | double |  |  |  |
| `prepaymentUsage` | Prepayment Usage | number | double |  |  |  |
| `prorateEndDate` | Prorate End Date | boolean |  |  |  |  |
| `prorateStartDate` | Prorate Start Date | boolean |  |  |  |  |
| `recurrenceStartDate` | Recurrence Start Date | string | date |  |  |  |
| `recurringAmount` | Recurring Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOption` |  | object |  |  |  |  |
| `revRecOption.id` | Internal identifier | string |  |  |  | `ONE_TIME`, `OVER_TERM` |
| `revRecOption.refName` | Reference Name | string |  |  |  |  |
| `saasCommitmentEndDate` | SaaS Metric Commitment End Date | string | date |  |  |  |
| `saasCommitmentStartDate` | SaaS Metric Commitment Start Date | string | date |  |  |  |
| `salesOrder` |  | salesOrder |  |  | [`salesOrder`](salesOrder.md#salesorder) |  |
| `salesOrderLineNumber` | Sales Order Line Number | integer | int64 |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subLineDiscount` | Discount | number | double |  |  |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `subscriptionLineStatus` |  | object |  |  |  |  |
| `subscriptionLineStatus.id` | Internal identifier | string |  |  |  | `NOT_INCLUDED`, `CLOSED`, `ACTIVE`, `TERMINATED`, `DRAFT`, `PENDING_ACTIVATION`, `SUSPENDED` |
| `subscriptionLineStatus.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLineType` |  | object |  |  |  |  |
| `subscriptionLineType.id` | Internal identifier | string |  |  |  |  |
| `subscriptionLineType.refName` | Reference Name | string |  |  |  |  |
| `subscriptionPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `subscriptionPlanLine` | Subscription Plan Line | string |  |  |  |  |
| `terminationDate` | Termination Date | string | date |  |  |  |
| `total` | Total | number | double |  |  |  |
| `totalDiscountAmount` | Total Discount Amount | number | double |  |  |  |
| `totalLineAmount` | Total Line Amount | number | double |  |  |  |

## subscriptionLineCollection

Browser definition `subscriptionLineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | subscriptionLine[] |  |  | [`subscriptionLine`](#subscriptionline) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionLineSelectOptions

Browser definition `subscriptionLineSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `catalogType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscription` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionLineStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionLineType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlanLine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

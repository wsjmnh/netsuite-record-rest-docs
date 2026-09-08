# Schemas: subscriptionPlan

Property tables for definitions owned by `subscriptionPlan`.

Record page: [subscriptionPlan](../records/subscriptionPlan.md).

## Index

- [subscriptionPlan](#subscriptionplan) — 37 properties
- [subscriptionPlan-memberCollection](#subscriptionplan-membercollection) — 6 properties
- [subscriptionPlan-memberElement](#subscriptionplan-memberelement) — 22 properties
- [subscriptionPlan-midtermUpliftCollection](#subscriptionplan-midtermupliftcollection) — 6 properties
- [subscriptionPlan-midtermUpliftElement](#subscriptionplan-midtermupliftelement) — 12 properties
- [subscriptionPlan-renewalupliftCollection](#subscriptionplan-renewalupliftcollection) — 6 properties
- [subscriptionPlan-renewalupliftElement](#subscriptionplan-renewalupliftelement) — 5 properties
- [subscriptionPlanCollection](#subscriptionplancollection) — 6 properties
- [subscriptionPlanSelectOptions](#subscriptionplanselectoptions) — 13 properties

## subscriptionPlan

Browser definition `subscriptionPlan`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advanceRenewalPeriodNumber` | Advance Renewal Period | integer | int64 |  |  |  |
| `advanceRenewalPeriodUnit` |  | object |  |  |  |  |
| `advanceRenewalPeriodUnit.id` | Internal identifier | string |  |  |  | `DAYS` |
| `advanceRenewalPeriodUnit.refName` | Reference Name | string |  |  |  |  |
| `autoRenewal` | Automatically Initiate Renewal Process | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultRenewalMethod` |  | object |  |  |  |  |
| `defaultRenewalMethod.id` | Internal identifier | string |  |  |  | `EXTEND_EXISTING_SUBSCRIPTION`, `CREATE_NEW_SUBSCRIPTION` |
| `defaultRenewalMethod.refName` | Reference Name | string |  |  |  |  |
| `defaultRenewalPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](#subscriptionplan) |  |
| `defaultRenewalTerm` |  | subscriptionTerm |  |  | [`subscriptionTerm`](subscriptionTerm.md#subscriptionterm) |  |
| `defaultRenewalTranType` |  | object |  |  |  |  |
| `defaultRenewalTranType.id` | Internal identifier | string |  |  |  | `Opprtnty`, `Estimate`, `SalesOrd` |
| `defaultRenewalTranType.refName` | Reference Name | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `initialTerm` |  | subscriptionTerm |  |  | [`subscriptionTerm`](subscriptionTerm.md#subscriptionterm) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `itemId` | Subscription Plan Name | string |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `member` |  | subscriptionPlan-memberCollection |  |  | [`subscriptionPlan-memberCollection`](#subscriptionplan-membercollection) |  |
| `midtermUplift` |  | subscriptionPlan-midtermUpliftCollection |  |  | [`subscriptionPlan-midtermUpliftCollection`](#subscriptionplan-midtermupliftcollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewaluplift` |  | subscriptionPlan-renewalupliftCollection |  |  | [`subscriptionPlan-renewalupliftCollection`](#subscriptionplan-renewalupliftcollection) |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |

## subscriptionPlan-memberCollection

Browser definition `subscriptionPlan-memberCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionPlan-memberElement[] |  |  | [`subscriptionPlan-memberElement`](#subscriptionplan-memberelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionPlan-memberElement

Browser definition `subscriptionPlan-memberElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingMode` |  | object |  |  |  |  |
| `billingMode.id` | Internal identifier | string |  |  |  | `IN_ARREARS`, `IN_ADVANCE` |
| `billingMode.refName` | Reference Name | string |  |  |  |  |
| `chargecommitonusage` | Charge Commit On Usage | boolean |  |  |  |  |
| `chargeperusagerecord` | Charge Per Usage Record | boolean |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isRequired` | Required | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `prorateEndDate` | Prorate End Date | boolean |  |  |  |  |
| `prorateStartDate` | Prorate Start Date | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalOption` |  | object |  |  |  |  |
| `renewalOption.id` | Internal identifier | string |  |  |  | `ALWAYS`, `NEVER`, `SAME_PLAN`, `DIFFERENT_PLAN` |
| `renewalOption.refName` | Reference Name | string |  |  |  |  |
| `revRecOption` |  | object |  |  |  |  |
| `revRecOption.id` | Internal identifier | string |  |  |  | `ONE_TIME`, `OVER_TERM` |
| `revRecOption.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLineType` |  | object |  |  |  |  |
| `subscriptionLineType.id` | Internal identifier | string |  |  |  |  |
| `subscriptionLineType.refName` | Reference Name | string |  |  |  |  |

## subscriptionPlan-midtermUpliftCollection

Browser definition `subscriptionPlan-midtermUpliftCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionPlan-midtermUpliftElement[] |  |  | [`subscriptionPlan-midtermUpliftElement`](#subscriptionplan-midtermupliftelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionPlan-midtermUpliftElement

Browser definition `subscriptionPlan-midtermUpliftElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `lineType` |  | object |  |  |  |  |
| `lineType.id` | Internal identifier | string |  |  |  |  |
| `lineType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `upliftFrequency` |  | object |  |  |  |  |
| `upliftFrequency.id` | Internal identifier | string |  |  |  | `ANNUALLY`, `MONTHLY` |
| `upliftFrequency.refName` | Reference Name | string |  |  |  |  |
| `upliftPercent` | % Uplift | number | double |  |  |  |
| `upliftRepeatEvery` | Repeat Every | integer | int64 |  |  |  |

## subscriptionPlan-renewalupliftCollection

Browser definition `subscriptionPlan-renewalupliftCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionPlan-renewalupliftElement[] |  |  | [`subscriptionPlan-renewalupliftElement`](#subscriptionplan-renewalupliftelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionPlan-renewalupliftElement

Browser definition `subscriptionPlan-renewalupliftElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalUplift` | % Renewal Uplift | number | double |  |  |  |

## subscriptionPlanCollection

Browser definition `subscriptionPlanCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | subscriptionPlan[] |  |  | [`subscriptionPlan`](#subscriptionplan) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionPlanSelectOptions

Browser definition `subscriptionPlanSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advanceRenewalPeriodUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalTranType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `initialTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

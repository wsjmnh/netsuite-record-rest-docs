# Schemas: subscription

Property tables for definitions owned by `subscription`.

Record page: [subscription](../records/subscription.md).

## Index

- [subscription](#subscription) — 64 properties
- [subscription-midtermUpliftCollection](#subscription-midtermupliftcollection) — 6 properties
- [subscription-midtermUpliftElement](#subscription-midtermupliftelement) — 13 properties
- [subscription-priceIntervalCollection](#subscription-priceintervalcollection) — 6 properties
- [subscription-priceIntervalElement](#subscription-priceintervalelement) — 51 properties
- [subscription-renewalupliftCollection](#subscription-renewalupliftcollection) — 6 properties
- [subscription-renewalupliftElement](#subscription-renewalupliftelement) — 5 properties
- [subscription-subscriptionLineCollection](#subscription-subscriptionlinecollection) — 6 properties
- [subscription-subscriptionLineElement](#subscription-subscriptionlineelement) — 42 properties
- [subscriptionCollection](#subscriptioncollection) — 6 properties
- [subscriptionSelectOptions](#subscriptionselectoptions) — 21 properties

## subscription

Browser definition `subscription`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `activeTotalContractValue` | Active Total Contract Value | number | double |  |  |  |
| `advanceRenewalPeriodNumber` | Advance Renewal Period | integer | int64 |  |  |  |
| `advanceRenewalPeriodUnit` |  | object |  |  |  |  |
| `advanceRenewalPeriodUnit.id` | Internal identifier | string |  |  |  | `DAYS` |
| `advanceRenewalPeriodUnit.refName` | Reference Name | string |  |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `autoRenewal` | Automatically Initiate Renewal Process | boolean |  |  |  |  |
| `billingAccount` |  | billingAccount |  |  | [`billingAccount`](billingAccount.md#billingaccount) |  |
| `billingAccountStartDate` | Start Date | string | date |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `billingSubscriptionStatus` |  | object |  |  |  |  |
| `billingSubscriptionStatus.id` | Internal identifier | string |  |  |  | `ACTIVE`, `PENDING_ACTIVATION`, `SUSPENDED`, `DRAFT`, `CLOSED`, `TERMINATED`, `NOT_INCLUDED` |
| `billingSubscriptionStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Created Date | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `defaultRenewalMethod` |  | object |  |  |  |  |
| `defaultRenewalMethod.id` | Internal identifier | string |  |  |  | `EXTEND_EXISTING_SUBSCRIPTION`, `CREATE_NEW_SUBSCRIPTION` |
| `defaultRenewalMethod.refName` | Reference Name | string |  |  |  |  |
| `defaultRenewalPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `defaultRenewalPriceBook` |  | priceBook |  |  | [`priceBook`](priceBook.md#pricebook) |  |
| `defaultRenewalTerm` |  | subscriptionTerm |  |  | [`subscriptionTerm`](subscriptionTerm.md#subscriptionterm) |  |
| `defaultRenewalTranType` |  | object |  |  |  |  |
| `defaultRenewalTranType.id` | Internal identifier | string |  |  |  | `Opprtnty`, `Estimate`, `SalesOrd` |
| `defaultRenewalTranType.refName` | Reference Name | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `endDate` | End Date | string | date |  |  |  |
| `estimatedRevRecEndDate` | Estimated Revenue Recognition End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `frequency` |  | object |  |  |  |  |
| `frequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `frequency.refName` | Reference Name | string |  |  |  |  |
| `generateModificationElements` | Generate Modification Elements | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `idNumber` | Number | string |  |  |  |  |
| `initialTerm` |  | subscriptionTerm |  |  | [`subscriptionTerm`](subscriptionTerm.md#subscriptionterm) |  |
| `lastBillCycleDate` | Last Bill Cycle Date | string | date |  |  |  |
| `lastBillDate` | Last Bill Date | string | date |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `midtermUplift` |  | subscription-midtermUpliftCollection |  |  | [`subscription-midtermUpliftCollection`](#subscription-midtermupliftcollection) |  |
| `name` | Name | string |  |  |  |  |
| `nextBillCycleDate` | Next Bill Cycle Date | string | date |  |  |  |
| `nextRenewalStartDate` | Next Renewal Start Date | string | date |  |  |  |
| `pendingTotalContractValue` | Pending Total Contract Value | number | double |  |  |  |
| `priceBook` |  | priceBook |  |  | [`priceBook`](priceBook.md#pricebook) |  |
| `priceInterval` |  | subscription-priceIntervalCollection |  |  | [`subscription-priceIntervalCollection`](#subscription-priceintervalcollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalNumber` | Number of Renewal | integer | int64 |  |  |  |
| `renewaluplift` |  | subscription-renewalupliftCollection |  |  | [`subscription-renewalupliftCollection`](#subscription-renewalupliftcollection) |  |
| `salesOrder` |  | salesOrder |  |  | [`salesOrder`](salesOrder.md#salesorder) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subscriptionLine` |  | subscription-subscriptionLineCollection |  |  | [`subscription-subscriptionLineCollection`](#subscription-subscriptionlinecollection) |  |
| `subscriptionPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `subscriptionPlanName` | Subscription Plan Name | string |  |  |  |  |
| `subscriptionRevision` | Subscription Revision | integer | int64 |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `totalActiveCommitPlusOverage` | Total Active Commit Plus Overage | number | double |  |  |  |
| `totalActiveOneTime` | Total Active One-Time | number | double |  |  |  |
| `totalActivePrepaidAmount` | Total Active Prepaid Amount | number | double |  |  |  |
| `totalActiveRecurring` | Total Active Recurring | number | double |  |  |  |
| `totalActiveUsage` | Total Active Usage | number | double |  |  |  |

## subscription-midtermUpliftCollection

Browser definition `subscription-midtermUpliftCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscription-midtermUpliftElement[] |  |  | [`subscription-midtermUpliftElement`](#subscription-midtermupliftelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscription-midtermUpliftElement

Browser definition `subscription-midtermUpliftElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `lineType` |  | object |  |  |  |  |
| `lineType.id` | Internal identifier | string |  |  |  |  |
| `lineType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `upliftDateDisplayViewMode` | Uplift Start Date | string |  |  |  |  |
| `upliftFrequency` |  | object |  |  |  |  |
| `upliftFrequency.id` | Internal identifier | string |  |  |  | `ANNUALLY`, `MONTHLY` |
| `upliftFrequency.refName` | Reference Name | string |  |  |  |  |
| `upliftPercent` | % Uplift | number | double |  |  |  |
| `upliftRepeatEvery` | Repeat Every | integer | int64 |  |  |  |

## subscription-priceIntervalCollection

Browser definition `subscription-priceIntervalCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscription-priceIntervalElement[] |  |  | [`subscription-priceIntervalElement`](#subscription-priceintervalelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscription-priceIntervalElement

Browser definition `subscription-priceIntervalElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `catalogType` |  | object |  |  |  |  |
| `catalogType.id` | Internal identifier | string |  |  |  | `ADD_ON`, `OPTIONAL`, `REQUIRED` |
| `catalogType.refName` | Reference Name | string |  |  |  |  |
| `chargeType` |  | object |  |  |  |  |
| `chargeType.id` | Internal identifier | string |  |  |  |  |
| `chargeType.refName` | Reference Name | string |  |  |  |  |
| `commitmentservice` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `discount` | Discount | number | double |  |  |  |
| `frequency` |  | object |  |  |  |  |
| `frequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `frequency.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `includedQuantity` | Included Quantity | number | float |  |  |  |
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
| `prepayLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `pricePlan` |  | pricePlan |  |  | [`pricePlan`](pricePlan.md#priceplan) |  |
| `pricingFrequency` |  | object |  |  |  |  |
| `pricingFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `pricingFrequency.refName` | Reference Name | string |  |  |  |  |
| `pricingRepeatEvery` | Pricing Repeat Every | integer | int64 |  |  |  |
| `prorateBy` |  | object |  |  |  |  |
| `prorateBy.id` | Internal identifier | string |  |  |  | `MONTH`, `DAY` |
| `prorateBy.refName` | Reference Name | string |  |  |  |  |
| `proratebyoption` |  | object |  |  |  |  |
| `proratebyoption.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `proratebyoption.refName` | Reference Name | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `recurringAmount` | Recurring Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `repeatEvery` | Repeat Every | integer | int64 |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `startOffsetValue` | Start On | integer | int64 |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOT_INCLUDED`, `CLOSED`, `ACTIVE`, `TERMINATED`, `DRAFT`, `PENDING_ACTIVATION`, `SUSPENDED` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscriptionPlanLineNumber` | Line Number | integer | int64 |  |  |  |
| `totalintervalvalue` | Total Interval Value | number | double |  |  |  |
| `upliftpercent` | % Uplift | number | double |  |  |  |

## subscription-renewalupliftCollection

Browser definition `subscription-renewalupliftCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscription-renewalupliftElement[] |  |  | [`subscription-renewalupliftElement`](#subscription-renewalupliftelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscription-renewalupliftElement

Browser definition `subscription-renewalupliftElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalUplift` | % Renewal Uplift | number | double |  |  |  |

## subscription-subscriptionLineCollection

Browser definition `subscription-subscriptionLineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscription-subscriptionLineElement[] |  |  | [`subscription-subscriptionLineElement`](#subscription-subscriptionlineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscription-subscriptionLineElement

Browser definition `subscription-subscriptionLineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingMode` |  | object |  |  |  |  |
| `billingMode.id` | Internal identifier | string |  |  |  | `IN_ARREARS`, `IN_ADVANCE` |
| `billingMode.refName` | Reference Name | string |  |  |  |  |
| `catalogType` |  | object |  |  |  |  |
| `catalogType.id` | Internal identifier | string |  |  |  | `ADD_ON`, `OPTIONAL`, `REQUIRED` |
| `catalogType.refName` | Reference Name | string |  |  |  |  |
| `changeOrderLine` |  | integer | int64 |  |  |  |
| `chargeCommitOnUsage` | Charge Commit On Usage | boolean |  |  |  |  |
| `chargePerUsageRecord` | Charge Per Usage Record | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `discount` | Discount | number | double |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `firstBillDate` | First Bill Date | string | date |  |  |  |
| `includeInRenewal` | Include In Renewal Subscription | boolean |  |  |  |  |
| `isIncluded` | Include | boolean |  |  |  |  |
| `isRequired` |  | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `planItem` |  | integer | int64 |  |  |  |
| `prorateEndDate` | Prorate End Date | boolean |  |  |  |  |
| `prorateStartDate` | Prorate Start Date | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `recurrenceStartDate` | Recurrence Start Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalOption` |  | string |  |  |  |  |
| `revRecOption` |  | object |  |  |  |  |
| `revRecOption.id` | Internal identifier | string |  |  |  | `ONE_TIME`, `OVER_TERM` |
| `revRecOption.refName` | Reference Name | string |  |  |  |  |
| `saasCommitmentEndDate` | SaaS Metric Commitment End Date | string | date |  |  |  |
| `saasCommitmentStartDate` | SaaS Metric Commitment Start Date | string | date |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOT_INCLUDED`, `CLOSED`, `ACTIVE`, `TERMINATED`, `DRAFT`, `PENDING_ACTIVATION`, `SUSPENDED` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLine` |  | integer | int64 |  |  |  |
| `subscriptionLineType` |  | object |  |  |  |  |
| `subscriptionLineType.id` | Internal identifier | string |  |  |  |  |
| `subscriptionLineType.refName` | Reference Name | string |  |  |  |  |
| `terminationDate` | Termination Date | string | date |  |  |  |

## subscriptionCollection

Browser definition `subscriptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | subscription[] |  |  | [`subscription`](#subscription) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionSelectOptions

Browser definition `subscriptionSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advanceRenewalPeriodUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalPriceBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultRenewalTranType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `frequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `initialTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priceBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

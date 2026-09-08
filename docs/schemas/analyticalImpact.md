# Schemas: analyticalImpact

Property tables for definitions owned by `analyticalImpact`.

Record page: [analyticalImpact](../records/analyticalImpact.md).

## Index

- [analyticalImpact](#analyticalimpact) — 36 properties
- [analyticalImpact-analyticalImpactEventCollection](#analyticalimpact-analyticalimpacteventcollection) — 6 properties
- [analyticalImpact-analyticalImpactEventElement](#analyticalimpact-analyticalimpacteventelement) — 22 properties
- [analyticalImpact-analyticalImpactLinkCollection](#analyticalimpact-analyticalimpactlinkcollection) — 6 properties
- [analyticalImpact-analyticalImpactLinkElement](#analyticalimpact-analyticalimpactlinkelement) — 7 properties
- [analyticalImpact-relatedRenewalsCollection](#analyticalimpact-relatedrenewalscollection) — 6 properties
- [analyticalImpact-relatedRenewalsElement](#analyticalimpact-relatedrenewalselement) — 5 properties
- [analyticalImpact-relatedSubscriptionChangeOrdersCollection](#analyticalimpact-relatedsubscriptionchangeorderscollection) — 6 properties
- [analyticalImpact-relatedSubscriptionChangeOrdersElement](#analyticalimpact-relatedsubscriptionchangeorderselement) — 4 properties
- [analyticalImpact-relatedSubscriptionLinesCollection](#analyticalimpact-relatedsubscriptionlinescollection) — 6 properties
- [analyticalImpact-relatedSubscriptionLinesElement](#analyticalimpact-relatedsubscriptionlineselement) — 5 properties
- [analyticalImpact-relatedSubscriptionsCollection](#analyticalimpact-relatedsubscriptionscollection) — 6 properties
- [analyticalImpact-relatedSubscriptionsElement](#analyticalimpact-relatedsubscriptionselement) — 6 properties
- [analyticalImpact-relatedTransactionLinesCollection](#analyticalimpact-relatedtransactionlinescollection) — 6 properties
- [analyticalImpact-relatedTransactionLinesElement](#analyticalimpact-relatedtransactionlineselement) — 6 properties
- [analyticalImpactCollection](#analyticalimpactcollection) — 6 properties
- [analyticalImpactSelectOptions](#analyticalimpactselectoptions) — 10 properties

## analyticalImpact

Browser definition `analyticalImpact`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `acquisitionMonthEndDate` | Acquisition Month End Date | string | date |  |  |  |
| `analyticalImpactEvent` |  | analyticalImpact-analyticalImpactEventCollection |  |  | [`analyticalImpact-analyticalImpactEventCollection`](#analyticalimpact-analyticalimpacteventcollection) |  |
| `analyticalImpactLink` |  | analyticalImpact-analyticalImpactLinkCollection |  |  | [`analyticalImpact-analyticalImpactLinkCollection`](#analyticalimpact-analyticalimpactlinkcollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `commitmentEndDate` | Commitment End Date | string | date |  |  |  |
| `commitmentStartDate` | Commitment Start Date | string | date |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `ignore` | Ignore | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedRenewals` |  | analyticalImpact-relatedRenewalsCollection |  |  | [`analyticalImpact-relatedRenewalsCollection`](#analyticalimpact-relatedrenewalscollection) |  |
| `relatedSubscriptionChangeOrders` |  | analyticalImpact-relatedSubscriptionChangeOrdersCollection |  |  | [`analyticalImpact-relatedSubscriptionChangeOrdersCollection`](#analyticalimpact-relatedsubscriptionchangeorderscollection) |  |
| `relatedSubscriptionLines` |  | analyticalImpact-relatedSubscriptionLinesCollection |  |  | [`analyticalImpact-relatedSubscriptionLinesCollection`](#analyticalimpact-relatedsubscriptionlinescollection) |  |
| `relatedSubscriptions` |  | analyticalImpact-relatedSubscriptionsCollection |  |  | [`analyticalImpact-relatedSubscriptionsCollection`](#analyticalimpact-relatedsubscriptionscollection) |  |
| `relatedTransactionLines` |  | analyticalImpact-relatedTransactionLinesCollection |  |  | [`analyticalImpact-relatedTransactionLinesCollection`](#analyticalimpact-relatedtransactionlinescollection) |  |
| `renewedFrom` |  | analyticalImpact |  |  | [`analyticalImpact`](#analyticalimpact) |  |
| `source` | Source | string |  |  |  |  |
| `sourceCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `sourceLine` | Source Line | string |  |  |  |  |
| `sourceRecordType` |  | object |  |  |  |  |
| `sourceRecordType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9` |
| `sourceRecordType.refName` | Reference Name | string |  |  |  |  |
| `sourceStatus` | Source Status | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `termInMonths` | Term In Months | string |  |  |  |  |

## analyticalImpact-analyticalImpactEventCollection

Browser definition `analyticalImpact-analyticalImpactEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-analyticalImpactEventElement[] |  |  | [`analyticalImpact-analyticalImpactEventElement`](#analyticalimpact-analyticalimpacteventelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-analyticalImpactEventElement

Browser definition `analyticalImpact-analyticalImpactEventElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `adjustImpactCategory` |  | object |  |  |  |  |
| `adjustImpactCategory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6` |
| `adjustImpactCategory.refName` | Reference Name | string |  |  |  |  |
| `adjustImpactSubcategory` |  | impactSubcategory |  |  | [`impactSubcategory`](impactSubcategory.md#impactsubcategory) |  |
| `adjustMonthlyImpactAmount` | Adjust Monthly Impact Amount | number | double |  |  |  |
| `commitmentDate` | Commitment Date | string | date |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `eventNumber` | Event Number | integer | int64 |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `impactCategory` |  | object |  |  |  |  |
| `impactCategory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6` |
| `impactCategory.refName` | Reference Name | string |  |  |  |  |
| `impactLevel` | Impact Level | string |  |  |  |  |
| `impactSubcategory` |  | impactSubcategory |  |  | [`impactSubcategory`](impactSubcategory.md#impactsubcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `monthlyImpactAmount` | Monthly Impact Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `remainingImpactCategory` |  | object |  |  |  |  |
| `remainingImpactCategory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6` |
| `remainingImpactCategory.refName` | Reference Name | string |  |  |  |  |
| `remainingImpactSubcategory` |  | impactSubcategory |  |  | [`impactSubcategory`](impactSubcategory.md#impactsubcategory) |  |
| `remainingMonthlyImpactAmount` | Remaining Monthly Impact Amount | number | double |  |  |  |

## analyticalImpact-analyticalImpactLinkCollection

Browser definition `analyticalImpact-analyticalImpactLinkCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-analyticalImpactLinkElement[] |  |  | [`analyticalImpact-analyticalImpactLinkElement`](#analyticalimpact-analyticalimpactlinkelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-analyticalImpactLinkElement

Browser definition `analyticalImpact-analyticalImpactLinkElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `linkEndDate` | End Date | string | date |  |  |  |
| `linkStartDate` | Start Date | string | date |  |  |  |
| `linkType` | Link Type | string |  |  |  |  |
| `linkedRecordName` | Source | string |  |  |  |  |
| `linkedRecordType` | Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## analyticalImpact-relatedRenewalsCollection

Browser definition `analyticalImpact-relatedRenewalsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-relatedRenewalsElement[] |  |  | [`analyticalImpact-relatedRenewalsElement`](#analyticalimpact-relatedrenewalselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-relatedRenewalsElement

Browser definition `analyticalImpact-relatedRenewalsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `linkType` | Link Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewal` |  | analyticalImpact |  |  | [`analyticalImpact`](#analyticalimpact) |  |
| `renewalId` | Record ID | number | double |  |  |  |

## analyticalImpact-relatedSubscriptionChangeOrdersCollection

Browser definition `analyticalImpact-relatedSubscriptionChangeOrdersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-relatedSubscriptionChangeOrdersElement[] |  |  | [`analyticalImpact-relatedSubscriptionChangeOrdersElement`](#analyticalimpact-relatedsubscriptionchangeorderselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-relatedSubscriptionChangeOrdersElement

Browser definition `analyticalImpact-relatedSubscriptionChangeOrdersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscriptionChangeOrder` |  | subscriptionChangeOrder |  |  | [`subscriptionChangeOrder`](subscriptionChangeOrder.md#subscriptionchangeorder) |  |
| `subscriptionChangeOrderId` | Record ID | number | double |  |  |  |

## analyticalImpact-relatedSubscriptionLinesCollection

Browser definition `analyticalImpact-relatedSubscriptionLinesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-relatedSubscriptionLinesElement[] |  |  | [`analyticalImpact-relatedSubscriptionLinesElement`](#analyticalimpact-relatedsubscriptionlineselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-relatedSubscriptionLinesElement

Browser definition `analyticalImpact-relatedSubscriptionLinesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `linkType` | Link Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `subscriptionLineId` | Record ID | number | double |  |  |  |

## analyticalImpact-relatedSubscriptionsCollection

Browser definition `analyticalImpact-relatedSubscriptionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-relatedSubscriptionsElement[] |  |  | [`analyticalImpact-relatedSubscriptionsElement`](#analyticalimpact-relatedsubscriptionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-relatedSubscriptionsElement

Browser definition `analyticalImpact-relatedSubscriptionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `linkTypeName` | Link Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `recordType` | Record Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `subscriptionId` | Record ID | number | double |  |  |  |

## analyticalImpact-relatedTransactionLinesCollection

Browser definition `analyticalImpact-relatedTransactionLinesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | analyticalImpact-relatedTransactionLinesElement[] |  |  | [`analyticalImpact-relatedTransactionLinesElement`](#analyticalimpact-relatedtransactionlineselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpact-relatedTransactionLinesElement

Browser definition `analyticalImpact-relatedTransactionLinesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `linkType` | Link Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourceType` | Source Type | string |  |  |  |  |
| `transaction` | Transaction | string |  |  |  |  |
| `transactionLine` | Transaction Line | string |  |  |  |  |

## analyticalImpactCollection

Browser definition `analyticalImpactCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | analyticalImpact[] |  |  | [`analyticalImpact`](#analyticalimpact) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## analyticalImpactSelectOptions

Browser definition `analyticalImpactSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewedFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceRecordType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

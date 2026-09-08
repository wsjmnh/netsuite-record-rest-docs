# Schemas: campaign

Property tables for definitions owned by `campaign`.

Record page: [campaign](../records/campaign.md).

## Index

- [campaign](#campaign) — 43 properties
- [campaign-campaignDirectMailCollection](#campaign-campaigndirectmailcollection) — 6 properties
- [campaign-campaignDirectMailElement](#campaign-campaigndirectmailelement) — 16 properties
- [campaign-campaignDripCollection](#campaign-campaigndripcollection) — 6 properties
- [campaign-campaignDripElement](#campaign-campaigndripelement) — 11 properties
- [campaign-campaignEmailCollection](#campaign-campaignemailcollection) — 6 properties
- [campaign-campaignEmailElement](#campaign-campaignemailelement) — 18 properties
- [campaign-campaignEventCollection](#campaign-campaigneventcollection) — 6 properties
- [campaign-campaignEventElement](#campaign-campaigneventelement) — 15 properties
- [campaign-defaultEventCollection](#campaign-defaulteventcollection) — 6 properties
- [campaign-defaultEventElement](#campaign-defaulteventelement) — 8 properties
- [campaignCollection](#campaigncollection) — 6 properties
- [campaignSelectOptions](#campaignselectoptions) — 10 properties

## campaign

Browser definition `campaign`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `audience` |  | campaignAudience |  |  | [`campaignAudience`](campaignAudience.md#campaignaudience) |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `baseCost` | Cost | number | double |  |  |  |
| `campaignDirectMail` |  | campaign-campaignDirectMailCollection |  |  | [`campaign-campaignDirectMailCollection`](#campaign-campaigndirectmailcollection) |  |
| `campaignDrip` |  | campaign-campaignDripCollection |  |  | [`campaign-campaignDripCollection`](#campaign-campaigndripcollection) |  |
| `campaignEmail` |  | campaign-campaignEmailCollection |  |  | [`campaign-campaignEmailCollection`](#campaign-campaignemailcollection) |  |
| `campaignEvent` |  | campaign-campaignEventCollection |  |  | [`campaign-campaignEventCollection`](#campaign-campaigneventcollection) |  |
| `campaignId` | ID | string |  |  |  |  |
| `category` |  | campaignCategory |  |  | [`campaignCategory`](campaignCategory.md#campaigncategory) |  |
| `convCostPerCustomer` | Cost per Purchaser | number | double |  |  |  |
| `conversions` | Number of Purchasers | integer | int64 |  |  |  |
| `cost` | Total Cost | number | double |  |  |  |
| `costPerCustomer` | Cost Per Lead | number | double |  |  |  |
| `createdDate` | Created Date | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultEvent` |  | campaign-defaultEventCollection |  |  | [`campaign-defaultEventCollection`](#campaign-defaulteventcollection) |  |
| `endDate` | End Date | string | date |  |  |  |
| `eventNumber` | Number | integer | int64 |  |  |  |
| `expectedRevenue` | Projected Income | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `family` |  | campaignFamily |  |  | [`campaignFamily`](campaignFamily.md#campaignfamily) |  |
| `id` | Internal ID | string |  |  |  |  |
| `isDefaultLeadSource` | Default Lead Source | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `item` |  | kitItemCollection |  |  | [`kitItemCollection`](kitItem.md#kititemcollection) |  |
| `keyword` | Keyword | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `leadsGenerated` | Leads Generated | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Description | string |  |  |  |  |
| `offer` |  | campaignOffer |  |  | [`campaignOffer`](campaignOffer.md#campaignoffer) |  |
| `owner` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `profit` | Profit | number | double |  |  |  |
| `promotionCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `roi` | Return on Investment | number | double |  |  |  |
| `searchEngine` |  | campaignSearchEngine |  |  | [`campaignSearchEngine`](campaignSearchEngine.md#campaignsearchengine) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `title` | Title | string |  |  |  |  |
| `totalRevenue` | Revenue | number | double |  |  |  |
| `uniqueVisitors` | Unique Visitors | integer | int64 |  |  |  |
| `url` | URL | string |  |  |  |  |
| `vertical` |  | campaignVertical |  |  | [`campaignVertical`](campaignVertical.md#campaignvertical) |  |

## campaign-campaignDirectMailCollection

Browser definition `campaign-campaignDirectMailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaign-campaignDirectMailElement[] |  |  | [`campaign-campaignDirectMailElement`](#campaign-campaigndirectmailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaign-campaignDirectMailElement

Browser definition `campaign-campaignDirectMailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `campaignGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `channel` |  | campaignChannel |  |  | [`campaignChannel`](campaignChannel.md#campaignchannel) |  |
| `cost` | Cost | number | double |  |  |  |
| `dateScheduled` | Date | string | date |  |  |  |
| `description` | Title | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTART`, `COMPLETE`, `EXECUTE`, `PROGRESS` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |
| `template` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## campaign-campaignDripCollection

Browser definition `campaign-campaignDripCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaign-campaignDripElement[] |  |  | [`campaign-campaignDripElement`](#campaign-campaigndripelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaign-campaignDripElement

Browser definition `campaign-campaignDripElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `channel` |  | campaignChannel |  |  | [`campaignChannel`](campaignChannel.md#campaignchannel) |  |
| `cost` | Cost | number | double |  |  |  |
| `description` | Title | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |
| `template` |  | campaignTemplate |  |  | [`campaignTemplate`](campaignTemplate.md#campaigntemplate) |  |

## campaign-campaignEmailCollection

Browser definition `campaign-campaignEmailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaign-campaignEmailElement[] |  |  | [`campaign-campaignEmailElement`](#campaign-campaignemailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaign-campaignEmailElement

Browser definition `campaign-campaignEmailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `campaignGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `channel` |  | campaignChannel |  |  | [`campaignChannel`](campaignChannel.md#campaignchannel) |  |
| `cost` | Cost | number | double |  |  |  |
| `dateScheduled` | Date | string | date |  |  |  |
| `description` | Title | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTART`, `PROGRESS`, `EXECUTE`, `SENT`, `FAILED` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |
| `template` |  | campaignTemplate |  |  | [`campaignTemplate`](campaignTemplate.md#campaigntemplate) |  |
| `testCell` | Test Cell | string |  |  |  |  |
| `timeScheduled` | Time | string |  |  |  |  |

## campaign-campaignEventCollection

Browser definition `campaign-campaignEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaign-campaignEventElement[] |  |  | [`campaign-campaignEventElement`](#campaign-campaigneventelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaign-campaignEventElement

Browser definition `campaign-campaignEventElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `campaignGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `channel` |  | campaignChannel |  |  | [`campaignChannel`](campaignChannel.md#campaignchannel) |  |
| `cost` | Cost | number | double |  |  |  |
| `dateScheduled` | Date | string | date |  |  |  |
| `description` | Title | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTART`, `COMPLETE`, `EXECUTE`, `PROGRESS` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |

## campaign-defaultEventCollection

Browser definition `campaign-defaultEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaign-defaultEventElement[] |  |  | [`campaign-defaultEventElement`](#campaign-defaulteventelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaign-defaultEventElement

Browser definition `campaign-defaultEventElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `dScheduled` | Date | string | date-time |  |  |  |
| `description` | Title | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` | Status | string |  |  |  |  |

## campaignCollection

Browser definition `campaignCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaign[] |  |  | [`campaign`](#campaign) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignSelectOptions

Browser definition `campaignSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `audience` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `family` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `offer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `owner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `promotionCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchEngine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vertical` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

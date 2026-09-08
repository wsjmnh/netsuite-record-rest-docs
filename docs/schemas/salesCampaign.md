# Schemas: salesCampaign

Property tables for definitions owned by `salesCampaign`.

Record page: [salesCampaign](../records/salesCampaign.md).

## Index

- [salesCampaign](#salescampaign) — 44 properties
- [salesCampaign-campaignDirectMailCollection](#salescampaign-campaigndirectmailcollection) — 6 properties
- [salesCampaign-campaignDirectMailElement](#salescampaign-campaigndirectmailelement) — 16 properties
- [salesCampaign-campaignDripCollection](#salescampaign-campaigndripcollection) — 6 properties
- [salesCampaign-campaignDripElement](#salescampaign-campaigndripelement) — 11 properties
- [salesCampaign-campaignEmailCollection](#salescampaign-campaignemailcollection) — 6 properties
- [salesCampaign-campaignEmailElement](#salescampaign-campaignemailelement) — 18 properties
- [salesCampaign-campaignEventCollection](#salescampaign-campaigneventcollection) — 6 properties
- [salesCampaign-campaignEventElement](#salescampaign-campaigneventelement) — 15 properties
- [salesCampaign-defaultEventCollection](#salescampaign-defaulteventcollection) — 6 properties
- [salesCampaign-defaultEventElement](#salescampaign-defaulteventelement) — 8 properties
- [salesCampaignCollection](#salescampaigncollection) — 6 properties
- [salesCampaignSelectOptions](#salescampaignselectoptions) — 11 properties

## salesCampaign

Browser definition `salesCampaign`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `audience` |  | campaignAudience |  |  | [`campaignAudience`](campaignAudience.md#campaignaudience) |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `baseCost` | Cost | number | double |  |  |  |
| `campaignDirectMail` |  | salesCampaign-campaignDirectMailCollection |  |  | [`salesCampaign-campaignDirectMailCollection`](#salescampaign-campaigndirectmailcollection) |  |
| `campaignDrip` |  | salesCampaign-campaignDripCollection |  |  | [`salesCampaign-campaignDripCollection`](#salescampaign-campaigndripcollection) |  |
| `campaignEmail` |  | salesCampaign-campaignEmailCollection |  |  | [`salesCampaign-campaignEmailCollection`](#salescampaign-campaignemailcollection) |  |
| `campaignEvent` |  | salesCampaign-campaignEventCollection |  |  | [`salesCampaign-campaignEventCollection`](#salescampaign-campaigneventcollection) |  |
| `campaignId` | ID | string |  |  |  |  |
| `category` |  | campaignCategory |  |  | [`campaignCategory`](campaignCategory.md#campaigncategory) |  |
| `convCostPerCustomer` | Cost per Purchaser | number | double |  |  |  |
| `conversions` | Number of Purchasers | integer | int64 |  |  |  |
| `cost` | Total Cost | number | double |  |  |  |
| `costPerCustomer` | Cost Per Lead | number | double |  |  |  |
| `createdDate` | Created Date | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultEvent` |  | salesCampaign-defaultEventCollection |  |  | [`salesCampaign-defaultEventCollection`](#salescampaign-defaulteventcollection) |  |
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
| `ownerrole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
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

## salesCampaign-campaignDirectMailCollection

Browser definition `salesCampaign-campaignDirectMailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesCampaign-campaignDirectMailElement[] |  |  | [`salesCampaign-campaignDirectMailElement`](#salescampaign-campaigndirectmailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaign-campaignDirectMailElement

Browser definition `salesCampaign-campaignDirectMailElement`.

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

## salesCampaign-campaignDripCollection

Browser definition `salesCampaign-campaignDripCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesCampaign-campaignDripElement[] |  |  | [`salesCampaign-campaignDripElement`](#salescampaign-campaigndripelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaign-campaignDripElement

Browser definition `salesCampaign-campaignDripElement`.

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

## salesCampaign-campaignEmailCollection

Browser definition `salesCampaign-campaignEmailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesCampaign-campaignEmailElement[] |  |  | [`salesCampaign-campaignEmailElement`](#salescampaign-campaignemailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaign-campaignEmailElement

Browser definition `salesCampaign-campaignEmailElement`.

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

## salesCampaign-campaignEventCollection

Browser definition `salesCampaign-campaignEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesCampaign-campaignEventElement[] |  |  | [`salesCampaign-campaignEventElement`](#salescampaign-campaigneventelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaign-campaignEventElement

Browser definition `salesCampaign-campaignEventElement`.

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

## salesCampaign-defaultEventCollection

Browser definition `salesCampaign-defaultEventCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesCampaign-defaultEventElement[] |  |  | [`salesCampaign-defaultEventElement`](#salescampaign-defaulteventelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaign-defaultEventElement

Browser definition `salesCampaign-defaultEventElement`.

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

## salesCampaignCollection

Browser definition `salesCampaignCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesCampaign[] |  |  | [`salesCampaign`](#salescampaign) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesCampaignSelectOptions

Browser definition `salesCampaignSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `audience` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `family` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `offer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `owner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ownerrole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `promotionCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchEngine` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vertical` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

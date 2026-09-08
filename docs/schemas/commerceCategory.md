# Schemas: commerceCategory

Property tables for definitions owned by `commerceCategory`.

Record page: [commerceCategory](../records/commerceCategory.md).

## Index

- [commerceCategory](#commercecategory) — 37 properties
- [commerceCategory-customerSegmentsCollection](#commercecategory-customersegmentscollection) — 6 properties
- [commerceCategory-customerSegmentsElement](#commercecategory-customersegmentselement) — 4 properties
- [commerceCategory-itemsCollection](#commercecategory-itemscollection) — 6 properties
- [commerceCategory-itemsElement](#commercecategory-itemselement) — 5 properties
- [commerceCategory-subcategoriesCollection](#commercecategory-subcategoriescollection) — 6 properties
- [commerceCategory-subcategoriesElement](#commercecategory-subcategorieselement) — 20 properties
- [commerceCategory-tagsCollection](#commercecategory-tagscollection) — 6 properties
- [commerceCategory-tagsElement](#commercecategory-tagselement) — 4 properties
- [commerceCategory-translationsCollection](#commercecategory-translationscollection) — 6 properties
- [commerceCategory-translationsElement](#commercecategory-translationselement) — 15 properties
- [commerceCategory-urlsCollection](#commercecategory-urlscollection) — 6 properties
- [commerceCategory-urlsElement](#commercecategory-urlselement) — 11 properties
- [commerceCategoryCollection](#commercecategorycollection) — 6 properties
- [commerceCategorySelectOptions](#commercecategoryselectoptions) — 7 properties

## commerceCategory

Browser definition `commerceCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `tags` |  | commerceCategory-tagsCollection |  |  | [`commerceCategory-tagsCollection`](#commercecategory-tagscollection) |  |
| `addToHead` | Addition to <head> | string |  |  |  |  |
| `catalog` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `created` | Creation Date/Time | string | date |  |  |  |
| `customerSegments` |  | commerceCategory-customerSegmentsCollection |  |  | [`commerceCategory-customerSegmentsCollection`](#commercecategory-customersegmentscollection) |  |
| `description` | Description | string |  |  |  |  |
| `displayInSite` |  | object |  |  |  |  |
| `displayInSite.id` | Internal identifier | string |  |  |  | `T`, `F` |
| `displayInSite.refName` | Reference Name | string |  |  |  |  |
| `endDate` | End Date | string | date-time |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `items` |  | commerceCategory-itemsCollection |  |  | [`commerceCategory-itemsCollection`](#commercecategory-itemscollection) |  |
| `lastModified` | Last Modified | string | date |  |  |  |
| `lastModifiedBy` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `metaDescription` | Meta Description | string |  |  |  |  |
| `metaKeywords` | Meta Keywords | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `pageBanner` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `pageHeading` | Heading | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `primaryParent` |  | commerceCategory |  |  | [`commerceCategory`](#commercecategory) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequenceNumber` | Sequence Number | integer | int64 |  |  |  |
| `sitemapPriority` |  | object |  |  |  |  |
| `sitemapPriority.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `sitemapPriority.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date-time |  |  |  |
| `subcategories` |  | commerceCategory-subcategoriesCollection |  |  | [`commerceCategory-subcategoriesCollection`](#commercecategory-subcategoriescollection) |  |
| `thumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `translations` |  | commerceCategory-translationsCollection |  |  | [`commerceCategory-translationsCollection`](#commercecategory-translationscollection) |  |
| `urlFragment` | URL Fragment | string |  |  |  |  |
| `urls` |  | commerceCategory-urlsCollection |  |  | [`commerceCategory-urlsCollection`](#commercecategory-urlscollection) |  |
| `version` | Version | integer | int64 |  |  |  |

## commerceCategory-customerSegmentsCollection

Browser definition `commerceCategory-customerSegmentsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-customerSegmentsElement[] |  |  | [`commerceCategory-customerSegmentsElement`](#commercecategory-customersegmentselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-customerSegmentsElement

Browser definition `commerceCategory-customerSegmentsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customerSegmentSize` | Size | string |  |  |  |  |
| `customersegment` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## commerceCategory-itemsCollection

Browser definition `commerceCategory-itemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-itemsElement[] |  |  | [`commerceCategory-itemsElement`](#commercecategory-itemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-itemsElement

Browser definition `commerceCategory-itemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `primarycategory` | Primary Category | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequenceNumber` | Sequence Number | integer | int64 |  |  |  |

## commerceCategory-subcategoriesCollection

Browser definition `commerceCategory-subcategoriesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-subcategoriesElement[] |  |  | [`commerceCategory-subcategoriesElement`](#commercecategory-subcategorieselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-subcategoriesElement

Browser definition `commerceCategory-subcategoriesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addtoheadoverride` | Addition to &lt;head&gt; Override | string |  |  |  |  |
| `descriptionoverride` | Description Override | string |  |  |  |  |
| `displayinsiteoverride` |  | object |  |  |  |  |
| `displayinsiteoverride.id` | Internal identifier | string |  |  |  | `T`, `F` |
| `displayinsiteoverride.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `metadescriptionoverride` | Meta Description Override | string |  |  |  |  |
| `metakeywordsoverride` | Meta Keywords Override | string |  |  |  |  |
| `nameoverride` | Name Override | string |  |  |  |  |
| `pagebanneroverride` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `pageheadingoverride` | Heading Override | string |  |  |  |  |
| `pagetitleoverride` | Title Override | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequenceNumber` | Sequence Number | integer | int64 |  |  |  |
| `sitemappriorityoverride` |  | object |  |  |  |  |
| `sitemappriorityoverride.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `sitemappriorityoverride.refName` | Reference Name | string |  |  |  |  |
| `subcategory` |  | commerceCategory |  |  | [`commerceCategory`](#commercecategory) |  |
| `thumbnailoverride` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `urlfragmentoverride` | URL Fragment Override | string |  |  |  |  |

## commerceCategory-tagsCollection

Browser definition `commerceCategory-tagsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-tagsElement[] |  |  | [`commerceCategory-tagsElement`](#commercecategory-tagselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-tagsElement

Browser definition `commerceCategory-tagsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## commerceCategory-translationsCollection

Browser definition `commerceCategory-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-translationsElement[] |  |  | [`commerceCategory-translationsElement`](#commercecategory-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-translationsElement

Browser definition `commerceCategory-translationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addtohead` | Addition to <head> | string |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | object |  |  |  |  |
| `locale.id` | Internal identifier | string |  |  |  | `ru_RU`, `zh_CN`, `fr_FR` |
| `locale.refName` | Reference Name | string |  |  |  |  |
| `metadescription` | Meta Description | string |  |  |  |  |
| `metakeywords` | Meta Keywords | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `pagebanner` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `pageheading` | Heading | string |  |  |  |  |
| `pagetitle` | Page Title | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `thumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## commerceCategory-urlsCollection

Browser definition `commerceCategory-urlsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | commerceCategory-urlsElement[] |  |  | [`commerceCategory-urlsElement`](#commercecategory-urlselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategory-urlsElement

Browser definition `commerceCategory-urlsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `actualenddate` | Actual End Date | string | date-time |  |  |  |
| `actualstartdate` | Actual Start Date | string | date-time |  |  |  |
| `catalog` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `fullurl` | Full Url | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `idpath` | ID Path | string |  |  |  |  |
| `isprimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nestlevel` | Level | integer | int64 |  |  |  |
| `parentcategory` |  | commerceCategory |  |  | [`commerceCategory`](#commercecategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## commerceCategoryCollection

Browser definition `commerceCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | commerceCategory[] |  |  | [`commerceCategory`](#commercecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## commerceCategorySelectOptions

Browser definition `commerceCategorySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `catalog` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `displayInSite` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `lastModifiedBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pageBanner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryParent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sitemapPriority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thumbnail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

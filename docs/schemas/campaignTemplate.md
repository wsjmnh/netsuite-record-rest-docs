# Schemas: campaignTemplate

Property tables for definitions owned by `campaignTemplate`.

Record page: [campaignTemplate](../records/campaignTemplate.md).

## Index

- [campaignTemplate](#campaigntemplate) — 30 properties
- [campaignTemplateCollection](#campaigntemplatecollection) — 6 properties
- [campaignTemplateSelectOptions](#campaigntemplateselectoptions) — 7 properties

## campaignTemplate

Browser definition `campaignTemplate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `content` | Content | string |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `emailAsSalesRep` | Email as Sales Rep | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fromEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `fromName` | From Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isAutoConverted` | Automatically Converted Template | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPrivate` | Private | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mediaItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `name` | Name | string |  |  |  |  |
| `previewEmail` | Email Preview Recipient | string |  |  |  |  |
| `recordType` | Record Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `replyToEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `restrictToGroup` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `sendEmailPreview` | Send Email Preview | boolean |  |  |  |  |
| `subject` | Subject | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |
| `templateType` | Template Type | string |  |  |  |  |
| `templateVersion` | Version | string |  |  |  |  |
| `trackStatistics` | Track Outgoing Email | boolean |  |  |  |  |
| `typeName` |  | object |  |  |  |  |
| `typeName.id` | Internal identifier | string |  |  |  | `GNCTEMPLATE`, `PDF`, `HCM`, `MAIL`, `KUDOS`, `SYSTEMEMAIL`, `EMAIL`, `ONLINEFORM`, `FAX`, `CAMPAIGN` |
| `typeName.refName` | Reference Name | string |  |  |  |  |
| `usesMedia` |  | object |  |  |  |  |
| `usesMedia.id` | Internal identifier | string |  |  |  | `T`, `F` |
| `usesMedia.refName` | Reference Name | string |  |  |  |  |

## campaignTemplateCollection

Browser definition `campaignTemplateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaignTemplate[] |  |  | [`campaignTemplate`](#campaigntemplate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignTemplateSelectOptions

Browser definition `campaignTemplateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `fromEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mediaItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `replyToEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `restrictToGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscription` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `typeName` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `usesMedia` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

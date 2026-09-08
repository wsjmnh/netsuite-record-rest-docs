# Schemas: emailTemplate

Property tables for definitions owned by `emailTemplate`.

Record page: [emailTemplate](../records/emailTemplate.md).

## Index

- [emailTemplate](#emailtemplate) — 28 properties
- [emailTemplateCollection](#emailtemplatecollection) — 6 properties
- [emailTemplateSelectOptions](#emailtemplateselectoptions) — 5 properties

## emailTemplate

Browser definition `emailTemplate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addCompanyAddress` | Add Company Address to Message Footer in Bulk Merges | boolean |  |  |  |  |
| `addUnsubscribeLink` | Add Unsubscribe Link to Message Footer in Bulk Merges | boolean |  |  |  |  |
| `content` | Content | string |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isAutoConverted` | Automatically Converted Template | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPrivate` | Private | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mediaItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `name` | Name | string |  |  |  |  |
| `package` | App ID | string |  |  |  |  |
| `publisherid` | Publisher ID | string |  |  |  |  |
| `recordType` | Record Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `restrictToGroup` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `scriptid` | ID | string |  |  |  |  |
| `subject` | Subject | string |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |
| `templateType` | Template Type | string |  |  |  |  |
| `templateVersion` | Version | string |  |  |  |  |
| `typeName` |  | object |  |  |  |  |
| `typeName.id` | Internal identifier | string |  |  |  | `GNCTEMPLATE`, `PDF`, `HCM`, `MAIL`, `KUDOS`, `SYSTEMEMAIL`, `EMAIL`, `ONLINEFORM`, `FAX`, `CAMPAIGN` |
| `typeName.refName` | Reference Name | string |  |  |  |  |
| `usesMedia` |  | object |  |  |  |  |
| `usesMedia.id` | Internal identifier | string |  |  |  | `T`, `F` |
| `usesMedia.refName` | Reference Name | string |  |  |  |  |

## emailTemplateCollection

Browser definition `emailTemplateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | emailTemplate[] |  |  | [`emailTemplate`](#emailtemplate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## emailTemplateSelectOptions

Browser definition `emailTemplateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `mediaItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `restrictToGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscription` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `typeName` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `usesMedia` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

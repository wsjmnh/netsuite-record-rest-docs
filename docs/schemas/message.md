# Schemas: message

Property tables for definitions owned by `message`.

Record page: [message](../records/message.md).

## Index

- [message](#message) — 26 properties
- [messageCollection](#messagecollection) — 6 properties
- [messageSelectOptions](#messageselectoptions) — 7 properties

## message

Browser definition `message`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `activity` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `author` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `authorEmail` | From Email Address | string |  |  |  |  |
| `bcc` | Bcc | string |  |  |  |  |
| `cc` | Cc | string |  |  |  |  |
| `emailed` | Emailed | boolean |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `hasAttachment` | Has Attachments | boolean |  |  |  |  |
| `htmlMessage` | HTML Format | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `incoming` | Is Incoming | boolean |  |  |  |  |
| `lastModifiedDate` | Modification Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Message | string |  |  |  |  |
| `messageDate` | Date | string | date |  |  |  |
| `primaryRecipient` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `recipient` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `recipientEmail` | Email Address | string |  |  |  |  |
| `record` | Record | string |  |  |  |  |
| `recordType` | Record Type | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subject` | Subject | string |  |  |  |  |
| `template` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `time` | Time | string |  |  |  |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## messageCollection

Browser definition `messageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | message[] |  |  | [`message`](#message) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## messageSelectOptions

Browser definition `messageSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `activity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `author` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryRecipient` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `recipient` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `template` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

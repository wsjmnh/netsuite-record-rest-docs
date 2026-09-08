# Schemas: campaignResponse

Property tables for definitions owned by `campaignResponse`.

Record page: [campaignResponse](../records/campaignResponse.md).

## Index

- [campaignResponse](#campaignresponse) — 16 properties
- [campaignResponse-responsesCollection](#campaignresponse-responsescollection) — 6 properties
- [campaignResponse-responsesElement](#campaignresponse-responseselement) — 9 properties
- [campaignResponseCollection](#campaignresponsecollection) — 6 properties
- [campaignResponseSelectOptions](#campaignresponseselectoptions) — 5 properties

## campaignResponse

Browser definition `campaignResponse`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `responses` |  | campaignResponse-responsesCollection |  |  | [`campaignResponse-responsesCollection`](#campaignresponse-responsescollection) |  |
| `campaignEvent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `campaignResponseDate` | Date Created | string | date-time |  |  |  |
| `channel` |  | campaignChannel |  |  | [`campaignChannel`](campaignChannel.md#campaignchannel) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `newResponseDate` | New Response Date | string | date |  |  |  |
| `newResponseTime` | New Response Time | string |  |  |  |  |
| `note` | Note | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `response` |  | object |  |  |  |  |
| `response.id` | Internal identifier | string |  |  |  | `BOUNCED`, `BOUNCED_INVALID_SENDER`, `BOUNCED_MAILBOX_FULL`, `FAILED_UNEXPECTED_ERROR`, `UNSUBSCRIBED_BY_FBL`, `BOUNCED_PREVIOUS_HARD_BOUNCE`, `BOUNCED_NETWORK_ISSUES`, `FAILED_TEMPLATE_ERROR`, `CLICKEDTHRU`, `SUBSCRIBED_BY_EMAIL`, `UNSUBSCRIBED_BY_EMAIL`, `BOUNCED_LIMITS_EXCEEDED`, `BOUNCED_MISC`, `RECEIVED`, `PURCHASED_TRANSACTION`, `ACCEPTED`, `TENTATIVE`, `UNSUBSCRIBED`, `RESPONDED`, `BOUNCED_NOT_ACCEPTING_MSGS`, `NORESPONSE`, `BOUNCED_MAIL_PROTOCOL_ISSUES`, `BOUNCED_MEDIA_ERROR`, `VIEWED`, `BOUNCED_INVALID_ADDRESS`, `CLICKEDTHRU_TO_URL`, `SENT_SUCCESSFULLY`, `BOUNCED_SPAM`, `PURCHASED`, `DECLINED`, `BOUNCED_FROM_EMAIL_HANDLER`, `DUMMY`, `SUBSCRIBED`, `BOUNCED_TOO_MANY_RECIPIENTS`, `QUEUED`, `RESPONDED_ONLINE`, `BOUNCED_SECURITY_ISSUES`, `RESPONDED_VIA_EMAIL`, `BOUNCED_MAILBOX_DISABLED`, `SENT`, `ESCALATED` |
| `response.refName` | Reference Name | string |  |  |  |  |

## campaignResponse-responsesCollection

Browser definition `campaignResponse-responsesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | campaignResponse-responsesElement[] |  |  | [`campaignResponse-responsesElement`](#campaignresponse-responseselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignResponse-responsesElement

Browser definition `campaignResponse-responsesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `author` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `note` | Notes | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `response` |  | object |  |  |  |  |
| `response.id` | Internal identifier | string |  |  |  | `BOUNCED`, `BOUNCED_INVALID_SENDER`, `BOUNCED_MAILBOX_FULL`, `FAILED_UNEXPECTED_ERROR`, `UNSUBSCRIBED_BY_FBL`, `BOUNCED_PREVIOUS_HARD_BOUNCE`, `BOUNCED_NETWORK_ISSUES`, `FAILED_TEMPLATE_ERROR`, `CLICKEDTHRU`, `SUBSCRIBED_BY_EMAIL`, `UNSUBSCRIBED_BY_EMAIL`, `BOUNCED_LIMITS_EXCEEDED`, `BOUNCED_MISC`, `RECEIVED`, `PURCHASED_TRANSACTION`, `ACCEPTED`, `TENTATIVE`, `UNSUBSCRIBED`, `RESPONDED`, `BOUNCED_NOT_ACCEPTING_MSGS`, `NORESPONSE`, `BOUNCED_MAIL_PROTOCOL_ISSUES`, `BOUNCED_MEDIA_ERROR`, `VIEWED`, `BOUNCED_INVALID_ADDRESS`, `CLICKEDTHRU_TO_URL`, `SENT_SUCCESSFULLY`, `BOUNCED_SPAM`, `PURCHASED`, `DECLINED`, `BOUNCED_FROM_EMAIL_HANDLER`, `DUMMY`, `SUBSCRIBED`, `BOUNCED_TOO_MANY_RECIPIENTS`, `QUEUED`, `RESPONDED_ONLINE`, `BOUNCED_SECURITY_ISSUES`, `RESPONDED_VIA_EMAIL`, `BOUNCED_MAILBOX_DISABLED`, `SENT`, `ESCALATED` |
| `response.refName` | Reference Name | string |  |  |  |  |
| `responseDate` | Date/Time | string | date-time |  |  |  |

## campaignResponseCollection

Browser definition `campaignResponseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | campaignResponse[] |  |  | [`campaignResponse`](#campaignresponse) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## campaignResponseSelectOptions

Browser definition `campaignResponseSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `campaignEvent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `channel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `response` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

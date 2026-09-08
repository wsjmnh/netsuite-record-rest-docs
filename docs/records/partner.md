# partner

Browser tag `partner` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/partner`, instance `/partner/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/partner` | `operation--partner-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/partner` | `operation--partner-get` | Get list of records. |  | 200 OK → `partnerCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/partner` | `operation--partner-patch` | Update records. | `partnerCollection` | 202 Accepted; default → `nsError` |
| POST | `/partner` | `operation--partner-post` | Insert record. | `partner` | 200 OK → `partner`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/partner` | `operation--partner-put` | Insert or update records. | `partnerCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/partner/{id}` | `operation--partner--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/partner/{id}` | `operation--partner--id--get` | Get record. |  | 200 OK → `partner`; 202 Accepted; default → `nsError` |
| PATCH | `/partner/{id}` | `operation--partner--id--patch` | Update record. | `partner` | 200 OK → `partner`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/partner/{id}` | `operation--partner--id--put` | Insert or update record. | `partner` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/partner/{targetId}/!attach/contact/{attachmentId}` | `operation--partner--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/partner/{targetId}/!detach/contact/{attachmentId}` | `operation--partner--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--partner-delete` | DELETE `/partner` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner-get` | GET `/partner` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner-patch` | PATCH `/partner` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner-post` | POST `/partner` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--partner-put` | PUT `/partner` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner--id--delete` | DELETE `/partner/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner--id--get` | GET `/partner/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner--id--patch` | PATCH `/partner/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--partner--id--put` | PUT `/partner/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--partner--targetId---attach-contact--attachmentId--post` | POST `/partner/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--partner--targetId---detach-contact--attachmentId--post` | POST `/partner/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--partner--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [partner schemas](../schemas/partner.md).

| Definition | Role |
| --- | --- |
| [`partner`](../schemas/partner.md#partner) | record body |
| [`partner-addressBook-addressBookAddress`](../schemas/partner.md#partner-addressbook-addressbookaddress) | related |
| [`partner-addressBookCollection`](../schemas/partner.md#partner-addressbookcollection) | sublist/collection |
| [`partner-addressBookElement`](../schemas/partner.md#partner-addressbookelement) | sublist/element |
| [`partner-campaignsCollection`](../schemas/partner.md#partner-campaignscollection) | sublist/collection |
| [`partner-campaignsElement`](../schemas/partner.md#partner-campaignselement) | sublist/element |
| [`partner-contactRolesCollection`](../schemas/partner.md#partner-contactrolescollection) | sublist/collection |
| [`partner-contactRolesElement`](../schemas/partner.md#partner-contactroleselement) | sublist/element |
| [`partner-subscriptionMessageHistoryCollection`](../schemas/partner.md#partner-subscriptionmessagehistorycollection) | sublist/collection |
| [`partner-subscriptionMessageHistoryElement`](../schemas/partner.md#partner-subscriptionmessagehistoryelement) | sublist/element |
| [`partner-subscriptionsCollection`](../schemas/partner.md#partner-subscriptionscollection) | sublist/collection |
| [`partner-subscriptionsElement`](../schemas/partner.md#partner-subscriptionselement) | sublist/element |
| [`partner-taxRegistrationCollection`](../schemas/partner.md#partner-taxregistrationcollection) | sublist/collection |
| [`partner-taxRegistrationElement`](../schemas/partner.md#partner-taxregistrationelement) | sublist/element |
| [`partnerCollection`](../schemas/partner.md#partnercollection) | collection page |
| [`partnerSelectOptions`](../schemas/partner.md#partnerselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`partner-addressBookCollection`](../schemas/partner.md#partner-addressbookcollection) | [`partner-addressBookElement`](../schemas/partner.md#partner-addressbookelement) |
| `campaigns` | [`partner-campaignsCollection`](../schemas/partner.md#partner-campaignscollection) | [`partner-campaignsElement`](../schemas/partner.md#partner-campaignselement) |
| `contactRoles` | [`partner-contactRolesCollection`](../schemas/partner.md#partner-contactrolescollection) | [`partner-contactRolesElement`](../schemas/partner.md#partner-contactroleselement) |
| `subscriptionMessageHistory` | [`partner-subscriptionMessageHistoryCollection`](../schemas/partner.md#partner-subscriptionmessagehistorycollection) | [`partner-subscriptionMessageHistoryElement`](../schemas/partner.md#partner-subscriptionmessagehistoryelement) |
| `subscriptions` | [`partner-subscriptionsCollection`](../schemas/partner.md#partner-subscriptionscollection) | [`partner-subscriptionsElement`](../schemas/partner.md#partner-subscriptionselement) |
| `taxRegistration` | [`partner-taxRegistrationCollection`](../schemas/partner.md#partner-taxregistrationcollection) | [`partner-taxRegistrationElement`](../schemas/partner.md#partner-taxregistrationelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/partner/{targetId}/!attach/contact/{attachmentId}` | `operation--partner--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/partner/{targetId}/!detach/contact/{attachmentId}` | `operation--partner--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

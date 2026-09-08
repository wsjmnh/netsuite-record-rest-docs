# customerRefund

Browser tag `customerRefund` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerRefund`, instance `/customerRefund/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerRefund` | `operation--customerRefund-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerRefund` | `operation--customerRefund-get` | Get list of records. |  | 200 OK → `customerRefundCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerRefund` | `operation--customerRefund-patch` | Update records. | `customerRefundCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerRefund` | `operation--customerRefund-post` | Insert record. | `customerRefund` | 200 OK → `customerRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerRefund` | `operation--customerRefund-put` | Insert or update records. | `customerRefundCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerRefund/{id}` | `operation--customerRefund--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerRefund/{id}` | `operation--customerRefund--id--get` | Get record. |  | 200 OK → `customerRefund`; 202 Accepted; default → `nsError` |
| PATCH | `/customerRefund/{id}` | `operation--customerRefund--id--patch` | Update record. | `customerRefund` | 200 OK → `customerRefund`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerRefund/{id}` | `operation--customerRefund--id--put` | Insert or update record. | `customerRefund` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/customerRefund/{targetId}/!attach/contact/{attachmentId}` | `operation--customerRefund--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/customerRefund/{targetId}/!detach/contact/{attachmentId}` | `operation--customerRefund--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerRefund-delete` | DELETE `/customerRefund` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund-get` | GET `/customerRefund` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund-patch` | PATCH `/customerRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund-post` | POST `/customerRefund` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerRefund-put` | PUT `/customerRefund` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund--id--delete` | DELETE `/customerRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund--id--get` | GET `/customerRefund/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund--id--patch` | PATCH `/customerRefund/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerRefund--id--put` | PUT `/customerRefund/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerRefund--targetId---attach-contact--attachmentId--post` | POST `/customerRefund/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerRefund--targetId---detach-contact--attachmentId--post` | POST `/customerRefund/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--customerRefund--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [customerRefund schemas](../schemas/customerRefund.md).

| Definition | Role |
| --- | --- |
| [`customerRefund`](../schemas/customerRefund.md#customerrefund) | record body |
| [`customerRefund-accountingBookDetailCollection`](../schemas/customerRefund.md#customerrefund-accountingbookdetailcollection) | sublist/collection |
| [`customerRefund-accountingBookDetailElement`](../schemas/customerRefund.md#customerrefund-accountingbookdetailelement) | sublist/element |
| [`customerRefund-applyCollection`](../schemas/customerRefund.md#customerrefund-applycollection) | sublist/collection |
| [`customerRefund-applyElement`](../schemas/customerRefund.md#customerrefund-applyelement) | sublist/element |
| [`customerRefund-depositCollection`](../schemas/customerRefund.md#customerrefund-depositcollection) | sublist/collection |
| [`customerRefund-depositElement`](../schemas/customerRefund.md#customerrefund-depositelement) | sublist/element |
| [`customerRefund-payeeAddress`](../schemas/customerRefund.md#customerrefund-payeeaddress) | related |
| [`customerRefundCollection`](../schemas/customerRefund.md#customerrefundcollection) | collection page |
| [`customerRefundSelectOptions`](../schemas/customerRefund.md#customerrefundselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`customerRefund-accountingBookDetailCollection`](../schemas/customerRefund.md#customerrefund-accountingbookdetailcollection) | [`customerRefund-accountingBookDetailElement`](../schemas/customerRefund.md#customerrefund-accountingbookdetailelement) |
| `apply` | [`customerRefund-applyCollection`](../schemas/customerRefund.md#customerrefund-applycollection) | [`customerRefund-applyElement`](../schemas/customerRefund.md#customerrefund-applyelement) |
| `deposit` | [`customerRefund-depositCollection`](../schemas/customerRefund.md#customerrefund-depositcollection) | [`customerRefund-depositElement`](../schemas/customerRefund.md#customerrefund-depositelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/customerRefund/{targetId}/!attach/contact/{attachmentId}` | `operation--customerRefund--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/customerRefund/{targetId}/!detach/contact/{attachmentId}` | `operation--customerRefund--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

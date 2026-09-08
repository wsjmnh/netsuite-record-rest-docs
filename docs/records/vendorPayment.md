# vendorPayment

Browser tag `vendorPayment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorPayment`, instance `/vendorPayment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorPayment` | `operation--vendorPayment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorPayment` | `operation--vendorPayment-get` | Get list of records. |  | 200 OK → `vendorPaymentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorPayment` | `operation--vendorPayment-patch` | Update records. | `vendorPaymentCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorPayment` | `operation--vendorPayment-post` | Insert record. | `vendorPayment` | 200 OK → `vendorPayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorPayment` | `operation--vendorPayment-put` | Insert or update records. | `vendorPaymentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorPayment/{id}` | `operation--vendorPayment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorPayment/{id}` | `operation--vendorPayment--id--get` | Get record. |  | 200 OK → `vendorPayment`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorPayment/{id}` | `operation--vendorPayment--id--patch` | Update record. | `vendorPayment` | 200 OK → `vendorPayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorPayment/{id}` | `operation--vendorPayment--id--put` | Insert or update record. | `vendorPayment` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendorPayment/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorPayment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/vendorPayment/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorPayment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorPayment-delete` | DELETE `/vendorPayment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment-get` | GET `/vendorPayment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment-patch` | PATCH `/vendorPayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment-post` | POST `/vendorPayment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorPayment-put` | PUT `/vendorPayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment--id--delete` | DELETE `/vendorPayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment--id--get` | GET `/vendorPayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment--id--patch` | PATCH `/vendorPayment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorPayment--id--put` | PUT `/vendorPayment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorPayment--targetId---attach-contact--attachmentId--post` | POST `/vendorPayment/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPayment--targetId---detach-contact--attachmentId--post` | POST `/vendorPayment/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--vendorPayment--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [vendorPayment schemas](../schemas/vendorPayment.md).

| Definition | Role |
| --- | --- |
| [`vendorPayment`](../schemas/vendorPayment.md#vendorpayment) | record body |
| [`vendorPayment-accountingBookDetailCollection`](../schemas/vendorPayment.md#vendorpayment-accountingbookdetailcollection) | sublist/collection |
| [`vendorPayment-accountingBookDetailElement`](../schemas/vendorPayment.md#vendorpayment-accountingbookdetailelement) | sublist/element |
| [`vendorPayment-applyCollection`](../schemas/vendorPayment.md#vendorpayment-applycollection) | sublist/collection |
| [`vendorPayment-applyElement`](../schemas/vendorPayment.md#vendorpayment-applyelement) | sublist/element |
| [`vendorPayment-creditCollection`](../schemas/vendorPayment.md#vendorpayment-creditcollection) | sublist/collection |
| [`vendorPayment-creditElement`](../schemas/vendorPayment.md#vendorpayment-creditelement) | sublist/element |
| [`vendorPayment-payeeAddress`](../schemas/vendorPayment.md#vendorpayment-payeeaddress) | related |
| [`vendorPaymentCollection`](../schemas/vendorPayment.md#vendorpaymentcollection) | collection page |
| [`vendorPaymentSelectOptions`](../schemas/vendorPayment.md#vendorpaymentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`vendorPayment-accountingBookDetailCollection`](../schemas/vendorPayment.md#vendorpayment-accountingbookdetailcollection) | [`vendorPayment-accountingBookDetailElement`](../schemas/vendorPayment.md#vendorpayment-accountingbookdetailelement) |
| `apply` | [`vendorPayment-applyCollection`](../schemas/vendorPayment.md#vendorpayment-applycollection) | [`vendorPayment-applyElement`](../schemas/vendorPayment.md#vendorpayment-applyelement) |
| `credit` | [`vendorPayment-creditCollection`](../schemas/vendorPayment.md#vendorpayment-creditcollection) | [`vendorPayment-creditElement`](../schemas/vendorPayment.md#vendorpayment-creditelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/vendorPayment/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorPayment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/vendorPayment/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorPayment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

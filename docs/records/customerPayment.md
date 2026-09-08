# customerPayment

Browser tag `customerPayment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerPayment`, instance `/customerPayment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerPayment` | `operation--customerPayment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerPayment` | `operation--customerPayment-get` | Get list of records. |  | 200 OK → `customerPaymentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerPayment` | `operation--customerPayment-patch` | Update records. | `customerPaymentCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerPayment` | `operation--customerPayment-post` | Insert record. | `customerPayment` | 200 OK → `customerPayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerPayment` | `operation--customerPayment-put` | Insert or update records. | `customerPaymentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerPayment/{id}` | `operation--customerPayment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerPayment/{id}` | `operation--customerPayment--id--get` | Get record. |  | 200 OK → `customerPayment`; 202 Accepted; default → `nsError` |
| PATCH | `/customerPayment/{id}` | `operation--customerPayment--id--patch` | Update record. | `customerPayment` | 200 OK → `customerPayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerPayment/{id}` | `operation--customerPayment--id--put` | Insert or update record. | `customerPayment` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/customerPayment/{id}/!transform/customerRefund` | `operation--customerPayment--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | 200 OK → `customerPayment`; 202 Accepted; 204 No Content → `customerRefund`; default → `nsError` |
| POST | `/customerPayment/{targetId}/!attach/contact/{attachmentId}` | `operation--customerPayment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/customerPayment/{targetId}/!detach/contact/{attachmentId}` | `operation--customerPayment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerPayment-delete` | DELETE `/customerPayment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment-get` | GET `/customerPayment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment-patch` | PATCH `/customerPayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment-post` | POST `/customerPayment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerPayment-put` | PUT `/customerPayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment--id--delete` | DELETE `/customerPayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment--id--get` | GET `/customerPayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment--id--patch` | PATCH `/customerPayment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerPayment--id--put` | PUT `/customerPayment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerPayment--id---transform-customerRefund-post` | POST `/customerPayment/{id}/!transform/customerRefund` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customerPayment--targetId---attach-contact--attachmentId--post` | POST `/customerPayment/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerPayment--targetId---detach-contact--attachmentId--post` | POST `/customerPayment/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--customerPayment--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [customerPayment schemas](../schemas/customerPayment.md).

| Definition | Role |
| --- | --- |
| [`customerPayment`](../schemas/customerPayment.md#customerpayment) | record body |
| [`customerPayment-accountingBookDetailCollection`](../schemas/customerPayment.md#customerpayment-accountingbookdetailcollection) | sublist/collection |
| [`customerPayment-accountingBookDetailElement`](../schemas/customerPayment.md#customerpayment-accountingbookdetailelement) | sublist/element |
| [`customerPayment-appliedRulesCollection`](../schemas/customerPayment.md#customerpayment-appliedrulescollection) | sublist/collection |
| [`customerPayment-appliedRulesElement`](../schemas/customerPayment.md#customerpayment-appliedruleselement) | sublist/element |
| [`customerPayment-applyCollection`](../schemas/customerPayment.md#customerpayment-applycollection) | sublist/collection |
| [`customerPayment-applyElement`](../schemas/customerPayment.md#customerpayment-applyelement) | sublist/element |
| [`customerPayment-creditCollection`](../schemas/customerPayment.md#customerpayment-creditcollection) | sublist/collection |
| [`customerPayment-creditElement`](../schemas/customerPayment.md#customerpayment-creditelement) | sublist/element |
| [`customerPayment-depositCollection`](../schemas/customerPayment.md#customerpayment-depositcollection) | sublist/collection |
| [`customerPayment-depositElement`](../schemas/customerPayment.md#customerpayment-depositelement) | sublist/element |
| [`customerPaymentCollection`](../schemas/customerPayment.md#customerpaymentcollection) | collection page |
| [`customerPaymentSelectOptions`](../schemas/customerPayment.md#customerpaymentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`customerRefund`](../schemas/customerRefund.md#customerrefund)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`customerPayment-accountingBookDetailCollection`](../schemas/customerPayment.md#customerpayment-accountingbookdetailcollection) | [`customerPayment-accountingBookDetailElement`](../schemas/customerPayment.md#customerpayment-accountingbookdetailelement) |
| `appliedRules` | [`customerPayment-appliedRulesCollection`](../schemas/customerPayment.md#customerpayment-appliedrulescollection) | [`customerPayment-appliedRulesElement`](../schemas/customerPayment.md#customerpayment-appliedruleselement) |
| `apply` | [`customerPayment-applyCollection`](../schemas/customerPayment.md#customerpayment-applycollection) | [`customerPayment-applyElement`](../schemas/customerPayment.md#customerpayment-applyelement) |
| `credit` | [`customerPayment-creditCollection`](../schemas/customerPayment.md#customerpayment-creditcollection) | [`customerPayment-creditElement`](../schemas/customerPayment.md#customerpayment-creditelement) |
| `deposit` | [`customerPayment-depositCollection`](../schemas/customerPayment.md#customerpayment-depositcollection) | [`customerPayment-depositElement`](../schemas/customerPayment.md#customerpayment-depositelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/customerPayment/{id}/!transform/customerRefund` | `operation--customerPayment--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | `customerRefund` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/customerPayment/{targetId}/!attach/contact/{attachmentId}` | `operation--customerPayment--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/customerPayment/{targetId}/!detach/contact/{attachmentId}` | `operation--customerPayment--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

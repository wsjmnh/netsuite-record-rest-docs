# customerDeposit

Browser tag `customerDeposit` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerDeposit`, instance `/customerDeposit/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerDeposit` | `operation--customerDeposit-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerDeposit` | `operation--customerDeposit-get` | Get list of records. |  | 200 OK → `customerDepositCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerDeposit` | `operation--customerDeposit-patch` | Update records. | `customerDepositCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerDeposit` | `operation--customerDeposit-post` | Insert record. | `customerDeposit` | 200 OK → `customerDeposit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerDeposit` | `operation--customerDeposit-put` | Insert or update records. | `customerDepositCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerDeposit/{id}` | `operation--customerDeposit--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerDeposit/{id}` | `operation--customerDeposit--id--get` | Get record. |  | 200 OK → `customerDeposit`; 202 Accepted; default → `nsError` |
| PATCH | `/customerDeposit/{id}` | `operation--customerDeposit--id--patch` | Update record. | `customerDeposit` | 200 OK → `customerDeposit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerDeposit/{id}` | `operation--customerDeposit--id--put` | Insert or update record. | `customerDeposit` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/customerDeposit/{id}/!transform/customerRefund` | `operation--customerDeposit--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | 200 OK → `customerDeposit`; 202 Accepted; 204 No Content → `customerRefund`; default → `nsError` |
| POST | `/customerDeposit/{id}/!transform/depositApplication` | `operation--customerDeposit--id---transform-depositApplication-post` | Transform to depositApplication. | `depositApplication` | 200 OK → `customerDeposit`; 202 Accepted; 204 No Content → `depositApplication`; default → `nsError` |
| POST | `/customerDeposit/{targetId}/!attach/contact/{attachmentId}` | `operation--customerDeposit--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/customerDeposit/{targetId}/!detach/contact/{attachmentId}` | `operation--customerDeposit--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerDeposit-delete` | DELETE `/customerDeposit` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit-get` | GET `/customerDeposit` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit-patch` | PATCH `/customerDeposit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit-post` | POST `/customerDeposit` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerDeposit-put` | PUT `/customerDeposit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit--id--delete` | DELETE `/customerDeposit/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit--id--get` | GET `/customerDeposit/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit--id--patch` | PATCH `/customerDeposit/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerDeposit--id--put` | PUT `/customerDeposit/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerDeposit--id---transform-customerRefund-post` | POST `/customerDeposit/{id}/!transform/customerRefund` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customerDeposit--id---transform-depositApplication-post` | POST `/customerDeposit/{id}/!transform/depositApplication` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customerDeposit--targetId---attach-contact--attachmentId--post` | POST `/customerDeposit/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerDeposit--targetId---detach-contact--attachmentId--post` | POST `/customerDeposit/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--customerDeposit--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [customerDeposit schemas](../schemas/customerDeposit.md).

| Definition | Role |
| --- | --- |
| [`customerDeposit`](../schemas/customerDeposit.md#customerdeposit) | record body |
| [`customerDeposit-accountingBookDetailCollection`](../schemas/customerDeposit.md#customerdeposit-accountingbookdetailcollection) | sublist/collection |
| [`customerDeposit-accountingBookDetailElement`](../schemas/customerDeposit.md#customerdeposit-accountingbookdetailelement) | sublist/element |
| [`customerDeposit-appliedRulesCollection`](../schemas/customerDeposit.md#customerdeposit-appliedrulescollection) | sublist/collection |
| [`customerDeposit-appliedRulesElement`](../schemas/customerDeposit.md#customerdeposit-appliedruleselement) | sublist/element |
| [`customerDepositCollection`](../schemas/customerDeposit.md#customerdepositcollection) | collection page |
| [`customerDepositSelectOptions`](../schemas/customerDeposit.md#customerdepositselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`customerRefund`](../schemas/customerRefund.md#customerrefund)
- [`depositApplication`](../schemas/depositApplication.md#depositapplication)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`customerDeposit-accountingBookDetailCollection`](../schemas/customerDeposit.md#customerdeposit-accountingbookdetailcollection) | [`customerDeposit-accountingBookDetailElement`](../schemas/customerDeposit.md#customerdeposit-accountingbookdetailelement) |
| `appliedRules` | [`customerDeposit-appliedRulesCollection`](../schemas/customerDeposit.md#customerdeposit-appliedrulescollection) | [`customerDeposit-appliedRulesElement`](../schemas/customerDeposit.md#customerdeposit-appliedruleselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/customerDeposit/{id}/!transform/customerRefund` | `operation--customerDeposit--id---transform-customerRefund-post` | Transform to customerRefund. | `customerRefund` | `customerRefund` |
| POST | `/customerDeposit/{id}/!transform/depositApplication` | `operation--customerDeposit--id---transform-depositApplication-post` | Transform to depositApplication. | `depositApplication` | `depositApplication` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/customerDeposit/{targetId}/!attach/contact/{attachmentId}` | `operation--customerDeposit--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/customerDeposit/{targetId}/!detach/contact/{attachmentId}` | `operation--customerDeposit--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

# vendorCredit

Browser tag `vendorCredit` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorCredit`, instance `/vendorCredit/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorCredit` | `operation--vendorCredit-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorCredit` | `operation--vendorCredit-get` | Get list of records. |  | 200 OK → `vendorCreditCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorCredit` | `operation--vendorCredit-patch` | Update records. | `vendorCreditCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorCredit` | `operation--vendorCredit-post` | Insert record. | `vendorCredit` | 200 OK → `vendorCredit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorCredit` | `operation--vendorCredit-put` | Insert or update records. | `vendorCreditCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorCredit/{id}` | `operation--vendorCredit--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorCredit/{id}` | `operation--vendorCredit--id--get` | Get record. |  | 200 OK → `vendorCredit`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorCredit/{id}` | `operation--vendorCredit--id--patch` | Update record. | `vendorCredit` | 200 OK → `vendorCredit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorCredit/{id}` | `operation--vendorCredit--id--put` | Insert or update record. | `vendorCredit` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendorCredit/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorCredit--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/vendorCredit/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorCredit--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorCredit-delete` | DELETE `/vendorCredit` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit-get` | GET `/vendorCredit` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit-patch` | PATCH `/vendorCredit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit-post` | POST `/vendorCredit` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorCredit-put` | PUT `/vendorCredit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit--id--delete` | DELETE `/vendorCredit/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit--id--get` | GET `/vendorCredit/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit--id--patch` | PATCH `/vendorCredit/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorCredit--id--put` | PUT `/vendorCredit/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorCredit--targetId---attach-contact--attachmentId--post` | POST `/vendorCredit/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorCredit--targetId---detach-contact--attachmentId--post` | POST `/vendorCredit/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--vendorCredit--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [vendorCredit schemas](../schemas/vendorCredit.md).

| Definition | Role |
| --- | --- |
| [`vendorCredit`](../schemas/vendorCredit.md#vendorcredit) | record body |
| [`vendorCredit-accountingBookDetailCollection`](../schemas/vendorCredit.md#vendorcredit-accountingbookdetailcollection) | sublist/collection |
| [`vendorCredit-accountingBookDetailElement`](../schemas/vendorCredit.md#vendorcredit-accountingbookdetailelement) | sublist/element |
| [`vendorCredit-appliedRulesCollection`](../schemas/vendorCredit.md#vendorcredit-appliedrulescollection) | sublist/collection |
| [`vendorCredit-appliedRulesElement`](../schemas/vendorCredit.md#vendorcredit-appliedruleselement) | sublist/element |
| [`vendorCredit-applyCollection`](../schemas/vendorCredit.md#vendorcredit-applycollection) | sublist/collection |
| [`vendorCredit-applyElement`](../schemas/vendorCredit.md#vendorcredit-applyelement) | sublist/element |
| [`vendorCredit-billingAddress`](../schemas/vendorCredit.md#vendorcredit-billingaddress) | related |
| [`vendorCredit-expenseCollection`](../schemas/vendorCredit.md#vendorcredit-expensecollection) | sublist/collection |
| [`vendorCredit-expenseElement`](../schemas/vendorCredit.md#vendorcredit-expenseelement) | sublist/element |
| [`vendorCredit-item-inventoryDetail`](../schemas/vendorCredit.md#vendorcredit-item-inventorydetail) | related |
| [`vendorCredit-item-inventoryDetail-inventoryAssignmentCollection`](../schemas/vendorCredit.md#vendorcredit-item-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`vendorCredit-item-inventoryDetail-inventoryAssignmentElement`](../schemas/vendorCredit.md#vendorcredit-item-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`vendorCredit-itemCollection`](../schemas/vendorCredit.md#vendorcredit-itemcollection) | sublist/collection |
| [`vendorCredit-itemElement`](../schemas/vendorCredit.md#vendorcredit-itemelement) | sublist/element |
| [`vendorCredit-taxDetailsCollection`](../schemas/vendorCredit.md#vendorcredit-taxdetailscollection) | sublist/collection |
| [`vendorCredit-taxDetailsElement`](../schemas/vendorCredit.md#vendorcredit-taxdetailselement) | sublist/element |
| [`vendorCreditCollection`](../schemas/vendorCredit.md#vendorcreditcollection) | collection page |
| [`vendorCreditSelectOptions`](../schemas/vendorCredit.md#vendorcreditselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`vendorCredit-accountingBookDetailCollection`](../schemas/vendorCredit.md#vendorcredit-accountingbookdetailcollection) | [`vendorCredit-accountingBookDetailElement`](../schemas/vendorCredit.md#vendorcredit-accountingbookdetailelement) |
| `appliedRules` | [`vendorCredit-appliedRulesCollection`](../schemas/vendorCredit.md#vendorcredit-appliedrulescollection) | [`vendorCredit-appliedRulesElement`](../schemas/vendorCredit.md#vendorcredit-appliedruleselement) |
| `apply` | [`vendorCredit-applyCollection`](../schemas/vendorCredit.md#vendorcredit-applycollection) | [`vendorCredit-applyElement`](../schemas/vendorCredit.md#vendorcredit-applyelement) |
| `expense` | [`vendorCredit-expenseCollection`](../schemas/vendorCredit.md#vendorcredit-expensecollection) | [`vendorCredit-expenseElement`](../schemas/vendorCredit.md#vendorcredit-expenseelement) |
| `item` | [`vendorCredit-itemCollection`](../schemas/vendorCredit.md#vendorcredit-itemcollection) | [`vendorCredit-itemElement`](../schemas/vendorCredit.md#vendorcredit-itemelement) |
| `taxDetails` | [`vendorCredit-taxDetailsCollection`](../schemas/vendorCredit.md#vendorcredit-taxdetailscollection) | [`vendorCredit-taxDetailsElement`](../schemas/vendorCredit.md#vendorcredit-taxdetailselement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/vendorCredit/{targetId}/!attach/contact/{attachmentId}` | `operation--vendorCredit--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/vendorCredit/{targetId}/!detach/contact/{attachmentId}` | `operation--vendorCredit--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

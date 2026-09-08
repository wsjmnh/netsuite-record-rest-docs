# job

Browser tag `job` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/job`, instance `/job/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/job` | `operation--job-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/job` | `operation--job-get` | Get list of records. |  | 200 OK → `jobCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/job` | `operation--job-patch` | Update records. | `jobCollection` | 202 Accepted; default → `nsError` |
| POST | `/job` | `operation--job-post` | Insert record. | `job` | 200 OK → `job`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/job` | `operation--job-put` | Insert or update records. | `jobCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/job/{id}` | `operation--job--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/job/{id}` | `operation--job--id--get` | Get record. |  | 200 OK → `job`; 202 Accepted; default → `nsError` |
| PATCH | `/job/{id}` | `operation--job--id--patch` | Update record. | `job` | 200 OK → `job`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/job/{id}` | `operation--job--id--put` | Insert or update record. | `job` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/job/{id}/!transform/cashSale` | `operation--job--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | 200 OK → `job`; 202 Accepted; 204 No Content → `cashSale`; default → `nsError` |
| POST | `/job/{id}/!transform/estimate` | `operation--job--id---transform-estimate-post` | Transform to estimate. | `estimate` | 200 OK → `job`; 202 Accepted; 204 No Content → `estimate`; default → `nsError` |
| POST | `/job/{id}/!transform/invoice` | `operation--job--id---transform-invoice-post` | Transform to invoice. | `invoice` | 200 OK → `job`; 202 Accepted; 204 No Content → `invoice`; default → `nsError` |
| POST | `/job/{id}/!transform/salesOrder` | `operation--job--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | 200 OK → `job`; 202 Accepted; 204 No Content → `salesOrder`; default → `nsError` |
| POST | `/job/{targetId}/!attach/contact/{attachmentId}` | `operation--job--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/job/{targetId}/!detach/contact/{attachmentId}` | `operation--job--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--job-delete` | DELETE `/job` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job-get` | GET `/job` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job-patch` | PATCH `/job` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job-post` | POST `/job` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--job-put` | PUT `/job` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job--id--delete` | DELETE `/job/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job--id--get` | GET `/job/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job--id--patch` | PATCH `/job/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--job--id--put` | PUT `/job/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--job--id---transform-cashSale-post` | POST `/job/{id}/!transform/cashSale` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--job--id---transform-estimate-post` | POST `/job/{id}/!transform/estimate` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--job--id---transform-invoice-post` | POST `/job/{id}/!transform/invoice` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--job--id---transform-salesOrder-post` | POST `/job/{id}/!transform/salesOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--job--targetId---attach-contact--attachmentId--post` | POST `/job/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--job--targetId---detach-contact--attachmentId--post` | POST `/job/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--job--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [job schemas](../schemas/job.md).

| Definition | Role |
| --- | --- |
| [`job`](../schemas/job.md#job) | record body |
| [`job-addressBook-addressBookAddress`](../schemas/job.md#job-addressbook-addressbookaddress) | related |
| [`job-addressBookCollection`](../schemas/job.md#job-addressbookcollection) | sublist/collection |
| [`job-addressBookElement`](../schemas/job.md#job-addressbookelement) | sublist/element |
| [`job-bBudgetCollection`](../schemas/job.md#job-bbudgetcollection) | sublist/collection |
| [`job-bBudgetElement`](../schemas/job.md#job-bbudgetelement) | sublist/element |
| [`job-cBudgetCollection`](../schemas/job.md#job-cbudgetcollection) | sublist/collection |
| [`job-cBudgetElement`](../schemas/job.md#job-cbudgetelement) | sublist/element |
| [`job-paStatementCollection`](../schemas/job.md#job-pastatementcollection) | sublist/collection |
| [`job-paStatementElement`](../schemas/job.md#job-pastatementelement) | sublist/element |
| [`job-percentCompleteOverrideCollection`](../schemas/job.md#job-percentcompleteoverridecollection) | sublist/collection |
| [`job-percentCompleteOverrideElement`](../schemas/job.md#job-percentcompleteoverrideelement) | sublist/element |
| [`job-plStatementCollection`](../schemas/job.md#job-plstatementcollection) | sublist/collection |
| [`job-plStatementElement`](../schemas/job.md#job-plstatementelement) | sublist/element |
| [`jobCollection`](../schemas/job.md#jobcollection) | collection page |
| [`jobSelectOptions`](../schemas/job.md#jobselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashSale`](../schemas/cashSale.md#cashsale)
- [`estimate`](../schemas/estimate.md#estimate)
- [`invoice`](../schemas/invoice.md#invoice)
- [`nsError`](../schemas/ns.md#nserror)
- [`salesOrder`](../schemas/salesOrder.md#salesorder)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`job-addressBookCollection`](../schemas/job.md#job-addressbookcollection) | [`job-addressBookElement`](../schemas/job.md#job-addressbookelement) |
| `bBudget` | [`job-bBudgetCollection`](../schemas/job.md#job-bbudgetcollection) | [`job-bBudgetElement`](../schemas/job.md#job-bbudgetelement) |
| `cBudget` | [`job-cBudgetCollection`](../schemas/job.md#job-cbudgetcollection) | [`job-cBudgetElement`](../schemas/job.md#job-cbudgetelement) |
| `paStatement` | [`job-paStatementCollection`](../schemas/job.md#job-pastatementcollection) | [`job-paStatementElement`](../schemas/job.md#job-pastatementelement) |
| `percentCompleteOverride` | [`job-percentCompleteOverrideCollection`](../schemas/job.md#job-percentcompleteoverridecollection) | [`job-percentCompleteOverrideElement`](../schemas/job.md#job-percentcompleteoverrideelement) |
| `plStatement` | [`job-plStatementCollection`](../schemas/job.md#job-plstatementcollection) | [`job-plStatementElement`](../schemas/job.md#job-plstatementelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/job/{id}/!transform/cashSale` | `operation--job--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | `cashSale` |
| POST | `/job/{id}/!transform/estimate` | `operation--job--id---transform-estimate-post` | Transform to estimate. | `estimate` | `estimate` |
| POST | `/job/{id}/!transform/invoice` | `operation--job--id---transform-invoice-post` | Transform to invoice. | `invoice` | `invoice` |
| POST | `/job/{id}/!transform/salesOrder` | `operation--job--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | `salesOrder` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/job/{targetId}/!attach/contact/{attachmentId}` | `operation--job--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/job/{targetId}/!detach/contact/{attachmentId}` | `operation--job--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

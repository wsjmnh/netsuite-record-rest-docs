# expenseReport

Browser tag `expenseReport` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/expenseReport`, instance `/expenseReport/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/expenseReport` | `operation--expenseReport-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/expenseReport` | `operation--expenseReport-get` | Get list of records. |  | 200 OK → `expenseReportCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/expenseReport` | `operation--expenseReport-patch` | Update records. | `expenseReportCollection` | 202 Accepted; default → `nsError` |
| POST | `/expenseReport` | `operation--expenseReport-post` | Insert record. | `expenseReport` | 200 OK → `expenseReport`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/expenseReport` | `operation--expenseReport-put` | Insert or update records. | `expenseReportCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/expenseReport/{id}` | `operation--expenseReport--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/expenseReport/{id}` | `operation--expenseReport--id--get` | Get record. |  | 200 OK → `expenseReport`; 202 Accepted; default → `nsError` |
| PATCH | `/expenseReport/{id}` | `operation--expenseReport--id--patch` | Update record. | `expenseReport` | 200 OK → `expenseReport`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/expenseReport/{id}` | `operation--expenseReport--id--put` | Insert or update record. | `expenseReport` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--expenseReport-delete` | DELETE `/expenseReport` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport-get` | GET `/expenseReport` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport-patch` | PATCH `/expenseReport` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport-post` | POST `/expenseReport` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--expenseReport-put` | PUT `/expenseReport` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport--id--delete` | DELETE `/expenseReport/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport--id--get` | GET `/expenseReport/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseReport--id--patch` | PATCH `/expenseReport/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--expenseReport--id--put` | PUT `/expenseReport/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [expenseReport schemas](../schemas/expenseReport.md).

| Definition | Role |
| --- | --- |
| [`expenseReport`](../schemas/expenseReport.md#expensereport) | record body |
| [`expenseReport-accountingBookDetailCollection`](../schemas/expenseReport.md#expensereport-accountingbookdetailcollection) | sublist/collection |
| [`expenseReport-accountingBookDetailElement`](../schemas/expenseReport.md#expensereport-accountingbookdetailelement) | sublist/element |
| [`expenseReport-appliedRulesCollection`](../schemas/expenseReport.md#expensereport-appliedrulescollection) | sublist/collection |
| [`expenseReport-appliedRulesElement`](../schemas/expenseReport.md#expensereport-appliedruleselement) | sublist/element |
| [`expenseReport-expenseCollection`](../schemas/expenseReport.md#expensereport-expensecollection) | sublist/collection |
| [`expenseReport-expenseElement`](../schemas/expenseReport.md#expensereport-expenseelement) | sublist/element |
| [`expenseReport-taxDetailsCollection`](../schemas/expenseReport.md#expensereport-taxdetailscollection) | sublist/collection |
| [`expenseReport-taxDetailsElement`](../schemas/expenseReport.md#expensereport-taxdetailselement) | sublist/element |
| [`expenseReportCollection`](../schemas/expenseReport.md#expensereportcollection) | collection page |
| [`expenseReportSelectOptions`](../schemas/expenseReport.md#expensereportselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`expenseReport-accountingBookDetailCollection`](../schemas/expenseReport.md#expensereport-accountingbookdetailcollection) | [`expenseReport-accountingBookDetailElement`](../schemas/expenseReport.md#expensereport-accountingbookdetailelement) |
| `appliedRules` | [`expenseReport-appliedRulesCollection`](../schemas/expenseReport.md#expensereport-appliedrulescollection) | [`expenseReport-appliedRulesElement`](../schemas/expenseReport.md#expensereport-appliedruleselement) |
| `expense` | [`expenseReport-expenseCollection`](../schemas/expenseReport.md#expensereport-expensecollection) | [`expenseReport-expenseElement`](../schemas/expenseReport.md#expensereport-expenseelement) |
| `taxDetails` | [`expenseReport-taxDetailsCollection`](../schemas/expenseReport.md#expensereport-taxdetailscollection) | [`expenseReport-taxDetailsElement`](../schemas/expenseReport.md#expensereport-taxdetailselement) |

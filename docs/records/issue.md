# issue

Browser tag `issue` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/issue`, instance `/issue/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/issue` | `operation--issue-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/issue` | `operation--issue-get` | Get list of records. |  | 200 OK → `issueCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/issue` | `operation--issue-patch` | Update records. | `issueCollection` | 202 Accepted; default → `nsError` |
| POST | `/issue` | `operation--issue-post` | Insert record. | `issue` | 200 OK → `issue`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/issue` | `operation--issue-put` | Insert or update records. | `issueCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/issue/{id}` | `operation--issue--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/issue/{id}` | `operation--issue--id--get` | Get record. |  | 200 OK → `issue`; 202 Accepted; default → `nsError` |
| PATCH | `/issue/{id}` | `operation--issue--id--patch` | Update record. | `issue` | 200 OK → `issue`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/issue/{id}` | `operation--issue--id--put` | Insert or update record. | `issue` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--issue-delete` | DELETE `/issue` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue-get` | GET `/issue` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue-patch` | PATCH `/issue` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue-post` | POST `/issue` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--issue-put` | PUT `/issue` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue--id--delete` | DELETE `/issue/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue--id--get` | GET `/issue/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--issue--id--patch` | PATCH `/issue/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--issue--id--put` | PUT `/issue/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [issue schemas](../schemas/issue.md).

| Definition | Role |
| --- | --- |
| [`issue`](../schemas/issue.md#issue) | record body |
| [`issue-brokenInVersionCollection`](../schemas/issue.md#issue-brokeninversioncollection) | sublist/collection |
| [`issue-brokenInVersionElement`](../schemas/issue.md#issue-brokeninversionelement) | sublist/element |
| [`issue-fixedInVersionCollection`](../schemas/issue.md#issue-fixedinversioncollection) | sublist/collection |
| [`issue-fixedInVersionElement`](../schemas/issue.md#issue-fixedinversionelement) | sublist/element |
| [`issue-relatedIssuesCollection`](../schemas/issue.md#issue-relatedissuescollection) | sublist/collection |
| [`issue-relatedIssuesElement`](../schemas/issue.md#issue-relatedissueselement) | sublist/element |
| [`issue-targetVersionCollection`](../schemas/issue.md#issue-targetversioncollection) | sublist/collection |
| [`issue-targetVersionElement`](../schemas/issue.md#issue-targetversionelement) | sublist/element |
| [`issueCollection`](../schemas/issue.md#issuecollection) | collection page |
| [`issueSelectOptions`](../schemas/issue.md#issueselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `brokenInVersion` | [`issue-brokenInVersionCollection`](../schemas/issue.md#issue-brokeninversioncollection) | [`issue-brokenInVersionElement`](../schemas/issue.md#issue-brokeninversionelement) |
| `fixedInVersion` | [`issue-fixedInVersionCollection`](../schemas/issue.md#issue-fixedinversioncollection) | [`issue-fixedInVersionElement`](../schemas/issue.md#issue-fixedinversionelement) |
| `relatedIssues` | [`issue-relatedIssuesCollection`](../schemas/issue.md#issue-relatedissuescollection) | [`issue-relatedIssuesElement`](../schemas/issue.md#issue-relatedissueselement) |
| `targetVersion` | [`issue-targetVersionCollection`](../schemas/issue.md#issue-targetversioncollection) | [`issue-targetVersionElement`](../schemas/issue.md#issue-targetversionelement) |

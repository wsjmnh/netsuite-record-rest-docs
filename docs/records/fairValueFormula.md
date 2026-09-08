# fairValueFormula

Browser tag `fairValueFormula` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/fairValueFormula`, instance `/fairValueFormula/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/fairValueFormula` | `operation--fairValueFormula-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/fairValueFormula` | `operation--fairValueFormula-get` | Get list of records. |  | 200 OK → `fairValueFormulaCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/fairValueFormula` | `operation--fairValueFormula-patch` | Update records. | `fairValueFormulaCollection` | 202 Accepted; default → `nsError` |
| POST | `/fairValueFormula` | `operation--fairValueFormula-post` | Insert record. | `fairValueFormula` | 200 OK → `fairValueFormula`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fairValueFormula` | `operation--fairValueFormula-put` | Insert or update records. | `fairValueFormulaCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/fairValueFormula/{id}` | `operation--fairValueFormula--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/fairValueFormula/{id}` | `operation--fairValueFormula--id--get` | Get record. |  | 200 OK → `fairValueFormula`; 202 Accepted; default → `nsError` |
| PATCH | `/fairValueFormula/{id}` | `operation--fairValueFormula--id--patch` | Update record. | `fairValueFormula` | 200 OK → `fairValueFormula`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/fairValueFormula/{id}` | `operation--fairValueFormula--id--put` | Insert or update record. | `fairValueFormula` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--fairValueFormula-delete` | DELETE `/fairValueFormula` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula-get` | GET `/fairValueFormula` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula-patch` | PATCH `/fairValueFormula` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula-post` | POST `/fairValueFormula` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--fairValueFormula-put` | PUT `/fairValueFormula` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula--id--delete` | DELETE `/fairValueFormula/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula--id--get` | GET `/fairValueFormula/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--fairValueFormula--id--patch` | PATCH `/fairValueFormula/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--fairValueFormula--id--put` | PUT `/fairValueFormula/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [fairValueFormula schemas](../schemas/fairValueFormula.md).

| Definition | Role |
| --- | --- |
| [`fairValueFormula`](../schemas/fairValueFormula.md#fairvalueformula) | record body |
| [`fairValueFormulaCollection`](../schemas/fairValueFormula.md#fairvalueformulacollection) | collection page |
| [`fairValueFormulaSelectOptions`](../schemas/fairValueFormula.md#fairvalueformulaselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.

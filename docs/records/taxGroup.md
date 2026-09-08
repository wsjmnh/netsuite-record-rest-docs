# taxGroup

Browser tag `taxGroup` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/taxGroup`, instance `/taxGroup/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/taxGroup` | `operation--taxGroup-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/taxGroup` | `operation--taxGroup-get` | Get list of records. |  | 200 OK → `taxGroupCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/taxGroup` | `operation--taxGroup-patch` | Update records. | `taxGroupCollection` | 202 Accepted; default → `nsError` |
| POST | `/taxGroup` | `operation--taxGroup-post` | Insert record. | `taxGroup` | 200 OK → `taxGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxGroup` | `operation--taxGroup-put` | Insert or update records. | `taxGroupCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/taxGroup/{id}` | `operation--taxGroup--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/taxGroup/{id}` | `operation--taxGroup--id--get` | Get record. |  | 200 OK → `taxGroup`; 202 Accepted; default → `nsError` |
| PATCH | `/taxGroup/{id}` | `operation--taxGroup--id--patch` | Update record. | `taxGroup` | 200 OK → `taxGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxGroup/{id}` | `operation--taxGroup--id--put` | Insert or update record. | `taxGroup` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--taxGroup-delete` | DELETE `/taxGroup` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup-get` | GET `/taxGroup` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup-patch` | PATCH `/taxGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup-post` | POST `/taxGroup` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--taxGroup-put` | PUT `/taxGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup--id--delete` | DELETE `/taxGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup--id--get` | GET `/taxGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxGroup--id--patch` | PATCH `/taxGroup/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--taxGroup--id--put` | PUT `/taxGroup/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [taxGroup schemas](../schemas/taxGroup.md).

| Definition | Role |
| --- | --- |
| [`taxGroup`](../schemas/taxGroup.md#taxgroup) | record body |
| [`taxGroup-taxItemCollection`](../schemas/taxGroup.md#taxgroup-taxitemcollection) | sublist/collection |
| [`taxGroup-taxItemElement`](../schemas/taxGroup.md#taxgroup-taxitemelement) | sublist/element |
| [`taxGroupCollection`](../schemas/taxGroup.md#taxgroupcollection) | collection page |
| [`taxGroupSelectOptions`](../schemas/taxGroup.md#taxgroupselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `taxItem` | [`taxGroup-taxItemCollection`](../schemas/taxGroup.md#taxgroup-taxitemcollection) | [`taxGroup-taxItemElement`](../schemas/taxGroup.md#taxgroup-taxitemelement) |

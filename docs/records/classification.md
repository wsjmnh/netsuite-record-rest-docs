# classification

Browser tag `classification` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/classification`, instance `/classification/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/classification` | `operation--classification-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/classification` | `operation--classification-get` | Get list of records. |  | 200 OK → `classificationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/classification` | `operation--classification-patch` | Update records. | `classificationCollection` | 202 Accepted; default → `nsError` |
| POST | `/classification` | `operation--classification-post` | Insert record. | `classification` | 200 OK → `classification`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/classification` | `operation--classification-put` | Insert or update records. | `classificationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/classification/{id}` | `operation--classification--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/classification/{id}` | `operation--classification--id--get` | Get record. |  | 200 OK → `classification`; 202 Accepted; default → `nsError` |
| PATCH | `/classification/{id}` | `operation--classification--id--patch` | Update record. | `classification` | 200 OK → `classification`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/classification/{id}` | `operation--classification--id--put` | Insert or update record. | `classification` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--classification-delete` | DELETE `/classification` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification-get` | GET `/classification` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification-patch` | PATCH `/classification` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification-post` | POST `/classification` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--classification-put` | PUT `/classification` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification--id--delete` | DELETE `/classification/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification--id--get` | GET `/classification/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--classification--id--patch` | PATCH `/classification/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--classification--id--put` | PUT `/classification/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [classification schemas](../schemas/classification.md).

| Definition | Role |
| --- | --- |
| [`classification`](../schemas/classification.md#classification) | record body |
| [`classification-classTranslationCollection`](../schemas/classification.md#classification-classtranslationcollection) | sublist/collection |
| [`classification-classTranslationElement`](../schemas/classification.md#classification-classtranslationelement) | sublist/element |
| [`classificationCollection`](../schemas/classification.md#classificationcollection) | collection page |
| [`classificationSelectOptions`](../schemas/classification.md#classificationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `classTranslation` | [`classification-classTranslationCollection`](../schemas/classification.md#classification-classtranslationcollection) | [`classification-classTranslationElement`](../schemas/classification.md#classification-classtranslationelement) |

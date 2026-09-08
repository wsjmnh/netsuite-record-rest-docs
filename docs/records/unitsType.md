# unitsType

Browser tag `unitsType` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/unitsType`, instance `/unitsType/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/unitsType` | `operation--unitsType-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/unitsType` | `operation--unitsType-get` | Get list of records. |  | 200 OK → `unitsTypeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/unitsType` | `operation--unitsType-patch` | Update records. | `unitsTypeCollection` | 202 Accepted; default → `nsError` |
| POST | `/unitsType` | `operation--unitsType-post` | Insert record. | `unitsType` | 200 OK → `unitsType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/unitsType` | `operation--unitsType-put` | Insert or update records. | `unitsTypeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/unitsType/{id}` | `operation--unitsType--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/unitsType/{id}` | `operation--unitsType--id--get` | Get record. |  | 200 OK → `unitsType`; 202 Accepted; default → `nsError` |
| PATCH | `/unitsType/{id}` | `operation--unitsType--id--patch` | Update record. | `unitsType` | 200 OK → `unitsType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/unitsType/{id}` | `operation--unitsType--id--put` | Insert or update record. | `unitsType` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--unitsType-delete` | DELETE `/unitsType` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType-get` | GET `/unitsType` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType-patch` | PATCH `/unitsType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType-post` | POST `/unitsType` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--unitsType-put` | PUT `/unitsType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType--id--delete` | DELETE `/unitsType/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType--id--get` | GET `/unitsType/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--unitsType--id--patch` | PATCH `/unitsType/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--unitsType--id--put` | PUT `/unitsType/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [unitsType schemas](../schemas/unitsType.md).

| Definition | Role |
| --- | --- |
| [`unitsType`](../schemas/unitsType.md#unitstype) | record body |
| [`unitsType-uomCollection`](../schemas/unitsType.md#unitstype-uomcollection) | sublist/collection |
| [`unitsType-uomElement`](../schemas/unitsType.md#unitstype-uomelement) | sublist/element |
| [`unitsTypeCollection`](../schemas/unitsType.md#unitstypecollection) | collection page |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `uom` | [`unitsType-uomCollection`](../schemas/unitsType.md#unitstype-uomcollection) | [`unitsType-uomElement`](../schemas/unitsType.md#unitstype-uomelement) |

# taxType

Browser tag `taxType` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/taxType`, instance `/taxType/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/taxType` | `operation--taxType-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/taxType` | `operation--taxType-get` | Get list of records. |  | 200 OK → `taxTypeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/taxType` | `operation--taxType-patch` | Update records. | `taxTypeCollection` | 202 Accepted; default → `nsError` |
| POST | `/taxType` | `operation--taxType-post` | Insert record. | `taxType` | 200 OK → `taxType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxType` | `operation--taxType-put` | Insert or update records. | `taxTypeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/taxType/{id}` | `operation--taxType--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/taxType/{id}` | `operation--taxType--id--get` | Get record. |  | 200 OK → `taxType`; 202 Accepted; default → `nsError` |
| PATCH | `/taxType/{id}` | `operation--taxType--id--patch` | Update record. | `taxType` | 200 OK → `taxType`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/taxType/{id}` | `operation--taxType--id--put` | Insert or update record. | `taxType` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--taxType-delete` | DELETE `/taxType` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType-get` | GET `/taxType` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType-patch` | PATCH `/taxType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType-post` | POST `/taxType` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--taxType-put` | PUT `/taxType` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType--id--delete` | DELETE `/taxType/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType--id--get` | GET `/taxType/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--taxType--id--patch` | PATCH `/taxType/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--taxType--id--put` | PUT `/taxType/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [taxType schemas](../schemas/taxType.md).

| Definition | Role |
| --- | --- |
| [`taxType`](../schemas/taxType.md#taxtype) | record body |
| [`taxType-nexusAccountsCollection`](../schemas/taxType.md#taxtype-nexusaccountscollection) | sublist/collection |
| [`taxType-nexusAccountsElement`](../schemas/taxType.md#taxtype-nexusaccountselement) | sublist/element |
| [`taxType-nexusesTaxCollection`](../schemas/taxType.md#taxtype-nexusestaxcollection) | sublist/collection |
| [`taxType-nexusesTaxElement`](../schemas/taxType.md#taxtype-nexusestaxelement) | sublist/element |
| [`taxTypeCollection`](../schemas/taxType.md#taxtypecollection) | collection page |
| [`taxTypeSelectOptions`](../schemas/taxType.md#taxtypeselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `nexusAccounts` | [`taxType-nexusAccountsCollection`](../schemas/taxType.md#taxtype-nexusaccountscollection) | [`taxType-nexusAccountsElement`](../schemas/taxType.md#taxtype-nexusaccountselement) |
| `nexusesTax` | [`taxType-nexusesTaxCollection`](../schemas/taxType.md#taxtype-nexusestaxcollection) | [`taxType-nexusesTaxElement`](../schemas/taxType.md#taxtype-nexusestaxelement) |

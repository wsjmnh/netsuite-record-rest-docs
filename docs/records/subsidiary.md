# subsidiary

Browser tag `subsidiary` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subsidiary`, instance `/subsidiary/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subsidiary` | `operation--subsidiary-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subsidiary` | `operation--subsidiary-get` | Get list of records. |  | 200 OK → `subsidiaryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subsidiary` | `operation--subsidiary-patch` | Update records. | `subsidiaryCollection` | 202 Accepted; default → `nsError` |
| POST | `/subsidiary` | `operation--subsidiary-post` | Insert record. | `subsidiary` | 200 OK → `subsidiary`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subsidiary` | `operation--subsidiary-put` | Insert or update records. | `subsidiaryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subsidiary/{id}` | `operation--subsidiary--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subsidiary/{id}` | `operation--subsidiary--id--get` | Get record. |  | 200 OK → `subsidiary`; 202 Accepted; default → `nsError` |
| PATCH | `/subsidiary/{id}` | `operation--subsidiary--id--patch` | Update record. | `subsidiary` | 200 OK → `subsidiary`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subsidiary/{id}` | `operation--subsidiary--id--put` | Insert or update record. | `subsidiary` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subsidiary-delete` | DELETE `/subsidiary` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary-get` | GET `/subsidiary` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary-patch` | PATCH `/subsidiary` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary-post` | POST `/subsidiary` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subsidiary-put` | PUT `/subsidiary` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary--id--delete` | DELETE `/subsidiary/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary--id--get` | GET `/subsidiary/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subsidiary--id--patch` | PATCH `/subsidiary/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subsidiary--id--put` | PUT `/subsidiary/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subsidiary schemas](../schemas/subsidiary.md).

| Definition | Role |
| --- | --- |
| [`subsidiary`](../schemas/subsidiary.md#subsidiary) | record body |
| [`subsidiary-accountingBookDetailCollection`](../schemas/subsidiary.md#subsidiary-accountingbookdetailcollection) | sublist/collection |
| [`subsidiary-accountingBookDetailElement`](../schemas/subsidiary.md#subsidiary-accountingbookdetailelement) | sublist/element |
| [`subsidiary-classTranslationCollection`](../schemas/subsidiary.md#subsidiary-classtranslationcollection) | sublist/collection |
| [`subsidiary-classTranslationElement`](../schemas/subsidiary.md#subsidiary-classtranslationelement) | sublist/element |
| [`subsidiary-mainAddress`](../schemas/subsidiary.md#subsidiary-mainaddress) | related |
| [`subsidiary-nexusCollection`](../schemas/subsidiary.md#subsidiary-nexuscollection) | sublist/collection |
| [`subsidiary-nexusElement`](../schemas/subsidiary.md#subsidiary-nexuselement) | sublist/element |
| [`subsidiary-returnAddress`](../schemas/subsidiary.md#subsidiary-returnaddress) | related |
| [`subsidiary-shippingAddress`](../schemas/subsidiary.md#subsidiary-shippingaddress) | related |
| [`subsidiary-taxRegistrationCollection`](../schemas/subsidiary.md#subsidiary-taxregistrationcollection) | sublist/collection |
| [`subsidiary-taxRegistrationElement`](../schemas/subsidiary.md#subsidiary-taxregistrationelement) | sublist/element |
| [`subsidiaryCollection`](../schemas/subsidiary.md#subsidiarycollection) | collection page |
| [`subsidiarySelectOptions`](../schemas/subsidiary.md#subsidiaryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`subsidiary-accountingBookDetailCollection`](../schemas/subsidiary.md#subsidiary-accountingbookdetailcollection) | [`subsidiary-accountingBookDetailElement`](../schemas/subsidiary.md#subsidiary-accountingbookdetailelement) |
| `classTranslation` | [`subsidiary-classTranslationCollection`](../schemas/subsidiary.md#subsidiary-classtranslationcollection) | [`subsidiary-classTranslationElement`](../schemas/subsidiary.md#subsidiary-classtranslationelement) |
| `nexus` | [`subsidiary-nexusCollection`](../schemas/subsidiary.md#subsidiary-nexuscollection) | [`subsidiary-nexusElement`](../schemas/subsidiary.md#subsidiary-nexuselement) |
| `taxRegistration` | [`subsidiary-taxRegistrationCollection`](../schemas/subsidiary.md#subsidiary-taxregistrationcollection) | [`subsidiary-taxRegistrationElement`](../schemas/subsidiary.md#subsidiary-taxregistrationelement) |

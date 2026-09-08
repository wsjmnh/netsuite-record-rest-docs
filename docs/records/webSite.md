# webSite

Browser tag `webSite` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/webSite`, instance `/webSite/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/webSite` | `operation--webSite-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/webSite` | `operation--webSite-get` | Get list of records. |  | 200 OK → `webSiteCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/webSite` | `operation--webSite-patch` | Update records. | `webSiteCollection` | 202 Accepted; default → `nsError` |
| POST | `/webSite` | `operation--webSite-post` | Insert record. | `webSite` | 200 OK → `webSite`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/webSite` | `operation--webSite-put` | Insert or update records. | `webSiteCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/webSite/{id}` | `operation--webSite--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/webSite/{id}` | `operation--webSite--id--get` | Get record. |  | 200 OK → `webSite`; 202 Accepted; default → `nsError` |
| PATCH | `/webSite/{id}` | `operation--webSite--id--patch` | Update record. | `webSite` | 200 OK → `webSite`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/webSite/{id}` | `operation--webSite--id--put` | Insert or update record. | `webSite` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--webSite-delete` | DELETE `/webSite` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite-get` | GET `/webSite` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite-patch` | PATCH `/webSite` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite-post` | POST `/webSite` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--webSite-put` | PUT `/webSite` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite--id--delete` | DELETE `/webSite/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite--id--get` | GET `/webSite/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--webSite--id--patch` | PATCH `/webSite/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--webSite--id--put` | PUT `/webSite/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [webSite schemas](../schemas/webSite.md).

| Definition | Role |
| --- | --- |
| [`webSite`](../schemas/webSite.md#website) | record body |
| [`webSite-entryPointsCollection`](../schemas/webSite.md#website-entrypointscollection) | sublist/collection |
| [`webSite-entryPointsElement`](../schemas/webSite.md#website-entrypointselement) | sublist/element |
| [`webSite-fieldsetCollection`](../schemas/webSite.md#website-fieldsetcollection) | sublist/collection |
| [`webSite-fieldsetElement`](../schemas/webSite.md#website-fieldsetelement) | sublist/element |
| [`webSiteCollection`](../schemas/webSite.md#websitecollection) | collection page |
| [`webSiteSelectOptions`](../schemas/webSite.md#websiteselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `entryPoints` | [`webSite-entryPointsCollection`](../schemas/webSite.md#website-entrypointscollection) | [`webSite-entryPointsElement`](../schemas/webSite.md#website-entrypointselement) |
| `fieldset` | [`webSite-fieldsetCollection`](../schemas/webSite.md#website-fieldsetcollection) | [`webSite-fieldsetElement`](../schemas/webSite.md#website-fieldsetelement) |

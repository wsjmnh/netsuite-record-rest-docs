# discountItem

Browser tag `discountItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/discountItem`, instance `/discountItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/discountItem` | `operation--discountItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/discountItem` | `operation--discountItem-get` | Get list of records. |  | 200 OK → `discountItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/discountItem` | `operation--discountItem-patch` | Update records. | `discountItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/discountItem` | `operation--discountItem-post` | Insert record. | `discountItem` | 200 OK → `discountItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/discountItem` | `operation--discountItem-put` | Insert or update records. | `discountItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/discountItem/{id}` | `operation--discountItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/discountItem/{id}` | `operation--discountItem--id--get` | Get record. |  | 200 OK → `discountItem`; 202 Accepted; default → `nsError` |
| PATCH | `/discountItem/{id}` | `operation--discountItem--id--patch` | Update record. | `discountItem` | 200 OK → `discountItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/discountItem/{id}` | `operation--discountItem--id--put` | Insert or update record. | `discountItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--discountItem-delete` | DELETE `/discountItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem-get` | GET `/discountItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem-patch` | PATCH `/discountItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem-post` | POST `/discountItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--discountItem-put` | PUT `/discountItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem--id--delete` | DELETE `/discountItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem--id--get` | GET `/discountItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--discountItem--id--patch` | PATCH `/discountItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--discountItem--id--put` | PUT `/discountItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [discountItem schemas](../schemas/discountItem.md).

| Definition | Role |
| --- | --- |
| [`discountItem`](../schemas/discountItem.md#discountitem) | record body |
| [`discountItem-translationsCollection`](../schemas/discountItem.md#discountitem-translationscollection) | sublist/collection |
| [`discountItem-translationsElement`](../schemas/discountItem.md#discountitem-translationselement) | sublist/element |
| [`discountItemCollection`](../schemas/discountItem.md#discountitemcollection) | collection page |
| [`discountItemSelectOptions`](../schemas/discountItem.md#discountitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `translations` | [`discountItem-translationsCollection`](../schemas/discountItem.md#discountitem-translationscollection) | [`discountItem-translationsElement`](../schemas/discountItem.md#discountitem-translationselement) |

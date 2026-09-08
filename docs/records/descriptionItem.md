# descriptionItem

Browser tag `descriptionItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/descriptionItem`, instance `/descriptionItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/descriptionItem` | `operation--descriptionItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/descriptionItem` | `operation--descriptionItem-get` | Get list of records. |  | 200 OK → `descriptionItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/descriptionItem` | `operation--descriptionItem-patch` | Update records. | `descriptionItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/descriptionItem` | `operation--descriptionItem-post` | Insert record. | `descriptionItem` | 200 OK → `descriptionItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/descriptionItem` | `operation--descriptionItem-put` | Insert or update records. | `descriptionItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/descriptionItem/{id}` | `operation--descriptionItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/descriptionItem/{id}` | `operation--descriptionItem--id--get` | Get record. |  | 200 OK → `descriptionItem`; 202 Accepted; default → `nsError` |
| PATCH | `/descriptionItem/{id}` | `operation--descriptionItem--id--patch` | Update record. | `descriptionItem` | 200 OK → `descriptionItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/descriptionItem/{id}` | `operation--descriptionItem--id--put` | Insert or update record. | `descriptionItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--descriptionItem-delete` | DELETE `/descriptionItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem-get` | GET `/descriptionItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem-patch` | PATCH `/descriptionItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem-post` | POST `/descriptionItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--descriptionItem-put` | PUT `/descriptionItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem--id--delete` | DELETE `/descriptionItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem--id--get` | GET `/descriptionItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--descriptionItem--id--patch` | PATCH `/descriptionItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--descriptionItem--id--put` | PUT `/descriptionItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [descriptionItem schemas](../schemas/descriptionItem.md).

| Definition | Role |
| --- | --- |
| [`descriptionItem`](../schemas/descriptionItem.md#descriptionitem) | record body |
| [`descriptionItem-translationsCollection`](../schemas/descriptionItem.md#descriptionitem-translationscollection) | sublist/collection |
| [`descriptionItem-translationsElement`](../schemas/descriptionItem.md#descriptionitem-translationselement) | sublist/element |
| [`descriptionItemCollection`](../schemas/descriptionItem.md#descriptionitemcollection) | collection page |
| [`descriptionItemSelectOptions`](../schemas/descriptionItem.md#descriptionitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `translations` | [`descriptionItem-translationsCollection`](../schemas/descriptionItem.md#descriptionitem-translationscollection) | [`descriptionItem-translationsElement`](../schemas/descriptionItem.md#descriptionitem-translationselement) |

# itemGroup

Browser tag `itemGroup` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemGroup`, instance `/itemGroup/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemGroup` | `operation--itemGroup-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemGroup` | `operation--itemGroup-get` | Get list of records. |  | 200 OK → `itemGroupCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemGroup` | `operation--itemGroup-patch` | Update records. | `itemGroupCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemGroup` | `operation--itemGroup-post` | Insert record. | `itemGroup` | 200 OK → `itemGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemGroup` | `operation--itemGroup-put` | Insert or update records. | `itemGroupCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemGroup/{id}` | `operation--itemGroup--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemGroup/{id}` | `operation--itemGroup--id--get` | Get record. |  | 200 OK → `itemGroup`; 202 Accepted; default → `nsError` |
| PATCH | `/itemGroup/{id}` | `operation--itemGroup--id--patch` | Update record. | `itemGroup` | 200 OK → `itemGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemGroup/{id}` | `operation--itemGroup--id--put` | Insert or update record. | `itemGroup` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemGroup-delete` | DELETE `/itemGroup` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup-get` | GET `/itemGroup` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup-patch` | PATCH `/itemGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup-post` | POST `/itemGroup` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemGroup-put` | PUT `/itemGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup--id--delete` | DELETE `/itemGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup--id--get` | GET `/itemGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemGroup--id--patch` | PATCH `/itemGroup/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemGroup--id--put` | PUT `/itemGroup/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [itemGroup schemas](../schemas/itemGroup.md).

| Definition | Role |
| --- | --- |
| [`itemGroup`](../schemas/itemGroup.md#itemgroup) | record body |
| [`itemGroup-hierarchyVersionsCollection`](../schemas/itemGroup.md#itemgroup-hierarchyversionscollection) | sublist/collection |
| [`itemGroup-hierarchyVersionsElement`](../schemas/itemGroup.md#itemgroup-hierarchyversionselement) | sublist/element |
| [`itemGroup-memberCollection`](../schemas/itemGroup.md#itemgroup-membercollection) | sublist/collection |
| [`itemGroup-memberElement`](../schemas/itemGroup.md#itemgroup-memberelement) | sublist/element |
| [`itemGroup-translationsCollection`](../schemas/itemGroup.md#itemgroup-translationscollection) | sublist/collection |
| [`itemGroup-translationsElement`](../schemas/itemGroup.md#itemgroup-translationselement) | sublist/element |
| [`itemGroupCollection`](../schemas/itemGroup.md#itemgroupcollection) | collection page |
| [`itemGroupSelectOptions`](../schemas/itemGroup.md#itemgroupselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `hierarchyVersions` | [`itemGroup-hierarchyVersionsCollection`](../schemas/itemGroup.md#itemgroup-hierarchyversionscollection) | [`itemGroup-hierarchyVersionsElement`](../schemas/itemGroup.md#itemgroup-hierarchyversionselement) |
| `member` | [`itemGroup-memberCollection`](../schemas/itemGroup.md#itemgroup-membercollection) | [`itemGroup-memberElement`](../schemas/itemGroup.md#itemgroup-memberelement) |
| `translations` | [`itemGroup-translationsCollection`](../schemas/itemGroup.md#itemgroup-translationscollection) | [`itemGroup-translationsElement`](../schemas/itemGroup.md#itemgroup-translationselement) |

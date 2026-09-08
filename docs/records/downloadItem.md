# downloadItem

Browser tag `downloadItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/downloadItem`, instance `/downloadItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/downloadItem` | `operation--downloadItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/downloadItem` | `operation--downloadItem-get` | Get list of records. |  | 200 OK → `downloadItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/downloadItem` | `operation--downloadItem-patch` | Update records. | `downloadItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/downloadItem` | `operation--downloadItem-post` | Insert record. | `downloadItem` | 200 OK → `downloadItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/downloadItem` | `operation--downloadItem-put` | Insert or update records. | `downloadItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/downloadItem/{id}` | `operation--downloadItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/downloadItem/{id}` | `operation--downloadItem--id--get` | Get record. |  | 200 OK → `downloadItem`; 202 Accepted; default → `nsError` |
| PATCH | `/downloadItem/{id}` | `operation--downloadItem--id--patch` | Update record. | `downloadItem` | 200 OK → `downloadItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/downloadItem/{id}` | `operation--downloadItem--id--put` | Insert or update record. | `downloadItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--downloadItem-delete` | DELETE `/downloadItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem-get` | GET `/downloadItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem-patch` | PATCH `/downloadItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem-post` | POST `/downloadItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--downloadItem-put` | PUT `/downloadItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem--id--delete` | DELETE `/downloadItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem--id--get` | GET `/downloadItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--downloadItem--id--patch` | PATCH `/downloadItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--downloadItem--id--put` | PUT `/downloadItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [downloadItem schemas](../schemas/downloadItem.md).

| Definition | Role |
| --- | --- |
| [`downloadItem`](../schemas/downloadItem.md#downloaditem) | record body |
| [`downloadItem-accountingBookDetailCollection`](../schemas/downloadItem.md#downloaditem-accountingbookdetailcollection) | sublist/collection |
| [`downloadItem-accountingBookDetailElement`](../schemas/downloadItem.md#downloaditem-accountingbookdetailelement) | sublist/element |
| [`downloadItem-correlatedItemsCollection`](../schemas/downloadItem.md#downloaditem-correlateditemscollection) | sublist/collection |
| [`downloadItem-correlatedItemsElement`](../schemas/downloadItem.md#downloaditem-correlateditemselement) | sublist/element |
| [`downloadItem-presentationItemCollection`](../schemas/downloadItem.md#downloaditem-presentationitemcollection) | sublist/collection |
| [`downloadItem-presentationItemElement`](../schemas/downloadItem.md#downloaditem-presentationitemelement) | sublist/element |
| [`downloadItem-price`](../schemas/downloadItem.md#downloaditem-price) | related |
| [`downloadItem-priceElement`](../schemas/downloadItem.md#downloaditem-priceelement) | sublist/element |
| [`downloadItem-siteCategoryCollection`](../schemas/downloadItem.md#downloaditem-sitecategorycollection) | sublist/collection |
| [`downloadItem-siteCategoryElement`](../schemas/downloadItem.md#downloaditem-sitecategoryelement) | sublist/element |
| [`downloadItem-translationsCollection`](../schemas/downloadItem.md#downloaditem-translationscollection) | sublist/collection |
| [`downloadItem-translationsElement`](../schemas/downloadItem.md#downloaditem-translationselement) | sublist/element |
| [`downloadItemCollection`](../schemas/downloadItem.md#downloaditemcollection) | collection page |
| [`downloadItemSelectOptions`](../schemas/downloadItem.md#downloaditemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`downloadItem-accountingBookDetailCollection`](../schemas/downloadItem.md#downloaditem-accountingbookdetailcollection) | [`downloadItem-accountingBookDetailElement`](../schemas/downloadItem.md#downloaditem-accountingbookdetailelement) |
| `correlatedItems` | [`downloadItem-correlatedItemsCollection`](../schemas/downloadItem.md#downloaditem-correlateditemscollection) | [`downloadItem-correlatedItemsElement`](../schemas/downloadItem.md#downloaditem-correlateditemselement) |
| `presentationItem` | [`downloadItem-presentationItemCollection`](../schemas/downloadItem.md#downloaditem-presentationitemcollection) | [`downloadItem-presentationItemElement`](../schemas/downloadItem.md#downloaditem-presentationitemelement) |
| `siteCategory` | [`downloadItem-siteCategoryCollection`](../schemas/downloadItem.md#downloaditem-sitecategorycollection) | [`downloadItem-siteCategoryElement`](../schemas/downloadItem.md#downloaditem-sitecategoryelement) |
| `translations` | [`downloadItem-translationsCollection`](../schemas/downloadItem.md#downloaditem-translationscollection) | [`downloadItem-translationsElement`](../schemas/downloadItem.md#downloaditem-translationselement) |

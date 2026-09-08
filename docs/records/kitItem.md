# kitItem

Browser tag `kitItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/kitItem`, instance `/kitItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/kitItem` | `operation--kitItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/kitItem` | `operation--kitItem-get` | Get list of records. |  | 200 OK → `kitItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/kitItem` | `operation--kitItem-patch` | Update records. | `kitItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/kitItem` | `operation--kitItem-post` | Insert record. | `kitItem` | 200 OK → `kitItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/kitItem` | `operation--kitItem-put` | Insert or update records. | `kitItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/kitItem/{id}` | `operation--kitItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/kitItem/{id}` | `operation--kitItem--id--get` | Get record. |  | 200 OK → `kitItem`; 202 Accepted; default → `nsError` |
| PATCH | `/kitItem/{id}` | `operation--kitItem--id--patch` | Update record. | `kitItem` | 200 OK → `kitItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/kitItem/{id}` | `operation--kitItem--id--put` | Insert or update record. | `kitItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--kitItem-delete` | DELETE `/kitItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem-get` | GET `/kitItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem-patch` | PATCH `/kitItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem-post` | POST `/kitItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--kitItem-put` | PUT `/kitItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem--id--delete` | DELETE `/kitItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem--id--get` | GET `/kitItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--kitItem--id--patch` | PATCH `/kitItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--kitItem--id--put` | PUT `/kitItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [kitItem schemas](../schemas/kitItem.md).

| Definition | Role |
| --- | --- |
| [`kitItem`](../schemas/kitItem.md#kititem) | record body |
| [`kitItem-accountingBookDetailCollection`](../schemas/kitItem.md#kititem-accountingbookdetailcollection) | sublist/collection |
| [`kitItem-accountingBookDetailElement`](../schemas/kitItem.md#kititem-accountingbookdetailelement) | sublist/element |
| [`kitItem-correlatedItemsCollection`](../schemas/kitItem.md#kititem-correlateditemscollection) | sublist/collection |
| [`kitItem-correlatedItemsElement`](../schemas/kitItem.md#kititem-correlateditemselement) | sublist/element |
| [`kitItem-hierarchyVersionsCollection`](../schemas/kitItem.md#kititem-hierarchyversionscollection) | sublist/collection |
| [`kitItem-hierarchyVersionsElement`](../schemas/kitItem.md#kititem-hierarchyversionselement) | sublist/element |
| [`kitItem-memberCollection`](../schemas/kitItem.md#kititem-membercollection) | sublist/collection |
| [`kitItem-memberElement`](../schemas/kitItem.md#kititem-memberelement) | sublist/element |
| [`kitItem-presentationItemCollection`](../schemas/kitItem.md#kititem-presentationitemcollection) | sublist/collection |
| [`kitItem-presentationItemElement`](../schemas/kitItem.md#kititem-presentationitemelement) | sublist/element |
| [`kitItem-price`](../schemas/kitItem.md#kititem-price) | related |
| [`kitItem-priceElement`](../schemas/kitItem.md#kititem-priceelement) | sublist/element |
| [`kitItem-siteCategoryCollection`](../schemas/kitItem.md#kititem-sitecategorycollection) | sublist/collection |
| [`kitItem-siteCategoryElement`](../schemas/kitItem.md#kititem-sitecategoryelement) | sublist/element |
| [`kitItem-translationsCollection`](../schemas/kitItem.md#kititem-translationscollection) | sublist/collection |
| [`kitItem-translationsElement`](../schemas/kitItem.md#kititem-translationselement) | sublist/element |
| [`kitItemCollection`](../schemas/kitItem.md#kititemcollection) | collection page |
| [`kitItemSelectOptions`](../schemas/kitItem.md#kititemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`kitItem-accountingBookDetailCollection`](../schemas/kitItem.md#kititem-accountingbookdetailcollection) | [`kitItem-accountingBookDetailElement`](../schemas/kitItem.md#kititem-accountingbookdetailelement) |
| `correlatedItems` | [`kitItem-correlatedItemsCollection`](../schemas/kitItem.md#kititem-correlateditemscollection) | [`kitItem-correlatedItemsElement`](../schemas/kitItem.md#kititem-correlateditemselement) |
| `hierarchyVersions` | [`kitItem-hierarchyVersionsCollection`](../schemas/kitItem.md#kititem-hierarchyversionscollection) | [`kitItem-hierarchyVersionsElement`](../schemas/kitItem.md#kititem-hierarchyversionselement) |
| `member` | [`kitItem-memberCollection`](../schemas/kitItem.md#kititem-membercollection) | [`kitItem-memberElement`](../schemas/kitItem.md#kititem-memberelement) |
| `presentationItem` | [`kitItem-presentationItemCollection`](../schemas/kitItem.md#kititem-presentationitemcollection) | [`kitItem-presentationItemElement`](../schemas/kitItem.md#kititem-presentationitemelement) |
| `siteCategory` | [`kitItem-siteCategoryCollection`](../schemas/kitItem.md#kititem-sitecategorycollection) | [`kitItem-siteCategoryElement`](../schemas/kitItem.md#kititem-sitecategoryelement) |
| `translations` | [`kitItem-translationsCollection`](../schemas/kitItem.md#kititem-translationscollection) | [`kitItem-translationsElement`](../schemas/kitItem.md#kititem-translationselement) |

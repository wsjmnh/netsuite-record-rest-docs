# nonInventorySaleItem

Browser tag `nonInventorySaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/nonInventorySaleItem`, instance `/nonInventorySaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/nonInventorySaleItem` | `operation--nonInventorySaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/nonInventorySaleItem` | `operation--nonInventorySaleItem-get` | Get list of records. |  | 200 OK → `nonInventorySaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventorySaleItem` | `operation--nonInventorySaleItem-patch` | Update records. | `nonInventorySaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/nonInventorySaleItem` | `operation--nonInventorySaleItem-post` | Insert record. | `nonInventorySaleItem` | 200 OK → `nonInventorySaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventorySaleItem` | `operation--nonInventorySaleItem-put` | Insert or update records. | `nonInventorySaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/nonInventorySaleItem/{id}` | `operation--nonInventorySaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/nonInventorySaleItem/{id}` | `operation--nonInventorySaleItem--id--get` | Get record. |  | 200 OK → `nonInventorySaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventorySaleItem/{id}` | `operation--nonInventorySaleItem--id--patch` | Update record. | `nonInventorySaleItem` | 200 OK → `nonInventorySaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventorySaleItem/{id}` | `operation--nonInventorySaleItem--id--put` | Insert or update record. | `nonInventorySaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--nonInventorySaleItem-delete` | DELETE `/nonInventorySaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem-get` | GET `/nonInventorySaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem-patch` | PATCH `/nonInventorySaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem-post` | POST `/nonInventorySaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--nonInventorySaleItem-put` | PUT `/nonInventorySaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem--id--delete` | DELETE `/nonInventorySaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem--id--get` | GET `/nonInventorySaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventorySaleItem--id--patch` | PATCH `/nonInventorySaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--nonInventorySaleItem--id--put` | PUT `/nonInventorySaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [nonInventorySaleItem schemas](../schemas/nonInventorySaleItem.md).

| Definition | Role |
| --- | --- |
| [`nonInventorySaleItem`](../schemas/nonInventorySaleItem.md#noninventorysaleitem) | record body |
| [`nonInventorySaleItem-accountingBookDetailCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-accountingbookdetailcollection) | sublist/collection |
| [`nonInventorySaleItem-accountingBookDetailElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-accountingbookdetailelement) | sublist/element |
| [`nonInventorySaleItem-correlatedItemsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-correlateditemscollection) | sublist/collection |
| [`nonInventorySaleItem-correlatedItemsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-correlateditemselement) | sublist/element |
| [`nonInventorySaleItem-hierarchyVersionsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-hierarchyversionscollection) | sublist/collection |
| [`nonInventorySaleItem-hierarchyVersionsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-hierarchyversionselement) | sublist/element |
| [`nonInventorySaleItem-presentationItemCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-presentationitemcollection) | sublist/collection |
| [`nonInventorySaleItem-presentationItemElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-presentationitemelement) | sublist/element |
| [`nonInventorySaleItem-price`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-price) | related |
| [`nonInventorySaleItem-priceElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-priceelement) | sublist/element |
| [`nonInventorySaleItem-siteCategoryCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-sitecategorycollection) | sublist/collection |
| [`nonInventorySaleItem-siteCategoryElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-sitecategoryelement) | sublist/element |
| [`nonInventorySaleItem-translationsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-translationscollection) | sublist/collection |
| [`nonInventorySaleItem-translationsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-translationselement) | sublist/element |
| [`nonInventorySaleItemCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitemcollection) | collection page |
| [`nonInventorySaleItemSelectOptions`](../schemas/nonInventorySaleItem.md#noninventorysaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`nonInventorySaleItem-accountingBookDetailCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-accountingbookdetailcollection) | [`nonInventorySaleItem-accountingBookDetailElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-accountingbookdetailelement) |
| `correlatedItems` | [`nonInventorySaleItem-correlatedItemsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-correlateditemscollection) | [`nonInventorySaleItem-correlatedItemsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-correlateditemselement) |
| `hierarchyVersions` | [`nonInventorySaleItem-hierarchyVersionsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-hierarchyversionscollection) | [`nonInventorySaleItem-hierarchyVersionsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-hierarchyversionselement) |
| `presentationItem` | [`nonInventorySaleItem-presentationItemCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-presentationitemcollection) | [`nonInventorySaleItem-presentationItemElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-presentationitemelement) |
| `siteCategory` | [`nonInventorySaleItem-siteCategoryCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-sitecategorycollection) | [`nonInventorySaleItem-siteCategoryElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-sitecategoryelement) |
| `translations` | [`nonInventorySaleItem-translationsCollection`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-translationscollection) | [`nonInventorySaleItem-translationsElement`](../schemas/nonInventorySaleItem.md#noninventorysaleitem-translationselement) |

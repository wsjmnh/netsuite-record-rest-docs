# nonInventoryResaleItem

Browser tag `nonInventoryResaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/nonInventoryResaleItem`, instance `/nonInventoryResaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/nonInventoryResaleItem` | `operation--nonInventoryResaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/nonInventoryResaleItem` | `operation--nonInventoryResaleItem-get` | Get list of records. |  | 200 OK → `nonInventoryResaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventoryResaleItem` | `operation--nonInventoryResaleItem-patch` | Update records. | `nonInventoryResaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/nonInventoryResaleItem` | `operation--nonInventoryResaleItem-post` | Insert record. | `nonInventoryResaleItem` | 200 OK → `nonInventoryResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventoryResaleItem` | `operation--nonInventoryResaleItem-put` | Insert or update records. | `nonInventoryResaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/nonInventoryResaleItem/{id}` | `operation--nonInventoryResaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/nonInventoryResaleItem/{id}` | `operation--nonInventoryResaleItem--id--get` | Get record. |  | 200 OK → `nonInventoryResaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventoryResaleItem/{id}` | `operation--nonInventoryResaleItem--id--patch` | Update record. | `nonInventoryResaleItem` | 200 OK → `nonInventoryResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventoryResaleItem/{id}` | `operation--nonInventoryResaleItem--id--put` | Insert or update record. | `nonInventoryResaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--nonInventoryResaleItem-delete` | DELETE `/nonInventoryResaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem-get` | GET `/nonInventoryResaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem-patch` | PATCH `/nonInventoryResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem-post` | POST `/nonInventoryResaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--nonInventoryResaleItem-put` | PUT `/nonInventoryResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem--id--delete` | DELETE `/nonInventoryResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem--id--get` | GET `/nonInventoryResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryResaleItem--id--patch` | PATCH `/nonInventoryResaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--nonInventoryResaleItem--id--put` | PUT `/nonInventoryResaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [nonInventoryResaleItem schemas](../schemas/nonInventoryResaleItem.md).

| Definition | Role |
| --- | --- |
| [`nonInventoryResaleItem`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem) | record body |
| [`nonInventoryResaleItem-accountingBookDetailCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-accountingbookdetailcollection) | sublist/collection |
| [`nonInventoryResaleItem-accountingBookDetailElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-accountingbookdetailelement) | sublist/element |
| [`nonInventoryResaleItem-correlatedItemsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-correlateditemscollection) | sublist/collection |
| [`nonInventoryResaleItem-correlatedItemsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-correlateditemselement) | sublist/element |
| [`nonInventoryResaleItem-hierarchyVersionsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-hierarchyversionscollection) | sublist/collection |
| [`nonInventoryResaleItem-hierarchyVersionsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-hierarchyversionselement) | sublist/element |
| [`nonInventoryResaleItem-itemVendor-itemVendorPrice`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendor-itemvendorprice) | related |
| [`nonInventoryResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`nonInventoryResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`nonInventoryResaleItem-itemVendorCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendorcollection) | sublist/collection |
| [`nonInventoryResaleItem-itemVendorElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendorelement) | sublist/element |
| [`nonInventoryResaleItem-presentationItemCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-presentationitemcollection) | sublist/collection |
| [`nonInventoryResaleItem-presentationItemElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-presentationitemelement) | sublist/element |
| [`nonInventoryResaleItem-price`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-price) | related |
| [`nonInventoryResaleItem-priceElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-priceelement) | sublist/element |
| [`nonInventoryResaleItem-siteCategoryCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-sitecategorycollection) | sublist/collection |
| [`nonInventoryResaleItem-siteCategoryElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-sitecategoryelement) | sublist/element |
| [`nonInventoryResaleItem-translationsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-translationscollection) | sublist/collection |
| [`nonInventoryResaleItem-translationsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-translationselement) | sublist/element |
| [`nonInventoryResaleItemCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitemcollection) | collection page |
| [`nonInventoryResaleItemSelectOptions`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`nonInventoryResaleItem-accountingBookDetailCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-accountingbookdetailcollection) | [`nonInventoryResaleItem-accountingBookDetailElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-accountingbookdetailelement) |
| `correlatedItems` | [`nonInventoryResaleItem-correlatedItemsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-correlateditemscollection) | [`nonInventoryResaleItem-correlatedItemsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-correlateditemselement) |
| `hierarchyVersions` | [`nonInventoryResaleItem-hierarchyVersionsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-hierarchyversionscollection) | [`nonInventoryResaleItem-hierarchyVersionsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-hierarchyversionselement) |
| `itemVendor` | [`nonInventoryResaleItem-itemVendorCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendorcollection) | [`nonInventoryResaleItem-itemVendorElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-itemvendorelement) |
| `presentationItem` | [`nonInventoryResaleItem-presentationItemCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-presentationitemcollection) | [`nonInventoryResaleItem-presentationItemElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-presentationitemelement) |
| `siteCategory` | [`nonInventoryResaleItem-siteCategoryCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-sitecategorycollection) | [`nonInventoryResaleItem-siteCategoryElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-sitecategoryelement) |
| `translations` | [`nonInventoryResaleItem-translationsCollection`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-translationscollection) | [`nonInventoryResaleItem-translationsElement`](../schemas/nonInventoryResaleItem.md#noninventoryresaleitem-translationselement) |

# inventoryItem

Browser tag `inventoryItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/inventoryItem`, instance `/inventoryItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/inventoryItem` | `operation--inventoryItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/inventoryItem` | `operation--inventoryItem-get` | Get list of records. |  | 200 OK → `inventoryItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryItem` | `operation--inventoryItem-patch` | Update records. | `inventoryItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/inventoryItem` | `operation--inventoryItem-post` | Insert record. | `inventoryItem` | 200 OK → `inventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryItem` | `operation--inventoryItem-put` | Insert or update records. | `inventoryItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/inventoryItem/{id}` | `operation--inventoryItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/inventoryItem/{id}` | `operation--inventoryItem--id--get` | Get record. |  | 200 OK → `inventoryItem`; 202 Accepted; default → `nsError` |
| PATCH | `/inventoryItem/{id}` | `operation--inventoryItem--id--patch` | Update record. | `inventoryItem` | 200 OK → `inventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/inventoryItem/{id}` | `operation--inventoryItem--id--put` | Insert or update record. | `inventoryItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--inventoryItem-delete` | DELETE `/inventoryItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem-get` | GET `/inventoryItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem-patch` | PATCH `/inventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem-post` | POST `/inventoryItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--inventoryItem-put` | PUT `/inventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem--id--delete` | DELETE `/inventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem--id--get` | GET `/inventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--inventoryItem--id--patch` | PATCH `/inventoryItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--inventoryItem--id--put` | PUT `/inventoryItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [inventoryItem schemas](../schemas/inventoryItem.md).

| Definition | Role |
| --- | --- |
| [`inventoryItem`](../schemas/inventoryItem.md#inventoryitem) | record body |
| [`inventoryItem-accountingBookDetailCollection`](../schemas/inventoryItem.md#inventoryitem-accountingbookdetailcollection) | sublist/collection |
| [`inventoryItem-accountingBookDetailElement`](../schemas/inventoryItem.md#inventoryitem-accountingbookdetailelement) | sublist/element |
| [`inventoryItem-binNumberCollection`](../schemas/inventoryItem.md#inventoryitem-binnumbercollection) | sublist/collection |
| [`inventoryItem-binNumberElement`](../schemas/inventoryItem.md#inventoryitem-binnumberelement) | sublist/element |
| [`inventoryItem-consignedlocationsCollection`](../schemas/inventoryItem.md#inventoryitem-consignedlocationscollection) | sublist/collection |
| [`inventoryItem-consignedlocationsElement`](../schemas/inventoryItem.md#inventoryitem-consignedlocationselement) | sublist/element |
| [`inventoryItem-correlatedItemsCollection`](../schemas/inventoryItem.md#inventoryitem-correlateditemscollection) | sublist/collection |
| [`inventoryItem-correlatedItemsElement`](../schemas/inventoryItem.md#inventoryitem-correlateditemselement) | sublist/element |
| [`inventoryItem-hierarchyVersionsCollection`](../schemas/inventoryItem.md#inventoryitem-hierarchyversionscollection) | sublist/collection |
| [`inventoryItem-hierarchyVersionsElement`](../schemas/inventoryItem.md#inventoryitem-hierarchyversionselement) | sublist/element |
| [`inventoryItem-itemVendor-itemVendorPrice`](../schemas/inventoryItem.md#inventoryitem-itemvendor-itemvendorprice) | related |
| [`inventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/inventoryItem.md#inventoryitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`inventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/inventoryItem.md#inventoryitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`inventoryItem-itemVendorCollection`](../schemas/inventoryItem.md#inventoryitem-itemvendorcollection) | sublist/collection |
| [`inventoryItem-itemVendorElement`](../schemas/inventoryItem.md#inventoryitem-itemvendorelement) | sublist/element |
| [`inventoryItem-locationsCollection`](../schemas/inventoryItem.md#inventoryitem-locationscollection) | sublist/collection |
| [`inventoryItem-locationsElement`](../schemas/inventoryItem.md#inventoryitem-locationselement) | sublist/element |
| [`inventoryItem-presentationItemCollection`](../schemas/inventoryItem.md#inventoryitem-presentationitemcollection) | sublist/collection |
| [`inventoryItem-presentationItemElement`](../schemas/inventoryItem.md#inventoryitem-presentationitemelement) | sublist/element |
| [`inventoryItem-price`](../schemas/inventoryItem.md#inventoryitem-price) | related |
| [`inventoryItem-priceElement`](../schemas/inventoryItem.md#inventoryitem-priceelement) | sublist/element |
| [`inventoryItem-siteCategoryCollection`](../schemas/inventoryItem.md#inventoryitem-sitecategorycollection) | sublist/collection |
| [`inventoryItem-siteCategoryElement`](../schemas/inventoryItem.md#inventoryitem-sitecategoryelement) | sublist/element |
| [`inventoryItem-translationsCollection`](../schemas/inventoryItem.md#inventoryitem-translationscollection) | sublist/collection |
| [`inventoryItem-translationsElement`](../schemas/inventoryItem.md#inventoryitem-translationselement) | sublist/element |
| [`inventoryItemCollection`](../schemas/inventoryItem.md#inventoryitemcollection) | collection page |
| [`inventoryItemSelectOptions`](../schemas/inventoryItem.md#inventoryitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`inventoryItem-accountingBookDetailCollection`](../schemas/inventoryItem.md#inventoryitem-accountingbookdetailcollection) | [`inventoryItem-accountingBookDetailElement`](../schemas/inventoryItem.md#inventoryitem-accountingbookdetailelement) |
| `binNumber` | [`inventoryItem-binNumberCollection`](../schemas/inventoryItem.md#inventoryitem-binnumbercollection) | [`inventoryItem-binNumberElement`](../schemas/inventoryItem.md#inventoryitem-binnumberelement) |
| `consignedlocations` | [`inventoryItem-consignedlocationsCollection`](../schemas/inventoryItem.md#inventoryitem-consignedlocationscollection) | [`inventoryItem-consignedlocationsElement`](../schemas/inventoryItem.md#inventoryitem-consignedlocationselement) |
| `correlatedItems` | [`inventoryItem-correlatedItemsCollection`](../schemas/inventoryItem.md#inventoryitem-correlateditemscollection) | [`inventoryItem-correlatedItemsElement`](../schemas/inventoryItem.md#inventoryitem-correlateditemselement) |
| `hierarchyVersions` | [`inventoryItem-hierarchyVersionsCollection`](../schemas/inventoryItem.md#inventoryitem-hierarchyversionscollection) | [`inventoryItem-hierarchyVersionsElement`](../schemas/inventoryItem.md#inventoryitem-hierarchyversionselement) |
| `itemVendor` | [`inventoryItem-itemVendorCollection`](../schemas/inventoryItem.md#inventoryitem-itemvendorcollection) | [`inventoryItem-itemVendorElement`](../schemas/inventoryItem.md#inventoryitem-itemvendorelement) |
| `locations` | [`inventoryItem-locationsCollection`](../schemas/inventoryItem.md#inventoryitem-locationscollection) | [`inventoryItem-locationsElement`](../schemas/inventoryItem.md#inventoryitem-locationselement) |
| `presentationItem` | [`inventoryItem-presentationItemCollection`](../schemas/inventoryItem.md#inventoryitem-presentationitemcollection) | [`inventoryItem-presentationItemElement`](../schemas/inventoryItem.md#inventoryitem-presentationitemelement) |
| `siteCategory` | [`inventoryItem-siteCategoryCollection`](../schemas/inventoryItem.md#inventoryitem-sitecategorycollection) | [`inventoryItem-siteCategoryElement`](../schemas/inventoryItem.md#inventoryitem-sitecategoryelement) |
| `translations` | [`inventoryItem-translationsCollection`](../schemas/inventoryItem.md#inventoryitem-translationscollection) | [`inventoryItem-translationsElement`](../schemas/inventoryItem.md#inventoryitem-translationselement) |

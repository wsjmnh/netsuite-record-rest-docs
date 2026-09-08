# lotNumberedInventoryItem

Browser tag `lotNumberedInventoryItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/lotNumberedInventoryItem`, instance `/lotNumberedInventoryItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/lotNumberedInventoryItem` | `operation--lotNumberedInventoryItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/lotNumberedInventoryItem` | `operation--lotNumberedInventoryItem-get` | Get list of records. |  | 200 OK → `lotNumberedInventoryItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/lotNumberedInventoryItem` | `operation--lotNumberedInventoryItem-patch` | Update records. | `lotNumberedInventoryItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/lotNumberedInventoryItem` | `operation--lotNumberedInventoryItem-post` | Insert record. | `lotNumberedInventoryItem` | 200 OK → `lotNumberedInventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/lotNumberedInventoryItem` | `operation--lotNumberedInventoryItem-put` | Insert or update records. | `lotNumberedInventoryItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/lotNumberedInventoryItem/{id}` | `operation--lotNumberedInventoryItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/lotNumberedInventoryItem/{id}` | `operation--lotNumberedInventoryItem--id--get` | Get record. |  | 200 OK → `lotNumberedInventoryItem`; 202 Accepted; default → `nsError` |
| PATCH | `/lotNumberedInventoryItem/{id}` | `operation--lotNumberedInventoryItem--id--patch` | Update record. | `lotNumberedInventoryItem` | 200 OK → `lotNumberedInventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/lotNumberedInventoryItem/{id}` | `operation--lotNumberedInventoryItem--id--put` | Insert or update record. | `lotNumberedInventoryItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--lotNumberedInventoryItem-delete` | DELETE `/lotNumberedInventoryItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem-get` | GET `/lotNumberedInventoryItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem-patch` | PATCH `/lotNumberedInventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem-post` | POST `/lotNumberedInventoryItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--lotNumberedInventoryItem-put` | PUT `/lotNumberedInventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem--id--delete` | DELETE `/lotNumberedInventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem--id--get` | GET `/lotNumberedInventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedInventoryItem--id--patch` | PATCH `/lotNumberedInventoryItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--lotNumberedInventoryItem--id--put` | PUT `/lotNumberedInventoryItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [lotNumberedInventoryItem schemas](../schemas/lotNumberedInventoryItem.md).

| Definition | Role |
| --- | --- |
| [`lotNumberedInventoryItem`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem) | record body |
| [`lotNumberedInventoryItem-accountingBookDetailCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-accountingbookdetailcollection) | sublist/collection |
| [`lotNumberedInventoryItem-accountingBookDetailElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-accountingbookdetailelement) | sublist/element |
| [`lotNumberedInventoryItem-binNumberCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-binnumbercollection) | sublist/collection |
| [`lotNumberedInventoryItem-binNumberElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-binnumberelement) | sublist/element |
| [`lotNumberedInventoryItem-consignedlocationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-consignedlocationscollection) | sublist/collection |
| [`lotNumberedInventoryItem-consignedlocationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-consignedlocationselement) | sublist/element |
| [`lotNumberedInventoryItem-correlatedItemsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-correlateditemscollection) | sublist/collection |
| [`lotNumberedInventoryItem-correlatedItemsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-correlateditemselement) | sublist/element |
| [`lotNumberedInventoryItem-hierarchyVersionsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-hierarchyversionscollection) | sublist/collection |
| [`lotNumberedInventoryItem-hierarchyVersionsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-hierarchyversionselement) | sublist/element |
| [`lotNumberedInventoryItem-itemVendor-itemVendorPrice`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendor-itemvendorprice) | related |
| [`lotNumberedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`lotNumberedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`lotNumberedInventoryItem-itemVendorCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendorcollection) | sublist/collection |
| [`lotNumberedInventoryItem-itemVendorElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendorelement) | sublist/element |
| [`lotNumberedInventoryItem-locationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-locationscollection) | sublist/collection |
| [`lotNumberedInventoryItem-locationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-locationselement) | sublist/element |
| [`lotNumberedInventoryItem-numbersCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-numberscollection) | sublist/collection |
| [`lotNumberedInventoryItem-numbersElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-numberselement) | sublist/element |
| [`lotNumberedInventoryItem-presentationItemCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-presentationitemcollection) | sublist/collection |
| [`lotNumberedInventoryItem-presentationItemElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-presentationitemelement) | sublist/element |
| [`lotNumberedInventoryItem-price`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-price) | related |
| [`lotNumberedInventoryItem-priceElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-priceelement) | sublist/element |
| [`lotNumberedInventoryItem-siteCategoryCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-sitecategorycollection) | sublist/collection |
| [`lotNumberedInventoryItem-siteCategoryElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-sitecategoryelement) | sublist/element |
| [`lotNumberedInventoryItem-translationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-translationscollection) | sublist/collection |
| [`lotNumberedInventoryItem-translationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-translationselement) | sublist/element |
| [`lotNumberedInventoryItemCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitemcollection) | collection page |
| [`lotNumberedInventoryItemSelectOptions`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`lotNumberedInventoryItem-accountingBookDetailCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-accountingbookdetailcollection) | [`lotNumberedInventoryItem-accountingBookDetailElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-accountingbookdetailelement) |
| `binNumber` | [`lotNumberedInventoryItem-binNumberCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-binnumbercollection) | [`lotNumberedInventoryItem-binNumberElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-binnumberelement) |
| `consignedlocations` | [`lotNumberedInventoryItem-consignedlocationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-consignedlocationscollection) | [`lotNumberedInventoryItem-consignedlocationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-consignedlocationselement) |
| `correlatedItems` | [`lotNumberedInventoryItem-correlatedItemsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-correlateditemscollection) | [`lotNumberedInventoryItem-correlatedItemsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-correlateditemselement) |
| `hierarchyVersions` | [`lotNumberedInventoryItem-hierarchyVersionsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-hierarchyversionscollection) | [`lotNumberedInventoryItem-hierarchyVersionsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-hierarchyversionselement) |
| `itemVendor` | [`lotNumberedInventoryItem-itemVendorCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendorcollection) | [`lotNumberedInventoryItem-itemVendorElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-itemvendorelement) |
| `locations` | [`lotNumberedInventoryItem-locationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-locationscollection) | [`lotNumberedInventoryItem-locationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-locationselement) |
| `numbers` | [`lotNumberedInventoryItem-numbersCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-numberscollection) | [`lotNumberedInventoryItem-numbersElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-numberselement) |
| `presentationItem` | [`lotNumberedInventoryItem-presentationItemCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-presentationitemcollection) | [`lotNumberedInventoryItem-presentationItemElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-presentationitemelement) |
| `siteCategory` | [`lotNumberedInventoryItem-siteCategoryCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-sitecategorycollection) | [`lotNumberedInventoryItem-siteCategoryElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-sitecategoryelement) |
| `translations` | [`lotNumberedInventoryItem-translationsCollection`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-translationscollection) | [`lotNumberedInventoryItem-translationsElement`](../schemas/lotNumberedInventoryItem.md#lotnumberedinventoryitem-translationselement) |

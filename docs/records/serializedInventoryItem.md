# serializedInventoryItem

Browser tag `serializedInventoryItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/serializedInventoryItem`, instance `/serializedInventoryItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/serializedInventoryItem` | `operation--serializedInventoryItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/serializedInventoryItem` | `operation--serializedInventoryItem-get` | Get list of records. |  | 200 OK → `serializedInventoryItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/serializedInventoryItem` | `operation--serializedInventoryItem-patch` | Update records. | `serializedInventoryItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/serializedInventoryItem` | `operation--serializedInventoryItem-post` | Insert record. | `serializedInventoryItem` | 200 OK → `serializedInventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serializedInventoryItem` | `operation--serializedInventoryItem-put` | Insert or update records. | `serializedInventoryItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/serializedInventoryItem/{id}` | `operation--serializedInventoryItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/serializedInventoryItem/{id}` | `operation--serializedInventoryItem--id--get` | Get record. |  | 200 OK → `serializedInventoryItem`; 202 Accepted; default → `nsError` |
| PATCH | `/serializedInventoryItem/{id}` | `operation--serializedInventoryItem--id--patch` | Update record. | `serializedInventoryItem` | 200 OK → `serializedInventoryItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serializedInventoryItem/{id}` | `operation--serializedInventoryItem--id--put` | Insert or update record. | `serializedInventoryItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--serializedInventoryItem-delete` | DELETE `/serializedInventoryItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem-get` | GET `/serializedInventoryItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem-patch` | PATCH `/serializedInventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem-post` | POST `/serializedInventoryItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--serializedInventoryItem-put` | PUT `/serializedInventoryItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem--id--delete` | DELETE `/serializedInventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem--id--get` | GET `/serializedInventoryItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedInventoryItem--id--patch` | PATCH `/serializedInventoryItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--serializedInventoryItem--id--put` | PUT `/serializedInventoryItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [serializedInventoryItem schemas](../schemas/serializedInventoryItem.md).

| Definition | Role |
| --- | --- |
| [`serializedInventoryItem`](../schemas/serializedInventoryItem.md#serializedinventoryitem) | record body |
| [`serializedInventoryItem-accountingBookDetailCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-accountingbookdetailcollection) | sublist/collection |
| [`serializedInventoryItem-accountingBookDetailElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-accountingbookdetailelement) | sublist/element |
| [`serializedInventoryItem-binNumberCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-binnumbercollection) | sublist/collection |
| [`serializedInventoryItem-binNumberElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-binnumberelement) | sublist/element |
| [`serializedInventoryItem-consignedlocationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-consignedlocationscollection) | sublist/collection |
| [`serializedInventoryItem-consignedlocationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-consignedlocationselement) | sublist/element |
| [`serializedInventoryItem-correlatedItemsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-correlateditemscollection) | sublist/collection |
| [`serializedInventoryItem-correlatedItemsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-correlateditemselement) | sublist/element |
| [`serializedInventoryItem-hierarchyVersionsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-hierarchyversionscollection) | sublist/collection |
| [`serializedInventoryItem-hierarchyVersionsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-hierarchyversionselement) | sublist/element |
| [`serializedInventoryItem-itemVendor-itemVendorPrice`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendor-itemvendorprice) | related |
| [`serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`serializedInventoryItem-itemVendorCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendorcollection) | sublist/collection |
| [`serializedInventoryItem-itemVendorElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendorelement) | sublist/element |
| [`serializedInventoryItem-locationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-locationscollection) | sublist/collection |
| [`serializedInventoryItem-locationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-locationselement) | sublist/element |
| [`serializedInventoryItem-numbersCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-numberscollection) | sublist/collection |
| [`serializedInventoryItem-numbersElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-numberselement) | sublist/element |
| [`serializedInventoryItem-presentationItemCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-presentationitemcollection) | sublist/collection |
| [`serializedInventoryItem-presentationItemElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-presentationitemelement) | sublist/element |
| [`serializedInventoryItem-price`](../schemas/serializedInventoryItem.md#serializedinventoryitem-price) | related |
| [`serializedInventoryItem-priceElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-priceelement) | sublist/element |
| [`serializedInventoryItem-siteCategoryCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-sitecategorycollection) | sublist/collection |
| [`serializedInventoryItem-siteCategoryElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-sitecategoryelement) | sublist/element |
| [`serializedInventoryItem-translationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-translationscollection) | sublist/collection |
| [`serializedInventoryItem-translationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-translationselement) | sublist/element |
| [`serializedInventoryItemCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitemcollection) | collection page |
| [`serializedInventoryItemSelectOptions`](../schemas/serializedInventoryItem.md#serializedinventoryitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`serializedInventoryItem-accountingBookDetailCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-accountingbookdetailcollection) | [`serializedInventoryItem-accountingBookDetailElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-accountingbookdetailelement) |
| `binNumber` | [`serializedInventoryItem-binNumberCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-binnumbercollection) | [`serializedInventoryItem-binNumberElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-binnumberelement) |
| `consignedlocations` | [`serializedInventoryItem-consignedlocationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-consignedlocationscollection) | [`serializedInventoryItem-consignedlocationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-consignedlocationselement) |
| `correlatedItems` | [`serializedInventoryItem-correlatedItemsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-correlateditemscollection) | [`serializedInventoryItem-correlatedItemsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-correlateditemselement) |
| `hierarchyVersions` | [`serializedInventoryItem-hierarchyVersionsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-hierarchyversionscollection) | [`serializedInventoryItem-hierarchyVersionsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-hierarchyversionselement) |
| `itemVendor` | [`serializedInventoryItem-itemVendorCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendorcollection) | [`serializedInventoryItem-itemVendorElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-itemvendorelement) |
| `locations` | [`serializedInventoryItem-locationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-locationscollection) | [`serializedInventoryItem-locationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-locationselement) |
| `numbers` | [`serializedInventoryItem-numbersCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-numberscollection) | [`serializedInventoryItem-numbersElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-numberselement) |
| `presentationItem` | [`serializedInventoryItem-presentationItemCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-presentationitemcollection) | [`serializedInventoryItem-presentationItemElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-presentationitemelement) |
| `siteCategory` | [`serializedInventoryItem-siteCategoryCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-sitecategorycollection) | [`serializedInventoryItem-siteCategoryElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-sitecategoryelement) |
| `translations` | [`serializedInventoryItem-translationsCollection`](../schemas/serializedInventoryItem.md#serializedinventoryitem-translationscollection) | [`serializedInventoryItem-translationsElement`](../schemas/serializedInventoryItem.md#serializedinventoryitem-translationselement) |

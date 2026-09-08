# serializedAssemblyItem

Browser tag `serializedAssemblyItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/serializedAssemblyItem`, instance `/serializedAssemblyItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/serializedAssemblyItem` | `operation--serializedAssemblyItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/serializedAssemblyItem` | `operation--serializedAssemblyItem-get` | Get list of records. |  | 200 OK → `serializedAssemblyItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/serializedAssemblyItem` | `operation--serializedAssemblyItem-patch` | Update records. | `serializedAssemblyItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/serializedAssemblyItem` | `operation--serializedAssemblyItem-post` | Insert record. | `serializedAssemblyItem` | 200 OK → `serializedAssemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serializedAssemblyItem` | `operation--serializedAssemblyItem-put` | Insert or update records. | `serializedAssemblyItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/serializedAssemblyItem/{id}` | `operation--serializedAssemblyItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/serializedAssemblyItem/{id}` | `operation--serializedAssemblyItem--id--get` | Get record. |  | 200 OK → `serializedAssemblyItem`; 202 Accepted; default → `nsError` |
| PATCH | `/serializedAssemblyItem/{id}` | `operation--serializedAssemblyItem--id--patch` | Update record. | `serializedAssemblyItem` | 200 OK → `serializedAssemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serializedAssemblyItem/{id}` | `operation--serializedAssemblyItem--id--put` | Insert or update record. | `serializedAssemblyItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--serializedAssemblyItem-delete` | DELETE `/serializedAssemblyItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem-get` | GET `/serializedAssemblyItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem-patch` | PATCH `/serializedAssemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem-post` | POST `/serializedAssemblyItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--serializedAssemblyItem-put` | PUT `/serializedAssemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem--id--delete` | DELETE `/serializedAssemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem--id--get` | GET `/serializedAssemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serializedAssemblyItem--id--patch` | PATCH `/serializedAssemblyItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--serializedAssemblyItem--id--put` | PUT `/serializedAssemblyItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [serializedAssemblyItem schemas](../schemas/serializedAssemblyItem.md).

| Definition | Role |
| --- | --- |
| [`serializedAssemblyItem`](../schemas/serializedAssemblyItem.md#serializedassemblyitem) | record body |
| [`serializedAssemblyItem-accountingBookDetailCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-accountingbookdetailcollection) | sublist/collection |
| [`serializedAssemblyItem-accountingBookDetailElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-accountingbookdetailelement) | sublist/element |
| [`serializedAssemblyItem-billOfMaterialsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-billofmaterialscollection) | sublist/collection |
| [`serializedAssemblyItem-billOfMaterialsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-billofmaterialselement) | sublist/element |
| [`serializedAssemblyItem-binNumberCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-binnumbercollection) | sublist/collection |
| [`serializedAssemblyItem-binNumberElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-binnumberelement) | sublist/element |
| [`serializedAssemblyItem-consignedlocationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-consignedlocationscollection) | sublist/collection |
| [`serializedAssemblyItem-consignedlocationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-consignedlocationselement) | sublist/element |
| [`serializedAssemblyItem-correlatedItemsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-correlateditemscollection) | sublist/collection |
| [`serializedAssemblyItem-correlatedItemsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-correlateditemselement) | sublist/element |
| [`serializedAssemblyItem-hierarchyVersionsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-hierarchyversionscollection) | sublist/collection |
| [`serializedAssemblyItem-hierarchyVersionsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-hierarchyversionselement) | sublist/element |
| [`serializedAssemblyItem-itemVendor-itemVendorPrice`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendor-itemvendorprice) | related |
| [`serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`serializedAssemblyItem-itemVendorCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendorcollection) | sublist/collection |
| [`serializedAssemblyItem-itemVendorElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendorelement) | sublist/element |
| [`serializedAssemblyItem-locationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-locationscollection) | sublist/collection |
| [`serializedAssemblyItem-locationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-locationselement) | sublist/element |
| [`serializedAssemblyItem-memberCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-membercollection) | sublist/collection |
| [`serializedAssemblyItem-memberElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-memberelement) | sublist/element |
| [`serializedAssemblyItem-numbersCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-numberscollection) | sublist/collection |
| [`serializedAssemblyItem-numbersElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-numberselement) | sublist/element |
| [`serializedAssemblyItem-presentationItemCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-presentationitemcollection) | sublist/collection |
| [`serializedAssemblyItem-presentationItemElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-presentationitemelement) | sublist/element |
| [`serializedAssemblyItem-price`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-price) | related |
| [`serializedAssemblyItem-priceElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-priceelement) | sublist/element |
| [`serializedAssemblyItem-siteCategoryCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-sitecategorycollection) | sublist/collection |
| [`serializedAssemblyItem-siteCategoryElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-sitecategoryelement) | sublist/element |
| [`serializedAssemblyItem-translationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-translationscollection) | sublist/collection |
| [`serializedAssemblyItem-translationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-translationselement) | sublist/element |
| [`serializedAssemblyItemCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitemcollection) | collection page |
| [`serializedAssemblyItemSelectOptions`](../schemas/serializedAssemblyItem.md#serializedassemblyitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`serializedAssemblyItem-accountingBookDetailCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-accountingbookdetailcollection) | [`serializedAssemblyItem-accountingBookDetailElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-accountingbookdetailelement) |
| `billOfMaterials` | [`serializedAssemblyItem-billOfMaterialsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-billofmaterialscollection) | [`serializedAssemblyItem-billOfMaterialsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-billofmaterialselement) |
| `binNumber` | [`serializedAssemblyItem-binNumberCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-binnumbercollection) | [`serializedAssemblyItem-binNumberElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-binnumberelement) |
| `consignedlocations` | [`serializedAssemblyItem-consignedlocationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-consignedlocationscollection) | [`serializedAssemblyItem-consignedlocationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-consignedlocationselement) |
| `correlatedItems` | [`serializedAssemblyItem-correlatedItemsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-correlateditemscollection) | [`serializedAssemblyItem-correlatedItemsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-correlateditemselement) |
| `hierarchyVersions` | [`serializedAssemblyItem-hierarchyVersionsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-hierarchyversionscollection) | [`serializedAssemblyItem-hierarchyVersionsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-hierarchyversionselement) |
| `itemVendor` | [`serializedAssemblyItem-itemVendorCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendorcollection) | [`serializedAssemblyItem-itemVendorElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-itemvendorelement) |
| `locations` | [`serializedAssemblyItem-locationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-locationscollection) | [`serializedAssemblyItem-locationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-locationselement) |
| `member` | [`serializedAssemblyItem-memberCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-membercollection) | [`serializedAssemblyItem-memberElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-memberelement) |
| `numbers` | [`serializedAssemblyItem-numbersCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-numberscollection) | [`serializedAssemblyItem-numbersElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-numberselement) |
| `presentationItem` | [`serializedAssemblyItem-presentationItemCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-presentationitemcollection) | [`serializedAssemblyItem-presentationItemElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-presentationitemelement) |
| `siteCategory` | [`serializedAssemblyItem-siteCategoryCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-sitecategorycollection) | [`serializedAssemblyItem-siteCategoryElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-sitecategoryelement) |
| `translations` | [`serializedAssemblyItem-translationsCollection`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-translationscollection) | [`serializedAssemblyItem-translationsElement`](../schemas/serializedAssemblyItem.md#serializedassemblyitem-translationselement) |

# lotNumberedAssemblyItem

Browser tag `lotNumberedAssemblyItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/lotNumberedAssemblyItem`, instance `/lotNumberedAssemblyItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/lotNumberedAssemblyItem` | `operation--lotNumberedAssemblyItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/lotNumberedAssemblyItem` | `operation--lotNumberedAssemblyItem-get` | Get list of records. |  | 200 OK → `lotNumberedAssemblyItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/lotNumberedAssemblyItem` | `operation--lotNumberedAssemblyItem-patch` | Update records. | `lotNumberedAssemblyItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/lotNumberedAssemblyItem` | `operation--lotNumberedAssemblyItem-post` | Insert record. | `lotNumberedAssemblyItem` | 200 OK → `lotNumberedAssemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/lotNumberedAssemblyItem` | `operation--lotNumberedAssemblyItem-put` | Insert or update records. | `lotNumberedAssemblyItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/lotNumberedAssemblyItem/{id}` | `operation--lotNumberedAssemblyItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/lotNumberedAssemblyItem/{id}` | `operation--lotNumberedAssemblyItem--id--get` | Get record. |  | 200 OK → `lotNumberedAssemblyItem`; 202 Accepted; default → `nsError` |
| PATCH | `/lotNumberedAssemblyItem/{id}` | `operation--lotNumberedAssemblyItem--id--patch` | Update record. | `lotNumberedAssemblyItem` | 200 OK → `lotNumberedAssemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/lotNumberedAssemblyItem/{id}` | `operation--lotNumberedAssemblyItem--id--put` | Insert or update record. | `lotNumberedAssemblyItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--lotNumberedAssemblyItem-delete` | DELETE `/lotNumberedAssemblyItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem-get` | GET `/lotNumberedAssemblyItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem-patch` | PATCH `/lotNumberedAssemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem-post` | POST `/lotNumberedAssemblyItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--lotNumberedAssemblyItem-put` | PUT `/lotNumberedAssemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem--id--delete` | DELETE `/lotNumberedAssemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem--id--get` | GET `/lotNumberedAssemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--lotNumberedAssemblyItem--id--patch` | PATCH `/lotNumberedAssemblyItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--lotNumberedAssemblyItem--id--put` | PUT `/lotNumberedAssemblyItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [lotNumberedAssemblyItem schemas](../schemas/lotNumberedAssemblyItem.md).

| Definition | Role |
| --- | --- |
| [`lotNumberedAssemblyItem`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem) | record body |
| [`lotNumberedAssemblyItem-accountingBookDetailCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-accountingbookdetailcollection) | sublist/collection |
| [`lotNumberedAssemblyItem-accountingBookDetailElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-accountingbookdetailelement) | sublist/element |
| [`lotNumberedAssemblyItem-billOfMaterialsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-billofmaterialscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-billOfMaterialsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-billofmaterialselement) | sublist/element |
| [`lotNumberedAssemblyItem-binNumberCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-binnumbercollection) | sublist/collection |
| [`lotNumberedAssemblyItem-binNumberElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-binnumberelement) | sublist/element |
| [`lotNumberedAssemblyItem-consignedlocationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-consignedlocationscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-consignedlocationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-consignedlocationselement) | sublist/element |
| [`lotNumberedAssemblyItem-correlatedItemsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-correlateditemscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-correlatedItemsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-correlateditemselement) | sublist/element |
| [`lotNumberedAssemblyItem-hierarchyVersionsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-hierarchyversionscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-hierarchyVersionsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-hierarchyversionselement) | sublist/element |
| [`lotNumberedAssemblyItem-itemVendor-itemVendorPrice`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendor-itemvendorprice) | related |
| [`lotNumberedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`lotNumberedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`lotNumberedAssemblyItem-itemVendorCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendorcollection) | sublist/collection |
| [`lotNumberedAssemblyItem-itemVendorElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendorelement) | sublist/element |
| [`lotNumberedAssemblyItem-locationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-locationscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-locationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-locationselement) | sublist/element |
| [`lotNumberedAssemblyItem-memberCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-membercollection) | sublist/collection |
| [`lotNumberedAssemblyItem-memberElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-memberelement) | sublist/element |
| [`lotNumberedAssemblyItem-numbersCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-numberscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-numbersElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-numberselement) | sublist/element |
| [`lotNumberedAssemblyItem-presentationItemCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-presentationitemcollection) | sublist/collection |
| [`lotNumberedAssemblyItem-presentationItemElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-presentationitemelement) | sublist/element |
| [`lotNumberedAssemblyItem-price`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-price) | related |
| [`lotNumberedAssemblyItem-priceElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-priceelement) | sublist/element |
| [`lotNumberedAssemblyItem-siteCategoryCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-sitecategorycollection) | sublist/collection |
| [`lotNumberedAssemblyItem-siteCategoryElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-sitecategoryelement) | sublist/element |
| [`lotNumberedAssemblyItem-translationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-translationscollection) | sublist/collection |
| [`lotNumberedAssemblyItem-translationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-translationselement) | sublist/element |
| [`lotNumberedAssemblyItemCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitemcollection) | collection page |
| [`lotNumberedAssemblyItemSelectOptions`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`lotNumberedAssemblyItem-accountingBookDetailCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-accountingbookdetailcollection) | [`lotNumberedAssemblyItem-accountingBookDetailElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-accountingbookdetailelement) |
| `billOfMaterials` | [`lotNumberedAssemblyItem-billOfMaterialsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-billofmaterialscollection) | [`lotNumberedAssemblyItem-billOfMaterialsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-billofmaterialselement) |
| `binNumber` | [`lotNumberedAssemblyItem-binNumberCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-binnumbercollection) | [`lotNumberedAssemblyItem-binNumberElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-binnumberelement) |
| `consignedlocations` | [`lotNumberedAssemblyItem-consignedlocationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-consignedlocationscollection) | [`lotNumberedAssemblyItem-consignedlocationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-consignedlocationselement) |
| `correlatedItems` | [`lotNumberedAssemblyItem-correlatedItemsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-correlateditemscollection) | [`lotNumberedAssemblyItem-correlatedItemsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-correlateditemselement) |
| `hierarchyVersions` | [`lotNumberedAssemblyItem-hierarchyVersionsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-hierarchyversionscollection) | [`lotNumberedAssemblyItem-hierarchyVersionsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-hierarchyversionselement) |
| `itemVendor` | [`lotNumberedAssemblyItem-itemVendorCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendorcollection) | [`lotNumberedAssemblyItem-itemVendorElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-itemvendorelement) |
| `locations` | [`lotNumberedAssemblyItem-locationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-locationscollection) | [`lotNumberedAssemblyItem-locationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-locationselement) |
| `member` | [`lotNumberedAssemblyItem-memberCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-membercollection) | [`lotNumberedAssemblyItem-memberElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-memberelement) |
| `numbers` | [`lotNumberedAssemblyItem-numbersCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-numberscollection) | [`lotNumberedAssemblyItem-numbersElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-numberselement) |
| `presentationItem` | [`lotNumberedAssemblyItem-presentationItemCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-presentationitemcollection) | [`lotNumberedAssemblyItem-presentationItemElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-presentationitemelement) |
| `siteCategory` | [`lotNumberedAssemblyItem-siteCategoryCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-sitecategorycollection) | [`lotNumberedAssemblyItem-siteCategoryElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-sitecategoryelement) |
| `translations` | [`lotNumberedAssemblyItem-translationsCollection`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-translationscollection) | [`lotNumberedAssemblyItem-translationsElement`](../schemas/lotNumberedAssemblyItem.md#lotnumberedassemblyitem-translationselement) |

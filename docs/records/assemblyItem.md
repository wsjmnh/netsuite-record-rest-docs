# assemblyItem

Browser tag `assemblyItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/assemblyItem`, instance `/assemblyItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/assemblyItem` | `operation--assemblyItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/assemblyItem` | `operation--assemblyItem-get` | Get list of records. |  | 200 OK → `assemblyItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyItem` | `operation--assemblyItem-patch` | Update records. | `assemblyItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/assemblyItem` | `operation--assemblyItem-post` | Insert record. | `assemblyItem` | 200 OK → `assemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyItem` | `operation--assemblyItem-put` | Insert or update records. | `assemblyItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/assemblyItem/{id}` | `operation--assemblyItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/assemblyItem/{id}` | `operation--assemblyItem--id--get` | Get record. |  | 200 OK → `assemblyItem`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyItem/{id}` | `operation--assemblyItem--id--patch` | Update record. | `assemblyItem` | 200 OK → `assemblyItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyItem/{id}` | `operation--assemblyItem--id--put` | Insert or update record. | `assemblyItem` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/assemblyItem/{id}/!transform/assemblyBuild` | `operation--assemblyItem--id---transform-assemblyBuild-post` | Transform to assemblyBuild. | `assemblyBuild` | 200 OK → `assemblyItem`; 202 Accepted; 204 No Content → `assemblyBuild`; default → `nsError` |
| POST | `/assemblyItem/{id}/!transform/workOrder` | `operation--assemblyItem--id---transform-workOrder-post` | Transform to workOrder. | `workOrder` | 200 OK → `assemblyItem`; 202 Accepted; 204 No Content → `workOrder`; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--assemblyItem-delete` | DELETE `/assemblyItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem-get` | GET `/assemblyItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem-patch` | PATCH `/assemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem-post` | POST `/assemblyItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--assemblyItem-put` | PUT `/assemblyItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem--id--delete` | DELETE `/assemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem--id--get` | GET `/assemblyItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyItem--id--patch` | PATCH `/assemblyItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--assemblyItem--id--put` | PUT `/assemblyItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--assemblyItem--id---transform-assemblyBuild-post` | POST `/assemblyItem/{id}/!transform/assemblyBuild` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--assemblyItem--id---transform-workOrder-post` | POST `/assemblyItem/{id}/!transform/workOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |

## Schema refs

Definitions owned by this record (property tables): [assemblyItem schemas](../schemas/assemblyItem.md).

| Definition | Role |
| --- | --- |
| [`assemblyItem`](../schemas/assemblyItem.md#assemblyitem) | record body |
| [`assemblyItem-accountingBookDetailCollection`](../schemas/assemblyItem.md#assemblyitem-accountingbookdetailcollection) | sublist/collection |
| [`assemblyItem-accountingBookDetailElement`](../schemas/assemblyItem.md#assemblyitem-accountingbookdetailelement) | sublist/element |
| [`assemblyItem-billOfMaterialsCollection`](../schemas/assemblyItem.md#assemblyitem-billofmaterialscollection) | sublist/collection |
| [`assemblyItem-billOfMaterialsElement`](../schemas/assemblyItem.md#assemblyitem-billofmaterialselement) | sublist/element |
| [`assemblyItem-binNumberCollection`](../schemas/assemblyItem.md#assemblyitem-binnumbercollection) | sublist/collection |
| [`assemblyItem-binNumberElement`](../schemas/assemblyItem.md#assemblyitem-binnumberelement) | sublist/element |
| [`assemblyItem-consignedlocationsCollection`](../schemas/assemblyItem.md#assemblyitem-consignedlocationscollection) | sublist/collection |
| [`assemblyItem-consignedlocationsElement`](../schemas/assemblyItem.md#assemblyitem-consignedlocationselement) | sublist/element |
| [`assemblyItem-correlatedItemsCollection`](../schemas/assemblyItem.md#assemblyitem-correlateditemscollection) | sublist/collection |
| [`assemblyItem-correlatedItemsElement`](../schemas/assemblyItem.md#assemblyitem-correlateditemselement) | sublist/element |
| [`assemblyItem-hierarchyVersionsCollection`](../schemas/assemblyItem.md#assemblyitem-hierarchyversionscollection) | sublist/collection |
| [`assemblyItem-hierarchyVersionsElement`](../schemas/assemblyItem.md#assemblyitem-hierarchyversionselement) | sublist/element |
| [`assemblyItem-itemVendor-itemVendorPrice`](../schemas/assemblyItem.md#assemblyitem-itemvendor-itemvendorprice) | related |
| [`assemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/assemblyItem.md#assemblyitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`assemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/assemblyItem.md#assemblyitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`assemblyItem-itemVendorCollection`](../schemas/assemblyItem.md#assemblyitem-itemvendorcollection) | sublist/collection |
| [`assemblyItem-itemVendorElement`](../schemas/assemblyItem.md#assemblyitem-itemvendorelement) | sublist/element |
| [`assemblyItem-locationsCollection`](../schemas/assemblyItem.md#assemblyitem-locationscollection) | sublist/collection |
| [`assemblyItem-locationsElement`](../schemas/assemblyItem.md#assemblyitem-locationselement) | sublist/element |
| [`assemblyItem-memberCollection`](../schemas/assemblyItem.md#assemblyitem-membercollection) | sublist/collection |
| [`assemblyItem-memberElement`](../schemas/assemblyItem.md#assemblyitem-memberelement) | sublist/element |
| [`assemblyItem-presentationItemCollection`](../schemas/assemblyItem.md#assemblyitem-presentationitemcollection) | sublist/collection |
| [`assemblyItem-presentationItemElement`](../schemas/assemblyItem.md#assemblyitem-presentationitemelement) | sublist/element |
| [`assemblyItem-price`](../schemas/assemblyItem.md#assemblyitem-price) | related |
| [`assemblyItem-priceElement`](../schemas/assemblyItem.md#assemblyitem-priceelement) | sublist/element |
| [`assemblyItem-siteCategoryCollection`](../schemas/assemblyItem.md#assemblyitem-sitecategorycollection) | sublist/collection |
| [`assemblyItem-siteCategoryElement`](../schemas/assemblyItem.md#assemblyitem-sitecategoryelement) | sublist/element |
| [`assemblyItem-translationsCollection`](../schemas/assemblyItem.md#assemblyitem-translationscollection) | sublist/collection |
| [`assemblyItem-translationsElement`](../schemas/assemblyItem.md#assemblyitem-translationselement) | sublist/element |
| [`assemblyItemCollection`](../schemas/assemblyItem.md#assemblyitemcollection) | collection page |
| [`assemblyItemSelectOptions`](../schemas/assemblyItem.md#assemblyitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`assemblyBuild`](../schemas/assemblyBuild.md#assemblybuild)
- [`nsError`](../schemas/ns.md#nserror)
- [`workOrder`](../schemas/workOrder.md#workorder)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`assemblyItem-accountingBookDetailCollection`](../schemas/assemblyItem.md#assemblyitem-accountingbookdetailcollection) | [`assemblyItem-accountingBookDetailElement`](../schemas/assemblyItem.md#assemblyitem-accountingbookdetailelement) |
| `billOfMaterials` | [`assemblyItem-billOfMaterialsCollection`](../schemas/assemblyItem.md#assemblyitem-billofmaterialscollection) | [`assemblyItem-billOfMaterialsElement`](../schemas/assemblyItem.md#assemblyitem-billofmaterialselement) |
| `binNumber` | [`assemblyItem-binNumberCollection`](../schemas/assemblyItem.md#assemblyitem-binnumbercollection) | [`assemblyItem-binNumberElement`](../schemas/assemblyItem.md#assemblyitem-binnumberelement) |
| `consignedlocations` | [`assemblyItem-consignedlocationsCollection`](../schemas/assemblyItem.md#assemblyitem-consignedlocationscollection) | [`assemblyItem-consignedlocationsElement`](../schemas/assemblyItem.md#assemblyitem-consignedlocationselement) |
| `correlatedItems` | [`assemblyItem-correlatedItemsCollection`](../schemas/assemblyItem.md#assemblyitem-correlateditemscollection) | [`assemblyItem-correlatedItemsElement`](../schemas/assemblyItem.md#assemblyitem-correlateditemselement) |
| `hierarchyVersions` | [`assemblyItem-hierarchyVersionsCollection`](../schemas/assemblyItem.md#assemblyitem-hierarchyversionscollection) | [`assemblyItem-hierarchyVersionsElement`](../schemas/assemblyItem.md#assemblyitem-hierarchyversionselement) |
| `itemVendor` | [`assemblyItem-itemVendorCollection`](../schemas/assemblyItem.md#assemblyitem-itemvendorcollection) | [`assemblyItem-itemVendorElement`](../schemas/assemblyItem.md#assemblyitem-itemvendorelement) |
| `locations` | [`assemblyItem-locationsCollection`](../schemas/assemblyItem.md#assemblyitem-locationscollection) | [`assemblyItem-locationsElement`](../schemas/assemblyItem.md#assemblyitem-locationselement) |
| `member` | [`assemblyItem-memberCollection`](../schemas/assemblyItem.md#assemblyitem-membercollection) | [`assemblyItem-memberElement`](../schemas/assemblyItem.md#assemblyitem-memberelement) |
| `presentationItem` | [`assemblyItem-presentationItemCollection`](../schemas/assemblyItem.md#assemblyitem-presentationitemcollection) | [`assemblyItem-presentationItemElement`](../schemas/assemblyItem.md#assemblyitem-presentationitemelement) |
| `siteCategory` | [`assemblyItem-siteCategoryCollection`](../schemas/assemblyItem.md#assemblyitem-sitecategorycollection) | [`assemblyItem-siteCategoryElement`](../schemas/assemblyItem.md#assemblyitem-sitecategoryelement) |
| `translations` | [`assemblyItem-translationsCollection`](../schemas/assemblyItem.md#assemblyitem-translationscollection) | [`assemblyItem-translationsElement`](../schemas/assemblyItem.md#assemblyitem-translationselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/assemblyItem/{id}/!transform/assemblyBuild` | `operation--assemblyItem--id---transform-assemblyBuild-post` | Transform to assemblyBuild. | `assemblyBuild` | `assemblyBuild` |
| POST | `/assemblyItem/{id}/!transform/workOrder` | `operation--assemblyItem--id---transform-workOrder-post` | Transform to workOrder. | `workOrder` | `workOrder` |

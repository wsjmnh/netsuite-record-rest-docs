# nonInventoryPurchaseItem

Browser tag `nonInventoryPurchaseItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/nonInventoryPurchaseItem`, instance `/nonInventoryPurchaseItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/nonInventoryPurchaseItem` | `operation--nonInventoryPurchaseItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/nonInventoryPurchaseItem` | `operation--nonInventoryPurchaseItem-get` | Get list of records. |  | 200 OK → `nonInventoryPurchaseItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventoryPurchaseItem` | `operation--nonInventoryPurchaseItem-patch` | Update records. | `nonInventoryPurchaseItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/nonInventoryPurchaseItem` | `operation--nonInventoryPurchaseItem-post` | Insert record. | `nonInventoryPurchaseItem` | 200 OK → `nonInventoryPurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventoryPurchaseItem` | `operation--nonInventoryPurchaseItem-put` | Insert or update records. | `nonInventoryPurchaseItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/nonInventoryPurchaseItem/{id}` | `operation--nonInventoryPurchaseItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/nonInventoryPurchaseItem/{id}` | `operation--nonInventoryPurchaseItem--id--get` | Get record. |  | 200 OK → `nonInventoryPurchaseItem`; 202 Accepted; default → `nsError` |
| PATCH | `/nonInventoryPurchaseItem/{id}` | `operation--nonInventoryPurchaseItem--id--patch` | Update record. | `nonInventoryPurchaseItem` | 200 OK → `nonInventoryPurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/nonInventoryPurchaseItem/{id}` | `operation--nonInventoryPurchaseItem--id--put` | Insert or update record. | `nonInventoryPurchaseItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--nonInventoryPurchaseItem-delete` | DELETE `/nonInventoryPurchaseItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem-get` | GET `/nonInventoryPurchaseItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem-patch` | PATCH `/nonInventoryPurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem-post` | POST `/nonInventoryPurchaseItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--nonInventoryPurchaseItem-put` | PUT `/nonInventoryPurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem--id--delete` | DELETE `/nonInventoryPurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem--id--get` | GET `/nonInventoryPurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--nonInventoryPurchaseItem--id--patch` | PATCH `/nonInventoryPurchaseItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--nonInventoryPurchaseItem--id--put` | PUT `/nonInventoryPurchaseItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [nonInventoryPurchaseItem schemas](../schemas/nonInventoryPurchaseItem.md).

| Definition | Role |
| --- | --- |
| [`nonInventoryPurchaseItem`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem) | record body |
| [`nonInventoryPurchaseItem-accountingBookDetailCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-accountingbookdetailcollection) | sublist/collection |
| [`nonInventoryPurchaseItem-accountingBookDetailElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-accountingbookdetailelement) | sublist/element |
| [`nonInventoryPurchaseItem-hierarchyVersionsCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-hierarchyversionscollection) | sublist/collection |
| [`nonInventoryPurchaseItem-hierarchyVersionsElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-hierarchyversionselement) | sublist/element |
| [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendor-itemvendorprice) | related |
| [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`nonInventoryPurchaseItem-itemVendorCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendorcollection) | sublist/collection |
| [`nonInventoryPurchaseItem-itemVendorElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendorelement) | sublist/element |
| [`nonInventoryPurchaseItem-translationsCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-translationscollection) | sublist/collection |
| [`nonInventoryPurchaseItem-translationsElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-translationselement) | sublist/element |
| [`nonInventoryPurchaseItemCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitemcollection) | collection page |
| [`nonInventoryPurchaseItemSelectOptions`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`nonInventoryPurchaseItem-accountingBookDetailCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-accountingbookdetailcollection) | [`nonInventoryPurchaseItem-accountingBookDetailElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-accountingbookdetailelement) |
| `hierarchyVersions` | [`nonInventoryPurchaseItem-hierarchyVersionsCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-hierarchyversionscollection) | [`nonInventoryPurchaseItem-hierarchyVersionsElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-hierarchyversionselement) |
| `itemVendor` | [`nonInventoryPurchaseItem-itemVendorCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendorcollection) | [`nonInventoryPurchaseItem-itemVendorElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-itemvendorelement) |
| `translations` | [`nonInventoryPurchaseItem-translationsCollection`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-translationscollection) | [`nonInventoryPurchaseItem-translationsElement`](../schemas/nonInventoryPurchaseItem.md#noninventorypurchaseitem-translationselement) |

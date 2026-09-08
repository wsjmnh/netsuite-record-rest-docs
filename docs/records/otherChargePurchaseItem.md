# otherChargePurchaseItem

Browser tag `otherChargePurchaseItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/otherChargePurchaseItem`, instance `/otherChargePurchaseItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/otherChargePurchaseItem` | `operation--otherChargePurchaseItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/otherChargePurchaseItem` | `operation--otherChargePurchaseItem-get` | Get list of records. |  | 200 OK → `otherChargePurchaseItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargePurchaseItem` | `operation--otherChargePurchaseItem-patch` | Update records. | `otherChargePurchaseItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/otherChargePurchaseItem` | `operation--otherChargePurchaseItem-post` | Insert record. | `otherChargePurchaseItem` | 200 OK → `otherChargePurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargePurchaseItem` | `operation--otherChargePurchaseItem-put` | Insert or update records. | `otherChargePurchaseItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/otherChargePurchaseItem/{id}` | `operation--otherChargePurchaseItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/otherChargePurchaseItem/{id}` | `operation--otherChargePurchaseItem--id--get` | Get record. |  | 200 OK → `otherChargePurchaseItem`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargePurchaseItem/{id}` | `operation--otherChargePurchaseItem--id--patch` | Update record. | `otherChargePurchaseItem` | 200 OK → `otherChargePurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargePurchaseItem/{id}` | `operation--otherChargePurchaseItem--id--put` | Insert or update record. | `otherChargePurchaseItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--otherChargePurchaseItem-delete` | DELETE `/otherChargePurchaseItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem-get` | GET `/otherChargePurchaseItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem-patch` | PATCH `/otherChargePurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem-post` | POST `/otherChargePurchaseItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--otherChargePurchaseItem-put` | PUT `/otherChargePurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem--id--delete` | DELETE `/otherChargePurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem--id--get` | GET `/otherChargePurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargePurchaseItem--id--patch` | PATCH `/otherChargePurchaseItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--otherChargePurchaseItem--id--put` | PUT `/otherChargePurchaseItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [otherChargePurchaseItem schemas](../schemas/otherChargePurchaseItem.md).

| Definition | Role |
| --- | --- |
| [`otherChargePurchaseItem`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem) | record body |
| [`otherChargePurchaseItem-accountingBookDetailCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-accountingbookdetailcollection) | sublist/collection |
| [`otherChargePurchaseItem-accountingBookDetailElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-accountingbookdetailelement) | sublist/element |
| [`otherChargePurchaseItem-hierarchyVersionsCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-hierarchyversionscollection) | sublist/collection |
| [`otherChargePurchaseItem-hierarchyVersionsElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-hierarchyversionselement) | sublist/element |
| [`otherChargePurchaseItem-itemVendor-itemVendorPrice`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendor-itemvendorprice) | related |
| [`otherChargePurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`otherChargePurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`otherChargePurchaseItem-itemVendorCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendorcollection) | sublist/collection |
| [`otherChargePurchaseItem-itemVendorElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendorelement) | sublist/element |
| [`otherChargePurchaseItem-translationsCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-translationscollection) | sublist/collection |
| [`otherChargePurchaseItem-translationsElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-translationselement) | sublist/element |
| [`otherChargePurchaseItemCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitemcollection) | collection page |
| [`otherChargePurchaseItemSelectOptions`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`otherChargePurchaseItem-accountingBookDetailCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-accountingbookdetailcollection) | [`otherChargePurchaseItem-accountingBookDetailElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-accountingbookdetailelement) |
| `hierarchyVersions` | [`otherChargePurchaseItem-hierarchyVersionsCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-hierarchyversionscollection) | [`otherChargePurchaseItem-hierarchyVersionsElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-hierarchyversionselement) |
| `itemVendor` | [`otherChargePurchaseItem-itemVendorCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendorcollection) | [`otherChargePurchaseItem-itemVendorElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-itemvendorelement) |
| `translations` | [`otherChargePurchaseItem-translationsCollection`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-translationscollection) | [`otherChargePurchaseItem-translationsElement`](../schemas/otherChargePurchaseItem.md#otherchargepurchaseitem-translationselement) |

# otherChargeResaleItem

Browser tag `otherChargeResaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/otherChargeResaleItem`, instance `/otherChargeResaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/otherChargeResaleItem` | `operation--otherChargeResaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/otherChargeResaleItem` | `operation--otherChargeResaleItem-get` | Get list of records. |  | 200 OK → `otherChargeResaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargeResaleItem` | `operation--otherChargeResaleItem-patch` | Update records. | `otherChargeResaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/otherChargeResaleItem` | `operation--otherChargeResaleItem-post` | Insert record. | `otherChargeResaleItem` | 200 OK → `otherChargeResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargeResaleItem` | `operation--otherChargeResaleItem-put` | Insert or update records. | `otherChargeResaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/otherChargeResaleItem/{id}` | `operation--otherChargeResaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/otherChargeResaleItem/{id}` | `operation--otherChargeResaleItem--id--get` | Get record. |  | 200 OK → `otherChargeResaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargeResaleItem/{id}` | `operation--otherChargeResaleItem--id--patch` | Update record. | `otherChargeResaleItem` | 200 OK → `otherChargeResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargeResaleItem/{id}` | `operation--otherChargeResaleItem--id--put` | Insert or update record. | `otherChargeResaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--otherChargeResaleItem-delete` | DELETE `/otherChargeResaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem-get` | GET `/otherChargeResaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem-patch` | PATCH `/otherChargeResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem-post` | POST `/otherChargeResaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--otherChargeResaleItem-put` | PUT `/otherChargeResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem--id--delete` | DELETE `/otherChargeResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem--id--get` | GET `/otherChargeResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeResaleItem--id--patch` | PATCH `/otherChargeResaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--otherChargeResaleItem--id--put` | PUT `/otherChargeResaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [otherChargeResaleItem schemas](../schemas/otherChargeResaleItem.md).

| Definition | Role |
| --- | --- |
| [`otherChargeResaleItem`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem) | record body |
| [`otherChargeResaleItem-accountingBookDetailCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-accountingbookdetailcollection) | sublist/collection |
| [`otherChargeResaleItem-accountingBookDetailElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-accountingbookdetailelement) | sublist/element |
| [`otherChargeResaleItem-hierarchyVersionsCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-hierarchyversionscollection) | sublist/collection |
| [`otherChargeResaleItem-hierarchyVersionsElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-hierarchyversionselement) | sublist/element |
| [`otherChargeResaleItem-itemVendor-itemVendorPrice`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendor-itemvendorprice) | related |
| [`otherChargeResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`otherChargeResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`otherChargeResaleItem-itemVendorCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendorcollection) | sublist/collection |
| [`otherChargeResaleItem-itemVendorElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendorelement) | sublist/element |
| [`otherChargeResaleItem-price`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-price) | related |
| [`otherChargeResaleItem-priceElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-priceelement) | sublist/element |
| [`otherChargeResaleItem-translationsCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-translationscollection) | sublist/collection |
| [`otherChargeResaleItem-translationsElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-translationselement) | sublist/element |
| [`otherChargeResaleItemCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitemcollection) | collection page |
| [`otherChargeResaleItemSelectOptions`](../schemas/otherChargeResaleItem.md#otherchargeresaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`otherChargeResaleItem-accountingBookDetailCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-accountingbookdetailcollection) | [`otherChargeResaleItem-accountingBookDetailElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-accountingbookdetailelement) |
| `hierarchyVersions` | [`otherChargeResaleItem-hierarchyVersionsCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-hierarchyversionscollection) | [`otherChargeResaleItem-hierarchyVersionsElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-hierarchyversionselement) |
| `itemVendor` | [`otherChargeResaleItem-itemVendorCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendorcollection) | [`otherChargeResaleItem-itemVendorElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-itemvendorelement) |
| `translations` | [`otherChargeResaleItem-translationsCollection`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-translationscollection) | [`otherChargeResaleItem-translationsElement`](../schemas/otherChargeResaleItem.md#otherchargeresaleitem-translationselement) |

# servicePurchaseItem

Browser tag `servicePurchaseItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/servicePurchaseItem`, instance `/servicePurchaseItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/servicePurchaseItem` | `operation--servicePurchaseItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/servicePurchaseItem` | `operation--servicePurchaseItem-get` | Get list of records. |  | 200 OK → `servicePurchaseItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/servicePurchaseItem` | `operation--servicePurchaseItem-patch` | Update records. | `servicePurchaseItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/servicePurchaseItem` | `operation--servicePurchaseItem-post` | Insert record. | `servicePurchaseItem` | 200 OK → `servicePurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/servicePurchaseItem` | `operation--servicePurchaseItem-put` | Insert or update records. | `servicePurchaseItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/servicePurchaseItem/{id}` | `operation--servicePurchaseItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/servicePurchaseItem/{id}` | `operation--servicePurchaseItem--id--get` | Get record. |  | 200 OK → `servicePurchaseItem`; 202 Accepted; default → `nsError` |
| PATCH | `/servicePurchaseItem/{id}` | `operation--servicePurchaseItem--id--patch` | Update record. | `servicePurchaseItem` | 200 OK → `servicePurchaseItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/servicePurchaseItem/{id}` | `operation--servicePurchaseItem--id--put` | Insert or update record. | `servicePurchaseItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--servicePurchaseItem-delete` | DELETE `/servicePurchaseItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem-get` | GET `/servicePurchaseItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem-patch` | PATCH `/servicePurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem-post` | POST `/servicePurchaseItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--servicePurchaseItem-put` | PUT `/servicePurchaseItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem--id--delete` | DELETE `/servicePurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem--id--get` | GET `/servicePurchaseItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--servicePurchaseItem--id--patch` | PATCH `/servicePurchaseItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--servicePurchaseItem--id--put` | PUT `/servicePurchaseItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [servicePurchaseItem schemas](../schemas/servicePurchaseItem.md).

| Definition | Role |
| --- | --- |
| [`servicePurchaseItem`](../schemas/servicePurchaseItem.md#servicepurchaseitem) | record body |
| [`servicePurchaseItem-accountingBookDetailCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-accountingbookdetailcollection) | sublist/collection |
| [`servicePurchaseItem-accountingBookDetailElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-accountingbookdetailelement) | sublist/element |
| [`servicePurchaseItem-hierarchyVersionsCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-hierarchyversionscollection) | sublist/collection |
| [`servicePurchaseItem-hierarchyVersionsElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-hierarchyversionselement) | sublist/element |
| [`servicePurchaseItem-itemVendor-itemVendorPrice`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendor-itemvendorprice) | related |
| [`servicePurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`servicePurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`servicePurchaseItem-itemVendorCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendorcollection) | sublist/collection |
| [`servicePurchaseItem-itemVendorElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendorelement) | sublist/element |
| [`servicePurchaseItem-translationsCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-translationscollection) | sublist/collection |
| [`servicePurchaseItem-translationsElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-translationselement) | sublist/element |
| [`servicePurchaseItemCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitemcollection) | collection page |
| [`servicePurchaseItemSelectOptions`](../schemas/servicePurchaseItem.md#servicepurchaseitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`servicePurchaseItem-accountingBookDetailCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-accountingbookdetailcollection) | [`servicePurchaseItem-accountingBookDetailElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-accountingbookdetailelement) |
| `hierarchyVersions` | [`servicePurchaseItem-hierarchyVersionsCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-hierarchyversionscollection) | [`servicePurchaseItem-hierarchyVersionsElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-hierarchyversionselement) |
| `itemVendor` | [`servicePurchaseItem-itemVendorCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendorcollection) | [`servicePurchaseItem-itemVendorElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-itemvendorelement) |
| `translations` | [`servicePurchaseItem-translationsCollection`](../schemas/servicePurchaseItem.md#servicepurchaseitem-translationscollection) | [`servicePurchaseItem-translationsElement`](../schemas/servicePurchaseItem.md#servicepurchaseitem-translationselement) |

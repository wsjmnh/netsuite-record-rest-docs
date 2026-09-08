# otherChargeSaleItem

Browser tag `otherChargeSaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/otherChargeSaleItem`, instance `/otherChargeSaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/otherChargeSaleItem` | `operation--otherChargeSaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/otherChargeSaleItem` | `operation--otherChargeSaleItem-get` | Get list of records. |  | 200 OK → `otherChargeSaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargeSaleItem` | `operation--otherChargeSaleItem-patch` | Update records. | `otherChargeSaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/otherChargeSaleItem` | `operation--otherChargeSaleItem-post` | Insert record. | `otherChargeSaleItem` | 200 OK → `otherChargeSaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargeSaleItem` | `operation--otherChargeSaleItem-put` | Insert or update records. | `otherChargeSaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/otherChargeSaleItem/{id}` | `operation--otherChargeSaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/otherChargeSaleItem/{id}` | `operation--otherChargeSaleItem--id--get` | Get record. |  | 200 OK → `otherChargeSaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/otherChargeSaleItem/{id}` | `operation--otherChargeSaleItem--id--patch` | Update record. | `otherChargeSaleItem` | 200 OK → `otherChargeSaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherChargeSaleItem/{id}` | `operation--otherChargeSaleItem--id--put` | Insert or update record. | `otherChargeSaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--otherChargeSaleItem-delete` | DELETE `/otherChargeSaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem-get` | GET `/otherChargeSaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem-patch` | PATCH `/otherChargeSaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem-post` | POST `/otherChargeSaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--otherChargeSaleItem-put` | PUT `/otherChargeSaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem--id--delete` | DELETE `/otherChargeSaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem--id--get` | GET `/otherChargeSaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherChargeSaleItem--id--patch` | PATCH `/otherChargeSaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--otherChargeSaleItem--id--put` | PUT `/otherChargeSaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [otherChargeSaleItem schemas](../schemas/otherChargeSaleItem.md).

| Definition | Role |
| --- | --- |
| [`otherChargeSaleItem`](../schemas/otherChargeSaleItem.md#otherchargesaleitem) | record body |
| [`otherChargeSaleItem-accountingBookDetailCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-accountingbookdetailcollection) | sublist/collection |
| [`otherChargeSaleItem-accountingBookDetailElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-accountingbookdetailelement) | sublist/element |
| [`otherChargeSaleItem-hierarchyVersionsCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-hierarchyversionscollection) | sublist/collection |
| [`otherChargeSaleItem-hierarchyVersionsElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-hierarchyversionselement) | sublist/element |
| [`otherChargeSaleItem-price`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-price) | related |
| [`otherChargeSaleItem-priceElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-priceelement) | sublist/element |
| [`otherChargeSaleItem-translationsCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-translationscollection) | sublist/collection |
| [`otherChargeSaleItem-translationsElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-translationselement) | sublist/element |
| [`otherChargeSaleItemCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitemcollection) | collection page |
| [`otherChargeSaleItemSelectOptions`](../schemas/otherChargeSaleItem.md#otherchargesaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`otherChargeSaleItem-accountingBookDetailCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-accountingbookdetailcollection) | [`otherChargeSaleItem-accountingBookDetailElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-accountingbookdetailelement) |
| `hierarchyVersions` | [`otherChargeSaleItem-hierarchyVersionsCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-hierarchyversionscollection) | [`otherChargeSaleItem-hierarchyVersionsElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-hierarchyversionselement) |
| `translations` | [`otherChargeSaleItem-translationsCollection`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-translationscollection) | [`otherChargeSaleItem-translationsElement`](../schemas/otherChargeSaleItem.md#otherchargesaleitem-translationselement) |

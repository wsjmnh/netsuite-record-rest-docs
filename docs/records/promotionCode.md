# promotionCode

Browser tag `promotionCode` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/promotionCode`, instance `/promotionCode/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/promotionCode` | `operation--promotionCode-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/promotionCode` | `operation--promotionCode-get` | Get list of records. |  | 200 OK → `promotionCodeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/promotionCode` | `operation--promotionCode-patch` | Update records. | `promotionCodeCollection` | 202 Accepted; default → `nsError` |
| POST | `/promotionCode` | `operation--promotionCode-post` | Insert record. | `promotionCode` | 200 OK → `promotionCode`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/promotionCode` | `operation--promotionCode-put` | Insert or update records. | `promotionCodeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/promotionCode/{id}` | `operation--promotionCode--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/promotionCode/{id}` | `operation--promotionCode--id--get` | Get record. |  | 200 OK → `promotionCode`; 202 Accepted; default → `nsError` |
| PATCH | `/promotionCode/{id}` | `operation--promotionCode--id--patch` | Update record. | `promotionCode` | 200 OK → `promotionCode`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/promotionCode/{id}` | `operation--promotionCode--id--put` | Insert or update record. | `promotionCode` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--promotionCode-delete` | DELETE `/promotionCode` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode-get` | GET `/promotionCode` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode-patch` | PATCH `/promotionCode` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode-post` | POST `/promotionCode` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--promotionCode-put` | PUT `/promotionCode` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode--id--delete` | DELETE `/promotionCode/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode--id--get` | GET `/promotionCode/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--promotionCode--id--patch` | PATCH `/promotionCode/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--promotionCode--id--put` | PUT `/promotionCode/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [promotionCode schemas](../schemas/promotionCode.md).

| Definition | Role |
| --- | --- |
| [`promotionCode`](../schemas/promotionCode.md#promotioncode) | record body |
| [`promotionCode-currencyCollection`](../schemas/promotionCode.md#promotioncode-currencycollection) | sublist/collection |
| [`promotionCode-currencyElement`](../schemas/promotionCode.md#promotioncode-currencyelement) | sublist/element |
| [`promotionCode-discountedItemsCollection`](../schemas/promotionCode.md#promotioncode-discounteditemscollection) | sublist/collection |
| [`promotionCode-discountedItemsElement`](../schemas/promotionCode.md#promotioncode-discounteditemselement) | sublist/element |
| [`promotionCode-itemsCollection`](../schemas/promotionCode.md#promotioncode-itemscollection) | sublist/collection |
| [`promotionCode-itemsElement`](../schemas/promotionCode.md#promotioncode-itemselement) | sublist/element |
| [`promotionCode-partnersCollection`](../schemas/promotionCode.md#promotioncode-partnerscollection) | sublist/collection |
| [`promotionCode-partnersElement`](../schemas/promotionCode.md#promotioncode-partnerselement) | sublist/element |
| [`promotionCodeCollection`](../schemas/promotionCode.md#promotioncodecollection) | collection page |
| [`promotionCodeSelectOptions`](../schemas/promotionCode.md#promotioncodeselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `currency` | [`promotionCode-currencyCollection`](../schemas/promotionCode.md#promotioncode-currencycollection) | [`promotionCode-currencyElement`](../schemas/promotionCode.md#promotioncode-currencyelement) |
| `discountedItems` | [`promotionCode-discountedItemsCollection`](../schemas/promotionCode.md#promotioncode-discounteditemscollection) | [`promotionCode-discountedItemsElement`](../schemas/promotionCode.md#promotioncode-discounteditemselement) |
| `items` | [`promotionCode-itemsCollection`](../schemas/promotionCode.md#promotioncode-itemscollection) | [`promotionCode-itemsElement`](../schemas/promotionCode.md#promotioncode-itemselement) |
| `partners` | [`promotionCode-partnersCollection`](../schemas/promotionCode.md#promotioncode-partnerscollection) | [`promotionCode-partnersElement`](../schemas/promotionCode.md#promotioncode-partnerselement) |

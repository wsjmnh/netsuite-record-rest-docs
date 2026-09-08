# purchaseContract

Browser tag `purchaseContract` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/purchaseContract`, instance `/purchaseContract/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/purchaseContract` | `operation--purchaseContract-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/purchaseContract` | `operation--purchaseContract-get` | Get list of records. |  | 200 OK → `purchaseContractCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseContract` | `operation--purchaseContract-patch` | Update records. | `purchaseContractCollection` | 202 Accepted; default → `nsError` |
| POST | `/purchaseContract` | `operation--purchaseContract-post` | Insert record. | `purchaseContract` | 200 OK → `purchaseContract`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseContract` | `operation--purchaseContract-put` | Insert or update records. | `purchaseContractCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/purchaseContract/{id}` | `operation--purchaseContract--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/purchaseContract/{id}` | `operation--purchaseContract--id--get` | Get record. |  | 200 OK → `purchaseContract`; 202 Accepted; default → `nsError` |
| PATCH | `/purchaseContract/{id}` | `operation--purchaseContract--id--patch` | Update record. | `purchaseContract` | 200 OK → `purchaseContract`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/purchaseContract/{id}` | `operation--purchaseContract--id--put` | Insert or update record. | `purchaseContract` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--purchaseContract-delete` | DELETE `/purchaseContract` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract-get` | GET `/purchaseContract` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract-patch` | PATCH `/purchaseContract` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract-post` | POST `/purchaseContract` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--purchaseContract-put` | PUT `/purchaseContract` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract--id--delete` | DELETE `/purchaseContract/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract--id--get` | GET `/purchaseContract/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--purchaseContract--id--patch` | PATCH `/purchaseContract/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--purchaseContract--id--put` | PUT `/purchaseContract/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [purchaseContract schemas](../schemas/purchaseContract.md).

| Definition | Role |
| --- | --- |
| [`purchaseContract`](../schemas/purchaseContract.md#purchasecontract) | record body |
| [`purchaseContract-accountingBookDetailCollection`](../schemas/purchaseContract.md#purchasecontract-accountingbookdetailcollection) | sublist/collection |
| [`purchaseContract-accountingBookDetailElement`](../schemas/purchaseContract.md#purchasecontract-accountingbookdetailelement) | sublist/element |
| [`purchaseContract-discountCollection`](../schemas/purchaseContract.md#purchasecontract-discountcollection) | sublist/collection |
| [`purchaseContract-discountElement`](../schemas/purchaseContract.md#purchasecontract-discountelement) | sublist/element |
| [`purchaseContract-item-itemPricing`](../schemas/purchaseContract.md#purchasecontract-item-itempricing) | related |
| [`purchaseContract-item-itemPricing-discountCollection`](../schemas/purchaseContract.md#purchasecontract-item-itempricing-discountcollection) | sublist/collection |
| [`purchaseContract-item-itemPricing-discountElement`](../schemas/purchaseContract.md#purchasecontract-item-itempricing-discountelement) | sublist/element |
| [`purchaseContract-itemCollection`](../schemas/purchaseContract.md#purchasecontract-itemcollection) | sublist/collection |
| [`purchaseContract-itemElement`](../schemas/purchaseContract.md#purchasecontract-itemelement) | sublist/element |
| [`purchaseContractCollection`](../schemas/purchaseContract.md#purchasecontractcollection) | collection page |
| [`purchaseContractSelectOptions`](../schemas/purchaseContract.md#purchasecontractselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`purchaseContract-accountingBookDetailCollection`](../schemas/purchaseContract.md#purchasecontract-accountingbookdetailcollection) | [`purchaseContract-accountingBookDetailElement`](../schemas/purchaseContract.md#purchasecontract-accountingbookdetailelement) |
| `discount` | [`purchaseContract-discountCollection`](../schemas/purchaseContract.md#purchasecontract-discountcollection) | [`purchaseContract-discountElement`](../schemas/purchaseContract.md#purchasecontract-discountelement) |
| `item` | [`purchaseContract-itemCollection`](../schemas/purchaseContract.md#purchasecontract-itemcollection) | [`purchaseContract-itemElement`](../schemas/purchaseContract.md#purchasecontract-itemelement) |

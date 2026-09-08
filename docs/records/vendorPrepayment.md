# vendorPrepayment

Browser tag `vendorPrepayment` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendorPrepayment`, instance `/vendorPrepayment/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendorPrepayment` | `operation--vendorPrepayment-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendorPrepayment` | `operation--vendorPrepayment-get` | Get list of records. |  | 200 OK → `vendorPrepaymentCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorPrepayment` | `operation--vendorPrepayment-patch` | Update records. | `vendorPrepaymentCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendorPrepayment` | `operation--vendorPrepayment-post` | Insert record. | `vendorPrepayment` | 200 OK → `vendorPrepayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorPrepayment` | `operation--vendorPrepayment-put` | Insert or update records. | `vendorPrepaymentCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendorPrepayment/{id}` | `operation--vendorPrepayment--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendorPrepayment/{id}` | `operation--vendorPrepayment--id--get` | Get record. |  | 200 OK → `vendorPrepayment`; 202 Accepted; default → `nsError` |
| PATCH | `/vendorPrepayment/{id}` | `operation--vendorPrepayment--id--patch` | Update record. | `vendorPrepayment` | 200 OK → `vendorPrepayment`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendorPrepayment/{id}` | `operation--vendorPrepayment--id--put` | Insert or update record. | `vendorPrepayment` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendorPrepayment/{id}/!transform/vendorPrepaymentApplication` | `operation--vendorPrepayment--id---transform-vendorPrepaymentApplication-post` | Transform to vendorPrepaymentApplication. | `vendorPrepaymentApplication` | 200 OK → `vendorPrepayment`; 202 Accepted; 204 No Content → `vendorPrepaymentApplication`; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendorPrepayment-delete` | DELETE `/vendorPrepayment` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment-get` | GET `/vendorPrepayment` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment-patch` | PATCH `/vendorPrepayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment-post` | POST `/vendorPrepayment` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendorPrepayment-put` | PUT `/vendorPrepayment` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment--id--delete` | DELETE `/vendorPrepayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment--id--get` | GET `/vendorPrepayment/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendorPrepayment--id--patch` | PATCH `/vendorPrepayment/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorPrepayment--id--put` | PUT `/vendorPrepayment/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendorPrepayment--id---transform-vendorPrepaymentApplication-post` | POST `/vendorPrepayment/{id}/!transform/vendorPrepaymentApplication` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |

## Schema refs

Definitions owned by this record (property tables): [vendorPrepayment schemas](../schemas/vendorPrepayment.md).

| Definition | Role |
| --- | --- |
| [`vendorPrepayment`](../schemas/vendorPrepayment.md#vendorprepayment) | record body |
| [`vendorPrepayment-accountingBookDetailCollection`](../schemas/vendorPrepayment.md#vendorprepayment-accountingbookdetailcollection) | sublist/collection |
| [`vendorPrepayment-accountingBookDetailElement`](../schemas/vendorPrepayment.md#vendorprepayment-accountingbookdetailelement) | sublist/element |
| [`vendorPrepayment-billCollection`](../schemas/vendorPrepayment.md#vendorprepayment-billcollection) | sublist/collection |
| [`vendorPrepayment-billElement`](../schemas/vendorPrepayment.md#vendorprepayment-billelement) | sublist/element |
| [`vendorPrepayment-payeeAddress`](../schemas/vendorPrepayment.md#vendorprepayment-payeeaddress) | related |
| [`vendorPrepaymentCollection`](../schemas/vendorPrepayment.md#vendorprepaymentcollection) | collection page |
| [`vendorPrepaymentSelectOptions`](../schemas/vendorPrepayment.md#vendorprepaymentselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)
- [`vendorPrepaymentApplication`](../schemas/vendorPrepaymentApplication.md#vendorprepaymentapplication)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`vendorPrepayment-accountingBookDetailCollection`](../schemas/vendorPrepayment.md#vendorprepayment-accountingbookdetailcollection) | [`vendorPrepayment-accountingBookDetailElement`](../schemas/vendorPrepayment.md#vendorprepayment-accountingbookdetailelement) |
| `bill` | [`vendorPrepayment-billCollection`](../schemas/vendorPrepayment.md#vendorprepayment-billcollection) | [`vendorPrepayment-billElement`](../schemas/vendorPrepayment.md#vendorprepayment-billelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/vendorPrepayment/{id}/!transform/vendorPrepaymentApplication` | `operation--vendorPrepayment--id---transform-vendorPrepaymentApplication-post` | Transform to vendorPrepaymentApplication. | `vendorPrepaymentApplication` | `vendorPrepaymentApplication` |

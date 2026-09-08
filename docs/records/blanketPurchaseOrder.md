# blanketPurchaseOrder

Browser tag `blanketPurchaseOrder` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/blanketPurchaseOrder`, instance `/blanketPurchaseOrder/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/blanketPurchaseOrder` | `operation--blanketPurchaseOrder-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/blanketPurchaseOrder` | `operation--blanketPurchaseOrder-get` | Get list of records. |  | 200 OK → `blanketPurchaseOrderCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/blanketPurchaseOrder` | `operation--blanketPurchaseOrder-patch` | Update records. | `blanketPurchaseOrderCollection` | 202 Accepted; default → `nsError` |
| POST | `/blanketPurchaseOrder` | `operation--blanketPurchaseOrder-post` | Insert record. | `blanketPurchaseOrder` | 200 OK → `blanketPurchaseOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/blanketPurchaseOrder` | `operation--blanketPurchaseOrder-put` | Insert or update records. | `blanketPurchaseOrderCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/blanketPurchaseOrder/{id}` | `operation--blanketPurchaseOrder--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/blanketPurchaseOrder/{id}` | `operation--blanketPurchaseOrder--id--get` | Get record. |  | 200 OK → `blanketPurchaseOrder`; 202 Accepted; default → `nsError` |
| PATCH | `/blanketPurchaseOrder/{id}` | `operation--blanketPurchaseOrder--id--patch` | Update record. | `blanketPurchaseOrder` | 200 OK → `blanketPurchaseOrder`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/blanketPurchaseOrder/{id}` | `operation--blanketPurchaseOrder--id--put` | Insert or update record. | `blanketPurchaseOrder` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--blanketPurchaseOrder-delete` | DELETE `/blanketPurchaseOrder` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder-get` | GET `/blanketPurchaseOrder` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder-patch` | PATCH `/blanketPurchaseOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder-post` | POST `/blanketPurchaseOrder` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--blanketPurchaseOrder-put` | PUT `/blanketPurchaseOrder` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder--id--delete` | DELETE `/blanketPurchaseOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder--id--get` | GET `/blanketPurchaseOrder/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--blanketPurchaseOrder--id--patch` | PATCH `/blanketPurchaseOrder/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--blanketPurchaseOrder--id--put` | PUT `/blanketPurchaseOrder/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [blanketPurchaseOrder schemas](../schemas/blanketPurchaseOrder.md).

| Definition | Role |
| --- | --- |
| [`blanketPurchaseOrder`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder) | record body |
| [`blanketPurchaseOrder-accountingBookDetailCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-accountingbookdetailcollection) | sublist/collection |
| [`blanketPurchaseOrder-accountingBookDetailElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-accountingbookdetailelement) | sublist/element |
| [`blanketPurchaseOrder-expense-orderSchedule`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expense-orderschedule) | related |
| [`blanketPurchaseOrder-expense-orderSchedule-scheduleCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expense-orderschedule-schedulecollection) | sublist/collection |
| [`blanketPurchaseOrder-expense-orderSchedule-scheduleElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expense-orderschedule-scheduleelement) | sublist/element |
| [`blanketPurchaseOrder-expenseCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expensecollection) | sublist/collection |
| [`blanketPurchaseOrder-expenseElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expenseelement) | sublist/element |
| [`blanketPurchaseOrder-item-orderSchedule`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-item-orderschedule) | related |
| [`blanketPurchaseOrder-item-orderSchedule-scheduleCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-item-orderschedule-schedulecollection) | sublist/collection |
| [`blanketPurchaseOrder-item-orderSchedule-scheduleElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-item-orderschedule-scheduleelement) | sublist/element |
| [`blanketPurchaseOrder-itemCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-itemcollection) | sublist/collection |
| [`blanketPurchaseOrder-itemElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-itemelement) | sublist/element |
| [`blanketPurchaseOrderCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseordercollection) | collection page |
| [`blanketPurchaseOrderSelectOptions`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorderselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`blanketPurchaseOrder-accountingBookDetailCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-accountingbookdetailcollection) | [`blanketPurchaseOrder-accountingBookDetailElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-accountingbookdetailelement) |
| `expense` | [`blanketPurchaseOrder-expenseCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expensecollection) | [`blanketPurchaseOrder-expenseElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-expenseelement) |
| `item` | [`blanketPurchaseOrder-itemCollection`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-itemcollection) | [`blanketPurchaseOrder-itemElement`](../schemas/blanketPurchaseOrder.md#blanketpurchaseorder-itemelement) |

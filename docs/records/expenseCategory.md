# expenseCategory

Browser tag `expenseCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/expenseCategory`, instance `/expenseCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/expenseCategory` | `operation--expenseCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/expenseCategory` | `operation--expenseCategory-get` | Get list of records. |  | 200 OK → `expenseCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/expenseCategory` | `operation--expenseCategory-patch` | Update records. | `expenseCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/expenseCategory` | `operation--expenseCategory-post` | Insert record. | `expenseCategory` | 200 OK → `expenseCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/expenseCategory` | `operation--expenseCategory-put` | Insert or update records. | `expenseCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/expenseCategory/{id}` | `operation--expenseCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/expenseCategory/{id}` | `operation--expenseCategory--id--get` | Get record. |  | 200 OK → `expenseCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/expenseCategory/{id}` | `operation--expenseCategory--id--patch` | Update record. | `expenseCategory` | 200 OK → `expenseCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/expenseCategory/{id}` | `operation--expenseCategory--id--put` | Insert or update record. | `expenseCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--expenseCategory-delete` | DELETE `/expenseCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory-get` | GET `/expenseCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory-patch` | PATCH `/expenseCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory-post` | POST `/expenseCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--expenseCategory-put` | PUT `/expenseCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory--id--delete` | DELETE `/expenseCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory--id--get` | GET `/expenseCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--expenseCategory--id--patch` | PATCH `/expenseCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--expenseCategory--id--put` | PUT `/expenseCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [expenseCategory schemas](../schemas/expenseCategory.md).

| Definition | Role |
| --- | --- |
| [`expenseCategory`](../schemas/expenseCategory.md#expensecategory) | record body |
| [`expenseCategory-ratesCollection`](../schemas/expenseCategory.md#expensecategory-ratescollection) | sublist/collection |
| [`expenseCategory-ratesElement`](../schemas/expenseCategory.md#expensecategory-rateselement) | sublist/element |
| [`expenseCategory-translationsCollection`](../schemas/expenseCategory.md#expensecategory-translationscollection) | sublist/collection |
| [`expenseCategory-translationsElement`](../schemas/expenseCategory.md#expensecategory-translationselement) | sublist/element |
| [`expenseCategoryCollection`](../schemas/expenseCategory.md#expensecategorycollection) | collection page |
| [`expenseCategorySelectOptions`](../schemas/expenseCategory.md#expensecategoryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `rates` | [`expenseCategory-ratesCollection`](../schemas/expenseCategory.md#expensecategory-ratescollection) | [`expenseCategory-ratesElement`](../schemas/expenseCategory.md#expensecategory-rateselement) |
| `translations` | [`expenseCategory-translationsCollection`](../schemas/expenseCategory.md#expensecategory-translationscollection) | [`expenseCategory-translationsElement`](../schemas/expenseCategory.md#expensecategory-translationselement) |

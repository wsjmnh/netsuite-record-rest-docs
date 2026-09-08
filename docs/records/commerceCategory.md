# commerceCategory

Browser tag `commerceCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/commerceCategory`, instance `/commerceCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/commerceCategory` | `operation--commerceCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/commerceCategory` | `operation--commerceCategory-get` | Get list of records. |  | 200 OK → `commerceCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/commerceCategory` | `operation--commerceCategory-patch` | Update records. | `commerceCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/commerceCategory` | `operation--commerceCategory-post` | Insert record. | `commerceCategory` | 200 OK → `commerceCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/commerceCategory` | `operation--commerceCategory-put` | Insert or update records. | `commerceCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/commerceCategory/{id}` | `operation--commerceCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/commerceCategory/{id}` | `operation--commerceCategory--id--get` | Get record. |  | 200 OK → `commerceCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/commerceCategory/{id}` | `operation--commerceCategory--id--patch` | Update record. | `commerceCategory` | 200 OK → `commerceCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/commerceCategory/{id}` | `operation--commerceCategory--id--put` | Insert or update record. | `commerceCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--commerceCategory-delete` | DELETE `/commerceCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory-get` | GET `/commerceCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory-patch` | PATCH `/commerceCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory-post` | POST `/commerceCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--commerceCategory-put` | PUT `/commerceCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory--id--delete` | DELETE `/commerceCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory--id--get` | GET `/commerceCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--commerceCategory--id--patch` | PATCH `/commerceCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--commerceCategory--id--put` | PUT `/commerceCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [commerceCategory schemas](../schemas/commerceCategory.md).

| Definition | Role |
| --- | --- |
| [`commerceCategory`](../schemas/commerceCategory.md#commercecategory) | record body |
| [`commerceCategory-customerSegmentsCollection`](../schemas/commerceCategory.md#commercecategory-customersegmentscollection) | sublist/collection |
| [`commerceCategory-customerSegmentsElement`](../schemas/commerceCategory.md#commercecategory-customersegmentselement) | sublist/element |
| [`commerceCategory-itemsCollection`](../schemas/commerceCategory.md#commercecategory-itemscollection) | sublist/collection |
| [`commerceCategory-itemsElement`](../schemas/commerceCategory.md#commercecategory-itemselement) | sublist/element |
| [`commerceCategory-subcategoriesCollection`](../schemas/commerceCategory.md#commercecategory-subcategoriescollection) | sublist/collection |
| [`commerceCategory-subcategoriesElement`](../schemas/commerceCategory.md#commercecategory-subcategorieselement) | sublist/element |
| [`commerceCategory-tagsCollection`](../schemas/commerceCategory.md#commercecategory-tagscollection) | sublist/collection |
| [`commerceCategory-tagsElement`](../schemas/commerceCategory.md#commercecategory-tagselement) | sublist/element |
| [`commerceCategory-translationsCollection`](../schemas/commerceCategory.md#commercecategory-translationscollection) | sublist/collection |
| [`commerceCategory-translationsElement`](../schemas/commerceCategory.md#commercecategory-translationselement) | sublist/element |
| [`commerceCategory-urlsCollection`](../schemas/commerceCategory.md#commercecategory-urlscollection) | sublist/collection |
| [`commerceCategory-urlsElement`](../schemas/commerceCategory.md#commercecategory-urlselement) | sublist/element |
| [`commerceCategoryCollection`](../schemas/commerceCategory.md#commercecategorycollection) | collection page |
| [`commerceCategorySelectOptions`](../schemas/commerceCategory.md#commercecategoryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `tags` | [`commerceCategory-tagsCollection`](../schemas/commerceCategory.md#commercecategory-tagscollection) | [`commerceCategory-tagsElement`](../schemas/commerceCategory.md#commercecategory-tagselement) |
| `customerSegments` | [`commerceCategory-customerSegmentsCollection`](../schemas/commerceCategory.md#commercecategory-customersegmentscollection) | [`commerceCategory-customerSegmentsElement`](../schemas/commerceCategory.md#commercecategory-customersegmentselement) |
| `items` | [`commerceCategory-itemsCollection`](../schemas/commerceCategory.md#commercecategory-itemscollection) | [`commerceCategory-itemsElement`](../schemas/commerceCategory.md#commercecategory-itemselement) |
| `subcategories` | [`commerceCategory-subcategoriesCollection`](../schemas/commerceCategory.md#commercecategory-subcategoriescollection) | [`commerceCategory-subcategoriesElement`](../schemas/commerceCategory.md#commercecategory-subcategorieselement) |
| `translations` | [`commerceCategory-translationsCollection`](../schemas/commerceCategory.md#commercecategory-translationscollection) | [`commerceCategory-translationsElement`](../schemas/commerceCategory.md#commercecategory-translationselement) |
| `urls` | [`commerceCategory-urlsCollection`](../schemas/commerceCategory.md#commercecategory-urlscollection) | [`commerceCategory-urlsElement`](../schemas/commerceCategory.md#commercecategory-urlselement) |

# salesPriceRule

Browser tag `salesPriceRule` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/salesPriceRule`, instance `/salesPriceRule/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/salesPriceRule` | `operation--salesPriceRule-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/salesPriceRule` | `operation--salesPriceRule-get` | Get list of records. |  | 200 OK → `salesPriceRuleCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/salesPriceRule` | `operation--salesPriceRule-patch` | Update records. | `salesPriceRuleCollection` | 202 Accepted; default → `nsError` |
| POST | `/salesPriceRule` | `operation--salesPriceRule-post` | Insert record. | `salesPriceRule` | 200 OK → `salesPriceRule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesPriceRule` | `operation--salesPriceRule-put` | Insert or update records. | `salesPriceRuleCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/salesPriceRule/{id}` | `operation--salesPriceRule--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/salesPriceRule/{id}` | `operation--salesPriceRule--id--get` | Get record. |  | 200 OK → `salesPriceRule`; 202 Accepted; default → `nsError` |
| PATCH | `/salesPriceRule/{id}` | `operation--salesPriceRule--id--patch` | Update record. | `salesPriceRule` | 200 OK → `salesPriceRule`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesPriceRule/{id}` | `operation--salesPriceRule--id--put` | Insert or update record. | `salesPriceRule` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--salesPriceRule-delete` | DELETE `/salesPriceRule` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule-get` | GET `/salesPriceRule` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule-patch` | PATCH `/salesPriceRule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule-post` | POST `/salesPriceRule` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--salesPriceRule-put` | PUT `/salesPriceRule` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule--id--delete` | DELETE `/salesPriceRule/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule--id--get` | GET `/salesPriceRule/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesPriceRule--id--patch` | PATCH `/salesPriceRule/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesPriceRule--id--put` | PUT `/salesPriceRule/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [salesPriceRule schemas](../schemas/salesPriceRule.md).

| Definition | Role |
| --- | --- |
| [`salesPriceRule`](../schemas/salesPriceRule.md#salespricerule) | record body |
| [`salesPriceRule-customerDimensionCollection`](../schemas/salesPriceRule.md#salespricerule-customerdimensioncollection) | sublist/collection |
| [`salesPriceRule-customerDimensionElement`](../schemas/salesPriceRule.md#salespricerule-customerdimensionelement) | sublist/element |
| [`salesPriceRule-customerGroupsCollection`](../schemas/salesPriceRule.md#salespricerule-customergroupscollection) | sublist/collection |
| [`salesPriceRule-customerGroupsElement`](../schemas/salesPriceRule.md#salespricerule-customergroupselement) | sublist/element |
| [`salesPriceRuleCollection`](../schemas/salesPriceRule.md#salespricerulecollection) | collection page |
| [`salesPriceRuleSelectOptions`](../schemas/salesPriceRule.md#salespriceruleselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `customerDimension` | [`salesPriceRule-customerDimensionCollection`](../schemas/salesPriceRule.md#salespricerule-customerdimensioncollection) | [`salesPriceRule-customerDimensionElement`](../schemas/salesPriceRule.md#salespricerule-customerdimensionelement) |
| `customerGroups` | [`salesPriceRule-customerGroupsCollection`](../schemas/salesPriceRule.md#salespricerule-customergroupscollection) | [`salesPriceRule-customerGroupsElement`](../schemas/salesPriceRule.md#salespricerule-customergroupselement) |

# shipItem

Browser tag `shipItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/shipItem`, instance `/shipItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/shipItem` | `operation--shipItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/shipItem` | `operation--shipItem-get` | Get list of records. |  | 200 OK → `shipItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/shipItem` | `operation--shipItem-patch` | Update records. | `shipItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/shipItem` | `operation--shipItem-post` | Insert record. | `shipItem` | 200 OK → `shipItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/shipItem` | `operation--shipItem-put` | Insert or update records. | `shipItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/shipItem/{id}` | `operation--shipItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/shipItem/{id}` | `operation--shipItem--id--get` | Get record. |  | 200 OK → `shipItem`; 202 Accepted; default → `nsError` |
| PATCH | `/shipItem/{id}` | `operation--shipItem--id--patch` | Update record. | `shipItem` | 200 OK → `shipItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/shipItem/{id}` | `operation--shipItem--id--put` | Insert or update record. | `shipItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--shipItem-delete` | DELETE `/shipItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem-get` | GET `/shipItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem-patch` | PATCH `/shipItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem-post` | POST `/shipItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--shipItem-put` | PUT `/shipItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem--id--delete` | DELETE `/shipItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem--id--get` | GET `/shipItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--shipItem--id--patch` | PATCH `/shipItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--shipItem--id--put` | PUT `/shipItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [shipItem schemas](../schemas/shipItem.md).

| Definition | Role |
| --- | --- |
| [`shipItem`](../schemas/shipItem.md#shipitem) | record body |
| [`shipItem-handlingTableCollection`](../schemas/shipItem.md#shipitem-handlingtablecollection) | sublist/collection |
| [`shipItem-handlingTableElement`](../schemas/shipItem.md#shipitem-handlingtableelement) | sublist/element |
| [`shipItem-itemsCollection`](../schemas/shipItem.md#shipitem-itemscollection) | sublist/collection |
| [`shipItem-itemsElement`](../schemas/shipItem.md#shipitem-itemselement) | sublist/element |
| [`shipItem-shipMethodRuleRelationsCollection`](../schemas/shipItem.md#shipitem-shipmethodrulerelationscollection) | sublist/collection |
| [`shipItem-shipMethodRuleRelationsElement`](../schemas/shipItem.md#shipitem-shipmethodrulerelationselement) | sublist/element |
| [`shipItem-shippingTableCollection`](../schemas/shipItem.md#shipitem-shippingtablecollection) | sublist/collection |
| [`shipItem-shippingTableElement`](../schemas/shipItem.md#shipitem-shippingtableelement) | sublist/element |
| [`shipItem-translationsCollection`](../schemas/shipItem.md#shipitem-translationscollection) | sublist/collection |
| [`shipItem-translationsElement`](../schemas/shipItem.md#shipitem-translationselement) | sublist/element |
| [`shipItemCollection`](../schemas/shipItem.md#shipitemcollection) | collection page |
| [`shipItemSelectOptions`](../schemas/shipItem.md#shipitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `handlingTable` | [`shipItem-handlingTableCollection`](../schemas/shipItem.md#shipitem-handlingtablecollection) | [`shipItem-handlingTableElement`](../schemas/shipItem.md#shipitem-handlingtableelement) |
| `items` | [`shipItem-itemsCollection`](../schemas/shipItem.md#shipitem-itemscollection) | [`shipItem-itemsElement`](../schemas/shipItem.md#shipitem-itemselement) |
| `shipMethodRuleRelations` | [`shipItem-shipMethodRuleRelationsCollection`](../schemas/shipItem.md#shipitem-shipmethodrulerelationscollection) | [`shipItem-shipMethodRuleRelationsElement`](../schemas/shipItem.md#shipitem-shipmethodrulerelationselement) |
| `shippingTable` | [`shipItem-shippingTableCollection`](../schemas/shipItem.md#shipitem-shippingtablecollection) | [`shipItem-shippingTableElement`](../schemas/shipItem.md#shipitem-shippingtableelement) |
| `translations` | [`shipItem-translationsCollection`](../schemas/shipItem.md#shipitem-translationscollection) | [`shipItem-translationsElement`](../schemas/shipItem.md#shipitem-translationselement) |

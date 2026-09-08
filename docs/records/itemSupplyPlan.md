# itemSupplyPlan

Browser tag `itemSupplyPlan` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/itemSupplyPlan`, instance `/itemSupplyPlan/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/itemSupplyPlan` | `operation--itemSupplyPlan-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/itemSupplyPlan` | `operation--itemSupplyPlan-get` | Get list of records. |  | 200 OK → `itemSupplyPlanCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/itemSupplyPlan` | `operation--itemSupplyPlan-patch` | Update records. | `itemSupplyPlanCollection` | 202 Accepted; default → `nsError` |
| POST | `/itemSupplyPlan` | `operation--itemSupplyPlan-post` | Insert record. | `itemSupplyPlan` | 200 OK → `itemSupplyPlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemSupplyPlan` | `operation--itemSupplyPlan-put` | Insert or update records. | `itemSupplyPlanCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/itemSupplyPlan/{id}` | `operation--itemSupplyPlan--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/itemSupplyPlan/{id}` | `operation--itemSupplyPlan--id--get` | Get record. |  | 200 OK → `itemSupplyPlan`; 202 Accepted; default → `nsError` |
| PATCH | `/itemSupplyPlan/{id}` | `operation--itemSupplyPlan--id--patch` | Update record. | `itemSupplyPlan` | 200 OK → `itemSupplyPlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/itemSupplyPlan/{id}` | `operation--itemSupplyPlan--id--put` | Insert or update record. | `itemSupplyPlan` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--itemSupplyPlan-delete` | DELETE `/itemSupplyPlan` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan-get` | GET `/itemSupplyPlan` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan-patch` | PATCH `/itemSupplyPlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan-post` | POST `/itemSupplyPlan` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--itemSupplyPlan-put` | PUT `/itemSupplyPlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan--id--delete` | DELETE `/itemSupplyPlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan--id--get` | GET `/itemSupplyPlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--itemSupplyPlan--id--patch` | PATCH `/itemSupplyPlan/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--itemSupplyPlan--id--put` | PUT `/itemSupplyPlan/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [itemSupplyPlan schemas](../schemas/itemSupplyPlan.md).

| Definition | Role |
| --- | --- |
| [`itemSupplyPlan`](../schemas/itemSupplyPlan.md#itemsupplyplan) | record body |
| [`itemSupplyPlan-orderCollection`](../schemas/itemSupplyPlan.md#itemsupplyplan-ordercollection) | sublist/collection |
| [`itemSupplyPlan-orderElement`](../schemas/itemSupplyPlan.md#itemsupplyplan-orderelement) | sublist/element |
| [`itemSupplyPlan-planningmessageCollection`](../schemas/itemSupplyPlan.md#itemsupplyplan-planningmessagecollection) | sublist/collection |
| [`itemSupplyPlan-planningmessageElement`](../schemas/itemSupplyPlan.md#itemsupplyplan-planningmessageelement) | sublist/element |
| [`itemSupplyPlanCollection`](../schemas/itemSupplyPlan.md#itemsupplyplancollection) | collection page |
| [`itemSupplyPlanSelectOptions`](../schemas/itemSupplyPlan.md#itemsupplyplanselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `order` | [`itemSupplyPlan-orderCollection`](../schemas/itemSupplyPlan.md#itemsupplyplan-ordercollection) | [`itemSupplyPlan-orderElement`](../schemas/itemSupplyPlan.md#itemsupplyplan-orderelement) |
| `planningmessage` | [`itemSupplyPlan-planningmessageCollection`](../schemas/itemSupplyPlan.md#itemsupplyplan-planningmessagecollection) | [`itemSupplyPlan-planningmessageElement`](../schemas/itemSupplyPlan.md#itemsupplyplan-planningmessageelement) |

# subscriptionPlan

Browser tag `subscriptionPlan` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subscriptionPlan`, instance `/subscriptionPlan/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subscriptionPlan` | `operation--subscriptionPlan-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subscriptionPlan` | `operation--subscriptionPlan-get` | Get list of records. |  | 200 OK → `subscriptionPlanCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionPlan` | `operation--subscriptionPlan-patch` | Update records. | `subscriptionPlanCollection` | 202 Accepted; default → `nsError` |
| POST | `/subscriptionPlan` | `operation--subscriptionPlan-post` | Insert record. | `subscriptionPlan` | 200 OK → `subscriptionPlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionPlan` | `operation--subscriptionPlan-put` | Insert or update records. | `subscriptionPlanCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subscriptionPlan/{id}` | `operation--subscriptionPlan--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subscriptionPlan/{id}` | `operation--subscriptionPlan--id--get` | Get record. |  | 200 OK → `subscriptionPlan`; 202 Accepted; default → `nsError` |
| PATCH | `/subscriptionPlan/{id}` | `operation--subscriptionPlan--id--patch` | Update record. | `subscriptionPlan` | 200 OK → `subscriptionPlan`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscriptionPlan/{id}` | `operation--subscriptionPlan--id--put` | Insert or update record. | `subscriptionPlan` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subscriptionPlan-delete` | DELETE `/subscriptionPlan` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan-get` | GET `/subscriptionPlan` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan-patch` | PATCH `/subscriptionPlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan-post` | POST `/subscriptionPlan` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subscriptionPlan-put` | PUT `/subscriptionPlan` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan--id--delete` | DELETE `/subscriptionPlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan--id--get` | GET `/subscriptionPlan/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscriptionPlan--id--patch` | PATCH `/subscriptionPlan/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subscriptionPlan--id--put` | PUT `/subscriptionPlan/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subscriptionPlan schemas](../schemas/subscriptionPlan.md).

| Definition | Role |
| --- | --- |
| [`subscriptionPlan`](../schemas/subscriptionPlan.md#subscriptionplan) | record body |
| [`subscriptionPlan-memberCollection`](../schemas/subscriptionPlan.md#subscriptionplan-membercollection) | sublist/collection |
| [`subscriptionPlan-memberElement`](../schemas/subscriptionPlan.md#subscriptionplan-memberelement) | sublist/element |
| [`subscriptionPlan-midtermUpliftCollection`](../schemas/subscriptionPlan.md#subscriptionplan-midtermupliftcollection) | sublist/collection |
| [`subscriptionPlan-midtermUpliftElement`](../schemas/subscriptionPlan.md#subscriptionplan-midtermupliftelement) | sublist/element |
| [`subscriptionPlan-renewalupliftCollection`](../schemas/subscriptionPlan.md#subscriptionplan-renewalupliftcollection) | sublist/collection |
| [`subscriptionPlan-renewalupliftElement`](../schemas/subscriptionPlan.md#subscriptionplan-renewalupliftelement) | sublist/element |
| [`subscriptionPlanCollection`](../schemas/subscriptionPlan.md#subscriptionplancollection) | collection page |
| [`subscriptionPlanSelectOptions`](../schemas/subscriptionPlan.md#subscriptionplanselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `member` | [`subscriptionPlan-memberCollection`](../schemas/subscriptionPlan.md#subscriptionplan-membercollection) | [`subscriptionPlan-memberElement`](../schemas/subscriptionPlan.md#subscriptionplan-memberelement) |
| `midtermUplift` | [`subscriptionPlan-midtermUpliftCollection`](../schemas/subscriptionPlan.md#subscriptionplan-midtermupliftcollection) | [`subscriptionPlan-midtermUpliftElement`](../schemas/subscriptionPlan.md#subscriptionplan-midtermupliftelement) |
| `renewaluplift` | [`subscriptionPlan-renewalupliftCollection`](../schemas/subscriptionPlan.md#subscriptionplan-renewalupliftcollection) | [`subscriptionPlan-renewalupliftElement`](../schemas/subscriptionPlan.md#subscriptionplan-renewalupliftelement) |

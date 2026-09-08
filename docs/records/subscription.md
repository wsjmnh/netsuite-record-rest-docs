# subscription

Browser tag `subscription` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/subscription`, instance `/subscription/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/subscription` | `operation--subscription-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/subscription` | `operation--subscription-get` | Get list of records. |  | 200 OK → `subscriptionCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/subscription` | `operation--subscription-patch` | Update records. | `subscriptionCollection` | 202 Accepted; default → `nsError` |
| POST | `/subscription` | `operation--subscription-post` | Insert record. | `subscription` | 200 OK → `subscription`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscription` | `operation--subscription-put` | Insert or update records. | `subscriptionCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/subscription/{id}` | `operation--subscription--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/subscription/{id}` | `operation--subscription--id--get` | Get record. |  | 200 OK → `subscription`; 202 Accepted; default → `nsError` |
| PATCH | `/subscription/{id}` | `operation--subscription--id--patch` | Update record. | `subscription` | 200 OK → `subscription`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/subscription/{id}` | `operation--subscription--id--put` | Insert or update record. | `subscription` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--subscription-delete` | DELETE `/subscription` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription-get` | GET `/subscription` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription-patch` | PATCH `/subscription` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription-post` | POST `/subscription` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--subscription-put` | PUT `/subscription` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription--id--delete` | DELETE `/subscription/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription--id--get` | GET `/subscription/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--subscription--id--patch` | PATCH `/subscription/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--subscription--id--put` | PUT `/subscription/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [subscription schemas](../schemas/subscription.md).

| Definition | Role |
| --- | --- |
| [`subscription`](../schemas/subscription.md#subscription) | record body |
| [`subscription-midtermUpliftCollection`](../schemas/subscription.md#subscription-midtermupliftcollection) | sublist/collection |
| [`subscription-midtermUpliftElement`](../schemas/subscription.md#subscription-midtermupliftelement) | sublist/element |
| [`subscription-priceIntervalCollection`](../schemas/subscription.md#subscription-priceintervalcollection) | sublist/collection |
| [`subscription-priceIntervalElement`](../schemas/subscription.md#subscription-priceintervalelement) | sublist/element |
| [`subscription-renewalupliftCollection`](../schemas/subscription.md#subscription-renewalupliftcollection) | sublist/collection |
| [`subscription-renewalupliftElement`](../schemas/subscription.md#subscription-renewalupliftelement) | sublist/element |
| [`subscription-subscriptionLineCollection`](../schemas/subscription.md#subscription-subscriptionlinecollection) | sublist/collection |
| [`subscription-subscriptionLineElement`](../schemas/subscription.md#subscription-subscriptionlineelement) | sublist/element |
| [`subscriptionCollection`](../schemas/subscription.md#subscriptioncollection) | collection page |
| [`subscriptionSelectOptions`](../schemas/subscription.md#subscriptionselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `midtermUplift` | [`subscription-midtermUpliftCollection`](../schemas/subscription.md#subscription-midtermupliftcollection) | [`subscription-midtermUpliftElement`](../schemas/subscription.md#subscription-midtermupliftelement) |
| `priceInterval` | [`subscription-priceIntervalCollection`](../schemas/subscription.md#subscription-priceintervalcollection) | [`subscription-priceIntervalElement`](../schemas/subscription.md#subscription-priceintervalelement) |
| `renewaluplift` | [`subscription-renewalupliftCollection`](../schemas/subscription.md#subscription-renewalupliftcollection) | [`subscription-renewalupliftElement`](../schemas/subscription.md#subscription-renewalupliftelement) |
| `subscriptionLine` | [`subscription-subscriptionLineCollection`](../schemas/subscription.md#subscription-subscriptionlinecollection) | [`subscription-subscriptionLineElement`](../schemas/subscription.md#subscription-subscriptionlineelement) |

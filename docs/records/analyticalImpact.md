# analyticalImpact

Browser tag `analyticalImpact` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/analyticalImpact`, instance `/analyticalImpact/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/analyticalImpact` | `operation--analyticalImpact-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/analyticalImpact` | `operation--analyticalImpact-get` | Get list of records. |  | 200 OK → `analyticalImpactCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/analyticalImpact` | `operation--analyticalImpact-patch` | Update records. | `analyticalImpactCollection` | 202 Accepted; default → `nsError` |
| POST | `/analyticalImpact` | `operation--analyticalImpact-post` | Insert record. | `analyticalImpact` | 200 OK → `analyticalImpact`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/analyticalImpact` | `operation--analyticalImpact-put` | Insert or update records. | `analyticalImpactCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/analyticalImpact/{id}` | `operation--analyticalImpact--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/analyticalImpact/{id}` | `operation--analyticalImpact--id--get` | Get record. |  | 200 OK → `analyticalImpact`; 202 Accepted; default → `nsError` |
| PATCH | `/analyticalImpact/{id}` | `operation--analyticalImpact--id--patch` | Update record. | `analyticalImpact` | 200 OK → `analyticalImpact`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/analyticalImpact/{id}` | `operation--analyticalImpact--id--put` | Insert or update record. | `analyticalImpact` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--analyticalImpact-delete` | DELETE `/analyticalImpact` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact-get` | GET `/analyticalImpact` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact-patch` | PATCH `/analyticalImpact` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact-post` | POST `/analyticalImpact` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--analyticalImpact-put` | PUT `/analyticalImpact` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact--id--delete` | DELETE `/analyticalImpact/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact--id--get` | GET `/analyticalImpact/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--analyticalImpact--id--patch` | PATCH `/analyticalImpact/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--analyticalImpact--id--put` | PUT `/analyticalImpact/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [analyticalImpact schemas](../schemas/analyticalImpact.md).

| Definition | Role |
| --- | --- |
| [`analyticalImpact`](../schemas/analyticalImpact.md#analyticalimpact) | record body |
| [`analyticalImpact-analyticalImpactEventCollection`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpacteventcollection) | sublist/collection |
| [`analyticalImpact-analyticalImpactEventElement`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpacteventelement) | sublist/element |
| [`analyticalImpact-analyticalImpactLinkCollection`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpactlinkcollection) | sublist/collection |
| [`analyticalImpact-analyticalImpactLinkElement`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpactlinkelement) | sublist/element |
| [`analyticalImpact-relatedRenewalsCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedrenewalscollection) | sublist/collection |
| [`analyticalImpact-relatedRenewalsElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedrenewalselement) | sublist/element |
| [`analyticalImpact-relatedSubscriptionChangeOrdersCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionchangeorderscollection) | sublist/collection |
| [`analyticalImpact-relatedSubscriptionChangeOrdersElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionchangeorderselement) | sublist/element |
| [`analyticalImpact-relatedSubscriptionLinesCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionlinescollection) | sublist/collection |
| [`analyticalImpact-relatedSubscriptionLinesElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionlineselement) | sublist/element |
| [`analyticalImpact-relatedSubscriptionsCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionscollection) | sublist/collection |
| [`analyticalImpact-relatedSubscriptionsElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionselement) | sublist/element |
| [`analyticalImpact-relatedTransactionLinesCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedtransactionlinescollection) | sublist/collection |
| [`analyticalImpact-relatedTransactionLinesElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedtransactionlineselement) | sublist/element |
| [`analyticalImpactCollection`](../schemas/analyticalImpact.md#analyticalimpactcollection) | collection page |
| [`analyticalImpactSelectOptions`](../schemas/analyticalImpact.md#analyticalimpactselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `analyticalImpactEvent` | [`analyticalImpact-analyticalImpactEventCollection`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpacteventcollection) | [`analyticalImpact-analyticalImpactEventElement`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpacteventelement) |
| `analyticalImpactLink` | [`analyticalImpact-analyticalImpactLinkCollection`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpactlinkcollection) | [`analyticalImpact-analyticalImpactLinkElement`](../schemas/analyticalImpact.md#analyticalimpact-analyticalimpactlinkelement) |
| `relatedRenewals` | [`analyticalImpact-relatedRenewalsCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedrenewalscollection) | [`analyticalImpact-relatedRenewalsElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedrenewalselement) |
| `relatedSubscriptionChangeOrders` | [`analyticalImpact-relatedSubscriptionChangeOrdersCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionchangeorderscollection) | [`analyticalImpact-relatedSubscriptionChangeOrdersElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionchangeorderselement) |
| `relatedSubscriptionLines` | [`analyticalImpact-relatedSubscriptionLinesCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionlinescollection) | [`analyticalImpact-relatedSubscriptionLinesElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionlineselement) |
| `relatedSubscriptions` | [`analyticalImpact-relatedSubscriptionsCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionscollection) | [`analyticalImpact-relatedSubscriptionsElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedsubscriptionselement) |
| `relatedTransactionLines` | [`analyticalImpact-relatedTransactionLinesCollection`](../schemas/analyticalImpact.md#analyticalimpact-relatedtransactionlinescollection) | [`analyticalImpact-relatedTransactionLinesElement`](../schemas/analyticalImpact.md#analyticalimpact-relatedtransactionlineselement) |

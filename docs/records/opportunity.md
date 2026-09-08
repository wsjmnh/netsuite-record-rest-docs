# opportunity

Browser tag `opportunity` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/opportunity`, instance `/opportunity/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/opportunity` | `operation--opportunity-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/opportunity` | `operation--opportunity-get` | Get list of records. |  | 200 OK → `opportunityCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/opportunity` | `operation--opportunity-patch` | Update records. | `opportunityCollection` | 202 Accepted; default → `nsError` |
| POST | `/opportunity` | `operation--opportunity-post` | Insert record. | `opportunity` | 200 OK → `opportunity`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/opportunity` | `operation--opportunity-put` | Insert or update records. | `opportunityCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/opportunity/{id}` | `operation--opportunity--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/opportunity/{id}` | `operation--opportunity--id--get` | Get record. |  | 200 OK → `opportunity`; 202 Accepted; default → `nsError` |
| PATCH | `/opportunity/{id}` | `operation--opportunity--id--patch` | Update record. | `opportunity` | 200 OK → `opportunity`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/opportunity/{id}` | `operation--opportunity--id--put` | Insert or update record. | `opportunity` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/opportunity/{id}/!transform/cashSale` | `operation--opportunity--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | 200 OK → `opportunity`; 202 Accepted; 204 No Content → `cashSale`; default → `nsError` |
| POST | `/opportunity/{id}/!transform/estimate` | `operation--opportunity--id---transform-estimate-post` | Transform to estimate. | `estimate` | 200 OK → `opportunity`; 202 Accepted; 204 No Content → `estimate`; default → `nsError` |
| POST | `/opportunity/{id}/!transform/invoice` | `operation--opportunity--id---transform-invoice-post` | Transform to invoice. | `invoice` | 200 OK → `opportunity`; 202 Accepted; 204 No Content → `invoice`; default → `nsError` |
| POST | `/opportunity/{id}/!transform/salesOrder` | `operation--opportunity--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | 200 OK → `opportunity`; 202 Accepted; 204 No Content → `salesOrder`; default → `nsError` |
| POST | `/opportunity/{targetId}/!attach/contact/{attachmentId}` | `operation--opportunity--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/opportunity/{targetId}/!detach/contact/{attachmentId}` | `operation--opportunity--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--opportunity-delete` | DELETE `/opportunity` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity-get` | GET `/opportunity` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity-patch` | PATCH `/opportunity` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity-post` | POST `/opportunity` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--opportunity-put` | PUT `/opportunity` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity--id--delete` | DELETE `/opportunity/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity--id--get` | GET `/opportunity/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity--id--patch` | PATCH `/opportunity/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--opportunity--id--put` | PUT `/opportunity/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--opportunity--id---transform-cashSale-post` | POST `/opportunity/{id}/!transform/cashSale` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--opportunity--id---transform-estimate-post` | POST `/opportunity/{id}/!transform/estimate` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--opportunity--id---transform-invoice-post` | POST `/opportunity/{id}/!transform/invoice` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--opportunity--id---transform-salesOrder-post` | POST `/opportunity/{id}/!transform/salesOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--opportunity--targetId---attach-contact--attachmentId--post` | POST `/opportunity/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--opportunity--targetId---detach-contact--attachmentId--post` | POST `/opportunity/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--opportunity--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [opportunity schemas](../schemas/opportunity.md).

| Definition | Role |
| --- | --- |
| [`opportunity`](../schemas/opportunity.md#opportunity) | record body |
| [`opportunity-accountingBookDetailCollection`](../schemas/opportunity.md#opportunity-accountingbookdetailcollection) | sublist/collection |
| [`opportunity-accountingBookDetailElement`](../schemas/opportunity.md#opportunity-accountingbookdetailelement) | sublist/element |
| [`opportunity-appliedRulesCollection`](../schemas/opportunity.md#opportunity-appliedrulescollection) | sublist/collection |
| [`opportunity-appliedRulesElement`](../schemas/opportunity.md#opportunity-appliedruleselement) | sublist/element |
| [`opportunity-billingAddress`](../schemas/opportunity.md#opportunity-billingaddress) | related |
| [`opportunity-competitorsCollection`](../schemas/opportunity.md#opportunity-competitorscollection) | sublist/collection |
| [`opportunity-competitorsElement`](../schemas/opportunity.md#opportunity-competitorselement) | sublist/element |
| [`opportunity-estimatesCollection`](../schemas/opportunity.md#opportunity-estimatescollection) | sublist/collection |
| [`opportunity-estimatesElement`](../schemas/opportunity.md#opportunity-estimateselement) | sublist/element |
| [`opportunity-itemCollection`](../schemas/opportunity.md#opportunity-itemcollection) | sublist/collection |
| [`opportunity-itemElement`](../schemas/opportunity.md#opportunity-itemelement) | sublist/element |
| [`opportunity-partnersCollection`](../schemas/opportunity.md#opportunity-partnerscollection) | sublist/collection |
| [`opportunity-partnersElement`](../schemas/opportunity.md#opportunity-partnerselement) | sublist/element |
| [`opportunity-salesTeamCollection`](../schemas/opportunity.md#opportunity-salesteamcollection) | sublist/collection |
| [`opportunity-salesTeamElement`](../schemas/opportunity.md#opportunity-salesteamelement) | sublist/element |
| [`opportunity-shippingAddress`](../schemas/opportunity.md#opportunity-shippingaddress) | related |
| [`opportunity-taxDetailsCollection`](../schemas/opportunity.md#opportunity-taxdetailscollection) | sublist/collection |
| [`opportunity-taxDetailsElement`](../schemas/opportunity.md#opportunity-taxdetailselement) | sublist/element |
| [`opportunityCollection`](../schemas/opportunity.md#opportunitycollection) | collection page |
| [`opportunitySelectOptions`](../schemas/opportunity.md#opportunityselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashSale`](../schemas/cashSale.md#cashsale)
- [`estimate`](../schemas/estimate.md#estimate)
- [`invoice`](../schemas/invoice.md#invoice)
- [`nsError`](../schemas/ns.md#nserror)
- [`salesOrder`](../schemas/salesOrder.md#salesorder)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`opportunity-accountingBookDetailCollection`](../schemas/opportunity.md#opportunity-accountingbookdetailcollection) | [`opportunity-accountingBookDetailElement`](../schemas/opportunity.md#opportunity-accountingbookdetailelement) |
| `appliedRules` | [`opportunity-appliedRulesCollection`](../schemas/opportunity.md#opportunity-appliedrulescollection) | [`opportunity-appliedRulesElement`](../schemas/opportunity.md#opportunity-appliedruleselement) |
| `competitors` | [`opportunity-competitorsCollection`](../schemas/opportunity.md#opportunity-competitorscollection) | [`opportunity-competitorsElement`](../schemas/opportunity.md#opportunity-competitorselement) |
| `estimates` | [`opportunity-estimatesCollection`](../schemas/opportunity.md#opportunity-estimatescollection) | [`opportunity-estimatesElement`](../schemas/opportunity.md#opportunity-estimateselement) |
| `item` | [`opportunity-itemCollection`](../schemas/opportunity.md#opportunity-itemcollection) | [`opportunity-itemElement`](../schemas/opportunity.md#opportunity-itemelement) |
| `partners` | [`opportunity-partnersCollection`](../schemas/opportunity.md#opportunity-partnerscollection) | [`opportunity-partnersElement`](../schemas/opportunity.md#opportunity-partnerselement) |
| `salesTeam` | [`opportunity-salesTeamCollection`](../schemas/opportunity.md#opportunity-salesteamcollection) | [`opportunity-salesTeamElement`](../schemas/opportunity.md#opportunity-salesteamelement) |
| `taxDetails` | [`opportunity-taxDetailsCollection`](../schemas/opportunity.md#opportunity-taxdetailscollection) | [`opportunity-taxDetailsElement`](../schemas/opportunity.md#opportunity-taxdetailselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/opportunity/{id}/!transform/cashSale` | `operation--opportunity--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | `cashSale` |
| POST | `/opportunity/{id}/!transform/estimate` | `operation--opportunity--id---transform-estimate-post` | Transform to estimate. | `estimate` | `estimate` |
| POST | `/opportunity/{id}/!transform/invoice` | `operation--opportunity--id---transform-invoice-post` | Transform to invoice. | `invoice` | `invoice` |
| POST | `/opportunity/{id}/!transform/salesOrder` | `operation--opportunity--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | `salesOrder` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/opportunity/{targetId}/!attach/contact/{attachmentId}` | `operation--opportunity--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/opportunity/{targetId}/!detach/contact/{attachmentId}` | `operation--opportunity--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

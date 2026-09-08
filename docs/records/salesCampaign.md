# salesCampaign

Browser tag `salesCampaign` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/salesCampaign`, instance `/salesCampaign/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/salesCampaign` | `operation--salesCampaign-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| PATCH | `/salesCampaign` | `operation--salesCampaign-patch` | Update records. | `salesCampaignCollection` | 202 Accepted; default → `nsError` |
| POST | `/salesCampaign` | `operation--salesCampaign-post` | Insert record. | `salesCampaign` | 200 OK → `salesCampaign`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesCampaign` | `operation--salesCampaign-put` | Insert or update records. | `salesCampaignCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/salesCampaign/{id}` | `operation--salesCampaign--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/salesCampaign/{id}` | `operation--salesCampaign--id--get` | Get record. |  | 200 OK → `salesCampaign`; 202 Accepted; default → `nsError` |
| PATCH | `/salesCampaign/{id}` | `operation--salesCampaign--id--patch` | Update record. | `salesCampaign` | 200 OK → `salesCampaign`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/salesCampaign/{id}` | `operation--salesCampaign--id--put` | Insert or update record. | `salesCampaign` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--salesCampaign-delete` | DELETE `/salesCampaign` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesCampaign-patch` | PATCH `/salesCampaign` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesCampaign-post` | POST `/salesCampaign` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--salesCampaign-put` | PUT `/salesCampaign` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesCampaign--id--delete` | DELETE `/salesCampaign/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesCampaign--id--get` | GET `/salesCampaign/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--salesCampaign--id--patch` | PATCH `/salesCampaign/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--salesCampaign--id--put` | PUT `/salesCampaign/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [salesCampaign schemas](../schemas/salesCampaign.md).

| Definition | Role |
| --- | --- |
| [`salesCampaign`](../schemas/salesCampaign.md#salescampaign) | record body |
| [`salesCampaign-campaignDirectMailCollection`](../schemas/salesCampaign.md#salescampaign-campaigndirectmailcollection) | sublist/collection |
| [`salesCampaign-campaignDirectMailElement`](../schemas/salesCampaign.md#salescampaign-campaigndirectmailelement) | sublist/element |
| [`salesCampaign-campaignDripCollection`](../schemas/salesCampaign.md#salescampaign-campaigndripcollection) | sublist/collection |
| [`salesCampaign-campaignDripElement`](../schemas/salesCampaign.md#salescampaign-campaigndripelement) | sublist/element |
| [`salesCampaign-campaignEmailCollection`](../schemas/salesCampaign.md#salescampaign-campaignemailcollection) | sublist/collection |
| [`salesCampaign-campaignEmailElement`](../schemas/salesCampaign.md#salescampaign-campaignemailelement) | sublist/element |
| [`salesCampaign-campaignEventCollection`](../schemas/salesCampaign.md#salescampaign-campaigneventcollection) | sublist/collection |
| [`salesCampaign-campaignEventElement`](../schemas/salesCampaign.md#salescampaign-campaigneventelement) | sublist/element |
| [`salesCampaign-defaultEventCollection`](../schemas/salesCampaign.md#salescampaign-defaulteventcollection) | sublist/collection |
| [`salesCampaign-defaultEventElement`](../schemas/salesCampaign.md#salescampaign-defaulteventelement) | sublist/element |
| [`salesCampaignCollection`](../schemas/salesCampaign.md#salescampaigncollection) | collection page |
| [`salesCampaignSelectOptions`](../schemas/salesCampaign.md#salescampaignselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `campaignDirectMail` | [`salesCampaign-campaignDirectMailCollection`](../schemas/salesCampaign.md#salescampaign-campaigndirectmailcollection) | [`salesCampaign-campaignDirectMailElement`](../schemas/salesCampaign.md#salescampaign-campaigndirectmailelement) |
| `campaignDrip` | [`salesCampaign-campaignDripCollection`](../schemas/salesCampaign.md#salescampaign-campaigndripcollection) | [`salesCampaign-campaignDripElement`](../schemas/salesCampaign.md#salescampaign-campaigndripelement) |
| `campaignEmail` | [`salesCampaign-campaignEmailCollection`](../schemas/salesCampaign.md#salescampaign-campaignemailcollection) | [`salesCampaign-campaignEmailElement`](../schemas/salesCampaign.md#salescampaign-campaignemailelement) |
| `campaignEvent` | [`salesCampaign-campaignEventCollection`](../schemas/salesCampaign.md#salescampaign-campaigneventcollection) | [`salesCampaign-campaignEventElement`](../schemas/salesCampaign.md#salescampaign-campaigneventelement) |
| `defaultEvent` | [`salesCampaign-defaultEventCollection`](../schemas/salesCampaign.md#salescampaign-defaulteventcollection) | [`salesCampaign-defaultEventElement`](../schemas/salesCampaign.md#salescampaign-defaulteventelement) |

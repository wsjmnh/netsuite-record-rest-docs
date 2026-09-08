# campaign

Browser tag `campaign` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaign`, instance `/campaign/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaign` | `operation--campaign-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaign` | `operation--campaign-get` | Get list of records. |  | 200 OK → `campaignCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaign` | `operation--campaign-patch` | Update records. | `campaignCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaign` | `operation--campaign-post` | Insert record. | `campaign` | 200 OK → `campaign`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaign` | `operation--campaign-put` | Insert or update records. | `campaignCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaign/{id}` | `operation--campaign--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaign/{id}` | `operation--campaign--id--get` | Get record. |  | 200 OK → `campaign`; 202 Accepted; default → `nsError` |
| PATCH | `/campaign/{id}` | `operation--campaign--id--patch` | Update record. | `campaign` | 200 OK → `campaign`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaign/{id}` | `operation--campaign--id--put` | Insert or update record. | `campaign` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaign-delete` | DELETE `/campaign` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign-get` | GET `/campaign` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign-patch` | PATCH `/campaign` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign-post` | POST `/campaign` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaign-put` | PUT `/campaign` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign--id--delete` | DELETE `/campaign/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign--id--get` | GET `/campaign/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaign--id--patch` | PATCH `/campaign/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaign--id--put` | PUT `/campaign/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaign schemas](../schemas/campaign.md).

| Definition | Role |
| --- | --- |
| [`campaign`](../schemas/campaign.md#campaign) | record body |
| [`campaign-campaignDirectMailCollection`](../schemas/campaign.md#campaign-campaigndirectmailcollection) | sublist/collection |
| [`campaign-campaignDirectMailElement`](../schemas/campaign.md#campaign-campaigndirectmailelement) | sublist/element |
| [`campaign-campaignDripCollection`](../schemas/campaign.md#campaign-campaigndripcollection) | sublist/collection |
| [`campaign-campaignDripElement`](../schemas/campaign.md#campaign-campaigndripelement) | sublist/element |
| [`campaign-campaignEmailCollection`](../schemas/campaign.md#campaign-campaignemailcollection) | sublist/collection |
| [`campaign-campaignEmailElement`](../schemas/campaign.md#campaign-campaignemailelement) | sublist/element |
| [`campaign-campaignEventCollection`](../schemas/campaign.md#campaign-campaigneventcollection) | sublist/collection |
| [`campaign-campaignEventElement`](../schemas/campaign.md#campaign-campaigneventelement) | sublist/element |
| [`campaign-defaultEventCollection`](../schemas/campaign.md#campaign-defaulteventcollection) | sublist/collection |
| [`campaign-defaultEventElement`](../schemas/campaign.md#campaign-defaulteventelement) | sublist/element |
| [`campaignCollection`](../schemas/campaign.md#campaigncollection) | collection page |
| [`campaignSelectOptions`](../schemas/campaign.md#campaignselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `campaignDirectMail` | [`campaign-campaignDirectMailCollection`](../schemas/campaign.md#campaign-campaigndirectmailcollection) | [`campaign-campaignDirectMailElement`](../schemas/campaign.md#campaign-campaigndirectmailelement) |
| `campaignDrip` | [`campaign-campaignDripCollection`](../schemas/campaign.md#campaign-campaigndripcollection) | [`campaign-campaignDripElement`](../schemas/campaign.md#campaign-campaigndripelement) |
| `campaignEmail` | [`campaign-campaignEmailCollection`](../schemas/campaign.md#campaign-campaignemailcollection) | [`campaign-campaignEmailElement`](../schemas/campaign.md#campaign-campaignemailelement) |
| `campaignEvent` | [`campaign-campaignEventCollection`](../schemas/campaign.md#campaign-campaigneventcollection) | [`campaign-campaignEventElement`](../schemas/campaign.md#campaign-campaigneventelement) |
| `defaultEvent` | [`campaign-defaultEventCollection`](../schemas/campaign.md#campaign-defaulteventcollection) | [`campaign-defaultEventElement`](../schemas/campaign.md#campaign-defaulteventelement) |

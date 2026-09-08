# campaignResponse

Browser tag `campaignResponse` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/campaignResponse`, instance `/campaignResponse/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/campaignResponse` | `operation--campaignResponse-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/campaignResponse` | `operation--campaignResponse-get` | Get list of records. |  | 200 OK → `campaignResponseCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignResponse` | `operation--campaignResponse-patch` | Update records. | `campaignResponseCollection` | 202 Accepted; default → `nsError` |
| POST | `/campaignResponse` | `operation--campaignResponse-post` | Insert record. | `campaignResponse` | 200 OK → `campaignResponse`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignResponse` | `operation--campaignResponse-put` | Insert or update records. | `campaignResponseCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/campaignResponse/{id}` | `operation--campaignResponse--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/campaignResponse/{id}` | `operation--campaignResponse--id--get` | Get record. |  | 200 OK → `campaignResponse`; 202 Accepted; default → `nsError` |
| PATCH | `/campaignResponse/{id}` | `operation--campaignResponse--id--patch` | Update record. | `campaignResponse` | 200 OK → `campaignResponse`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/campaignResponse/{id}` | `operation--campaignResponse--id--put` | Insert or update record. | `campaignResponse` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--campaignResponse-delete` | DELETE `/campaignResponse` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse-get` | GET `/campaignResponse` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse-patch` | PATCH `/campaignResponse` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse-post` | POST `/campaignResponse` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--campaignResponse-put` | PUT `/campaignResponse` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse--id--delete` | DELETE `/campaignResponse/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse--id--get` | GET `/campaignResponse/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--campaignResponse--id--patch` | PATCH `/campaignResponse/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--campaignResponse--id--put` | PUT `/campaignResponse/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [campaignResponse schemas](../schemas/campaignResponse.md).

| Definition | Role |
| --- | --- |
| [`campaignResponse`](../schemas/campaignResponse.md#campaignresponse) | record body |
| [`campaignResponse-responsesCollection`](../schemas/campaignResponse.md#campaignresponse-responsescollection) | sublist/collection |
| [`campaignResponse-responsesElement`](../schemas/campaignResponse.md#campaignresponse-responseselement) | sublist/element |
| [`campaignResponseCollection`](../schemas/campaignResponse.md#campaignresponsecollection) | collection page |
| [`campaignResponseSelectOptions`](../schemas/campaignResponse.md#campaignresponseselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `responses` | [`campaignResponse-responsesCollection`](../schemas/campaignResponse.md#campaignresponse-responsescollection) | [`campaignResponse-responsesElement`](../schemas/campaignResponse.md#campaignresponse-responseselement) |

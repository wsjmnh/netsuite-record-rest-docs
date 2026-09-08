# customerSubsidiaryRelationship

Browser tag `customerSubsidiaryRelationship` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customerSubsidiaryRelationship`, instance `/customerSubsidiaryRelationship/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customerSubsidiaryRelationship` | `operation--customerSubsidiaryRelationship-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customerSubsidiaryRelationship` | `operation--customerSubsidiaryRelationship-get` | Get list of records. |  | 200 OK → `customerSubsidiaryRelationshipCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customerSubsidiaryRelationship` | `operation--customerSubsidiaryRelationship-patch` | Update records. | `customerSubsidiaryRelationshipCollection` | 202 Accepted; default → `nsError` |
| POST | `/customerSubsidiaryRelationship` | `operation--customerSubsidiaryRelationship-post` | Insert record. | `customerSubsidiaryRelationship` | 200 OK → `customerSubsidiaryRelationship`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerSubsidiaryRelationship` | `operation--customerSubsidiaryRelationship-put` | Insert or update records. | `customerSubsidiaryRelationshipCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customerSubsidiaryRelationship/{id}` | `operation--customerSubsidiaryRelationship--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customerSubsidiaryRelationship/{id}` | `operation--customerSubsidiaryRelationship--id--get` | Get record. |  | 200 OK → `customerSubsidiaryRelationship`; 202 Accepted; default → `nsError` |
| PATCH | `/customerSubsidiaryRelationship/{id}` | `operation--customerSubsidiaryRelationship--id--patch` | Update record. | `customerSubsidiaryRelationship` | 200 OK → `customerSubsidiaryRelationship`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customerSubsidiaryRelationship/{id}` | `operation--customerSubsidiaryRelationship--id--put` | Insert or update record. | `customerSubsidiaryRelationship` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customerSubsidiaryRelationship-delete` | DELETE `/customerSubsidiaryRelationship` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship-get` | GET `/customerSubsidiaryRelationship` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship-patch` | PATCH `/customerSubsidiaryRelationship` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship-post` | POST `/customerSubsidiaryRelationship` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customerSubsidiaryRelationship-put` | PUT `/customerSubsidiaryRelationship` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship--id--delete` | DELETE `/customerSubsidiaryRelationship/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship--id--get` | GET `/customerSubsidiaryRelationship/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customerSubsidiaryRelationship--id--patch` | PATCH `/customerSubsidiaryRelationship/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customerSubsidiaryRelationship--id--put` | PUT `/customerSubsidiaryRelationship/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [customerSubsidiaryRelationship schemas](../schemas/customerSubsidiaryRelationship.md).

| Definition | Role |
| --- | --- |
| [`customerSubsidiaryRelationship`](../schemas/customerSubsidiaryRelationship.md#customersubsidiaryrelationship) | record body |
| [`customerSubsidiaryRelationshipCollection`](../schemas/customerSubsidiaryRelationship.md#customersubsidiaryrelationshipcollection) | collection page |
| [`customerSubsidiaryRelationshipSelectOptions`](../schemas/customerSubsidiaryRelationship.md#customersubsidiaryrelationshipselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.

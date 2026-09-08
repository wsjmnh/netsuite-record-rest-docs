# gLNumberingSequence

Browser tag `gLNumberingSequence` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/gLNumberingSequence`, instance `/gLNumberingSequence/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/gLNumberingSequence` | `operation--gLNumberingSequence-get` | Get list of records. |  | 200 OK → `gLNumberingSequenceCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/gLNumberingSequence` | `operation--gLNumberingSequence-patch` | Update records. | `gLNumberingSequenceCollection` | 202 Accepted; default → `nsError` |
| POST | `/gLNumberingSequence` | `operation--gLNumberingSequence-post` | Insert record. | `gLNumberingSequence` | 200 OK → `gLNumberingSequence`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/gLNumberingSequence` | `operation--gLNumberingSequence-put` | Insert or update records. | `gLNumberingSequenceCollection` | 202 Accepted; default → `nsError` |
| GET | `/gLNumberingSequence/{id}` | `operation--gLNumberingSequence--id--get` | Get record. |  | 200 OK → `gLNumberingSequence`; 202 Accepted; default → `nsError` |
| PATCH | `/gLNumberingSequence/{id}` | `operation--gLNumberingSequence--id--patch` | Update record. | `gLNumberingSequence` | 200 OK → `gLNumberingSequence`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/gLNumberingSequence/{id}` | `operation--gLNumberingSequence--id--put` | Insert or update record. | `gLNumberingSequence` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--gLNumberingSequence-get` | GET `/gLNumberingSequence` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--gLNumberingSequence-patch` | PATCH `/gLNumberingSequence` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--gLNumberingSequence-post` | POST `/gLNumberingSequence` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--gLNumberingSequence-put` | PUT `/gLNumberingSequence` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--gLNumberingSequence--id--get` | GET `/gLNumberingSequence/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--gLNumberingSequence--id--patch` | PATCH `/gLNumberingSequence/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--gLNumberingSequence--id--put` | PUT `/gLNumberingSequence/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [gLNumberingSequence schemas](../schemas/gLNumberingSequence.md).

| Definition | Role |
| --- | --- |
| [`gLNumberingSequence`](../schemas/gLNumberingSequence.md#glnumberingsequence) | record body |
| [`gLNumberingSequenceCollection`](../schemas/gLNumberingSequence.md#glnumberingsequencecollection) | collection page |
| [`gLNumberingSequenceSelectOptions`](../schemas/gLNumberingSequence.md#glnumberingsequenceselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.

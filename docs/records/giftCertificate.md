# giftCertificate

Browser tag `giftCertificate` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/giftCertificate`, instance `/giftCertificate/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/giftCertificate` | `operation--giftCertificate-get` | Get list of records. |  | 200 OK → `giftCertificateCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/giftCertificate` | `operation--giftCertificate-patch` | Update records. | `giftCertificateCollection` | 202 Accepted; default → `nsError` |
| PUT | `/giftCertificate` | `operation--giftCertificate-put` | Insert or update records. | `giftCertificateCollection` | 202 Accepted; default → `nsError` |
| GET | `/giftCertificate/{id}` | `operation--giftCertificate--id--get` | Get record. |  | 200 OK → `giftCertificate`; 202 Accepted; default → `nsError` |
| PATCH | `/giftCertificate/{id}` | `operation--giftCertificate--id--patch` | Update record. | `giftCertificate` | 200 OK → `giftCertificate`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/giftCertificate/{id}` | `operation--giftCertificate--id--put` | Insert or update record. | `giftCertificate` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--giftCertificate-get` | GET `/giftCertificate` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificate-patch` | PATCH `/giftCertificate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificate-put` | PUT `/giftCertificate` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificate--id--get` | GET `/giftCertificate/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificate--id--patch` | PATCH `/giftCertificate/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--giftCertificate--id--put` | PUT `/giftCertificate/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [giftCertificate schemas](../schemas/giftCertificate.md).

| Definition | Role |
| --- | --- |
| [`giftCertificate`](../schemas/giftCertificate.md#giftcertificate) | record body |
| [`giftCertificateCollection`](../schemas/giftCertificate.md#giftcertificatecollection) | collection page |
| [`giftCertificateSelectOptions`](../schemas/giftCertificate.md#giftcertificateselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

No `*Collection` properties on the record schema other than the record’s own collection type.

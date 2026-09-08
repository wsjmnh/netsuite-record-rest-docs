# statisticalJournalEntry

Browser tag `statisticalJournalEntry` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/statisticalJournalEntry`, instance `/statisticalJournalEntry/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/statisticalJournalEntry` | `operation--statisticalJournalEntry-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/statisticalJournalEntry` | `operation--statisticalJournalEntry-get` | Get list of records. |  | 200 OK → `statisticalJournalEntryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/statisticalJournalEntry` | `operation--statisticalJournalEntry-patch` | Update records. | `statisticalJournalEntryCollection` | 202 Accepted; default → `nsError` |
| POST | `/statisticalJournalEntry` | `operation--statisticalJournalEntry-post` | Insert record. | `statisticalJournalEntry` | 200 OK → `statisticalJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/statisticalJournalEntry` | `operation--statisticalJournalEntry-put` | Insert or update records. | `statisticalJournalEntryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/statisticalJournalEntry/{id}` | `operation--statisticalJournalEntry--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/statisticalJournalEntry/{id}` | `operation--statisticalJournalEntry--id--get` | Get record. |  | 200 OK → `statisticalJournalEntry`; 202 Accepted; default → `nsError` |
| PATCH | `/statisticalJournalEntry/{id}` | `operation--statisticalJournalEntry--id--patch` | Update record. | `statisticalJournalEntry` | 200 OK → `statisticalJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/statisticalJournalEntry/{id}` | `operation--statisticalJournalEntry--id--put` | Insert or update record. | `statisticalJournalEntry` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--statisticalJournalEntry-delete` | DELETE `/statisticalJournalEntry` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry-get` | GET `/statisticalJournalEntry` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry-patch` | PATCH `/statisticalJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry-post` | POST `/statisticalJournalEntry` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--statisticalJournalEntry-put` | PUT `/statisticalJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry--id--delete` | DELETE `/statisticalJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry--id--get` | GET `/statisticalJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--statisticalJournalEntry--id--patch` | PATCH `/statisticalJournalEntry/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--statisticalJournalEntry--id--put` | PUT `/statisticalJournalEntry/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [statisticalJournalEntry schemas](../schemas/statisticalJournalEntry.md).

| Definition | Role |
| --- | --- |
| [`statisticalJournalEntry`](../schemas/statisticalJournalEntry.md#statisticaljournalentry) | record body |
| [`statisticalJournalEntry-lineCollection`](../schemas/statisticalJournalEntry.md#statisticaljournalentry-linecollection) | sublist/collection |
| [`statisticalJournalEntry-lineElement`](../schemas/statisticalJournalEntry.md#statisticaljournalentry-lineelement) | sublist/element |
| [`statisticalJournalEntryCollection`](../schemas/statisticalJournalEntry.md#statisticaljournalentrycollection) | collection page |
| [`statisticalJournalEntrySelectOptions`](../schemas/statisticalJournalEntry.md#statisticaljournalentryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `line` | [`statisticalJournalEntry-lineCollection`](../schemas/statisticalJournalEntry.md#statisticaljournalentry-linecollection) | [`statisticalJournalEntry-lineElement`](../schemas/statisticalJournalEntry.md#statisticaljournalentry-lineelement) |

# journalEntry

Browser tag `journalEntry` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/journalEntry`, instance `/journalEntry/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/journalEntry` | `operation--journalEntry-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/journalEntry` | `operation--journalEntry-get` | Get list of records. |  | 200 OK → `journalEntryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/journalEntry` | `operation--journalEntry-patch` | Update records. | `journalEntryCollection` | 202 Accepted; default → `nsError` |
| POST | `/journalEntry` | `operation--journalEntry-post` | Insert record. | `journalEntry` | 200 OK → `journalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/journalEntry` | `operation--journalEntry-put` | Insert or update records. | `journalEntryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/journalEntry/{id}` | `operation--journalEntry--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/journalEntry/{id}` | `operation--journalEntry--id--get` | Get record. |  | 200 OK → `journalEntry`; 202 Accepted; default → `nsError` |
| PATCH | `/journalEntry/{id}` | `operation--journalEntry--id--patch` | Update record. | `journalEntry` | 200 OK → `journalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/journalEntry/{id}` | `operation--journalEntry--id--put` | Insert or update record. | `journalEntry` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--journalEntry-delete` | DELETE `/journalEntry` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry-get` | GET `/journalEntry` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry-patch` | PATCH `/journalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry-post` | POST `/journalEntry` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--journalEntry-put` | PUT `/journalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry--id--delete` | DELETE `/journalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry--id--get` | GET `/journalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--journalEntry--id--patch` | PATCH `/journalEntry/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--journalEntry--id--put` | PUT `/journalEntry/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [journalEntry schemas](../schemas/journalEntry.md).

| Definition | Role |
| --- | --- |
| [`journalEntry`](../schemas/journalEntry.md#journalentry) | record body |
| [`journalEntry-accountingBookDetailCollection`](../schemas/journalEntry.md#journalentry-accountingbookdetailcollection) | sublist/collection |
| [`journalEntry-accountingBookDetailElement`](../schemas/journalEntry.md#journalentry-accountingbookdetailelement) | sublist/element |
| [`journalEntry-appliedRulesCollection`](../schemas/journalEntry.md#journalentry-appliedrulescollection) | sublist/collection |
| [`journalEntry-appliedRulesElement`](../schemas/journalEntry.md#journalentry-appliedruleselement) | sublist/element |
| [`journalEntry-lineCollection`](../schemas/journalEntry.md#journalentry-linecollection) | sublist/collection |
| [`journalEntry-lineElement`](../schemas/journalEntry.md#journalentry-lineelement) | sublist/element |
| [`journalEntryCollection`](../schemas/journalEntry.md#journalentrycollection) | collection page |
| [`journalEntrySelectOptions`](../schemas/journalEntry.md#journalentryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`journalEntry-accountingBookDetailCollection`](../schemas/journalEntry.md#journalentry-accountingbookdetailcollection) | [`journalEntry-accountingBookDetailElement`](../schemas/journalEntry.md#journalentry-accountingbookdetailelement) |
| `appliedRules` | [`journalEntry-appliedRulesCollection`](../schemas/journalEntry.md#journalentry-appliedrulescollection) | [`journalEntry-appliedRulesElement`](../schemas/journalEntry.md#journalentry-appliedruleselement) |
| `line` | [`journalEntry-lineCollection`](../schemas/journalEntry.md#journalentry-linecollection) | [`journalEntry-lineElement`](../schemas/journalEntry.md#journalentry-lineelement) |

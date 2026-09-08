# intercompanyJournalEntry

Browser tag `intercompanyJournalEntry` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/intercompanyJournalEntry`, instance `/intercompanyJournalEntry/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/intercompanyJournalEntry` | `operation--intercompanyJournalEntry-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/intercompanyJournalEntry` | `operation--intercompanyJournalEntry-get` | Get list of records. |  | 200 OK → `intercompanyJournalEntryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/intercompanyJournalEntry` | `operation--intercompanyJournalEntry-patch` | Update records. | `intercompanyJournalEntryCollection` | 202 Accepted; default → `nsError` |
| POST | `/intercompanyJournalEntry` | `operation--intercompanyJournalEntry-post` | Insert record. | `intercompanyJournalEntry` | 200 OK → `intercompanyJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/intercompanyJournalEntry` | `operation--intercompanyJournalEntry-put` | Insert or update records. | `intercompanyJournalEntryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/intercompanyJournalEntry/{id}` | `operation--intercompanyJournalEntry--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/intercompanyJournalEntry/{id}` | `operation--intercompanyJournalEntry--id--get` | Get record. |  | 200 OK → `intercompanyJournalEntry`; 202 Accepted; default → `nsError` |
| PATCH | `/intercompanyJournalEntry/{id}` | `operation--intercompanyJournalEntry--id--patch` | Update record. | `intercompanyJournalEntry` | 200 OK → `intercompanyJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/intercompanyJournalEntry/{id}` | `operation--intercompanyJournalEntry--id--put` | Insert or update record. | `intercompanyJournalEntry` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--intercompanyJournalEntry-delete` | DELETE `/intercompanyJournalEntry` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry-get` | GET `/intercompanyJournalEntry` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry-patch` | PATCH `/intercompanyJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry-post` | POST `/intercompanyJournalEntry` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--intercompanyJournalEntry-put` | PUT `/intercompanyJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry--id--delete` | DELETE `/intercompanyJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry--id--get` | GET `/intercompanyJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--intercompanyJournalEntry--id--patch` | PATCH `/intercompanyJournalEntry/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--intercompanyJournalEntry--id--put` | PUT `/intercompanyJournalEntry/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [intercompanyJournalEntry schemas](../schemas/intercompanyJournalEntry.md).

| Definition | Role |
| --- | --- |
| [`intercompanyJournalEntry`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry) | record body |
| [`intercompanyJournalEntry-accountingBookDetailCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-accountingbookdetailcollection) | sublist/collection |
| [`intercompanyJournalEntry-accountingBookDetailElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-accountingbookdetailelement) | sublist/element |
| [`intercompanyJournalEntry-appliedRulesCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-appliedrulescollection) | sublist/collection |
| [`intercompanyJournalEntry-appliedRulesElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-appliedruleselement) | sublist/element |
| [`intercompanyJournalEntry-lineCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-linecollection) | sublist/collection |
| [`intercompanyJournalEntry-lineElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-lineelement) | sublist/element |
| [`intercompanyJournalEntryCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentrycollection) | collection page |
| [`intercompanyJournalEntrySelectOptions`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`intercompanyJournalEntry-accountingBookDetailCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-accountingbookdetailcollection) | [`intercompanyJournalEntry-accountingBookDetailElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-accountingbookdetailelement) |
| `appliedRules` | [`intercompanyJournalEntry-appliedRulesCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-appliedrulescollection) | [`intercompanyJournalEntry-appliedRulesElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-appliedruleselement) |
| `line` | [`intercompanyJournalEntry-lineCollection`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-linecollection) | [`intercompanyJournalEntry-lineElement`](../schemas/intercompanyJournalEntry.md#intercompanyjournalentry-lineelement) |

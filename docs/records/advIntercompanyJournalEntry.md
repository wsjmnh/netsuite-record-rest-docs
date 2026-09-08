# advIntercompanyJournalEntry

Browser tag `advIntercompanyJournalEntry` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/advIntercompanyJournalEntry`, instance `/advIntercompanyJournalEntry/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/advIntercompanyJournalEntry` | `operation--advIntercompanyJournalEntry-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/advIntercompanyJournalEntry` | `operation--advIntercompanyJournalEntry-get` | Get list of records. |  | 200 OK → `advIntercompanyJournalEntryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/advIntercompanyJournalEntry` | `operation--advIntercompanyJournalEntry-patch` | Update records. | `advIntercompanyJournalEntryCollection` | 202 Accepted; default → `nsError` |
| POST | `/advIntercompanyJournalEntry` | `operation--advIntercompanyJournalEntry-post` | Insert record. | `advIntercompanyJournalEntry` | 200 OK → `advIntercompanyJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/advIntercompanyJournalEntry` | `operation--advIntercompanyJournalEntry-put` | Insert or update records. | `advIntercompanyJournalEntryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/advIntercompanyJournalEntry/{id}` | `operation--advIntercompanyJournalEntry--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/advIntercompanyJournalEntry/{id}` | `operation--advIntercompanyJournalEntry--id--get` | Get record. |  | 200 OK → `advIntercompanyJournalEntry`; 202 Accepted; default → `nsError` |
| PATCH | `/advIntercompanyJournalEntry/{id}` | `operation--advIntercompanyJournalEntry--id--patch` | Update record. | `advIntercompanyJournalEntry` | 200 OK → `advIntercompanyJournalEntry`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/advIntercompanyJournalEntry/{id}` | `operation--advIntercompanyJournalEntry--id--put` | Insert or update record. | `advIntercompanyJournalEntry` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--advIntercompanyJournalEntry-delete` | DELETE `/advIntercompanyJournalEntry` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry-get` | GET `/advIntercompanyJournalEntry` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry-patch` | PATCH `/advIntercompanyJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry-post` | POST `/advIntercompanyJournalEntry` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--advIntercompanyJournalEntry-put` | PUT `/advIntercompanyJournalEntry` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry--id--delete` | DELETE `/advIntercompanyJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry--id--get` | GET `/advIntercompanyJournalEntry/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--advIntercompanyJournalEntry--id--patch` | PATCH `/advIntercompanyJournalEntry/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--advIntercompanyJournalEntry--id--put` | PUT `/advIntercompanyJournalEntry/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [advIntercompanyJournalEntry schemas](../schemas/advIntercompanyJournalEntry.md).

| Definition | Role |
| --- | --- |
| [`advIntercompanyJournalEntry`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry) | record body |
| [`advIntercompanyJournalEntry-accountingBookDetailCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-accountingbookdetailcollection) | sublist/collection |
| [`advIntercompanyJournalEntry-accountingBookDetailElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-accountingbookdetailelement) | sublist/element |
| [`advIntercompanyJournalEntry-appliedRulesCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-appliedrulescollection) | sublist/collection |
| [`advIntercompanyJournalEntry-appliedRulesElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-appliedruleselement) | sublist/element |
| [`advIntercompanyJournalEntry-lineCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-linecollection) | sublist/collection |
| [`advIntercompanyJournalEntry-lineElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-lineelement) | sublist/element |
| [`advIntercompanyJournalEntryCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentrycollection) | collection page |
| [`advIntercompanyJournalEntrySelectOptions`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`advIntercompanyJournalEntry-accountingBookDetailCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-accountingbookdetailcollection) | [`advIntercompanyJournalEntry-accountingBookDetailElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-accountingbookdetailelement) |
| `appliedRules` | [`advIntercompanyJournalEntry-appliedRulesCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-appliedrulescollection) | [`advIntercompanyJournalEntry-appliedRulesElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-appliedruleselement) |
| `line` | [`advIntercompanyJournalEntry-lineCollection`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-linecollection) | [`advIntercompanyJournalEntry-lineElement`](../schemas/advIntercompanyJournalEntry.md#advintercompanyjournalentry-lineelement) |

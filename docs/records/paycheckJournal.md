# paycheckJournal

Browser tag `paycheckJournal` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paycheckJournal`, instance `/paycheckJournal/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paycheckJournal` | `operation--paycheckJournal-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paycheckJournal` | `operation--paycheckJournal-get` | Get list of records. |  | 200 OK → `paycheckJournalCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paycheckJournal` | `operation--paycheckJournal-patch` | Update records. | `paycheckJournalCollection` | 202 Accepted; default → `nsError` |
| POST | `/paycheckJournal` | `operation--paycheckJournal-post` | Insert record. | `paycheckJournal` | 200 OK → `paycheckJournal`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paycheckJournal` | `operation--paycheckJournal-put` | Insert or update records. | `paycheckJournalCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paycheckJournal/{id}` | `operation--paycheckJournal--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paycheckJournal/{id}` | `operation--paycheckJournal--id--get` | Get record. |  | 200 OK → `paycheckJournal`; 202 Accepted; default → `nsError` |
| PATCH | `/paycheckJournal/{id}` | `operation--paycheckJournal--id--patch` | Update record. | `paycheckJournal` | 200 OK → `paycheckJournal`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paycheckJournal/{id}` | `operation--paycheckJournal--id--put` | Insert or update record. | `paycheckJournal` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paycheckJournal-delete` | DELETE `/paycheckJournal` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal-get` | GET `/paycheckJournal` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal-patch` | PATCH `/paycheckJournal` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal-post` | POST `/paycheckJournal` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--paycheckJournal-put` | PUT `/paycheckJournal` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal--id--delete` | DELETE `/paycheckJournal/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal--id--get` | GET `/paycheckJournal/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheckJournal--id--patch` | PATCH `/paycheckJournal/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paycheckJournal--id--put` | PUT `/paycheckJournal/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paycheckJournal schemas](../schemas/paycheckJournal.md).

| Definition | Role |
| --- | --- |
| [`paycheckJournal`](../schemas/paycheckJournal.md#paycheckjournal) | record body |
| [`paycheckJournal-companycontributionCollection`](../schemas/paycheckJournal.md#paycheckjournal-companycontributioncollection) | sublist/collection |
| [`paycheckJournal-companycontributionElement`](../schemas/paycheckJournal.md#paycheckjournal-companycontributionelement) | sublist/element |
| [`paycheckJournal-companytaxCollection`](../schemas/paycheckJournal.md#paycheckjournal-companytaxcollection) | sublist/collection |
| [`paycheckJournal-companytaxElement`](../schemas/paycheckJournal.md#paycheckjournal-companytaxelement) | sublist/element |
| [`paycheckJournal-deductionCollection`](../schemas/paycheckJournal.md#paycheckjournal-deductioncollection) | sublist/collection |
| [`paycheckJournal-deductionElement`](../schemas/paycheckJournal.md#paycheckjournal-deductionelement) | sublist/element |
| [`paycheckJournal-earningCollection`](../schemas/paycheckJournal.md#paycheckjournal-earningcollection) | sublist/collection |
| [`paycheckJournal-earningElement`](../schemas/paycheckJournal.md#paycheckjournal-earningelement) | sublist/element |
| [`paycheckJournal-employeetaxCollection`](../schemas/paycheckJournal.md#paycheckjournal-employeetaxcollection) | sublist/collection |
| [`paycheckJournal-employeetaxElement`](../schemas/paycheckJournal.md#paycheckjournal-employeetaxelement) | sublist/element |
| [`paycheckJournalCollection`](../schemas/paycheckJournal.md#paycheckjournalcollection) | collection page |
| [`paycheckJournalSelectOptions`](../schemas/paycheckJournal.md#paycheckjournalselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `companycontribution` | [`paycheckJournal-companycontributionCollection`](../schemas/paycheckJournal.md#paycheckjournal-companycontributioncollection) | [`paycheckJournal-companycontributionElement`](../schemas/paycheckJournal.md#paycheckjournal-companycontributionelement) |
| `companytax` | [`paycheckJournal-companytaxCollection`](../schemas/paycheckJournal.md#paycheckjournal-companytaxcollection) | [`paycheckJournal-companytaxElement`](../schemas/paycheckJournal.md#paycheckjournal-companytaxelement) |
| `deduction` | [`paycheckJournal-deductionCollection`](../schemas/paycheckJournal.md#paycheckjournal-deductioncollection) | [`paycheckJournal-deductionElement`](../schemas/paycheckJournal.md#paycheckjournal-deductionelement) |
| `earning` | [`paycheckJournal-earningCollection`](../schemas/paycheckJournal.md#paycheckjournal-earningcollection) | [`paycheckJournal-earningElement`](../schemas/paycheckJournal.md#paycheckjournal-earningelement) |
| `employeetax` | [`paycheckJournal-employeetaxCollection`](../schemas/paycheckJournal.md#paycheckjournal-employeetaxcollection) | [`paycheckJournal-employeetaxElement`](../schemas/paycheckJournal.md#paycheckjournal-employeetaxelement) |

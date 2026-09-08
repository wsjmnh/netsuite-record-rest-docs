# periodEndJournal

Browser tag `periodEndJournal` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/periodEndJournal`, instance `/periodEndJournal/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| GET | `/periodEndJournal` | `operation--periodEndJournal-get` | Get list of records. |  | 200 OK → `periodEndJournalCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/periodEndJournal` | `operation--periodEndJournal-patch` | Update records. | `periodEndJournalCollection` | 202 Accepted; default → `nsError` |
| PUT | `/periodEndJournal` | `operation--periodEndJournal-put` | Insert or update records. | `periodEndJournalCollection` | 202 Accepted; default → `nsError` |
| GET | `/periodEndJournal/{id}` | `operation--periodEndJournal--id--get` | Get record. |  | 200 OK → `periodEndJournal`; 202 Accepted; default → `nsError` |
| PATCH | `/periodEndJournal/{id}` | `operation--periodEndJournal--id--patch` | Update record. | `periodEndJournal` | 200 OK → `periodEndJournal`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/periodEndJournal/{id}` | `operation--periodEndJournal--id--put` | Insert or update record. | `periodEndJournal` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--periodEndJournal-get` | GET `/periodEndJournal` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--periodEndJournal-patch` | PATCH `/periodEndJournal` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--periodEndJournal-put` | PUT `/periodEndJournal` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--periodEndJournal--id--get` | GET `/periodEndJournal/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--periodEndJournal--id--patch` | PATCH `/periodEndJournal/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--periodEndJournal--id--put` | PUT `/periodEndJournal/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [periodEndJournal schemas](../schemas/periodEndJournal.md).

| Definition | Role |
| --- | --- |
| [`periodEndJournal`](../schemas/periodEndJournal.md#periodendjournal) | record body |
| [`periodEndJournal-lineCollection`](../schemas/periodEndJournal.md#periodendjournal-linecollection) | sublist/collection |
| [`periodEndJournal-lineElement`](../schemas/periodEndJournal.md#periodendjournal-lineelement) | sublist/element |
| [`periodEndJournalCollection`](../schemas/periodEndJournal.md#periodendjournalcollection) | collection page |
| [`periodEndJournalSelectOptions`](../schemas/periodEndJournal.md#periodendjournalselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `line` | [`periodEndJournal-lineCollection`](../schemas/periodEndJournal.md#periodendjournal-linecollection) | [`periodEndJournal-lineElement`](../schemas/periodEndJournal.md#periodendjournal-lineelement) |

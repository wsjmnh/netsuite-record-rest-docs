# paycheck

Browser tag `paycheck` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/paycheck`, instance `/paycheck/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/paycheck` | `operation--paycheck-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/paycheck` | `operation--paycheck-get` | Get list of records. |  | 200 OK → `paycheckCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/paycheck` | `operation--paycheck-patch` | Update records. | `paycheckCollection` | 202 Accepted; default → `nsError` |
| PUT | `/paycheck` | `operation--paycheck-put` | Insert or update records. | `paycheckCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/paycheck/{id}` | `operation--paycheck--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/paycheck/{id}` | `operation--paycheck--id--get` | Get record. |  | 200 OK → `paycheck`; 202 Accepted; default → `nsError` |
| PATCH | `/paycheck/{id}` | `operation--paycheck--id--patch` | Update record. | `paycheck` | 200 OK → `paycheck`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/paycheck/{id}` | `operation--paycheck--id--put` | Insert or update record. | `paycheck` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--paycheck-delete` | DELETE `/paycheck` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck-get` | GET `/paycheck` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck-patch` | PATCH `/paycheck` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck-put` | PUT `/paycheck` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck--id--delete` | DELETE `/paycheck/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck--id--get` | GET `/paycheck/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--paycheck--id--patch` | PATCH `/paycheck/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--paycheck--id--put` | PUT `/paycheck/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [paycheck schemas](../schemas/paycheck.md).

| Definition | Role |
| --- | --- |
| [`paycheck`](../schemas/paycheck.md#paycheck) | record body |
| [`paycheck-payContribCollection`](../schemas/paycheck.md#paycheck-paycontribcollection) | sublist/collection |
| [`paycheck-payContribElement`](../schemas/paycheck.md#paycheck-paycontribelement) | sublist/element |
| [`paycheck-payDeductCollection`](../schemas/paycheck.md#paycheck-paydeductcollection) | sublist/collection |
| [`paycheck-payDeductElement`](../schemas/paycheck.md#paycheck-paydeductelement) | sublist/element |
| [`paycheck-payDisburseCollection`](../schemas/paycheck.md#paycheck-paydisbursecollection) | sublist/collection |
| [`paycheck-payDisburseElement`](../schemas/paycheck.md#paycheck-paydisburseelement) | sublist/element |
| [`paycheck-payEarnCollection`](../schemas/paycheck.md#paycheck-payearncollection) | sublist/collection |
| [`paycheck-payEarnElement`](../schemas/paycheck.md#paycheck-payearnelement) | sublist/element |
| [`paycheck-payExpCollection`](../schemas/paycheck.md#paycheck-payexpcollection) | sublist/collection |
| [`paycheck-payExpElement`](../schemas/paycheck.md#paycheck-payexpelement) | sublist/element |
| [`paycheck-payPtoCollection`](../schemas/paycheck.md#paycheck-payptocollection) | sublist/collection |
| [`paycheck-payPtoElement`](../schemas/paycheck.md#paycheck-payptoelement) | sublist/element |
| [`paycheck-paySummaryCollection`](../schemas/paycheck.md#paycheck-paysummarycollection) | sublist/collection |
| [`paycheck-paySummaryElement`](../schemas/paycheck.md#paycheck-paysummaryelement) | sublist/element |
| [`paycheck-payTaxCollection`](../schemas/paycheck.md#paycheck-paytaxcollection) | sublist/collection |
| [`paycheck-payTaxElement`](../schemas/paycheck.md#paycheck-paytaxelement) | sublist/element |
| [`paycheck-payTimeCollection`](../schemas/paycheck.md#paycheck-paytimecollection) | sublist/collection |
| [`paycheck-payTimeElement`](../schemas/paycheck.md#paycheck-paytimeelement) | sublist/element |
| [`paycheckCollection`](../schemas/paycheck.md#paycheckcollection) | collection page |
| [`paycheckSelectOptions`](../schemas/paycheck.md#paycheckselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `payContrib` | [`paycheck-payContribCollection`](../schemas/paycheck.md#paycheck-paycontribcollection) | [`paycheck-payContribElement`](../schemas/paycheck.md#paycheck-paycontribelement) |
| `payDeduct` | [`paycheck-payDeductCollection`](../schemas/paycheck.md#paycheck-paydeductcollection) | [`paycheck-payDeductElement`](../schemas/paycheck.md#paycheck-paydeductelement) |
| `payDisburse` | [`paycheck-payDisburseCollection`](../schemas/paycheck.md#paycheck-paydisbursecollection) | [`paycheck-payDisburseElement`](../schemas/paycheck.md#paycheck-paydisburseelement) |
| `payEarn` | [`paycheck-payEarnCollection`](../schemas/paycheck.md#paycheck-payearncollection) | [`paycheck-payEarnElement`](../schemas/paycheck.md#paycheck-payearnelement) |
| `payExp` | [`paycheck-payExpCollection`](../schemas/paycheck.md#paycheck-payexpcollection) | [`paycheck-payExpElement`](../schemas/paycheck.md#paycheck-payexpelement) |
| `payPto` | [`paycheck-payPtoCollection`](../schemas/paycheck.md#paycheck-payptocollection) | [`paycheck-payPtoElement`](../schemas/paycheck.md#paycheck-payptoelement) |
| `paySummary` | [`paycheck-paySummaryCollection`](../schemas/paycheck.md#paycheck-paysummarycollection) | [`paycheck-paySummaryElement`](../schemas/paycheck.md#paycheck-paysummaryelement) |
| `payTax` | [`paycheck-payTaxCollection`](../schemas/paycheck.md#paycheck-paytaxcollection) | [`paycheck-payTaxElement`](../schemas/paycheck.md#paycheck-paytaxelement) |
| `payTime` | [`paycheck-payTimeCollection`](../schemas/paycheck.md#paycheck-paytimecollection) | [`paycheck-payTimeElement`](../schemas/paycheck.md#paycheck-paytimeelement) |

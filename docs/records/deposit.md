# deposit

Browser tag `deposit` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/deposit`, instance `/deposit/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/deposit` | `operation--deposit-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/deposit` | `operation--deposit-get` | Get list of records. |  | 200 OK → `depositCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/deposit` | `operation--deposit-patch` | Update records. | `depositCollection` | 202 Accepted; default → `nsError` |
| POST | `/deposit` | `operation--deposit-post` | Insert record. | `deposit` | 200 OK → `deposit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/deposit` | `operation--deposit-put` | Insert or update records. | `depositCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/deposit/{id}` | `operation--deposit--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/deposit/{id}` | `operation--deposit--id--get` | Get record. |  | 200 OK → `deposit`; 202 Accepted; default → `nsError` |
| PATCH | `/deposit/{id}` | `operation--deposit--id--patch` | Update record. | `deposit` | 200 OK → `deposit`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/deposit/{id}` | `operation--deposit--id--put` | Insert or update record. | `deposit` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--deposit-delete` | DELETE `/deposit` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit-get` | GET `/deposit` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit-patch` | PATCH `/deposit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit-post` | POST `/deposit` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--deposit-put` | PUT `/deposit` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit--id--delete` | DELETE `/deposit/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit--id--get` | GET `/deposit/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--deposit--id--patch` | PATCH `/deposit/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--deposit--id--put` | PUT `/deposit/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [deposit schemas](../schemas/deposit.md).

| Definition | Role |
| --- | --- |
| [`deposit`](../schemas/deposit.md#deposit) | record body |
| [`deposit-accountingBookDetailCollection`](../schemas/deposit.md#deposit-accountingbookdetailcollection) | sublist/collection |
| [`deposit-accountingBookDetailElement`](../schemas/deposit.md#deposit-accountingbookdetailelement) | sublist/element |
| [`deposit-appliedRulesCollection`](../schemas/deposit.md#deposit-appliedrulescollection) | sublist/collection |
| [`deposit-appliedRulesElement`](../schemas/deposit.md#deposit-appliedruleselement) | sublist/element |
| [`deposit-cashbackCollection`](../schemas/deposit.md#deposit-cashbackcollection) | sublist/collection |
| [`deposit-cashbackElement`](../schemas/deposit.md#deposit-cashbackelement) | sublist/element |
| [`deposit-otherCollection`](../schemas/deposit.md#deposit-othercollection) | sublist/collection |
| [`deposit-otherElement`](../schemas/deposit.md#deposit-otherelement) | sublist/element |
| [`deposit-paymentCollection`](../schemas/deposit.md#deposit-paymentcollection) | sublist/collection |
| [`deposit-paymentElement`](../schemas/deposit.md#deposit-paymentelement) | sublist/element |
| [`depositCollection`](../schemas/deposit.md#depositcollection) | collection page |
| [`depositSelectOptions`](../schemas/deposit.md#depositselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`deposit-accountingBookDetailCollection`](../schemas/deposit.md#deposit-accountingbookdetailcollection) | [`deposit-accountingBookDetailElement`](../schemas/deposit.md#deposit-accountingbookdetailelement) |
| `appliedRules` | [`deposit-appliedRulesCollection`](../schemas/deposit.md#deposit-appliedrulescollection) | [`deposit-appliedRulesElement`](../schemas/deposit.md#deposit-appliedruleselement) |
| `cashback` | [`deposit-cashbackCollection`](../schemas/deposit.md#deposit-cashbackcollection) | [`deposit-cashbackElement`](../schemas/deposit.md#deposit-cashbackelement) |
| `other` | [`deposit-otherCollection`](../schemas/deposit.md#deposit-othercollection) | [`deposit-otherElement`](../schemas/deposit.md#deposit-otherelement) |
| `payment` | [`deposit-paymentCollection`](../schemas/deposit.md#deposit-paymentcollection) | [`deposit-paymentElement`](../schemas/deposit.md#deposit-paymentelement) |

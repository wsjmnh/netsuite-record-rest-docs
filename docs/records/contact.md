# contact

Browser tag `contact` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/contact`, instance `/contact/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/contact` | `operation--contact-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/contact` | `operation--contact-get` | Get list of records. |  | 200 OK → `contactCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/contact` | `operation--contact-patch` | Update records. | `contactCollection` | 202 Accepted; default → `nsError` |
| POST | `/contact` | `operation--contact-post` | Insert record. | `contact` | 200 OK → `contact`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/contact` | `operation--contact-put` | Insert or update records. | `contactCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/contact/{id}` | `operation--contact--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/contact/{id}` | `operation--contact--id--get` | Get record. |  | 200 OK → `contact`; 202 Accepted; default → `nsError` |
| PATCH | `/contact/{id}` | `operation--contact--id--patch` | Update record. | `contact` | 200 OK → `contact`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/contact/{id}` | `operation--contact--id--put` | Insert or update record. | `contact` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--contact-delete` | DELETE `/contact` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact-get` | GET `/contact` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact-patch` | PATCH `/contact` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact-post` | POST `/contact` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--contact-put` | PUT `/contact` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact--id--delete` | DELETE `/contact/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact--id--get` | GET `/contact/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--contact--id--patch` | PATCH `/contact/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--contact--id--put` | PUT `/contact/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [contact schemas](../schemas/contact.md).

| Definition | Role |
| --- | --- |
| [`contact`](../schemas/contact.md#contact) | record body |
| [`contact-addressBook-addressBookAddress`](../schemas/contact.md#contact-addressbook-addressbookaddress) | related |
| [`contact-addressBookCollection`](../schemas/contact.md#contact-addressbookcollection) | sublist/collection |
| [`contact-addressBookElement`](../schemas/contact.md#contact-addressbookelement) | sublist/element |
| [`contactCollection`](../schemas/contact.md#contactcollection) | collection page |
| [`contactSelectOptions`](../schemas/contact.md#contactselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`contact-addressBookCollection`](../schemas/contact.md#contact-addressbookcollection) | [`contact-addressBookElement`](../schemas/contact.md#contact-addressbookelement) |

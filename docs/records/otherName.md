# otherName

Browser tag `otherName` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/otherName`, instance `/otherName/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/otherName` | `operation--otherName-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/otherName` | `operation--otherName-get` | Get list of records. |  | 200 OK → `otherNameCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/otherName` | `operation--otherName-patch` | Update records. | `otherNameCollection` | 202 Accepted; default → `nsError` |
| POST | `/otherName` | `operation--otherName-post` | Insert record. | `otherName` | 200 OK → `otherName`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherName` | `operation--otherName-put` | Insert or update records. | `otherNameCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/otherName/{id}` | `operation--otherName--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/otherName/{id}` | `operation--otherName--id--get` | Get record. |  | 200 OK → `otherName`; 202 Accepted; default → `nsError` |
| PATCH | `/otherName/{id}` | `operation--otherName--id--patch` | Update record. | `otherName` | 200 OK → `otherName`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/otherName/{id}` | `operation--otherName--id--put` | Insert or update record. | `otherName` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--otherName-delete` | DELETE `/otherName` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName-get` | GET `/otherName` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName-patch` | PATCH `/otherName` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName-post` | POST `/otherName` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--otherName-put` | PUT `/otherName` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName--id--delete` | DELETE `/otherName/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName--id--get` | GET `/otherName/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--otherName--id--patch` | PATCH `/otherName/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--otherName--id--put` | PUT `/otherName/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [otherName schemas](../schemas/otherName.md).

| Definition | Role |
| --- | --- |
| [`otherName`](../schemas/otherName.md#othername) | record body |
| [`otherName-addressBook-addressBookAddress`](../schemas/otherName.md#othername-addressbook-addressbookaddress) | related |
| [`otherName-addressBookCollection`](../schemas/otherName.md#othername-addressbookcollection) | sublist/collection |
| [`otherName-addressBookElement`](../schemas/otherName.md#othername-addressbookelement) | sublist/element |
| [`otherName-campaignsCollection`](../schemas/otherName.md#othername-campaignscollection) | sublist/collection |
| [`otherName-campaignsElement`](../schemas/otherName.md#othername-campaignselement) | sublist/element |
| [`otherName-subscriptionMessageHistoryCollection`](../schemas/otherName.md#othername-subscriptionmessagehistorycollection) | sublist/collection |
| [`otherName-subscriptionMessageHistoryElement`](../schemas/otherName.md#othername-subscriptionmessagehistoryelement) | sublist/element |
| [`otherName-subscriptionsCollection`](../schemas/otherName.md#othername-subscriptionscollection) | sublist/collection |
| [`otherName-subscriptionsElement`](../schemas/otherName.md#othername-subscriptionselement) | sublist/element |
| [`otherName-taxRegistrationCollection`](../schemas/otherName.md#othername-taxregistrationcollection) | sublist/collection |
| [`otherName-taxRegistrationElement`](../schemas/otherName.md#othername-taxregistrationelement) | sublist/element |
| [`otherNameCollection`](../schemas/otherName.md#othernamecollection) | collection page |
| [`otherNameSelectOptions`](../schemas/otherName.md#othernameselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`otherName-addressBookCollection`](../schemas/otherName.md#othername-addressbookcollection) | [`otherName-addressBookElement`](../schemas/otherName.md#othername-addressbookelement) |
| `campaigns` | [`otherName-campaignsCollection`](../schemas/otherName.md#othername-campaignscollection) | [`otherName-campaignsElement`](../schemas/otherName.md#othername-campaignselement) |
| `subscriptionMessageHistory` | [`otherName-subscriptionMessageHistoryCollection`](../schemas/otherName.md#othername-subscriptionmessagehistorycollection) | [`otherName-subscriptionMessageHistoryElement`](../schemas/otherName.md#othername-subscriptionmessagehistoryelement) |
| `subscriptions` | [`otherName-subscriptionsCollection`](../schemas/otherName.md#othername-subscriptionscollection) | [`otherName-subscriptionsElement`](../schemas/otherName.md#othername-subscriptionselement) |
| `taxRegistration` | [`otherName-taxRegistrationCollection`](../schemas/otherName.md#othername-taxregistrationcollection) | [`otherName-taxRegistrationElement`](../schemas/otherName.md#othername-taxregistrationelement) |

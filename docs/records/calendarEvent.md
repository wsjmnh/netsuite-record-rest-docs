# calendarEvent

Browser tag `calendarEvent` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/calendarEvent`, instance `/calendarEvent/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/calendarEvent` | `operation--calendarEvent-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/calendarEvent` | `operation--calendarEvent-get` | Get list of records. |  | 200 OK → `calendarEventCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/calendarEvent` | `operation--calendarEvent-patch` | Update records. | `calendarEventCollection` | 202 Accepted; default → `nsError` |
| POST | `/calendarEvent` | `operation--calendarEvent-post` | Insert record. | `calendarEvent` | 200 OK → `calendarEvent`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/calendarEvent` | `operation--calendarEvent-put` | Insert or update records. | `calendarEventCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/calendarEvent/{id}` | `operation--calendarEvent--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/calendarEvent/{id}` | `operation--calendarEvent--id--get` | Get record. |  | 200 OK → `calendarEvent`; 202 Accepted; default → `nsError` |
| PATCH | `/calendarEvent/{id}` | `operation--calendarEvent--id--patch` | Update record. | `calendarEvent` | 200 OK → `calendarEvent`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/calendarEvent/{id}` | `operation--calendarEvent--id--put` | Insert or update record. | `calendarEvent` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--calendarEvent-delete` | DELETE `/calendarEvent` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent-get` | GET `/calendarEvent` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent-patch` | PATCH `/calendarEvent` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent-post` | POST `/calendarEvent` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--calendarEvent-put` | PUT `/calendarEvent` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent--id--delete` | DELETE `/calendarEvent/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent--id--get` | GET `/calendarEvent/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--calendarEvent--id--patch` | PATCH `/calendarEvent/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--calendarEvent--id--put` | PUT `/calendarEvent/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [calendarEvent schemas](../schemas/calendarEvent.md).

| Definition | Role |
| --- | --- |
| [`calendarEvent`](../schemas/calendarEvent.md#calendarevent) | record body |
| [`calendarEvent-attendeeCollection`](../schemas/calendarEvent.md#calendarevent-attendeecollection) | sublist/collection |
| [`calendarEvent-attendeeElement`](../schemas/calendarEvent.md#calendarevent-attendeeelement) | sublist/element |
| [`calendarEvent-resourceCollection`](../schemas/calendarEvent.md#calendarevent-resourcecollection) | sublist/collection |
| [`calendarEvent-resourceElement`](../schemas/calendarEvent.md#calendarevent-resourceelement) | sublist/element |
| [`calendarEvent-timeItemCollection`](../schemas/calendarEvent.md#calendarevent-timeitemcollection) | sublist/collection |
| [`calendarEvent-timeItemElement`](../schemas/calendarEvent.md#calendarevent-timeitemelement) | sublist/element |
| [`calendarEventCollection`](../schemas/calendarEvent.md#calendareventcollection) | collection page |
| [`calendarEventSelectOptions`](../schemas/calendarEvent.md#calendareventselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `attendee` | [`calendarEvent-attendeeCollection`](../schemas/calendarEvent.md#calendarevent-attendeecollection) | [`calendarEvent-attendeeElement`](../schemas/calendarEvent.md#calendarevent-attendeeelement) |
| `resource` | [`calendarEvent-resourceCollection`](../schemas/calendarEvent.md#calendarevent-resourcecollection) | [`calendarEvent-resourceElement`](../schemas/calendarEvent.md#calendarevent-resourceelement) |
| `timeItem` | [`calendarEvent-timeItemCollection`](../schemas/calendarEvent.md#calendarevent-timeitemcollection) | [`calendarEvent-timeItemElement`](../schemas/calendarEvent.md#calendarevent-timeitemelement) |

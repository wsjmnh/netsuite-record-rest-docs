# entityGroup

Browser tag `entityGroup` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/entityGroup`, instance `/entityGroup/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/entityGroup` | `operation--entityGroup-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/entityGroup` | `operation--entityGroup-get` | Get list of records. |  | 200 OK → `entityGroupCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/entityGroup` | `operation--entityGroup-patch` | Update records. | `entityGroupCollection` | 202 Accepted; default → `nsError` |
| POST | `/entityGroup` | `operation--entityGroup-post` | Insert record. | `entityGroup` | 200 OK → `entityGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/entityGroup` | `operation--entityGroup-put` | Insert or update records. | `entityGroupCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/entityGroup/{id}` | `operation--entityGroup--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/entityGroup/{id}` | `operation--entityGroup--id--get` | Get record. |  | 200 OK → `entityGroup`; 202 Accepted; default → `nsError` |
| PATCH | `/entityGroup/{id}` | `operation--entityGroup--id--patch` | Update record. | `entityGroup` | 200 OK → `entityGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/entityGroup/{id}` | `operation--entityGroup--id--put` | Insert or update record. | `entityGroup` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/entityGroup/{targetId}/!attach/contact/{attachmentId}` | `operation--entityGroup--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!attach/customer/{attachmentId}` | `operation--entityGroup--targetId---attach-customer--attachmentId--post` | Attach a customer. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!attach/employee/{attachmentId}` | `operation--entityGroup--targetId---attach-employee--attachmentId--post` | Attach a employee. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!attach/job/{attachmentId}` | `operation--entityGroup--targetId---attach-job--attachmentId--post` | Attach a job. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!attach/partner/{attachmentId}` | `operation--entityGroup--targetId---attach-partner--attachmentId--post` | Attach a partner. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!attach/vendor/{attachmentId}` | `operation--entityGroup--targetId---attach-vendor--attachmentId--post` | Attach a vendor. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/contact/{attachmentId}` | `operation--entityGroup--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/customer/{attachmentId}` | `operation--entityGroup--targetId---detach-customer--attachmentId--post` | Detach a customer. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/employee/{attachmentId}` | `operation--entityGroup--targetId---detach-employee--attachmentId--post` | Detach a employee. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/job/{attachmentId}` | `operation--entityGroup--targetId---detach-job--attachmentId--post` | Detach a job. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/partner/{attachmentId}` | `operation--entityGroup--targetId---detach-partner--attachmentId--post` | Detach a partner. |  | 202 Accepted; 204 No Content |
| POST | `/entityGroup/{targetId}/!detach/vendor/{attachmentId}` | `operation--entityGroup--targetId---detach-vendor--attachmentId--post` | Detach a vendor. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--entityGroup-delete` | DELETE `/entityGroup` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup-get` | GET `/entityGroup` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup-patch` | PATCH `/entityGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup-post` | POST `/entityGroup` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--entityGroup-put` | PUT `/entityGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--id--delete` | DELETE `/entityGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--id--get` | GET `/entityGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--id--patch` | PATCH `/entityGroup/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--entityGroup--id--put` | PUT `/entityGroup/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--entityGroup--targetId---attach-contact--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---attach-customer--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/customer/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---attach-employee--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/employee/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---attach-job--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/job/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---attach-partner--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/partner/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---attach-vendor--attachmentId--post` | POST `/entityGroup/{targetId}/!attach/vendor/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-contact--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-customer--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/customer/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-employee--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/employee/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-job--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/job/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-partner--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/partner/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--entityGroup--targetId---detach-vendor--attachmentId--post` | POST `/entityGroup/{targetId}/!detach/vendor/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--entityGroup--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [entityGroup schemas](../schemas/entityGroup.md).

| Definition | Role |
| --- | --- |
| [`entityGroup`](../schemas/entityGroup.md#entitygroup) | record body |
| [`entityGroup-groupMembersCollection`](../schemas/entityGroup.md#entitygroup-groupmemberscollection) | sublist/collection |
| [`entityGroup-groupMembersElement`](../schemas/entityGroup.md#entitygroup-groupmemberselement) | sublist/element |
| [`entityGroup-testCellCollection`](../schemas/entityGroup.md#entitygroup-testcellcollection) | sublist/collection |
| [`entityGroup-testCellElement`](../schemas/entityGroup.md#entitygroup-testcellelement) | sublist/element |
| [`entityGroupCollection`](../schemas/entityGroup.md#entitygroupcollection) | collection page |
| [`entityGroupSelectOptions`](../schemas/entityGroup.md#entitygroupselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `groupMembers` | [`entityGroup-groupMembersCollection`](../schemas/entityGroup.md#entitygroup-groupmemberscollection) | [`entityGroup-groupMembersElement`](../schemas/entityGroup.md#entitygroup-groupmemberselement) |
| `testCell` | [`entityGroup-testCellCollection`](../schemas/entityGroup.md#entitygroup-testcellcollection) | [`entityGroup-testCellElement`](../schemas/entityGroup.md#entitygroup-testcellelement) |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/entityGroup/{targetId}/!attach/contact/{attachmentId}` | `operation--entityGroup--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/entityGroup/{targetId}/!attach/customer/{attachmentId}` | `operation--entityGroup--targetId---attach-customer--attachmentId--post` | Attach a customer. |  |
| POST | `/entityGroup/{targetId}/!attach/employee/{attachmentId}` | `operation--entityGroup--targetId---attach-employee--attachmentId--post` | Attach a employee. |  |
| POST | `/entityGroup/{targetId}/!attach/job/{attachmentId}` | `operation--entityGroup--targetId---attach-job--attachmentId--post` | Attach a job. |  |
| POST | `/entityGroup/{targetId}/!attach/partner/{attachmentId}` | `operation--entityGroup--targetId---attach-partner--attachmentId--post` | Attach a partner. |  |
| POST | `/entityGroup/{targetId}/!attach/vendor/{attachmentId}` | `operation--entityGroup--targetId---attach-vendor--attachmentId--post` | Attach a vendor. |  |
| POST | `/entityGroup/{targetId}/!detach/contact/{attachmentId}` | `operation--entityGroup--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |
| POST | `/entityGroup/{targetId}/!detach/customer/{attachmentId}` | `operation--entityGroup--targetId---detach-customer--attachmentId--post` | Detach a customer. |  |
| POST | `/entityGroup/{targetId}/!detach/employee/{attachmentId}` | `operation--entityGroup--targetId---detach-employee--attachmentId--post` | Detach a employee. |  |
| POST | `/entityGroup/{targetId}/!detach/job/{attachmentId}` | `operation--entityGroup--targetId---detach-job--attachmentId--post` | Detach a job. |  |
| POST | `/entityGroup/{targetId}/!detach/partner/{attachmentId}` | `operation--entityGroup--targetId---detach-partner--attachmentId--post` | Detach a partner. |  |
| POST | `/entityGroup/{targetId}/!detach/vendor/{attachmentId}` | `operation--entityGroup--targetId---detach-vendor--attachmentId--post` | Detach a vendor. |  |

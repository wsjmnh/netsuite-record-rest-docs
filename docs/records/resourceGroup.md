# resourceGroup

Browser tag `resourceGroup` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/resourceGroup`, instance `/resourceGroup/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/resourceGroup` | `operation--resourceGroup-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/resourceGroup` | `operation--resourceGroup-get` | Get list of records. |  | 200 OK → `resourceGroupCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/resourceGroup` | `operation--resourceGroup-patch` | Update records. | `resourceGroupCollection` | 202 Accepted; default → `nsError` |
| POST | `/resourceGroup` | `operation--resourceGroup-post` | Insert record. | `resourceGroup` | 200 OK → `resourceGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/resourceGroup` | `operation--resourceGroup-put` | Insert or update records. | `resourceGroupCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/resourceGroup/{id}` | `operation--resourceGroup--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/resourceGroup/{id}` | `operation--resourceGroup--id--get` | Get record. |  | 200 OK → `resourceGroup`; 202 Accepted; default → `nsError` |
| PATCH | `/resourceGroup/{id}` | `operation--resourceGroup--id--patch` | Update record. | `resourceGroup` | 200 OK → `resourceGroup`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/resourceGroup/{id}` | `operation--resourceGroup--id--put` | Insert or update record. | `resourceGroup` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--resourceGroup-delete` | DELETE `/resourceGroup` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup-get` | GET `/resourceGroup` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup-patch` | PATCH `/resourceGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup-post` | POST `/resourceGroup` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--resourceGroup-put` | PUT `/resourceGroup` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup--id--delete` | DELETE `/resourceGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup--id--get` | GET `/resourceGroup/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--resourceGroup--id--patch` | PATCH `/resourceGroup/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--resourceGroup--id--put` | PUT `/resourceGroup/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [resourceGroup schemas](../schemas/resourceGroup.md).

| Definition | Role |
| --- | --- |
| [`resourceGroup`](../schemas/resourceGroup.md#resourcegroup) | record body |
| [`resourceGroup-resourceGroupMembersCollection`](../schemas/resourceGroup.md#resourcegroup-resourcegroupmemberscollection) | sublist/collection |
| [`resourceGroup-resourceGroupMembersElement`](../schemas/resourceGroup.md#resourcegroup-resourcegroupmemberselement) | sublist/element |
| [`resourceGroupCollection`](../schemas/resourceGroup.md#resourcegroupcollection) | collection page |
| [`resourceGroupSelectOptions`](../schemas/resourceGroup.md#resourcegroupselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `resourceGroupMembers` | [`resourceGroup-resourceGroupMembersCollection`](../schemas/resourceGroup.md#resourcegroup-resourcegroupmemberscollection) | [`resourceGroup-resourceGroupMembersElement`](../schemas/resourceGroup.md#resourcegroup-resourcegroupmemberselement) |

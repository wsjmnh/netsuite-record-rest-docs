# assemblyUnbuild

Browser tag `assemblyUnbuild` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/assemblyUnbuild`, instance `/assemblyUnbuild/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/assemblyUnbuild` | `operation--assemblyUnbuild-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/assemblyUnbuild` | `operation--assemblyUnbuild-get` | Get list of records. |  | 200 OK → `assemblyUnbuildCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyUnbuild` | `operation--assemblyUnbuild-patch` | Update records. | `assemblyUnbuildCollection` | 202 Accepted; default → `nsError` |
| POST | `/assemblyUnbuild` | `operation--assemblyUnbuild-post` | Insert record. | `assemblyUnbuild` | 200 OK → `assemblyUnbuild`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyUnbuild` | `operation--assemblyUnbuild-put` | Insert or update records. | `assemblyUnbuildCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/assemblyUnbuild/{id}` | `operation--assemblyUnbuild--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/assemblyUnbuild/{id}` | `operation--assemblyUnbuild--id--get` | Get record. |  | 200 OK → `assemblyUnbuild`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyUnbuild/{id}` | `operation--assemblyUnbuild--id--patch` | Update record. | `assemblyUnbuild` | 200 OK → `assemblyUnbuild`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyUnbuild/{id}` | `operation--assemblyUnbuild--id--put` | Insert or update record. | `assemblyUnbuild` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--assemblyUnbuild-delete` | DELETE `/assemblyUnbuild` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild-get` | GET `/assemblyUnbuild` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild-patch` | PATCH `/assemblyUnbuild` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild-post` | POST `/assemblyUnbuild` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--assemblyUnbuild-put` | PUT `/assemblyUnbuild` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild--id--delete` | DELETE `/assemblyUnbuild/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild--id--get` | GET `/assemblyUnbuild/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyUnbuild--id--patch` | PATCH `/assemblyUnbuild/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--assemblyUnbuild--id--put` | PUT `/assemblyUnbuild/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [assemblyUnbuild schemas](../schemas/assemblyUnbuild.md).

| Definition | Role |
| --- | --- |
| [`assemblyUnbuild`](../schemas/assemblyUnbuild.md#assemblyunbuild) | record body |
| [`assemblyUnbuild-accountingBookDetailCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-accountingbookdetailcollection) | sublist/collection |
| [`assemblyUnbuild-accountingBookDetailElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-accountingbookdetailelement) | sublist/element |
| [`assemblyUnbuild-component-componentInventoryDetail`](../schemas/assemblyUnbuild.md#assemblyunbuild-component-componentinventorydetail) | related |
| [`assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-component-componentinventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`assemblyUnbuild-component-componentInventoryDetail-inventoryAssignmentElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-component-componentinventorydetail-inventoryassignmentelement) | sublist/element |
| [`assemblyUnbuild-componentCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-componentcollection) | sublist/collection |
| [`assemblyUnbuild-componentElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-componentelement) | sublist/element |
| [`assemblyUnbuild-inventoryDetail`](../schemas/assemblyUnbuild.md#assemblyunbuild-inventorydetail) | related |
| [`assemblyUnbuild-inventoryDetail-inventoryAssignmentCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`assemblyUnbuild-inventoryDetail-inventoryAssignmentElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`assemblyUnbuildCollection`](../schemas/assemblyUnbuild.md#assemblyunbuildcollection) | collection page |
| [`assemblyUnbuildSelectOptions`](../schemas/assemblyUnbuild.md#assemblyunbuildselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`assemblyUnbuild-accountingBookDetailCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-accountingbookdetailcollection) | [`assemblyUnbuild-accountingBookDetailElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-accountingbookdetailelement) |
| `component` | [`assemblyUnbuild-componentCollection`](../schemas/assemblyUnbuild.md#assemblyunbuild-componentcollection) | [`assemblyUnbuild-componentElement`](../schemas/assemblyUnbuild.md#assemblyunbuild-componentelement) |

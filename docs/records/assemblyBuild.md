# assemblyBuild

Browser tag `assemblyBuild` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/assemblyBuild`, instance `/assemblyBuild/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/assemblyBuild` | `operation--assemblyBuild-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/assemblyBuild` | `operation--assemblyBuild-get` | Get list of records. |  | 200 OK → `assemblyBuildCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyBuild` | `operation--assemblyBuild-patch` | Update records. | `assemblyBuildCollection` | 202 Accepted; default → `nsError` |
| POST | `/assemblyBuild` | `operation--assemblyBuild-post` | Insert record. | `assemblyBuild` | 200 OK → `assemblyBuild`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyBuild` | `operation--assemblyBuild-put` | Insert or update records. | `assemblyBuildCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/assemblyBuild/{id}` | `operation--assemblyBuild--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/assemblyBuild/{id}` | `operation--assemblyBuild--id--get` | Get record. |  | 200 OK → `assemblyBuild`; 202 Accepted; default → `nsError` |
| PATCH | `/assemblyBuild/{id}` | `operation--assemblyBuild--id--patch` | Update record. | `assemblyBuild` | 200 OK → `assemblyBuild`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/assemblyBuild/{id}` | `operation--assemblyBuild--id--put` | Insert or update record. | `assemblyBuild` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/assemblyBuild/{id}/!transform/assemblyUnbuild` | `operation--assemblyBuild--id---transform-assemblyUnbuild-post` | Transform to assemblyUnbuild. | `assemblyUnbuild` | 200 OK → `assemblyBuild`; 202 Accepted; 204 No Content → `assemblyUnbuild`; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--assemblyBuild-delete` | DELETE `/assemblyBuild` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild-get` | GET `/assemblyBuild` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild-patch` | PATCH `/assemblyBuild` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild-post` | POST `/assemblyBuild` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--assemblyBuild-put` | PUT `/assemblyBuild` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild--id--delete` | DELETE `/assemblyBuild/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild--id--get` | GET `/assemblyBuild/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--assemblyBuild--id--patch` | PATCH `/assemblyBuild/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--assemblyBuild--id--put` | PUT `/assemblyBuild/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--assemblyBuild--id---transform-assemblyUnbuild-post` | POST `/assemblyBuild/{id}/!transform/assemblyUnbuild` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |

## Schema refs

Definitions owned by this record (property tables): [assemblyBuild schemas](../schemas/assemblyBuild.md).

| Definition | Role |
| --- | --- |
| [`assemblyBuild`](../schemas/assemblyBuild.md#assemblybuild) | record body |
| [`assemblyBuild-accountingBookDetailCollection`](../schemas/assemblyBuild.md#assemblybuild-accountingbookdetailcollection) | sublist/collection |
| [`assemblyBuild-accountingBookDetailElement`](../schemas/assemblyBuild.md#assemblybuild-accountingbookdetailelement) | sublist/element |
| [`assemblyBuild-component-componentInventoryDetail`](../schemas/assemblyBuild.md#assemblybuild-component-componentinventorydetail) | related |
| [`assemblyBuild-component-componentInventoryDetail-inventoryAssignmentCollection`](../schemas/assemblyBuild.md#assemblybuild-component-componentinventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`assemblyBuild-component-componentInventoryDetail-inventoryAssignmentElement`](../schemas/assemblyBuild.md#assemblybuild-component-componentinventorydetail-inventoryassignmentelement) | sublist/element |
| [`assemblyBuild-componentCollection`](../schemas/assemblyBuild.md#assemblybuild-componentcollection) | sublist/collection |
| [`assemblyBuild-componentElement`](../schemas/assemblyBuild.md#assemblybuild-componentelement) | sublist/element |
| [`assemblyBuild-inventoryDetail`](../schemas/assemblyBuild.md#assemblybuild-inventorydetail) | related |
| [`assemblyBuild-inventoryDetail-inventoryAssignmentCollection`](../schemas/assemblyBuild.md#assemblybuild-inventorydetail-inventoryassignmentcollection) | sublist/collection |
| [`assemblyBuild-inventoryDetail-inventoryAssignmentElement`](../schemas/assemblyBuild.md#assemblybuild-inventorydetail-inventoryassignmentelement) | sublist/element |
| [`assemblyBuildCollection`](../schemas/assemblyBuild.md#assemblybuildcollection) | collection page |
| [`assemblyBuildSelectOptions`](../schemas/assemblyBuild.md#assemblybuildselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`assemblyUnbuild`](../schemas/assemblyUnbuild.md#assemblyunbuild)
- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`assemblyBuild-accountingBookDetailCollection`](../schemas/assemblyBuild.md#assemblybuild-accountingbookdetailcollection) | [`assemblyBuild-accountingBookDetailElement`](../schemas/assemblyBuild.md#assemblybuild-accountingbookdetailelement) |
| `component` | [`assemblyBuild-componentCollection`](../schemas/assemblyBuild.md#assemblybuild-componentcollection) | [`assemblyBuild-componentElement`](../schemas/assemblyBuild.md#assemblybuild-componentelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/assemblyBuild/{id}/!transform/assemblyUnbuild` | `operation--assemblyBuild--id---transform-assemblyUnbuild-post` | Transform to assemblyUnbuild. | `assemblyUnbuild` | `assemblyUnbuild` |

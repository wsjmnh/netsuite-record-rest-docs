# siteCategory

Browser tag `siteCategory` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/siteCategory`, instance `/siteCategory/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/siteCategory` | `operation--siteCategory-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/siteCategory` | `operation--siteCategory-get` | Get list of records. |  | 200 OK → `siteCategoryCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/siteCategory` | `operation--siteCategory-patch` | Update records. | `siteCategoryCollection` | 202 Accepted; default → `nsError` |
| POST | `/siteCategory` | `operation--siteCategory-post` | Insert record. | `siteCategory` | 200 OK → `siteCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/siteCategory` | `operation--siteCategory-put` | Insert or update records. | `siteCategoryCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/siteCategory/{id}` | `operation--siteCategory--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/siteCategory/{id}` | `operation--siteCategory--id--get` | Get record. |  | 200 OK → `siteCategory`; 202 Accepted; default → `nsError` |
| PATCH | `/siteCategory/{id}` | `operation--siteCategory--id--patch` | Update record. | `siteCategory` | 200 OK → `siteCategory`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/siteCategory/{id}` | `operation--siteCategory--id--put` | Insert or update record. | `siteCategory` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--siteCategory-delete` | DELETE `/siteCategory` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory-get` | GET `/siteCategory` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory-patch` | PATCH `/siteCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory-post` | POST `/siteCategory` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--siteCategory-put` | PUT `/siteCategory` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory--id--delete` | DELETE `/siteCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory--id--get` | GET `/siteCategory/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--siteCategory--id--patch` | PATCH `/siteCategory/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--siteCategory--id--put` | PUT `/siteCategory/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [siteCategory schemas](../schemas/siteCategory.md).

| Definition | Role |
| --- | --- |
| [`siteCategory`](../schemas/siteCategory.md#sitecategory) | record body |
| [`siteCategory-currentaudienceCollection`](../schemas/siteCategory.md#sitecategory-currentaudiencecollection) | sublist/collection |
| [`siteCategory-currentaudienceElement`](../schemas/siteCategory.md#sitecategory-currentaudienceelement) | sublist/element |
| [`siteCategory-presentationItemCollection`](../schemas/siteCategory.md#sitecategory-presentationitemcollection) | sublist/collection |
| [`siteCategory-presentationItemElement`](../schemas/siteCategory.md#sitecategory-presentationitemelement) | sublist/element |
| [`siteCategory-tag_subs_machineCollection`](../schemas/siteCategory.md#sitecategory-tag_subs_machinecollection) | sublist/collection |
| [`siteCategory-tag_subs_machineElement`](../schemas/siteCategory.md#sitecategory-tag_subs_machineelement) | sublist/element |
| [`siteCategory-translationsCollection`](../schemas/siteCategory.md#sitecategory-translationscollection) | sublist/collection |
| [`siteCategory-translationsElement`](../schemas/siteCategory.md#sitecategory-translationselement) | sublist/element |
| [`siteCategory-urlcomponentaliasesCollection`](../schemas/siteCategory.md#sitecategory-urlcomponentaliasescollection) | sublist/collection |
| [`siteCategory-urlcomponentaliasesElement`](../schemas/siteCategory.md#sitecategory-urlcomponentaliaseselement) | sublist/element |
| [`siteCategoryCollection`](../schemas/siteCategory.md#sitecategorycollection) | collection page |
| [`siteCategorySelectOptions`](../schemas/siteCategory.md#sitecategoryselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `currentaudience` | [`siteCategory-currentaudienceCollection`](../schemas/siteCategory.md#sitecategory-currentaudiencecollection) | [`siteCategory-currentaudienceElement`](../schemas/siteCategory.md#sitecategory-currentaudienceelement) |
| `presentationItem` | [`siteCategory-presentationItemCollection`](../schemas/siteCategory.md#sitecategory-presentationitemcollection) | [`siteCategory-presentationItemElement`](../schemas/siteCategory.md#sitecategory-presentationitemelement) |
| `tag_subs_machine` | [`siteCategory-tag_subs_machineCollection`](../schemas/siteCategory.md#sitecategory-tag_subs_machinecollection) | [`siteCategory-tag_subs_machineElement`](../schemas/siteCategory.md#sitecategory-tag_subs_machineelement) |
| `translations` | [`siteCategory-translationsCollection`](../schemas/siteCategory.md#sitecategory-translationscollection) | [`siteCategory-translationsElement`](../schemas/siteCategory.md#sitecategory-translationselement) |
| `urlcomponentaliases` | [`siteCategory-urlcomponentaliasesCollection`](../schemas/siteCategory.md#sitecategory-urlcomponentaliasescollection) | [`siteCategory-urlcomponentaliasesElement`](../schemas/siteCategory.md#sitecategory-urlcomponentaliaseselement) |

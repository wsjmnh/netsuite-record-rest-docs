# serviceSaleItem

Browser tag `serviceSaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/serviceSaleItem`, instance `/serviceSaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/serviceSaleItem` | `operation--serviceSaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/serviceSaleItem` | `operation--serviceSaleItem-get` | Get list of records. |  | 200 OK → `serviceSaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/serviceSaleItem` | `operation--serviceSaleItem-patch` | Update records. | `serviceSaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/serviceSaleItem` | `operation--serviceSaleItem-post` | Insert record. | `serviceSaleItem` | 200 OK → `serviceSaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serviceSaleItem` | `operation--serviceSaleItem-put` | Insert or update records. | `serviceSaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/serviceSaleItem/{id}` | `operation--serviceSaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/serviceSaleItem/{id}` | `operation--serviceSaleItem--id--get` | Get record. |  | 200 OK → `serviceSaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/serviceSaleItem/{id}` | `operation--serviceSaleItem--id--patch` | Update record. | `serviceSaleItem` | 200 OK → `serviceSaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serviceSaleItem/{id}` | `operation--serviceSaleItem--id--put` | Insert or update record. | `serviceSaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--serviceSaleItem-delete` | DELETE `/serviceSaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem-get` | GET `/serviceSaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem-patch` | PATCH `/serviceSaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem-post` | POST `/serviceSaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--serviceSaleItem-put` | PUT `/serviceSaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem--id--delete` | DELETE `/serviceSaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem--id--get` | GET `/serviceSaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceSaleItem--id--patch` | PATCH `/serviceSaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--serviceSaleItem--id--put` | PUT `/serviceSaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [serviceSaleItem schemas](../schemas/serviceSaleItem.md).

| Definition | Role |
| --- | --- |
| [`serviceSaleItem`](../schemas/serviceSaleItem.md#servicesaleitem) | record body |
| [`serviceSaleItem-accountingBookDetailCollection`](../schemas/serviceSaleItem.md#servicesaleitem-accountingbookdetailcollection) | sublist/collection |
| [`serviceSaleItem-accountingBookDetailElement`](../schemas/serviceSaleItem.md#servicesaleitem-accountingbookdetailelement) | sublist/element |
| [`serviceSaleItem-correlatedItemsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-correlateditemscollection) | sublist/collection |
| [`serviceSaleItem-correlatedItemsElement`](../schemas/serviceSaleItem.md#servicesaleitem-correlateditemselement) | sublist/element |
| [`serviceSaleItem-hierarchyVersionsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-hierarchyversionscollection) | sublist/collection |
| [`serviceSaleItem-hierarchyVersionsElement`](../schemas/serviceSaleItem.md#servicesaleitem-hierarchyversionselement) | sublist/element |
| [`serviceSaleItem-itemTaskTemplatesCollection`](../schemas/serviceSaleItem.md#servicesaleitem-itemtasktemplatescollection) | sublist/collection |
| [`serviceSaleItem-itemTaskTemplatesElement`](../schemas/serviceSaleItem.md#servicesaleitem-itemtasktemplateselement) | sublist/element |
| [`serviceSaleItem-presentationItemCollection`](../schemas/serviceSaleItem.md#servicesaleitem-presentationitemcollection) | sublist/collection |
| [`serviceSaleItem-presentationItemElement`](../schemas/serviceSaleItem.md#servicesaleitem-presentationitemelement) | sublist/element |
| [`serviceSaleItem-price`](../schemas/serviceSaleItem.md#servicesaleitem-price) | related |
| [`serviceSaleItem-priceElement`](../schemas/serviceSaleItem.md#servicesaleitem-priceelement) | sublist/element |
| [`serviceSaleItem-siteCategoryCollection`](../schemas/serviceSaleItem.md#servicesaleitem-sitecategorycollection) | sublist/collection |
| [`serviceSaleItem-siteCategoryElement`](../schemas/serviceSaleItem.md#servicesaleitem-sitecategoryelement) | sublist/element |
| [`serviceSaleItem-translationsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-translationscollection) | sublist/collection |
| [`serviceSaleItem-translationsElement`](../schemas/serviceSaleItem.md#servicesaleitem-translationselement) | sublist/element |
| [`serviceSaleItemCollection`](../schemas/serviceSaleItem.md#servicesaleitemcollection) | collection page |
| [`serviceSaleItemSelectOptions`](../schemas/serviceSaleItem.md#servicesaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`serviceSaleItem-accountingBookDetailCollection`](../schemas/serviceSaleItem.md#servicesaleitem-accountingbookdetailcollection) | [`serviceSaleItem-accountingBookDetailElement`](../schemas/serviceSaleItem.md#servicesaleitem-accountingbookdetailelement) |
| `correlatedItems` | [`serviceSaleItem-correlatedItemsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-correlateditemscollection) | [`serviceSaleItem-correlatedItemsElement`](../schemas/serviceSaleItem.md#servicesaleitem-correlateditemselement) |
| `hierarchyVersions` | [`serviceSaleItem-hierarchyVersionsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-hierarchyversionscollection) | [`serviceSaleItem-hierarchyVersionsElement`](../schemas/serviceSaleItem.md#servicesaleitem-hierarchyversionselement) |
| `itemTaskTemplates` | [`serviceSaleItem-itemTaskTemplatesCollection`](../schemas/serviceSaleItem.md#servicesaleitem-itemtasktemplatescollection) | [`serviceSaleItem-itemTaskTemplatesElement`](../schemas/serviceSaleItem.md#servicesaleitem-itemtasktemplateselement) |
| `presentationItem` | [`serviceSaleItem-presentationItemCollection`](../schemas/serviceSaleItem.md#servicesaleitem-presentationitemcollection) | [`serviceSaleItem-presentationItemElement`](../schemas/serviceSaleItem.md#servicesaleitem-presentationitemelement) |
| `siteCategory` | [`serviceSaleItem-siteCategoryCollection`](../schemas/serviceSaleItem.md#servicesaleitem-sitecategorycollection) | [`serviceSaleItem-siteCategoryElement`](../schemas/serviceSaleItem.md#servicesaleitem-sitecategoryelement) |
| `translations` | [`serviceSaleItem-translationsCollection`](../schemas/serviceSaleItem.md#servicesaleitem-translationscollection) | [`serviceSaleItem-translationsElement`](../schemas/serviceSaleItem.md#servicesaleitem-translationselement) |

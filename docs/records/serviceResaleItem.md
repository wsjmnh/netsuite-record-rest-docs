# serviceResaleItem

Browser tag `serviceResaleItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/serviceResaleItem`, instance `/serviceResaleItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/serviceResaleItem` | `operation--serviceResaleItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/serviceResaleItem` | `operation--serviceResaleItem-get` | Get list of records. |  | 200 OK → `serviceResaleItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/serviceResaleItem` | `operation--serviceResaleItem-patch` | Update records. | `serviceResaleItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/serviceResaleItem` | `operation--serviceResaleItem-post` | Insert record. | `serviceResaleItem` | 200 OK → `serviceResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serviceResaleItem` | `operation--serviceResaleItem-put` | Insert or update records. | `serviceResaleItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/serviceResaleItem/{id}` | `operation--serviceResaleItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/serviceResaleItem/{id}` | `operation--serviceResaleItem--id--get` | Get record. |  | 200 OK → `serviceResaleItem`; 202 Accepted; default → `nsError` |
| PATCH | `/serviceResaleItem/{id}` | `operation--serviceResaleItem--id--patch` | Update record. | `serviceResaleItem` | 200 OK → `serviceResaleItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/serviceResaleItem/{id}` | `operation--serviceResaleItem--id--put` | Insert or update record. | `serviceResaleItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--serviceResaleItem-delete` | DELETE `/serviceResaleItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem-get` | GET `/serviceResaleItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem-patch` | PATCH `/serviceResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem-post` | POST `/serviceResaleItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--serviceResaleItem-put` | PUT `/serviceResaleItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem--id--delete` | DELETE `/serviceResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem--id--get` | GET `/serviceResaleItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--serviceResaleItem--id--patch` | PATCH `/serviceResaleItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--serviceResaleItem--id--put` | PUT `/serviceResaleItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [serviceResaleItem schemas](../schemas/serviceResaleItem.md).

| Definition | Role |
| --- | --- |
| [`serviceResaleItem`](../schemas/serviceResaleItem.md#serviceresaleitem) | record body |
| [`serviceResaleItem-accountingBookDetailCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-accountingbookdetailcollection) | sublist/collection |
| [`serviceResaleItem-accountingBookDetailElement`](../schemas/serviceResaleItem.md#serviceresaleitem-accountingbookdetailelement) | sublist/element |
| [`serviceResaleItem-correlatedItemsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-correlateditemscollection) | sublist/collection |
| [`serviceResaleItem-correlatedItemsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-correlateditemselement) | sublist/element |
| [`serviceResaleItem-hierarchyVersionsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-hierarchyversionscollection) | sublist/collection |
| [`serviceResaleItem-hierarchyVersionsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-hierarchyversionselement) | sublist/element |
| [`serviceResaleItem-itemTaskTemplatesCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-itemtasktemplatescollection) | sublist/collection |
| [`serviceResaleItem-itemTaskTemplatesElement`](../schemas/serviceResaleItem.md#serviceresaleitem-itemtasktemplateselement) | sublist/element |
| [`serviceResaleItem-itemVendor-itemVendorPrice`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendor-itemvendorprice) | related |
| [`serviceResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) | sublist/collection |
| [`serviceResaleItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendor-itemvendorprice-itemvendorpricelineselement) | sublist/element |
| [`serviceResaleItem-itemVendorCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendorcollection) | sublist/collection |
| [`serviceResaleItem-itemVendorElement`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendorelement) | sublist/element |
| [`serviceResaleItem-presentationItemCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-presentationitemcollection) | sublist/collection |
| [`serviceResaleItem-presentationItemElement`](../schemas/serviceResaleItem.md#serviceresaleitem-presentationitemelement) | sublist/element |
| [`serviceResaleItem-price`](../schemas/serviceResaleItem.md#serviceresaleitem-price) | related |
| [`serviceResaleItem-priceElement`](../schemas/serviceResaleItem.md#serviceresaleitem-priceelement) | sublist/element |
| [`serviceResaleItem-siteCategoryCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-sitecategorycollection) | sublist/collection |
| [`serviceResaleItem-siteCategoryElement`](../schemas/serviceResaleItem.md#serviceresaleitem-sitecategoryelement) | sublist/element |
| [`serviceResaleItem-translationsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-translationscollection) | sublist/collection |
| [`serviceResaleItem-translationsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-translationselement) | sublist/element |
| [`serviceResaleItemCollection`](../schemas/serviceResaleItem.md#serviceresaleitemcollection) | collection page |
| [`serviceResaleItemSelectOptions`](../schemas/serviceResaleItem.md#serviceresaleitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accountingBookDetail` | [`serviceResaleItem-accountingBookDetailCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-accountingbookdetailcollection) | [`serviceResaleItem-accountingBookDetailElement`](../schemas/serviceResaleItem.md#serviceresaleitem-accountingbookdetailelement) |
| `correlatedItems` | [`serviceResaleItem-correlatedItemsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-correlateditemscollection) | [`serviceResaleItem-correlatedItemsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-correlateditemselement) |
| `hierarchyVersions` | [`serviceResaleItem-hierarchyVersionsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-hierarchyversionscollection) | [`serviceResaleItem-hierarchyVersionsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-hierarchyversionselement) |
| `itemTaskTemplates` | [`serviceResaleItem-itemTaskTemplatesCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-itemtasktemplatescollection) | [`serviceResaleItem-itemTaskTemplatesElement`](../schemas/serviceResaleItem.md#serviceresaleitem-itemtasktemplateselement) |
| `itemVendor` | [`serviceResaleItem-itemVendorCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendorcollection) | [`serviceResaleItem-itemVendorElement`](../schemas/serviceResaleItem.md#serviceresaleitem-itemvendorelement) |
| `presentationItem` | [`serviceResaleItem-presentationItemCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-presentationitemcollection) | [`serviceResaleItem-presentationItemElement`](../schemas/serviceResaleItem.md#serviceresaleitem-presentationitemelement) |
| `siteCategory` | [`serviceResaleItem-siteCategoryCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-sitecategorycollection) | [`serviceResaleItem-siteCategoryElement`](../schemas/serviceResaleItem.md#serviceresaleitem-sitecategoryelement) |
| `translations` | [`serviceResaleItem-translationsCollection`](../schemas/serviceResaleItem.md#serviceresaleitem-translationscollection) | [`serviceResaleItem-translationsElement`](../schemas/serviceResaleItem.md#serviceresaleitem-translationselement) |

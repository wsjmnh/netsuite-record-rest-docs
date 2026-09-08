# giftCertificateItem

Browser tag `giftCertificateItem` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/giftCertificateItem`, instance `/giftCertificateItem/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/giftCertificateItem` | `operation--giftCertificateItem-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/giftCertificateItem` | `operation--giftCertificateItem-get` | Get list of records. |  | 200 OK → `giftCertificateItemCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/giftCertificateItem` | `operation--giftCertificateItem-patch` | Update records. | `giftCertificateItemCollection` | 202 Accepted; default → `nsError` |
| POST | `/giftCertificateItem` | `operation--giftCertificateItem-post` | Insert record. | `giftCertificateItem` | 200 OK → `giftCertificateItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/giftCertificateItem` | `operation--giftCertificateItem-put` | Insert or update records. | `giftCertificateItemCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/giftCertificateItem/{id}` | `operation--giftCertificateItem--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/giftCertificateItem/{id}` | `operation--giftCertificateItem--id--get` | Get record. |  | 200 OK → `giftCertificateItem`; 202 Accepted; default → `nsError` |
| PATCH | `/giftCertificateItem/{id}` | `operation--giftCertificateItem--id--patch` | Update record. | `giftCertificateItem` | 200 OK → `giftCertificateItem`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/giftCertificateItem/{id}` | `operation--giftCertificateItem--id--put` | Insert or update record. | `giftCertificateItem` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--giftCertificateItem-delete` | DELETE `/giftCertificateItem` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem-get` | GET `/giftCertificateItem` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem-patch` | PATCH `/giftCertificateItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem-post` | POST `/giftCertificateItem` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--giftCertificateItem-put` | PUT `/giftCertificateItem` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem--id--delete` | DELETE `/giftCertificateItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem--id--get` | GET `/giftCertificateItem/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--giftCertificateItem--id--patch` | PATCH `/giftCertificateItem/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--giftCertificateItem--id--put` | PUT `/giftCertificateItem/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [giftCertificateItem schemas](../schemas/giftCertificateItem.md).

| Definition | Role |
| --- | --- |
| [`giftCertificateItem`](../schemas/giftCertificateItem.md#giftcertificateitem) | record body |
| [`giftCertificateItem-authCodesCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-authcodescollection) | sublist/collection |
| [`giftCertificateItem-authCodesElement`](../schemas/giftCertificateItem.md#giftcertificateitem-authcodeselement) | sublist/element |
| [`giftCertificateItem-correlatedItemsCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-correlateditemscollection) | sublist/collection |
| [`giftCertificateItem-correlatedItemsElement`](../schemas/giftCertificateItem.md#giftcertificateitem-correlateditemselement) | sublist/element |
| [`giftCertificateItem-presentationItemCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-presentationitemcollection) | sublist/collection |
| [`giftCertificateItem-presentationItemElement`](../schemas/giftCertificateItem.md#giftcertificateitem-presentationitemelement) | sublist/element |
| [`giftCertificateItem-price`](../schemas/giftCertificateItem.md#giftcertificateitem-price) | related |
| [`giftCertificateItem-priceElement`](../schemas/giftCertificateItem.md#giftcertificateitem-priceelement) | sublist/element |
| [`giftCertificateItem-siteCategoryCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-sitecategorycollection) | sublist/collection |
| [`giftCertificateItem-siteCategoryElement`](../schemas/giftCertificateItem.md#giftcertificateitem-sitecategoryelement) | sublist/element |
| [`giftCertificateItem-translationsCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-translationscollection) | sublist/collection |
| [`giftCertificateItem-translationsElement`](../schemas/giftCertificateItem.md#giftcertificateitem-translationselement) | sublist/element |
| [`giftCertificateItemCollection`](../schemas/giftCertificateItem.md#giftcertificateitemcollection) | collection page |
| [`giftCertificateItemSelectOptions`](../schemas/giftCertificateItem.md#giftcertificateitemselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `authCodes` | [`giftCertificateItem-authCodesCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-authcodescollection) | [`giftCertificateItem-authCodesElement`](../schemas/giftCertificateItem.md#giftcertificateitem-authcodeselement) |
| `correlatedItems` | [`giftCertificateItem-correlatedItemsCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-correlateditemscollection) | [`giftCertificateItem-correlatedItemsElement`](../schemas/giftCertificateItem.md#giftcertificateitem-correlateditemselement) |
| `presentationItem` | [`giftCertificateItem-presentationItemCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-presentationitemcollection) | [`giftCertificateItem-presentationItemElement`](../schemas/giftCertificateItem.md#giftcertificateitem-presentationitemelement) |
| `siteCategory` | [`giftCertificateItem-siteCategoryCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-sitecategorycollection) | [`giftCertificateItem-siteCategoryElement`](../schemas/giftCertificateItem.md#giftcertificateitem-sitecategoryelement) |
| `translations` | [`giftCertificateItem-translationsCollection`](../schemas/giftCertificateItem.md#giftcertificateitem-translationscollection) | [`giftCertificateItem-translationsElement`](../schemas/giftCertificateItem.md#giftcertificateitem-translationselement) |

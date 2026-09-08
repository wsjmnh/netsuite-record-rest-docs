# location

Browser tag `location` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/location`, instance `/location/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/location` | `operation--location-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/location` | `operation--location-get` | Get list of records. |  | 200 OK → `locationCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/location` | `operation--location-patch` | Update records. | `locationCollection` | 202 Accepted; default → `nsError` |
| POST | `/location` | `operation--location-post` | Insert record. | `location` | 200 OK → `location`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/location` | `operation--location-put` | Insert or update records. | `locationCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/location/{id}` | `operation--location--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/location/{id}` | `operation--location--id--get` | Get record. |  | 200 OK → `location`; 202 Accepted; default → `nsError` |
| PATCH | `/location/{id}` | `operation--location--id--patch` | Update record. | `location` | 200 OK → `location`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/location/{id}` | `operation--location--id--put` | Insert or update record. | `location` | 202 Accepted; 204 No Content; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--location-delete` | DELETE `/location` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location-get` | GET `/location` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location-patch` | PATCH `/location` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location-post` | POST `/location` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--location-put` | PUT `/location` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location--id--delete` | DELETE `/location/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location--id--get` | GET `/location/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--location--id--patch` | PATCH `/location/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--location--id--put` | PUT `/location/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |

## Schema refs

Definitions owned by this record (property tables): [location schemas](../schemas/location.md).

| Definition | Role |
| --- | --- |
| [`location`](../schemas/location.md#location) | record body |
| [`location-businessHoursCollection`](../schemas/location.md#location-businesshourscollection) | sublist/collection |
| [`location-businessHoursElement`](../schemas/location.md#location-businesshourselement) | sublist/element |
| [`location-classTranslationCollection`](../schemas/location.md#location-classtranslationcollection) | sublist/collection |
| [`location-classTranslationElement`](../schemas/location.md#location-classtranslationelement) | sublist/element |
| [`location-docNumberingCollection`](../schemas/location.md#location-docnumberingcollection) | sublist/collection |
| [`location-docNumberingElement`](../schemas/location.md#location-docnumberingelement) | sublist/element |
| [`location-excludeLocationRegionsCollection`](../schemas/location.md#location-excludelocationregionscollection) | sublist/collection |
| [`location-excludeLocationRegionsElement`](../schemas/location.md#location-excludelocationregionselement) | sublist/element |
| [`location-includeLocationRegionsCollection`](../schemas/location.md#location-includelocationregionscollection) | sublist/collection |
| [`location-includeLocationRegionsElement`](../schemas/location.md#location-includelocationregionselement) | sublist/element |
| [`location-inventoryBalanceCollection`](../schemas/location.md#location-inventorybalancecollection) | sublist/collection |
| [`location-inventoryBalanceElement`](../schemas/location.md#location-inventorybalanceelement) | sublist/element |
| [`location-mainAddress`](../schemas/location.md#location-mainaddress) | related |
| [`location-returnAddress`](../schemas/location.md#location-returnaddress) | related |
| [`location-tranNumberingCollection`](../schemas/location.md#location-trannumberingcollection) | sublist/collection |
| [`location-tranNumberingElement`](../schemas/location.md#location-trannumberingelement) | sublist/element |
| [`locationCollection`](../schemas/location.md#locationcollection) | collection page |
| [`locationSelectOptions`](../schemas/location.md#locationselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`nsError`](../schemas/ns.md#nserror)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `businessHours` | [`location-businessHoursCollection`](../schemas/location.md#location-businesshourscollection) | [`location-businessHoursElement`](../schemas/location.md#location-businesshourselement) |
| `classTranslation` | [`location-classTranslationCollection`](../schemas/location.md#location-classtranslationcollection) | [`location-classTranslationElement`](../schemas/location.md#location-classtranslationelement) |
| `docNumbering` | [`location-docNumberingCollection`](../schemas/location.md#location-docnumberingcollection) | [`location-docNumberingElement`](../schemas/location.md#location-docnumberingelement) |
| `excludeLocationRegions` | [`location-excludeLocationRegionsCollection`](../schemas/location.md#location-excludelocationregionscollection) | [`location-excludeLocationRegionsElement`](../schemas/location.md#location-excludelocationregionselement) |
| `includeLocationRegions` | [`location-includeLocationRegionsCollection`](../schemas/location.md#location-includelocationregionscollection) | [`location-includeLocationRegionsElement`](../schemas/location.md#location-includelocationregionselement) |
| `inventoryBalance` | [`location-inventoryBalanceCollection`](../schemas/location.md#location-inventorybalancecollection) | [`location-inventoryBalanceElement`](../schemas/location.md#location-inventorybalanceelement) |
| `tranNumbering` | [`location-tranNumberingCollection`](../schemas/location.md#location-trannumberingcollection) | [`location-tranNumberingElement`](../schemas/location.md#location-trannumberingelement) |

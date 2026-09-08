# employee

Browser tag `employee` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/employee`, instance `/employee/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/employee` | `operation--employee-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/employee` | `operation--employee-get` | Get list of records. |  | 200 OK → `employeeCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/employee` | `operation--employee-patch` | Update records. | `employeeCollection` | 202 Accepted; default → `nsError` |
| POST | `/employee` | `operation--employee-post` | Insert record. | `employee` | 200 OK → `employee`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/employee` | `operation--employee-put` | Insert or update records. | `employeeCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/employee/{id}` | `operation--employee--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/employee/{id}` | `operation--employee--id--get` | Get record. |  | 200 OK → `employee`; 202 Accepted; default → `nsError` |
| PATCH | `/employee/{id}` | `operation--employee--id--patch` | Update record. | `employee` | 200 OK → `employee`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/employee/{id}` | `operation--employee--id--put` | Insert or update record. | `employee` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/employee/{id}/!transform/expenseReport` | `operation--employee--id---transform-expenseReport-post` | Transform to expenseReport. | `expenseReport` | 200 OK → `employee`; 202 Accepted; 204 No Content → `expenseReport`; default → `nsError` |
| POST | `/employee/{id}/!transform/timeBill` | `operation--employee--id---transform-timeBill-post` | Transform to timeBill. | `timeBill` | 200 OK → `employee`; 202 Accepted; 204 No Content → `timeBill`; default → `nsError` |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--employee-delete` | DELETE `/employee` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee-get` | GET `/employee` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee-patch` | PATCH `/employee` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee-post` | POST `/employee` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--employee-put` | PUT `/employee` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee--id--delete` | DELETE `/employee/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee--id--get` | GET `/employee/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--employee--id--patch` | PATCH `/employee/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--employee--id--put` | PUT `/employee/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--employee--id---transform-expenseReport-post` | POST `/employee/{id}/!transform/expenseReport` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--employee--id---transform-timeBill-post` | POST `/employee/{id}/!transform/timeBill` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |

## Schema refs

Definitions owned by this record (property tables): [employee schemas](../schemas/employee.md).

| Definition | Role |
| --- | --- |
| [`employee`](../schemas/employee.md#employee) | record body |
| [`employee-accruedTimeCollection`](../schemas/employee.md#employee-accruedtimecollection) | sublist/collection |
| [`employee-accruedTimeElement`](../schemas/employee.md#employee-accruedtimeelement) | sublist/element |
| [`employee-addressBook-addressBookAddress`](../schemas/employee.md#employee-addressbook-addressbookaddress) | related |
| [`employee-addressBookCollection`](../schemas/employee.md#employee-addressbookcollection) | sublist/collection |
| [`employee-addressBookElement`](../schemas/employee.md#employee-addressbookelement) | sublist/element |
| [`employee-campaignsCollection`](../schemas/employee.md#employee-campaignscollection) | sublist/collection |
| [`employee-campaignsElement`](../schemas/employee.md#employee-campaignselement) | sublist/element |
| [`employee-companyContributionCollection`](../schemas/employee.md#employee-companycontributioncollection) | sublist/collection |
| [`employee-companyContributionElement`](../schemas/employee.md#employee-companycontributionelement) | sublist/element |
| [`employee-corporatecardsCollection`](../schemas/employee.md#employee-corporatecardscollection) | sublist/collection |
| [`employee-corporatecardsElement`](../schemas/employee.md#employee-corporatecardselement) | sublist/element |
| [`employee-currencylistCollection`](../schemas/employee.md#employee-currencylistcollection) | sublist/collection |
| [`employee-currencylistElement`](../schemas/employee.md#employee-currencylistelement) | sublist/element |
| [`employee-deductionCollection`](../schemas/employee.md#employee-deductioncollection) | sublist/collection |
| [`employee-deductionElement`](../schemas/employee.md#employee-deductionelement) | sublist/element |
| [`employee-directDepositListCollection`](../schemas/employee.md#employee-directdepositlistcollection) | sublist/collection |
| [`employee-directDepositListElement`](../schemas/employee.md#employee-directdepositlistelement) | sublist/element |
| [`employee-earningCollection`](../schemas/employee.md#employee-earningcollection) | sublist/collection |
| [`employee-earningElement`](../schemas/employee.md#employee-earningelement) | sublist/element |
| [`employee-emergencycontactCollection`](../schemas/employee.md#employee-emergencycontactcollection) | sublist/collection |
| [`employee-emergencycontactElement`](../schemas/employee.md#employee-emergencycontactelement) | sublist/element |
| [`employee-emppermsCollection`](../schemas/employee.md#employee-emppermscollection) | sublist/collection |
| [`employee-emppermsElement`](../schemas/employee.md#employee-emppermselement) | sublist/element |
| [`employee-formw2Collection`](../schemas/employee.md#employee-formw2collection) | sublist/collection |
| [`employee-formw2Element`](../schemas/employee.md#employee-formw2element) | sublist/element |
| [`employee-hcmpositionCollection`](../schemas/employee.md#employee-hcmpositioncollection) | sublist/collection |
| [`employee-hcmpositionElement`](../schemas/employee.md#employee-hcmpositionelement) | sublist/element |
| [`employee-hreducationCollection`](../schemas/employee.md#employee-hreducationcollection) | sublist/collection |
| [`employee-hreducationElement`](../schemas/employee.md#employee-hreducationelement) | sublist/element |
| [`employee-ratesCollection`](../schemas/employee.md#employee-ratescollection) | sublist/collection |
| [`employee-ratesElement`](../schemas/employee.md#employee-rateselement) | sublist/element |
| [`employee-rolesCollection`](../schemas/employee.md#employee-rolescollection) | sublist/collection |
| [`employee-rolesElement`](../schemas/employee.md#employee-roleselement) | sublist/element |
| [`employee-subscriptionMessageHistoryCollection`](../schemas/employee.md#employee-subscriptionmessagehistorycollection) | sublist/collection |
| [`employee-subscriptionMessageHistoryElement`](../schemas/employee.md#employee-subscriptionmessagehistoryelement) | sublist/element |
| [`employee-subscriptionsCollection`](../schemas/employee.md#employee-subscriptionscollection) | sublist/collection |
| [`employee-subscriptionsElement`](../schemas/employee.md#employee-subscriptionselement) | sublist/element |
| [`employeeCollection`](../schemas/employee.md#employeecollection) | collection page |
| [`employeeSelectOptions`](../schemas/employee.md#employeeselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`expenseReport`](../schemas/expenseReport.md#expensereport)
- [`nsError`](../schemas/ns.md#nserror)
- [`timeBill`](../schemas/timeBill.md#timebill)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `accruedTime` | [`employee-accruedTimeCollection`](../schemas/employee.md#employee-accruedtimecollection) | [`employee-accruedTimeElement`](../schemas/employee.md#employee-accruedtimeelement) |
| `addressBook` | [`employee-addressBookCollection`](../schemas/employee.md#employee-addressbookcollection) | [`employee-addressBookElement`](../schemas/employee.md#employee-addressbookelement) |
| `campaigns` | [`employee-campaignsCollection`](../schemas/employee.md#employee-campaignscollection) | [`employee-campaignsElement`](../schemas/employee.md#employee-campaignselement) |
| `companyContribution` | [`employee-companyContributionCollection`](../schemas/employee.md#employee-companycontributioncollection) | [`employee-companyContributionElement`](../schemas/employee.md#employee-companycontributionelement) |
| `corporatecards` | [`employee-corporatecardsCollection`](../schemas/employee.md#employee-corporatecardscollection) | [`employee-corporatecardsElement`](../schemas/employee.md#employee-corporatecardselement) |
| `currencylist` | [`employee-currencylistCollection`](../schemas/employee.md#employee-currencylistcollection) | [`employee-currencylistElement`](../schemas/employee.md#employee-currencylistelement) |
| `deduction` | [`employee-deductionCollection`](../schemas/employee.md#employee-deductioncollection) | [`employee-deductionElement`](../schemas/employee.md#employee-deductionelement) |
| `directDepositList` | [`employee-directDepositListCollection`](../schemas/employee.md#employee-directdepositlistcollection) | [`employee-directDepositListElement`](../schemas/employee.md#employee-directdepositlistelement) |
| `earning` | [`employee-earningCollection`](../schemas/employee.md#employee-earningcollection) | [`employee-earningElement`](../schemas/employee.md#employee-earningelement) |
| `emergencycontact` | [`employee-emergencycontactCollection`](../schemas/employee.md#employee-emergencycontactcollection) | [`employee-emergencycontactElement`](../schemas/employee.md#employee-emergencycontactelement) |
| `empperms` | [`employee-emppermsCollection`](../schemas/employee.md#employee-emppermscollection) | [`employee-emppermsElement`](../schemas/employee.md#employee-emppermselement) |
| `formw2` | [`employee-formw2Collection`](../schemas/employee.md#employee-formw2collection) | [`employee-formw2Element`](../schemas/employee.md#employee-formw2element) |
| `hcmposition` | [`employee-hcmpositionCollection`](../schemas/employee.md#employee-hcmpositioncollection) | [`employee-hcmpositionElement`](../schemas/employee.md#employee-hcmpositionelement) |
| `hreducation` | [`employee-hreducationCollection`](../schemas/employee.md#employee-hreducationcollection) | [`employee-hreducationElement`](../schemas/employee.md#employee-hreducationelement) |
| `rates` | [`employee-ratesCollection`](../schemas/employee.md#employee-ratescollection) | [`employee-ratesElement`](../schemas/employee.md#employee-rateselement) |
| `roles` | [`employee-rolesCollection`](../schemas/employee.md#employee-rolescollection) | [`employee-rolesElement`](../schemas/employee.md#employee-roleselement) |
| `subscriptionMessageHistory` | [`employee-subscriptionMessageHistoryCollection`](../schemas/employee.md#employee-subscriptionmessagehistorycollection) | [`employee-subscriptionMessageHistoryElement`](../schemas/employee.md#employee-subscriptionmessagehistoryelement) |
| `subscriptions` | [`employee-subscriptionsCollection`](../schemas/employee.md#employee-subscriptionscollection) | [`employee-subscriptionsElement`](../schemas/employee.md#employee-subscriptionselement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/employee/{id}/!transform/expenseReport` | `operation--employee--id---transform-expenseReport-post` | Transform to expenseReport. | `expenseReport` | `expenseReport` |
| POST | `/employee/{id}/!transform/timeBill` | `operation--employee--id---transform-timeBill-post` | Transform to timeBill. | `timeBill` | `timeBill` |

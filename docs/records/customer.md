# customer

Browser tag `customer` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/customer`, instance `/customer/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/customer` | `operation--customer-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/customer` | `operation--customer-get` | Get list of records. |  | 200 OK → `customerCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/customer` | `operation--customer-patch` | Update records. | `customerCollection` | 202 Accepted; default → `nsError` |
| POST | `/customer` | `operation--customer-post` | Insert record. | `customer` | 200 OK → `customer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customer` | `operation--customer-put` | Insert or update records. | `customerCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/customer/{id}` | `operation--customer--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/customer/{id}` | `operation--customer--id--get` | Get record. |  | 200 OK → `customer`; 202 Accepted; default → `nsError` |
| PATCH | `/customer/{id}` | `operation--customer--id--patch` | Update record. | `customer` | 200 OK → `customer`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/customer/{id}` | `operation--customer--id--put` | Insert or update record. | `customer` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/customer/{id}/!transform/cashSale` | `operation--customer--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | 200 OK → `customer`; 202 Accepted; 204 No Content → `cashSale`; default → `nsError` |
| POST | `/customer/{id}/!transform/customerPayment` | `operation--customer--id---transform-customerPayment-post` | Transform to customerPayment. | `customerPayment` | 200 OK → `customer`; 202 Accepted; 204 No Content → `customerPayment`; default → `nsError` |
| POST | `/customer/{id}/!transform/estimate` | `operation--customer--id---transform-estimate-post` | Transform to estimate. | `estimate` | 200 OK → `customer`; 202 Accepted; 204 No Content → `estimate`; default → `nsError` |
| POST | `/customer/{id}/!transform/invoice` | `operation--customer--id---transform-invoice-post` | Transform to invoice. | `invoice` | 200 OK → `customer`; 202 Accepted; 204 No Content → `invoice`; default → `nsError` |
| POST | `/customer/{id}/!transform/opportunity` | `operation--customer--id---transform-opportunity-post` | Transform to opportunity. | `opportunity` | 200 OK → `customer`; 202 Accepted; 204 No Content → `opportunity`; default → `nsError` |
| POST | `/customer/{id}/!transform/salesOrder` | `operation--customer--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | 200 OK → `customer`; 202 Accepted; 204 No Content → `salesOrder`; default → `nsError` |
| POST | `/customer/{id}/!transform/vendor` | `operation--customer--id---transform-vendor-post` | Transform to vendor. | `vendor` | 200 OK → `customer`; 202 Accepted; 204 No Content → `vendor`; default → `nsError` |
| POST | `/customer/{targetId}/!attach/contact/{attachmentId}` | `operation--customer--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/customer/{targetId}/!detach/contact/{attachmentId}` | `operation--customer--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--customer-delete` | DELETE `/customer` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer-get` | GET `/customer` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer-patch` | PATCH `/customer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer-post` | POST `/customer` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--customer-put` | PUT `/customer` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer--id--delete` | DELETE `/customer/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer--id--get` | GET `/customer/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer--id--patch` | PATCH `/customer/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customer--id--put` | PUT `/customer/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--customer--id---transform-cashSale-post` | POST `/customer/{id}/!transform/cashSale` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-customerPayment-post` | POST `/customer/{id}/!transform/customerPayment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-estimate-post` | POST `/customer/{id}/!transform/estimate` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-invoice-post` | POST `/customer/{id}/!transform/invoice` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-opportunity-post` | POST `/customer/{id}/!transform/opportunity` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-salesOrder-post` | POST `/customer/{id}/!transform/salesOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--id---transform-vendor-post` | POST `/customer/{id}/!transform/vendor` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--customer--targetId---attach-contact--attachmentId--post` | POST `/customer/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--customer--targetId---detach-contact--attachmentId--post` | POST `/customer/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--customer--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [customer schemas](../schemas/customer.md).

| Definition | Role |
| --- | --- |
| [`customer`](../schemas/customer.md#customer) | record body |
| [`customer-addressBook-addressBookAddress`](../schemas/customer.md#customer-addressbook-addressbookaddress) | related |
| [`customer-addressBookCollection`](../schemas/customer.md#customer-addressbookcollection) | sublist/collection |
| [`customer-addressBookElement`](../schemas/customer.md#customer-addressbookelement) | sublist/element |
| [`customer-campaignsCollection`](../schemas/customer.md#customer-campaignscollection) | sublist/collection |
| [`customer-campaignsElement`](../schemas/customer.md#customer-campaignselement) | sublist/element |
| [`customer-contactRolesCollection`](../schemas/customer.md#customer-contactrolescollection) | sublist/collection |
| [`customer-contactRolesElement`](../schemas/customer.md#customer-contactroleselement) | sublist/element |
| [`customer-currencyListCollection`](../schemas/customer.md#customer-currencylistcollection) | sublist/collection |
| [`customer-currencyListElement`](../schemas/customer.md#customer-currencylistelement) | sublist/element |
| [`customer-groupPricingCollection`](../schemas/customer.md#customer-grouppricingcollection) | sublist/collection |
| [`customer-groupPricingElement`](../schemas/customer.md#customer-grouppricingelement) | sublist/element |
| [`customer-itemPricingCollection`](../schemas/customer.md#customer-itempricingcollection) | sublist/collection |
| [`customer-itemPricingElement`](../schemas/customer.md#customer-itempricingelement) | sublist/element |
| [`customer-partnersCollection`](../schemas/customer.md#customer-partnerscollection) | sublist/collection |
| [`customer-partnersElement`](../schemas/customer.md#customer-partnerselement) | sublist/element |
| [`customer-salesTeamCollection`](../schemas/customer.md#customer-salesteamcollection) | sublist/collection |
| [`customer-salesTeamElement`](../schemas/customer.md#customer-salesteamelement) | sublist/element |
| [`customer-subscriptionMessageHistoryCollection`](../schemas/customer.md#customer-subscriptionmessagehistorycollection) | sublist/collection |
| [`customer-subscriptionMessageHistoryElement`](../schemas/customer.md#customer-subscriptionmessagehistoryelement) | sublist/element |
| [`customer-subscriptionsCollection`](../schemas/customer.md#customer-subscriptionscollection) | sublist/collection |
| [`customer-subscriptionsElement`](../schemas/customer.md#customer-subscriptionselement) | sublist/element |
| [`customer-taxRegistrationCollection`](../schemas/customer.md#customer-taxregistrationcollection) | sublist/collection |
| [`customer-taxRegistrationElement`](../schemas/customer.md#customer-taxregistrationelement) | sublist/element |
| [`customerCollection`](../schemas/customer.md#customercollection) | collection page |
| [`customerSelectOptions`](../schemas/customer.md#customerselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`cashSale`](../schemas/cashSale.md#cashsale)
- [`customerPayment`](../schemas/customerPayment.md#customerpayment)
- [`estimate`](../schemas/estimate.md#estimate)
- [`invoice`](../schemas/invoice.md#invoice)
- [`nsError`](../schemas/ns.md#nserror)
- [`opportunity`](../schemas/opportunity.md#opportunity)
- [`salesOrder`](../schemas/salesOrder.md#salesorder)
- [`vendor`](../schemas/vendor.md#vendor)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`customer-addressBookCollection`](../schemas/customer.md#customer-addressbookcollection) | [`customer-addressBookElement`](../schemas/customer.md#customer-addressbookelement) |
| `campaigns` | [`customer-campaignsCollection`](../schemas/customer.md#customer-campaignscollection) | [`customer-campaignsElement`](../schemas/customer.md#customer-campaignselement) |
| `contactRoles` | [`customer-contactRolesCollection`](../schemas/customer.md#customer-contactrolescollection) | [`customer-contactRolesElement`](../schemas/customer.md#customer-contactroleselement) |
| `currencyList` | [`customer-currencyListCollection`](../schemas/customer.md#customer-currencylistcollection) | [`customer-currencyListElement`](../schemas/customer.md#customer-currencylistelement) |
| `groupPricing` | [`customer-groupPricingCollection`](../schemas/customer.md#customer-grouppricingcollection) | [`customer-groupPricingElement`](../schemas/customer.md#customer-grouppricingelement) |
| `itemPricing` | [`customer-itemPricingCollection`](../schemas/customer.md#customer-itempricingcollection) | [`customer-itemPricingElement`](../schemas/customer.md#customer-itempricingelement) |
| `partners` | [`customer-partnersCollection`](../schemas/customer.md#customer-partnerscollection) | [`customer-partnersElement`](../schemas/customer.md#customer-partnerselement) |
| `salesTeam` | [`customer-salesTeamCollection`](../schemas/customer.md#customer-salesteamcollection) | [`customer-salesTeamElement`](../schemas/customer.md#customer-salesteamelement) |
| `subscriptionMessageHistory` | [`customer-subscriptionMessageHistoryCollection`](../schemas/customer.md#customer-subscriptionmessagehistorycollection) | [`customer-subscriptionMessageHistoryElement`](../schemas/customer.md#customer-subscriptionmessagehistoryelement) |
| `subscriptions` | [`customer-subscriptionsCollection`](../schemas/customer.md#customer-subscriptionscollection) | [`customer-subscriptionsElement`](../schemas/customer.md#customer-subscriptionselement) |
| `taxRegistration` | [`customer-taxRegistrationCollection`](../schemas/customer.md#customer-taxregistrationcollection) | [`customer-taxRegistrationElement`](../schemas/customer.md#customer-taxregistrationelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/customer/{id}/!transform/cashSale` | `operation--customer--id---transform-cashSale-post` | Transform to cashSale. | `cashSale` | `cashSale` |
| POST | `/customer/{id}/!transform/customerPayment` | `operation--customer--id---transform-customerPayment-post` | Transform to customerPayment. | `customerPayment` | `customerPayment` |
| POST | `/customer/{id}/!transform/estimate` | `operation--customer--id---transform-estimate-post` | Transform to estimate. | `estimate` | `estimate` |
| POST | `/customer/{id}/!transform/invoice` | `operation--customer--id---transform-invoice-post` | Transform to invoice. | `invoice` | `invoice` |
| POST | `/customer/{id}/!transform/opportunity` | `operation--customer--id---transform-opportunity-post` | Transform to opportunity. | `opportunity` | `opportunity` |
| POST | `/customer/{id}/!transform/salesOrder` | `operation--customer--id---transform-salesOrder-post` | Transform to salesOrder. | `salesOrder` | `salesOrder` |
| POST | `/customer/{id}/!transform/vendor` | `operation--customer--id---transform-vendor-post` | Transform to vendor. | `vendor` | `vendor` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/customer/{targetId}/!attach/contact/{attachmentId}` | `operation--customer--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/customer/{targetId}/!detach/contact/{attachmentId}` | `operation--customer--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

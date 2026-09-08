# vendor

Browser tag `vendor` (Record REST v1, 2026.1).

Base path: `https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1` — collection `/vendor`, instance `/vendor/{id}`.

Shared query/header conventions: [overview](../overview.md).

## Methods

| Method | Path | Operation ID | Summary | Request body | Responses |
| --- | --- | --- | --- | --- | --- |
| DELETE | `/vendor` | `operation--vendor-delete` | Delete a list of records. |  | 202 Accepted; default → `nsError` |
| GET | `/vendor` | `operation--vendor-get` | Get list of records. |  | 200 OK → `vendorCollection`; 202 Accepted; default → `nsError` |
| PATCH | `/vendor` | `operation--vendor-patch` | Update records. | `vendorCollection` | 202 Accepted; default → `nsError` |
| POST | `/vendor` | `operation--vendor-post` | Insert record. | `vendor` | 200 OK → `vendor`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendor` | `operation--vendor-put` | Insert or update records. | `vendorCollection` | 202 Accepted; default → `nsError` |
| DELETE | `/vendor/{id}` | `operation--vendor--id--delete` | Remove record. |  | 202 Accepted; 204 No Content; default → `nsError` |
| GET | `/vendor/{id}` | `operation--vendor--id--get` | Get record. |  | 200 OK → `vendor`; 202 Accepted; default → `nsError` |
| PATCH | `/vendor/{id}` | `operation--vendor--id--patch` | Update record. | `vendor` | 200 OK → `vendor`; 202 Accepted; 204 No Content; default → `nsError` |
| PUT | `/vendor/{id}` | `operation--vendor--id--put` | Insert or update record. | `vendor` | 202 Accepted; 204 No Content; default → `nsError` |
| POST | `/vendor/{id}/!transform/customer` | `operation--vendor--id---transform-customer-post` | Transform to customer. | `customer` | 200 OK → `vendor`; 202 Accepted; 204 No Content → `customer`; default → `nsError` |
| POST | `/vendor/{id}/!transform/purchaseOrder` | `operation--vendor--id---transform-purchaseOrder-post` | Transform to purchaseOrder. | `purchaseOrder` | 200 OK → `vendor`; 202 Accepted; 204 No Content → `purchaseOrder`; default → `nsError` |
| POST | `/vendor/{id}/!transform/vendorBill` | `operation--vendor--id---transform-vendorBill-post` | Transform to vendorBill. | `vendorBill` | 200 OK → `vendor`; 202 Accepted; 204 No Content → `vendorBill`; default → `nsError` |
| POST | `/vendor/{id}/!transform/vendorPayment` | `operation--vendor--id---transform-vendorPayment-post` | Transform to vendorPayment. | `vendorPayment` | 200 OK → `vendor`; 202 Accepted; 204 No Content → `vendorPayment`; default → `nsError` |
| POST | `/vendor/{targetId}/!attach/contact/{attachmentId}` | `operation--vendor--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` | 202 Accepted; 204 No Content |
| POST | `/vendor/{targetId}/!detach/contact/{attachmentId}` | `operation--vendor--targetId---detach-contact--attachmentId--post` | Detach a contact. |  | 202 Accepted; 204 No Content |

## Parameters

Parameters that appear on this tag’s operations. Shared names are defined in the overview; this table only records presence, location, required, type, format, enum, and default.

| Operation ID | Method / path | Parameters |
| --- | --- | --- |
| `operation--vendor-delete` | DELETE `/vendor` | `ids`; in query; required; string · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor-get` | GET `/vendor` | `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandRecords`; in query; boolean · `ids`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor-patch` | PATCH `/vendor` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor-post` | POST `/vendor` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form`, `application/vnd.oracle.resource+json; type=select-options` · `replace`; in query; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` |
| `operation--vendor-put` | PUT `/vendor` | `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` · `Prefer`; in header; required; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor--id--delete` | DELETE `/vendor/{id}` | `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor--id--get` | GET `/vendor/{id}` | `id`; in path; required; integer (int32); internal identifier · `expandSubResources`; in query; boolean; default `false` · `simpleEnumFormat`; in query; boolean; default `false` · `fields`; in query; string · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor--id--patch` | PATCH `/vendor/{id}` | `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `fields`; in query; string · `q`; in query; string · `limit`; in query; integer (int32); default `1000` · `offset`; in query; integer (int32); default `0` · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=edit-form`, `application/vnd.oracle.resource+json; type=select-options` · `id`; in path; required; integer (int32); internal identifier · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendor--id--put` | PUT `/vendor/{id}` | `id`; in path; required; string; external identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `replaceSelectedFields`; in query; boolean; default `false` |
| `operation--vendor--id---transform-customer-post` | POST `/vendor/{id}/!transform/customer` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendor--id---transform-purchaseOrder-post` | POST `/vendor/{id}/!transform/purchaseOrder` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendor--id---transform-vendorBill-post` | POST `/vendor/{id}/!transform/vendorBill` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendor--id---transform-vendorPayment-post` | POST `/vendor/{id}/!transform/vendorPayment` | `X-NetSuite-PropertyNameValidation`; in header; string; default `Warning`; enum `Error`, `Warning`, `Ignore` · `X-NetSuite-PropertyValueValidation`; in header; string; default `Error`; enum `Error`, `Warning`, `Ignore` · `replace`; in query; string · `id`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string · `expandSubResources`; in query; boolean; default `false` · `expand`; in query; string · `fields`; in query; string · `Accept`; in header; string; enum `application/vnd.oracle.resource+json; type=create-form` |
| `operation--vendor--targetId---attach-contact--attachmentId--post` | POST `/vendor/{targetId}/!attach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |
| `operation--vendor--targetId---detach-contact--attachmentId--post` | POST `/vendor/{targetId}/!detach/contact/{attachmentId}` | `targetId`; in path; required; integer (int32); internal identifier · `attachmentId`; in path; required; integer (int32); internal identifier · `Prefer`; in header; string; enum `respond-async` · `X-NetSuite-Idempotency-Key`; in header; string |

## Inline request bodies

### `operation--vendor--targetId---attach-contact--attachmentId--post`

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `role` |  | object |  |  |  |  |
| `role.externalId` |  | string |  |  |  |  |
| `role.id` |  | integer | int32 |  |  |  |


## Schema refs

Definitions owned by this record (property tables): [vendor schemas](../schemas/vendor.md).

| Definition | Role |
| --- | --- |
| [`vendor`](../schemas/vendor.md#vendor) | record body |
| [`vendor-addressBook-addressBookAddress`](../schemas/vendor.md#vendor-addressbook-addressbookaddress) | related |
| [`vendor-addressBookCollection`](../schemas/vendor.md#vendor-addressbookcollection) | sublist/collection |
| [`vendor-addressBookElement`](../schemas/vendor.md#vendor-addressbookelement) | sublist/element |
| [`vendor-campaignsCollection`](../schemas/vendor.md#vendor-campaignscollection) | sublist/collection |
| [`vendor-campaignsElement`](../schemas/vendor.md#vendor-campaignselement) | sublist/element |
| [`vendor-currencyListCollection`](../schemas/vendor.md#vendor-currencylistcollection) | sublist/collection |
| [`vendor-currencyListElement`](../schemas/vendor.md#vendor-currencylistelement) | sublist/element |
| [`vendor-ratesCollection`](../schemas/vendor.md#vendor-ratescollection) | sublist/collection |
| [`vendor-ratesElement`](../schemas/vendor.md#vendor-rateselement) | sublist/element |
| [`vendor-rolesCollection`](../schemas/vendor.md#vendor-rolescollection) | sublist/collection |
| [`vendor-rolesElement`](../schemas/vendor.md#vendor-roleselement) | sublist/element |
| [`vendor-subscriptionMessageHistoryCollection`](../schemas/vendor.md#vendor-subscriptionmessagehistorycollection) | sublist/collection |
| [`vendor-subscriptionMessageHistoryElement`](../schemas/vendor.md#vendor-subscriptionmessagehistoryelement) | sublist/element |
| [`vendor-subscriptionsCollection`](../schemas/vendor.md#vendor-subscriptionscollection) | sublist/collection |
| [`vendor-subscriptionsElement`](../schemas/vendor.md#vendor-subscriptionselement) | sublist/element |
| [`vendor-taxRegistrationCollection`](../schemas/vendor.md#vendor-taxregistrationcollection) | sublist/collection |
| [`vendor-taxRegistrationElement`](../schemas/vendor.md#vendor-taxregistrationelement) | sublist/element |
| [`vendorCollection`](../schemas/vendor.md#vendorcollection) | collection page |
| [`vendorSelectOptions`](../schemas/vendor.md#vendorselectoptions) | select-options |

Other schemas referenced by this tag’s operations:

- [`customer`](../schemas/customer.md#customer)
- [`nsError`](../schemas/ns.md#nserror)
- [`purchaseOrder`](../schemas/purchaseOrder.md#purchaseorder)
- [`vendorBill`](../schemas/vendorBill.md#vendorbill)
- [`vendorPayment`](../schemas/vendorPayment.md#vendorpayment)

## Sublists

Nested collection properties on the record schema. This dump has no dedicated sublist URLs.

| Property | Collection schema | Element schema |
| --- | --- | --- |
| `addressBook` | [`vendor-addressBookCollection`](../schemas/vendor.md#vendor-addressbookcollection) | [`vendor-addressBookElement`](../schemas/vendor.md#vendor-addressbookelement) |
| `campaigns` | [`vendor-campaignsCollection`](../schemas/vendor.md#vendor-campaignscollection) | [`vendor-campaignsElement`](../schemas/vendor.md#vendor-campaignselement) |
| `currencyList` | [`vendor-currencyListCollection`](../schemas/vendor.md#vendor-currencylistcollection) | [`vendor-currencyListElement`](../schemas/vendor.md#vendor-currencylistelement) |
| `rates` | [`vendor-ratesCollection`](../schemas/vendor.md#vendor-ratescollection) | [`vendor-ratesElement`](../schemas/vendor.md#vendor-rateselement) |
| `roles` | [`vendor-rolesCollection`](../schemas/vendor.md#vendor-rolescollection) | [`vendor-rolesElement`](../schemas/vendor.md#vendor-roleselement) |
| `subscriptionMessageHistory` | [`vendor-subscriptionMessageHistoryCollection`](../schemas/vendor.md#vendor-subscriptionmessagehistorycollection) | [`vendor-subscriptionMessageHistoryElement`](../schemas/vendor.md#vendor-subscriptionmessagehistoryelement) |
| `subscriptions` | [`vendor-subscriptionsCollection`](../schemas/vendor.md#vendor-subscriptionscollection) | [`vendor-subscriptionsElement`](../schemas/vendor.md#vendor-subscriptionselement) |
| `taxRegistration` | [`vendor-taxRegistrationCollection`](../schemas/vendor.md#vendor-taxregistrationcollection) | [`vendor-taxRegistrationElement`](../schemas/vendor.md#vendor-taxregistrationelement) |

## Transforms

| Method | Path | Operation ID | Summary | Target | Request body |
| --- | --- | --- | --- | --- | --- |
| POST | `/vendor/{id}/!transform/customer` | `operation--vendor--id---transform-customer-post` | Transform to customer. | `customer` | `customer` |
| POST | `/vendor/{id}/!transform/purchaseOrder` | `operation--vendor--id---transform-purchaseOrder-post` | Transform to purchaseOrder. | `purchaseOrder` | `purchaseOrder` |
| POST | `/vendor/{id}/!transform/vendorBill` | `operation--vendor--id---transform-vendorBill-post` | Transform to vendorBill. | `vendorBill` | `vendorBill` |
| POST | `/vendor/{id}/!transform/vendorPayment` | `operation--vendor--id---transform-vendorPayment-post` | Transform to vendorPayment. | `vendorPayment` | `vendorPayment` |

## Attach / detach

| Method | Path | Operation ID | Summary | Request body |
| --- | --- | --- | --- | --- |
| POST | `/vendor/{targetId}/!attach/contact/{attachmentId}` | `operation--vendor--targetId---attach-contact--attachmentId--post` | Attach a contact. | inline: `role` |
| POST | `/vendor/{targetId}/!detach/contact/{attachmentId}` | `operation--vendor--targetId---detach-contact--attachmentId--post` | Detach a contact. |  |

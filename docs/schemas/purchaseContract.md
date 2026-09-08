# Schemas: purchaseContract

Property tables for definitions owned by `purchaseContract`.

Record page: [purchaseContract](../records/purchaseContract.md).

## Index

- [purchaseContract](#purchasecontract) — 75 properties
- [purchaseContract-accountingBookDetailCollection](#purchasecontract-accountingbookdetailcollection) — 6 properties
- [purchaseContract-accountingBookDetailElement](#purchasecontract-accountingbookdetailelement) — 7 properties
- [purchaseContract-discountCollection](#purchasecontract-discountcollection) — 6 properties
- [purchaseContract-discountElement](#purchasecontract-discountelement) — 7 properties
- [purchaseContract-item-itemPricing](#purchasecontract-item-itempricing) — 14 properties
- [purchaseContract-item-itemPricing-discountCollection](#purchasecontract-item-itempricing-discountcollection) — 6 properties
- [purchaseContract-item-itemPricing-discountElement](#purchasecontract-item-itempricing-discountelement) — 8 properties
- [purchaseContract-itemCollection](#purchasecontract-itemcollection) — 6 properties
- [purchaseContract-itemElement](#purchasecontract-itemelement) — 48 properties
- [purchaseContractCollection](#purchasecontractcollection) — 6 properties
- [purchaseContractSelectOptions](#purchasecontractselectoptions) — 21 properties

## purchaseContract

Browser definition `purchaseContract`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | purchaseContract-accountingBookDetailCollection |  |  | [`purchaseContract-accountingBookDetailCollection`](#purchasecontract-accountingbookdetailcollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `billedAmount` | Billed Amount | number | double |  |  |  |
| `billingInstructions` | Billing Instructions | string |  |  |  |  |
| `carrier` | Carrier | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consigned` | Consigned | boolean |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `discount` |  | purchaseContract-discountCollection |  |  | [`purchaseContract-discountCollection`](#purchasecontract-discountcollection) |  |
| `discountAmount` | Discount Amount | number | double |  |  |  |
| `discountDate` | Discount Date | string | date |  |  |  |
| `dueDate` | Due Date | string | date |  |  |  |
| `effectivityBasedOn` |  | object |  |  |  |  |
| `effectivityBasedOn.id` | Internal identifier | string |  |  |  | `ORDERDATE`, `RECEIPTDATE` |
| `effectivityBasedOn.refName` | Reference Name | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `incoTerm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `item` |  | purchaseContract-itemCollection |  |  | [`purchaseContract-itemCollection`](#purchasecontract-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `maximumAmount` | Maximum Amount | number | double |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Vendor Message | string |  |  |  |  |
| `minimumAmount` | Minimum Amount | number | double |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `A`, `B`, `R`, `H` |
| `orderStatus.refName` | Reference Name | string |  |  |  |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `packingListInstructions` | Packing List Instructions | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `productLabelingInstructions` | Product Labeling Instructions | string |  |  |  |  |
| `purchaseOrderInstructions` | Purchase Order Instructions | string |  |  |  |  |
| `purchasedAmount` | Purchased Amount | number | double |  |  |  |
| `receivedAmount` | Received Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `R`, `H` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `toBeEmailed` | To Be Emailed | boolean |  |  |  |  |
| `toBeFaxed` | To Be Faxed | boolean |  |  |  |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Transaction Number | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `updateItemVendor` | Update Item Vendor | boolean |  |  |  |  |
| `webSite` |  | string |  |  |  |  |

## purchaseContract-accountingBookDetailCollection

Browser definition `purchaseContract-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseContract-accountingBookDetailElement[] |  |  | [`purchaseContract-accountingBookDetailElement`](#purchasecontract-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseContract-accountingBookDetailElement

Browser definition `purchaseContract-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## purchaseContract-discountCollection

Browser definition `purchaseContract-discountCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseContract-discountElement[] |  |  | [`purchaseContract-discountElement`](#purchasecontract-discountelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseContract-discountElement

Browser definition `purchaseContract-discountElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amountOrdered` | Amount Ordered | number | float |  |  |  |
| `fromAmount` | From Amount | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `percent` | Percent Discount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## purchaseContract-item-itemPricing

Browser definition `purchaseContract-item-itemPricing`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `calculateQuantityDiscounts` |  | object |  |  |  |  |
| `calculateQuantityDiscounts.id` | Internal identifier | string |  |  |  | `OVERALL`, `LINE`, `OVERALLPO` |
| `calculateQuantityDiscounts.refName` | Reference Name | string |  |  |  |  |
| `discount` |  | purchaseContract-item-itemPricing-discountCollection |  |  | [`purchaseContract-item-itemPricing-discountCollection`](#purchasecontract-item-itempricing-discountcollection) |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `inputUsing` |  | object |  |  |  |  |
| `inputUsing.id` | Internal identifier | string |  |  |  | `RATE`, `PERCENT` |
| `inputUsing.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `priceUsing` |  | object |  |  |  |  |
| `priceUsing.id` | Internal identifier | string |  |  |  | `MARGINALRATE`, `RATE`, `LOTRATE` |
| `priceUsing.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `transactionId` |  | purchaseContract |  |  | [`purchaseContract`](#purchasecontract) |  |

## purchaseContract-item-itemPricing-discountCollection

Browser definition `purchaseContract-item-itemPricing-discountCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseContract-item-itemPricing-discountElement[] |  |  | [`purchaseContract-item-itemPricing-discountElement`](#purchasecontract-item-itempricing-discountelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseContract-item-itemPricing-discountElement

Browser definition `purchaseContract-item-itemPricing-discountElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `fromQuantity` | From Quantity | number | float |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `percent` | Percent Discount | number | double |  |  |  |
| `quantityOrdered` | Quantity Ordered | number | float |  |  |  |
| `rate` | Rate or Lot Price | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## purchaseContract-itemCollection

Browser definition `purchaseContract-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseContract-itemElement[] |  |  | [`purchaseContract-itemElement`](#purchasecontract-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseContract-itemElement

Browser definition `purchaseContract-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `expectedReceiptDate` | Expected Receipt Date | string | date |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isConsignmentItem` |  | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemPricing` |  | purchaseContract-item-itemPricing |  |  | [`purchaseContract-item-itemPricing`](#purchasecontract-item-itempricing) |  |
| `itemSubtype` |  | object |  |  |  |  |
| `itemSubtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `itemSubtype.refName` | Reference Name | string |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `licenseCode` | License Code | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `uniqueKey` | Unique Key | integer | int64 |  |  |  |
| `units` | Units | string |  |  |  |  |
| `vendorName` | Vendor Name | string |  |  |  |  |

## purchaseContractCollection

Browser definition `purchaseContractCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | purchaseContract[] |  |  | [`purchaseContract`](#purchasecontract) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseContractSelectOptions

Browser definition `purchaseContractSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `effectivityBasedOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incoTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
